# Comparing `tmp/SplatStats-2.2.1.tar.gz` & `tmp/SplatStats-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplatStats-2.2.1.tar", last modified: Mon Jul 17 20:56:13 2023, max compression
+gzip compressed data, was "SplatStats-2.3.1.tar", last modified: Wed Jul 26 18:20:31 2023, max compression
```

## Comparing `SplatStats-2.2.1.tar` & `SplatStats-2.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-17 20:56:13.418653 SplatStats-2.2.1/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-2.2.1/LICENSE
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-07-17 20:56:13.418370 SplatStats-2.2.1/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6367 2023-05-29 20:06:53.000000 SplatStats-2.2.1/README.md
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-17 20:56:13.417290 SplatStats-2.2.1/SplatStats/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-2.2.1/SplatStats/Battle.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10398 2023-05-11 17:29:12.000000 SplatStats-2.2.1/SplatStats/Player.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-07-17 20:54:12.000000 SplatStats-2.2.1/SplatStats/StatInk.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-2.2.1/SplatStats/Team.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-2.2.1/SplatStats/__init__.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-07-17 20:56:13.000000 SplatStats-2.2.1/SplatStats/_version.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-2.2.1/SplatStats/auxiliary.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    14036 2023-07-17 16:23:54.000000 SplatStats-2.2.1/SplatStats/colors.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5905 2023-06-06 02:59:04.000000 SplatStats-2.2.1/SplatStats/constants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-2.2.1/SplatStats/files.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8663 2023-05-11 17:29:12.000000 SplatStats-2.2.1/SplatStats/parsers.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    56269 2023-05-11 17:29:12.000000 SplatStats-2.2.1/SplatStats/plots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-2.2.1/SplatStats/plotsAux.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1709 2023-05-11 17:29:12.000000 SplatStats-2.2.1/SplatStats/plotsTeam.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10747 2023-07-17 20:47:10.000000 SplatStats-2.2.1/SplatStats/statInkConstants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10625 2023-06-05 15:55:49.000000 SplatStats-2.2.1/SplatStats/statInkPlots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-2.2.1/SplatStats/statInkStats.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    14368 2023-05-29 19:37:30.000000 SplatStats-2.2.1/SplatStats/stats.py
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-17 20:56:13.418143 SplatStats-2.2.1/SplatStats.egg-info/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-07-17 20:56:13.000000 SplatStats-2.2.1/SplatStats.egg-info/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-07-17 20:56:13.000000 SplatStats-2.2.1/SplatStats.egg-info/SOURCES.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-07-17 20:56:13.000000 SplatStats-2.2.1/SplatStats.egg-info/dependency_links.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-07-17 20:56:13.000000 SplatStats-2.2.1/SplatStats.egg-info/requires.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-07-17 20:56:13.000000 SplatStats-2.2.1/SplatStats.egg-info/top_level.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-07-17 20:56:13.418699 SplatStats-2.2.1/setup.cfg
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-2.2.1/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-26 18:20:31.379848 SplatStats-2.3.1/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-2.3.1/LICENSE
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-07-26 18:20:31.379711 SplatStats-2.3.1/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6367 2023-05-29 20:06:53.000000 SplatStats-2.3.1/README.md
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-26 18:20:31.378609 SplatStats-2.3.1/SplatStats/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/Battle.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10734 2023-07-20 20:13:44.000000 SplatStats-2.3.1/SplatStats/Player.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-07-17 20:54:12.000000 SplatStats-2.3.1/SplatStats/StatInk.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/Team.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-07-26 18:20:31.000000 SplatStats-2.3.1/SplatStats/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    14036 2023-07-17 16:23:54.000000 SplatStats-2.3.1/SplatStats/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5905 2023-06-06 02:59:04.000000 SplatStats-2.3.1/SplatStats/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/files.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8968 2023-07-26 17:04:38.000000 SplatStats-2.3.1/SplatStats/parsers.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    59461 2023-07-26 18:06:33.000000 SplatStats-2.3.1/SplatStats/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/plotsAux.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1707 2023-07-26 17:48:54.000000 SplatStats-2.3.1/SplatStats/plotsTeam.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10747 2023-07-17 20:47:10.000000 SplatStats-2.3.1/SplatStats/statInkConstants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10625 2023-06-05 15:55:49.000000 SplatStats-2.3.1/SplatStats/statInkPlots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-2.3.1/SplatStats/statInkStats.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    15022 2023-07-26 17:22:01.000000 SplatStats-2.3.1/SplatStats/stats.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-26 18:20:31.379519 SplatStats-2.3.1/SplatStats.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-07-26 18:20:31.000000 SplatStats-2.3.1/SplatStats.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-07-26 18:20:31.000000 SplatStats-2.3.1/SplatStats.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-07-26 18:20:31.000000 SplatStats-2.3.1/SplatStats.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-07-26 18:20:31.000000 SplatStats-2.3.1/SplatStats.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-07-26 18:20:31.000000 SplatStats-2.3.1/SplatStats.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-07-26 18:20:31.379900 SplatStats-2.3.1/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-2.3.1/setup.py
```

### Comparing `SplatStats-2.2.1/LICENSE` & `SplatStats-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/PKG-INFO` & `SplatStats-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 2.2.1
+Version: 2.3.1
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-2.2.1/README.md` & `SplatStats-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/SplatStats/Battle.py` & `SplatStats-2.3.1/SplatStats/Battle.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/SplatStats/Player.py` & `SplatStats-2.3.1/SplatStats/Player.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
+import numpy as np
 import pandas as pd
 from tqdm import tqdm
 from termcolor import colored
 from collections import Counter
 import SplatStats.stats as stt
 import SplatStats.Battle as bat
 import SplatStats.parsers as par
