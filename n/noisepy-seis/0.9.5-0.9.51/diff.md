# Comparing `tmp/noisepy_seis-0.9.5.tar.gz` & `tmp/noisepy_seis-0.9.51.tar.gz`

## Comparing `noisepy_seis-0.9.5.tar` & `noisepy_seis-0.9.51.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    12878 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/_version.py
--rw-r--r--   0        0        0    10254 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/asdfstore.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/channelcatalog.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/constants.py
--rw-r--r--   0        0        0     9190 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/datatypes.py
--rw-r--r--   0        0        0     8461 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   113005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    34841 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/pnwstore.py
--rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/scedc_s3store.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/scheduler.py
--rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/stores.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/utils.py
--rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/zarrstore.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/LICENSE
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/README.md
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/pyproject.toml
--rw-r--r--   0        0        0    10729 2020-02-02 00:00:00.000000 noisepy_seis-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0    11683 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    12766 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/_version.py
+-rw-r--r--   0        0        0    10254 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/asdfstore.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/channelcatalog.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/constants.py
+-rw-r--r--   0        0        0     9190 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/datatypes.py
+-rw-r--r--   0        0        0     8461 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   113005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    34841 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/pnwstore.py
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/scedc_s3store.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/scheduler.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/stores.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/utils.py
+-rw-r--r--   0        0        0     7463 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/zarrstore.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4721 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/LICENSE
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/README.md
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/pyproject.toml
+-rw-r--r--   0        0        0    10730 2020-02-02 00:00:00.000000 noisepy_seis-0.9.51/PKG-INFO
```

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.9.51/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.9.51/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.9.51/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import gc
 import logging
 import sys
 import time
 from collections import OrderedDict
-from concurrent.futures import Executor, Future, ThreadPoolExecutor, as_completed
-from typing import Dict, Iterable, List, Tuple
+from concurrent.futures import Executor, ThreadPoolExecutor, as_completed
+from typing import Dict, List, Tuple
 
 import numpy as np
 import obspy
 from datetimerange import DateTimeRange
 from scipy.fftpack.helper import next_fast_len
 
 from . import noise_module
 from .datatypes import Channel, ChannelData, ConfigParameters, NoiseFFT
 from .scheduler import Scheduler, SingleNodeScheduler
 from .stores import CrossCorrelationDataStore, RawDataStore
-from .utils import TimeLogger, error_if
+from .utils import TimeLogger, _get_results, error_if
 
 logger = logging.getLogger(__name__)
 # ignore warnings
 if not sys.warnoptions:
     import warnings
 
     warnings.simplefilter("ignore")
@@ -338,11 +338,7 @@
     memory_size = nsta * npts_chunk * 4 / 1024**3
     if memory_size > MAX_MEM:
         raise ValueError(
             "Require %5.3fG memory but only %5.3fG provided)! Reduce inc_hours to avoid this issue!"
             % (memory_size, MAX_MEM)
         )
     return nseg_chunk
-
-
-def _get_results(futures: Iterable[Future]) -> Iterable[Future]:
-    return [f.result() for f in futures]
```

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.9.51/src/noisepy/seis/S2_stacking.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import logging
 import sys
 import time
+from concurrent.futures import ProcessPoolExecutor
 from typing import Any, Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
 from datetimerange import DateTimeRange
 
-from noisepy.seis.datatypes import ConfigParameters, StackMethod
+from noisepy.seis.datatypes import ConfigParameters, StackMethod, Station
 from noisepy.seis.scheduler import Scheduler, SingleNodeScheduler
 from noisepy.seis.stores import CrossCorrelationDataStore, StackStore
-from noisepy.seis.utils import TimeLogger
+from noisepy.seis.utils import TimeLogger, _get_results
 
 from . import noise_module
 
 logger = logging.getLogger(__name__)
 if not sys.warnoptions:
     import warnings
 
@@ -45,16 +46,57 @@
 
 def stack(
     cc_store: CrossCorrelationDataStore,
     stack_store: StackStore,
     fft_params: ConfigParameters,
     scheduler: Scheduler = SingleNodeScheduler(),
 ):
