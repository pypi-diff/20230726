# Comparing `tmp/pympc-1.0.0.tar.gz` & `tmp/pympc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pympc-1.0.0.tar", last modified: Fri Mar  4 18:17:04 2022, max compression
+gzip compressed data, was "dist/pympc-1.1.0.tar", last modified: Wed Jul 26 12:09:34 2023, max compression
```

## Comparing `pympc-1.0.0.tar` & `pympc-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 jdl       (1000) jdl       (1000)        0 2022-03-04 18:17:04.000000 pympc-1.0.0/
--rw-rw-r--   0 jdl       (1000) jdl       (1000)    32422 2019-09-12 12:07:32.000000 pympc-1.0.0/LICENSE.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)     6581 2022-03-04 18:17:04.000000 pympc-1.0.0/PKG-INFO
--rw-r--r--   0 jdl       (1000) jdl       (1000)     6234 2022-03-04 18:06:24.000000 pympc-1.0.0/README.md
-drwxrwxr-x   0 jdl       (1000) jdl       (1000)        0 2022-03-04 18:17:04.000000 pympc-1.0.0/pympc/
--rw-rw-r--   0 jdl       (1000) jdl       (1000)      150 2022-03-04 18:11:49.000000 pympc-1.0.0/pympc/__init__.py
-drwxrwxr-x   0 jdl       (1000) jdl       (1000)        0 2022-03-04 18:17:04.000000 pympc-1.0.0/pympc/data/
--rw-r--r--   0 jdl       (1000) jdl       (1000)    84540 2022-03-04 16:22:51.000000 pympc-1.0.0/pympc/data/obs_codes.npy
--rw-r--r--   0 jdl       (1000) jdl       (1000)    25202 2022-03-04 18:07:58.000000 pympc-1.0.0/pympc/pympc.py
-drwxrwxr-x   0 jdl       (1000) jdl       (1000)        0 2022-03-04 18:17:04.000000 pympc-1.0.0/pympc.egg-info/
--rw-rw-r--   0 jdl       (1000) jdl       (1000)     6581 2022-03-04 18:17:04.000000 pympc-1.0.0/pympc.egg-info/PKG-INFO
--rw-rw-r--   0 jdl       (1000) jdl       (1000)      310 2022-03-04 18:17:04.000000 pympc-1.0.0/pympc.egg-info/SOURCES.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)        1 2022-03-04 18:17:04.000000 pympc-1.0.0/pympc.egg-info/dependency_links.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)       67 2022-03-04 18:17:04.000000 pympc-1.0.0/pympc.egg-info/entry_points.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)       54 2022-03-04 18:17:04.000000 pympc-1.0.0/pympc.egg-info/requires.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)       11 2022-03-04 18:17:04.000000 pympc-1.0.0/pympc.egg-info/top_level.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)      113 2022-03-04 18:17:04.000000 pympc-1.0.0/setup.cfg
--rw-r--r--   0 jdl       (1000) jdl       (1000)      762 2022-03-04 17:41:32.000000 pympc-1.0.0/setup.py
-drwxrwxr-x   0 jdl       (1000) jdl       (1000)        0 2022-03-04 18:17:04.000000 pympc-1.0.0/test/
--rw-r--r--   0 jdl       (1000) jdl       (1000)        0 2021-04-01 14:53:21.000000 pympc-1.0.0/test/__init__.py
--rw-r--r--   0 jdl       (1000) jdl       (1000)     2685 2022-03-04 17:52:28.000000 pympc-1.0.0/test/test_pympc.py
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:09:34.000000 pympc-1.1.0/
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)    32422 2019-09-12 12:07:32.000000 pympc-1.1.0/LICENSE.txt
+-rw-r--r--   0 jdl       (1000) jdl       (1000)     7286 2023-07-26 12:09:34.000000 pympc-1.1.0/PKG-INFO
+-rw-r--r--   0 jdl       (1000) jdl       (1000)     6939 2023-07-25 17:00:47.000000 pympc-1.1.0/README.md
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc/
+-rw-r--r--   0 jdl       (1000) jdl       (1000)      150 2023-07-26 12:08:44.000000 pympc-1.1.0/pympc/__init__.py
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc/data/
+-rw-r--r--   0 jdl       (1000) jdl       (1000)    84540 2022-03-04 16:22:51.000000 pympc-1.1.0/pympc/data/obs_codes.npy
+-rw-r--r--   0 jdl       (1000) jdl       (1000)    26650 2023-04-21 16:04:55.000000 pympc-1.1.0/pympc/pympc.py
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)     7286 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/PKG-INFO
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)      310 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/SOURCES.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)        1 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/dependency_links.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)       67 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/entry_points.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)       56 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/requires.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)       11 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/top_level.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)      113 2023-07-26 12:09:34.000000 pympc-1.1.0/setup.cfg
+-rw-r--r--   0 jdl       (1000) jdl       (1000)      764 2023-07-26 11:58:35.000000 pympc-1.1.0/setup.py
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:09:34.000000 pympc-1.1.0/test/
+-rw-r--r--   0 jdl       (1000) jdl       (1000)        0 2021-04-01 14:53:21.000000 pympc-1.1.0/test/__init__.py
+-rw-r--r--   0 jdl       (1000) jdl       (1000)     8914 2023-07-26 12:08:44.000000 pympc-1.1.0/test/test_pympc.py
```

### Comparing `pympc-1.0.0/LICENSE.txt` & `pympc-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pympc-1.0.0/PKG-INFO` & `pympc-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympc
-Version: 1.0.0
+Version: 1.1.0
 Summary: minor planet checking
 Home-page: https://github.com/lyalpha/pympc
 Author: Joe Lyman
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
@@ -121,22 +121,28 @@
 > an existing observatory code must be passed.
 
 ## Limitations
 The orbits are propagated following [xephem](http://www.clearskyinstitute.com/xephem) (via the 
 [pyephem](https://rhodesmill.org/pyephem/) package), and this does not account for perturbations of the orbits. Thus, 
 the accuracy of the position is dependent on the time difference between the epoch of the orbit elements and the epoch 
 at which the search is being performed. Epoch differences between orbital elements calculation and observation of 
-around a month or two should be fine for typical positional accuracies of less than a few arcsecond for the vast
+around a month or two are fine for typical positional accuracies of less than a few arcsecond for the vast
 majority of minor bodies. Note, however, that a small number of bodies (those undergoing strong perturbations and
-close to Earth) maybe quite inaccurate (arcminutes).
+close to Earth) maybe quite inaccurate (arcminutes). A fuller analysis is given in [notebooks/positional_accuracy.ipynb](notebooks/positional_accuracy.ipynb).
+
+![histogram showing positional accuracy of pympc vs minor planet center](/notebooks/position_accuracy.png "Histogram showing positional accuracy of `pympc` vs Minor Planet Center")
 
 The `xephem` package can only provide geocentric astrometric positions. `pympc` will calculate the topocentric 
 correction as a post-processing to the initial position. The simple geometric correction applied is more than sufficient
 for the overwhelming majority of minor bodies, but for some near earth objects the correction can be large and the 
-relatively simple treatment by `pympc` may not be sufficient.
+relatively simple treatment by `pympc` may not be sufficient. Additionally, in order to find matches in geocentric
+positions prior to applying the topocentric correction, a buffer is added to the search radius - this should capture
+the vast majority of cases where the geocentric position is outside the seach radius but the topocentric position is 
+within it - although no guarantees. To work around this you can artifically inflate your search radius and filter
+yourself afterwards.
 
 The filtering of matches based on magnitude via `max_mag` argument to `minor_planet_check()` is limited by the accuracy 
 of the magnitude information in the database so some buffer should be applied to the desired magnitude cutoff to allow 
 for this.
 
 ### Acknowledgements
 This package makes use of data and/or services provided by the International Astronomical Union's
```

### Comparing `pympc-1.0.0/README.md` & `pympc-1.1.0/pympc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: pympc
+Version: 1.1.0
+Summary: minor planet checking
+Home-page: https://github.com/lyalpha/pympc
+Author: Joe Lyman
+License: GNU General Public License v3 (GPLv3)
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 pympc
 =====
 
 Perform checks for the presence of minor bodies at astronomical locations for a given epoch.
 
 ## Installation
 
@@ -108,28 +121,35 @@
 > an existing observatory code must be passed.
 
 ## Limitations
 The orbits are propagated following [xephem](http://www.clearskyinstitute.com/xephem) (via the 
 [pyephem](https://rhodesmill.org/pyephem/) package), and this does not account for perturbations of the orbits. Thus, 
 the accuracy of the position is dependent on the time difference between the epoch of the orbit elements and the epoch 
 at which the search is being performed. Epoch differences between orbital elements calculation and observation of 
-around a month or two should be fine for typical positional accuracies of less than a few arcsecond for the vast
+around a month or two are fine for typical positional accuracies of less than a few arcsecond for the vast
 majority of minor bodies. Note, however, that a small number of bodies (those undergoing strong perturbations and
-close to Earth) maybe quite inaccurate (arcminutes).
+close to Earth) maybe quite inaccurate (arcminutes). A fuller analysis is given in [notebooks/positional_accuracy.ipynb](notebooks/positional_accuracy.ipynb).
+
+![histogram showing positional accuracy of pympc vs minor planet center](/notebooks/position_accuracy.png "Histogram showing positional accuracy of `pympc` vs Minor Planet Center")
 
 The `xephem` package can only provide geocentric astrometric positions. `pympc` will calculate the topocentric 
 correction as a post-processing to the initial position. The simple geometric correction applied is more than sufficient
 for the overwhelming majority of minor bodies, but for some near earth objects the correction can be large and the 
-relatively simple treatment by `pympc` may not be sufficient.
+relatively simple treatment by `pympc` may not be sufficient. Additionally, in order to find matches in geocentric
+positions prior to applying the topocentric correction, a buffer is added to the search radius - this should capture
+the vast majority of cases where the geocentric position is outside the seach radius but the topocentric position is 
+within it - although no guarantees. To work around this you can artifically inflate your search radius and filter
+yourself afterwards.
 
 The filtering of matches based on magnitude via `max_mag` argument to `minor_planet_check()` is limited by the accuracy 
 of the magnitude information in the database so some buffer should be applied to the desired magnitude cutoff to allow 
 for this.
 
 ### Acknowledgements
 This package makes use of data and/or services provided by the International Astronomical Union's 
 [Minor Planet Center](https://www.minorplanetcenter.net).
 
 Orbit elements are also sourced from [Lowell Observatory](https://asteroid.lowell.edu/main/), which is funded by the 
 Lowell Observatory Endowment and NASA PDART grant NNX16AG52G.
 
-Based from a package developed by Chris Klein and Duncan Galloway.
+Based from a package developed by Chris Klein and Duncan Galloway.
+
```

### Comparing `pympc-1.0.0/pympc/data/obs_codes.npy` & `pympc-1.1.0/pympc/data/obs_codes.npy`

 * *Files identical despite different names*

### Comparing `pympc-1.0.0/pympc/pympc.py` & `pympc-1.1.0/pympc/pympc.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,16 +37,17 @@
     },
 }
 MPCORB_XEPHEM = "mpcorb_xephem.csv"
 OBS_CODES_ARRAY_PATH = pkg_resources.resource_filename(__name__, "data/obs_codes.npy")
 DAY_IN_YEAR = 365.25689
 RADTODEG = 180.0 / np.pi
 DEGTORAD = 1 / RADTODEG
-# angle subtended by Earth's equatorial radius at a distance of 1 AU in radians
-SOLAR_PARALLAX = 8.794143 / 3600.0 / RADTODEG
+# angle subtended by Earth's equatorial radius at a distance of 1 AU
+SOLAR_PARALLAX_ARCSEC = 8.794143
+SOLAR_PARALLAX_RAD = (SOLAR_PARALLAX_ARCSEC / 3600.0) * DEGTORAD
 
 
 def update_catalogue(include_nea=True, include_comets=True, cat_dir=None, cleanup=True):
     """
     download MPC asteroid orbit elements and save as csv database readable by xephem
 
     must be run prior to doing any minor planet checking.
@@ -216,15 +217,15 @@
     ra,
     dec,
     epoch,
     search_radius,
     xephem_filepath=None,
     max_mag=None,
     observatory=(0.0, 0.0, 0.0),
-    chunk_size=2e4,
+    chunk_size=20000,
 ):
     """
     perform a minor planet check around a search position
 
     this is a convenience call to _minor_planet_check(), which actually does
     the work, and allows more flexibility in argument format.
 
@@ -251,18 +252,23 @@
         default returns geometric positions.
     chunk_size : int, optional
         the chunk size for multiprocessing of the search. avoid setting too low
         (<<1e4) to avoid large setup time costs. set to 0 to disable multiprocessing.
 
     Returns
     -------
-    results : list of length 4-tuples
-        a list of matching minor planet entries. each list entry is a tuple of the format
-        ((ra [degrees], dec [degrees]), separation in arcseconds, magnitude of body,
-        xephem db-formatted string of matched body)
+    results : astropy.table.Table object
+        a table of minor planet matches, with columns:
+            * name - the name of the minor planet
+            * ra - the RA of the minor planet at the given epoch
+            * dec - the Dec of the minor planet at the given epoch
+            * mag - the magnitude of the minor planet as given by the orbital catalogue
+            * separation - the angular separation between the minor planet and the search position in arcseconds
+            * xephem_str - the xephem string for the minor planet
+
 
     Notes
     -----
     If passing an observatory code it should match one defined in the Minor Planet Center
     list of obseratory codes (see https://minorplanetcenter.net/iau/lists/ObsCodes.html).
     """
     coo = []
@@ -378,24 +384,42 @@
         logger.exception(
             "xephem db csv file not found at {}. run pympc.update_catalogue() "
             "if necessary.".format(xephem_filepath)
         )
         raise
     if max_mag is None:
         max_mag = np.inf
+    if any([longitude, rho_cos_phi, rho_sin_phi]):
+        # If we are using topocentric coordinates, there needs to be a small buffer
+        # on searching to ensure the geocentric coordinates returned by xephem contain
+        # all matches within the search radius, once topocentric corrections are applied.
+        # This buffer is roughly the maximal correction for a 1/3 AU distance object. We
+        # incure a slight speed penalty for this, but it is necessary.
+        search_radius_buffer = SOLAR_PARALLAX_ARCSEC * 3
+    else:
+        search_radius_buffer = 0
+
     logger.info(
         "searching for minor planets within {:.2f} arcsec of ra, dec = {:.5f}, {:.5f} rad at MJD = {:.5f}".format(
             search_radius, ra, dec, Time(epoch, format="decimalyear").mjd
         )
     )
     date = ephem.date(str(epoch))
     t0 = time()
     if c == 0:
         results = _cone_search_xephem_entries(
-            xephem_db, (ra, dec), date, search_radius, max_mag, longitude, rho_cos_phi, rho_sin_phi
+            xephem_db,
+            (ra, dec),
+            date,
+            search_radius,
+            max_mag,
+            longitude,
+            rho_cos_phi,
+            rho_sin_phi,
+            search_radius_buffer,
         )
     else:
         xephem_db_chunks = np.array_split(xephem_db, max(len(xephem_db) // c, 1))
         with Pool() as pool:
             results = pool.starmap(
                 _cone_search_xephem_entries,
                 zip(
@@ -403,25 +427,26 @@
                     repeat((ra, dec)),
                     repeat(date),
                     repeat(search_radius),
                     repeat(max_mag),
                     repeat(longitude),
                     repeat(rho_cos_phi),
                     repeat(rho_sin_phi),
+                    repeat(search_radius_buffer),
                 ),
             )
         # flatten our list of lists
         results = [r for result in results for r in result]
     logger.info("search took {:.1f} seconds".format(time() - t0))
     logger.info("found {} matches".format(len(results)))
     return results
 
 
 def _cone_search_xephem_entries(
-    xephem_db, coo, date, search_radius, max_mag, longitude, rho_cos_phi, rho_sin_phi,
+    xephem_db, coo, date, search_radius, max_mag, longitude, rho_cos_phi, rho_sin_phi, buffer
 ):
     """
     performs a cone search around a `ra`, `dec` position at `date` to locate any entries
     in the provided `xephem_db` entries that match within `search_radius`.
 
     Parameters
     ----------
@@ -437,41 +462,47 @@
         maximum magnitude of minor planet matches to return.
     longitude: float
         Longitude of observer in degrees.
     rho_cos_phi: float
         Parallax constant for cosine of the latitude of the observer.
     rho_sin_phi: float
         Parallax constant for sine of the latitude of the observer.
+    buffer: float
+        Buffer to add to search radius to ensure all matches are found even after
+        topocentric corrections are applied.
 
     Returns
     -------
     results : list of length 4-tuples
         a list of matching minor planet entries. each list entry is a tuple of the format
         ((ra [degrees], dec [degrees]), separation in arcseconds, magnitude of body,
         xephem db-formatted string of matched body)
     """
     results = []
     for xephem_str in xephem_db:
         mp = ephem.readdb(xephem_str.strip())
         mp.compute(date)
         separation = 3600.0 * RADTODEG * (float(ephem.separation((mp.a_ra, mp.a_dec), coo)))
-        if separation <= search_radius and mp.mag <= max_mag:
+        # First match geocentric positions against the buffered search radius
+        if separation <= search_radius + buffer and mp.mag <= max_mag:
             ra, dec = float(mp.a_ra), float(mp.a_dec)
             if any([longitude, rho_cos_phi, rho_sin_phi]):
                 # Perform a topocentric correction
                 ra, dec = equitorial_geocentric_to_topocentric(
                     mp.a_ra,
                     mp.a_dec,
                     mp.earth_distance,
                     date.datetime(),
                     longitude,
                     rho_cos_phi,
                     rho_sin_phi,
                 )
                 separation = 3600.0 * RADTODEG * (float(ephem.separation((ra, dec), coo)))
+                # Apply the search radius check again, here without the buffer since we now have
+                # topocentric coordinates
                 if separation > search_radius:
                     continue
             results.append(
                 [
                     _get_minor_planet_name(xephem_str),
                     ra * RADTODEG,
                     dec * RADTODEG,
@@ -515,15 +546,15 @@
     """
 
     ra_geo = ra_geo
     dec_geo = dec_geo
     local_sidereal_time = Time(epoch).sidereal_time("apparent", longitude=longitude).radian
     local_hour_angle = local_sidereal_time - ra_geo
 
-    parallax = SOLAR_PARALLAX / dist_au
+    parallax = SOLAR_PARALLAX_RAD / dist_au
     incrra = np.arctan2(
         -(rho_cos_phi * np.sin(parallax) * np.sin(local_hour_angle)),
         np.cos(dec_geo) - rho_cos_phi * np.sin(parallax) * np.cos(local_hour_angle),
     )
     ra_topo = ra_geo + incrra
     dec_topo = np.arctan2(
         np.cos(incrra) * (np.sin(dec_geo) - rho_sin_phi * np.sin(parallax)),
```

### Comparing `pympc-1.0.0/pympc.egg-info/PKG-INFO` & `pympc-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: pympc
-Version: 1.0.0
-Summary: minor planet checking
-Home-page: https://github.com/lyalpha/pympc
-Author: Joe Lyman
-License: GNU General Public License v3 (GPLv3)
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 pympc
 =====
 
 Perform checks for the presence of minor bodies at astronomical locations for a given epoch.
 
 ## Installation
 
@@ -121,29 +108,34 @@
 > an existing observatory code must be passed.
 
 ## Limitations
 The orbits are propagated following [xephem](http://www.clearskyinstitute.com/xephem) (via the 
 [pyephem](https://rhodesmill.org/pyephem/) package), and this does not account for perturbations of the orbits. Thus, 
 the accuracy of the position is dependent on the time difference between the epoch of the orbit elements and the epoch 
 at which the search is being performed. Epoch differences between orbital elements calculation and observation of 
-around a month or two should be fine for typical positional accuracies of less than a few arcsecond for the vast
+around a month or two are fine for typical positional accuracies of less than a few arcsecond for the vast
 majority of minor bodies. Note, however, that a small number of bodies (those undergoing strong perturbations and
-close to Earth) maybe quite inaccurate (arcminutes).
+close to Earth) maybe quite inaccurate (arcminutes). A fuller analysis is given in [notebooks/positional_accuracy.ipynb](notebooks/positional_accuracy.ipynb).
+
+![histogram showing positional accuracy of pympc vs minor planet center](/notebooks/position_accuracy.png "Histogram showing positional accuracy of `pympc` vs Minor Planet Center")
 
 The `xephem` package can only provide geocentric astrometric positions. `pympc` will calculate the topocentric 
 correction as a post-processing to the initial position. The simple geometric correction applied is more than sufficient
 for the overwhelming majority of minor bodies, but for some near earth objects the correction can be large and the 
-relatively simple treatment by `pympc` may not be sufficient.
+relatively simple treatment by `pympc` may not be sufficient. Additionally, in order to find matches in geocentric
+positions prior to applying the topocentric correction, a buffer is added to the search radius - this should capture
+the vast majority of cases where the geocentric position is outside the seach radius but the topocentric position is 
+within it - although no guarantees. To work around this you can artifically inflate your search radius and filter
+yourself afterwards.
 
 The filtering of matches based on magnitude via `max_mag` argument to `minor_planet_check()` is limited by the accuracy 
 of the magnitude information in the database so some buffer should be applied to the desired magnitude cutoff to allow 
 for this.
 
 ### Acknowledgements
 This package makes use of data and/or services provided by the International Astronomical Union's 
 [Minor Planet Center](https://www.minorplanetcenter.net).
 
 Orbit elements are also sourced from [Lowell Observatory](https://asteroid.lowell.edu/main/), which is funded by the 
 Lowell Observatory Endowment and NASA PDART grant NNX16AG52G.
 
-Based from a package developed by Chris Klein and Duncan Galloway.
-
+Based from a package developed by Chris Klein and Duncan Galloway.
```

### Comparing `pympc-1.0.0/setup.py` & `pympc-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     name="pympc",
     author="Joe Lyman",
     description="minor planet checking",
     packages=setuptools.find_packages(),
-    install_requires=["ephem>=3.7.7.1", "astropy>=4.2", "pandas>=1.0", "requests>=2.0"],
+    install_requires=["ephem>=3.7.7.1", "astropy>=4.2", "pandas>=1.0", "pyerfa>=2.0.0.0"],
     license="GNU General Public License v3 (GPLv3)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lyalpha/pympc",
     entry_points={"console_scripts": ["minor_planet_check=pympc.pympc:_console_script"]},
     classifiers=["Programming Language :: Python :: 3"],
     python_requires=">=3.6",
```

