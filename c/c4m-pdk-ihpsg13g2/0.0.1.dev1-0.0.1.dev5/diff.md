# Comparing `tmp/c4m_pdk_ihpsg13g2-0.0.1.dev1.tar.gz` & `tmp/c4m_pdk_ihpsg13g2-0.0.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_pdk_ihpsg13g2-0.0.1.dev1.tar", last modified: Sun Jun 25 22:00:06 2023, max compression
+gzip compressed data, was "c4m_pdk_ihpsg13g2-0.0.1.dev5.tar", last modified: Wed Jul 26 13:46:33 2023, max compression
```

## Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1.tar` & `c4m_pdk_ihpsg13g2-0.0.1.dev5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 22:00:06.240271 c4m_pdk_ihpsg13g2-0.0.1.dev1/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       90 2023-06-25 21:37:52.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-06-23 16:20:33.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/LICENSE.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 22:00:06.236271 c4m_pdk_ihpsg13g2-0.0.1.dev1/LICENSES/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2023-06-23 16:20:33.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/LICENSES/agpl-3.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-06-23 16:20:33.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/LICENSES/apache-2.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2023-06-23 16:20:33.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/LICENSES/cern_ohl_s_v2.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2023-06-23 16:20:33.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/LICENSES/gpl-2.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3345 2023-06-25 22:00:06.240271 c4m_pdk_ihpsg13g2-0.0.1.dev1/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2866 2023-06-25 21:37:46.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/README.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 22:00:06.236271 c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 22:00:06.236271 c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m/pdk/
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 22:00:06.240271 c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m/pdk/ihpsg13g2/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      256 2023-06-25 21:37:52.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m/pdk/ihpsg13g2/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    14457 2023-06-25 21:37:52.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m/pdk/ihpsg13g2/pdkmaster.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1171 2023-06-25 21:37:52.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m/pdk/ihpsg13g2/pyspice.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2098 2023-06-25 21:37:52.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m/pdk/ihpsg13g2/stdcell.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 22:00:06.240271 c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m_pdk_ihpsg13g2.egg-info/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3345 2023-06-25 22:00:06.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m_pdk_ihpsg13g2.egg-info/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      479 2023-06-25 22:00:06.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m_pdk_ihpsg13g2.egg-info/SOURCES.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-06-25 22:00:06.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m_pdk_ihpsg13g2.egg-info/dependency_links.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       53 2023-06-25 22:00:06.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m_pdk_ihpsg13g2.egg-info/requires.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-06-25 22:00:06.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m_pdk_ihpsg13g2.egg-info/top_level.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1108 2023-06-25 21:37:52.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/cell_list.yml
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    16597 2023-06-25 21:57:26.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/dodo.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-06-25 22:00:06.240271 c4m_pdk_ihpsg13g2-0.0.1.dev1/setup.cfg
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1497 2023-06-25 21:59:28.000000 c4m_pdk_ihpsg13g2-0.0.1.dev1/setup.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:46:33.075985 c4m_pdk_ihpsg13g2-0.0.1.dev5/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       90 2023-07-14 12:42:38.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      566 2023-07-14 12:42:38.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/LICENSE.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:46:33.071985 c4m_pdk_ihpsg13g2-0.0.1.dev5/LICENSES/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2023-07-14 12:42:38.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/LICENSES/agpl-3.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11358 2023-07-14 12:42:38.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/LICENSES/apache-2.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2023-07-14 12:42:38.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/LICENSES/cern_ohl_s_v2.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2023-07-14 12:42:38.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/LICENSES/gpl-2.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3345 2023-07-26 13:46:33.075985 c4m_pdk_ihpsg13g2-0.0.1.dev5/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2866 2023-07-14 12:42:38.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/README.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:46:33.067985 c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:46:33.067985 c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m/pdk/
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:46:33.075985 c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m/pdk/ihpsg13g2/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      256 2023-07-14 12:42:38.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m/pdk/ihpsg13g2/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    12806 2023-07-26 13:45:33.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m/pdk/ihpsg13g2/pdkmaster.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1171 2023-07-14 12:42:38.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m/pdk/ihpsg13g2/pyspice.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2099 2023-07-26 13:45:33.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m/pdk/ihpsg13g2/stdcell.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-07-26 13:46:33.075985 c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m_pdk_ihpsg13g2.egg-info/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3345 2023-07-26 13:46:33.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m_pdk_ihpsg13g2.egg-info/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      479 2023-07-26 13:46:33.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m_pdk_ihpsg13g2.egg-info/SOURCES.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-07-26 13:46:33.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m_pdk_ihpsg13g2.egg-info/dependency_links.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       53 2023-07-26 13:46:33.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m_pdk_ihpsg13g2.egg-info/requires.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-07-26 13:46:33.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m_pdk_ihpsg13g2.egg-info/top_level.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1108 2023-07-14 12:42:38.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/cell_list.yml
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    16597 2023-07-14 12:42:38.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/dodo.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-07-26 13:46:33.075985 c4m_pdk_ihpsg13g2-0.0.1.dev5/setup.cfg
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1497 2023-07-26 13:45:33.000000 c4m_pdk_ihpsg13g2-0.0.1.dev5/setup.py
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/LICENSE.md` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/LICENSES/agpl-3.0.txt` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/LICENSES/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/LICENSES/apache-2.0.txt` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/LICENSES/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/LICENSES/cern_ohl_s_v2.txt` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/LICENSES/gpl-2.0.txt` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/LICENSES/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/PKG-INFO` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m_pdk_ihpsg13g2
-Version: 0.0.1.dev1
+Version: 0.0.1.dev5
 Summary: IHP SG13G2 as PDKMaster based PDK
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/issues
 Requires-Python: ~=3.6
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/README.md` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/README.md`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m/pdk/ihpsg13g2/pdkmaster.py` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m/pdk/ihpsg13g2/pdkmaster.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,24 +51,14 @@
 
         # single mask based primitives
         NWell = _prm.Well(
             name="NWell", type_=_prm.nImpl,
             min_width=0.62, # NW.a
             min_space=0.62, # NW.b
         )
