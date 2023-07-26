# Comparing `tmp/gpcal-0.9.4.tar.gz` & `tmp/gpcal-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpcal-0.9.4.tar", last modified: Mon Jul 25 09:33:03 2022, max compression
+gzip compressed data, was "gpcal-0.9.5.tar", last modified: Wed Jul 26 06:42:57 2023, max compression
```

## Comparing `gpcal-0.9.4.tar` & `gpcal-0.9.5.tar`

### file list

```diff
@@ -1,8 +1,22 @@
-drwxr-xr-x   0 jpark      (501) staff       (20)        0 2022-07-25 09:33:03.664065 gpcal-0.9.4/
--rw-r--r--   0 jpark      (501) staff       (20)      699 2022-07-25 09:33:03.664117 gpcal-0.9.4/PKG-INFO
--rw-r--r--   0 jpark      (501) staff       (20)     2372 2022-02-23 01:47:39.000000 gpcal-0.9.4/README.rst
-drwxr-xr-x   0 jpark      (501) staff       (20)        0 2022-07-25 09:33:03.664041 gpcal-0.9.4/gpcal/
--rw-r--r--   0 jpark      (501) staff       (20)       25 2022-02-22 10:38:15.000000 gpcal-0.9.4/gpcal/__init__.py
--rw-r--r--   0 jpark      (501) staff       (20)   216274 2022-07-25 09:23:11.750130 gpcal-0.9.4/gpcal/gpcal.py
--rw-r--r--   0 jpark      (501) staff       (20)       62 2022-02-22 10:38:15.000000 gpcal-0.9.4/setup.cfg
--rw-r--r--   0 jpark      (501) staff       (20)     1651 2022-07-25 09:30:43.337585 gpcal-0.9.4/setup.py
+drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 06:42:57.839108 gpcal-0.9.5/
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)      660 2023-07-26 06:42:57.839108 gpcal-0.9.5/PKG-INFO
+-rw-r--r--   0 jpark     (1000) jpark     (1000)     2991 2023-03-20 13:01:37.000000 gpcal-0.9.5/README.rst
+drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 06:42:57.839108 gpcal-0.9.5/gpcal/
+-rw-r--r--   0 jpark     (1000) jpark     (1000)      245 2023-07-26 06:25:22.000000 gpcal-0.9.5/gpcal/__init__.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)    15099 2023-07-26 06:24:04.000000 gpcal-0.9.5/gpcal/aipsutil.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    66474 2023-07-26 06:24:04.000000 gpcal-0.9.5/gpcal/channelcal.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)     1256 2023-07-26 06:24:04.000000 gpcal-0.9.5/gpcal/cleanhelpers.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)   193550 2023-07-26 06:24:04.000000 gpcal-0.9.5/gpcal/gpcal.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)    27032 2023-07-26 06:24:04.000000 gpcal-0.9.5/gpcal/obshelpers.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    19954 2023-07-26 06:24:04.000000 gpcal-0.9.5/gpcal/plothelpers.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    36468 2023-07-26 06:24:04.000000 gpcal-0.9.5/gpcal/polsolver.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    25263 2023-07-26 06:24:04.000000 gpcal-0.9.5/gpcal/synthetic.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    67744 2023-07-26 06:24:04.000000 gpcal-0.9.5/gpcal/timecal.py
+drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 06:42:57.839108 gpcal-0.9.5/gpcal.egg-info/
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)      660 2023-07-26 06:42:57.000000 gpcal-0.9.5/gpcal.egg-info/PKG-INFO
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)      362 2023-07-26 06:42:57.000000 gpcal-0.9.5/gpcal.egg-info/SOURCES.txt
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)        1 2023-07-26 06:42:57.000000 gpcal-0.9.5/gpcal.egg-info/dependency_links.txt
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)       38 2023-07-26 06:42:57.000000 gpcal-0.9.5/gpcal.egg-info/requires.txt
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)        6 2023-07-26 06:42:57.000000 gpcal-0.9.5/gpcal.egg-info/top_level.txt
+-rw-r--r--   0 jpark     (1000) jpark     (1000)       79 2023-07-26 06:42:57.839108 gpcal-0.9.5/setup.cfg
+-rw-r--r--   0 jpark     (1000) jpark     (1000)     1651 2023-07-26 06:42:51.000000 gpcal-0.9.5/setup.py
```

### Comparing `gpcal-0.9.4/PKG-INFO` & `gpcal-0.9.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: gpcal
-Version: 0.9.4
+Version: 0.9.5
 Summary: A generalized instrumental polarization calibration pipeline for VLBI data
 Home-page: https://github.com/jhparkastro/gpcal
+Download-URL: https://github.com/jhparkastro/gpcal/archive/v1.0.tar.gz
 Author: Jongho Park
 Author-email: jpark@asiaa.sinica.edu.tw
 License: gpl-2.0
-Download-URL: https://github.com/jhparkastro/gpcal/archive/v1.0.tar.gz
-Description: UNKNOWN
 Keywords: VLBI,polarimetry,astronomy,calibration
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `gpcal-0.9.4/README.rst` & `gpcal-0.9.5/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -28,23 +28,25 @@
 .. code-block:: bash
 
     conda install -c free bsddb
 
 
 Tutorial
 -------------
-There are example data and scripts in the "examples" folder. Tutorial slides using one of those data can be found `here <https://docs.google.com/presentation/d/1RRiT4r6H7yeu8ErvdhLN_f8XoMGg0QU3kO_WVWr85W8/edit?usp=sharing>`_.
+There are example data and scripts in the "examples" folder. Tutorial slides using one of those data can be found `here <https://docs.google.com/presentation/d/1TXLHfwVqXNnr7cwLodQQHx2dnVA0WC9iz8e7s1CKgmk/edit?usp=sharing>`_.
 
 Some publications that use GPCAL
 ------------
-If you use GPCAL in your publication, please cite `Park et al. 2020 <>`_.
+If you use GPCAL in your publication, please cite `Park et al. 2021 <https://ui.adsabs.harvard.edu/abs/2021ApJ...906...85P/abstract>`_.
 
 Let us know if you use GPCAL in your publication and we'll list it here!
 
-- GPCAL: a generalized calibration pipeline for instrumental polarization in VLBI data, `Park et al. 2020 <>`_ 
-
+- GPCAL: a generalized calibration pipeline for instrumental polarization in VLBI data, `Park et al. 2021 <https://ui.adsabs.harvard.edu/abs/2021ApJ...906...85P/abstract>`_ 
+- Jet Collimation and Acceleration in the Giant Radio Galaxy NGC 315 `Park et al. 2021 <https://ui.adsabs.harvard.edu/abs/2021ApJ...909...76P/abstract>`_ 
+- First M87 Event Horizon Telescope Results. VII. Polarization of the Ring `EHT Collaboration et al. 2021 <https://ui.adsabs.harvard.edu/abs/2021ApJ...910L..12E/abstract>`_ 
+- A Revised View of the Linear Polarization in the Subparsec Core of M87 at 7 mm `Park et al. 2021 <https://ui.adsabs.harvard.edu/abs/2021ApJ...922..180P/abstract>`_ 
 
 License
 -------
 GPCAL is licensed under GPLv2+. See LICENSE.txt for more details.
```

### Comparing `gpcal-0.9.4/gpcal/gpcal.py` & `gpcal-0.9.5/gpcal/gpcal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 
-
 import sys, os
 from os import path
 
 import pandas as pd
 import numpy as np
+from numpy.linalg import inv
 
 import timeit
 import logging
 import copy
+import glob
 
 from AIPS import AIPS
 from AIPSTask import AIPSTask
 from AIPSData import AIPSUVData, AIPSImage
 from Wizardry.AIPSData import AIPSUVData as WAIPSUVData
 
 from astropy.coordinates import EarthLocation
 import astropy.time as at
-import datetime as dt
 
 from scipy.optimize import curve_fit
 
 import matplotlib
 matplotlib.use('Agg')
 import matplotlib.pyplot as plt
 
+import gpcaltest.aipsutil as au
+import gpcaltest.obshelpers as oh
+import gpcaltest.cleanhelpers as ch
+import gpcaltest.plothelpers as ph
+import gpcaltest.polsolver as ps
+
+import gc
+import psutil
+
+from astropy.io import fits
 
+from multiprocessing import cpu_count, Pool
+
+from IPython import embed
+        
 
 # Default matplotlib parameters
 plt.rc('font', size=21)
-matplotlib.rc('font', family='Times New Roman')
+matplotlib.rc('font', family='Dejavu Sans')
 matplotlib.rc('font', serif='Helvetica Neue')
 plt.rc('text', usetex=True)
 plt.rc('xtick', labelsize=18)
 plt.rc('ytick', labelsize=18)
 plt.rc('axes', titlesize=25)
 plt.rcParams['xtick.top'] = True
 plt.rcParams['ytick.right'] = True
 plt.rcParams['xtick.direction'] = 'in'
 plt.rcParams['ytick.direction'] = 'in'
 plt.subplots_adjust(left = 0.15, bottom = 0.15)
 
 np.set_printoptions(threshold=sys.maxsize)
 
 
-# Suppress AIPS printing on terminal
-def blockPrint():
-    sys.stdout = open(os.devnull, 'w')
-
-# Enable AIPS printing on terminal
-def enablePrint():
-    sys.stdout = sys.__stdout__
-    
 # -----------------------------------------------------------------------------
 # GPCAL Class
 # -----------------------------------------------------------------------------    
 class polcal(object):
     """
     This is a class to calibrate instrumental polarization in VLBI data and produce D-term corrected UVFITS files.
     
@@ -117,104 +123,129 @@
         aipslog (boolean): if it is True, then the output log will contain messages created by AIPS.
         difmaplog (boolean): if it is True, then the output log will contain messages created by Difmap.
         
     Returns:
         gpcal.polcal object
             
     """