+    executor = ProcessPoolExecutor()
     tlog = TimeLogger(logger=logger, level=logging.INFO)
     t_tot = tlog.reset()
+
+    def initializer():
+        timespans = cc_store.get_timespans()
+        pairs_all = cc_store.get_station_pairs()
+        logger.info(f"Station pairs: {pairs_all}")
+
+        if len(timespans) == 0 or len(pairs_all) == 0:
+            raise IOError("Abort! no available CCF data for stacking")
+        return timespans, pairs_all
+
+    timespans, pairs_all = scheduler.initialize(initializer, 2)
+
+    # Get the pairs that need to be processed by this node
+    pairs_node = [pairs_all[i] for i in scheduler.get_indices(pairs_all)]
+
+    tasks = [executor.submit(stack_pair, p[0], p[1], timespans, cc_store, stack_store, fft_params) for p in pairs_node]
+    _ = _get_results(tasks)
+    scheduler.synchronize()
+    tlog.log("step 2 in total", t_tot)
+
+
+def stack_pair(
+    src_sta: Station,
+    rec_sta: Station,
+    timespans: List[DateTimeRange],
+    cc_store: CrossCorrelationDataStore,
+    stack_store: StackStore,
+    fft_params: ConfigParameters,
+):
+    if stack_store.is_done(src_sta, rec_sta):
+        return
+
+    tlog = TimeLogger(logger=logger, level=logging.INFO)
+    t_append = 0.0
+    # check if it is auto-correlation
+    if src_sta == rec_sta:
+        fauto = 1
+    else:
+        fauto = 0
+    nccomp = fft_params.ncomp * fft_params.ncomp
     if fft_params.rotation and fft_params.correction:
         if not fft_params.correction_csv:
             logger.warning("Missing correction_csv parameter but rotation=True and correction=True")
         else:
             locs = pd.read_csv(fft_params.correction_csv)
     else:
         locs = []
@@ -63,207 +105,168 @@
     if fft_params.ncomp == 1:
         enz_system = ["ZZ"]
     else:
         enz_system = ["EE", "EN", "EZ", "NE", "NN", "NZ", "ZE", "ZN", "ZZ"]
 
     # ZZ_R component used to avoid a collision with ZZ component above
     rtz_components = ["ZR", "ZT", "ZZ_R", "RR", "RT", "RZ", "TR", "TT", "TZ"]
-
-    #######################################
-    # #########PROCESSING SECTION##########
-    #######################################
-    def initializer():
-        timespans = cc_store.get_timespans()
-        pairs_all = cc_store.get_station_pairs()
-        logger.info(f"Station pairs: {pairs_all}")
-
-        if len(timespans) == 0 or len(pairs_all) == 0:
-            raise IOError("Abort! no available CCF data for stacking")
-        return timespans, pairs_all
-
-    timespans, pairs_all = scheduler.initialize(initializer, 2)
-
-    nccomp = fft_params.ncomp * fft_params.ncomp
     num_chunk = len(timespans) * nccomp
     num_segmts = 1
-
-    # loop through each pair assigned to this process by the scheduler
-    for ipair in scheduler.get_indices(pairs_all):
-        tlog.reset()
-        t_append = 0.0
-
-        logger.debug("%dth path for station-pair %s" % (ipair, pairs_all[ipair]))
-        sta_pair = pairs_all[ipair]
-        src_sta = sta_pair[0]
-        rec_sta = sta_pair[1]
-
-        # check if it is auto-correlation
-        if src_sta == rec_sta:
-            fauto = 1
-        else:
-            fauto = 0
-
-        if stack_store.is_done(src_sta, rec_sta):
+    # crude estimation on memory needs (assume float32)
+    num_segmts, npts_segmt = calc_segments(fft_params, num_chunk)
+    # allocate array to store fft data/info
+    cc_array = np.zeros((num_chunk * num_segmts, npts_segmt), dtype=np.float32)
+    cc_time = np.zeros(num_chunk * num_segmts, dtype=np.float32)
+    cc_ngood = np.zeros(num_chunk * num_segmts, dtype=np.int16)
+    cc_comp = np.chararray(num_chunk * num_segmts, itemsize=2, unicode=True)
+
+    # loop through all time-chuncks
+    iseg = 0
+    for ts in timespans:
+        # load the data from daily compilation
+        ch_pairs = cc_store.get_channeltype_pairs(ts, src_sta, rec_sta)
+
+        logger.debug(f"path_list for {src_sta}-{rec_sta}: {ch_pairs}")
+        # seperate auto and cross-correlation
+        if not validate_pairs(fft_params.ncomp, str((src_sta, rec_sta)), fauto, ts, len(ch_pairs)):
             continue
 