@@ -86,14 +87,18 @@
         """        
         battlesHistory = par.parsePlayerHistoryFromBattles(
             self.battleRecords, self.name, 
             validOnly=validOnly, timezone=self.timezone
         )
         battlesHistory['winBool'] = [1 if i=='W' else 0 for i in battlesHistory['win']]
         battlesHistory['loseBool'] = [1 if i=='L' else 0 for i in battlesHistory['win']]
+        battlesHistory['participation'] = [1]*battlesHistory.shape[0]
+        battlesHistory['kassist'] = (battlesHistory['kill']+0.5*battlesHistory['assist'])
+        battlesHistory['kad'] = battlesHistory['kassist']/battlesHistory['death']
+        battlesHistory.replace([np.inf, np.nan, -np.inf], 0, inplace=True)
         if ammendWeapons:
             self.battlesHistory = battlesHistory.replace('Hero Shot Replica', 'Splattershot')
         else:
             self.battlesHistory = battlesHistory
         return self.battlesHistory
     
     def getPlayerHistoryByTypes(self):
```

### Comparing `SplatStats-2.2.1/SplatStats/StatInk.py` & `SplatStats-2.3.1/SplatStats/StatInk.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/SplatStats/Team.py` & `SplatStats-2.3.1/SplatStats/Team.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/SplatStats/__init__.py` & `SplatStats-2.3.1/SplatStats/__init__.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/SplatStats/auxiliary.py` & `SplatStats-2.3.1/SplatStats/auxiliary.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/SplatStats/colors.py` & `SplatStats-2.3.1/SplatStats/colors.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/SplatStats/constants.py` & `SplatStats-2.3.1/SplatStats/constants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/SplatStats/files.py` & `SplatStats-2.3.1/SplatStats/files.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/SplatStats/parsers.py` & `SplatStats-2.3.1/SplatStats/parsers.py`

 * *Files 3% similar despite different names*

```diff
@@ -240,8 +240,19 @@
         naValue (int): value to return if the entry is not bool 
     Returns:
         int: Converted value.
     """    
     if type(entry) is not bool:
         return naValue
     else:
-        return int(entry)
+        return int(entry)
+    
+
+def addDateGroup(
+        playerHistory, 
+        slicer=(lambda x: "{}/{:02d}".format(
+            x.isocalendar().year, x.isocalendar().week
+        ))
+    ):
+    dteSlice = playerHistory['datetime'].apply(slicer).copy()
+    playerHistory.insert(3, 'DateGroup', dteSlice)
+    return playerHistory
```

### Comparing `SplatStats-2.2.1/SplatStats/plots.py` & `SplatStats-2.3.1/SplatStats/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import math
 import squarify
 import pandas as pd
 import numpy as np
 import seaborn as sns
 from pywaffle import Waffle
+from matplotlib.colors import LogNorm
 import matplotlib.pyplot as plt
 from math import radians, log10
 import matplotlib.colors as mcolors
 from matplotlib.patches import Rectangle
 import SplatStats.constants as cst
 import SplatStats.stats as stats
 import SplatStats.auxiliary as aux
@@ -1313,8 +1314,82 @@
             kassist=kassist, paint=paint, 
             clockwise=clockwise, innerOffset=innerOffset,
             colorsKD=colorsKD, colorP=colorP,
             rangeKD=rangeKD, rangeP=rangeP,
             lw=0.25
         )
     # Return figAx ------------------------------------------------------------
+    return (fig, ax)
+
+
+def plotTimecard(
+        timecard, wpnSorting,
+        figAx=None, yearRange=None, weekRange=None,
+        origin='N', direction=1, rRange=(0, 90), 
+        offset=0, height=1, edgeWidth=1, fontSize=12,
+        highColors=['#DE0B64AA', '#311AA8AA', '#6BFF00AA', '#9030FF55', '#B62EA7AA'],
+        baseColor='#ffffff55', maxValue=None,
+        fmtStr='  {} ({:.2f})', statScaler=1 
+    ):
+    # Get auxiliary variables -------------------------------------------------
+    wpnsNumber = len(wpnSorting)
+    cmaps = [clr.colorPaletteFromHexList([baseColor, c]) for c in highColors]
+    if not maxValue:
+        maxMag = max(timecard.max())
+        norm = LogNorm(vmin=1, vmax=maxMag)
+    else:
+        norm = LogNorm(vmin=1, vmax=maxValue)
+    if (yearRange is None) or (weekRange is None):
+        (minDate, maxDate) = (
+            sorted(timecard.columns)[0], sorted(timecard.columns)[-1]
+        )
+        (minYear, minWeek) = (int(minDate[:4]), int(minDate[5:]))
+        (maxYear, maxWeek) = (int(maxDate[:4]), int(maxDate[5:]))
+    else:
+        (minYear, maxYear) = yearRange
+        (minWeek, maxWeek) = weekRange
+    # Plot --------------------------------------------------------------------
+    if not figAx:
+        (fig, ax) = plt.subplots(
+            figsize=(10, 10), subplot_kw={"projection": "polar"}
+        )
+    for wpix in range(wpnsNumber):
+        (wpnCurrent, wpnTotal) = (
+            wpnSorting.index[::-1][wpix], wpnSorting.values[::-1][wpix]
+        )
+        wpnLabel = fmtStr.format(wpnCurrent, wpnTotal/statScaler)
+        cmapCurrent = cmaps[wpix%len(cmaps)]
+        # Get weapon values and dates -----------------------------------------
+        rowValues = timecard.loc[wpnCurrent]
+        (rowDates, rowMagnitudes) = (
+            list(rowValues.index), list(rowValues.values)
+        )
+        # Convert dates to x coordinates --------------------------------------
+        dateTuples = [[int(x) for x in d.split('/')] for d in rowDates]
+        weekNumber = [(y%minYear)*52+w-minWeek+1 for (y, w) in dateTuples]
+        # Convert values to colors --------------------------------------------
+        rDelta = radians(rRange[1])/weekNumber[-1]
+        deltas = np.arange(0, radians(rRange[1])+rDelta, rDelta)
+        weekBars = [(i*rDelta, rDelta) for i in range(len(deltas)-1)]
+        clrsBlocks = [cmapCurrent(norm(value)) for value in rowMagnitudes]
+        ax.broken_barh(
+            weekBars, (offset+wpix*height, height), lw=edgeWidth,
+            facecolors=clrsBlocks, edgecolors=baseColor
+        )
+        ax.text(
+            0, offset+wpix*height+height/2, wpnLabel,
+            va='center', ha='left', fontsize=fontSize
+        )
+    # Axis tweaks -------------------------------------------------------------
+    ax.set_xticklabels([])
+    ax.set_yticklabels([])
+    ax.set_thetamin(0)
+    ax.set_thetamax(rRange[1])
+    ax.set_ylim(0, offset+wpnsNumber*height)
+    ax.set_theta_zero_location(origin)
+    ax.set_theta_direction(direction)
+    ax.spines['polar'].set_visible(False)
+    ax.axis("off")
+    ax.set_rlabel_position(0)
+    ax.xaxis.grid(False)
+    ax.yaxis.grid(False)
     return (fig, ax)