-        # We need n implant layer as we currently don't support transistor
-        # without an implant.
-        # We take smame design rules as pSD
-        virt_nSD = _prm.Implant(
-            name="virt_nSD", type_=_prm.nImpl,
-            min_width=0.31, # pSD.a
-            min_space=0.31, # pSD.b
-            min_area=0.25, # pSD.k
-            # min_hole_area=0.25, # pSD.l
-        )
         pSD = _prm.Implant(
             name="pSD", type_=_prm.pImpl,
             min_width=0.31, # pSD.a
             min_space=0.31, # pSD.b
             min_area=0.25, # pSD.k
             # min_hole_area=0.25, # pSD.l
         )
@@ -76,23 +66,23 @@
             name="ThickGateOx",
             min_width=0.86, # TGO.f
             min_space=0.86, # TGO.e
         )
         # Recognition layers
         RES = _prm.Marker(name="RES")
         prims += (
-            NWell, virt_nSD, pSD, ThickGateOx, #RES,
+            NWell, pSD, ThickGateOx, #RES,
         )
 
         # layers diff and tap will be generated out of Activ
         Activ = _prm.WaferWire(
             name="Activ", pin=pin_prims["Activ"], blockage=obs_prims["Activ"],
             min_width=0.15, # Act.a
             min_space=0.21, # Act.b
-            allow_in_substrate=True, well=NWell, implant=(virt_nSD, pSD),
+            allow_in_substrate=True, well=NWell, implant=pSD,
             min_implant_enclosure=_prp.Enclosure(0.18), # pSD.c
             implant_abut="none",
             allow_contactless_implant=False,
             min_well_enclosure=_prp.Enclosure(0.31), # NW.c
             min_substrate_enclosure=_prp.Enclosure(0.31), # NW.d
             min_well_enclosure_same_type=_prp.Enclosure(0.03), # pSD.d1
             min_substrate_enclosure_same_type=_prp.Enclosure(0.03), # pSD.sc1
@@ -241,14 +231,17 @@
             min_bottom_enclosure=_prp.Enclosure(2.1), # Pas.c
         )
         prims += (*vias.values(), Passiv)
 
         # misc using wires
         prims += (
             # extra space rules
+            _prm.Spacing( # pSD.d
+                primitives1=Activ, primitives2=pSD, min_space=0.18,
+            ),
             _prm.Spacing( # NW.e
                 primitives1=NWell, primitives2=Activ, min_space=0.24,
             ),
             _prm.Spacing( # TGO.b
                 primitives1=Activ, primitives2=ThickGateOx, min_space=0.27,
             ),
             _prm.Spacing( # Gat.d
@@ -280,44 +273,32 @@
         )
         trans = {
             name: _prm.MOSFET(name=name,
                 gate=gate, implant=impl, well=well,
                 min_gateimplant_enclosure=impl_enc, # Implant.1
             )
             for name, gate, well, impl, impl_enc in (
-                ("sg13g2_lv_nmos", lvmosgate, None, virt_nSD, _prp.Enclosure(0.30)), # pSD.j
+                ("sg13g2_lv_nmos", lvmosgate, None, (), ()),
                 ("sg13g2_lv_pmos", lvmosgate, NWell, pSD, _prp.Enclosure(0.30)), # pSD.i
-                ("sg13g2_hv_nmos", hvmosgate, None, virt_nSD, _prp.Enclosure(0.40)), # pSD.j1
+                ("sg13g2_hv_nmos", hvmosgate, None, (), ()),
                 ("sg13g2_hv_pmos", hvmosgate, NWell, pSD, _prp.Enclosure(0.40)), # pSD.i1
             )
         }
-        # prims += (mosgate, mosgate_sc, hvmosgate, *trans.values())
         prims += (lvmosgate, hvmosgate, *trans.values())
 
-        # bipolars =  tuple(
-        #     _prm.Bipolar(name=name, type_=type_, indicator=ind)
-        #     for name, type_, ind in (
-        #         ("npn_05v5_w1u00l1u00", _prm.npnBipolarT, npn),
-        #         ("npn_05v5_w1u00l2u00", _prm.npnBipolarT, npn),
-        #         ("pnp_05v5_w0u68l0u68", _prm.pnpBipolarT, pnp),
-        #         ("pnp_05v5_w3u40l3u40", _prm.pnpBipolarT, pnp),
-        #     )
-        # )
-        # prims += bipolars
-
-        # prims += _prm.Auxiliary(name="prBoundary")
+        prims += _prm.Auxiliary(name="prBoundary")
 
         super().__init__(primitives=prims)
 
 tech = technology = _IHPSG13G2()
 cktfab = circuit_factory = ckt.CircuitFactory(tech=tech)
 layoutfab = layout_factory = lay.LayoutFactory(tech=tech)
 
 gds_layers: Dict[str, Tuple[int, int]] = {
-    "virt_nSD": (7, 99), # (7, 0) is generated nSD layer
+    "prBoundary": (189, 0),
 }
 # Use datatype 100 for obstruction layer;
 # datatype 23 'nofill' would cause no dummy generation if accidently not removed before tape-out
 for name, layer, has_pin, has_obs in (
     ("Activ", 1, True, True),
     ("GatPoly", 5, True, True),
     ("Cont", 6, False, True),
@@ -341,20 +322,7 @@
     ("TopMetal2", 134, True, True),
 ):
     gds_layers[name] = (layer, 0)
     if has_pin:
         gds_layers[f"{name}.pin"] = (layer, 2)
     if has_obs:
         gds_layers[f"{name}.obs"] = (layer, 100)
-
-# plotter = nb.Plotter({
-#     # "pwell": {"fc": (1.0, 1.0, 0.0, 0.2), "ec": "orange", "zorder": 10},
-#     "nwm": {"fc": (0.0, 0.0, 0.0, 0.1), "ec": "grey", "zorder": 10},
-#     "Activ": {"fc": "lawngreen", "ec": "lawngreen", "zorder": 11},
-#     "poly": {"fc": "red", "ec": "red", "zorder": 12},
-#     "nsdm": {"fc": "purple", "ec": "purple", "alpha": 0.3, "zorder": 13},
-#     "psdm": {"fc": "blueviolet", "ec": "blueviolet", "alpha": 0.3, "zorder": 13},
-#     "lvtn": {"fc": (0.0, 0.0, 0.0, 0.0), "ec": "grey", "zorder": 13},
-#     "hvtp": {"fc": (1, 1, 1, 0.3), "ec": "whitesmoke", "zorder": 13},
-#     "licon": {"fc": "black", "ec": "black", "zorder": 14},
-#     "li": {"fc": (0.1, 0.1, 1, 0.4), "ec": "blue", "zorder": 15},
-# })
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m/pdk/ihpsg13g2/pyspice.py` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m/pdk/ihpsg13g2/pyspice.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m/pdk/ihpsg13g2/stdcell.py` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m/pdk/ihpsg13g2/stdcell.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             lib=lib, cktfab=cktfab, layoutfab=layoutfab,
             name_prefix=name_prefix, name_suffix=name_suffix,
             canvas=stdcell1v2canvas,
         )
 
 
 stdcell1v2canvas = _fab.StdCellCanvas(
-    tech=tech, lambda_=0.05,
+    tech=tech, lambda_=0.060,
     nmos=cast(_prm.MOSFET, prims.sg13g2_lv_nmos), pmos=cast(_prm.MOSFET, prims.sg13g2_lv_pmos),
 )
 stdcell1v2lib = _lbry.RoutingGaugeLibrary(
     name="StdCell1V2Lib", tech=tech, routinggauge=stdcell1v2canvas.routinggauge,
 )
 StdCell1V2Factory(lib=stdcell1v2lib).add_default()
 merge(stdcell1v2lib)
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/c4m_pdk_ihpsg13g2.egg-info/PKG-INFO` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/c4m_pdk_ihpsg13g2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m-pdk-ihpsg13g2
-Version: 0.0.1.dev1
+Version: 0.0.1.dev5
 Summary: IHP SG13G2 as PDKMaster based PDK
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/issues
 Requires-Python: ~=3.6
```

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/cell_list.yml` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/cell_list.yml`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/dodo.py` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/dodo.py`

 * *Files identical despite different names*

### Comparing `c4m_pdk_ihpsg13g2-0.0.1.dev1/setup.py` & `c4m_pdk_ihpsg13g2-0.0.1.dev5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     description="IHP SG13G2 as PDKMaster based PDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+",
     python_requires="~=3.6",
     setup_requires=["setuptools_scm"],
     install_requires=[
-        "setuptools", "PDKMaster~=0.9.3", "c4m-flexcell~=0.4.0.dev0",
+        "setuptools", "PDKMaster~=0.9.4", "c4m-flexcell~=0.4.0.dev9",
     ],
     include_package_data=True,
     packages=_packages,
     project_urls={
         #"Documentation": "???",
         "Source Code": "https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2",
         "Bug Tracker": "https://gitlab.com/Chips4Makers/c4m-pdk-ihpsg13g2/issues",
```