-        # crude estimation on memory needs (assume float32)
-        num_segmts, npts_segmt = calc_segments(fft_params, num_chunk)
-        # allocate array to store fft data/info
-        cc_array = np.zeros((num_chunk * num_segmts, npts_segmt), dtype=np.float32)
-        cc_time = np.zeros(num_chunk * num_segmts, dtype=np.float32)
-        cc_ngood = np.zeros(num_chunk * num_segmts, dtype=np.int16)
-        cc_comp = np.chararray(num_chunk * num_segmts, itemsize=2, unicode=True)
-
-        # loop through all time-chuncks
-        iseg = 0
-        for ts in timespans:
-            # load the data from daily compilation
-            ch_pairs = cc_store.get_channeltype_pairs(ts, src_sta, rec_sta)
-
-            logger.debug(f"path_list for {src_sta}-{rec_sta}: {ch_pairs}")
-            # seperate auto and cross-correlation
-            if not validate_pairs(fft_params.ncomp, str(sta_pair), fauto, ts, len(ch_pairs)):
-                continue
-
-            # load the 9-component data, which is in order in the ASDF
-            for ch_pair in ch_pairs:
-                src_chan, rec_chan = ch_pair
-                tcmp1 = src_chan.get_orientation()
-                tcmp2 = rec_chan.get_orientation()
-
-                # read data and parameter matrix
-                tparameters, tdata = cc_store.read(ts, src_sta, rec_sta, src_chan, rec_chan)
-                ttime = tparameters["time"]
-                tgood = tparameters["ngood"]
-                if fft_params.substack:
-                    for ii in range(tdata.shape[0]):
-                        cc_array[iseg] = tdata[ii]
-                        cc_time[iseg] = ttime[ii]
-                        cc_ngood[iseg] = tgood[ii]
-                        cc_comp[iseg] = tcmp1 + tcmp2
-                        iseg += 1
-                else:
-                    cc_array[iseg] = tdata
-                    cc_time[iseg] = ttime
-                    cc_ngood[iseg] = tgood
+        # load the 9-component data, which is in order in the ASDF
+        for ch_pair in ch_pairs:
+            src_chan, rec_chan = ch_pair
+            tcmp1 = src_chan.get_orientation()
+            tcmp2 = rec_chan.get_orientation()
+
+            # read data and parameter matrix
+            tparameters, tdata = cc_store.read(ts, src_sta, rec_sta, src_chan, rec_chan)
+            ttime = tparameters["time"]
+            tgood = tparameters["ngood"]
+            if fft_params.substack:
+                for ii in range(tdata.shape[0]):
+                    cc_array[iseg] = tdata[ii]
+                    cc_time[iseg] = ttime[ii]
+                    cc_ngood[iseg] = tgood[ii]
                     cc_comp[iseg] = tcmp1 + tcmp2
                     iseg += 1