-    def __init__(self, aips_userno, direc, dataname, calsour, source, cnum, autoccedt, Dbound = 1.0, Pbound = np.inf, outputname = None, drange = None, \
-                 selfcal=False, solint = None, solmode = None, soltype = None, weightit = None, zblcal = False, zblcalsour = None, zblant = None, \
-                 fixdterm = False, pol_fixdterm = False, fixdr = None, fixdl = None, transferdterm = False, transferdtermant = None, \
-                 selfpol = False, polcalsour = None, selfpoliter = None, ms = None, ps = None, uvbin = None, uvpower = None, dynam = None, \
-                 manualweight = False, weightfactors = None, lpcal = True, remove_weight_outlier_threshold = 10000., \
-                 vplot = True, resplot = True, parplot = True, allplot = False, dplot_IFsep = False, tsep = 2./60., filetype = 'pdf', \
+    def __init__(self, aips_userno, direc, dataname, calsour, source, cnum, autoccedt, \
+                 Dbound = 1.0, Pbound = np.inf, outputname = None, drange = None, multiproc = True, nproc = 2, \
+                 selfcal = False, solint = 10./60., solmode = 'A&P', soltype = 'L1R', weightit = 1, \
+                 zblcal = False, zblcalsour = None, zblant = None, \
+                 fixdterm = False, pol_fixdterm = False, fixdr = None, fixdl = None, \
+                 selfpol = False, polcalsour = None, polcal_unpol = None, selfpoliter = None, ms = None, ps = None, uvbin = None, uvpower = None, shift_x = 0, shift_y = 0, dynam = None, pol_IF_combine = False, \
+                 manualweight = False, weightfactors = None, lpcal = True, remove_weight_outlier_threshold = 10000, \
+                 vplot = False, vplot_title = None, vplot_scanavg = False, vplot_avg_nat = False, resplot = False, parplot = True, allplot = False, dplot_IFsep = False, tsep = 2./60., filetype = 'pdf', \
                  aipslog = True, difmaplog = True):
-        
+
+
         self.aips_userno = aips_userno
         
         self.direc = direc
         
-        # If direc does not finish with a slash, then append it.
-        if(self.direc[-1] != '/'): self.direc = self.direc + '/'
-        
-        # Create a folder named 'gpcal' in the working directory if it does not exist.
-        if(os.path.exists(self.direc+'gpcal') == False):
-            os.system('mkdir ' + self.direc+'gpcal') 
+        self.multiproc = multiproc
+        self.nproc = nproc
         
         self.dataname = dataname
         self.calsour = copy.deepcopy(calsour)
         self.source = copy.deepcopy(source)
         self.cnum = copy.deepcopy(cnum)
+        self.unpolsource = []
+        for i in range(len(self.calsour)):
+            if(self.cnum[i] == 0):
+                self.unpolsource.append(self.calsour[i])
         self.autoccedt = copy.deepcopy(autoccedt)
         
         self.Dbound = Dbound
         self.Pbound = Pbound
         
         self.drange = drange
         
+        self.remove_weight_outlier_threshold = remove_weight_outlier_threshold
+                
+        
+        if(self.dataname[-1] != '.'): self.dataname = self.dataname + '.'
+        
         self.outputname = copy.deepcopy(outputname)
         if(self.outputname == None):
             self.outputname = copy.deepcopy(self.dataname)
         else:
             if(self.outputname[-1] != '.'): self.outputname = self.outputname + '.'
-            
+        
         self.selfcal = selfcal
         self.solint = solint
         self.solmode = solmode
         self.soltype = soltype
         self.weightit = weightit
         
         self.zblcal = zblcal
         self.zblcalsour = copy.deepcopy(zblcalsour)
         self.zblant = copy.deepcopy(zblant)
         
         self.fixdterm = fixdterm
         self.pol_fixdterm = pol_fixdterm
         self.fixdr = copy.deepcopy(fixdr)
         self.fixdl = copy.deepcopy(fixdl)
-        self.transferdterm = transferdterm
-        self.transferdtermant = transferdtermant
         
         self.selfpol = selfpol
         self.polcalsour = copy.deepcopy(polcalsour)
+        self.polcal_unpol = polcal_unpol
+        if(self.polcal_unpol == None) & (self.polcalsour != None): 
+            self.polcal_unpol = [False] * len(self.polcalsour)
         self.selfpoliter = selfpoliter
+        self.pol_IF_combine = pol_IF_combine
+        
         self.ms = ms
         self.ps = ps
         self.uvbin = uvbin
         self.uvpower = uvpower
+        self.shift_x = shift_x
+        self.shift_y = shift_y
         self.dynam = dynam
         
         self.manualweight = manualweight
-        self.weightfactors = copy.deepcopy(weightfactors)
+        self.weightfactors = weightfactors
         self.lpcal = lpcal
         
+        
         self.vplot = vplot
+        self.vplot_title = vplot_title
+        self.vplot_scanavg = vplot_scanavg
+        self.vplot_avg_nat = vplot_avg_nat
         self.resplot = resplot
         self.parplot = parplot
         self.allplot = allplot
         self.tsep = tsep
         self.dplot_IFsep = dplot_IFsep
         self.filetype = filetype
-        self.remove_weight_outlier_threshold = remove_weight_outlier_threshold
-
+        
         self.aipslog = aipslog
         self.difmaplog = difmaplog
         
         self.aipstime = 0.
         self.difmaptime = 0.
         self.gpcaltime = 0.
         
 
         # Create a list of colors
-        self.colors = ['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728', '#9467bd', '#8c564b', '#e377c2', '#7f7f7f', '#bcbd22', '#17becf'] + \
-                       ['blue', 'red', 'orange', 'steelblue', 'green', 'slategrey', 'cyan', 'royalblue', 'purple', 'blueviolet', 'darkcyan', 'darkkhaki', 'magenta', 'navajowhite', 'darkred']
+        self.colors = ['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728', '#7f7f7f', '#9467bd', '#8c564b', '#e377c2', '#bcbd22', '#17becf'] + \
+                       ['blue', 'red', 'orange', 'steelblue', 'green', 'slategrey', 'cyan', 'royalblue', 'purple', 'blueviolet', 'darkcyan', 'darkkhaki', 'magenta', 'navajowhite', 'darkred'] + \
+                           ['#1f77b4', '#ff7f0e', '#2ca02c', '#d62728', '#7f7f7f', '#9467bd', '#8c564b', '#e377c2', '#bcbd22', '#17becf'] + \
+                                          ['blue', 'red', 'orange', 'steelblue', 'green', 'slategrey', 'cyan', 'royalblue', 'purple', 'blueviolet', 'darkcyan', 'darkkhaki', 'magenta', 'navajowhite', 'darkred']
         # Define a list of markers
         self.markerarr = ['o', '^', 's', '<', 'p', '*', 'X', 'P', 'D', 'v', 'd', 'x'] * 5
         
         
+        # If direc does not finish with a slash, then append it.
+        if(self.direc[-1] != '/'): self.direc = self.direc + '/'
+
+        # Create a folder named 'gpcal' in the working directory if it does not exist.
+        if(os.path.exists(self.direc+'gpcal') == False):
+            os.system('mkdir ' + self.direc+'gpcal') 
+            
         # Setup of logging
         if path.exists(direc+'gpcal/'+dataname+'gpcal.log'):
             os.system('rm ' + direc+'gpcal/'+dataname+'gpcal.log')
         self.logfile = direc+'gpcal/'+dataname+'gpcal.log'
         
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(logging.INFO)
@@ -223,687 +254,169 @@
         logformat = logging.Formatter('%(message)s')
         logs.setFormatter(logformat)
         if not len(self.logger.handlers):
             self.logger.addHandler(logs)
             logf = logging.FileHandler(self.logfile)
             self.logger.addHandler(logf)
         
-        # Check the input parameters
-        for i in range(len(self.calsour)):
-            if(self.calsour[i] not in self.source):
-                self.source.append(self.calsour[i])
-                self.logger.info('{:s} is not in SOURCE. It will be added.'.format(self.calsour[i]))
-        
-        for i in range(len(self.polcalsour)):
-            if(self.polcalsour[i] not in self.source):
-                self.source.append(self.polcalsour[i])
-                self.logger.info('{:s} is not in SOURCE. It will be added.'.format(self.polcalsour[i]))
-        
-        if(len(self.calsour) != len(self.cnum)):
-            raise Exception("The number of CALSOUR and CNUM do nat match!")
-        
-        if(len(self.calsour) != len(self.autoccedt)):
-            raise Exception("The number of CALSOUR and AUTOCCEDT do nat match!")
-        
-        for i in range(len(self.calsour)):
-            if not path.exists(self.direc + self.dataname + self.calsour[i] + '.uvf'):
-                raise Exception("{:s} does not exist in {:s}.".format(self.dataname + self.calsour[i] + '.uvf', self.direc))
-            
-            if not path.exists(self.direc + self.dataname + self.calsour[i] + '.fits'):
-                raise Exception("{:s} does not exist in {:s}.".format(self.dataname + self.calsour[i] + '.fits', self.direc))
-            
-            if(self.autoccedt[i] == False):
-                if (cnum[i] != 0) & (not path.exists(self.direc + 'gpcal/' + self.dataname + self.calsour[i] + '.box')):
-                    message = "It was requested to split the total intensity CLEAN components of {:s} into sub-models (autoccedt = False) but there is no '.box' file in '{:s}'.".format(self.calsour[i], self.direc + 'gpcal/')
-                    raise Exception(message)
-        
-        for i in range(len(self.polcalsour)):
-            if not path.exists(self.direc + self.dataname + self.polcalsour[i] + '.uvf'):
-                raise Exception("{:s} does not exist in {:s}.".format(self.dataname + self.polcalsour[i] + '.uvf', self.direc))
-            
-            if not path.exists(self.direc + self.dataname + self.polcalsour[i] + '.fits'):
-                raise Exception("{:s} does not exist in {:s}.".format(self.dataname + self.polcalsour[i] + '.fits', self.direc))
-                                
-            
-    
-    def runfitld(self, outname, outclass, datain):
-        """
-        Run FITLD in AIPS.
-        
-        Args:
-            outname (str): a FITLD parameter outname.
-            outclass (str): a FITLD parameter outclass.
-            datain (str): a FITLD parameter datain.
-        """
-        time1 = timeit.default_timer()
-        fitld = AIPSTask('fitld')
-        fitld.outname = outname
-        fitld.outclass = outclass
-        fitld.datain = datain
-        fitld.outseq = 1
-        blockPrint()
-        fitld.go()    
-        enablePrint()
-        time2 = timeit.default_timer()        
-        self.aipstime += time2 - time1
-    
-    def runlpcal(self, inname, inclass, in2class, cnum):
-        """
-        Run LPCAL in AIPS.
-        
-        Args:
-            inname (str): a FITLD parameter inname.
-            inclass (str): a FITLD parameter inclass.
-            in2class (str): a FITLD parameter in2class.
-            cnum (int): a FITLD parameter in2vers.
-        """
-        time1 = timeit.default_timer()
-        lpcal = AIPSTask('lpcal')
-        lpcal.inname = inname
-        lpcal.inclass = inclass
-        lpcal.indisk = 1
-        lpcal.inseq = 1
-        if(cnum >= 1):
-            lpcal.in2name = inname
-            lpcal.in2class = in2class
-            lpcal.in2disk = 1
-            lpcal.in2vers = 1
-            lpcal.in2seq = 1
-            if(cnum >= 2):
-                lpcal.in2vers = 2
-            lpcal.cmethod = 'DFT'
-            lpcal.cmodel = 'COMP'
-        
-        blockPrint()
-        lpcal.go()
-        enablePrint()
-        time2 = timeit.default_timer()        
-        self.aipstime += time2 - time1
-    
-    
-    def runccedt(self, inname, boxfile, cnum, autoccedt):
-        """
-        Run CCEDT in AIPS.
-        
-        Args:
-            inname (str): a FITLD parameter inname.
-            boxfile (str): a FITLD parameter boxfile.
-            cnum (int): a FITLD parameter cparm(3).
-            autoccedt (boolean): if it is True, then CCEDT splits CLEAN models into sub-models automatically. If it is False, then the boxfile which specifies the locations of sub-model boxes should be provided.
-        """
-        time1 = timeit.default_timer()
-        ccedt = AIPSTask('ccedt')
-        ccedt.inname = inname
-        ccedt.inclass = 'CMAP'
-        ccedt.indisk = 1
-        ccedt.inseq = 1
-        if (cnum == 1):
-            return
-        
-        if autoccedt:
-            ccedt.cparm[3] = cnum
-            ccedt.cparm[4] = 1
-        else:
-            ccedt.nboxes = cnum
-            ccedt.boxfile = boxfile
-            ccedt.nccbox = -cnum
-        
-        blockPrint()
-        ccedt.go()
-        enablePrint()
-        time2 = timeit.default_timer()        
-        self.aipstime += time2 - time1
-    
-    
-    
-    def runprtab(self, data, outprint):
-        """
-        Run PRTAB in AIPS.
-        
-        Args:
-            data (ParselTongue UVData): an input ParselTongue UVData.
-            outprint (str): the output filename of the D-terms in the antenna table.
-        """
-        time1 = timeit.default_timer()
-        prtab = data.table('AN', 1)
-    
-        anname = np.empty([0])
-        DRArr = np.empty([0])
-        DLArr = np.empty([0])
-        
-        for row in prtab:
-            anname = np.append(anname, np.repeat(row.anname.replace(' ', ''), self.ifnum*2))
-            DRArr = np.append(DRArr, row.polcala)
-            DLArr = np.append(DLArr, row.polcalb)
-        
-        
-        df = pd.DataFrame(DRArr.transpose())
-        df['antennas'] = np.array(anname)
-        df['DRArr'] = np.array(DRArr)
-        df['DLArr'] = np.array(DLArr)
-        del df[0]
-        
-        df.to_csv(outprint, sep = "\t")
-        time2 = timeit.default_timer()        
-        self.aipstime += time2 - time1
-        
-    
-    def runtbout(self, inname, inclass, outtext):
-        """
-        Run TBOUT in AIPS.
-        
-        Args:
-            inname (str): a TBOUT parameter inname.
-            inclass (str): a TBOUT parameter inclass.
-            outtext (str): the filename of the antenna table output.
-        """
-        time1 = timeit.default_timer()
-        tbout = AIPSTask('tbout')
-        tbout.inname = inname
-        tbout.inclass = inclass
-        tbout.inseq = 1
-        tbout.indisk = 1
-        tbout.inext = 'AN'
-        tbout.invers = 1
-        tbout.outtext = outtext
-        tbout.docrt = -3
-        blockPrint()
-        tbout.go()
-        enablePrint()
-    
-        time2 = timeit.default_timer()        
-        self.aipstime += time2 - time1
-        
-    
-    
-    def runcalib(self, inname, inclass, outclass, solint, soltype, solmode, weightit):
-        """
-        Run CALIB in AIPS.
-        
-        Args:
-            inname (str): a CALIB parameter inname.
-            inclass (str): a CALIB parameter inclass.
-            outclass (str): a CALIB parameter outclass.
-            solint (float): a CALIB parameter solint.
-            soltype (str): a CALIB parameter soltype.
-            solmode (str): a CALIB parameter solmode.
-            weightit (int): a CALIB parameter weightit.
-        """
-        time1 = timeit.default_timer()
-        calib = AIPSTask('calib')
-        calib.inname = inname
-        calib.inclass = inclass
-        calib.indisk = 1
-        calib.inseq = 1
-        calib.in2name = inname
-        calib.in2class = 'CMAP'
-        calib.in2disk = 1
-        calib.in2seq = 1
-        calib.invers = 1
-        calib.outclass = outclass
-        calib.cmethod = 'DFT'
-        calib.cmodel = 'COMP'
-        calib.solint = solint
-        calib.refant = 0
-        if(solmode == 'a&p'):
-            calib.aparm[1] = 3
-        else:
-            calib.aparm[1] = 3
-        calib.aparm[7] = 0.1
-        calib.weightit = weightit
-        calib.soltype = soltype
-        calib.solmode = solmode
-        
-        blockPrint()
-        calib.go()
-        enablePrint()
-        time2 = timeit.default_timer()        
-        self.aipstime += time2 - time1
-        
-        
-    def runsplit(self, inname, inclass):
-        """
-        Run SPLIT in AIPS to apply the D-terms.
-        
-        Args:
-            inname (str): a SPLIT parameter inname.
-            inclass (str): a SPLIT parameter inclass.
-        """
-        time1 = timeit.default_timer()        
-        split = AIPSTask('split')
-        split.inname = inname
-        split.inclass = inclass
-        split.indisk = 1
-        split.dopol = 3
-        blockPrint()
-        split.go()
-        enablePrint()
-        time2 = timeit.default_timer()        
-        self.aipstime += time2 - time1
-    
-    
-    def runmulti(self, inname, inclass):
-        """
-        Run MULTI in AIPS for the EVPA calibration.
-        
-        Args:
-            inname (str): a MULTI parameter inname.
-            inclass (str): a MULTI parameter inclass.
-        """
-        multi = AIPSTask('multi')
-        multi.inname = inname
-        multi.inclass = inclass
-        multi.indisk = 1
-        multi.inseq = 1
-        multi.outname = inname
-        blockPrint()
-        multi.go()
-        enablePrint()
-    
-    
-    def runclcor(self, inname, clcorprm):
-        """
-        Run CLCOR in AIPS for the EVPA calibration.
-        
-        Args:
-            inname (str): a CLCOR parameter inname.
-            clcorprm (list): the list of floats of the amounts of the RCP and LCP phase offset at the reference antenna.
-        """
-        clcor = AIPSTask('clcor')
-        clcor.inname = inname
-        clcor.inclass = 'MULTI'
-        clcor.indisk = 1
-        clcor.inseq = 1
-        clcor.stokes = 'L'
-        clcor.opcode = 'PHAS'
-        for i in range(len(clcorprm)):
-            clcor.clcorprm[i+1] = float(clcorprm[i])
-        blockPrint()
-        clcor.go()
-        enablePrint()
-
-
-    
-    def runsplitpang(self, inname):
-        """
-        Run SPLIT in AIPS for the EVPA calibration.
-        
-        Args:
-            inname (str): a SPLIT parameter inname.
-        """        
-        time1 = timeit.default_timer()        
-        split = AIPSTask('split')
-        split.inname = inname
-        split.inclass = 'MULTI'
-        split.indisk = 1
-        split.inseq = 1
-        split.dopol = -1
-        split.outclass = 'PANG'
-        split.docalib = 1
-        split.gainuse = 2
-        blockPrint()
-        split.go()
-        enablePrint()
-        time2 = timeit.default_timer()        
-        self.aipstime += time2 - time1        
-    
-    
-    
-    def runuvsub(self, inname, inclass, in2class, invers, outseq):
-        """
-        Run UVSUB in AIPS.
-        
-        Args:
-            inname (str): a UVSUB parameter inname.
-            inclass (str): a UVSUB parameter inclass.
-            in2class (str): a UVSUB parameter in2class.
-            invers (int): a UVSUB parameter invers.
-            outseq (int): a UVSUB parameter outseq.
-        """
-        time1 = timeit.default_timer()        
-        uvsub = AIPSTask('uvsub')
-        uvsub.inname = inname
-        uvsub.inclass = inclass
-        uvsub.indisk = 1
-        uvsub.inseq = 1
-        uvsub.in2name = inname
-        uvsub.in2class = in2class
-        uvsub.in2disk = 1
-        uvsub.in2seq = 1
-        uvsub.outseq = outseq
-        uvsub.cmethod = 'DFT'
-        uvsub.cmodel = 'COMP'
-        uvsub.opcode = 'MODL'
-        uvsub.invers = invers
-        
-        blockPrint()
-        uvsub.go()
-        enablePrint()
-        time2 = timeit.default_timer()        
-        self.aipstime += time2 - time1
-    
-    
-    
-    def runfittp(self, inname, inclass, dataout):
-        """
-        Run FITTP in AIPS.
-        
-        Args:
-            inname (str): a FITTP parameter inname.
-            inclass (str): a FITTP parameter inclass.
-            dataout (str): the FITTP output filename.
-        """
-        time1 = timeit.default_timer()        
-        fittp = AIPSTask('fittp')
-        fittp.inname = inname
-        fittp.inclass = inclass
-        fittp.indisk = 1
-        fittp.dataout = dataout
-        blockPrint()
-        fittp.go()
-        enablePrint()
-        time2 = timeit.default_timer()        
-        self.aipstime += time2 - time1
-    
-    
-    
-    def runtacop(self, inname, inclass, outname, outclass):
-        """
-        Run TACOP in AIPS.
-        
-        Args:
-            inname (str): a TACOP parameter inname.
-            inclass (str): a TACOP parameter inclass.
-            outname (str): a TACOP parameter outname.
-            outclass (str): a TACOP parameter outclass.
-        """
-        time1 = timeit.default_timer()
-        tacop = AIPSTask('tacop')
-        tacop.inname = inname
-        tacop.inclass = inclass
-        tacop.inseq = 1
-        tacop.indisk = 1
-        tacop.inext = 'AN'
-        tacop.invers = 1
-        tacop.outname = outname
-        tacop.outclass = outclass
-        blockPrint()
-        tacop.go()
-        enablePrint()
-        time2 = timeit.default_timer()        
-        self.aipstime += time2 - time1
-        
-    
-    def uvprt(self, data, select):
-        """
-        Extract UV data from ParselTongue UVData.
-        
-        Args:
-            data (ParselTongue UVData): an input ParselTongue UVData.
-            select (str): type of the data that will be extracted.
-        
-        Returns:
-            list(s) of the selected UV data.
-        """        
-        dumu, dumv, ifarr, time, ant1, ant2, rrreal, rrimag, rrweight, llreal, llimag, llweight, rlreal, rlimag, rlweight, lrreal, lrimag, lrweight = \
-            [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], []
-        
-        for ifn in range(self.ifnum):
-            for visibility in data:
-                if((visibility.visibility[ifn,0,0,2] <= 0) | (visibility.visibility[ifn,0,1,2] <= 0) | (visibility.visibility[ifn,0,2,2] <= 0) | (visibility.visibility[ifn,0,3,2] <= 0)): continue
-		#if((visibility.visibility[ifn,0,0,2] == 0) | (visibility.visibility[ifn,0,1,2] == 0) | (visibility.visibility[ifn,0,2,2] == 0) | (visibility.visibility[ifn,0,3,2] == 0)): continue
-                dumu.append(visibility.uvw[0])
-                dumv.append(visibility.uvw[1])
-                ifarr.append(ifn+1)
-                time.append(visibility.time)
-                rrreal.append(visibility.visibility[ifn,0,0,0])
-                rrimag.append(visibility.visibility[ifn,0,0,1])
-                rrweight.append(visibility.visibility[ifn,0,0,2])
-                llreal.append(visibility.visibility[ifn,0,1,0])
-                llimag.append(visibility.visibility[ifn,0,1,1])
-                llweight.append(visibility.visibility[ifn,0,1,2])
-                rlreal.append(visibility.visibility[ifn,0,2,0])
-                rlimag.append(visibility.visibility[ifn,0,2,1])
-                rlweight.append(visibility.visibility[ifn,0,2,2])
-                lrreal.append(visibility.visibility[ifn,0,3,0])
-                lrimag.append(visibility.visibility[ifn,0,3,1])
-                lrweight.append(visibility.visibility[ifn,0,3,2])
-                ant1.append(visibility.baseline[0])
-                ant2.append(visibility.baseline[1])
-            
-        if(np.sum(rrreal) == 0.):
-            return
-
-        
-        selectarr = ["u", "v", "ifarr", "time", "ant1", "ant2", "rrreal", "rrimag", "rrweight", "llreal", "llimag", "llweight", "rlreal", "rlimag", "rlweight", "lrreal", "lrimag", "lrweight"]
-        package = [dumu, dumv, ifarr, time, ant1, ant2, rrreal, rrimag, rrweight, llreal, llimag, llweight, rlreal, rlimag, rlweight, lrreal, lrimag, lrweight]
-        
-        for i in range(len(selectarr)):
-            if(select == selectarr[i]): return package[i]
-        
-        if(select == "all"): return dumu, dumv, ifarr, time, ant1, ant2, rrreal, rrimag, rrweight, llreal, llimag, llweight, rlreal, rlimag, rlweight, lrreal, lrimag, lrweight
-        
-
-    
-    def pol_model_uvprt(self, data, ifn, select):
-        """
-        Extract UV data from ParselTongue UVData for instrumental polarization self-calibration.
-        
-        Args:
-            data (ParselTongue UVData): an input ParselTongue UVData.
-            ifn (int): selected IF number
-            select (str): type of the data that will be extracted.
-        
-        Returns:
-            list(s) of the selected UV data.
-        """        
-        real, imag = [], []
-
-        for visibility in data:
-            if((visibility.visibility[ifn,0,0,2] <= 0) | (visibility.visibility[ifn,0,1,2] <= 0) | (visibility.visibility[ifn,0,2,2] <= 0) | (visibility.visibility[ifn,0,3,2] <= 0)): continue
-            real.append(visibility.visibility[ifn,0,0,0])
-            imag.append(visibility.visibility[ifn,0,0,1])
-            
-        if(np.sum(real) == 0.):
-            return
                 
-        selectarr = ["real", "imag"]
-        package = [real, imag]
-        
-        for i in range(len(selectarr)):
-            if(select == selectarr[i]): return package[i]
-        
-        if(select == "all"): return real, imag
-        
-
-
-    
-    def get_parang(self, time, ant, sourcearr, source, obsra, obsdec):
-        """
-        Calculate antenna field-rotation angles.
-        
-        Args:
-            time (numpy.array): a numpy array of time in UTC of the visibilities.
-            ant (numpy.array): a numpy array of antenna number of the visibilities.
-            sourcearr (numpy.array): a numpy array of source of the visibilities.
-            source (list): a list of calibrators.
-            obsra (list): a list of calibrators' right ascension in units of degrees.
-            obsdec (list): a list of calibrators' declination in units of degrees.
-        
-        Returns:
-            a numpy of the field-rotation angles.
-        """        
-        
-        num = len(time)
-        
-        lonarr, latarr, raarr, decarr, elarr, pararr, phiarr = \
-            np.zeros(num), np.zeros(num), np.zeros(num), np.zeros(num), np.zeros(num), np.zeros(num), np.zeros(num)
-            
-        # Produce numpy arrays for antenna longitudes, latitudes, and the coefficients of the field-rotation angle equations.
-        for m in range(self.nant):
-            lonarr[(ant == m)] = self.lonarr[m]
-            latarr[(ant == m)] = self.latarr[m]
-            elarr[(ant == m)] = self.f_el[m]
-            pararr[(ant == m)] = self.f_par[m]
-            phiarr[(ant == m)] = self.phi_off[m]
-        
-        # Produce numpy arrays for sources RA and Dec.
-        for l in range(len(source)):
-            raarr[sourcearr == source[l]] = obsra[l]
-            decarr[sourcearr == source[l]] = obsdec[l]
-            
-        latarr, decarr = np.radians(latarr), np.radians(decarr)
-
-        
-        date = np.zeros(len(time))
-        date[time>=24.] = 1
-        
-        hour = np.floor(time)
-        minute = np.floor((time - hour) * 60.)
-        second = (time - hour - minute / 60.) * 3600.
-        
-        hour[hour>=24.] -= 24.
-        
-        dumdatetime = dt.datetime(self.year, self.month, self.day)
-        dumdatetime2 = np.array([dumdatetime + dt.timedelta(hours=float(it)) for it in time])
-        
-
-        dumt = [] 
-
-        for dum in dumdatetime2:
-            dumt.append("{:04d}-{:02d}-{:02d}T{:02d}:{:02d}:{:f}".format(dum.year, dum.month, dum.day, dum.hour, dum.minute, dum.second + dum.microsecond * 1e-6))
-
-        dumt = at.Time(dumt)
-        gst = dumt.sidereal_time('mean','greenwich').hour
-
-
-        # # Convert UTC to GST using astropy Time.
-        # dumt = at.Time(["{:04d}-{:02d}-{:02d}T{:02d}:{:02d}:{:f}".format(self.year, self.month, self.day+int(dt), int(hr), int(mn), sec) for dt, hr, mn, sec in zip(date, hour, minute, second)])
-        # gst = dumt.sidereal_time('mean','greenwich').hour
-        
-        # Obtain field-rotation angles using the known equations.
-        hangle = np.radians(gst * 15. + lonarr - raarr)        
-        parang = np.arctan2((np.sin(hangle) * np.cos(latarr)), (np.sin(latarr) * np.cos(decarr) - np.cos(latarr) * np.sin(decarr) * np.cos(hangle)))        
-        altitude = np.arcsin(np.sin(decarr) * np.sin(latarr) + np.cos(decarr) * np.cos(latarr) * np.cos(hangle))
-        pang = elarr * altitude + pararr * parang + phiarr
-        
-        
-        return pang
-        
-    
-    
-
-    def coord(self):
-        """
-        Convert antenna positions from Cartesian to spherical coordinates using astropy.
-        
-        Returns:
-            lists of antenna longitudes, latitudes, and heights.
-        """      
-        self.lonarr = []
-        self.latarr = []
-        self.heightarr = []
-        
-        for i in range(len(self.antname)):
-            self.lonarr.append(EarthLocation.from_geocentric(self.antx[i], self.anty[i], self.antz[i], unit = 'm').to_geodetic()[0].value)
-            self.latarr.append(EarthLocation.from_geocentric(self.antx[i], self.anty[i], self.antz[i], unit = 'm').to_geodetic()[1].value)
-            self.heightarr.append(EarthLocation.from_geocentric(self.antx[i], self.anty[i], self.antz[i], unit = 'm').to_geodetic()[2].value)
-            
-        
-        return self.lonarr, self.latarr, self.heightarr
-
+#        # Check the input parameters
+#        for i in range(len(self.calsour)):
+#            if(self.calsour[i] not in self.source):
+#                self.source.append(self.calsour[i])
+#                self.logger.info('{:s} is not in SOURCE. It will be added.'.format(self.calsour[i]))
+#        
+#        for i in range(len(self.polcalsour)):
+#            if(self.polcalsour[i] not in self.source):
+#                self.source.append(self.polcalsour[i])
+#                self.logger.info('{:s} is not in SOURCE. It will be added.'.format(self.polcalsour[i]))
+        
+#        if(len(self.calsour) != len(self.cnum)):
+#            raise Exception("The number of CALSOUR and CNUM do nat match!")
+#        
+#        if(len(self.calsour) != len(self.autoccedt)):
+#            raise Exception("The number of CALSOUR and AUTOCCEDT do nat match!")
+#        
+#        for i in range(len(self.calsour)):
+#            if not path.exists(self.direc + self.dataname + self.calsour[i] + '.uvf'):
+#                raise Exception("{:s} does not exist in {:s}.".format(self.dataname + self.calsour[i] + '.uvf', self.direc))
+#            
+#            if not path.exists(self.direc + self.dataname + self.calsour[i] + '.fits'):
+#                raise Exception("{:s} does not exist in {:s}.".format(self.dataname + self.calsour[i] + '.fits', self.direc))
+#            
+#            if(self.autoccedt[i] == False):
+#                if (cnum[i] != 0) & (not path.exists(self.direc + 'gpcal/' + self.dataname + self.calsour[i] + '.box')):
+#                    message = "It was requested to split the total intensity CLEAN components of {:s} into sub-models (autoccedt = False) but there is no '.box' file in '{:s}'.".format(self.calsour[i], self.direc + 'gpcal/')
+#                    raise Exception(message)
+#        
+#        for i in range(len(self.polcalsour)):
+#            if not path.exists(self.direc + self.dataname + self.polcalsour[i] + '.uvf'):
+#                raise Exception("{:s} does not exist in {:s}.".format(self.dataname + self.polcalsour[i] + '.uvf', self.direc))
+#            
+#            if not path.exists(self.direc + self.dataname + self.polcalsour[i] + '.fits'):
+#                raise Exception("{:s} does not exist in {:s}.".format(self.dataname + self.polcalsour[i] + '.fits', self.direc))
 
 
     def get_zbl_data(self):
         """
         Make a pandas dataframe containing UV data and models for the zero-baseline D-term estimation
         
         """      
         
-        self.logger.info('\nGetting data for {:d} sources for {:d} IFs...\n'.format(len(self.zblcalsour), self.ifnum))
         
         AIPS.userno = self.aips_userno
         
         if self.aipslog:
             AIPS.log = open(self.logfile, 'a')
         AIPSTask.msgkill = -1
         
         
-        self.zbl_obsra = []
-        self.zbl_obsdec = []
+        ifarr, timearr, sourcearr, ant1arr, ant2arr, uarr, varr, rrrealarr, rrimagarr, rrweightarr, llrealarr, llimagarr, llweightarr, rlrealarr, rlimagarr, rlweightarr, lrrealarr, lrimagarr, lrweightarr = \
+            [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], []
+
+        pdkey = ["IF", "year", "month", "day", "time", "source", "ant1", "ant2", "u", "v", "pang1", "pang2", "rrreal", "rrimag", "rrsigma", "llreal", "llimag", "llsigma", "rlreal", "rlimag", "rlsigma", "lrreal", "lrimag", "lrsigma", \
+             "rramp", "rrphas", "rramp_sigma", "rrphas_sigma", "llamp", "llphas", "llamp_sigma", "llphas_sigma", "rlamp", "rlphas", "rlamp_sigma", "rlphas_sigma", "lramp", "lrphas", "lramp_sigma", "lrphas_sigma", \
+             "qamp", "qphas", "qamp_sigma", "qphas_sigma", "qsigma", "uamp", "uphas", "uamp_sigma", "uphas_sigma", "usigma"]
+
+        info = oh.basic_info(self.zblcalsour, self.direc, self.dataname)
+
+        obsra = info['obsra']
+        obsdec = info['obsdec']
+        year = info['year']
+        month = info['month']
+        day = info['day']
+        antname = info['antname']
+        antx = info['antx']
+        anty = info['anty']
+        antz = info['antz']
+        antmount = info['antmount']
+        ifnum = info['ifnum']
+        freq = info['freq']
+        f_par = info['f_par']
+        f_el = info['f_el']
+        phi_off = info['phi_off']
+        
+        self.logger.info('\nGetting data for {:d} sources for {:d} IFs...\n'.format(len(self.zblcalsour), ifnum))
+
+        lonarr, latarr, heightarr = oh.coord(antname, antx, anty, antz)
+
+        nant = len(antname)
+        
+        self.ifnum = ifnum
+        self.year = year
+        self.month = month
+        self.day = day
+        self.antname = antname
+        self.antmount = antmount
+        self.antx = antx
+        self.anty = anty
+        self.antz = antz
+        self.zbl_obsra = obsra
+        self.zbl_obsdec = obsdec
+
 
         zbl_antname = []
         for i in range(len(self.zblant)):
             zbl_antname.append(self.zblant[i][0])
             zbl_antname.append(self.zblant[i][1])   
             
 
         ifarr, timearr, sourcearr, ant1arr, ant2arr, uarr, varr, rrrealarr, rrimagarr, rrweightarr, llrealarr, llimagarr, llweightarr, rlrealarr, rlimagarr, rlweightarr, lrrealarr, lrimagarr, lrweightarr = \
             [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], []
 
         
-        # Define a pandas dataframe for the data array.
-        pdkey = ["IF", "time", "source", "ant1", "ant2", "u", "v", "pang1", "pang2", "rrreal", "rrimag", "rrsigma", "llreal", "llimag", "llsigma", "rlreal", "rlimag", "rlsigma", "lrreal", "lrimag", "lrsigma", \
-                 "rramp", "rrphas", "rramp_sigma", "rrphas_sigma", "llamp", "llphas", "llamp_sigma", "llphas_sigma", "rlamp", "rlphas", "rlamp_sigma", "rlphas_sigma", "lramp", "lrphas", "lramp_sigma", "lrphas_sigma", \
-                 "qamp", "qphas", "qamp_sigma", "qphas_sigma", "qsigma", "uamp", "uphas", "uamp_sigma", "uphas_sigma", "usigma"]
-
-            
         self.zbl_data = pd.DataFrame(columns = pdkey)
         
         
         for l in range(len(self.zblcalsour)):
         
-            inname = self.zblcalsour[l]
+            inname = str(self.zblcalsour[l])
         
             data = AIPSUVData(inname, 'EDIT', 1, 1)
             if(data.exists() == True):
                 data.clrstat()
                 data.zap()
             
             # Load UVFITS file.
-            self.runfitld(inname, 'EDIT', self.direc+self.dataname+self.zblcalsour[l]+'.uvf')
+            au.runfitld(inname, 'EDIT', self.direc+self.dataname+self.zblcalsour[l]+'.uvf')
                 
             data = AIPSUVData(inname, 'EDIT', 1, 1)
-            
-            # Extract source coordinates from the header.
-            self.zbl_obsra.append(data.header.crval[4])
-            self.zbl_obsdec.append(data.header.crval[5])
-            
+                        
             # Perform additional self-calibration with CALIB if requested.
             if self.selfcal:            
                 
                 cmap = AIPSImage(inname, 'CMAP', 1, 1)
                 if(cmap.exists() == True):
                     cmap.clrstat()
                     cmap.zap()
                     
-                self.runfitld(inname, 'CMAP', self.direc+self.dataname+self.zblcalsour[l]+'.fits')
+                au.runfitld(inname, 'CMAP', self.direc+self.dataname+self.zblcalsour[l]+'.fits')
                 
                 
                 calib = AIPSUVData(inname, 'CALIB', 1, 1)
                 if(calib.exists() == True):
                     calib.clrstat()
                     calib.zap()
                 
-                self.runcalib(inname, 'EDIT', 'CALIB', self.solint, self.soltype, self.solmode, self.weightit)
+                au.runcalib(inname, 'EDIT', inname, 'CMAP', 'CALIB', self.solint, self.soltype, self.solmode, self.weightit)
                 
                 calib = WAIPSUVData(inname, 'CALIB', 1, 1)
                 
                 dumu, dumv, ifname, time, ant1, ant2, rrreal, rrimag, rrweight, llreal, llimag, llweight, rlreal, rlimag, rlweight, lrreal, lrimag, lrweight = \
-                    self.uvprt(calib, "all")
+                    oh.uvprt(calib, "all")
                 
                 cmap.zap()                
                 calib.zap()
             
             else:
                 
                 data = WAIPSUVData(inname, 'EDIT', 1, 1)
                 
                 dumu, dumv, ifname, time, ant1, ant2, rrreal, rrimag, rrweight, llreal, llimag, llweight, rlreal, rlimag, rlweight, lrreal, lrimag, lrweight = \
-                    self.uvprt(data, "all")
+                    oh.uvprt(data, "all")
                     
                 
             data.zap()
             
             
             uarr = uarr + dumu
             varr = varr + dumv
@@ -927,14 +440,16 @@
 
         
         # Convert the lists to numpy arrays.
         ifarr, timearr, sourcearr, ant1arr, ant2arr, uarr, varr, rrrealarr, rrimagarr, rrweightarr, llrealarr, llimagarr, llweightarr, rlrealarr, rlimagarr, rlweightarr, lrrealarr, lrimagarr, lrweightarr = \
             np.array(ifarr), np.array(timearr), np.array(sourcearr), np.array(ant1arr), np.array(ant2arr), np.array(uarr), np.array(varr), np.array(rrrealarr), np.array(rrimagarr), np.array(rrweightarr), np.array(llrealarr), np.array(llimagarr), np.array(llweightarr), \
             np.array(rlrealarr), np.array(rlimagarr), np.array(rlweightarr), np.array(lrrealarr), np.array(lrimagarr), np.array(lrweightarr)
         
+        rlweightarr[rlweightarr > self.remove_weight_outlier_threshold * np.median(rlweightarr)] = np.median(rlweightarr)
+        lrweightarr[lrweightarr > self.remove_weight_outlier_threshold * np.median(lrweightarr)] = np.median(lrweightarr)
         
         # Combine the numpy arrays into a single pandas dataframe.
         self.zbl_data.loc[:,"IF"], self.zbl_data.loc[:,"time"], self.zbl_data.loc[:,"source"], self.zbl_data.loc[:,"ant1"], self.zbl_data.loc[:,"ant2"], self.zbl_data.loc[:,"u"], self.zbl_data.loc[:,"v"], \
         self.zbl_data.loc[:,"rrreal"], self.zbl_data.loc[:,"rrimag"], self.zbl_data.loc[:,"rrweight"], self.zbl_data.loc[:,"llreal"], self.zbl_data.loc[:,"llimag"], self.zbl_data.loc[:,"llweight"], \
         self.zbl_data.loc[:,"rlreal"], self.zbl_data.loc[:,"rlimag"], self.zbl_data.loc[:,"rlweight"], self.zbl_data.loc[:,"lrreal"], self.zbl_data.loc[:,"lrimag"], self.zbl_data.loc[:,"lrweight"] = \
                 ifarr, timearr * 24., sourcearr, ant1arr - 1, ant2arr - 1, uarr, varr, rrrealarr, rrimagarr, rrweightarr, llrealarr, llimagarr, llweightarr, rlrealarr, rlimagarr, rlweightarr, lrrealarr, lrimagarr, lrweightarr
         
@@ -943,63 +458,42 @@
         select = (ant1arr-1 == zbl_antname.index(zblant[0])) & (ant2arr-1 == zbl_antname.index(zblant[1]))
         for j in range(len(self.zblant)):
             zblant = self.zblant[j]
             dumselect = (ant1arr-1 == zbl_antname.index(zblant[0])) & (ant2arr-1 == zbl_antname.index(zblant[1]))
             select = np.logical_or(select, dumselect)
             
         # Filter bad data points.
-        select = select & (rrrealarr != 0.) & (llrealarr != 0.) & (rlrealarr != 0.) & (lrrealarr != 0.) & (rrimagarr != 0.) & (llimagarr != 0.) & (rlimagarr != 0.) & (lrimagarr != 0.) & \
-            (rrweightarr > 0.) & (llweightarr > 0.) & (rlweightarr > 0.) & (lrweightarr > 0.)
+        select = select & (rrweightarr > 0.) & (llweightarr > 0.) & (rlweightarr > 0.) & (lrweightarr > 0.) & (~np.isnan(rrweightarr)) & (~np.isnan(llweightarr)) & (~np.isnan(rlweightarr)) & (~np.isnan(lrweightarr))
+        
         
         self.zbl_data = self.zbl_data.loc[select].reset_index(drop=True)
         
-        self.zbl_data.loc[:,"pang1"] = self.get_parang(np.array(self.zbl_data["time"]), np.array(self.zbl_data["ant1"]), np.array(self.zbl_data["source"]), self.zblcalsour, self.zbl_obsra, self.zbl_obsdec)
-        self.zbl_data.loc[:,"pang2"] = self.get_parang(np.array(self.zbl_data["time"]), np.array(self.zbl_data["ant2"]), np.array(self.zbl_data["source"]), self.zblcalsour, self.zbl_obsra, self.zbl_obsdec)
-
-      
-        # Make new columns for amplitudes, phases, and corresponding errors, etc.
-        self.zbl_data.loc[:,"rrsigma"], self.zbl_data.loc[:,"llsigma"], self.zbl_data.loc[:,"rlsigma"], self.zbl_data.loc[:,"lrsigma"] = \
-            1. / self.zbl_data.loc[:,"rrweight"] ** (0.5), 1. / self.zbl_data.loc[:,"llweight"], 1. / self.zbl_data.loc[:,"rlweight"] ** (0.5), 1. / self.zbl_data.loc[:,"lrweight"] ** (0.5)
-        
-        self.zbl_data.loc[:,"rramp"], self.zbl_data.loc[:,"llamp"], self.zbl_data.loc[:,"rlamp"], self.zbl_data.loc[:,"lramp"] = \
-            np.absolute(self.zbl_data.loc[:,"rrreal"] + 1j*self.zbl_data.loc[:,"rrimag"]), np.absolute(self.zbl_data.loc[:,"llreal"] + 1j*self.zbl_data.loc[:,"llimag"]), \
-            np.absolute(self.zbl_data.loc[:,"rlreal"] + 1j*self.zbl_data.loc[:,"rlimag"]), np.absolute(self.zbl_data.loc[:,"lrreal"] + 1j*self.zbl_data.loc[:,"lrimag"])
-        
-        self.zbl_data.loc[:,"rrphas"], self.zbl_data.loc[:,"llphas"], self.zbl_data.loc[:,"rlphas"], self.zbl_data.loc[:,"lrphas"] = \
-            np.angle(self.zbl_data.loc[:,"rrreal"] + 1j*self.zbl_data.loc[:,"rrimag"]), np.angle(self.zbl_data.loc[:,"llreal"] + 1j*self.zbl_data.loc[:,"llimag"]), \
-            np.angle(self.zbl_data.loc[:,"rlreal"] + 1j*self.zbl_data.loc[:,"rlimag"]), np.angle(self.zbl_data.loc[:,"lrreal"] + 1j*self.zbl_data.loc[:,"lrimag"])
-        
-        self.zbl_data.loc[:,"rramp_sigma"], self.zbl_data.loc[:,"llamp_sigma"], self.zbl_data.loc[:,"rlamp_sigma"], self.zbl_data.loc[:,"lramp_sigma"] = \
-            self.amperror(self.zbl_data.loc[:,"rrreal"] + 1j*self.zbl_data.loc[:,"rrimag"], self.zbl_data.loc[:,"rrsigma"] + 1j*self.zbl_data.loc[:,"rrsigma"]), \
-            self.amperror(self.zbl_data.loc[:,"llreal"] + 1j*self.zbl_data.loc[:,"llimag"], self.zbl_data.loc[:,"llsigma"] + 1j*self.zbl_data.loc[:,"llsigma"]), \
-            self.amperror(self.zbl_data.loc[:,"rlreal"] + 1j*self.zbl_data.loc[:,"rlimag"], self.zbl_data.loc[:,"rlsigma"] + 1j*self.zbl_data.loc[:,"rlsigma"]), \
-            self.amperror(self.zbl_data.loc[:,"lrreal"] + 1j*self.zbl_data.loc[:,"lrimag"], self.zbl_data.loc[:,"lrsigma"] + 1j*self.zbl_data.loc[:,"lrsigma"])
-        
-        self.zbl_data.loc[:,"rrphas_sigma"], self.zbl_data.loc[:,"llphas_sigma"], self.zbl_data.loc[:,"rlphas_sigma"], self.zbl_data.loc[:,"lrphas_sigma"] = \
-            self.phaserror(self.zbl_data.loc[:,"rrreal"] + 1j*self.zbl_data.loc[:,"rrimag"], self.zbl_data.loc[:,"rrsigma"] + 1j*self.zbl_data.loc[:,"rrsigma"]), \
-            self.phaserror(self.zbl_data.loc[:,"llreal"] + 1j*self.zbl_data.loc[:,"llimag"], self.zbl_data.loc[:,"llsigma"] + 1j*self.zbl_data.loc[:,"llsigma"]), \
-            self.phaserror(self.zbl_data.loc[:,"rlreal"] + 1j*self.zbl_data.loc[:,"rlimag"], self.zbl_data.loc[:,"rlsigma"] + 1j*self.zbl_data.loc[:,"rlsigma"]), \
-            self.phaserror(self.zbl_data.loc[:,"lrreal"] + 1j*self.zbl_data.loc[:,"lrimag"], self.zbl_data.loc[:,"lrsigma"] + 1j*self.zbl_data.loc[:,"lrsigma"])
-            
-        
-        dumrl, dumlr = self.zbl_data.loc[:,"rlreal"] + 1j*self.zbl_data.loc[:,"rlimag"], self.zbl_data.loc[:,"lrreal"] + 1j*self.zbl_data.loc[:,"lrimag"]
-        dumrlsigma, dumlrsigma = self.zbl_data.loc[:,"rlsigma"] + 1j*self.zbl_data.loc[:,"rlsigma"], self.zbl_data.loc[:,"lrsigma"] + 1j*self.zbl_data.loc[:,"lrsigma"]
-        
-        dumq, dumu = (dumrl + dumlr) / 2., -1j * (dumrl - dumlr) / 2.
-        dumqsigma, dumusigma = np.sqrt(dumrlsigma**2 + dumlrsigma**2) / 2., np.sqrt(dumrlsigma**2 + dumlrsigma**2) / 2.
-        
-        self.zbl_data.loc[:,"qamp"], self.zbl_data.loc[:,"uamp"], self.zbl_data.loc[:,"qphas"], self.zbl_data.loc[:,"uphas"] = np.absolute(dumq), np.absolute(dumu), np.angle(dumq), np.angle(dumu)
-        self.zbl_data.loc[:,"qamp_sigma"], self.zbl_data.loc[:,"uamp_sigma"], self.zbl_data.loc[:,"qphas_sigma"], self.zbl_data.loc[:,"uphas_sigma"] = \
-            self.amperror(dumq, dumqsigma), self.amperror(dumu, dumusigma), self.phaserror(dumq, dumqsigma), self.phaserror(dumu, dumusigma)
-        self.zbl_data.loc[:,"qsigma"], self.zbl_data.loc[:,"usigma"] = np.real(dumqsigma), np.real(dumusigma)
-
-        self.zbl_data["IF"] = self.zbl_data["IF"].astype('int32')
-        self.zbl_data["ant1"] = self.zbl_data["ant1"].astype('int32')
-        self.zbl_data["ant2"] = self.zbl_data["ant2"].astype('int32')
+        dumant1 = self.zbl_data.loc[:,"ant1"]
+        dumant2 = self.zbl_data.loc[:,"ant2"]
+        dumsource = self.zbl_data.loc[:,"source"]
 
+        longarr1, latarr1, f_el1, f_par1, phi_off1 = oh.coordarr(lonarr, latarr, f_el, f_par, phi_off, dumant1)
+        longarr2, latarr2, f_el2, f_par2, phi_off2 = oh.coordarr(lonarr, latarr, f_el, f_par, phi_off, dumant2)
+        
+        yeararr, montharr, dayarr, raarr, decarr = oh.calendar(dumsource, self.zblcalsour, year, month, day, obsra, obsdec)
+        
+        timearr = np.array(self.zbl_data.loc[:,"time"])
+                
+        for i in range(10):
+            dayarr[timearr>=24.] += 1 
+            timearr[timearr>=24.] -= 24. 
+                
+        self.zbl_data.loc[:,"year"] = yeararr
+        self.zbl_data.loc[:,"month"] = montharr
+        self.zbl_data.loc[:,"day"] = dayarr
+        
+        self.zbl_data.loc[:,"pang1"] = oh.get_parang(yeararr, montharr, dayarr, timearr, raarr, decarr, longarr1, latarr1, f_el1, f_par1, phi_off1)
+        self.zbl_data.loc[:,"pang2"] = oh.get_parang(yeararr, montharr, dayarr, timearr, raarr, decarr, longarr2, latarr2, f_el2, f_par2, phi_off2)          
+        
+        self.zbl_data = oh.pd_modifier(self.zbl_data)
 
     
 
     def get_data(self):
         """
         Make a pandas dataframe containing UV data and models for the D-term estimation using the similarity assumption.
         
@@ -1007,105 +501,54 @@
         
         AIPS.userno = self.aips_userno
         
         if self.aipslog:
             AIPS.log = open(self.logfile, 'a')
         AIPSTask.msgkill = -1
         
-        self.obsra = []
-        self.obsdec = []
+        self.obsra, self.obsdec, self.year, self.month, self.day = [], [], [], [], []
 
 
         ifarr, timearr, sourcearr, ant1arr, ant2arr, uarr, varr, rrrealarr, rrimagarr, rrweightarr, llrealarr, llimagarr, llweightarr, rlrealarr, rlimagarr, rlweightarr, lrrealarr, lrimagarr, lrweightarr = \
             [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], []
 
-        # Define a pandas dataframe for the data array.
-        pdkey = ["IF", "time", "source", "ant1", "ant2", "u", "v", "pang1", "pang2", "rrreal", "rrimag", "rrsigma", "llreal", "llimag", "llsigma", "rlreal", "rlimag", "rlsigma", "lrreal", "lrimag", "lrsigma", \
+        pdkey = ["IF", "year", "month", "day", "time", "source", "ant1", "ant2", "u", "v", "pang1", "pang2", "rrreal", "rrimag", "rrsigma", "llreal", "llimag", "llsigma", "rlreal", "rlimag", "rlsigma", "lrreal", "lrimag", "lrsigma", \
                  "rramp", "rrphas", "rramp_sigma", "rrphas_sigma", "llamp", "llphas", "llamp_sigma", "llphas_sigma", "rlamp", "rlphas", "rlamp_sigma", "rlphas_sigma", "lramp", "lrphas", "lramp_sigma", "lrphas_sigma", \
                  "qamp", "qphas", "qamp_sigma", "qphas_sigma", "qsigma", "uamp", "uphas", "uamp_sigma", "uphas_sigma", "usigma"]
 
         orig_cnum = copy.deepcopy(self.cnum)
         
         for i in range(max(self.cnum)):
             pdkey.append("model"+str(i+1)+"_amp")
             pdkey.append("model"+str(i+1)+"_phas")
             
         self.data = pd.DataFrame(columns = pdkey)
- 
+
+
+        info = oh.basic_info(self.calsour, self.direc, self.dataname)
         
-        for l in range(len(self.calsour)):
-            inname = self.calsour[l]
-            
-            data = AIPSUVData(inname, 'EDIT', 1, 1)
-            if(data.exists() == True):
-                data.clrstat()
-                data.zap()
-            
-            # Load UVFITS files.
-            self.runfitld(inname, 'EDIT', self.direc+self.dataname+self.calsour[l]+'.uvf')
-            
-            data = AIPSUVData(inname, 'EDIT', 1, 1)
-            
-            # Extract source coordinates from the header.
-            self.obsra.append(data.header.crval[4])
-            self.obsdec.append(data.header.crval[5])
-            
-            
-            # Extract antenna, frequency, mount information, etc, from the header.
-            if(l == 0):
-                self.antname = []
-                self.antx = []
-                self.anty = []
-                self.antz = []
-                self.antmount = []
-                
-                antable = data.table('AN', 1)
-                for row in antable:
-                    self.antname.append(row.anname.replace(' ', ''))
-                    self.antx.append(row.stabxyz[0])
-                    self.anty.append(row.stabxyz[1])
-                    self.antz.append(row.stabxyz[2])
-                    self.antmount.append(row.mntsta)
-                
-                fqtable = data.table('FQ', 1)
-                if(isinstance(fqtable[0].if_freq, float) == True):
-                    self.ifnum = 1
-                    IFfreq = [data.header.crval[2] / 1e9]
-                    self.freq = "{0:.3f}".format(IFfreq[0]) + ' GHz'
-                else:
-                    self.ifnum = len(fqtable[0].if_freq)
-                    self.freq = [str((it + data.header.crval[2]) / 1e9) + ' GHz' for it in fqtable[0].if_freq]
-                self.obsdate = data.header.date_obs
-                
-                
-                self.f_par = []
-                self.f_el = []
-                self.phi_off = []
-                
-                for st in range(len(self.antname)):
-                    self.f_par.append(1.)
-                    if(self.antmount[st] == 0):
-                        self.f_el.append(0.)
-                    if(self.antmount[st] == 4):
-                        self.f_el.append(1.)
-                    if(self.antmount[st] == 5):
-                        self.f_el.append(-1.)
-                    self.phi_off.append(0.)
-            
-            
-                self.lonarr, self.latarr, self.heightarr = self.coord()
-                
-                self.year = int(self.obsdate[0:4])
-                self.month = int(self.obsdate[5:7])
-                self.day = int(self.obsdate[8:10])
-                
-                self.nant = len(self.antname)    
+        self.obsra = info['obsra']
+        self.obsdec = info['obsdec']
+        self.year = info['year']
+        self.month = info['month']
+        self.day = info['day']
+        self.antname = info['antname']
+        self.antx = info['antx']
+        self.anty = info['anty']
+        self.antz = info['antz']
+        self.antmount = info['antmount']
+        self.ifnum = info['ifnum']
+        self.freq = info['freq']
+        self.f_par = info['f_par']
+        self.f_el = info['f_el']
+        self.phi_off = info['phi_off']
         
-
-            data.zap()
+        self.lonarr, self.latarr, self.heightarr = oh.coord(self.antname, self.antx, self.anty, self.antz)
+        
+        self.nant = len(self.antname)
         
 
             
         self.logger.info('\nGetting data for {:d} sources for {:d} IFs...\n'.format(len(self.calsour), self.ifnum))
         
         
         # Add source sub-model columns to the pandas dataframe.
@@ -1118,37 +561,37 @@
         self.chisq = pd.DataFrame(index = index, columns = ['IF'+str(it+1) for it in np.arange(self.ifnum)])
         
         
         for l in range(len(self.calsour)):
             
             dumdata = pd.DataFrame(columns = pdkey)
         
-            inname = self.calsour[l]
+            inname = str(self.calsour[l])
         
             data = AIPSUVData(inname, 'EDIT', 1, 1)
             if(data.exists() == True):
                 data.clrstat()
                 data.zap()
             
             cmap = AIPSImage(inname, 'CMAP', 1, 1)
             if(cmap.exists() == True):
                 cmap.clrstat()
                 cmap.zap()
                 
             # Load UVFITS and image fits files.
-            self.runfitld(inname, 'EDIT', self.direc+self.dataname+self.calsour[l]+'.uvf')
-            self.runfitld(inname, 'CMAP', self.direc+self.dataname+self.calsour[l]+'.fits')
+            au.runfitld(inname, 'EDIT', self.direc+self.dataname+self.calsour[l]+'.uvf')
+            au.runfitld(inname, 'CMAP', self.direc+self.dataname+self.calsour[l]+'.fits')
         
                 
             data = AIPSUVData(inname, 'EDIT', 1, 1)
             
             # Perform additional self-calibration with CALIB if requested.
             if self.selfcal:            
                 if(self.cnum[l] >= 2):
-                    self.runccedt(inname, self.direc+'gpcal/'+self.dataname+self.calsour[l]+'.box', self.cnum[l], self.autoccedt[l])
+                    au.runccedt(inname, self.direc+'gpcal/'+self.dataname+self.calsour[l]+'.box', self.cnum[l], self.autoccedt[l])
                 
                 # If automatic CCEDT is performed, then sometimes the output number of sub-models is not the same as the input number. Correct for cnum if this is the case.
                 if self.autoccedt[l]:
                     if(self.cnum[l] != 1):
                         dumcnum = 0
                         
                         for cn in cmap.tables:
@@ -1159,49 +602,49 @@
                     
                 
                 calib = AIPSUVData(inname, 'CALIB', 1, 1)
                 if(calib.exists() == True):
                     calib.clrstat()
                     calib.zap()
                 
-                self.runcalib(inname, 'EDIT', 'CALIB', self.solint, self.soltype, self.solmode, self.weightit)
+                au.runcalib(inname, 'EDIT', inname, 'CMAP', 'CALIB', self.solint, self.soltype, self.solmode, self.weightit)
                 
                 # Export the self-calibrated UVFITS files to the working directory.
                 if path.exists(self.direc + self.dataname + self.calsour[l] + '.calib'):
                     os.system('rm ' + self.direc + self.dataname + self.calsour[l] + '.calib')
-                self.runfittp(inname, 'CALIB', self.direc + self.dataname + self.calsour[l] + '.calib')
+                au.runfittp(inname, 'CALIB', self.direc + self.dataname + self.calsour[l] + '.calib')
                 
                 calib = AIPSUVData(inname, 'CALIB', 1, 1)
                 
                 # Obtain model visibilities for each visibility measurement for each sub-model.
                 if(self.cnum[l] >= 2):
                     for m in range(self.cnum[l]):
                         
                         moddata = AIPSUVData(inname, 'UVSUB', 1, m+1)
                         if(moddata.exists() == True):
                             moddata.clrstat()
                             moddata.zap()
                             
-                        self.runuvsub(inname, 'CALIB', 'CMAP', m+2, m+1)
+                        au.runuvsub(inname, 'CALIB', 'CMAP', m+2, m+1)
                         
                 elif (self.cnum[l] == 1):
                     moddata = AIPSUVData(inname, 'UVSUB', 1, 1)
                     if(moddata.exists() == True):
                         moddata.clrstat()
                         moddata.zap()
                     
-                    self.runuvsub(inname, 'CALIB', 'CMAP', 1, 1)
+                    au.runuvsub(inname, 'CALIB', 'CMAP', 1, 1)
                 
                 
                 calib = WAIPSUVData(inname, 'CALIB', 1, 1)
                 
                 
                 # Extract UV data.
                 dumu, dumv, ifname, time, ant1, ant2, rrreal, rrimag, rrweight, llreal, llimag, llweight, rlreal, rlimag, rlweight, lrreal, lrimag, lrweight = \
-                    self.uvprt(calib, "all")
+                    oh.uvprt(calib, "all")
                 
                 # Stack the data lists.
                 uarr = uarr + dumu
                 varr = varr + dumv
                 sourcearr = sourcearr + [self.calsour[l]] * len(time)
                 ifarr = ifarr + ifname
                 timearr = timearr + time
@@ -1227,31 +670,31 @@
                     nanarr[:] = np.NaN
                     dumdata.loc[:,"model1_amp"] = nanarr
                 else:
                     for m in range(self.cnum[l]):
                         
                         moddata = WAIPSUVData(inname, 'UVSUB', 1, m+1)
                         
-                        modreal = np.array(self.uvprt(moddata, "rrreal"), dtype = 'float64')
-                        modimag = np.array(self.uvprt(moddata, "rrimag"), dtype = 'float64')
+                        modreal = np.array(oh.uvprt(moddata, "rrreal"), dtype = 'float64')
+                        modimag = np.array(oh.uvprt(moddata, "rrimag"), dtype = 'float64')
                             
                         dumdata.loc[:,"model"+str(m+1)+"_amp"] = np.absolute(modreal + 1j*modimag)
                         dumdata.loc[:,"model"+str(m+1)+"_phas"] = np.angle(modreal + 1j*modimag)
 
 
                 # Run LPCAL and export the antenna files if requested.
                 if self.lpcal:
-                    self.runlpcal(inname, 'CALIB', 'CMAP', self.cnum[l])
+                    au.runlpcal(inname, 'CALIB', 'CMAP', self.cnum[l])
                     
-                    self.runprtab(calib, self.direc+'gpcal/'+self.dataname+self.calsour[l]+'.an')
+                    au.runprtab(calib, self.direc+'gpcal/'+self.dataname+self.calsour[l]+'.an')
             
             else:
                 # Repeat the same procedure except for additional self-calibration.
                 if(self.cnum[l] >= 2):
-                    self.runccedt(inname, self.direc+'gpcal/' + self.dataname+self.calsour[l]+'.box', self.cnum[l], self.autoccedt[l])
+                    au.runccedt(inname, self.direc+'gpcal/' + self.dataname+self.calsour[l]+'.box', self.cnum[l], self.autoccedt[l])
                 
                 if self.autoccedt[l]:
                     
                     if(self.cnum[l] != 1):
                         dumcnum = 0
                         
                         for cn in cmap.tables:
@@ -1265,28 +708,28 @@
                     for m in range(self.cnum[l]):
                         
                         moddata = AIPSUVData(inname, 'UVSUB', 1, m+1)
                         if(moddata.exists() == True):
                             moddata.clrstat()
                             moddata.zap()
                             
-                        self.runuvsub(inname, 'EDIT', 'CMAP', m+2, m+1)
+                        au.runuvsub(inname, 'EDIT', 'CMAP', m+2, m+1)
                 elif (self.cnum[l] == 1):
                     moddata = AIPSUVData(inname, 'UVSUB', 1, 1)
                     if(moddata.exists() == True):
                         moddata.clrstat()
                         moddata.zap()
                         
-                    self.runuvsub(inname, 'EDIT', 'CMAP', 1, 1)
+                    au.runuvsub(inname, 'EDIT', 'CMAP', 1, 1)
                     
                     
                 data = WAIPSUVData(inname, 'EDIT', 1, 1)
                 
                 dumu, dumv, ifname, time, ant1, ant2, rrreal, rrimag, rrweight, llreal, llimag, llweight, rlreal, rlimag, rlweight, lrreal, lrimag, lrweight = \
-                    self.uvprt(data, "all")
+                    oh.uvprt(data, "all")
                 
                 uarr = uarr + dumu
                 varr = varr + dumv
                 sourcearr = sourcearr + [self.calsour[l]] * len(time)
                 ifarr = ifarr + ifname
                 timearr = timearr + time
                 ant1arr = ant1arr + ant1
@@ -1309,25 +752,25 @@
                     nanarr = np.empty(len(time))
                     nanarr[:] = np.NaN
                     dumdata.loc[:,"model1_amp"] = nanarr
                 else:
                     for m in range(self.cnum[l]):
                         moddata = WAIPSUVData(inname, 'UVSUB', 1, m+1)
                         
-                        modreal = np.array(self.uvprt(moddata, "rrreal"), dtype = 'float64')
-                        modimag = np.array(self.uvprt(moddata, "rrimag"), dtype = 'float64')
+                        modreal = np.array(oh.uvprt(moddata, "rrreal"), dtype = 'float64')
+                        modimag = np.array(oh.uvprt(moddata, "rrimag"), dtype = 'float64')
                         
                         dumdata.loc[:,"model"+str(m+1)+"_amp"] = np.absolute(modreal + 1j*modimag)
                         dumdata.loc[:,"model"+str(m+1)+"_phas"] = np.angle(modreal + 1j*modimag)
 
                 
                 if self.lpcal:
-                    self.runlpcal(inname, 'EDIT', 'CMAP', self.cnum[l])
+                    au.runlpcal(inname, 'EDIT', 'CMAP', self.cnum[l])
                     lpcal = AIPSUVData(inname, 'EDIT', 1, 1)
-                    self.runprtab(lpcal, self.direc+'gpcal/'+self.dataname+self.calsour[l]+'.an')
+                    au.runprtab(lpcal, self.direc+'gpcal/'+self.dataname+self.calsour[l]+'.an')
             
             if(self.cnum[l] >= 2):
                 for m in range(self.cnum[l]):
                     moddata = AIPSUVData(inname, 'UVSUB', 1, m+1)
                     moddata.zap()
             elif (self.cnum[l] == 1):
                 moddata = AIPSUVData(inname, 'UVSUB', 1, 1)
@@ -1355,73 +798,55 @@
         ifarr, timearr, sourcearr, ant1arr, ant2arr, uarr, varr, rrrealarr, rrimagarr, rrweightarr, llrealarr, llimagarr, llweightarr, rlrealarr, rlimagarr, rlweightarr, lrrealarr, lrimagarr, lrweightarr = \
             np.array(ifarr), np.array(timearr), np.array(sourcearr), np.array(ant1arr), np.array(ant2arr), np.array(uarr), np.array(varr), np.array(rrrealarr), np.array(rrimagarr), np.array(rrweightarr), np.array(llrealarr), np.array(llimagarr), np.array(llweightarr), \
             np.array(rlrealarr), np.array(rlimagarr), np.array(rlweightarr), np.array(lrrealarr), np.array(lrimagarr), np.array(lrweightarr)
         
         rlweightarr[rlweightarr > self.remove_weight_outlier_threshold * np.median(rlweightarr)] = np.median(rlweightarr)
         lrweightarr[lrweightarr > self.remove_weight_outlier_threshold * np.median(lrweightarr)] = np.median(lrweightarr)
         
-        
         # Combine the numpy arrays into a single pandas dataframe.
         self.data.loc[:,"IF"], self.data.loc[:,"time"], self.data.loc[:,"source"], self.data.loc[:,"ant1"], self.data.loc[:,"ant2"], self.data.loc[:,"u"], self.data.loc[:,"v"], \
         self.data.loc[:,"rrreal"], self.data.loc[:,"rrimag"], self.data.loc[:,"rrweight"], self.data.loc[:,"llreal"], self.data.loc[:,"llimag"], self.data.loc[:,"llweight"], \
         self.data.loc[:,"rlreal"], self.data.loc[:,"rlimag"], self.data.loc[:,"rlweight"], self.data.loc[:,"lrreal"], self.data.loc[:,"lrimag"], self.data.loc[:,"lrweight"] = \
                 ifarr, timearr * 24., sourcearr, ant1arr - 1, ant2arr - 1, uarr, varr, rrrealarr, rrimagarr, rrweightarr, llrealarr, llimagarr, llweightarr, rlrealarr, rlimagarr, rlweightarr, lrrealarr, lrimagarr, lrweightarr
         
-                
-        self.data.loc[:,"pang1"] = self.get_parang(np.array(self.data["time"]), np.array(self.data["ant1"]), np.array(self.data["source"]), self.calsour, self.obsra, self.obsdec)
-        self.data.loc[:,"pang2"] = self.get_parang(np.array(self.data["time"]), np.array(self.data["ant2"]), np.array(self.data["source"]), self.calsour, self.obsra, self.obsdec)
-
-        # Make new columns for amplitudes, phases, and corresponding errors, etc.
-        self.data.loc[:,"rrsigma"], self.data.loc[:,"llsigma"], self.data.loc[:,"rlsigma"], self.data.loc[:,"lrsigma"] = \
-            1. / self.data.loc[:,"rrweight"] ** (0.5), 1. / self.data.loc[:,"llweight"], 1. / self.data.loc[:,"rlweight"] ** (0.5), 1. / self.data.loc[:,"lrweight"] ** (0.5)
-        
-        self.data.loc[:,"rramp"], self.data.loc[:,"llamp"], self.data.loc[:,"rlamp"], self.data.loc[:,"lramp"] = \
-            np.absolute(self.data.loc[:,"rrreal"] + 1j*self.data.loc[:,"rrimag"]), np.absolute(self.data.loc[:,"llreal"] + 1j*self.data.loc[:,"llimag"]), \
-            np.absolute(self.data.loc[:,"rlreal"] + 1j*self.data.loc[:,"rlimag"]), np.absolute(self.data.loc[:,"lrreal"] + 1j*self.data.loc[:,"lrimag"])
-        
-        self.data.loc[:,"rrphas"], self.data.loc[:,"llphas"], self.data.loc[:,"rlphas"], self.data.loc[:,"lrphas"] = \
-            np.angle(self.data.loc[:,"rrreal"] + 1j*self.data.loc[:,"rrimag"]), np.angle(self.data.loc[:,"llreal"] + 1j*self.data.loc[:,"llimag"]), \
-            np.angle(self.data.loc[:,"rlreal"] + 1j*self.data.loc[:,"rlimag"]), np.angle(self.data.loc[:,"lrreal"] + 1j*self.data.loc[:,"lrimag"])
-        
-        self.data.loc[:,"rramp_sigma"], self.data.loc[:,"llamp_sigma"], self.data.loc[:,"rlamp_sigma"], self.data.loc[:,"lramp_sigma"] = \
-            self.amperror(self.data.loc[:,"rrreal"] + 1j*self.data.loc[:,"rrimag"], self.data.loc[:,"rrsigma"] + 1j*self.data.loc[:,"rrsigma"]), \
-            self.amperror(self.data.loc[:,"llreal"] + 1j*self.data.loc[:,"llimag"], self.data.loc[:,"llsigma"] + 1j*self.data.loc[:,"llsigma"]), \
-            self.amperror(self.data.loc[:,"rlreal"] + 1j*self.data.loc[:,"rlimag"], self.data.loc[:,"rlsigma"] + 1j*self.data.loc[:,"rlsigma"]), \
-            self.amperror(self.data.loc[:,"lrreal"] + 1j*self.data.loc[:,"lrimag"], self.data.loc[:,"lrsigma"] + 1j*self.data.loc[:,"lrsigma"])
-        
-        self.data.loc[:,"rrphas_sigma"], self.data.loc[:,"llphas_sigma"], self.data.loc[:,"rlphas_sigma"], self.data.loc[:,"lrphas_sigma"] = \
-            self.phaserror(self.data.loc[:,"rrreal"] + 1j*self.data.loc[:,"rrimag"], self.data.loc[:,"rrsigma"] + 1j*self.data.loc[:,"rrsigma"]), \
-            self.phaserror(self.data.loc[:,"llreal"] + 1j*self.data.loc[:,"llimag"], self.data.loc[:,"llsigma"] + 1j*self.data.loc[:,"llsigma"]), \
-            self.phaserror(self.data.loc[:,"rlreal"] + 1j*self.data.loc[:,"rlimag"], self.data.loc[:,"rlsigma"] + 1j*self.data.loc[:,"rlsigma"]), \
-            self.phaserror(self.data.loc[:,"lrreal"] + 1j*self.data.loc[:,"lrimag"], self.data.loc[:,"lrsigma"] + 1j*self.data.loc[:,"lrsigma"])
-            
-        
-        dumrl, dumlr = self.data.loc[:,"rlreal"] + 1j*self.data.loc[:,"rlimag"], self.data.loc[:,"lrreal"] + 1j*self.data.loc[:,"lrimag"]
-        dumrlsigma, dumlrsigma = self.data.loc[:,"rlsigma"] + 1j*self.data.loc[:,"rlsigma"], self.data.loc[:,"lrsigma"] + 1j*self.data.loc[:,"lrsigma"]
-        
-        dumq, dumu = (dumrl + dumlr) / 2., -1j * (dumrl - dumlr) / 2.
-        dumqsigma, dumusigma = np.sqrt(dumrlsigma**2 + dumlrsigma**2) / 2., np.sqrt(dumrlsigma**2 + dumlrsigma**2) / 2.
-        
-        self.data.loc[:,"qamp"], self.data.loc[:,"uamp"], self.data.loc[:,"qphas"], self.data.loc[:,"uphas"] = np.absolute(dumq), np.absolute(dumu), np.angle(dumq), np.angle(dumu)
-        self.data.loc[:,"qamp_sigma"], self.data.loc[:,"uamp_sigma"], self.data.loc[:,"qphas_sigma"], self.data.loc[:,"uphas_sigma"] = \
-            self.amperror(dumq, dumqsigma), self.amperror(dumu, dumusigma), self.phaserror(dumq, dumqsigma), self.phaserror(dumu, dumusigma)
-        self.data.loc[:,"qsigma"], self.data.loc[:,"usigma"] = np.real(dumqsigma), np.real(dumusigma)
-
-        self.data["IF"] = self.data["IF"].astype('int32')
-        self.data["ant1"] = self.data["ant1"].astype('int32')
-        self.data["ant2"] = self.data["ant2"].astype('int32')
-        self.data["pang1"] = self.data["pang1"].astype('float64')
-        self.data["pang2"] = self.data["pang2"].astype('float64')
+        # Filter bad data points.
+        select = (rrweightarr > 0.) & (llweightarr > 0.) & (rlweightarr > 0.) & (lrweightarr > 0.) & (~np.isnan(rrweightarr)) & (~np.isnan(llweightarr)) & (~np.isnan(rlweightarr)) & (~np.isnan(lrweightarr))
         
+        self.data = self.data.loc[select].reset_index(drop=True)
+   
+        dumant1 = self.data.loc[:,"ant1"]
+        dumant2 = self.data.loc[:,"ant2"]
+        dumsource = self.data.loc[:,"source"]
+        
+        longarr1, latarr1, f_el1, f_par1, phi_off1 = oh.coordarr(self.lonarr, self.latarr, self.f_el, self.f_par, self.phi_off, dumant1)
+        longarr2, latarr2, f_el2, f_par2, phi_off2 = oh.coordarr(self.lonarr, self.latarr, self.f_el, self.f_par, self.phi_off, dumant2)
+        
+        yeararr, montharr, dayarr, raarr, decarr = oh.calendar(dumsource, self.calsour, self.year, self.month, self.day, self.obsra, self.obsdec)
+        
+        timearr = np.array(self.data.loc[:,"time"])
+        
+        for i in range(10):
+            dayarr[timearr>=24.] += 1 
+            timearr[timearr>=24.] -= 24. 
+        
+        self.data.loc[:,"time"] = timearr
+        self.data.loc[:,"year"] = yeararr
+        self.data.loc[:,"month"] = montharr
+        self.data.loc[:,"day"] = dayarr
+        
+        self.data.loc[:,"pang1"] = oh.get_parang(yeararr, montharr, dayarr, timearr, raarr, decarr, longarr1, latarr1, f_el1, f_par1, phi_off1)
+        self.data.loc[:,"pang2"] = oh.get_parang(yeararr, montharr, dayarr, timearr, raarr, decarr, longarr2, latarr2, f_el2, f_par2, phi_off2)          
+        
+        self.data = oh.pd_modifier(self.data)
+
         for i in range(max(self.cnum)):
             self.data["model"+str(i+1)+"_amp"] = self.data["model"+str(i+1)+"_amp"].astype('float64')
             self.data["model"+str(i+1)+"_phas"] = self.data["model"+str(i+1)+"_phas"].astype('float64')
-
-
-
+            
+        
     def get_pol_data(self):
         """
         Make a pandas dataframe containing UV data and models for the D-term estimation with instrumental polarization self-calibration.
         
         """
         
         # If polcalsour == calsour, then don't repeat the procedure and just copy the data array that was already made.
@@ -1436,99 +861,113 @@
             for i in range(max(self.cnum)):
                 del self.pol_data["model"+str(i+1)+"_amp"]
                 del self.pol_data["model"+str(i+1)+"_phas"]
                         
             return
         
         
+        info = oh.basic_info(self.polcalsour, self.direc, self.dataname)
+        
+        self.pol_obsra = info['obsra']
+        self.pol_obsdec = info['obsdec']
+        self.pol_year = info['year']
+        self.pol_month = info['month']
+        self.pol_day = info['day']
+        self.antname = info['antname']
+        self.antx = info['antx']
+        self.anty = info['anty']
+        self.antz = info['antz']
+        self.antmount = info['antmount']
+        self.ifnum = info['ifnum']
+        self.freq = info['freq']
+        self.f_par = info['f_par']
+        self.f_el = info['f_el']
+        self.phi_off = info['phi_off']
+        
+        self.lonarr, self.latarr, self.heightarr = oh.coord(self.antname, self.antx, self.anty, self.antz)
+        
+        self.nant = len(self.antname)
+        
         self.logger.info('\nGetting data for {:d} sources for {:d} IFs...'.format(len(self.polcalsour), self.ifnum))
             
         AIPS.userno = self.aips_userno
         
         if self.aipslog:
             AIPS.log = open(self.logfile, 'a')
         AIPSTask.msgkill = -1
         
-        self.pol_obsra = []
-        self.pol_obsdec = []
-        
-        
-        # Define a pandas dataframe for the data array.
-        pdkey = ["IF", "time", "source", "ant1", "ant2", "u", "v", "pang1", "pang2", \
+        pdkey = ["IF", "year", "month", "day", "time", "source", "ant1", "ant2", "u", "v", "pang1", "pang2", \
                  "rrreal", "rrimag", "rrsigma", "llreal", "llimag", "llsigma", "rlreal", "rlimag", "rlsigma", "lrreal", "lrimag", "lrsigma", \
                  "rramp", "rrphas", "rramp_sigma", "rrphas_sigma", "llamp", "llphas", "llamp_sigma", "llphas_sigma", "rlamp", "rlphas", "rlamp_sigma", "rlphas_sigma", "lramp", "lrphas", "lramp_sigma", "lrphas_sigma", \
                  "qamp", "qphas", "qamp_sigma", "qphas_sigma", "qsigma", "uamp", "uphas", "uamp_sigma", "uphas_sigma", "usigma"]
 
             
         self.pol_data = pd.DataFrame(columns = pdkey)       
         
         
         ifarr, timearr, sourcearr, ant1arr, ant2arr, uarr, varr, rrrealarr, rrimagarr, rrweightarr, llrealarr, llimagarr, llweightarr, rlrealarr, rlimagarr, rlweightarr, lrrealarr, lrimagarr, lrweightarr = \
             [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], [], []
 
 
         for l in range(len(self.polcalsour)):
         
-            inname = self.polcalsour[l]
+            inname = str(self.polcalsour[l])
 
             # Perform additional self-calibration with CALIB if requested.
             if self.selfcal:
                 if not self.polcalsour[l] in self.calsour:
         
                     data = AIPSUVData(inname, 'EDIT', 1, 1)
                     if(data.exists() == True):
                         data.clrstat()
                         data.zap()
                 
-                    self.runfitld(inname, 'EDIT', self.direc+self.dataname+self.polcalsour[l]+'.uvf')
+                    au.runfitld(inname, 'EDIT', self.direc+self.dataname+self.polcalsour[l]+'.uvf')
                     
                     cmap = AIPSImage(inname, 'CMAP', 1, 1)
                     if(cmap.exists() == True):
                         cmap.clrstat()
                         cmap.zap()
                         
-                    self.runfitld(inname, 'CMAP', self.direc+self.dataname+self.polcalsour[l]+'.fits')
+                    au.runfitld(inname, 'CMAP', self.direc+self.dataname+self.polcalsour[l]+'.fits')
                         
                     calib = AIPSUVData(inname, 'CALIB', 1, 1)
                     if(calib.exists() == True):
                         calib.clrstat()
                         calib.zap()
                     
-                    self.runcalib(inname, 'EDIT', 'CALIB', self.solint, self.soltype, self.solmode, self.weightit)
+                    au.runcalib(inname, 'EDIT', inname, 'CMAP', 'CALIB', self.solint, self.soltype, self.solmode, self.weightit)
                     
-                    os.system('rm ' + self.direc + self.dataname + self.polcalsour[l] + '.calib')
-                    self.runfittp(inname, 'CALIB', self.direc + self.dataname + self.polcalsour[l] + '.calib')
+                    if path.exists(self.direc + self.dataname + self.polcalsour[l] + '.calib'):
+                        os.system('rm ' + self.direc + self.dataname + self.polcalsour[l] + '.calib')
+                    au.runfittp(inname, 'CALIB', self.direc + self.dataname + self.polcalsour[l] + '.calib')
                     
                     data.zap()
                     cmap.zap()
-		    calib.zap()
-                    
-		    self.runfitld(inname, 'CALIB', self.direc+self.dataname+self.polcalsour[l]+'.calib')
-
                 
                 else:
                     calib = AIPSUVData(inname, 'CALIB', 1, 1)
                     if(calib.exists() == True):
                         calib.clrstat()
                         calib.zap()
                         
-                    self.runfitld(inname, 'CALIB', self.direc+self.dataname+self.polcalsour[l]+'.calib')
+                    au.runfitld(inname, 'CALIB', self.direc+self.dataname+self.polcalsour[l]+'.calib')
                 
             else:                    
                 calib = AIPSUVData(inname, 'CALIB', 1, 1)
                 if(calib.exists() == True):
                     calib.clrstat()
                     calib.zap()
-                self.runfitld(inname, 'CALIB', self.direc+self.dataname+self.polcalsour[l]+'.uvf')
+                au.runfitld(inname, 'CALIB', self.direc+self.dataname+self.polcalsour[l]+'.uvf')
                 
                     
             calib = WAIPSUVData(inname, 'CALIB', 1, 1)
             
             dumu, dumv, ifname, time, ant1, ant2, rrreal, rrimag, rrweight, llreal, llimag, llweight, rlreal, rlimag, rlweight, lrreal, lrimag, lrweight = \
-                self.uvprt(calib, "all")
+                oh.uvprt(calib, "all")
             
             uarr = uarr + dumu
             varr = varr + dumv
             sourcearr = sourcearr + [self.polcalsour[l]] * len(time)
             ifarr = ifarr + ifname
             timearr = timearr + time
             ant1arr = ant1arr + ant1
@@ -1541,219 +980,63 @@
             llweightarr = llweightarr + llweight
             rlrealarr = rlrealarr + rlreal
             rlimagarr = rlimagarr + rlimag
             rlweightarr = rlweightarr + rlweight
             lrrealarr = lrrealarr + lrreal
             lrimagarr = lrimagarr + lrimag
             lrweightarr = lrweightarr + lrweight
-
-
-            self.pol_obsra.append(calib.header.crval[4])
-            self.pol_obsdec.append(calib.header.crval[5])
-            
-            
+                        
             calib.zap()
 
 
         # Convert the lists to numpy arrays.
         ifarr, timearr, sourcearr, ant1arr, ant2arr, uarr, varr, rrrealarr, rrimagarr, rrweightarr, llrealarr, llimagarr, llweightarr, rlrealarr, rlimagarr, rlweightarr, lrrealarr, lrimagarr, lrweightarr = \
             np.array(ifarr), np.array(timearr), np.array(sourcearr), np.array(ant1arr), np.array(ant2arr), np.array(uarr), np.array(varr), np.array(rrrealarr), np.array(rrimagarr), np.array(rrweightarr), np.array(llrealarr), np.array(llimagarr), np.array(llweightarr), \
             np.array(rlrealarr), np.array(rlimagarr), np.array(rlweightarr), np.array(lrrealarr), np.array(lrimagarr), np.array(lrweightarr)
-       
+        
         rlweightarr[rlweightarr > self.remove_weight_outlier_threshold * np.median(rlweightarr)] = np.median(rlweightarr)
         lrweightarr[lrweightarr > self.remove_weight_outlier_threshold * np.median(lrweightarr)] = np.median(lrweightarr)
         
         # Combine the numpy arrays into a single pandas dataframe.
         self.pol_data.loc[:,"IF"], self.pol_data.loc[:,"time"], self.pol_data.loc[:,"source"], self.pol_data.loc[:,"ant1"], self.pol_data.loc[:,"ant2"], self.pol_data.loc[:,"u"], self.pol_data.loc[:,"v"], \
         self.pol_data.loc[:,"rrreal"], self.pol_data.loc[:,"rrimag"], self.pol_data.loc[:,"rrweight"], self.pol_data.loc[:,"llreal"], self.pol_data.loc[:,"llimag"], self.pol_data.loc[:,"llweight"], \
         self.pol_data.loc[:,"rlreal"], self.pol_data.loc[:,"rlimag"], self.pol_data.loc[:,"rlweight"], self.pol_data.loc[:,"lrreal"], self.pol_data.loc[:,"lrimag"], self.pol_data.loc[:,"lrweight"] = \
                 ifarr, timearr * 24., sourcearr, ant1arr - 1, ant2arr - 1, uarr, varr, rrrealarr, rrimagarr, rrweightarr, llrealarr, llimagarr, llweightarr, rlrealarr, rlimagarr, rlweightarr, lrrealarr, lrimagarr, lrweightarr
         
-
-        self.pol_data.loc[:,"pang1"] = self.get_parang(np.array(self.pol_data["time"]), np.array(self.pol_data["ant1"]), np.array(self.pol_data["source"]), self.polcalsour, self.pol_obsra, self.pol_obsdec)
-        self.pol_data.loc[:,"pang2"] = self.get_parang(np.array(self.pol_data["time"]), np.array(self.pol_data["ant2"]), np.array(self.pol_data["source"]), self.polcalsour, self.pol_obsra, self.pol_obsdec)
-
-
-        # Make new columns for amplitudes, phases, and corresponding errors, etc.
-        self.pol_data.loc[:,"rrsigma"], self.pol_data.loc[:,"llsigma"], self.pol_data.loc[:,"rlsigma"], self.pol_data.loc[:,"lrsigma"] = \
-            1. / self.pol_data.loc[:,"rrweight"] ** (0.5), 1. / self.pol_data.loc[:,"llweight"], 1. / self.pol_data.loc[:,"rlweight"] ** (0.5), 1. / self.pol_data.loc[:,"lrweight"] ** (0.5)
-        
-        self.pol_data.loc[:,"rramp"], self.pol_data.loc[:,"llamp"], self.pol_data.loc[:,"rlamp"], self.pol_data.loc[:,"lramp"] = \
-            np.absolute(self.pol_data.loc[:,"rrreal"] + 1j*self.pol_data.loc[:,"rrimag"]), np.absolute(self.pol_data.loc[:,"llreal"] + 1j*self.pol_data.loc[:,"llimag"]), \
-            np.absolute(self.pol_data.loc[:,"rlreal"] + 1j*self.pol_data.loc[:,"rlimag"]), np.absolute(self.pol_data.loc[:,"lrreal"] + 1j*self.pol_data.loc[:,"lrimag"])
-        
-        self.pol_data.loc[:,"rrphas"], self.pol_data.loc[:,"llphas"], self.pol_data.loc[:,"rlphas"], self.pol_data.loc[:,"lrphas"] = \
-            np.angle(self.pol_data.loc[:,"rrreal"] + 1j*self.pol_data.loc[:,"rrimag"]), np.angle(self.pol_data.loc[:,"llreal"] + 1j*self.pol_data.loc[:,"llimag"]), \
-            np.angle(self.pol_data.loc[:,"rlreal"] + 1j*self.pol_data.loc[:,"rlimag"]), np.angle(self.pol_data.loc[:,"lrreal"] + 1j*self.pol_data.loc[:,"lrimag"])
-        
-        self.pol_data.loc[:,"rramp_sigma"], self.pol_data.loc[:,"llamp_sigma"], self.pol_data.loc[:,"rlamp_sigma"], self.pol_data.loc[:,"lramp_sigma"] = \
-            self.amperror(self.pol_data.loc[:,"rrreal"] + 1j*self.pol_data.loc[:,"rrimag"], self.pol_data.loc[:,"rrsigma"] + 1j*self.pol_data.loc[:,"rrsigma"]), \
-            self.amperror(self.pol_data.loc[:,"llreal"] + 1j*self.pol_data.loc[:,"llimag"], self.pol_data.loc[:,"llsigma"] + 1j*self.pol_data.loc[:,"llsigma"]), \
-            self.amperror(self.pol_data.loc[:,"rlreal"] + 1j*self.pol_data.loc[:,"rlimag"], self.pol_data.loc[:,"rlsigma"] + 1j*self.pol_data.loc[:,"rlsigma"]), \
-            self.amperror(self.pol_data.loc[:,"lrreal"] + 1j*self.pol_data.loc[:,"lrimag"], self.pol_data.loc[:,"lrsigma"] + 1j*self.pol_data.loc[:,"lrsigma"])
-        
-        self.pol_data.loc[:,"rrphas_sigma"], self.pol_data.loc[:,"llphas_sigma"], self.pol_data.loc[:,"rlphas_sigma"], self.pol_data.loc[:,"lrphas_sigma"] = \
-            self.phaserror(self.pol_data.loc[:,"rrreal"] + 1j*self.pol_data.loc[:,"rrimag"], self.pol_data.loc[:,"rrsigma"] + 1j*self.pol_data.loc[:,"rrsigma"]), \
-            self.phaserror(self.pol_data.loc[:,"llreal"] + 1j*self.pol_data.loc[:,"llimag"], self.pol_data.loc[:,"llsigma"] + 1j*self.pol_data.loc[:,"llsigma"]), \
-            self.phaserror(self.pol_data.loc[:,"rlreal"] + 1j*self.pol_data.loc[:,"rlimag"], self.pol_data.loc[:,"rlsigma"] + 1j*self.pol_data.loc[:,"rlsigma"]), \
-            self.phaserror(self.pol_data.loc[:,"lrreal"] + 1j*self.pol_data.loc[:,"lrimag"], self.pol_data.loc[:,"lrsigma"] + 1j*self.pol_data.loc[:,"lrsigma"])
-            
-        
-        dumrl, dumlr = self.pol_data.loc[:,"rlreal"] + 1j*self.pol_data.loc[:,"rlimag"], self.pol_data.loc[:,"lrreal"] + 1j*self.pol_data.loc[:,"lrimag"]
-        dumrlsigma, dumlrsigma = self.pol_data.loc[:,"rlsigma"] + 1j*self.pol_data.loc[:,"rlsigma"], self.pol_data.loc[:,"lrsigma"] + 1j*self.pol_data.loc[:,"lrsigma"]
-        
-        dumq, dumu = (dumrl + dumlr) / 2., -1j * (dumrl - dumlr) / 2.
-        dumqsigma, dumusigma = np.sqrt(dumrlsigma**2 + dumlrsigma**2) / 2., np.sqrt(dumrlsigma**2 + dumlrsigma**2) / 2.
-        
-        self.pol_data.loc[:,"qamp"], self.pol_data.loc[:,"uamp"], self.pol_data.loc[:,"qphas"], self.pol_data.loc[:,"uphas"] = np.absolute(dumq), np.absolute(dumu), np.angle(dumq), np.angle(dumu)
-        self.pol_data.loc[:,"qamp_sigma"], self.pol_data.loc[:,"uamp_sigma"], self.pol_data.loc[:,"qphas_sigma"], self.pol_data.loc[:,"uphas_sigma"] = \
-            self.amperror(dumq, dumqsigma), self.amperror(dumu, dumusigma), self.phaserror(dumq, dumqsigma), self.phaserror(dumu, dumusigma)
-        self.pol_data.loc[:,"qsigma"], self.pol_data.loc[:,"usigma"] = np.real(dumqsigma), np.real(dumusigma)
-
-        self.pol_data["IF"] = self.pol_data["IF"].astype('int32')
-        self.pol_data["ant1"] = self.pol_data["ant1"].astype('int32')
-        self.pol_data["ant2"] = self.pol_data["ant2"].astype('int32')
-
-        
-
-    def get_pol_model(self):
-        """
-        Extract Stokes Q and U visibility models and append them to the pandas dataframe.
-        
-        """
-        
-        self.logger.info('\nGetting source polarization models for {:d} sources for {:d} IFs...'.format(len(self.polcalsour), self.ifnum))
-            
-        AIPS.userno = self.aips_userno
-        
-        if self.aipslog:
-            AIPS.log = open(self.logfile, 'a')
-        AIPSTask.msgkill = -1
-
-        
-        mod_qrealarr, mod_qimagarr, mod_urealarr, mod_uimagarr = [], [], [], []
-        
-        
-        for l in range(len(self.polcalsour)):
+        # Filter bad data points.
+        select = (rrweightarr > 0.) & (llweightarr > 0.) & (rlweightarr > 0.) & (lrweightarr > 0.) & (~np.isnan(rrweightarr)) & (~np.isnan(llweightarr)) & (~np.isnan(rlweightarr)) & (~np.isnan(lrweightarr))
         
-            inname = self.polcalsour[l]
+        self.pol_data = self.pol_data.loc[select].reset_index(drop=True)
         
-            calib = AIPSUVData(inname, 'CALIB', 1, 1)
-            if(calib.exists() == True):
-                calib.clrstat()
-                calib.zap()
-            
+        dumant1 = self.pol_data.loc[:,"ant1"]
+        dumant2 = self.pol_data.loc[:,"ant2"]
+        dumsource = self.pol_data.loc[:,"source"]
                 
-            if self.selfcal: 
-                self.runfitld(inname, 'CALIB', self.direc+self.dataname+self.polcalsour[l]+'.calib')
-            else:
-                self.runfitld(inname, 'CALIB', self.direc+self.dataname+self.polcalsour[l]+'.uvf')
+        longarr1, latarr1, f_el1, f_par1, phi_off1 = oh.coordarr(self.lonarr, self.latarr, self.f_el, self.f_par, self.phi_off, dumant1)
+        longarr2, latarr2, f_el2, f_par2, phi_off2 = oh.coordarr(self.lonarr, self.latarr, self.f_el, self.f_par, self.phi_off, dumant2)
         
-                
-            calib = AIPSUVData(inname, 'CALIB', 1, 1)
-           
-
-            for k in range(self.ifnum):
+        yeararr, montharr, dayarr, raarr, decarr = oh.calendar(dumsource, self.polcalsour, self.pol_year, self.pol_month, self.pol_day, self.pol_obsra, self.pol_obsdec)
         
-                qmap = AIPSUVData(inname, 'QMAP', 1, 1)
-                if(qmap.exists() == True):
-                    qmap.clrstat()
-                    qmap.zap()
-                
-                if not path.exists(self.direc+self.dataname+self.polcalsour[l]+'.IF'+str(k+1)+'.q.fits'):
-		    dum = 0
-            	    calib = WAIPSUVData(inname, 'CALIB', 1, 1)
-        	    for visibility in calib:
-            		if((visibility.visibility[k,0,0,2] <= 0) | (visibility.visibility[k,0,1,2] <= 0) | (visibility.visibility[k,0,2,2] <= 0) | (visibility.visibility[k,0,3,2] <= 0)): continue
-                	dum += 1
-
-                    mod_qrealarr = mod_qrealarr + [0.] * dum
-                    mod_qimagarr = mod_qimagarr + [0.] * dum
-
-            	    calib = AIPSUVData(inname, 'CALIB', 1, 1)
-	        else:
-                # Load the Stokes Q CLEAN models of the calibrators. Note that the Difmap files are saved after selecting Stokes I because AIPS UVSUB cannot handle models other than Stokes I.
-                    self.runfitld(inname, 'QMAP', self.direc+self.dataname+self.polcalsour[l]+'.IF'+str(k+1)+'.q.fits')
-                    qmap = AIPSImage(inname, 'QMAP', 1, 1)     
-                
-                    uvsub = AIPSUVData(inname, 'UVSUB', 1, 1)
-                    if(uvsub.exists() == True):
-                        uvsub.clrstat()
-                        uvsub.zap()
-                
-                    self.runuvsub(inname, 'CALIB', 'QMAP', 1, 1)
-                
-                
-                    moddata = WAIPSUVData(inname, 'UVSUB', 1, 1)
-                    mod_qreal, mod_qimag = self.pol_model_uvprt(moddata, k, "all")
-                
-                    mod_qrealarr = mod_qrealarr + mod_qreal
-                    mod_qimagarr = mod_qimagarr + mod_qimag
-              
-                    moddata.zap()
-                    qmap.zap()
-        
-                
-		umap = AIPSUVData(inname, 'UMAP', 1, 1)
-                if(umap.exists() == True):
-                    umap.clrstat()
-                    umap.zap()
-                
-                
-		if not path.exists(self.direc+self.dataname+self.polcalsour[l]+'.IF'+str(k+1)+'.u.fits'):
-            	    calib = WAIPSUVData(inname, 'CALIB', 1, 1)
-		    dum = 0
-        	    for visibility in calib:
-            		if((visibility.visibility[k,0,0,2] <= 0) | (visibility.visibility[k,0,1,2] <= 0) | (visibility.visibility[k,0,2,2] <= 0) | (visibility.visibility[k,0,3,2] <= 0)): continue
-                	dum += 1
-
-                    mod_urealarr = mod_urealarr + [0.] * dum
-                    mod_uimagarr = mod_uimagarr + [0.] * dum
-            	    calib = AIPSUVData(inname, 'CALIB', 1, 1)
-               
-                # Load the Stokes U CLEAN models of the calibrators. Note that the Difmap files are saved after selecting Stokes I because AIPS UVSUB cannot handle models other than Stokes I.
-	        else:
-		    self.runfitld(inname, 'UMAP', self.direc+self.dataname+self.polcalsour[l]+'.IF'+str(k+1)+'.u.fits')    
-                    umap = AIPSImage(inname, 'UMAP', 1, 1)
-                
-                    uvsub = AIPSUVData(inname, 'UVSUB', 1, 1)
-                    if(uvsub.exists() == True):
-                        uvsub.clrstat()
-                        uvsub.zap()
-                    
-                    self.runuvsub(inname, 'CALIB', 'UMAP', 1, 1)
-                
-                
-                    moddata = WAIPSUVData(inname, 'UVSUB', 1, 1)
-                    mod_ureal, mod_uimag = self.pol_model_uvprt(moddata, k, "all")
-                
-                    mod_urealarr = mod_urealarr + mod_ureal
-                    mod_uimagarr = mod_uimagarr + mod_uimag
-                
-            
-                    moddata.zap()
-                    umap.zap()
-                
-            calib.zap()
-
+        timearr = np.array(self.pol_data.loc[:,"time"])
         
-        mod_qreal, mod_qimag, mod_ureal, mod_uimag = np.array(mod_qrealarr), np.array(mod_qimagarr), np.array(mod_urealarr), np.array(mod_uimagarr)
+        for i in range(10):
+            dayarr[timearr>=24.] += 1
+            timearr[timearr>=24.] -= 24.
         
+        self.pol_data.loc[:,"time"] = timearr
+        self.pol_data.loc[:,"year"] = yeararr
+        self.pol_data.loc[:,"month"] = montharr
+        self.pol_data.loc[:,"day"] = dayarr
         
-        mod_q, mod_u = mod_qreal + 1j*mod_qimag, mod_ureal + 1j*mod_uimag
-        mod_rlreal, mod_rlimag, mod_lrreal, mod_lrimag = np.real(mod_q + 1j*mod_u), np.imag(mod_q + 1j*mod_u), np.real(mod_q - 1j*mod_u), np.imag(mod_q - 1j*mod_u)
-        mod_rlamp, mod_rlphas, mod_lramp, mod_lrphas = np.absolute(mod_rlreal + 1j*mod_rlimag), np.angle(mod_rlreal + 1j*mod_rlimag), np.absolute(mod_lrreal + 1j*mod_lrimag), np.angle(mod_lrreal + 1j*mod_lrimag)
-        mod_qamp, mod_qphas, mod_uamp, mod_uphas = np.absolute(mod_q), np.angle(mod_q), np.absolute(mod_u), np.angle(mod_u)
+        self.pol_data.loc[:,"pang1"] = oh.get_parang(yeararr, montharr, dayarr, timearr, raarr, decarr, longarr1, latarr1, f_el1, f_par1, phi_off1)
+        self.pol_data.loc[:,"pang2"] = oh.get_parang(yeararr, montharr, dayarr, timearr, raarr, decarr, longarr2, latarr2, f_el2, f_par2, phi_off2)
+
+        self.pol_data = oh.pd_modifier(self.pol_data)
         
 
-        # Append the model visibilities to the existing pandas dataframe as new columns.
-        self.pol_data.loc[:,"model_rlreal"], self.pol_data.loc[:,"model_rlimag"], self.pol_data.loc[:,"model_lrreal"], self.pol_data.loc[:,"model_lrimag"], \
-        self.pol_data.loc[:,"model_rlamp"], self.pol_data.loc[:,"model_rlphas"], self.pol_data.loc[:,"model_lramp"], self.pol_data.loc[:,"model_lrphas"], \
-        self.pol_data.loc[:,"model_qamp"], self.pol_data.loc[:,"model_qphas"], self.pol_data.loc[:,"model_uamp"], self.pol_data.loc[:,"model_uphas"] = \
-        mod_rlreal, mod_rlimag, mod_lrreal, mod_lrimag, mod_rlamp, mod_rlphas, mod_lramp, mod_lrphas, mod_qamp, mod_qphas, mod_uamp, mod_uphas
 
 
     def parangplot(self, k, nant, antname, source, time, ant1, ant2, sourcearr, pang1, pang2, filename):
         """
         Draw field-rotation angle plots.
         
         Args:
@@ -2012,15 +1295,15 @@
         second_q, second_u = (second_rl + second_lr) / 2., -1j * (second_rl - second_lr) / 2.
         second_qamp, second_qphas, second_uamp, second_uphas = np.absolute(second_q), np.angle(second_q), np.absolute(second_u), np.angle(second_u)
 
         
         if(comp == 'pol'): return pol_qamp, pol_qphas, pol_uamp, pol_uphas
         if(comp == 'dterm'): return dterm_qamp, dterm_qphas, dterm_uamp, dterm_uphas
         if(comp == 'second'): return second_qamp, second_qphas, second_uamp, second_uphas
-        
+
 
 
     def zbl_deq(self, x, *p):
         """
         The D-term models for the zero-baseline D-term estimation.
         
         Args:
@@ -2203,372 +1486,277 @@
         
         if(comp == 'pol'): return pol_qamp, pol_qphas, pol_uamp, pol_uphas
         if(comp == 'dterm'): return dterm_qamp, dterm_qphas, dterm_uamp, dterm_uphas
         if(comp == 'second'): return second_qamp, second_qphas, second_uamp, second_uphas
         
 
 
-    def pol_deq(self, x, *p):
+    def pol_deq(self, parmset, *p):
         """
         The D-term models for the D-term estimation with instrumental polarization self-calibration.
         
         Args:
             x: dummy parameters (not to be used).
             *p (args): the best-fit parameters args.
         """
         
-        RiLj_Real = np.zeros(len(self.pang1))
-        RiLj_Imag = np.zeros(len(self.pang1))
-        LiRj_Real = np.zeros(len(self.pang1))
-        LiRj_Imag = np.zeros(len(self.pang1))
+        (nant, polcalsour, sourcearr, pang1, pang2, ant1, ant2, model_rlreal, model_rlimag, model_lrreal, model_lrimag, rramp, rrphas, llamp, llphas) = parmset
+        
+        model_rlamp = np.abs(model_rlreal + 1j * model_rlimag)
+        model_rlphas = np.angle(model_rlreal + 1j * model_rlimag)
+        model_lramp = np.abs(model_lrreal + 1j * model_lrimag)
+        model_lrphas = np.angle(model_lrreal + 1j * model_lrimag)
+        
+        
+        RiLj_Real = np.zeros(len(pang1))
+        RiLj_Imag = np.zeros(len(pang1))
+        LiRj_Real = np.zeros(len(pang1))
+        LiRj_Imag = np.zeros(len(pang1))
         
         
         dump = np.array(p)
         
-        dumreal = dump[2*self.ant1]
-        dumimag = dump[2*self.ant1 + 1]
+        dumreal = dump[2*ant1]
+        dumimag = dump[2*ant1 + 1]
         Tot_D_iR_amp = np.absolute(dumreal + 1j * dumimag)
         Tot_D_iR_phas = np.angle(dumreal + 1j*dumimag)
 
-        dumreal = dump[2*self.nant + 2*self.ant2]
-        dumimag = dump[2*self.nant + 2*self.ant2 + 1]
+        dumreal = dump[2*nant + 2*ant2]
+        dumimag = dump[2*nant + 2*ant2 + 1]
         Tot_D_jL_amp = np.absolute(dumreal + 1j * dumimag)
         Tot_D_jL_phas = np.angle(dumreal + 1j*dumimag)
         
-        dumreal = dump[2*self.nant + 2*self.ant1]
-        dumimag = dump[2*self.nant + 2*self.ant1 + 1]
+        dumreal = dump[2*nant + 2*ant1]
+        dumimag = dump[2*nant + 2*ant1 + 1]
         Tot_D_iL_amp = np.absolute(dumreal + 1j * dumimag)
         Tot_D_iL_phas = np.angle(dumreal + 1j*dumimag)
         
-        dumreal = dump[2*self.ant2]
-        dumimag = dump[2*self.ant2 + 1]
+        dumreal = dump[2*ant2]
+        dumimag = dump[2*ant2 + 1]
         Tot_D_jR_amp = np.absolute(dumreal + 1j * dumimag)
         Tot_D_jR_phas = np.angle(dumreal + 1j*dumimag)
         
         
-        for l in range(len(self.polcalsour)):
+        for l in range(len(polcalsour)):
         
-            select = (self.sourcearr == self.polcalsour[l])
+            select = (sourcearr == polcalsour[l])
             
-            RiLj_Real[select] += self.model_rlreal[select] + \
-              Tot_D_iR_amp[select] * Tot_D_jL_amp[select] * self.model_lramp[select] * np.cos(self.model_lrphas[select] + Tot_D_iR_phas[select] - Tot_D_jL_phas[select] + 2. * (self.pang1[select] + self.pang2[select]))
+            RiLj_Real[select] += model_rlreal[select] + \
+              Tot_D_iR_amp[select] * Tot_D_jL_amp[select] * model_lramp[select] * np.cos(model_lrphas[select] + Tot_D_iR_phas[select] - Tot_D_jL_phas[select] + 2. * (pang1[select] + pang2[select]))
     
-            RiLj_Imag[select] += self.model_rlimag[select] + \
-              Tot_D_iR_amp[select] * Tot_D_jL_amp[select] * self.model_lramp[select] * np.sin(self.model_lrphas[select] + Tot_D_iR_phas[select] - Tot_D_jL_phas[select] + 2. * (self.pang1[select] + self.pang2[select]))
+            RiLj_Imag[select] += model_rlimag[select] + \
+              Tot_D_iR_amp[select] * Tot_D_jL_amp[select] * model_lramp[select] * np.sin(model_lrphas[select] + Tot_D_iR_phas[select] - Tot_D_jL_phas[select] + 2. * (pang1[select] + pang2[select]))
     
-            LiRj_Real[select] += self.model_lrreal[select] + \
-              Tot_D_iL_amp[select] * Tot_D_jR_amp[select] * self.model_rlamp[select] * np.cos(self.model_rlphas[select] + Tot_D_iL_phas[select] - Tot_D_jR_phas[select] - 2. * (self.pang1[select] + self.pang2[select]))
+            LiRj_Real[select] += model_lrreal[select] + \
+              Tot_D_iL_amp[select] * Tot_D_jR_amp[select] * model_rlamp[select] * np.cos(model_rlphas[select] + Tot_D_iL_phas[select] - Tot_D_jR_phas[select] - 2. * (pang1[select] + pang2[select]))
     
-            LiRj_Imag[select] += self.model_lrimag[select] + \
-              Tot_D_iL_amp[select] * Tot_D_jR_amp[select] * self.model_rlamp[select] * np.sin(self.model_rlphas[select] + Tot_D_iL_phas[select] - Tot_D_jR_phas[select] - 2. * (self.pang1[select] + self.pang2[select]))
+            LiRj_Imag[select] += model_lrimag[select] + \
+              Tot_D_iL_amp[select] * Tot_D_jR_amp[select] * model_rlamp[select] * np.sin(model_rlphas[select] + Tot_D_iL_phas[select] - Tot_D_jR_phas[select] - 2. * (pang1[select] + pang2[select]))
             
             
         RiLj_Real += \
-          Tot_D_iR_amp * self.llamp * np.cos(Tot_D_iR_phas + self.llphas + 2. * self.pang1) + \
-          Tot_D_jL_amp * self.rramp * np.cos(-Tot_D_jL_phas + self.rrphas + 2. * self.pang2)
+          Tot_D_iR_amp * llamp * np.cos(Tot_D_iR_phas + llphas + 2. * pang1) + \
+          Tot_D_jL_amp * rramp * np.cos(-Tot_D_jL_phas + rrphas + 2. * pang2)
         
         RiLj_Imag += \
-          Tot_D_iR_amp * self.llamp * np.sin(Tot_D_iR_phas + self.llphas + 2. * self.pang1) + \
-          Tot_D_jL_amp * self.rramp * np.sin(-Tot_D_jL_phas + self.rrphas + 2. * self.pang2)
+          Tot_D_iR_amp * llamp * np.sin(Tot_D_iR_phas + llphas + 2. * pang1) + \
+          Tot_D_jL_amp * rramp * np.sin(-Tot_D_jL_phas + rrphas + 2. * pang2)
     
         LiRj_Real += \
-          Tot_D_iL_amp * self.rramp * np.cos(Tot_D_iL_phas + self.rrphas - 2. * self.pang1) + \
-          Tot_D_jR_amp * self.llamp * np.cos(-Tot_D_jR_phas + self.llphas - 2. * self.pang2)
+          Tot_D_iL_amp * rramp * np.cos(Tot_D_iL_phas + rrphas - 2. * pang1) + \
+          Tot_D_jR_amp * llamp * np.cos(-Tot_D_jR_phas + llphas - 2. * pang2)
     
         LiRj_Imag += \
-          Tot_D_iL_amp * self.rramp * np.sin(Tot_D_iL_phas + self.rrphas - 2. * self.pang1) + \
-          Tot_D_jR_amp * self.llamp * np.sin(-Tot_D_jR_phas + self.llphas - 2. * self.pang2)  
+          Tot_D_iL_amp * rramp * np.sin(Tot_D_iL_phas + rrphas - 2. * pang1) + \
+          Tot_D_jR_amp * llamp * np.sin(-Tot_D_jR_phas + llphas - 2. * pang2)  
        
     
         compv = np.concatenate([LiRj_Real, LiRj_Imag, RiLj_Real, RiLj_Imag])
         
         return compv
 
 
-
-    def pol_deq_comp(self, comp, *p):
+    def pol_deq_comp(self, comp, parmset, *p):
         """
         Extract component-wise best-fit models with instrumental polarization self-calibration.
         
         Args:
             comp (str): the name of the component to be extracted.
             *p (args): the best-fit parameters args.
         """
         
-        pol_RiLj_Real = np.zeros(len(self.pang1))
-        pol_RiLj_Imag = np.zeros(len(self.pang1))
-        pol_LiRj_Real = np.zeros(len(self.pang1))
-        pol_LiRj_Imag = np.zeros(len(self.pang1))
+        (nant, polcalsour, sourcearr, pang1, pang2, ant1, ant2, model_rlreal, model_rlimag, model_lrreal, model_lrimag, rramp, rrphas, llamp, llphas) = parmset
         
-        dterm_RiLj_Real = np.zeros(len(self.pang1))
-        dterm_RiLj_Imag = np.zeros(len(self.pang1))
-        dterm_LiRj_Real = np.zeros(len(self.pang1))
-        dterm_LiRj_Imag = np.zeros(len(self.pang1))
-        
-        second_RiLj_Real = np.zeros(len(self.pang1))
-        second_RiLj_Imag = np.zeros(len(self.pang1))
-        second_LiRj_Real = np.zeros(len(self.pang1))
-        second_LiRj_Imag = np.zeros(len(self.pang1))
+        model_rlamp = np.abs(model_rlreal + 1j * model_rlimag)
+        model_rlphas = np.angle(model_rlreal + 1j * model_rlimag)
+        model_lramp = np.abs(model_lrreal + 1j * model_lrimag)
+        model_lrphas = np.angle(model_lrreal + 1j * model_lrimag)
+        
+        
+        pol_RiLj_Real = np.zeros(len(pang1))
+        pol_RiLj_Imag = np.zeros(len(pang1))
+        pol_LiRj_Real = np.zeros(len(pang1))
+        pol_LiRj_Imag = np.zeros(len(pang1))
+        
+        dterm_RiLj_Real = np.zeros(len(pang1))
+        dterm_RiLj_Imag = np.zeros(len(pang1))
+        dterm_LiRj_Real = np.zeros(len(pang1))
+        dterm_LiRj_Imag = np.zeros(len(pang1))
+        
+        second_RiLj_Real = np.zeros(len(pang1))
+        second_RiLj_Imag = np.zeros(len(pang1))
+        second_LiRj_Real = np.zeros(len(pang1))
+        second_LiRj_Imag = np.zeros(len(pang1))
         
         
         dump = np.array(p)
         
         
-        dumreal = np.array([dump[2*int(s)] for s in self.ant1])
-        dumimag = np.array([dump[2*int(s)+1] for s in self.ant1])
+        dumreal = np.array([dump[2*int(s)] for s in ant1])
+        dumimag = np.array([dump[2*int(s)+1] for s in ant1])
         Tot_D_iR_amp = np.sqrt(dumreal**2 + dumimag**2)
         Tot_D_iR_phas = np.angle(dumreal + 1j*dumimag)
     
-        dumreal = np.array([dump[2*self.nant + 2*int(s)] for s in self.ant2])
-        dumimag = np.array([dump[2*self.nant + 2*int(s)+1] for s in self.ant2])
+        dumreal = np.array([dump[2*nant + 2*int(s)] for s in ant2])
+        dumimag = np.array([dump[2*nant + 2*int(s)+1] for s in ant2])
         Tot_D_jL_amp = np.sqrt(dumreal**2 + dumimag**2)
         Tot_D_jL_phas = np.angle(dumreal + 1j*dumimag)
     
     
-        dumreal = np.array([dump[2*self.nant + 2*int(s)] for s in self.ant1])
-        dumimag = np.array([dump[2*self.nant + 2*int(s)+1] for s in self.ant1])
+        dumreal = np.array([dump[2*nant + 2*int(s)] for s in ant1])
+        dumimag = np.array([dump[2*nant + 2*int(s)+1] for s in ant1])
         Tot_D_iL_amp = np.sqrt(dumreal**2 + dumimag**2)
         Tot_D_iL_phas = np.angle(dumreal + 1j*dumimag)
     
     
-        dumreal = np.array([dump[2*int(s)] for s in self.ant2])
-        dumimag = np.array([dump[2*int(s)+1] for s in self.ant2])
+        dumreal = np.array([dump[2*int(s)] for s in ant2])
+        dumimag = np.array([dump[2*int(s)+1] for s in ant2])
         Tot_D_jR_amp = np.sqrt(dumreal**2 + dumimag**2)
         Tot_D_jR_phas = np.angle(dumreal + 1j*dumimag)
         
     
-        for l in range(len(self.polcalsour)):
+        for l in range(len(polcalsour)):
           
-            select = (self.sourcearr == self.polcalsour[l])
+            select = (sourcearr == polcalsour[l])
             
-            pol_RiLj_Real[select] += self.model_rlreal[select]
-            pol_RiLj_Imag[select] += self.model_rlimag[select]
-            pol_LiRj_Real[select] += self.model_lrreal[select]
-            pol_LiRj_Imag[select] += self.model_lrimag[select]
-            
-            second_RiLj_Real[select] += Tot_D_iR_amp[select] * Tot_D_jL_amp[select] * self.model_rlamp[select] * np.cos(self.model_rlphas[select] + Tot_D_iR_phas[select] - Tot_D_jL_phas[select] + 2. * (self.pang1[select] + self.pang2[select]))
-            second_RiLj_Imag[select] += Tot_D_iR_amp[select] * Tot_D_jL_amp[select] * self.model_rlamp[select] * np.sin(self.model_rlphas[select] + Tot_D_iR_phas[select] - Tot_D_jL_phas[select] + 2. * (self.pang1[select] + self.pang2[select]))
-            second_LiRj_Real[select] += Tot_D_iL_amp[select] * Tot_D_jR_amp[select] * self.model_lramp[select] * np.cos(self.model_lrphas[select] + Tot_D_iL_phas[select] - Tot_D_jR_phas[select] - 2. * (self.pang1[select] + self.pang2[select]))
-            second_LiRj_Imag[select] += Tot_D_iL_amp[select] * Tot_D_jR_amp[select] * self.model_lramp[select] * np.sin(self.model_lrphas[select] + Tot_D_iL_phas[select] - Tot_D_jR_phas[select] - 2. * (self.pang1[select] + self.pang2[select]))
+            pol_RiLj_Real[select] += model_rlreal[select]
+            pol_RiLj_Imag[select] += model_rlimag[select]
+            pol_LiRj_Real[select] += model_lrreal[select]
+            pol_LiRj_Imag[select] += model_lrimag[select]
+            
+            second_RiLj_Real[select] += Tot_D_iR_amp[select] * Tot_D_jL_amp[select] * model_rlamp[select] * np.cos(model_rlphas[select] + Tot_D_iR_phas[select] - Tot_D_jL_phas[select] + 2. * (pang1[select] + pang2[select]))
+            second_RiLj_Imag[select] += Tot_D_iR_amp[select] * Tot_D_jL_amp[select] * model_rlamp[select] * np.sin(model_rlphas[select] + Tot_D_iR_phas[select] - Tot_D_jL_phas[select] + 2. * (pang1[select] + pang2[select]))
+            second_LiRj_Real[select] += Tot_D_iL_amp[select] * Tot_D_jR_amp[select] * model_lramp[select] * np.cos(model_lrphas[select] + Tot_D_iL_phas[select] - Tot_D_jR_phas[select] - 2. * (pang1[select] + pang2[select]))
+            second_LiRj_Imag[select] += Tot_D_iL_amp[select] * Tot_D_jR_amp[select] * model_lramp[select] * np.sin(model_lrphas[select] + Tot_D_iL_phas[select] - Tot_D_jR_phas[select] - 2. * (pang1[select] + pang2[select]))
               
             
-        dterm_RiLj_Real += Tot_D_iR_amp * self.llamp * np.cos(Tot_D_iR_phas + self.llphas + 2. * self.pang1) + Tot_D_jL_amp * self.rramp * np.cos(-Tot_D_jL_phas + self.rrphas + 2. * self.pang2)
-        dterm_RiLj_Imag += Tot_D_iR_amp * self.llamp * np.sin(Tot_D_iR_phas + self.llphas + 2. * self.pang1) + Tot_D_jL_amp * self.rramp * np.sin(-Tot_D_jL_phas + self.rrphas + 2. * self.pang2)
-        dterm_LiRj_Real += Tot_D_iL_amp * self.rramp * np.cos(Tot_D_iL_phas + self.rrphas - 2. * self.pang1) + Tot_D_jR_amp * self.llamp * np.cos(-Tot_D_jR_phas + self.llphas - 2. * self.pang2)
-        dterm_LiRj_Imag += Tot_D_iL_amp * self.rramp * np.sin(Tot_D_iL_phas + self.rrphas - 2. * self.pang1) + Tot_D_jR_amp * self.llamp * np.sin(-Tot_D_jR_phas + self.llphas - 2. * self.pang2)  
+        dterm_RiLj_Real += Tot_D_iR_amp * llamp * np.cos(Tot_D_iR_phas + llphas + 2. * pang1) + Tot_D_jL_amp * rramp * np.cos(-Tot_D_jL_phas + rrphas + 2. * pang2)
+        dterm_RiLj_Imag += Tot_D_iR_amp * llamp * np.sin(Tot_D_iR_phas + llphas + 2. * pang1) + Tot_D_jL_amp * rramp * np.sin(-Tot_D_jL_phas + rrphas + 2. * pang2)
+        dterm_LiRj_Real += Tot_D_iL_amp * rramp * np.cos(Tot_D_iL_phas + rrphas - 2. * pang1) + Tot_D_jR_amp * llamp * np.cos(-Tot_D_jR_phas + llphas - 2. * pang2)
+        dterm_LiRj_Imag += Tot_D_iL_amp * rramp * np.sin(Tot_D_iL_phas + rrphas - 2. * pang1) + Tot_D_jR_amp * llamp * np.sin(-Tot_D_jR_phas + llphas - 2. * pang2)  
 
 
         pol_rl, pol_lr = pol_RiLj_Real + 1j * pol_RiLj_Imag, pol_LiRj_Real + 1j * pol_LiRj_Imag
         pol_q, pol_u = (pol_rl + pol_lr) / 2., -1j * (pol_rl - pol_lr) / 2.
         pol_qamp, pol_qphas, pol_uamp, pol_uphas = np.absolute(pol_q), np.angle(pol_q), np.absolute(pol_u), np.angle(pol_u)
         
         dterm_rl, dterm_lr = dterm_RiLj_Real + 1j * dterm_RiLj_Imag, dterm_LiRj_Real + 1j * dterm_LiRj_Imag
         dterm_q, dterm_u = (dterm_rl + dterm_lr) / 2., -1j * (dterm_rl - dterm_lr) / 2.
         dterm_qamp, dterm_qphas, dterm_uamp, dterm_uphas = np.absolute(dterm_q), np.angle(dterm_q), np.absolute(dterm_u), np.angle(dterm_u)
         
         second_rl, second_lr = second_RiLj_Real + 1j * second_RiLj_Imag, second_LiRj_Real + 1j * second_LiRj_Imag
         second_q, second_u = (second_rl + second_lr) / 2., -1j * (second_rl - second_lr) / 2.
         second_qamp, second_qphas, second_uamp, second_uphas = np.absolute(second_q), np.angle(second_q), np.absolute(second_u), np.angle(second_u)
 
-        
+
         if(comp == 'pol'): return pol_qamp, pol_qphas, pol_uamp, pol_uphas
         if(comp == 'dterm'): return dterm_qamp, dterm_qphas, dterm_uamp, dterm_uphas
         if(comp == 'second'): return second_qamp, second_qphas, second_uamp, second_uphas
 
 
-    def visualplot(self, k, nant, antname, source, time, ant1, ant2, sourcearr, qamp, qphas, uamp, uphas, qamp_sigma, qphas_sigma, uamp_sigma, uphas_sigma, \
-                   mod_pol_qamp, mod_pol_qphas, mod_pol_uamp, mod_pol_uphas, mod_dterm_qamp, mod_dterm_qphas, mod_dterm_uamp, mod_dterm_uphas, mod_second_qamp, mod_second_qphas, mod_second_uamp, mod_second_uphas, \
-                   dumfit, Iteration, filename):
+    def dum_deq(self, x, *p):
         """
-        Draw vplots.
-        """        
+        The D-term models for the D-term estimation with instrumental polarization self-calibration.
         
-        mod_lr, mod_rl = dumfit[0:len(time)] + 1j*dumfit[len(time):len(time)*2], dumfit[len(time)*2:len(time)*3] + 1j*dumfit[len(time)*3:len(time)*4]
-        mod_q, mod_u = (mod_rl + mod_lr) / 2., -1j * (mod_rl - mod_lr) / 2.
-        mod_qamp, mod_qphas, mod_uamp, mod_uphas = np.absolute(mod_q), np.angle(mod_q), np.absolute(mod_u), np.angle(mod_u)
+        Args:
+            x: dummy parameters (not to be used).
+            *p (args): the best-fit parameters args.
+        """
         
+        RiLj_Real = np.zeros(len(self.pang1))
+        RiLj_Imag = np.zeros(len(self.pang1))
+        LiRj_Real = np.zeros(len(self.pang1))
+        LiRj_Imag = np.zeros(len(self.pang1))
         
-        for m in range(nant):
-            
-            for n in range(nant):
-                if(m==n):
-                    continue
-                dumm = m
-                dumn = n
-                if(m>n):
-                    dumm = n
-                    dumn = m
-                        
-                figure, axes = plt.subplots(2, sharex=True, gridspec_kw={'hspace': 0}, figsize=(10, 8))
         
-                for ax in axes.flat:
-                    ax.tick_params(length=6, width=2,which = 'major')
-                    ax.tick_params(length=4, width=1.5,which = 'minor')
+        dump = np.array(p)
         
-                axes[0].set_xlim(np.min(time) - (np.max(time) - np.min(time)) * 0.3, np.max(time) + (np.max(time) - np.min(time)) * 0.1)
-                axes[1].set_xlim(np.min(time) - (np.max(time) - np.min(time)) * 0.3, np.max(time) + (np.max(time) - np.min(time)) * 0.1)
-                axes[1].set_ylim(-180, 180)
-                
-                axes[1].set(xlabel = 'Time (UT)')
-                
-                axes[0].set(ylabel = 'Amplitude (Jy)')
-                axes[1].set(ylabel = 'Phase (deg)')
-                
-                axes[0].set_title(self.dataname)
-
-                axes[0].annotate('Stokes Q', xy=(1, 1), xycoords = 'axes fraction', xytext = (-25, -25), size = 24, textcoords='offset pixels', horizontalalignment='right', verticalalignment='top')
-                
-                axes[1].annotate(self.antname[dumm] + '-' + self.antname[dumn], xy=(0, 0), xycoords = 'axes fraction', xytext = (25, 25), size = 24, textcoords='offset pixels', horizontalalignment='left', verticalalignment='bottom')
-                axes[1].annotate('IF {:d}'.format(k+1), xy = (0, 1), xycoords = 'axes fraction', xytext = (25, -25), size = 24, textcoords='offset pixels', horizontalalignment='left', verticalalignment='top')
-
-
-                dumx, dumy1, dumy2 = np.empty([0]), np.empty([0]), np.empty([0])
-                
-                
-                for l in range(len(source)):
-                    
-                    select = (ant1 == dumm) & (ant2 == dumn) & (sourcearr == source[l])
-                    
-                    dumx = np.append(dumx, time[select])
-                    dumy1 = np.append(dumy1, mod_qamp[select])
-                    dumy2 = np.append(dumy2, np.degrees(mod_qphas[select]))
+        dumreal = dump[2*self.ant1]
+        dumimag = dump[2*self.ant1 + 1]
+        Tot_D_iR_amp = np.absolute(dumreal + 1j * dumimag)
+        Tot_D_iR_phas = np.angle(dumreal + 1j*dumimag)
 
-                    if(len(dumx) == 0): continue
-                
-                    axes[0].errorbar(time[select], qamp[select], qamp_sigma[select], fmt = 'o', markerfacecolor = 'None', markeredgecolor = self.colors[l], ecolor = self.colors[l], label = source[l].upper(), zorder = 0)
-                    axes[1].errorbar(time[select], np.degrees(qphas[select]), np.degrees(qphas_sigma[select]), fmt = 'o', markerfacecolor = 'None', markeredgecolor = self.colors[l], ecolor = self.colors[l], zorder = 0)
-                    
-                    if self.allplot:
-                        axes[0].plot(time[select], mod_pol_qamp[select], color = self.colors[l], linestyle = '--')
-                        axes[1].plot(time[select], np.degrees(mod_pol_qphas[select]), color = self.colors[l], linestyle = '--')
-                        
-                        axes[0].plot(time[select], mod_dterm_qamp[select], color = self.colors[l], linestyle = ':')
-                        axes[1].plot(time[select], np.degrees(mod_dterm_qphas[select]), color = self.colors[l], linestyle = ':')
-                
-                
-                if(len(dumx) == 0): continue
+        dumreal = dump[2*self.nant + 2*self.ant2]
+        dumimag = dump[2*self.nant + 2*self.ant2 + 1]
+        Tot_D_jL_amp = np.absolute(dumreal + 1j * dumimag)
+        Tot_D_jL_phas = np.angle(dumreal + 1j*dumimag)
+        
+        dumreal = dump[2*self.nant + 2*self.ant1]
+        dumimag = dump[2*self.nant + 2*self.ant1 + 1]
+        Tot_D_iL_amp = np.absolute(dumreal + 1j * dumimag)
+        Tot_D_iL_phas = np.angle(dumreal + 1j*dumimag)
+        
+        dumreal = dump[2*self.ant2]
+        dumimag = dump[2*self.ant2 + 1]
+        Tot_D_jR_amp = np.absolute(dumreal + 1j * dumimag)
+        Tot_D_jR_phas = np.angle(dumreal + 1j*dumimag)
+        
+        
+        for l in range(len(self.timecalsour)):
+        
+            select = (self.sourcearr == self.timecalsour[l])
+            
+            RiLj_Real[select] += self.model_rlreal[select] + \
+              Tot_D_iR_amp[select] * Tot_D_jL_amp[select] * self.model_lramp[select] * np.cos(self.model_lrphas[select] + Tot_D_iR_phas[select] - Tot_D_jL_phas[select] + 2. * (self.pang1[select] + self.pang2[select]))
     
-                           
-                axes[0].legend(loc='upper left', fontsize = 18 - int(len(source)/2.), frameon=False, markerfirst=True, handlelength=1.0)
-                
-                dumx = np.array(dumx)
-                
-                argsort = np.argsort(dumx)
-                
-                axes[0].plot(dumx[argsort], dumy1[argsort], color = 'magenta')
-                if self.allplot:
-                    axes[1].plot(dumx[argsort], dumy2[argsort], color = 'magenta', label = 'whole terms')
-                    
-                    axes[1].plot(np.nan, np.nan, color = 'black', linestyle = '--', label = 'source pol')
-                    axes[1].plot(np.nan, np.nan, color = 'black', linestyle = ':', label = 'd-terms')
+            RiLj_Imag[select] += self.model_rlimag[select] + \
+              Tot_D_iR_amp[select] * Tot_D_jL_amp[select] * self.model_lramp[select] * np.sin(self.model_lrphas[select] + Tot_D_iR_phas[select] - Tot_D_jL_phas[select] + 2. * (self.pang1[select] + self.pang2[select]))
     
-                    axes[1].legend(loc = 'upper left', frameon=False, fontsize = 16, handlelength=1.0)
-                else:
-                    axes[1].plot(dumx[argsort], dumy2[argsort], color = 'magenta')
-
+            LiRj_Real[select] += self.model_lrreal[select] + \
+              Tot_D_iL_amp[select] * Tot_D_jR_amp[select] * self.model_rlamp[select] * np.cos(self.model_rlphas[select] + Tot_D_iL_phas[select] - Tot_D_jR_phas[select] - 2. * (self.pang1[select] + self.pang2[select]))
     
-                figure.savefig(filename+'.baseline'+str(m+1)+'_'+str(n+1)+'.Q'+'.'+self.filetype, bbox_inches = 'tight')
-                
-                plt.close('all')
-
-                        
-                
-                
-                figure, axes = plt.subplots(2, sharex=True, gridspec_kw={'hspace': 0}, figsize=(10, 8))
-        
-                for ax in axes.flat:
-                    ax.tick_params(length=6, width=2,which = 'major')
-                    ax.tick_params(length=4, width=1.5,which = 'minor')
+            LiRj_Imag[select] += self.model_lrimag[select] + \
+              Tot_D_iL_amp[select] * Tot_D_jR_amp[select] * self.model_rlamp[select] * np.sin(self.model_rlphas[select] + Tot_D_iL_phas[select] - Tot_D_jR_phas[select] - 2. * (self.pang1[select] + self.pang2[select]))
+            
+            
+        RiLj_Real += \
+          Tot_D_iR_amp * self.llamp * np.cos(Tot_D_iR_phas + self.llphas + 2. * self.pang1) + \
+          Tot_D_jL_amp * self.rramp * np.cos(-Tot_D_jL_phas + self.rrphas + 2. * self.pang2)
         
-                axes[0].set_xlim(np.min(time) - (np.max(time) - np.min(time)) * 0.3, np.max(time) + (np.max(time) - np.min(time)) * 0.1)
-                axes[1].set_xlim(np.min(time) - (np.max(time) - np.min(time)) * 0.3, np.max(time) + (np.max(time) - np.min(time)) * 0.1)
-                axes[1].set_ylim(-180, 180)
-                
-                axes[1].set(xlabel = 'Time (UT)')
-                
-                axes[0].set(ylabel = 'Amplitude (Jy)')
-                axes[1].set(ylabel = 'Phase (deg)')
-                
-                axes[0].set_title(self.dataname)
-
-                axes[0].annotate('Stokes U', xy=(1, 1), xycoords = 'axes fraction', xytext = (-25, -25), size = 24, textcoords='offset pixels', horizontalalignment='right', verticalalignment='top')
-                
-                axes[1].annotate(self.antname[dumm] + '-' + self.antname[dumn], xy=(0, 0), xycoords = 'axes fraction', xytext = (25, 25), size = 24, textcoords='offset pixels', horizontalalignment='left', verticalalignment='bottom')
-                axes[1].annotate('IF {:d}'.format(k+1), xy = (0, 1), xycoords = 'axes fraction', xytext = (25, -25), size = 24, textcoords='offset pixels', horizontalalignment='left', verticalalignment='top')
-                
-                
-                dumx, dumy1, dumy2 = np.empty([0]), np.empty([0]), np.empty([0])
-                
-                
-                for l in range(len(source)):
-                    
-                    select = (ant1 == dumm) & (ant2 == dumn) & (sourcearr == source[l])
-                    
-                    dumx = np.append(dumx, time[select])
-                    dumy1 = np.append(dumy1, mod_uamp[select])
-                    dumy2 = np.append(dumy2, np.degrees(mod_uphas[select]))
-
-                    if(len(dumx) == 0): continue
-                
-                    axes[0].errorbar(time[select], uamp[select], uamp_sigma[select], fmt = 'o', markerfacecolor = 'None', markeredgecolor = self.colors[l], ecolor = self.colors[l], label = source[l].upper(), zorder = 0)
-                    axes[1].errorbar(time[select], np.degrees(uphas[select]), np.degrees(uphas_sigma[select]), fmt = 'o', markerfacecolor = 'None', markeredgecolor = self.colors[l], ecolor = self.colors[l], zorder = 0)
-                    
-                    
-                    if self.allplot:
-                        axes[0].plot(time[select], mod_pol_uamp[select], color = self.colors[l], linestyle = '--')
-                        axes[1].plot(time[select], np.degrees(mod_pol_uphas[select]), color = self.colors[l], linestyle = '--')
-                        
-                        axes[0].plot(time[select], mod_dterm_uamp[select], color = self.colors[l], linestyle = ':')
-                        axes[1].plot(time[select], np.degrees(mod_dterm_uphas[select]), color = self.colors[l], linestyle = ':')
-                    
-                
-                if(len(dumx) == 0): continue
+        RiLj_Imag += \
+          Tot_D_iR_amp * self.llamp * np.sin(Tot_D_iR_phas + self.llphas + 2. * self.pang1) + \
+          Tot_D_jL_amp * self.rramp * np.sin(-Tot_D_jL_phas + self.rrphas + 2. * self.pang2)
     
-                           
-                axes[0].legend(loc='upper left', fontsize = 18 - int(len(source)/2.), frameon=False, markerfirst=True, handlelength=1.0)
-                
-                dumx = np.array(dumx)
-                
-                argsort = np.argsort(dumx)
-                
-                axes[0].plot(dumx[argsort], dumy1[argsort], color = 'magenta')
-                if self.allplot:
-                    axes[1].plot(dumx[argsort], dumy2[argsort], color = 'magenta', label = 'whole terms')
-                    
-                    axes[1].plot(np.nan, np.nan, color = 'black', linestyle = '--', label = 'source pol')
-                    axes[1].plot(np.nan, np.nan, color = 'black', linestyle = ':', label = 'd-terms')
+        LiRj_Real += \
+          Tot_D_iL_amp * self.rramp * np.cos(Tot_D_iL_phas + self.rrphas - 2. * self.pang1) + \
+          Tot_D_jR_amp * self.llamp * np.cos(-Tot_D_jR_phas + self.llphas - 2. * self.pang2)
     
-                    axes[1].legend(loc = 'upper left', frameon=False, fontsize = 16, handlelength=1.0)
-                else:
-                    axes[1].plot(dumx[argsort], dumy2[argsort], color = 'magenta')
-
+        LiRj_Imag += \
+          Tot_D_iL_amp * self.rramp * np.sin(Tot_D_iL_phas + self.rrphas - 2. * self.pang1) + \
+          Tot_D_jR_amp * self.llamp * np.sin(-Tot_D_jR_phas + self.llphas - 2. * self.pang2)  
+       
     
-                figure.savefig(filename+'.baseline'+str(m+1)+'_'+str(n+1)+'.U'+'.'+self.filetype, bbox_inches = 'tight')
-                plt.close('all')
-
+        compv = np.concatenate([LiRj_Real, LiRj_Imag, RiLj_Real, RiLj_Imag])
+        
+        return compv
     
-    def amperror(self, value, error):
-        x = np.real(value)
-        y = np.imag(value)
-        xerr = np.real(error)
-        yerr = np.imag(error)
-        r = np.absolute(value)
-        return np.sqrt((x**2*xerr**2 + y**2*yerr**2) / r**2)
-    
-    
-    def phaserror(self, value, error):
-        x = np.real(value)
-        y = np.imag(value)
-        xerr = np.real(error)
-        yerr = np.imag(error)
-        r = np.absolute(value)
-        return np.sqrt((y**2*xerr**2 + x**2*yerr**2) / r**4)
 
     
 
+    
     def residualplot(self, k, nant, antname, source, dumfit, time, ant1, ant2, sourcearr, qamp, qphas, uamp, uphas, qsigma, usigma, tsep, filename):
         """
         Draw fitting residual plots.
         """  
         
         qreal, qimag, ureal, uimag = qamp * np.cos(qphas), qamp * np.sin(qphas), uamp * np.cos(uphas), uamp * np.sin(uphas)
         data_q = qreal + 1j*qimag
@@ -2578,23 +1766,25 @@
         mod_q, mod_u = (mod_rl + mod_lr) / 2., -1j * (mod_rl - mod_lr) / 2.
         
         
         for m in range(nant):
             
             if(sum(ant1 == m) == 0) & (sum(ant2 == m) == 0): continue
             
-            figure, axes = plt.subplots(2, sharex=True, gridspec_kw={'hspace': 0}, figsize=(10, 8))
+            figure, axes = plt.subplots(2, sharex=True, gridspec_kw={'hspace': 0}, figsize=(8, 8))
     
             for ax in axes.flat:
                 ax.tick_params(length=6, width=2,which = 'major')
                 ax.tick_params(length=4, width=1.5,which = 'minor')
-    
+                
             axes[0].set_xlim(np.min(time) - (np.max(time) - np.min(time)) * 0.35, np.max(time) + (np.max(time) - np.min(time)) * 0.1)
             axes[1].set_xlim(np.min(time) - (np.max(time) - np.min(time)) * 0.35, np.max(time) + (np.max(time) - np.min(time)) * 0.1)
             
+#            axes[0].set(title = 'BL229AE')
+            
             axes[1].set(xlabel = 'Time (UT)')
             
             axes[0].set(ylabel = 'Stokes Q (sigma)')
             axes[1].set(ylabel = 'Stokes U (sigma)')
             
             axes[0].set_title(self.dataname)
             
@@ -2631,52 +1821,70 @@
                 binyerr = np.zeros(len(boundary_left))
                 
                 for j in range(len(boundary_left)):
                     binx[j] = (boundary_left[j] + boundary_right[j]) / 2.
                     biny[j] = np.mean(dumy[(dumx >= boundary_left[j]) & (dumx <= boundary_right[j])])
                     binyerr[j] = np.std(dumy[(dumx >= boundary_left[j]) & (dumx <= boundary_right[j])])
                     
-                axes[0].scatter(binx, biny, s = 30, marker = 'o', facecolor = self.colors[l], edgecolor = self.colors[l], label = source[l].upper(), zorder = 0)
+                axes[0].scatter(binx, biny, s = 30, marker = self.markerarr[l], facecolor = 'None', edgecolor = self.colors[l], label = source[l].upper(), zorder = 0)
                 
                 dumy = np.abs(((data_u[select] - mod_u[select]) / usigma[select]))
     
                 dumy = dumy[argsort]
                 
                 binx = np.zeros(len(boundary_left))
                 biny = np.zeros(len(boundary_left))
                 binyerr = np.zeros(len(boundary_left))
                 
                 for j in range(len(boundary_left)):
                     binx[j] = (boundary_left[j] + boundary_right[j]) / 2.
                     biny[j] = np.mean(dumy[(dumx >= boundary_left[j]) & (dumx <= boundary_right[j])])
                     binyerr[j] = np.std(dumy[(dumx >= boundary_left[j]) & (dumx <= boundary_right[j])])
                     
-                axes[1].scatter(binx, biny, s = 30, marker = 'o', facecolor = self.colors[l], edgecolor = self.colors[l], label = source[l].upper(), zorder = 0)
+                axes[1].scatter(binx, biny, s = 30, marker = self.markerarr[l], facecolor = 'None', edgecolor = self.colors[l], zorder = 0)
                 
                        
             axes[0].legend(loc='upper left', fontsize = 18 - int(len(source)/2.), frameon=False, markerfirst=True, handlelength=1.0)
 
+
+            dumxticks = axes[1].get_xticks()
+            dumxticklabel = []
+            for it in dumxticks:
+                if(it % 1) == 0.: dumxticklabel.append(str(int(it)))
+                if(it % 1) != 0.: dumxticklabel.append(str(it))
+            if(np.max(dumxticks) > 24.):
+                dumit = 0
+                for it in range(len(dumxticks)):
+                    if(dumxticks[it] > 24.): 
+                        if(dumxticks[it] % 1) == 0.: dumxticklabel[it] = str(int(dumxticks[it] - 24.))
+                        if(dumxticks[it] % 1) != 0.: dumxticklabel[it] = str(dumxticks[it] - 24.)
+                        if(dumit == 0): dumxticklabel[it] = '{:02d}d/'.format(np.min(self.day) + 1) + dumxticklabel[it]
+                        dumit += 1
+            
+            axes[1].set_xticklabels(dumxticklabel)
+    
     
             figure.savefig(filename+'.'+antname[m]+'.'+self.filetype, bbox_inches = 'tight')
             
             plt.close('all')
 
-    
+
+
     def dplot(self, pol, filename, antname, DRArr, DLArr, source, lpcal):
         """
         Draw D-term plots on the complex plane.
         """  
         if not self.dplot_IFsep:
             fig, ax = plt.subplots(figsize=(8, 8))
             
             ax.tick_params(length=6, width=2,which = 'major')
             ax.tick_params(length=4, width=1.5,which = 'minor')
             
             plt.grid()
-    
+                
             for m in range(len(antname)):
                 
                 drreal = DRArr.dropna().applymap(np.real).loc[:,antname[m]].to_numpy() * 1e2
                 drimag = DRArr.dropna().applymap(np.imag).loc[:,antname[m]].to_numpy() * 1e2
                 
                 dlreal = DLArr.dropna().applymap(np.real).loc[:,antname[m]].to_numpy() * 1e2
                 dlimag = DLArr.dropna().applymap(np.imag).loc[:,antname[m]].to_numpy() * 1e2
@@ -2824,15 +2032,195 @@
                 
                 if lpcal:
                     ax.add_artist(leg2)
                 
                 
                 plt.savefig(self.direc + 'gpcal/' + filename + '.IF'+str(k+1) + '.'+self.filetype, bbox_inches = 'tight')
                 plt.close('all')
+
+
+
+    def dplot_new(self, pol, filename, antname, IFarr, DRArr, DLArr, source = None, lpcal = True, IFsep = False):
+        """
+        Draw D-term plots on the complex plane.
+        """  
+        
+        uniqant = np.unique(antname)
+        
+        if not IFsep:
+            fig, ax = plt.subplots(figsize=(8, 8))
+            
+            ax.tick_params(length=6, width=2,which = 'major')
+            ax.tick_params(length=4, width=1.5,which = 'minor')
+            
+            plt.grid()
+    
+            for m in range(len(uniqant)):
                 
+                select = (antname == uniqant[m])
+                
+                drreal = np.real(DRArr[select]) * 1e2
+                drimag = np.imag(DRArr[select]) * 1e2
+                
+                dlreal = np.real(DLArr[select]) * 1e2
+                dlimag = np.imag(DLArr[select]) * 1e2
+                
+                ax.scatter(drreal, drimag, s = 180, facecolor = self.colors[m], edgecolor = self.colors[m], marker = self.markerarr[m], label = antname[m])
+                ax.scatter(dlreal, dlimag, s = 180, facecolor = 'None', edgecolor = self.colors[m], marker = self.markerarr[m])
+                
+            if lpcal:
+                for l in range(len(source)):
+                    read = pd.read_csv(self.direc+'gpcal/'+self.dataname+source[l]+'.an', header = None, skiprows=1, delimiter = '\t')
+                    anname, lpcaldr, lpcaldl = read[1].to_numpy(), read[2].to_numpy(), read[3].to_numpy()
+                    dumant, dumdrreal, dumdrimag, dumdlreal, dumdlimag = anname[::2], lpcaldr[::2] * 1e2, lpcaldr[1::2] * 1e2, lpcaldl[::2] * 1e2, lpcaldl[1::2] * 1e2
+                    for m in range(len(antname)):
+                        ax.scatter(dumdrreal[dumant == antname[m]], dumdrimag[dumant == antname[m]], s = 20, facecolor = self.colors[m], edgecolor = self.colors[m], marker = self.markerarr[m], \
+                                   alpha = 0.2)
+                        ax.scatter(dumdlreal[dumant == antname[m]], dumdlimag[dumant == antname[m]], s = 20, facecolor = 'None', edgecolor = self.colors[m], marker = self.markerarr[m], \
+                                   alpha = 0.2)
+                        
+    
+            if(self.drange == None):
+                dumbound = np.max([np.abs(DRArr), np.abs(DLArr)]) * 1e2 * 1.2
+            else:
+                dumbound = self.drange
+                
+            
+            plt.xlim(-dumbound, dumbound)
+            plt.ylim(-dumbound, dumbound)
+            plt.xlabel('Real (\%)')
+            plt.ylabel('Imaginary (\%)')
+            plt.title(self.dataname)
+            
+            
+            ax.annotate('Calibrators:', xy=(0, 1), xycoords = 'axes fraction', xytext = (25, -25), size = 18, textcoords='offset pixels', horizontalalignment='left', verticalalignment='top')
+            for i in range(len(source)):
+                ax.annotate(source[i], xy=(0, 1), xycoords = 'axes fraction', xytext = (25, -25*(i+2)), size = 18, textcoords='offset pixels', horizontalalignment='left', verticalalignment='top')
+            
+            
+            if(pol >= 0):
+                ax.annotate('Pol-selfcal, Iteration = {:d}/{:d}'.format(pol, self.selfpoliter), xy=(1, 1), xycoords = 'axes fraction', xytext = (-25, -25), size = 22, textcoords='offset pixels', horizontalalignment='right', verticalalignment='top')
+    
+            
+            leg1 = ax.legend(loc='lower left', fontsize = 18, frameon=False, markerfirst=True, handlelength=0.3, labelspacing=0.3)
+            
+            rcp = ax.scatter([], [], s = 120, facecolor = 'black', edgecolor = 'black', marker = 'o')
+            lcp = ax.scatter([], [], s = 120, facecolor = 'none', edgecolor = 'black', marker = 'o')
+            
+            leg2 = ax.legend([rcp, lcp], ['Filled - RCP', 'Open - LCP'], loc = 'lower right', frameon=False, fontsize = 24, handlelength=0.3)
+            
+            if lpcal:
+                gpcal = ax.scatter([], [], s = 180, facecolor = 'black', edgecolor = 'black', marker = 'o')
+                lpcal = ax.scatter([], [], s = 20, facecolor = 'black', edgecolor = 'black', marker = 'o')
+                leg3 = ax.legend([gpcal, lpcal], ['GPCAL', 'LPCAL'], loc = 'upper right', frameon=False, fontsize = 24, handlelength=0.3)
+            
+            ax.add_artist(leg1)
+            
+            if lpcal:
+                ax.add_artist(leg2)
+            
+            
+            plt.savefig(self.direc + 'gpcal/' + filename +'.'+self.filetype, bbox_inches = 'tight')
+            plt.close('all')
+
+
+        # If dplot_IFsep == True, then plot the D-terms for each IF separately.
+        else:
+
+            for k in range(self.ifnum):
+                
+                if(np.sum((IFarr == k+1)) == 0.):
+                    continue
+                
+                fig, ax = plt.subplots(figsize=(8, 8))
+                
+                ax.tick_params(length=6, width=2,which = 'major')
+                ax.tick_params(length=4, width=1.5,which = 'minor')
+                
+                plt.grid()
+        
+                
+                for m in range(len(uniqant)):
+                    
+                    select = (antname == uniqant[m]) & (IFarr == k+1)
+                    
+                    drreal = np.real(DRArr[select]) * 1e2
+                    drimag = np.imag(DRArr[select]) * 1e2
+                    
+                    dlreal = np.real(DLArr[select]) * 1e2
+                    dlimag = np.imag(DLArr[select]) * 1e2
+                    
+                    
+                    if(drreal == 0.) & (drimag == 0.) & (dlreal == 0.) & (dlimag == 0.): continue
+                    
+                    ax.scatter(drreal[drreal != 0.], drimag[drimag != 0.], s = 180, facecolor = self.colors[m], edgecolor = self.colors[m], marker = self.markerarr[m], label = antname[m])
+                    ax.scatter(dlreal[drreal != 0.], dlimag[drimag != 0.], s = 180, facecolor = 'None', edgecolor = self.colors[m], marker = self.markerarr[m])
+                    
+                if lpcal:
+                    for l in range(len(source)):
+                        read = pd.read_csv(self.direc+'gpcal/'+self.dataname+source[l]+'.an', header = None, skiprows=1, delimiter = '\t')
+                        anname, lpcaldr, lpcaldl = read[1].to_numpy(), read[2].to_numpy(), read[3].to_numpy()
+                        dumant, dumdrreal, dumdrimag, dumdlreal, dumdlimag = anname[::2], lpcaldr[::2] * 1e2, lpcaldr[1::2] * 1e2, lpcaldl[::2] * 1e2, lpcaldl[1::2] * 1e2
+                        for m in range(len(antname)):
+                            dumx = dumdrreal[dumant == antname[m]]
+                            dumy = dumdrimag[dumant == antname[m]]
+                            if(dumx[k] == 0.) & (dumy[k] == 0.): continue
+                            ax.scatter(dumx[k], dumy[k], s = 20, facecolor = self.colors[m], edgecolor = self.colors[m], marker = self.markerarr[m], \
+                                       alpha = 0.2)
+                            dumx = dumdlreal[dumant == antname[m]]
+                            dumy = dumdlimag[dumant == antname[m]]
+                            ax.scatter(dumx[k], dumy[k], s = 20, facecolor = 'None', edgecolor = self.colors[m], marker = self.markerarr[m], \
+                                       alpha = 0.2)
+                            
+        
+                if(self.drange == None):
+                    dumbound = np.max([np.abs(DRArr), np.abs(DLArr)]) * 1e2 * 1.2
+                else:
+                    dumbound = self.drange
+                
+                plt.xlim(-dumbound, dumbound)
+                plt.ylim(-dumbound, dumbound)
+                plt.xlabel('Real (\%)')
+                plt.ylabel('Imaginary (\%)')
+                plt.title(self.dataname + ', IF' + str(k+1))
+                
+                
+                sourcename = ''
+                for i in range(len(source)):
+                    sourcename = sourcename + source[i]+'-'
+                
+                ax.annotate('Calibrators:', xy=(0, 1), xycoords = 'axes fraction', xytext = (25, -25), size = 18, textcoords='offset pixels', horizontalalignment='left', verticalalignment='top')
+                for i in range(len(source)):
+                    ax.annotate(source[i], xy=(0, 1), xycoords = 'axes fraction', xytext = (25, -25*(i+2)), size = 18, textcoords='offset pixels', horizontalalignment='left', verticalalignment='top')
+                
+                if(pol >= 0):
+                    ax.annotate('Pol-selfcal, Iteration = {:d}/{:d}'.format(pol, self.selfpoliter), xy=(1, 1), xycoords = 'axes fraction', xytext = (-25, -25), size = 22, textcoords='offset pixels', horizontalalignment='right', verticalalignment='top')
+        
+                
+                leg1 = ax.legend(loc='lower left', fontsize = 18, frameon=False, markerfirst=True, handlelength=0.3, labelspacing=0.3)
+                
+                rcp = ax.scatter([], [], s = 120, facecolor = 'black', edgecolor = 'black', marker = 'o')
+                lcp = ax.scatter([], [], s = 120, facecolor = 'none', edgecolor = 'black', marker = 'o')
+                
+                leg2 = ax.legend([rcp, lcp], ['Filled - RCP', 'Open - LCP'], loc = 'lower right', frameon=False, fontsize = 24, handlelength=0.3)
+                
+                if lpcal:
+                    gpcal = ax.scatter([], [], s = 180, facecolor = 'black', edgecolor = 'black', marker = 'o')
+                    lpcal = ax.scatter([], [], s = 20, facecolor = 'black', edgecolor = 'black', marker = 'o')
+                    leg3 = ax.legend([gpcal, lpcal], ['GPCAL', 'LPCAL'], loc = 'upper right', frameon=False, fontsize = 24, handlelength=0.3)
+                
+                ax.add_artist(leg1)
+                
+                if lpcal:
+                    ax.add_artist(leg2)
+                
+                
+                plt.savefig(self.direc + 'gpcal/' + filename + '.IF'+str(k+1) + '.'+self.filetype, bbox_inches = 'tight')
+                plt.close('all')
+                                
 
 
     def chisqplot(self, chisq):
         """
         Draw the fitting chi-square plots.
         """  
         fig, ax = plt.subplots(figsize=(9, 7))
@@ -2847,15 +2235,15 @@
         for k in range(self.ifnum):
             ax.scatter(np.arange(0, len(chisq["IF1"])), chisq["IF"+str(k+1)], s = 180, facecolor = 'None', edgecolor = self.colors[k], marker = self.markerarr[k], label = "IF"+str(k+1))
         
         plt.xlim(-1, len(chisq["IF1"])+2)
         plt.xlabel('Iteration')
         plt.ylabel('Reduced chi-square')
         plt.title(self.dataname)
-        
+                
         ax.legend(loc='upper right', fontsize = 18, frameon=False, markerfirst=True, handlelength=0.3, labelspacing=0.3)
         
         
         plt.savefig(self.direc + 'gpcal/' + self.outputname+'chisq.'+self.filetype, bbox_inches = 'tight')
         plt.close('all')
         
 
@@ -2879,327 +2267,352 @@
             data.zap()
         
         cmap = AIPSImage(dtermname, 'CMAP', 1, 1)
         if(cmap.exists() == True):
             cmap.clrstat()
             cmap.zap()
             
-        self.runfitld(dtermname, 'DTERM', self.direc+self.dataname+source[0]+'.uvf')
-        self.runfitld(dtermname, 'CMAP', self.direc+self.dataname+source[0]+'.fits')
+        au.runfitld(dtermname, 'DTERM', self.direc+self.dataname+source[0]+'.uvf')
+        au.runfitld(dtermname, 'CMAP', self.direc+self.dataname+source[0]+'.fits')
     
-        self.runlpcal(dtermname, 'DTERM', 'CMAP', 1)
+        au.runlpcal(dtermname, 'DTERM', 'CMAP', 1)
         
         cmap.zap()
         
         
         dterm = WAIPSUVData(dtermname, 'DTERM', 1, 1)
         
         tabed = dterm.table('AN', 1)
         
         
         # Update the antenna tables using the input D-terms.
         i = 0
         for row in tabed:
             
-            dumreal = DRArr.applymap(np.real).loc[:,row.anname.replace(' ', '')]
-            dumimag = DRArr.applymap(np.imag).loc[:,row.anname.replace(' ', '')]
+            dumdr = DRArr.loc[:,row.anname.replace(' ', '')]
+            dumreal = np.real(np.array([complex(it) for it in dumdr]))
+            dumimag = np.imag(np.array([complex(it) for it in dumdr]))
             row.polcala = list(np.ravel([dumreal, dumimag], 'F'))
-            
-            dumreal = DLArr.applymap(np.real).loc[:,row.anname.replace(' ', '')]
-            dumimag = DLArr.applymap(np.imag).loc[:,row.anname.replace(' ', '')]
+
+            dumdl = DLArr.loc[:,row.anname.replace(' ', '')]
+            dumreal = np.real(np.array([complex(it) for it in dumdl]))
+            dumimag = np.imag(np.array([complex(it) for it in dumdl]))
             row.polcalb = list(np.ravel([dumreal, dumimag], 'F'))
             
             row.update()
             row.update()
             
             i += 1
+                
+        if path.exists(self.direc+'gpcal/'+self.outputname+'dterm.tbout'):
+            os.system('rm ' + self.direc+'gpcal/'+self.outputname+'dterm.tbout')
+        au.runtbout(dtermname, 'DTERM', self.direc+'gpcal/'+self.outputname+'dterm.tbout')
         
-        if path.exists(self.direc+'gpcal/'+self.dataname+'dterm.tbout'):
-            os.system('rm ' + self.direc+'gpcal/'+self.dataname+'dterm.tbout')
-        self.runtbout(dtermname, 'DTERM', self.direc+'gpcal/'+self.dataname+'dterm.tbout')
-        
-       
         # Apply the D-terms and export the D-term corrected UVFITS files to the working directory.
         for l in range(len(source)):
-            inname = source[l]
+            inname = str(source[l])
             
             if self.selfcal:
                 if (not source[l] in self.calsour) | (not source[l] in self.polcalsour):
                     
                     data = AIPSUVData(inname, 'EDIT', 1, 1)
                     if(data.exists() == True):
                         data.clrstat()
                         data.zap()
                         
-                    self.runfitld(inname, 'EDIT', self.direc+self.dataname+source[l]+'.uvf')
+                    au.runfitld(inname, 'EDIT', self.direc+self.dataname+source[l]+'.uvf')
                     
                             
                     cmap = AIPSImage(inname, 'CMAP', 1, 1)
                     if(cmap.exists() == True):
                         cmap.clrstat()
                         cmap.zap()
                         
-                    self.runfitld(inname, 'CMAP', self.direc+self.dataname+source[l]+'.fits')
+                    au.runfitld(inname, 'CMAP', self.direc+self.dataname+source[l]+'.fits')
         
                     calib = AIPSUVData(inname, 'CALIB', 1, 1)
                     if(calib.exists() == True):
                         calib.clrstat()
                         calib.zap()
                             
-                    self.runcalib(inname, 'EDIT', 'CALIB', self.solint, self.soltype, self.solmode, self.weightit)
+                    au.runcalib(inname, 'EDIT', inname, 'CMAP', 'CALIB', self.solint, self.soltype, self.solmode, self.weightit)
                     calib = AIPSUVData(inname, 'CALIB', 1, 1)
     
                     if path.exists(self.direc + self.dataname + source[l] + '.calib'):
                         os.system('rm ' + self.direc + self.dataname + source[l] + '.calib')
-                    self.runfittp(inname, 'CALIB', self.direc + self.dataname + source[l] + '.calib')
+                    au.runfittp(inname, 'CALIB', self.direc + self.dataname + source[l] + '.calib')
                     
                     data.zap()
                     cmap.zap()
                 
                 else:
                     calib = AIPSUVData(inname, 'CALIB', 1, 1)
                     if(calib.exists() == True):
                         calib.clrstat()
                         calib.zap()
                     
-                    self.runfitld(inname, 'CALIB', self.direc+self.dataname+source[l]+'.calib')
+                    au.runfitld(inname, 'CALIB', self.direc+self.dataname+source[l]+'.calib')
                     
                 
                 calib.zap_table('AN', 1)
                 
-                self.runtacop(dtermname, 'DTERM', inname, 'CALIB')
+                au.runtacop(dtermname, 'DTERM', inname, 'CALIB')
                 
                 
                 split = AIPSUVData(inname, 'SPLIT', 1, 1)
                 if(split.exists() == True):
                     split.clrstat()
                     split.zap()
                 
-                self.runsplit(inname, 'CALIB')
+                au.runsplit(inname, 'CALIB')
                 
-                if path.exists(self.direc+self.dataname+source[l]+'.dtcal.uvf'):
-                    os.system('rm ' + self.direc+self.dataname+source[l]+'.dtcal.uvf')
-                self.runfittp(inname, 'SPLIT', self.direc+self.dataname+source[l]+'.dtcal.uvf')
+                if path.exists(self.direc+self.outputname+source[l]+'.dtcal.uvf'):
+                    os.system('rm ' + self.direc+self.outputname+source[l]+'.dtcal.uvf')
+                au.runfittp(inname, 'SPLIT', self.direc+self.outputname+source[l]+'.dtcal.uvf')
                 
                 split = AIPSUVData(inname, 'SPLIT', 1, 1)
                 split.zap()
                 
                 calib.zap()
                 
             
             else:
                 data = AIPSUVData(inname, 'EDIT', 1, 1)
                 if(data.exists() == True):
                     data.clrstat()
                     data.zap()
                     
-                self.runfitld(inname, 'EDIT', self.direc+self.dataname+source[l]+'.uvf')
+                au.runfitld(inname, 'EDIT', self.direc+self.dataname+source[l]+'.uvf')
                 
                 data = AIPSUVData(inname, 'EDIT', 1, 1)
                 
                 data.zap_table('AN', 1)
                 
-                self.runtacop(dtermname, 'DTERM', inname, 'EDIT')
+                au.runtacop(dtermname, 'DTERM', inname, 'EDIT')
                 
                 
                 split = AIPSUVData(inname, 'SPLIT', 1, 1)
                 
                 if(split.exists() == True):
                     split.clrstat()
                     split.zap()
                 
-                self.runsplit(inname, 'EDIT')
+                au.runsplit(inname, 'EDIT')
                 
-                if path.exists(self.direc+self.dataname+source[l]+'.dtcal.uvf'):
-                    os.system('rm ' + self.direc+self.dataname+source[l]+'.dtcal.uvf')
-                self.runfittp(inname, 'SPLIT', self.direc+self.dataname+source[l]+'.dtcal.uvf')
+                if path.exists(self.direc+self.outputname+source[l]+'.dtcal.uvf'):
+                    os.system('rm ' + self.direc+self.outputname+source[l]+'.dtcal.uvf')
+                au.runfittp(inname, 'SPLIT', self.direc+self.outputname+source[l]+'.dtcal.uvf')
                 
                 split = AIPSUVData(inname, 'SPLIT', 1, 1)
                 split.zap()
             
                 data.zap()
-            
         
         dterm.zap()
 
 
-    def pol_applydterm(self, source, DRArr, DLArr, filename):
+    def pol_applydterm(self, source, read, filename):
         """
         Apply the best-fit D-terms estimated by using instrumental polarization self-calibration to UVFITS data.
         
         Args:
             source (list): a list of the sources for which D-terms will be corrected.
             DRArr (list): a list of the best-fit RCP D-terms.
             DLArr (list): a list of the best-fit LCP D-terms.
             filename (str): the output file name.
         """
         
         self.logger.info('Applying the estimated D-Terms to {:d} sources...\n'.format(len(self.source)))
+        
+        
+        dtermread = pd.read_csv(read, header = 0, skiprows=0, delimiter = '\t', index_col = 0)
+            
+        pol_ant = np.array(dtermread['antennas'])
+        pol_IF = np.array(dtermread['IF'])
+        dum_DRArr = np.array(dtermread['DRArr'])
+        dum_DLArr = np.array(dtermread['DLArr'])
+        
+        pol_DRArr = np.array([complex(it) for it in dum_DRArr])
+        pol_DLArr = np.array([complex(it) for it in dum_DLArr])
+        
     
-        inname = self.dataname[0:10]
+        inname = 'APPLY'
         
         data = AIPSUVData(inname, 'DTERM', 1, 1)
         if(data.exists() == True):
             data.clrstat()
             data.zap()
         
         cmap = AIPSImage(inname, 'CMAP', 1, 1)
         if(cmap.exists() == True):
             cmap.clrstat()
             cmap.zap()
         
         
         if self.selfcal:
-            self.runfitld(inname, 'DTERM', self.direc+self.dataname+source[0]+'.calib')
+            au.runfitld(inname, 'DTERM', self.direc+self.dataname+source[0]+'.calib')
         else:
-            self.runfitld(inname, 'DTERM', self.direc+self.dataname+source[0]+'.uvf')
+            au.runfitld(inname, 'DTERM', self.direc+self.dataname+source[0]+'.uvf')
         
-        self.runfitld(inname, 'CMAP', self.direc+self.dataname+source[0]+'.fits')
+        au.runfitld(inname, 'CMAP', self.direc+self.dataname+source[0]+'.fits')
         
-        self.runlpcal(inname, 'DTERM', 'CMAP', 1)
+        au.runlpcal(inname, 'DTERM', 'CMAP', 1)
         
         
         image = AIPSImage(inname, 'CMAP', 1, 1)
         image.zap()
         
         
         dterm = WAIPSUVData(inname, 'DTERM', 1, 1)
         
         tabed = dterm.table('AN', 1)
         
         
+        fqtable = data.table('FQ', 1)
+        if(isinstance(fqtable[0].if_freq, float) == True):
+            ifnum = 1
+        else:
+            ifnum = len(fqtable[0].if_freq)
+            
+        
         # Update the D-terms in the antenna table.
-        i = 0
         for row in tabed:
+            anname = row.anname.replace(' ', '')
             
-            dumreal = DRArr.applymap(np.real).loc[:,row.anname.replace(' ', '')]
-            dumimag = DRArr.applymap(np.imag).loc[:,row.anname.replace(' ', '')]
+            select = (pol_ant == anname)
+            
+            dumif = pol_IF[select]
+            dum_DRArr = pol_DRArr[select]
+            dum_DLArr = pol_DLArr[select]
+            
+            dumreal, dumimag = [], []
+            
+            for i in range(ifnum):
+                dumselect = (dumif == i+1)
+                if(np.sum(dumselect) > 0):
+                    dumreal.append(np.real(dum_DRArr[dumselect]))
+                    dumimag.append(np.imag(dum_DRArr[dumselect]))
+                else:
+                    dumreal.append(0.)
+                    dumimag.append(0.)
+                        
             row.polcala = list(np.ravel([dumreal, dumimag], 'F'))
             
-            dumreal = DLArr.applymap(np.real).loc[:,row.anname.replace(' ', '')]
-            dumimag = DLArr.applymap(np.imag).loc[:,row.anname.replace(' ', '')]
-            row.polcalb = list(np.ravel([dumreal, dumimag], 'F'))
             
+            dumreal, dumimag = [], []
+            
+            for i in range(ifnum):
+                dumselect = (dumif == i+1)
+                if(np.sum(dumselect) > 0):
+                    dumreal.append(np.real(dum_DLArr[dumselect]))
+                    dumimag.append(np.imag(dum_DLArr[dumselect]))
+                else:
+                    dumreal.append(0.)
+                    dumimag.append(0.)
+                    
+            row.polcalb = list(np.ravel([dumreal, dumimag], 'F'))
+                        
             row.update()
             row.update()
+                
             
-            i += 1
             
         if path.exists(filename+'dterm.tbout'):
             os.system('rm ' + filename+'dterm.tbout')
-        self.runtbout(inname, 'DTERM', filename+'dterm.tbout')
+        au.runtbout(inname, 'DTERM', filename+'dterm.tbout')
             
             
         for l in range(len(source)):
-            inname = source[l]
+            inname = str(source[l])
             
             calib = AIPSUVData(inname, 'CALIB', 1, 1)
             if(calib.exists() == True):
                 calib.clrstat()
                 calib.zap()
             
             if self.selfcal:
-                self.runfitld(inname, 'CALIB', self.direc + self.dataname + source[l]+'.calib')
+                au.runfitld(inname, 'CALIB', self.direc + self.dataname + source[l]+'.calib')
             else:
-                self.runfitld(inname, 'CALIB', self.direc + self.dataname + source[l]+'.uvf')
+                au.runfitld(inname, 'CALIB', self.direc + self.dataname + source[l]+'.uvf')
         
             calib = AIPSUVData(inname, 'CALIB', 1, 1)
         
             calib.zap_table('AN', 1)
             
-            self.runtacop(self.dataname[0:10], 'DTERM', inname, 'CALIB')
+            au.runtacop('APPLY', 'DTERM', inname, 'CALIB')
         
         
             split = AIPSUVData(inname, 'SPLIT', 1, 1)
             if(split.exists() == True):
                 split.clrstat()
                 split.zap()
                     
-            self.runsplit(inname, 'CALIB')
+            au.runsplit(inname, 'CALIB')
             
         
             if path.exists(filename+source[l]+'.dtcal.uvf'):
                 os.system('rm ' + filename+source[l]+'.dtcal.uvf')
-            self.runfittp(inname, 'SPLIT', filename+source[l]+'.dtcal.uvf')
+            au.runfittp(inname, 'SPLIT', filename+source[l]+'.dtcal.uvf')
             
             split = AIPSUVData(inname, 'SPLIT', 1, 1)
             split.zap()
             
         
             calib.zap()
             
         
         dterm.zap()
         
-        
 
 
-    def cleanqu(self, data, mask, save, log):
-        """
-        Perform imaging of Stokes Q and U in Difmap.
+    def evpacal(self, datain, dataout, clcorprm):
         
-        Args:
-            data (str): the name of the UVFITS file to be CLEANed.
-            mask (str): the name of the CLEAN windows to be used.
-            save (str): the name of the output Difmap save file.
-            log (str): the name of the Difmap log file.
-        """
-            
-        time1 = timeit.default_timer()
+        self.logger.info('Correcting EVPAs... \n Input file: {:} \n Output file: {:}'.format(datain, dataout))
         
-        curdirec = os.getcwd()
+        pinal = AIPSUVData('EVPA', 'PINAL', 1, 1)
+        if(pinal.exists() == True):
+            pinal.zap()
+            
+        au.runfitld('EVPA', 'PINAL', datain)
         
-        logname = ''
+        pinal = AIPSUVData('EVPA', 'PINAL', 1, 1)
         
+        aipssource = pinal.header.object
         
-        # Write a simple Difmap script for CLEAN in the working directory.
-#        if not path.exists(self.direc+'GPCAL_Difmap_v1'):
-        f = open(self.direc+'GPCAL_Difmap_v1','w')
-        f.write('observe %1\nmapcolor rainbow, 1, 0.5\nselect q, %2\nmapsize %3, %4\nuvweight %5, %6\nrwin %7\ndo i=1,100\nclean 100, 0.02, imstat(rms)*%8\nend do\nselect i, %2\nsave %9.IF%2.q\nclrmod tru\n' + \
-                'select u, %2\ndo i=1,100\nclean 100, 0.02, imstat(rms)*%8\nend do\nselect i, %2\nsave %9.IF%2.u\nexit')
-        f.close()
+        multi = AIPSUVData('EVPA', 'MULTI', 1, 1)
+        if(multi.exists() == True):
+            multi.zap()
             
+        au.runmulti('EVPA', 'PINAL', 1, 1)
+        au.runclcor('EVPA', 'MULTI', 1, 1, clcorprm)
         
-        # Run the Difmap script for each IF.
-        for i in range(self.ifnum):
+        pang = AIPSUVData(aipssource, 'PANG', 1, 1)
+        if(pang.exists() == True):
+            pang.zap()
             
-            if (len(self.pol_data.loc[self.pol_data["IF"] == i+1]) == 0):
-                self.logger.info('Will skip IF '+str(i+1)+' because there is no data.')
-                continue
+        au.runsplitpang('EVPA')
                 
-            os.chdir(self.direc)
-            command = "echo @GPCAL_Difmap_v1 %s,%s,%s,%s,%s,%s,%s,%s,%s | difmap > %s" %(data,i+1,self.ms,self.ps,self.uvbin,self.uvpower,mask,self.dynam,save,log+'.IF'+str(i+1))
-            os.system(command)
-            
-            logname = logname + log+'.IF'+str(i+1) + ' '
-        
-        
-        os.system('cat ' + logname + ' > ' + log)
-        os.system('rm ' + log + '.IF*')
+        au.runfittp(aipssource, 'PANG', dataout)
         
-        os.chdir(curdirec)
-        
-        time2 = timeit.default_timer()
-        
-        self.difmaptime += time2 - time1
-
-
+        pinal.zap()
+        multi.zap()
+        pang.zap()
+    
 
+        
     def zbl_dtermsolve(self):
         """
         Estimate the D-terms using the zero baselines.
         """        
-        
-        # Get the zero baseline data.
-        self.get_zbl_data()
-
-        
+                
         self.logger.info('\n####################################################################')
         self.logger.info('Zero-baseline D-Term estimation mode...\n')
 
+        # Get the zero baseline data.
+        self.get_zbl_data()
         
         # Print the basic information of the data.
         zblblname = ''
         for i in range(len(self.zblant)):
             zblblname = zblblname+('{:s}-{:s}'.format(self.zblant[i][0], self.zblant[i][1]))+','
         zblblname = zblblname[:-1]
         self.logger.info('baselines to be used: ' + zblblname + '\n')
@@ -3223,15 +2636,15 @@
                     if(self.antmount[j] == 0): mount = 'Cassegrain'
                     if(self.antmount[j] == 4): mount = 'Nasmyth-Right'
                     if(self.antmount[j] == 5): mount = 'Nasmyth-Left'
                     self.logger.info('{:s}: antenna mount = {:13s}, X = {:11.2f}m, Y = {:11.2f}m, Z = {:11.2f}m'.format(self.zblant[i][1], mount, self.antx[j], self.anty[j], self.antz[j]))
         
         self.logger.info(' ')
         
-        self.logger.info('Observation date = {:s}'.format(str(self.year)+'-'+str(self.month)+'-'+str(self.day)))
+        self.logger.info('Observation date = {:s}'.format(str(np.min(self.year))+'-'+str(np.min(self.month))+'-'+str(np.min(self.day))))
         
         
         self.zbl_nant = len(self.zblant)*2
         
         
         zbl_antname = []
         for i in range(len(self.zblant)):
@@ -3259,19 +2672,19 @@
         for k in range(self.ifnum):
             
             self.logger.info('\n####################################################################')
             self.logger.info('Processing IF {:d}'.format(k+1) + '...')
             self.logger.info('####################################################################\n')
             
             
-            ifdata = self.zbl_data.loc[self.data["IF"] == k+1]
+            ifdata = self.zbl_data.loc[self.zbl_data["IF"] == k+1]
                  
-            time, sourcearr, pang1, pang2, ant1, ant2, rrreal, rrimag, llreal, llimag, rlreal, rlimag, lrreal, lrimag, rlsigma, lrsigma, rramp, rrphas, llamp, llphas, \
+            time, dayarr, sourcearr, pang1, pang2, ant1, ant2, rrreal, rrimag, llreal, llimag, rlreal, rlimag, lrreal, lrimag, rlsigma, lrsigma, rramp, rrphas, llamp, llphas, \
             qamp, qphas, uamp, uphas, qamp_sigma, qphas_sigma, uamp_sigma, uphas_sigma, qsigma, usigma = \
-                np.array(ifdata["time"]), np.array(ifdata["source"]), np.array(ifdata["pang1"]), np.array(ifdata["pang2"]), np.array(ifdata["ant1"]), np.array(ifdata["ant2"]), \
+                np.array(ifdata["time"]), np.array(ifdata["day"]), np.array(ifdata["source"]), np.array(ifdata["pang1"]), np.array(ifdata["pang2"]), np.array(ifdata["ant1"]), np.array(ifdata["ant2"]), \
                 np.array(ifdata["rrreal"]), np.array(ifdata["rrimag"]), np.array(ifdata["llreal"]), np.array(ifdata["llimag"]), \
                 np.array(ifdata["rlreal"]), np.array(ifdata["rlimag"]), np.array(ifdata["lrreal"]), np.array(ifdata["lrimag"]), \
                 np.array(ifdata["rlsigma"]), np.array(ifdata["lrsigma"]), np.array(ifdata["rramp"]), np.array(ifdata["rrphas"]), np.array(ifdata["llamp"]), np.array(ifdata["llphas"]), \
                 np.array(ifdata["qamp"]), np.array(ifdata["qphas"]), np.array(ifdata["uamp"]), np.array(ifdata["uphas"]), \
                 np.array(ifdata["qamp_sigma"]), np.array(ifdata["qphas_sigma"]), np.array(ifdata["uamp_sigma"]), np.array(ifdata["uphas_sigma"]), np.array(ifdata["qsigma"]), np.array(ifdata["usigma"])
 
             
@@ -3354,15 +2767,15 @@
             
             ydata = np.concatenate([lrreal+1j*lrimag, rlreal+1j*rlimag])
             yfit = np.concatenate([dumfit[0:len(lrreal)]+1j*dumfit[len(lrreal):len(lrreal)*2], dumfit[len(lrreal)*2:len(lrreal)*3]+1j*dumfit[len(lrreal)*3:len(lrreal)*4]])
             ysigma = np.concatenate([lrsigma, rlsigma])
             
             chisq = np.sum(np.abs(((ydata - yfit) / ysigma) ** 2)) / (2. * len(ydata))
             
-            self.chisq.loc["zbl", "IF"+str(k+1)] = chisq
+            self.zbl_chisq = chisq
             
             self.logger.info('\nThe reduced chi-square of the fitting is {:5.3f}.'.format(chisq))
         
         
             self.logger.info(' ')
             for m in range(self.zbl_nant):
                 self.logger.info('{:s}: RCP - amplitude = {:6.3f} %, phase = {:7.2f} deg, LCP - amplitude = {:6.3f} %, phase = {:7.2f} deg'.format(zbl_antname[m], \
@@ -3375,27 +2788,86 @@
             
                 dumr = Iteration[self.zbl_nant * 4 + 2*l]
                 dumi = Iteration[self.zbl_nant * 4 + 2*l + 1]
                 
                 self.logger.info(r'{:s}: Polarized Intensity = {:6.3f} Jy, EVPA = {:6.2f} deg'.format(self.zblcalsour[l], np.sqrt(dumr ** 2 + dumi ** 2), np.degrees(np.angle(dumr + 1j * dumi)) / 2.))
             
             
-            mod_pol_qamp, mod_pol_qphas, mod_pol_uamp, mod_pol_uphas = self.zbl_deq_comp('pol', *Iteration)
-            mod_dterm_qamp, mod_dterm_qphas, mod_dterm_uamp, mod_dterm_uphas = self.zbl_deq_comp('dterm', *Iteration)
-            mod_second_qamp, mod_second_qphas, mod_second_uamp, mod_second_uphas = self.zbl_deq_comp('second', *Iteration)
-        
+            mod_lr, mod_rl = dumfit[0:len(time)] + 1j*dumfit[len(time):len(time)*2], dumfit[len(time)*2:len(time)*3] + 1j*dumfit[len(time)*3:len(time)*4]
+            mod_q, mod_u = (mod_rl + mod_lr) / 2., -1j * (mod_rl - mod_lr) / 2.
+            mod_qamp, mod_qphas, mod_uamp, mod_uphas = np.absolute(mod_q), np.angle(mod_q), np.absolute(mod_u), np.angle(mod_u)
+            
+            if self.allplot:
+                mod_pol_qamp, mod_pol_qphas, mod_pol_uamp, mod_pol_uphas = self.zbl_deq_comp('pol', *Iteration)
+                mod_dterm_qamp, mod_dterm_qphas, mod_dterm_uamp, mod_dterm_uphas = self.zbl_deq_comp('dterm', *Iteration)
+                mod_second_qamp, mod_second_qphas, mod_second_uamp, mod_second_uphas = self.zbl_deq_comp('second', *Iteration)
+                allplots = (mod_pol_qamp, mod_pol_qphas, mod_pol_uamp, mod_pol_uphas, mod_dterm_qamp, mod_dterm_qphas, mod_dterm_uamp, mod_dterm_uphas)
+            else:
+                allplots = None
+            
+            
+            if (self.vplot_title == None):
+                self.vplot_title = self.dataname[:-1]
+                
             # Create vplots if requested.
             if self.vplot:
-                self.logger.info('Creating vplots for all baselines... It may take some time.')
-                self.visualplot(k, self.zbl_nant, zbl_antname, self.zblcalsour, time, ant1, ant2, sourcearr, qamp, qphas, uamp, uphas, qamp_sigma, qphas_sigma, uamp_sigma, uphas_sigma, \
-                                mod_pol_qamp, mod_pol_qphas, mod_pol_uamp, mod_pol_uphas, mod_dterm_qamp, mod_dterm_qphas, mod_dterm_uamp, mod_dterm_uphas, mod_second_qamp, mod_second_qphas, mod_second_uamp, mod_second_uphas, \
-                                dumfit, Iteration, self.direc+'gpcal/'+self.outputname+'zbl.vplot.IF'+str(k+1))
+                self.logger.info('\nCreating vplots for all baselines... It may take some time.')
                 
+                parmset = []
+
+                for l in range(len(self.zblcalsour)):
+                    for m in range(self.zbl_nant):
+                        for n in range(self.zbl_nant):
+                            if(m==n):
+                                continue
+                            dumm = m
+                            dumn = n
+                            if(m>n):
+                                dumm = n
+                                dumn = m
+                                
+                                select = (ant1 == dumm) & (ant2 == dumn) & (sourcearr == self.zblcalsour[l])
+                            
+                                selected_time, selected_day, selected_qamp, selected_qphas, selected_qsigma, selected_uamp, selected_uphas, selected_usigma, selected_mod_qamp, selected_mod_qphas, selected_mod_uamp, selected_mod_uphas = \
+                                    time[select], dayarr[select], qamp[select], qphas[select], qsigma[select], uamp[select], uphas[select], usigma[select], \
+                                    mod_qamp[select], mod_qphas[select], mod_uamp[select], mod_uphas[select]
+                                    
+                                if self.allplot:
+                                    selected_mod_pol_qamp = mod_pol_qamp[select]
+                                    selected_mod_pol_qphas = mod_pol_qphas[select]
+                                    selected_mod_pol_uamp = mod_pol_uamp[select]
+                                    selected_mod_pol_uphas = mod_pol_uphas[select]
+                                    
+                                    selected_mod_dterm_qamp = mod_dterm_qamp[select]
+                                    selected_mod_dterm_qphas = mod_dterm_qphas[select]
+                                    selected_mod_dterm_uamp = mod_dterm_uamp[select]
+                                    selected_mod_dterm_uphas = mod_dterm_uphas[select]
+                                    
+                                    allplots = (selected_mod_pol_qamp, selected_mod_pol_qphas, selected_mod_pol_uamp, selected_mod_pol_uphas, \
+                                                selected_mod_dterm_qamp, selected_mod_dterm_qphas, selected_mod_dterm_uamp, selected_mod_dterm_uphas)
+                                
+                                    
+                                if self.multiproc:
+                                    parmset.append((self.colors[l], self.zblcalsour[l], k+1, zbl_antname[dumm], zbl_antname[dumn], \
+                                                   selected_day, selected_time, selected_qamp, selected_qphas, selected_qsigma, selected_uamp, selected_uphas, selected_usigma, \
+                                                   selected_mod_qamp, selected_mod_qphas, selected_mod_uamp, selected_mod_uphas, self.direc+'gpcal/'+self.outputname+'zbl.vplot.IF'+str(k+1), self.filetype, \
+                                                   allplots, self.vplot_title, self.vplot_scanavg, self.vplot_avg_nat, self.tsep))
+                                else:
+                                    ph.visualplot(self.colors[l], self.zblcalsour[l], k+1, zbl_antname[dumm], zbl_antname[dumn], \
+                                                   selected_day, selected_time, selected_qamp, selected_qphas, selected_qsigma, selected_uamp, selected_uphas, selected_usigma, \
+                                                   selected_mod_qamp, selected_mod_qphas, selected_mod_uamp, selected_mod_uphas, self.direc+'gpcal/'+self.outputname+'zbl.vplot.IF'+str(k+1), self.filetype, \
+                                                   allplots = allplots, title = self.dataname, scanavg = self.vplot_scanavg, avg_nat = self.vplot_avg_nat, tsep = self.tsep)
+
+
+                if self.multiproc:
+                    ph.visualplot_run(parmset, nproc = self.nproc)
+                    
                 self.logger.info('...completed.\n')
             
+            
             # Create fitting residual plots if requested.
             if self.resplot:
                 self.logger.info('Creating fitting residual plots for all stations... It may take some time.')
                 self.residualplot(k, self.zbl_nant, zbl_antname, self.zblcalsour, dumfit, time, ant1, ant2, sourcearr, qamp, qphas, uamp, uphas, qsigma, usigma, self.tsep, \
                                   self.direc+'gpcal/'+self.outputname+'zbl.res.IF'+str(k+1)) 
                    
                 self.logger.info('...completed.\n')
@@ -3403,30 +2875,39 @@
             
             del self.pang1, self.pang2, self.ant1, self.ant2, self.sourcearr, self.rramp, self.rrphas, self.llamp, self.llphas 
             
         
         # Create D-term plots.
         self.dplot(-1, self.outputname+'zbl.D_Terms', zbl_antname, self.zbl_DRArr, self.zbl_DLArr, self.zblcalsour, False)
         
+        self.zbl_sourcepol.to_csv(self.direc+'gpcal/'+self.outputname+'sourcepol.txt', sep = "\t")
+        
+        
+        f = open(self.direc+'GPCAL_Difmap_v1','w')
+        
+        f.write('observe %1\nmapcolor rainbow, 1, 0.5\nselect %13, %2, %3\nmapsize %4, %5\nuvweight %6, %7\nrwin %8\nshift %9,%10\ndo i=1,100\nclean 100, 0.02, imstat(rms)*%11\nend do\nselect i\nsave %12.%13\nexit')
+            
+        f.close()
         
     
     def dtermsolve(self):    
         """
         A main function.
         """        
-                
-        self.get_data()
         
         if self.zblcal: self.zbl_dtermsolve()
         
-        self.simil_dtermsolve()
+        self.get_data()
         
+        self.simil_dtermsolve()
+                
         if self.selfpol: self.pol_dtermsolve()
         
         
+        
     def simil_dtermsolve(self):
         """
         Estimate the D-terms using the similarity assumption.
         """  
         
         # Print the basic information of the data.
         self.logger.info('\n####################################################################')
@@ -3445,53 +2926,56 @@
             if(self.antmount[i] == 4): mount = 'Nasmyth-Right'
             if(self.antmount[i] == 5): mount = 'Nasmyth-Left'
             self.logger.info('{:s}: antenna mount = {:13s}, X = {:11.2f}m, Y = {:11.2f}m, Z = {:11.2f}m'.format(self.antname[i], mount, self.antx[i], self.anty[i], self.antz[i]))
                 
         
         self.logger.info(' ')
         
-        self.logger.info('Observation date = {:s}'.format(str(self.year)+'-'+str(self.month)+'-'+str(self.day)))
+        self.logger.info('Observation date = {:s}'.format(str(np.min(self.year))+'-'+str(np.min(self.month))+'-'+str(np.min(self.day))))
         
         
         # Create pandas dataframes where the best-fit D-terms will be stored.
         self.DRArr = pd.DataFrame(index = ['IF'+str(it+1) for it in np.arange(self.ifnum)], columns = self.antname)
         self.DLArr = pd.DataFrame(index = ['IF'+str(it+1) for it in np.arange(self.ifnum)], columns = self.antname)
         
         self.DRErr = pd.DataFrame(index = ['IF'+str(it+1) for it in np.arange(self.ifnum)], columns = self.antname)
         self.DLErr = pd.DataFrame(index = ['IF'+str(it+1) for it in np.arange(self.ifnum)], columns = self.antname)
         
         
+        simil_IF, simil_ant, simil_DRArr, simil_DLArr = [], [], [], []
+        
         # Create a pandas dataframe where the best-fit source-polarization terms will be stored.
         sourcepolcolumns = []
         
         for l in range(len(self.calsour)):
             if(self.cnum[l] == 0):
                 sourcepolcolumns.append(self.calsour[l])
             else:
                 for i in range(self.cnum[l]):
                     sourcepolcolumns.append(self.calsour[l] + ', R' + str(i+1))
         
         self.sourcepol = pd.DataFrame(index = ['IF'+str(it+1) for it in np.arange(self.ifnum)], columns = sourcepolcolumns)
         
         
+        
         for k in range(self.ifnum):
             
             self.logger.info('\n####################################################################')
             self.logger.info('Processing IF {:d}'.format(k+1) + '...')
             self.logger.info('####################################################################\n')
             
             ifdata = self.data.loc[self.data["IF"] == k+1]
             
             if(np.sum(self.data["IF"] == k+1) == 0.):
                 self.logger.info('Will skip this IF because there is no data.\n')
                 continue
                   
-            time, sourcearr, pang1, pang2, ant1, ant2, rrreal, rrimag, llreal, llimag, rlreal, rlimag, lrreal, lrimag, rrsigma, llsigma, rlsigma, lrsigma, rramp, rrphas, llamp, llphas, \
+            time, dayarr, sourcearr, pang1, pang2, ant1, ant2, rrreal, rrimag, llreal, llimag, rlreal, rlimag, lrreal, lrimag, rrsigma, llsigma, rlsigma, lrsigma, rramp, rrphas, llamp, llphas, \
             qamp, qphas, uamp, uphas, qamp_sigma, qphas_sigma, uamp_sigma, uphas_sigma, qsigma, usigma = \
-                np.array(ifdata["time"]), np.array(ifdata["source"]), np.array(ifdata["pang1"]), np.array(ifdata["pang2"]), np.array(ifdata["ant1"]), np.array(ifdata["ant2"]), \
+                np.array(ifdata["time"]), np.array(ifdata["day"]), np.array(ifdata["source"]), np.array(ifdata["pang1"]), np.array(ifdata["pang2"]), np.array(ifdata["ant1"]), np.array(ifdata["ant2"]), \
                 np.array(ifdata["rrreal"]), np.array(ifdata["rrimag"]), np.array(ifdata["llreal"]), np.array(ifdata["llimag"]), \
                 np.array(ifdata["rlreal"]), np.array(ifdata["rlimag"]), np.array(ifdata["lrreal"]), np.array(ifdata["lrimag"]), \
                 np.array(ifdata["rrsigma"]), np.array(ifdata["llsigma"]), np.array(ifdata["rlsigma"]), np.array(ifdata["lrsigma"]), \
                 np.array(ifdata["rramp"]), np.array(ifdata["rrphas"]), np.array(ifdata["llamp"]), np.array(ifdata["llphas"]), \
                 np.array(ifdata["qamp"]), np.array(ifdata["qphas"]), np.array(ifdata["uamp"]), np.array(ifdata["uphas"]), \
                 np.array(ifdata["qamp_sigma"]), np.array(ifdata["qphas_sigma"]), np.array(ifdata["uamp_sigma"]), np.array(ifdata["uphas_sigma"]), np.array(ifdata["qsigma"]), np.array(ifdata["usigma"])
                 
@@ -3632,20 +3116,21 @@
             self.modphas = []
             for l in range(len(self.calsour)):            
                 if(self.cnum[l] != 0.):
                     for t in range(self.cnum[l]):
                         self.modamp.append(ifdata["model"+str(t+1)+"_amp"])
                         self.modphas.append(ifdata["model"+str(t+1)+"_phas"])
             
-           
+            
             # Perform the least-square fitting using Scipy curve_fit.
             time1 = timeit.default_timer()
             Iteration, pco = curve_fit(self.deq, inputx, inputy, p0=init, sigma = outputsigma, absolute_sigma = False, bounds = bounds)
             error = np.sqrt(np.diag(pco))
-            
+
+
             self.inputy = np.copy(inputy)
             self.outputsigma = np.copy(outputsigma)
             
             
             # Restore the original antenna numbers.
             insert_index = []
             
@@ -3663,30 +3148,33 @@
             
             
             self.logger.info('The fitting is completed within {:d} seconds.\n'.format(int(round(time2 - time1))))
             
             
             self.nant = orig_nant
             
-            ant1 = orig_ant1
-            ant2 = orig_ant2
+            ant1 = np.copy(orig_ant1)
+            ant2 = np.copy(orig_ant2)
             
-            self.ant1, self.ant2 = ant1, ant2
+            self.ant1, self.ant2 = np.copy(ant1), np.copy(ant2)
                        
             
             # Calculate the reduced chi-square of the fitting.
             dumfit = self.deq(pang1, *Iteration)
             
             ydata = np.concatenate([lrreal+1j*lrimag, rlreal+1j*rlimag])
             yfit = np.concatenate([dumfit[0:len(lrreal)]+1j*dumfit[len(lrreal):len(lrreal)*2], dumfit[len(lrreal)*2:len(lrreal)*3]+1j*dumfit[len(lrreal)*3:len(lrreal)*4]])
             ysigma = np.concatenate([lrsigma, rlsigma])
             
             chisq = np.sum(np.abs(((ydata - yfit) / ysigma) ** 2)) / (2. * len(ydata))
             
             
+            if self.zblcal:
+                self.chisq.loc["zbl", "IF"+str(k+1)] = self.zbl_chisq
+            
             self.chisq.loc["simil", "IF"+str(k+1)] = chisq
             
             self.logger.info('The reduced chi-square of the fitting is {:5.3f}.\n'.format(chisq))
             
 
             # Save the best-fit D-terms in the pandas dataframes.
             for m in range(self.nant-1):
@@ -3706,14 +3194,19 @@
             self.DLamp = pd.concat([self.DLArr.applymap(np.absolute)])
             self.DLphas = pd.concat([self.DLArr.applymap(np.angle).applymap(np.degrees)])            
         
             for m in range(self.nant):
                 self.logger.info('{:s}: RCP - amplitude = {:6.3f} %, phase = {:7.2f} deg, LCP - amplitude = {:6.3f} %, phase = {:7.2f} deg'.format(self.antname[m], \
                       self.DRamp.loc["IF"+str(k+1), self.antname[m]] * 1e2, self.DRphas.loc["IF"+str(k+1), self.antname[m]], 
                       self.DLamp.loc["IF"+str(k+1), self.antname[m]] * 1e2, self.DLphas.loc["IF"+str(k+1), self.antname[m]]))
+                
+                simil_IF.append(k+1)
+                simil_ant.append(self.antname[m])
+                simil_DRArr.append(self.DRArr.loc["IF"+str(k+1), self.antname[m]])
+                simil_DLArr.append(self.DLArr.loc["IF"+str(k+1), self.antname[m]])
             
             # Save the best-fit source-polarization terms in the pandas dataframe.
             for l in range(len(self.calsour)):
                 if(self.cnum[l] == 0):
                     self.logger.info('\n{:s} is assumed to be unpolarized.'.format(self.calsour[l].replace('.','')))
                     self.sourcepol.loc["IF"+str(k+1), self.calsour[l]] = 0.
                 else:
@@ -3733,392 +3226,294 @@
             self.sourcepolamp = pd.concat([self.sourcepol.applymap(np.absolute)])
             self.sourcepolphas = pd.concat([self.sourcepol.applymap(np.angle).applymap(np.degrees)])
             
             
             self.logger.info(' ')
             
             
-            mod_pol_qamp, mod_pol_qphas, mod_pol_uamp, mod_pol_uphas = self.deq_comp('pol', *Iteration)
-            mod_dterm_qamp, mod_dterm_qphas, mod_dterm_uamp, mod_dterm_uphas = self.deq_comp('dterm', *Iteration)
-            mod_second_qamp, mod_second_qphas, mod_second_uamp, mod_second_uphas = self.deq_comp('second', *Iteration)
-        
+            mod_lr, mod_rl = dumfit[0:len(time)] + 1j*dumfit[len(time):len(time)*2], dumfit[len(time)*2:len(time)*3] + 1j*dumfit[len(time)*3:len(time)*4]
+            mod_q, mod_u = (mod_rl + mod_lr) / 2., -1j * (mod_rl - mod_lr) / 2.
+            mod_qamp, mod_qphas, mod_uamp, mod_uphas = np.absolute(mod_q), np.angle(mod_q), np.absolute(mod_u), np.angle(mod_u)
+            
+            if self.allplot:
+                mod_pol_qamp, mod_pol_qphas, mod_pol_uamp, mod_pol_uphas = self.deq_comp('pol', *Iteration)
+                mod_dterm_qamp, mod_dterm_qphas, mod_dterm_uamp, mod_dterm_uphas = self.deq_comp('dterm', *Iteration)
+                mod_second_qamp, mod_second_qphas, mod_second_uamp, mod_second_uphas = self.deq_comp('second', *Iteration)
+                allplots = (mod_pol_qamp, mod_pol_qphas, mod_pol_uamp, mod_pol_uphas, mod_dterm_qamp, mod_dterm_qphas, mod_dterm_uamp, mod_dterm_uphas)
+            else:
+                allplots = None
+
+
             # Create vplots if requested.
             if self.vplot:
-                self.logger.info('Creating vplots for all baselines... It may take some time.')
-                self.visualplot(k, self.nant, self.antname, self.calsour, time, ant1, ant2, sourcearr, qamp, qphas, uamp, uphas, qamp_sigma, qphas_sigma, uamp_sigma, uphas_sigma, \
-                                mod_pol_qamp, mod_pol_qphas, mod_pol_uamp, mod_pol_uphas, mod_dterm_qamp, mod_dterm_qphas, mod_dterm_uamp, mod_dterm_uphas, mod_second_qamp, mod_second_qphas, mod_second_uamp, mod_second_uphas, \
-                                dumfit, Iteration, self.direc+'gpcal/'+self.outputname+'vplot.IF'+str(k+1))
+                self.logger.info('\nCreating vplots for all baselines... It may take some time.')
+                
+                parmset = []
 
+                for l in range(len(self.calsour)):
+                    for m in range(self.nant):
+                        for n in range(self.nant):
+                            if(m==n):
+                                continue
+                            dumm = m
+                            dumn = n
+                            if(m>n):
+                                dumm = n
+                                dumn = m
+                                
+                                select = (ant1 == dumm) & (ant2 == dumn) & (sourcearr == self.calsour[l])
+                            
+                                selected_time, selected_day, selected_qamp, selected_qphas, selected_qsigma, selected_uamp, selected_uphas, selected_usigma, selected_mod_qamp, selected_mod_qphas, selected_mod_uamp, selected_mod_uphas = \
+                                    time[select], dayarr[select], qamp[select], qphas[select], qsigma[select], uamp[select], uphas[select], usigma[select], \
+                                    mod_qamp[select], mod_qphas[select], mod_uamp[select], mod_uphas[select]
+                                    
+                                if self.allplot:
+                                    selected_mod_pol_qamp = mod_pol_qamp[select]
+                                    selected_mod_pol_qphas = mod_pol_qphas[select]
+                                    selected_mod_pol_uamp = mod_pol_uamp[select]
+                                    selected_mod_pol_uphas = mod_pol_uphas[select]
+                                    
+                                    selected_mod_dterm_qamp = mod_dterm_qamp[select]
+                                    selected_mod_dterm_qphas = mod_dterm_qphas[select]
+                                    selected_mod_dterm_uamp = mod_dterm_uamp[select]
+                                    selected_mod_dterm_uphas = mod_dterm_uphas[select]
+                                    
+                                    allplots = (selected_mod_pol_qamp, selected_mod_pol_qphas, selected_mod_pol_uamp, selected_mod_pol_uphas, \
+                                                selected_mod_dterm_qamp, selected_mod_dterm_qphas, selected_mod_dterm_uamp, selected_mod_dterm_uphas)
+                                
+                                
+                                if self.multiproc:
+                                    parmset.append((self.colors[l], self.calsour[l], k+1, self.antname[dumm], self.antname[dumn], \
+                                                    selected_day, selected_time, selected_qamp, selected_qphas, selected_qsigma, selected_uamp, selected_uphas, selected_usigma, \
+                                                    selected_mod_qamp, selected_mod_qphas, selected_mod_uamp, selected_mod_uphas, self.direc+'gpcal/'+self.outputname+'vplot.IF'+str(k+1), self.filetype, \
+                                                    allplots, self.vplot_title, self.vplot_scanavg, self.vplot_avg_nat, self.tsep))
+                                else:
+                                    ph.visualplot(self.calsour[l], k+1, self.antname[dumm], self.antname[dumn], \
+                                                    selected_day, selected_time, selected_qamp, selected_qphas, selected_qsigma, selected_uamp, selected_uphas, selected_usigma, \
+                                                    selected_mod_qamp, selected_mod_qphas, selected_mod_uamp, selected_mod_uphas, self.direc+'gpcal/'+self.outputname+'vplot.IF'+str(k+1), self.filetype, \
+                                                    allplots = allplots, title = self.dataname, scanavg = self.vplot_scanavg, avg_nat = self.vplot_avg_nat, tsep = self.tsep, color = self.colors[l])
+                                            
+                if self.multiproc:
+                    ph.visualplot_run(parmset, nproc = self.nproc)
+                    
                 self.logger.info('...completed.\n')
-                
+            
+                        
             # Create fitting residual plots if requested.
             if self.resplot:
                 self.logger.info('Creating fitting residual plots for all stations... It may take some time.')
-                self.residualplot(k, self.nant, self.antname, self.calsour, dumfit, time, ant1, ant2, sourcearr, qamp, qphas, uamp, uphas, qsigma, usigma, self.tsep, \
-                   self.direc+'gpcal/'+self.outputname+'res.IF'+str(k+1))
-                   
+                # self.residualplot(k, self.nant, self.antname, self.calsour, dumfit, time, ant1, ant2, sourcearr, qamp, qphas, uamp, uphas, qsigma, usigma, self.tsep, \
+                #    self.direc+'gpcal/'+self.outputname+'res.IF'+str(k+1))
+
+                ph.residualplot(self.markerarr, self.colors, dayarr, k, self.nant, self.antname, self.calsour, \
+                                dumfit, time, ant1, ant2, sourcearr, qamp, qphas, uamp, uphas, qsigma, usigma, self.direc+'gpcal/'+self.outputname+'res.IF'+str(k+1), tsep = 2. / 60., title = self.dataname, filetype = self.filetype)
+                    
                 self.logger.info('...completed.\n')
                 
             del self.pang1, self.pang2, self.ant1, self.ant2, self.sourcearr, self.rramp, self.rrphas, self.llamp, self.llphas 
             
         
+        simil_IF, simil_ant, simil_DRArr, simil_DLArr = np.array(simil_IF), np.array(simil_ant), np.array(simil_DRArr), np.array(simil_DLArr)
+        
+        
         # Create D-term plots.
         self.dplot(-1, self.outputname+'D_Terms', self.antname, self.DRArr, self.DLArr, self.calsour, lpcal=self.lpcal)
         
         
         # Produce the D-term corrected UVFITS files in the working directory.
         self.applydterm(self.source, self.DRArr, self.DLArr)
-        
+                
         # Save the fitting results into ASCII files.
         self.chisq.to_csv(self.direc+'gpcal/'+self.outputname+'chisq.txt', sep = "\t")
         self.sourcepol.to_csv(self.direc+'gpcal/'+self.outputname+'sourcepol.txt', sep = "\t")
         self.DRArr.to_csv(self.direc+'gpcal/'+self.outputname+'DRArr.txt', sep = "\t")
         self.DLArr.to_csv(self.direc+'gpcal/'+self.outputname+'DLArr.txt', sep = "\t")
         
+        
+        
+        df = pd.DataFrame(simil_IF.transpose())
+        df['antennas'] = np.array(simil_ant)
+        df['IF'] = np.array(simil_IF)
+        df['DRArr'] = np.array(simil_DRArr)
+        df['DLArr'] = np.array(simil_DLArr)
+        del df[0]
+        
+        df.to_csv(self.direc+'gpcal/'+self.outputname+'dterm.csv', sep = "\t")
+        
 
 
-    def pol_gpcal(self, spoliter):
+    def pol_dtermsolve(self):
         """
-        Estimate the D-terms using instrumental polarization self-calibration.
+        Estimate the D-terms using instrumental polarization self-calibration. Iterate (i) obtaining D-term solutions and (ii) modeling calibrators Stokes Q and U models with CLEAN as many times as specified by users.
+        """ 
         
-        Args:
-            spoliter (int): the number of iteration of instrumental polarization self-calibration.
-        """  
+        # Create D-term plots.
+        self.dplot(0, self.outputname+'pol.iter{:02d}'.format(0)+'.D_Terms', self.antname, self.DRArr, self.DLArr, self.calsour, lpcal=False)
+                
+        # Get the data to be used for the D-term estimation using instrumental polarization self-calibraiton
+        self.get_pol_data()
         
-        # Create pandas dataframes where the best-fit D-terms will be stored.
-        self.pol_DRArr = pd.DataFrame(index = ['IF'+str(it+1) for it in np.arange(self.ifnum)], columns = self.antname)
-        self.pol_DLArr = pd.DataFrame(index = ['IF'+str(it+1) for it in np.arange(self.ifnum)], columns = self.antname)
         
-        self.pol_DRErr = pd.DataFrame(index = ['IF'+str(it+1) for it in np.arange(self.ifnum)], columns = self.antname)
-        self.pol_DLErr = pd.DataFrame(index = ['IF'+str(it+1) for it in np.arange(self.ifnum)], columns = self.antname)
+        if(type(self.ms) == int) | (type(self.ms) == float):
+            self.ms = [self.ms] * len(self.polcalsour)
+        if(type(self.ps) == int) | (type(self.ps) == float):
+            self.ps = [self.ps] * len(self.polcalsour)
+        if(type(self.uvbin) == int) | (type(self.uvbin) == float):
+            self.uvbin = [self.uvbin] * len(self.polcalsour)
+        if(type(self.uvpower) == int) | (type(self.uvpower) == float):
+            self.uvpower = [self.uvpower] * len(self.polcalsour)
+        if(type(self.dynam) == int) | (type(self.dynam) == float):
+            self.dynam = [self.dynam] * len(self.polcalsour)
+        if(type(self.shift_x) == int) | (type(self.shift_x) == float):
+            self.shift_x = [self.shift_x] * len(self.polcalsour)
+        if(type(self.shift_y) == int) | (type(self.shift_y) == float):
+            self.shift_y = [self.shift_y] * len(self.polcalsour)
         
         
-        for k in range(self.ifnum):
-            
-            self.logger.info('\n####################################################################')
-            self.logger.info('Processing IF {:d}'.format(k+1) + '...')
-            self.logger.info('####################################################################\n')
-            
-            self.logger.info('Instrumental polarization self-calibration mode...')
-            self.logger.info('Iteration: {:d}/{:d}\n'.format(spoliter+1, self.selfpoliter))
-
-
-            ifdata = self.pol_data.loc[self.pol_data["IF"] == k+1]
-            
-            if(np.sum(self.pol_data["IF"] == k+1) == 0.):
-                self.logger.info('Will skip this IF because there is no data.\n')
-                continue
-                  
-            time, sourcearr, pang1, pang2, ant1, ant2, rrreal, rrimag, llreal, llimag, rlreal, rlimag, lrreal, lrimag, rrsigma, llsigma, rlsigma, lrsigma, rramp, rrphas, llamp, llphas, \
-            qamp, qphas, uamp, uphas, qamp_sigma, qphas_sigma, uamp_sigma, uphas_sigma, qsigma, usigma, \
-            model_rlreal, model_rlimag, model_lrreal, model_lrimag, model_rlamp, model_rlphas, model_lramp, model_lrphas, model_qamp, model_qphas, model_uamp, model_uphas = \
-                np.array(ifdata["time"]), np.array(ifdata["source"]), np.array(ifdata["pang1"]), np.array(ifdata["pang2"]), np.array(ifdata["ant1"]), np.array(ifdata["ant2"]), \
-                np.array(ifdata["rrreal"]), np.array(ifdata["rrimag"]), np.array(ifdata["llreal"]), np.array(ifdata["llimag"]), \
-                np.array(ifdata["rlreal"]), np.array(ifdata["rlimag"]), np.array(ifdata["lrreal"]), np.array(ifdata["lrimag"]), \
-                np.array(ifdata["rrsigma"]), np.array(ifdata["llsigma"]), np.array(ifdata["rlsigma"]), np.array(ifdata["lrsigma"]), \
-                np.array(ifdata["rramp"]), np.array(ifdata["rrphas"]), np.array(ifdata["llamp"]), np.array(ifdata["llphas"]), \
-                np.array(ifdata["qamp"]), np.array(ifdata["qphas"]), np.array(ifdata["uamp"]), np.array(ifdata["uphas"]), \
-                np.array(ifdata["qamp_sigma"]), np.array(ifdata["qphas_sigma"]), np.array(ifdata["uamp_sigma"]), np.array(ifdata["uphas_sigma"]), np.array(ifdata["qsigma"]), np.array(ifdata["usigma"]), \
-                np.array(ifdata["model_rlreal"]), np.array(ifdata["model_rlimag"]), np.array(ifdata["model_lrreal"]), np.array(ifdata["model_lrimag"]), \
-                np.array(ifdata["model_rlamp"]), np.array(ifdata["model_rlphas"]), np.array(ifdata["model_lramp"]), np.array(ifdata["model_lrphas"]), \
-                np.array(ifdata["model_qamp"]), np.array(ifdata["model_qphas"]), np.array(ifdata["model_uamp"]), np.array(ifdata["model_uphas"])
-                
-            
-            # Draw field-rotation angle plots if requested.
-            if self.parplot: 
-                self.logger.info('Creating field-rotation-angle plots...\n')
-                self.parangplot(k, self.nant, self.antname, self.polcalsour, time, ant1, ant2, sourcearr, pang1, pang2, self.direc+'gpcal/'+self.outputname+'pol.FRA.IF'+str(k+1))
-            
-            
-            inputx = np.concatenate([pang1, pang2, pang1, pang2])
-            inputy = np.concatenate([lrreal, lrimag, rlreal, rlimag])
+        
+        f = open(self.direc+'GPCAL_Difmap_v1','w')
+        f.write('observe %1\nmapcolor rainbow, 1, 0.5\nselect %13, %2, %3\nmapsize %4, %5\nuvweight %6, %7\nrwin %8\nshift %9,%10\ndo i=1,100\nclean 100, 0.02, imstat(rms)*%11\nend do\nselect i\nsave %12.%13\nexit')
+        f.close()
             
-            inputsigma = np.concatenate([lrsigma, lrsigma, rlsigma, rlsigma])
+        
+        # Iterate (i) obtaining D-term solutions and (ii) modeling calibrators Stokes Q and U models with CLEAN as many times as specified by users.
+        for spoliter in range(self.selfpoliter):
+            # Obtain Stokes Q and U models of the calibrators with CLEAN in Difmap.
             
             
-            # Rescale the visibility weights of specific stations if requested.
-            if self.manualweight:
+            if self.multiproc:
+                parmset = []
                 
-                sigmaant1 = np.concatenate([ant1, ant1, ant1, ant1])
-                sigmaant2 = np.concatenate([ant2, ant2, ant2, ant2])
-                
-                outputweight = 1. / inputsigma ** 2
-                for m in range(self.nant):
-                    if(self.antname[m] in self.weightfactors):
-                        outputweight[(sigmaant1 == m) | (sigmaant2 == m)] = outputweight[(sigmaant1 == m) | (sigmaant2 == m)] * self.weightfactors.get(self.antname[m])
-                        self.logger.info('The visibility weights for {:s} station are rescaled by a factor of {:4.2f}.'.format(self.antname[m], self.weightfactors.get(self.antname[m])))
+            for l in range(len(self.polcalsour)):
+                if self.polcal_unpol[l]:
+                    self.logger.info('Skip CLEAN for {:s} because it was assumed to be unpolarized...'.format(self.polcalsour[l]))
+                    continue
                 
-                self.logger.info(' ')
+                # self.logger.info('Making CLEAN models for Stokes Q & U maps for {:s}...'.format(self.polcalsour[l]))
                 
-                outputsigma = 1. / outputweight ** (1. / 2.)
-                
-            else:
-                outputsigma = np.copy(inputsigma)
-                self.logger.info('No visibility weight rescaling applied.\n')
-            
-            
-            
-            dumantname = np.copy(self.antname)
-            orig_ant1 = np.copy(ant1)
-            orig_ant2 = np.copy(ant2)
-            
-            
-            orig_nant = self.nant
-            
-            
-            #If there are antennas having no data, then rearrange the antenna numbers for fitting. This change will be reverted after the fitting.
-            dum = 0
-            
-            removed_Index = []
-            
-            
-            for m in range(orig_nant):
-                if((sum(ant1 == dum) == 0) & (sum(ant2 == dum) == 0)):
-                    ant1[ant1 > dum] -= 1
-                    ant2[ant2 > dum] -= 1
-                    self.nant -= 1
-                    removed_Index.append(m)
-                    self.logger.info('{:s} has no data, the fitting will not solve the D-Terms for it.'.format(self.antname[m]))
-                else:
-                    dum += 1
-            
-            if(len(removed_Index) != 0): dumantname = np.delete(dumantname, removed_Index)
-            
-            if(k == 0): 
-                init = np.zeros(2*2*self.nant)
-            else:
-                if('Iteration' in locals()):
-                    init = Iteration
-                    if(len(removed_Index) != 0.):
-                        dum = []
-                        for it in removed_Index:
-                            dum.append(2*it)
-                            dum.append(2*it+1)
-                            dum.append(2*orig_nant + 2*it)
-                            dum.append(2*orig_nant + 2*it+1)
-                        init = np.delete(init, dum)
-                else:
-                    init = np.zeros(2*2*self.nant)
-            
-            
-            # The boundaries of parameters allowed for the least-square fitting.
-            lbound = [-self.Dbound]*(2*2*self.nant)
-            ubound = [self.Dbound]*(2*2*self.nant)
-            
-            
-            if not self.pol_fixdterm:
-                self.fixdr = None
-                self.fixdl = None
-            
-            # If the zero-baseline D-term estimation was performed, then fix the D-terms of those stations for fitting for the rest of the array.
-            if self.zblcal:
-                if(self.fixdr == None):
-                    self.fixdr = {}
-                    self.fixdl = {}
-                for i in range(len(self.zblant)):
-                    if(self.zblant[i][0] in self.fixdr):
-                        self.fixdr[self.zblant[i][0]] = self.zbl_DRArr.loc["IF"+str(k+1), self.zblant[i][0]]
-                        self.fixdl[self.zblant[i][0]] = self.zbl_DLArr.loc["IF"+str(k+1), self.zblant[i][0]]
+                if(spoliter == 0): 
+
+                    if self.pol_IF_combine:
+                        bif = 1
+                        eif = self.ifnum
+                        ch.cleanqu(self.direc, self.outputname+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.allIF', \
+                                   bif, eif, self.ms[l], self.ps[l], self.uvbin[l], self.uvpower[l], self.dynam[l], self.shift_x[l], self.shift_y[l], 'q')
+                        ch.cleanqu(self.direc, self.outputname+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.allIF', \
+                                   bif, eif, self.ms[l], self.ps[l], self.uvbin[l], self.uvpower[l], self.dynam[l], self.shift_x[l], self.shift_y[l], 'u')
+                        
+                        self.logger.info('\nMaking CLEAN models for Stokes Q & U maps using a single core...\n')
+                        
+                        self.logger.info('uvfits file: {:s}, CLEAN mask: {:s}, save file: {:s}\n'.format(self.outputname+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', \
+                                          self.dataname+self.polcalsour[l] + '.allIF.q,u'))
+                            
                     else:
-                        self.fixdr.update({self.zblant[i][0]: self.zbl_DRArr.loc["IF"+str(k+1), self.zblant[i][0]]})
-                        self.fixdl.update({self.zblant[i][0]: self.zbl_DLArr.loc["IF"+str(k+1), self.zblant[i][0]]})
+                        
+                        if self.multiproc:
+                            
+                            for ifn in range(self.ifnum):
+                                bif = ifn + 1
+                                eif = ifn + 1
+                                parmset.append([self.direc, self.outputname+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.IF{:}'.format(ifn+1), \
+                                           bif, eif, self.ms[l], self.ps[l], self.uvbin[l], self.uvpower[l], self.dynam[l], self.shift_x[l], self.shift_y[l], 'q'])
+                                parmset.append([self.direc, self.outputname+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.IF{:}'.format(ifn+1), \
+                                            bif, eif, self.ms[l], self.ps[l], self.uvbin[l], self.uvpower[l], self.dynam[l], self.shift_x[l], self.shift_y[l], 'u'])
+                            
+                        else:
+                            
+                            for ifn in range(self.ifnum):
+                                bif = ifn + 1
+                                eif = ifn + 1
+                                ch.cleanqu(self.direc, self.outputname+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.IF{:}'.format(ifn+1), \
+                                            bif, eif, self.ms[l], self.ps[l], self.uvbin[l], self.uvpower[l], self.dynam[l], self.shift_x[l], self.shift_y[l], 'q')
+                                ch.cleanqu(self.direc, self.outputname+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.IF{:}'.format(ifn+1), \
+                                            bif, eif, self.ms[l], self.ps[l], self.uvbin[l], self.uvpower[l], self.dynam[l], self.shift_x[l], self.shift_y[l], 'u')
+                                
+                                self.logger.info('\nMaking CLEAN models for Stokes Q & U maps using a single core...\n')
+                                
+                                self.logger.info('uvfits file: {:s}, CLEAN mask: {:s}, save file: {:s}\n'.format(self.outputname+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', \
+                                                  self.dataname+self.polcalsour[l] + '.IF{:}.q,u'.format(ifn+1)))
+                        
+                        
+                else:
                     
-                    if(self.zblant[i][1] in self.fixdr):
-                        self.fixdr[self.zblant[i][1]] = self.zbl_DRArr.loc["IF"+str(k+1), self.zblant[i][1]]
-                        self.fixdl[self.zblant[i][1]] = self.zbl_DLArr.loc["IF"+str(k+1), self.zblant[i][1]]
-                    else:
-                        self.fixdr.update({self.zblant[i][1]: self.zbl_DRArr.loc["IF"+str(k+1), self.zblant[i][1]]})
-                        self.fixdl.update({self.zblant[i][1]: self.zbl_DLArr.loc["IF"+str(k+1), self.zblant[i][1]]})
-
-            
-            # If the D-terms of some stations are requested to be transferred from the initial estimation using the similarity assumption, then fix those D-terms for fitting.
-            if self.transferdterm:
-                if(self.fixdr == None):
-                    self.fixdr = {}
-                    self.fixdl = {}
-                for i in range(len(self.transferdtermant)):
-                    self.fixdr[dumantname[i]] = self.DRArr.loc["IF"+str(k+1),self.transferdtermant[i]]
-                    self.fixdl[dumantname[i]] = self.DLArr.loc["IF"+str(k+1),self.transferdtermant[i]]
-
-
-            # Fix the D-terms of specific stations to be certain values for fitting if requested.
-            if (self.pol_fixdterm == True) | (self.zblcal == True) | (self.transferdterm == True):
-                
-                for i in range(self.nant):
-                    if dumantname[i] in self.fixdr:
-                        lbound[2*i] = np.real(self.fixdr.get(dumantname[i])) - 1e-8
-                        ubound[2*i] = np.real(self.fixdr.get(dumantname[i])) + 1e-8
-                        lbound[2*i+1] = np.imag(self.fixdr.get(dumantname[i])) - 1e-8
-                        ubound[2*i+1] = np.imag(self.fixdr.get(dumantname[i])) + 1e-8
-                        lbound[2*self.nant+2*i] = np.real(self.fixdl.get(dumantname[i])) - 1e-8
-                        ubound[2*self.nant+2*i] = np.real(self.fixdl.get(dumantname[i])) + 1e-8
-                        lbound[2*self.nant+2*i+1] = np.imag(self.fixdl.get(dumantname[i])) - 1e-8
-                        ubound[2*self.nant+2*i+1] = np.imag(self.fixdl.get(dumantname[i])) + 1e-8
-                        init[2*i] = np.real(self.fixdr.get(dumantname[i]))
-                        init[2*i+1] = np.imag(self.fixdr.get(dumantname[i]))
-                        init[2*self.nant+2*i] = np.real(self.fixdl.get(dumantname[i]))
-                        init[2*self.nant+2*i+1] = np.imag(self.fixdl.get(dumantname[i]))
+                    if self.pol_IF_combine:
+                        
+                        bif = 1
+                        eif = self.ifnum
+                        ch.cleanqu(self.direc, self.outputname+'pol.iter'+str(spoliter)+'.'+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.allIF', \
+                                   bif, eif, self.ms[l], self.ps[l], self.uvbin[l], self.uvpower[l], self.dynam[l], self.shift_x[l], self.shift_y[l], 'q')
+                        ch.cleanqu(self.direc, self.outputname+'pol.iter'+str(spoliter)+'.'+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.allIF', \
+                                   bif, eif, self.ms[l], self.ps[l], self.uvbin[l], self.uvpower[l], self.dynam[l], self.shift_x[l], self.shift_y[l], 'u')
                     
-            
-            bounds=(lbound,ubound)
-            
-            # Define global variables to be transferred into the fitting functions.
-            self.pang1, self.pang2, self.ant1, self.ant2, self.sourcearr, self.rramp, self.rrphas, self.llamp, self.llphas, \
-            self.model_rlreal, self.model_rlimag, self.model_rlamp, self.model_rlphas, self.model_lrreal, self.model_lrimag, self.model_lramp, self.model_lrphas= \
-                pang1, pang2, ant1, ant2, sourcearr, rramp, rrphas, llamp, llphas, model_rlreal, model_rlimag, model_rlamp, model_rlphas, model_lrreal, model_lrimag, model_lramp, model_lrphas
-            
-            
-            # Perform the least-square fitting using Scipy curve_fit.
-            time1 = timeit.default_timer()
-            Iteration, pco = curve_fit(self.pol_deq, pang1, inputy, p0=init, sigma = outputsigma, absolute_sigma = False, bounds = bounds)
-            error = np.sqrt(np.diag(pco))
-        
-        
-            # Restore the original antenna numbers.
-            insert_index = []
-            
-            dum = 0
-            for it in removed_Index:
-                insert_index.append(2*it - 2*dum)
-                insert_index.append(2*it - 2*dum)
-                insert_index.append(2*self.nant + 2*it - 2*dum)
-                insert_index.append(2*self.nant + 2*it - 2*dum)
-                dum += 1
-                
-            Iteration = np.insert(Iteration, insert_index, [0.]*len(insert_index))
-            error = np.insert(error, insert_index, [0.]*len(insert_index))
-            time2 = timeit.default_timer()
-            
-            self.logger.info('The fitting is completed within {:d} seconds.\n'.format(int(round(time2 - time1))))
-            
-
-
-            self.nant = orig_nant
-            
-            ant1 = orig_ant1
-            ant2 = orig_ant2
+                        self.logger.info('\nMaking CLEAN models for Stokes Q & U maps using a single core...\n')
+                        
+                        self.logger.info('uvfits file: {:s}, CLEAN mask: {:s}, save file: {:s}\n'.format(self.outputname+'pol.iter'+str(spoliter)+'.'+self.polcalsour[l]+'.dtcal.uvf', \
+                                                                                                         self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.allIF.q,u'))
+                            
+                    else:
+                        
+                        if self.multiproc:
+                            for ifn in range(self.ifnum):
+                                bif = ifn + 1
+                                eif = ifn + 1
+                                parmset.append([self.direc, self.outputname+'pol.iter'+str(spoliter)+'.'+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.IF{:}'.format(ifn+1), \
+                                           bif, eif, self.ms[l], self.ps[l], self.uvbin[l], self.uvpower[l], self.dynam[l], self.shift_x[l], self.shift_y[l], 'q'])
+                                parmset.append([self.direc, self.outputname+'pol.iter'+str(spoliter)+'.'+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.IF{:}'.format(ifn+1), \
+                                           bif, eif, self.ms[l], self.ps[l], self.uvbin[l], self.uvpower[l], self.dynam[l], self.shift_x[l], self.shift_y[l], 'u'])
+                            
+                                    
+                        else:
+                            for ifn in range(self.ifnum):
+                                bif = ifn + 1
+                                eif = ifn + 1
+                                ch.cleanqu(self.direc, self.outputname+'pol.iter'+str(spoliter)+'.'+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.IF{:}'.format(ifn+1), \
+                                           bif, eif, self.ms[l], self.ps[l], self.uvbin[l], self.uvpower[l], self.dynam[l], self.shift_x[l], self.shift_y[l], 'q')
+                                ch.cleanqu(self.direc, self.outputname+'pol.iter'+str(spoliter)+'.'+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.IF{:}'.format(ifn+1), \
+                                           bif, eif, self.ms[l], self.ps[l], self.uvbin[l], self.uvpower[l], self.dynam[l], self.shift_x[l], self.shift_y[l], 'u')
+                                
+                                self.logger.info('\nMaking CLEAN models for Stokes Q & U maps using a single core...\n')
+                                
+                                self.logger.info('uvfits file: {:s}, CLEAN mask: {:s}, save file: {:s}\n'.format(self.outputname+'pol.iter'+str(spoliter)+'.'+self.polcalsour[l]+'.dtcal.uvf', \
+                                                                                                                 self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l] + '.IF{:}.q,u'.format(ifn+1)))
             
             
-            # Save the best-fit D-terms in the pandas dataframes.
-            for m in range(self.nant-1):
-                for n in np.arange(m+1, self.nant):
-                    self.pol_DRArr.loc["IF"+str(k+1), self.antname[m]] = Iteration[2*m] + 1j*Iteration[2*m+1]
-                    self.pol_DRArr.loc["IF"+str(k+1), self.antname[n]] = Iteration[2*n] + 1j*Iteration[2*n+1]
-                    self.pol_DLArr.loc["IF"+str(k+1), self.antname[m]] = Iteration[2*self.nant+2*m] + 1j*Iteration[2*self.nant+2*m+1]
-                    self.pol_DLArr.loc["IF"+str(k+1), self.antname[n]] = Iteration[2*self.nant+2*n] + 1j*Iteration[2*self.nant+2*n+1]
-
-                    self.pol_DRErr.loc["IF"+str(k+1), self.antname[m]] = error[2*m] + 1j*error[2*m+1]
-                    self.pol_DRErr.loc["IF"+str(k+1), self.antname[n]] = error[2*n] + 1j*error[2*n+1]
-                    self.pol_DLErr.loc["IF"+str(k+1), self.antname[m]] = error[2*self.nant+2*m] + 1j*error[2*self.nant+2*m+1]
-                    self.pol_DLErr.loc["IF"+str(k+1), self.antname[n]] = error[2*self.nant+2*n] + 1j*error[2*self.nant+2*n+1]
+            if self.multiproc:                
+                pool = Pool(processes = self.nproc)
+                pool.map(ch.cleanqu2, parmset)
+                pool.close()
+                pool.join()
                 
+                self.logger.info('\nMaking CLEAN models for Stokes Q & U maps using multiple cores...\n')
                 
-            self.pol_DRamp = pd.concat([self.pol_DRArr.applymap(np.absolute)])
-            self.pol_DRphas = pd.concat([self.pol_DRArr.applymap(np.angle).applymap(np.degrees)])
-            self.pol_DLamp = pd.concat([self.pol_DLArr.applymap(np.absolute)])
-            self.pol_DLphas = pd.concat([self.pol_DLArr.applymap(np.angle).applymap(np.degrees)])
-            
+                for i in range(len(parmset)):
+                    self.logger.info('uvfits file: {:s}, CLEAN mask: {:s}, save file: {:s}.q,u'.format(parmset[i][1], parmset[i][2], parmset[i][3]))
             
-            self.ant1, self.ant2 = ant1, ant2
-            
-            
-            # Calculate the reduced chi-square of the fitting.
-            dumfit = self.pol_deq(pang1, *Iteration)
-
-            ydata = np.concatenate([lrreal+1j*lrimag, rlreal+1j*rlimag])
-            yfit = np.concatenate([dumfit[0:len(lrreal)]+1j*dumfit[len(lrreal):len(lrreal)*2], dumfit[len(lrreal)*2:len(lrreal)*3]+1j*dumfit[len(lrreal)*3:len(lrreal)*4]])
-            ysigma = np.concatenate([lrsigma, rlsigma])
-            
-            chisq = np.sum(np.abs(((ydata - yfit) / ysigma) ** 2)) / (2. * len(ydata))
-            
-            dumsigma = (inputy - dumfit) ** 2 / inputsigma ** 2
-            
-            self.chisq.loc["pol_iter"+str(spoliter+1), "IF"+str(k+1)] = chisq
-            
-            self.logger.info('The reduced chi-square of the fitting is {:5.3f}.\n'.format(chisq))
-            
-            for m in range(self.nant):
-                self.logger.info('{:s}: RCP - amplitude = {:6.3f} %, phase = {:7.2f} deg, RCP - amplitude = {:6.3f} %, phase = {:7.2f} deg'.format(self.antname[m], \
-                      self.pol_DRamp.loc["IF"+str(k+1), self.antname[m]] * 1e2, self.pol_DRphas.loc["IF"+str(k+1), self.antname[m]], 
-                      self.pol_DLamp.loc["IF"+str(k+1), self.antname[m]] * 1e2, self.pol_DLphas.loc["IF"+str(k+1), self.antname[m]]))
-        
             
+            # Extract visibility models using the CLEAN Stokes Q and U models.
+            self.pol_data = oh.get_model(self.pol_data, self.direc, self.dataname, self.polcalsour, self.polcal_unpol, self.ifnum, self.pol_IF_combine, selfcal = self.selfcal, outputname = self.outputname)
             
-            mod_pol_qamp, mod_pol_qphas, mod_pol_uamp, mod_pol_uphas = self.pol_deq_comp('pol', *Iteration)
-            mod_dterm_qamp, mod_dterm_qphas, mod_dterm_uamp, mod_dterm_uphas = self.pol_deq_comp('dterm', *Iteration)
-            mod_second_qamp, mod_second_qphas, mod_second_uamp, mod_second_uphas = self.pol_deq_comp('second', *Iteration)
+            curdirec = os.getcwd()
             
+            os.chdir(self.direc)
             
-            self.logger.info(' ')
-        
-            # Create vplots if requested.
-            if self.vplot:
-                if(spoliter == self.selfpoliter-1):
-                    self.logger.info('Creating vplots for all baselines... It may take some time.')
-                    self.visualplot(k, self.nant, self.antname, self.polcalsour, time, ant1, ant2, sourcearr, qamp, qphas, uamp, uphas, qamp_sigma, qphas_sigma, uamp_sigma, uphas_sigma, \
-                                    mod_pol_qamp, mod_pol_qphas, mod_pol_uamp, mod_pol_uphas, mod_dterm_qamp, mod_dterm_qphas, mod_dterm_uamp, mod_dterm_uphas, mod_second_qamp, mod_second_qphas, mod_second_uamp, mod_second_uphas, \
-                                    dumfit, Iteration, self.direc+'gpcal/'+self.outputname+'pol.vplot.IF'+str(k+1))
-                    
-                    self.logger.info('...completed.\n')
+            os.system('rm {:}difmap.log*')
             
-            # Create fitting residual plots if requested.
-            if self.resplot:
-                if(spoliter == self.selfpoliter-1):
-                    self.logger.info('Creating fitting residual plots for all stations... It may take some time.')
-                    self.residualplot(k, self.nant, self.antname, self.polcalsour, dumfit, time, ant1, ant2, sourcearr, qamp, qphas, uamp, uphas, qsigma, usigma, self.tsep, \
-                       self.direc+'gpcal/'+self.outputname+'pol.res.IF'+str(k+1))
-                       
-                    self.logger.info('...completed.\n')
+            os.chdir(curdirec)
             
             
-            del self.pang1, self.pang2, self.ant1, self.ant2, self.sourcearr, self.rramp, self.rrphas, self.llamp, self.llphas, \
-            self.model_rlreal, self.model_rlimag, self.model_rlamp, self.model_rlphas, self.model_lrreal, self.model_lrimag, self.model_lramp, self.model_lrphas
-        
-
-    
-    def pol_dtermsolve(self):
-        """
-        Estimate the D-terms using instrumental polarization self-calibration. Iterate (i) obtaining D-term solutions and (ii) modeling calibrators Stokes Q and U models with CLEAN as many times as specified by users.
-        """ 
-        
-        # Create D-term plots.
-        self.dplot(0, self.outputname+'pol.iter{:02d}'.format(0)+'.D_Terms', self.antname, self.DRArr, self.DLArr, self.calsour, lpcal=False)
-                
-        # Get the data to be used for the D-term estimation using instrumental polarization self-calibraiton
-        self.get_pol_data()
-        
-        # Iterate (i) obtaining D-term solutions and (ii) modeling calibrators Stokes Q and U models with CLEAN as many times as specified by users.
-        for spoliter in range(self.selfpoliter):
-            # Obtain Stokes Q and U models of the calibrators with CLEAN in Difmap.
-            for l in range(len(self.polcalsour)):
-                
-                self.logger.info('Making CLEAN models for Stokes Q & U maps for {:s}...'.format(self.polcalsour[l]))
-                
-                if self.difmaplog:
-                    difmaplogfile = self.direc+'gpcal/'+self.dataname+'difmap.log'
-                else:
-                    difmaplogfile = '/dev/null 2>&1'
+            if self.pol_IF_combine:
+                for l in range(len(self.polcalsour)):
+                    os.system('rm {:}{:}{:}.allIF.q.*'.format(self.direc, self.dataname, self.polcalsour[l]))
+                    os.system('rm {:}{:}{:}.allIF.u.*'.format(self.direc, self.dataname, self.polcalsour[l]))
+            else:
+                for ifn in range(self.ifnum):
+                    for l in range(len(self.polcalsour)):
+                        os.system('rm {:}{:}{:}.IF{:}.q.*'.format(self.direc, self.dataname, self.polcalsour[l], ifn+1))
+                        os.system('rm {:}{:}{:}.IF{:}.u.*'.format(self.direc, self.dataname, self.polcalsour[l], ifn+1))
                         
-                if(spoliter == 0): 
-                    self.logger.info('uvfits file: {:s}, CLEAN mask: {:s}, save file: {:s}\n'.format(self.dataname+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', \
-                                     self.dataname+self.polcalsour[l]+'.IF*.q,u'))
-                    self.cleanqu(self.dataname+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l], difmaplogfile)
-                    if self.difmaplog:
-                        os.system('cat ' + self.logfile + ' ' + difmaplogfile + ' > ' + self.direc+'gpcal/'+'temp.log')
-                        os.system('mv ' +self.direc+'gpcal/'+'temp.log ' + self.logfile)
-                else:
-                    self.logger.info('uvfits file: {:s}, CLEAN mask: {:s}, save file: {:s}\n'.format(self.dataname+'pol.iter'+str(spoliter)+'.'+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', \
-                                     self.dataname+self.polcalsour[l]+'.IF*.q,u'))
-                    self.cleanqu(self.dataname+'pol.iter'+str(spoliter)+'.'+self.polcalsour[l]+'.dtcal.uvf', self.dataname+self.polcalsour[l]+'.win', self.dataname+self.polcalsour[l], difmaplogfile)
-                    if self.difmaplog:
-                        os.system('cat ' + self.logfile + ' ' + difmaplogfile + ' > ' + self.direc+'gpcal/'+'temp.log')
-                        os.system('mv ' +self.direc+'gpcal/'+'temp.log ' + self.logfile)
-            
-            # Extract visibility models using the CLEAN Stokes Q and U models.
-            self.get_pol_model()
             
             if(spoliter == 0):
                 self.logger.info('\n####################################################################')
                 self.logger.info('Instrumental polarization self-calibration mode...\n')
                 sourcename = ''
                 for i in range(len(self.polcalsour)):
                     sourcename = sourcename+('{:s}'.format(self.polcalsour[i]))+','
@@ -4133,30 +3528,108 @@
                     if(self.antmount[i] == 4): mount = 'Nasmyth-Right'
                     if(self.antmount[i] == 5): mount = 'Nasmyth-Left'
                     self.logger.info('{:s}: antenna mount = {:13s}, X = {:11.2f}m, Y = {:11.2f}m, Z = {:11.2f}m'.format(self.antname[i], mount, self.antx[i], self.anty[i], self.antz[i]))
                         
                 
                 self.logger.info(' ')
                 
-                self.logger.info('Observation date = {:s}'.format(str(self.year)+'-'+str(self.month)+'-'+str(self.day)))
+                self.logger.info('Observation date = {:s}'.format(str(np.min(self.year))+'-'+str(np.min(self.month))+'-'+str(np.min(self.day))))
             
             
-            # Obtain the best-fit D-terms using the model visibilities.
-            self.pol_gpcal(spoliter)
+            pol_IF, pol_ant, pol_DRArr, pol_DLArr = [], [], [], []
             
-            # Create D-term plots.
-            self.dplot(spoliter+1, self.outputname+'pol.iter{:02d}'.format(spoliter+1)+'.D_Terms', self.antname, self.pol_DRArr, self.pol_DLArr, self.polcalsour, lpcal=False)
+            for ifn in range(self.ifnum):
+                
+                ifdata = self.pol_data.loc[self.pol_data["IF"] == ifn+1]
+                
+                if(np.sum(self.pol_data["IF"] == ifn+1) == 0.):
+                    self.logger.info('Will skip this IF because there is no data.\n')
+                    continue
+                
+                self.logger.info('\n####################################################################')
+                self.logger.info('Processing IF {:d}'.format(ifn+1) + '...')
+                self.logger.info('####################################################################\n')
+                
+                self.logger.info('Instrumental polarization self-calibration mode...')
+                self.logger.info('Iteration: {:d}/{:d}\n'.format(spoliter+1, self.selfpoliter))
+                
+                
+                dumantname = np.copy(self.antname)
+                
+                if not self.fixdterm:
+                    self.fixdr = None
+                    self.fixdl = None
+
+                # If the zero-baseline D-term estimation was performed, then fix the D-terms of those stations for fitting for the rest of the array.
+                if self.zblcal:
+                    self.fixdterm = True
+                    if(self.fixdr == None):
+                        self.fixdr = {}
+                        self.fixdl = {}
+                    for i in range(len(self.zblant)):
+                        if(self.zblant[i][0] in self.fixdr):
+                            self.fixdr[self.zblant[i][0]] = self.zbl_DRArr.loc["IF"+str(ifn+1), self.zblant[i][0]]
+                            self.fixdl[self.zblant[i][0]] = self.zbl_DLArr.loc["IF"+str(ifn+1), self.zblant[i][0]]
+                        else:
+                            self.fixdr.update({self.zblant[i][0]: self.zbl_DRArr.loc["IF"+str(ifn+1), self.zblant[i][0]]})
+                            self.fixdl.update({self.zblant[i][0]: self.zbl_DLArr.loc["IF"+str(ifn+1), self.zblant[i][0]]})
+                        
+                        if(self.zblant[i][1] in self.fixdr):
+                            self.fixdr[self.zblant[i][1]] = self.zbl_DRArr.loc["IF"+str(ifn+1), self.zblant[i][1]]
+                            self.fixdl[self.zblant[i][1]] = self.zbl_DLArr.loc["IF"+str(ifn+1), self.zblant[i][1]]
+                        else:
+                            self.fixdr.update({self.zblant[i][1]: self.zbl_DRArr.loc["IF"+str(ifn+1), self.zblant[i][1]]})
+                            self.fixdl.update({self.zblant[i][1]: self.zbl_DLArr.loc["IF"+str(ifn+1), self.zblant[i][1]]})
+
+                
+                if (spoliter == self.selfpoliter - 1) & (self.vplot):
+                    dum_vplot = True
+                else:
+                    dum_vplot = False
+                
+                if (spoliter == self.selfpoliter - 1) & (self.vplot):
+                    dum_resplot = True
+                else:
+                    dum_resplot = False
+                    
+                    
+                fitresults, fitdterms, chisq = ps.pol_gpcal(self.direc, self.outputname, ifdata, self.polcalsour, self.antname, self.logger, Dbound = self.Dbound, Pbound = self.Pbound, \
+                                                     manualweight = self.manualweight, weightfactors = self.weightfactors, fixdterm = self.fixdterm, fixdr = self.fixdr, fixdl = self.fixdl, \
+                                                     multiproc = self.multiproc, nproc = self.nproc, colors = self.colors, vplot = dum_vplot, allplot = self.allplot, \
+                                                     vplot_title = self.vplot_title, vplot_scanavg = self.vplot_scanavg, vplot_avg_nat = self.vplot_avg_nat, tsep = self.tsep, \
+                                                     resplot = dum_resplot, markerarr = self.markerarr)
+                
+                    
+                dum_ant, dum_DRArr, dum_DLArr = fitdterms
+                dum_IF = np.repeat(ifn+1, len(dum_ant))
+                
+                pol_ant = pol_ant + dum_ant.tolist()
+                pol_DRArr = pol_DRArr + dum_DRArr.tolist()
+                pol_DLArr = pol_DLArr + dum_DLArr.tolist()
+                pol_IF = pol_IF + dum_IF.tolist()
+                
+                    
+            pol_IF, pol_ant, pol_DRArr, pol_DLArr = np.array(pol_IF), np.array(pol_ant), np.array(pol_DRArr), np.array(pol_DLArr)
+                
             
-            # Apply the best-fit D-terms and produce the D-term corrected UVFITS files.
-            self.pol_applydterm(self.source, self.pol_DRArr, self.pol_DLArr, self.direc+self.dataname+'pol.iter'+str(spoliter+1)+'.')
+            df = pd.DataFrame(pol_IF.transpose())
+            df['antennas'] = np.array(pol_ant)
+            df['IF'] = np.array(pol_IF)
+            df['DRArr'] = np.array(pol_DRArr)
+            df['DLArr'] = np.array(pol_DLArr)
+            del df[0]
             
-            # Save the fitting results into ASCII files.
-            self.pol_DRArr.to_csv(self.direc+'gpcal/'+self.outputname+'pol.iter'+str(spoliter+1)+'.DRArr.txt', sep = "\t")
-            self.pol_DLArr.to_csv(self.direc+'gpcal/'+self.outputname+'pol.iter'+str(spoliter+1)+'.DLArr.txt', sep = "\t")
+            df.to_csv(self.direc+'gpcal/'+self.outputname+'pol.iter'+str(spoliter+1)+'.dterm.csv', sep = "\t")
+    
+            # Create D-term plots.
+            self.dplot_new(spoliter+1, self.outputname+'pol.iter{:02d}'.format(spoliter+1)+'.D_Terms', pol_ant, pol_IF, pol_DRArr, pol_DLArr, self.polcalsour, lpcal=False)
             
+            # Apply the best-fit D-terms and produce the D-term corrected UVFITS files.
+            self.pol_applydterm(self.source, self.direc+'gpcal/'+self.outputname+'pol.iter'+str(spoliter+1)+'.dterm.csv', self.direc+self.outputname+'pol.iter'+str(spoliter+1)+'.')
+
         # Save the reduced chi-squares into ASCII files.
         self.chisq.to_csv(self.direc+'gpcal/'+self.outputname+'chisq.txt', sep = "\t")
         
         # Create a reduced chi-square plot.
         self.chisqplot(self.chisq)
         
-        
+
```

### Comparing `gpcal-0.9.4/setup.py` & `gpcal-0.9.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'gpcal',         # How you named your package folder (MyLib)
   packages = ['gpcal'],   # Chose the same as "name"
-  version = '0.9.4',      # Start with a small number and increase it with every change you make
+  version = '0.9.5',      # Start with a small number and increase it with every change you make
   license='gpl-2.0',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A generalized instrumental polarization calibration pipeline for VLBI data',   # Give a short description about your library
   author = 'Jongho Park',                   # Type in your name
   author_email = 'jpark@asiaa.sinica.edu.tw',      # Type in your E-Mail
   url = 'https://github.com/jhparkastro/gpcal',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/jhparkastro/gpcal/archive/v1.0.tar.gz',    # I explain this later on
   keywords = ['VLBI', 'polarimetry', 'astronomy', 'calibration'],   # Keywords that define your package best
```