```

### Comparing `SplatStats-2.2.1/SplatStats/plotsAux.py` & `SplatStats-2.3.1/SplatStats/plotsAux.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/SplatStats/plotsTeam.py` & `SplatStats-2.3.1/SplatStats/plotsTeam.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 import numpy as np
 import SplatStats.stats as stats
-import SplatStats.colors as clrs
+import SplatStats.colors as clr
 
 
 def plotStreamTeam(
         figAx, team, teamHistBT,
-        colors=clrs.ALL_COLORS,
+        colors=clr.ALL_COLORS,
         metric='kill', normalized=False, smooth=True, 
         smoothness=0.75, gridSize=500, baseline='sym'
     ):
     (fig, ax) = figAx
     # Reshape dataframe and get vars ------------------------------------------
     dfByPlayer = teamHistBT.reorder_levels(["player", "datetime"])
     names = team.names
```

### Comparing `SplatStats-2.2.1/SplatStats/statInkConstants.py` & `SplatStats-2.3.1/SplatStats/statInkConstants.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/SplatStats/statInkPlots.py` & `SplatStats-2.3.1/SplatStats/statInkPlots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/SplatStats/statInkStats.py` & `SplatStats-2.3.1/SplatStats/statInkStats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/SplatStats/stats.py` & `SplatStats-2.3.1/SplatStats/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pandas as pd
 import scipy.stats as sts
+import SplatStats.parsers as par
 
 
 def calcBattleHistoryStats(bHist, kassistWeight=0.5):
     """Calculates the basic player stats for a battle history dataframe.
 
     Args:
         bHist (dataframe): Battle history dataframe for a player.
@@ -364,8 +365,24 @@
 def statSummaries(playerHistory, stat, summaryFuns=(np.sum, np.mean)):
     return [fun(playerHistory[stat]) for fun in summaryFuns]
 
 
 def statPerMinute(playerHistory, stat, summaryFun=None):
     statPM = (playerHistory[stat]/(playerHistory['duration']/60))
     stpm = summaryFun(statPM) if summaryFun else statPM
-    return stpm
+    return stpm
+
+
+def getTimecard(
+        playerHistory, 
+        slicer=(lambda x: "{}/{:02d}".format(
+            x.isocalendar().year, x.isocalendar().week
+        ))
+    ):
+    par.addDateGroup(playerHistory, slicer=slicer)
+    grpd = playerHistory.groupby(['main weapon', 'DateGroup']).sum('kill')
+    grpd['kad'] = grpd['kassist']/grpd['death']
+    grpd.replace([np.inf, np.nan, -np.inf], 0, inplace=True)
+    dfGroups = grpd.unstack().reset_index().set_index("main weapon")
+    statsCats = sorted(list(set([i[0] for i in list(dfGroups.columns)])))
+    tCardsDict = {cat: dfGroups[cat] for cat in statsCats}
+    return tCardsDict
```

### Comparing `SplatStats-2.2.1/SplatStats.egg-info/PKG-INFO` & `SplatStats-2.3.1/SplatStats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 2.2.1
+Version: 2.3.1
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-2.2.1/SplatStats.egg-info/SOURCES.txt` & `SplatStats-2.3.1/SplatStats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SplatStats-2.2.1/setup.py` & `SplatStats-2.3.1/setup.py`

 * *Files identical despite different names*