-
-        t_load = tlog.log("loading CCF data")
-
-        # continue when there is no data or for auto-correlation
-        if iseg <= 1 and fauto == 1:
+            else:
+                cc_array[iseg] = tdata
+                cc_time[iseg] = ttime
+                cc_ngood[iseg] = tgood
+                cc_comp[iseg] = tcmp1 + tcmp2
+                iseg += 1
+
+    t_load = tlog.log("loading CCF data")
+
+    # continue when there is no data or for auto-correlation
+    if iseg <= 1 and fauto == 1:
+        return
+    outfn = f"{src_sta}_{rec_sta}.h5"
+    logger.debug("ready to output to %s" % (outfn))
+
+    # matrix used for rotation
+    if fft_params.rotation:
+        bigstack = np.zeros(shape=(9, npts_segmt), dtype=np.float32)
+    if fft_params.stack_method == "all":
+        bigstack1 = np.zeros(shape=(9, npts_segmt), dtype=np.float32)
+        bigstack2 = np.zeros(shape=(9, npts_segmt), dtype=np.float32)
+
+    def write_stacks(comp: str, tparameters: Dict[str, Any], stacks: List[Tuple[StackMethod, np.ndarray]]):
+        nonlocal t_append
+        t_start = time.time()
+        for method, data in stacks:
+            stack_store.append(src_sta, rec_sta, comp, f"Allstack_{method.value}", tparameters, data)
+        t_append += time.time() - t_start
+
+    # loop through cross-component for stacking
+    iflag = 1
+    for icomp in range(nccomp):
+        tlog.reset()
+        comp = enz_system[icomp]
+        indx = np.where(cc_comp.lower() == comp.lower())[0]
+        logger.debug(f"index to find the comp: {indx}")
+
+        # jump if there are not enough data
+        if len(indx) < 2:
+            iflag = 0
             continue
-        outfn = f"{src_sta}_{rec_sta}.h5"
-        logger.debug("ready to output to %s" % (outfn))
 
-        # matrix used for rotation
+        # output stacked data
+        (
+            cc_final,
+            ngood_final,
+            stamps_final,
+            allstacks1,
+            allstacks2,
+            allstacks3,
+            nstacks,
+        ) = noise_module.stacking(cc_array[indx], cc_time[indx], cc_ngood[indx], fft_params)
+        logger.debug(f"after stacking nstacks: {nstacks}")
+        if not len(allstacks1):
+            continue
         if fft_params.rotation:
-            bigstack = np.zeros(shape=(9, npts_segmt), dtype=np.float32)
-        if fft_params.stack_method == "all":
-            bigstack1 = np.zeros(shape=(9, npts_segmt), dtype=np.float32)
-            bigstack2 = np.zeros(shape=(9, npts_segmt), dtype=np.float32)
-
-        def write_stacks(comp: str, tparameters: Dict[str, Any], stacks: List[Tuple[StackMethod, np.ndarray]]):
-            nonlocal t_append
-            t_start = time.time()
-            for method, data in stacks:
-                stack_store.append(src_sta, rec_sta, comp, f"Allstack_{method.value}", tparameters, data)
-            t_append += time.time() - t_start
-
-        # loop through cross-component for stacking
-        iflag = 1
-        for icomp in range(nccomp):
-            tlog.reset()
-            comp = enz_system[icomp]
-            indx = np.where(cc_comp.lower() == comp.lower())[0]
-            logger.debug(f"index to find the comp: {indx}")
-
-            # jump if there are not enough data
-            if len(indx) < 2:
-                iflag = 0
-                continue
-
-            # output stacked data
-            (
-                cc_final,
-                ngood_final,
-                stamps_final,
-                allstacks1,
-                allstacks2,
-                allstacks3,
-                nstacks,
-            ) = noise_module.stacking(cc_array[indx], cc_time[indx], cc_ngood[indx], fft_params)
-            logger.debug(f"after stacking nstacks: {nstacks}")
-            if not len(allstacks1):
-                continue
-            if fft_params.rotation:
-                bigstack[icomp] = allstacks1
-                if fft_params.stack_method == "all":
-                    bigstack1[icomp] = allstacks2
-                    bigstack2[icomp] = allstacks3
+            bigstack[icomp] = allstacks1
+            if fft_params.stack_method == "all":
+                bigstack1[icomp] = allstacks2
+                bigstack2[icomp] = allstacks3
 
-                tparameters["time"] = stamps_final[0]
-                tparameters["ngood"] = nstacks
-                if fft_params.stack_method != "all":
-                    to_write = [(fft_params.stack_method, allstacks1)]
-                else:
-                    to_write = [
-                        (StackMethod.LINEAR, allstacks1),
-                        (StackMethod.PWS, allstacks2),
-                        (StackMethod.ROBUST, allstacks3),
-                    ]
-                write_stacks(comp, tparameters, to_write)
-
-            # keep a track of all sub-stacked data from S1
-            if fft_params.keep_substack:
-                for ii in range(cc_final.shape[0]):
-                    tparameters["time"] = stamps_final[ii]
-                    tparameters["ngood"] = ngood_final[ii]
-                    stack_name = "T" + str(int(stamps_final[ii]))
-                    write_stacks(comp, tparameters, [(stack_name, cc_final[ii])])
-
-        # do rotation if needed
-        if fft_params.rotation and iflag:
-            if np.all(bigstack == 0):
-                continue
-            tparameters["station_source"] = src_sta.name
-            tparameters["station_receiver"] = rec_sta.name
+            tparameters["time"] = stamps_final[0]
+            tparameters["ngood"] = nstacks
             if fft_params.stack_method != "all":
-                bigstack_rotated = noise_module.rotation(bigstack, tparameters, locs)
-
-                # write to file
-                for icomp in range(nccomp):
-                    comp = rtz_components[icomp]
-                    tparameters["time"] = stamps_final[0]
-                    tparameters["ngood"] = nstacks
-                    write_stacks(comp, tparameters, [(fft_params.stack_method, bigstack_rotated[icomp])])
+                to_write = [(fft_params.stack_method, allstacks1)]
             else:
-                bigstack_rotated = noise_module.rotation(bigstack, tparameters, locs)
-                bigstack_rotated1 = noise_module.rotation(bigstack1, tparameters, locs)
-                bigstack_rotated2 = noise_module.rotation(bigstack2, tparameters, locs)
-
-                # write to file
-                for icomp in range(nccomp):
-                    comp = rtz_components[icomp]
-                    tparameters["time"] = stamps_final[0]
-                    tparameters["ngood"] = nstacks
-                    stacks = [
-                        (StackMethod.LINEAR, bigstack_rotated[icomp]),
-                        (StackMethod.PWS, bigstack_rotated1[icomp]),
-                        (StackMethod.ROBUST, bigstack_rotated2[icomp]),
-                    ]
-                    write_stacks(comp, tparameters, stacks)
-        tlog.log(f"stack/rotate all station pairs {pairs_all[ipair]}", t_load)
-        tlog.log_raw("store.append", t_append)
-
-        stack_store.mark_done(src_sta, rec_sta)
+                to_write = [
+                    (StackMethod.LINEAR, allstacks1),
+                    (StackMethod.PWS, allstacks2),
+                    (StackMethod.ROBUST, allstacks3),
+                ]
+            write_stacks(comp, tparameters, to_write)
+
+        # keep a track of all sub-stacked data from S1
+        if fft_params.keep_substack:
+            for ii in range(cc_final.shape[0]):
+                tparameters["time"] = stamps_final[ii]
+                tparameters["ngood"] = ngood_final[ii]
+                stack_name = "T" + str(int(stamps_final[ii]))
+                write_stacks(comp, tparameters, [(stack_name, cc_final[ii])])
+
+    # do rotation if needed
+    if fft_params.rotation and iflag:
+        if np.all(bigstack == 0):
+            return
+        tparameters["station_source"] = src_sta.name
+        tparameters["station_receiver"] = rec_sta.name
+        if fft_params.stack_method != "all":
+            bigstack_rotated = noise_module.rotation(bigstack, tparameters, locs)
+
+            # write to file
+            for icomp in range(nccomp):
+                comp = rtz_components[icomp]
+                tparameters["time"] = stamps_final[0]
+                tparameters["ngood"] = nstacks
+                write_stacks(comp, tparameters, [(fft_params.stack_method, bigstack_rotated[icomp])])
+        else:
+            bigstack_rotated = noise_module.rotation(bigstack, tparameters, locs)
+            bigstack_rotated1 = noise_module.rotation(bigstack1, tparameters, locs)
+            bigstack_rotated2 = noise_module.rotation(bigstack2, tparameters, locs)
+
+            # write to file
+            for icomp in range(nccomp):
+                comp = rtz_components[icomp]
+                tparameters["time"] = stamps_final[0]
+                tparameters["ngood"] = nstacks
+                stacks = [
+                    (StackMethod.LINEAR, bigstack_rotated[icomp]),
+                    (StackMethod.PWS, bigstack_rotated1[icomp]),
+                    (StackMethod.ROBUST, bigstack_rotated2[icomp]),
+                ]
+                write_stacks(comp, tparameters, stacks)
+    tlog.log(f"stack/rotate all station pairs {(src_sta,rec_sta)}", t_load)
+    # tlog.log_raw("store.append", t_append)
 
-    tlog.log("step 2 in total", t_tot)
-    scheduler.synchronize()
+    stack_store.mark_done(src_sta, rec_sta)
 
 
 def validate_pairs(ncomp: int, sta_pair: str, fauto: int, ts: DateTimeRange, n_pairs: int) -> bool:
     if fauto == 1:
         if ncomp == 3 and n_pairs < 6:
             logger.warning("continue! not enough cross components for auto-correlation %s in %s" % (sta_pair, ts))
             return False
```

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/__init__.py` & `noisepy_seis-0.9.51/src/noisepy/seis/__init__.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/asdfstore.py` & `noisepy_seis-0.9.51/src/noisepy/seis/asdfstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/channelcatalog.py` & `noisepy_seis-0.9.51/src/noisepy/seis/channelcatalog.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/datatypes.py` & `noisepy_seis-0.9.51/src/noisepy/seis/datatypes.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/main.py` & `noisepy_seis-0.9.51/src/noisepy/seis/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             else ASDFCCStore(args.ccf_path, mode=mode)
         )
 
     def get_stack_store(args):
         return (
             ZarrStackStore(args.stack_path, mode="a")
             if args.format == DataFormat.ZARR.value
-            else ASDFStackStore(args.stack_path, "w")
+            else ASDFStackStore(args.stack_path, "a")
         )
 
     def run_cross_correlation():
         ccf_dir = args.ccf_path
         cc_store = get_cc_store(args)
         params = initialize_params(args, args.raw_data_path)
         raw_store = create_raw_store(args, params)
```

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.9.51/src/noisepy/seis/noise_module.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.9.51/src/noisepy/seis/plotting_modules.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/pnwstore.py` & `noisepy_seis-0.9.51/src/noisepy/seis/pnwstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/scedc_s3store.py` & `noisepy_seis-0.9.51/src/noisepy/seis/scedc_s3store.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/scheduler.py` & `noisepy_seis-0.9.51/src/noisepy/seis/scheduler.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/stores.py` & `noisepy_seis-0.9.51/src/noisepy/seis/stores.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/utils.py` & `noisepy_seis-0.9.51/src/noisepy/seis/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 import os
 import posixpath
 import time
+from concurrent.futures import Future
+from typing import Iterable
 from urllib.parse import urlparse
 
 import fsspec
 
 S3_SCHEME = "s3"
 ANON_ARG = "anon"
 utils_logger = logging.getLogger(__name__)
@@ -86,7 +88,11 @@
     Args:
         condition (bool): Condition to evaluate
         msg (str): Error message
         error_type (type): Type of error to raise, e.g. ValueError
     """
     if condition:
         raise error_type(msg)
+
+
+def _get_results(futures: Iterable[Future]) -> Iterable[Future]:
+    return [f.result() for f in futures]
```

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/zarrstore.py` & `noisepy_seis-0.9.51/src/noisepy/seis/zarrstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.9.51/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.9.51/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.9.51/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.9.51/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/.gitignore` & `noisepy_seis-0.9.51/.gitignore`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/LICENSE` & `noisepy_seis-0.9.51/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/README.md` & `noisepy_seis-0.9.51/README.md`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/pyproject.toml` & `noisepy_seis-0.9.51/pyproject.toml`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.9.5/PKG-INFO` & `noisepy_seis-0.9.51/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.9.5
+Version: 0.9.51
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@uw.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
```

