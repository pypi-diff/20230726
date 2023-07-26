# Comparing `tmp/myokit-1.35.2.tar.gz` & `tmp/myokit-1.35.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myokit-1.35.2.tar", last modified: Wed Jul 19 11:02:37 2023, max compression
+gzip compressed data, was "myokit-1.35.3.tar", last modified: Wed Jul 26 21:00:29 2023, max compression
```

## Comparing `myokit-1.35.2.tar` & `myokit-1.35.3.tar`

### file list

```diff
@@ -1,458 +1,458 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.553743 myokit-1.35.2/
--rw-r--r--   0 michael   (1000) michael   (1000)     1833 2023-07-11 14:14:16.000000 myokit-1.35.2/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      221 2023-06-07 13:48:23.000000 myokit-1.35.2/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     5059 2023-07-19 11:02:37.553743 myokit-1.35.2/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     3821 2023-06-25 10:52:15.000000 myokit-1.35.2/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.496743 myokit-1.35.2/myokit/
--rw-r--r--   0 michael   (1000) michael   (1000)    14034 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    57971 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23743 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_aux.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.497743 myokit-1.35.2/myokit/_bin/
--rw-r--r--   0 michael   (1000) michael   (1000)     6226 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_bin/example.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.502743 myokit-1.35.2/myokit/_bin/gui/
--rw-r--r--   0 michael   (1000) michael   (1000)      784 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/find.png
--rw-r--r--   0 michael   (1000) michael   (1000)    96412 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-128.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     3528 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-16.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-24.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   233500 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-256.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    12232 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-32.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    23817 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-48.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    36761 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-64.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    65257 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-96.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer.ico
--rw-r--r--   0 michael   (1000) michael   (1000)    30396 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer.png
--rw-r--r--   0 michael   (1000) michael   (1000)    47406 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-ide-128.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     2987 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-ide-16.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     4971 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-ide-24.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   152751 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-ide-256.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     7355 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-ide-32.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)     9835 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-ide-48.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    16235 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-ide-64.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)    30683 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-ide-96.xpm
--rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-ide.ico
--rw-r--r--   0 michael   (1000) michael   (1000)    15096 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/icon-ide.png
--rw-r--r--   0 michael   (1000) michael   (1000)      571 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/new.png
--rw-r--r--   0 michael   (1000) michael   (1000)      544 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/open.png
--rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/redo.png
--rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/run.png
--rw-r--r--   0 michael   (1000) michael   (1000)      565 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/save.png
--rw-r--r--   0 michael   (1000) michael   (1000)      284 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/_bin/gui/undo.png
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.503743 myokit-1.35.2/myokit/_bin/install-lin/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      254 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/_bin/install-lin/myokit-datablock-viewer.desktop
--rwxr-xr-x   0 michael   (1000) michael   (1000)      266 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/_bin/install-lin/myokit-datalog-viewer.desktop
--rwxr-xr-x   0 michael   (1000) michael   (1000)      264 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/install-lin/myokit-ide.desktop
--rw-r--r--   0 michael   (1000) michael   (1000)     4338 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/_bin/install-lin/myokit.lang
--rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-06-07 13:47:50.000000 myokit-1.35.2/myokit/_bin/install-lin/x-abf.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      246 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/install-lin/x-cellml.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      247 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/_bin/install-lin/x-myokit.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      275 2023-06-07 13:47:50.000000 myokit-1.35.2/myokit/_bin/install-lin/x-wcp.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.503743 myokit-1.35.2/myokit/_bin/install-win/
--rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_bin/install-win/menu.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.503743 myokit-1.35.2/myokit/_bin/sundials-win-vs/
--rw-r--r--   0 michael   (1000) michael   (1000)     1758 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/LICENSE
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.492743 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.504743 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/cvodes/
--rw-r--r--   0 michael   (1000) michael   (1000)    27506 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h
--rw-r--r--   0 michael   (1000) michael   (1000)     2427 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h
--rw-r--r--   0 michael   (1000) michael   (1000)    12344 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.504743 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/nvector/
--rw-r--r--   0 michael   (1000) michael   (1000)     8934 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.506743 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/
--rw-r--r--   0 michael   (1000) michael   (1000)     5785 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h
--rw-r--r--   0 michael   (1000) michael   (1000)     8997 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h
--rw-r--r--   0 michael   (1000) michael   (1000)    13330 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h
--rw-r--r--   0 michael   (1000) michael   (1000)     1024 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h
--rw-r--r--   0 michael   (1000) michael   (1000)    10283 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h
--rw-r--r--   0 michael   (1000) michael   (1000)     9385 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h
--rw-r--r--   0 michael   (1000) michael   (1000)     5420 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h
--rw-r--r--   0 michael   (1000) michael   (1000)     9190 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h
--rw-r--r--   0 michael   (1000) michael   (1000)    12559 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h
--rw-r--r--   0 michael   (1000) michael   (1000)     5165 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h
--rw-r--r--   0 michael   (1000) michael   (1000)     1266 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.506743 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sunlinsol/
--rw-r--r--   0 michael   (1000) michael   (1000)     2983 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.506743 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sunmatrix/
--rw-r--r--   0 michael   (1000) michael   (1000)     3647 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.513743 myokit-1.35.2/myokit/_bin/sundials-win-vs/lib/
--rw-r--r--   0 michael   (1000) michael   (1000)   677888 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll
--rw-r--r--   0 michael   (1000) michael   (1000)   169196 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib
--rw-r--r--   0 michael   (1000) michael   (1000)   160768 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll
--rw-r--r--   0 michael   (1000) michael   (1000)    59576 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib
--rw-r--r--   0 michael   (1000) michael   (1000)    11987 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/_config.py
--rw-r--r--   0 michael   (1000) michael   (1000)    89061 2023-07-18 23:19:29.000000 myokit-1.35.2/myokit/_datablock.py
--rw-r--r--   0 michael   (1000) michael   (1000)    67472 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_datalog.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11060 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_err.py
--rw-r--r--   0 michael   (1000) michael   (1000)   103962 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_expressions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8948 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_io.py
--rw-r--r--   0 michael   (1000) michael   (1000)   193081 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/_model_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)      726 2023-07-19 11:01:45.000000 myokit-1.35.2/myokit/_myokit_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)    74065 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_parsing.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4410 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_progress.py
--rw-r--r--   0 michael   (1000) michael   (1000)    30595 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/_protocol.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.517743 myokit-1.35.2/myokit/_sim/
--rw-r--r--   0 michael   (1000) michael   (1000)    13412 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_sim/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    19156 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/_sim/cable.c
--rw-r--r--   0 michael   (1000) michael   (1000)    18908 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/_sim/cable.py
--rw-r--r--   0 michael   (1000) michael   (1000)    38785 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/_sim/cmodel.h
--rw-r--r--   0 michael   (1000) michael   (1000)    15775 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_sim/cmodel.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4047 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_sim/compiler.c
--rw-r--r--   0 michael   (1000) michael   (1000)     2664 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_sim/compiler.py
--rw-r--r--   0 michael   (1000) michael   (1000)    72435 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/_sim/cvodessim.c
--rw-r--r--   0 michael   (1000) michael   (1000)    43186 2023-07-18 22:48:59.000000 myokit-1.35.2/myokit/_sim/cvodessim.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15446 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_sim/differential.hpp
--rw-r--r--   0 michael   (1000) michael   (1000)    47444 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/_sim/fiber_tissue.c
--rw-r--r--   0 michael   (1000) michael   (1000)    50792 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/_sim/fiber_tissue.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8012 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_sim/jacobian.cpp
--rw-r--r--   0 michael   (1000) michael   (1000)    12957 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_sim/jacobian.py
--rw-r--r--   0 michael   (1000) michael   (1000)    32352 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_sim/mcl.h
--rw-r--r--   0 michael   (1000) michael   (1000)     5037 2023-06-25 10:43:52.000000 myokit-1.35.2/myokit/_sim/opencl.c
--rw-r--r--   0 michael   (1000) michael   (1000)    16446 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_sim/opencl.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46541 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/_sim/openclsim.c
--rw-r--r--   0 michael   (1000) michael   (1000)    19360 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_sim/openclsim.cl
--rw-r--r--   0 michael   (1000) michael   (1000)    69159 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/_sim/openclsim.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29888 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/_sim/pacing.h
--rw-r--r--   0 michael   (1000) michael   (1000)    10914 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_sim/rhs.c
--rw-r--r--   0 michael   (1000) michael   (1000)     7392 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_sim/rhs.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1720 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/_sim/sundials.c
--rw-r--r--   0 michael   (1000) michael   (1000)     2972 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_sim/sundials.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4602 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/_system.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29849 2023-07-12 17:16:09.000000 myokit-1.35.2/myokit/_unit.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3066 2023-07-14 13:14:46.000000 myokit-1.35.2/myokit/float.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.517743 myokit-1.35.2/myokit/formats/
--rw-r--r--   0 michael   (1000) michael   (1000)    26714 2023-07-14 10:16:32.000000 myokit-1.35.2/myokit/formats/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.518743 myokit-1.35.2/myokit/formats/ansic/
--rw-r--r--   0 michael   (1000) michael   (1000)     3347 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/ansic/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3566 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/ansic/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5361 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/ansic/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.518743 myokit-1.35.2/myokit/formats/ansic/template/
--rw-r--r--   0 michael   (1000) michael   (1000)    11965 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/ansic/template/cable.c
--rw-r--r--   0 michael   (1000) michael   (1000)     6044 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/ansic/template/euler.c
--rw-r--r--   0 michael   (1000) michael   (1000)    14244 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/ansic/template/sim.c
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.519743 myokit-1.35.2/myokit/formats/axon/
--rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/axon/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    74286 2023-07-14 10:16:32.000000 myokit-1.35.2/myokit/formats/axon/_abf.py
--rw-r--r--   0 michael   (1000) michael   (1000)    10543 2023-07-12 17:16:09.000000 myokit-1.35.2/myokit/formats/axon/_atf.py
--rw-r--r--   0 michael   (1000) michael   (1000)      826 2023-07-12 17:16:09.000000 myokit-1.35.2/myokit/formats/axon/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.519743 myokit-1.35.2/myokit/formats/cellml/
--rw-r--r--   0 michael   (1000) michael   (1000)     1466 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cellml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2719 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cellml/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2283 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cellml/_exporter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2229 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cellml/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.519743 myokit-1.35.2/myokit/formats/cellml/v1/
--rw-r--r--   0 michael   (1000) michael   (1000)      608 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cellml/v1/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    59011 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cellml/v1/_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)    43554 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cellml/v1/_parser.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15055 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cellml/v1/_writer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.520743 myokit-1.35.2/myokit/formats/cellml/v2/
--rw-r--r--   0 michael   (1000) michael   (1000)      598 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cellml/v2/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    59012 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cellml/v2/_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29536 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cellml/v2/_parser.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11994 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cellml/v2/_writer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.520743 myokit-1.35.2/myokit/formats/channelml/
--rw-r--r--   0 michael   (1000) michael   (1000)      443 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/channelml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    14605 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/channelml/_importer.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.520743 myokit-1.35.2/myokit/formats/cpp/
--rw-r--r--   0 michael   (1000) michael   (1000)      526 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cpp/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      421 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cpp/_ewriter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.520743 myokit-1.35.2/myokit/formats/cuda/
--rw-r--r--   0 michael   (1000) michael   (1000)      816 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cuda/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4472 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cuda/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2059 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cuda/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.520743 myokit-1.35.2/myokit/formats/cuda/template/
--rw-r--r--   0 michael   (1000) michael   (1000)     8863 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/cuda/template/kernel.cu
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.521743 myokit-1.35.2/myokit/formats/easyml/
--rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/easyml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3482 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/easyml/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15771 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/easyml/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.521743 myokit-1.35.2/myokit/formats/heka/
--rw-r--r--   0 michael   (1000) michael   (1000)      761 2023-07-14 10:16:32.000000 myokit-1.35.2/myokit/formats/heka/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1154 2023-07-14 10:16:32.000000 myokit-1.35.2/myokit/formats/heka/_importer.py
--rw-r--r--   0 michael   (1000) michael   (1000)    90645 2023-07-18 23:18:20.000000 myokit-1.35.2/myokit/formats/heka/_patchmaster.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.521743 myokit-1.35.2/myokit/formats/html/
--rw-r--r--   0 michael   (1000) michael   (1000)      457 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/html/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2343 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/html/_exporter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6606 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/html/_flatten.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.521743 myokit-1.35.2/myokit/formats/latex/
--rw-r--r--   0 michael   (1000) michael   (1000)      682 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/latex/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6690 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/latex/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5117 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/latex/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.522743 myokit-1.35.2/myokit/formats/mathml/
--rw-r--r--   0 michael   (1000) michael   (1000)      637 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/mathml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    12194 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/mathml/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)    34289 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/mathml/_parser.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.522743 myokit-1.35.2/myokit/formats/matlab/
--rw-r--r--   0 michael   (1000) michael   (1000)      695 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/matlab/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3172 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/matlab/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2868 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/matlab/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.522743 myokit-1.35.2/myokit/formats/matlab/template/
--rw-r--r--   0 michael   (1000) michael   (1000)      528 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/formats/matlab/template/constants.m
--rw-r--r--   0 michael   (1000) michael   (1000)      374 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/formats/matlab/template/ifthenelse.m
--rw-r--r--   0 michael   (1000) michael   (1000)     2095 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/matlab/template/main.m
--rw-r--r--   0 michael   (1000) michael   (1000)      861 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/formats/matlab/template/model.m
--rw-r--r--   0 michael   (1000) michael   (1000)      461 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/formats/matlab/template/model_wrapper.m
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.523743 myokit-1.35.2/myokit/formats/opencl/
--rw-r--r--   0 michael   (1000) michael   (1000)     6962 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/opencl/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5261 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/opencl/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3903 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/opencl/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.523743 myokit-1.35.2/myokit/formats/opencl/template/
--rw-r--r--   0 michael   (1000) michael   (1000)    11633 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/opencl/template/cable.c
--rw-r--r--   0 michael   (1000) michael   (1000)     8158 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/opencl/template/kernel.cl
--rw-r--r--   0 michael   (1000) michael   (1000)     9018 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/opencl/template/minilog.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1042 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/formats/opencl/template/plot.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      162 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/opencl/template/test.sh
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.524743 myokit-1.35.2/myokit/formats/python/
--rw-r--r--   0 michael   (1000) michael   (1000)     1049 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/python/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6751 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/python/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)      969 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/python/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.524743 myokit-1.35.2/myokit/formats/python/template/
--rw-r--r--   0 michael   (1000) michael   (1000)    10311 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/python/template/sim.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.524743 myokit-1.35.2/myokit/formats/sbml/
--rw-r--r--   0 michael   (1000) michael   (1000)      653 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/sbml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    59396 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/sbml/_api.py
--rw-r--r--   0 michael   (1000) michael   (1000)      987 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/sbml/_importer.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29181 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/sbml/_parser.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.524743 myokit-1.35.2/myokit/formats/stan/
--rw-r--r--   0 michael   (1000) michael   (1000)     2877 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/stan/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3102 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/stan/_ewriter.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3745 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/stan/_exporter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.525743 myokit-1.35.2/myokit/formats/stan/template/
--rw-r--r--   0 michael   (1000) michael   (1000)     5305 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/stan/template/cell.stan
--rwxr-xr-x   0 michael   (1000) michael   (1000)       92 2023-02-05 15:45:10.000000 myokit-1.35.2/myokit/formats/stan/template/run.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.525743 myokit-1.35.2/myokit/formats/sympy/
--rw-r--r--   0 michael   (1000) michael   (1000)     1638 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/sympy/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6758 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/sympy/_ereader.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4875 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/sympy/_ewriter.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.525743 myokit-1.35.2/myokit/formats/wcp/
--rw-r--r--   0 michael   (1000) michael   (1000)      254 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/wcp/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    17140 2023-07-14 10:16:32.000000 myokit-1.35.2/myokit/formats/wcp/_wcp.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.525743 myokit-1.35.2/myokit/formats/xml/
--rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/xml/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1494 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/xml/_exporter.py
--rw-r--r--   0 michael   (1000) michael   (1000)      393 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/formats/xml/_split.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.526743 myokit-1.35.2/myokit/gui/
--rw-r--r--   0 michael   (1000) michael   (1000)     6154 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/gui/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    49529 2023-07-19 10:57:19.000000 myokit-1.35.2/myokit/gui/datablock_viewer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    32561 2023-07-18 22:48:59.000000 myokit-1.35.2/myokit/gui/datalog_viewer.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8588 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/gui/explorer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)   108238 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/gui/ide.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2157 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/gui/progress.py
--rw-r--r--   0 michael   (1000) michael   (1000)    52418 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/gui/source.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6072 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/gui/vargrapher.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.527743 myokit-1.35.2/myokit/lib/
--rw-r--r--   0 michael   (1000) michael   (1000)      216 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/lib/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    23859 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/lib/deps.py
--rw-r--r--   0 michael   (1000) michael   (1000)    28056 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/lib/guess.py
--rw-r--r--   0 michael   (1000) michael   (1000)    46678 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/lib/hh.py
--rw-r--r--   0 michael   (1000) michael   (1000)    67773 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/lib/markov.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4408 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/lib/multi.py
--rw-r--r--   0 michael   (1000) michael   (1000)    13874 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/lib/plots.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4552 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/pacing.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8230 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/pype.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.533743 myokit-1.35.2/myokit/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2738 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/tests/ansic_event_based_pacing.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1250 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/tests/ansic_time_series_pacing.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.536743 myokit-1.35.2/myokit/tests/data/
--rw-r--r--   0 michael   (1000) michael   (1000)     3022 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/tests/data/beeler-1977-model-compare-a.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     2889 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/data/beeler-1977-model-compare-b.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3137 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/tests/data/beeler-1977-model.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/beeler-1977-protocol.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/beeler-1977-script.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3287 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/tests/data/beeler-1977-units.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     5091 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/data/clancy-1999-fitting.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3128 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/conditional.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     6067 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/tests/data/cv1d.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/cv1d.zip
--rw-r--r--   0 michael   (1000) michael   (1000)    23916 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/decker-2009.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)    18350 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/decker.model
--rw-r--r--   0 michael   (1000) michael   (1000)    10416 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/dn-1985-normalised.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      800 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/dom-markov.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.537743 myokit-1.35.2/myokit/tests/data/formats/
--rw-r--r--   0 michael   (1000) michael   (1000)     8192 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/abf-protocol.pro
--rw-r--r--   0 michael   (1000) michael   (1000)    98376 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/abf-v1.abf
--rw-r--r--   0 michael   (1000) michael   (1000)    44544 2023-07-12 17:16:09.000000 myokit-1.35.2/myokit/tests/data/formats/abf-v2.abf
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.540743 myokit-1.35.2/myokit/tests/data/formats/cellml/
--rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/cellml/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)    59093 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/cellml/br-1977-dot.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)    58593 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/cellml/br-1977.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)   117223 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/cellml/corrias.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)   221953 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/cellml/decker-2009.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)     1595 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/cellml/documentation.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/cellml/invalid-file.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)    44837 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml
--rw-r--r--   0 michael   (1000) michael   (1000)    44947 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.542743 myokit-1.35.2/myokit/tests/data/formats/channelml/
--rw-r--r--   0 michael   (1000) michael   (1000)     2648 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      557 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     2702 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     2369 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1258 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1539 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1290 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1289 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1374 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1373 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)      675 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1398 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml
--rw-r--r--   0 michael   (1000) michael   (1000)     1317 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.543743 myokit-1.35.2/myokit/tests/data/formats/sbml/
--rw-r--r--   0 michael   (1000) michael   (1000)     8719 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml
--rw-r--r--   0 michael   (1000) michael   (1000)     9801 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml
--rw-r--r--   0 michael   (1000) michael   (1000)    31408 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/sbml/HodgkinHuxley.xml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/sbml/LICENSE
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.543743 myokit-1.35.2/myokit/tests/data/formats/sbml/model/
--rw-r--r--   0 michael   (1000) michael   (1000)     2149 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml
--rw-r--r--   0 michael   (1000) michael   (1000)     2952 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml
--rw-r--r--   0 michael   (1000) michael   (1000)     1226 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.543743 myokit-1.35.2/myokit/tests/data/formats/sbml/result/
--rw-r--r--   0 michael   (1000) michael   (1000)     2457 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/sbml/result/00001-results.csv
--rw-r--r--   0 michael   (1000) michael   (1000)     2206 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/sbml/result/00004-results.csv
--rw-r--r--   0 michael   (1000) michael   (1000)     1131 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/sbml/result/01103-results.csv
--rw-r--r--   0 michael   (1000) michael   (1000)    25600 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/formats/wcp-file.wcp
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.552743 myokit-1.35.2/myokit/tests/data/io/
--rw-r--r--   0 michael   (1000) michael   (1000)      735 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad1d-1-not-enough-files.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   109429 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad1d-2-no-header.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   104768 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad1d-3-no-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad1d-4-not-a-zip.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   109458 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad1d-5-bad-data-type.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1549 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad1d-6-time-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1584 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad1d-7-0d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad1d-8-1d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)      739 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad2d-1-not-enough-files.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   346240 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad2d-2-no-header.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   333091 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad2d-3-no-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad2d-4-not-a-zip.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   346257 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad2d-5-bad-data-type.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1553 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad2d-6-time-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1588 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad2d-7-0d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/bad2d-8-2d-too-short.zip
--rw-r--r--   0 michael   (1000) michael   (1000)      623 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/badlog-1-no-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1281 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/badlog-2-no-structure.zip
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/badlog-3-not-a-zip.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/badlog-4-invalid-n-fields.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/badlog-5-invalid-data-size.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1457 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/badlog-6-bad-data-type.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/badlog-7-not-enough-data.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     6031 2023-06-07 13:48:59.000000 myokit-1.35.2/myokit/tests/data/io/block2d.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/block2d.zip
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-1-empty.csv
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-10-just-spaces.csv
--rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-11-just-a-semicolon.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-12-bad-header.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-13-header-with-empty-1.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-14-header-with-empty-2.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-15-header-with-empty-3.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-16-wrong-columns-in-data.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-17-non-float-data.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      112 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-2-windows.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      103 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-3-old-mac.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-4-empty-lines.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-5-semicolons.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      119 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-6-open-string.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-7-empty-lines-2.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      100 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-8-unquoted-header.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      114 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog-9-double-quoted-header.csv
--rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/datalog.csv
--rw-r--r--   0 michael   (1000) michael   (1000)     1421 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/io/goodlog.zip
--rw-r--r--   0 michael   (1000) michael   (1000)     4992 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/lr-1991-dep.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     2315 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/lr-1991-fitting.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     4571 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/lr-1991-testing.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     6124 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/lr-1991.mmt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.553743 myokit-1.35.2/myokit/tests/data/multi/
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/multi/beeler-1977-protocol.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/multi/beeler-1977-script.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/multi/beeler-no-name.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     6013 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/multi/lr-1991.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/multi/not-a-model.csv
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.553743 myokit-1.35.2/myokit/tests/data/multi/subdir/
--rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/multi/subdir/beeler-no-name.mmt
--rw-r--r--   0 michael   (1000) michael   (1000)     3754 2023-06-07 13:48:23.000000 myokit-1.35.2/myokit/tests/data/noble-1962.mmt
--rwxr-xr-x   0 michael   (1000) michael   (1000)    22536 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_aux.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    56981 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_cellml_v1_api.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    41869 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_cellml_v1_parser.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    12532 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_cellml_v1_writer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    73319 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_cellml_v2_api.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    26345 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_cellml_v2_parser.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10977 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_cellml_v2_writer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4058 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_cmodel.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      476 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_compiler_detection.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    14096 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_component.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    11511 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_config.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    52565 2023-07-18 23:19:29.000000 myokit-1.35.2/myokit/tests/test_datablock.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    82855 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/tests/test_datalog.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    60654 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_dependency_checking.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)   138508 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_expressions.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4882 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_float.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4236 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_formats.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    32603 2023-07-13 10:36:29.000000 myokit-1.35.2/myokit/tests/test_formats_axon.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    19078 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_formats_cellml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     6703 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_formats_channelml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    11358 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_formats_easyml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     9169 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_formats_exporters.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    40800 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_formats_expression_writers.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3539 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_formats_html.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1531 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_formats_importers.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    37444 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_formats_mathml_content.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8726 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_formats_mathml_presentation.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    17298 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_formats_opencl.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4672 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_formats_sbml.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10324 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_formats_sympy.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     7658 2023-07-13 10:36:31.000000 myokit-1.35.2/myokit/tests/test_formats_wcp.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    14334 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_io.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1821 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_jacobian_calculator.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1767 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_jacobian_tracer.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     7476 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_lib_deps.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    42333 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_lib_guess.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    31014 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_lib_hh.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    39983 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_lib_markov.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5145 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_lib_multi.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     6062 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_lib_plots.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2829 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_meta.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    84972 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_model.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    16720 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_model_building.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3834 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_opencl_info.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8193 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_pacing_factory.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     6504 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/tests/test_pacing_system_c.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3637 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/tests/test_pacing_system_py.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    50865 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_parsing.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2762 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_progress_reporters.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    15092 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_protocol.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    12565 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_protocol_floating_point.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2318 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_protocol_time_series.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2402 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_pype.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     7353 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_quantity.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3452 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_rhs_benchmarker.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    71633 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_sbml_api.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    54542 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_sbml_parser.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    19281 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/tests/test_simulation_1d.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    44343 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/tests/test_simulation_cvodes.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1853 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_simulation_cvodes_from_disk.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    36596 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/tests/test_simulation_fiber_tissue.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    14033 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_simulation_log_interval.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    60162 2023-07-11 14:14:16.000000 myokit-1.35.2/myokit/tests/test_simulation_opencl.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3005 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_simulation_opencl_log_interval.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    20114 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_simulation_opencl_vs_cvode.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5216 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_simulation_opencl_vs_sim1d.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      562 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_system_info.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10358 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_tools.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    13635 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_unit.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1721 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_user_functions.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    33331 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tests/test_variable.py
--rw-r--r--   0 michael   (1000) michael   (1000)    16868 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/tools.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8503 2023-06-25 10:52:15.000000 myokit-1.35.2/myokit/units.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-19 11:02:37.497743 myokit-1.35.2/myokit.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)     5059 2023-07-19 11:02:37.000000 myokit-1.35.2/myokit.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)    15109 2023-07-19 11:02:37.000000 myokit-1.35.2/myokit.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-07-19 11:02:37.000000 myokit-1.35.2/myokit.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       48 2023-07-19 11:02:37.000000 myokit-1.35.2/myokit.egg-info/entry_points.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-01-04 14:18:38.000000 myokit-1.35.2/myokit.egg-info/not-zip-safe
--rw-rw-r--   0 michael   (1000) michael   (1000)      176 2023-07-19 11:02:37.000000 myokit-1.35.2/myokit.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        7 2023-07-19 11:02:37.000000 myokit-1.35.2/myokit.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-07-19 11:02:37.554743 myokit-1.35.2/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     3183 2023-06-25 10:52:15.000000 myokit-1.35.2/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.690508 myokit-1.35.3/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1833 2023-07-11 14:14:16.000000 myokit-1.35.3/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      221 2023-06-07 13:48:23.000000 myokit-1.35.3/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     5059 2023-07-26 21:00:29.690508 myokit-1.35.3/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     3821 2023-06-25 10:52:15.000000 myokit-1.35.3/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.646508 myokit-1.35.3/myokit/
+-rw-r--r--   0 michael   (1000) michael   (1000)    14132 2023-07-26 10:23:11.000000 myokit-1.35.3/myokit/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    57971 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23743 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_aux.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.647508 myokit-1.35.3/myokit/_bin/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6226 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_bin/example.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.654508 myokit-1.35.3/myokit/_bin/gui/
+-rw-r--r--   0 michael   (1000) michael   (1000)      784 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/find.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    96412 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-128.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     3528 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-16.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-24.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   233500 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-256.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    12232 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-32.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    23817 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-48.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    36761 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-64.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    65257 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-96.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)    30396 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer.png
+-rw-r--r--   0 michael   (1000) michael   (1000)    47406 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-ide-128.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     2987 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-ide-16.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     4971 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-ide-24.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   152751 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-ide-256.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     7355 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-ide-32.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)     9835 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-ide-48.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    16235 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-ide-64.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)    30683 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-ide-96.xpm
+-rw-r--r--   0 michael   (1000) michael   (1000)   143766 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-ide.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)    15096 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/icon-ide.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      571 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/new.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      544 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/open.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/redo.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/run.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      565 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/save.png
+-rw-r--r--   0 michael   (1000) michael   (1000)      284 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/_bin/gui/undo.png
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.655508 myokit-1.35.3/myokit/_bin/install-lin/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      254 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/_bin/install-lin/myokit-datablock-viewer.desktop
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      266 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/_bin/install-lin/myokit-datalog-viewer.desktop
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      264 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/install-lin/myokit-ide.desktop
+-rw-r--r--   0 michael   (1000) michael   (1000)     4338 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/_bin/install-lin/myokit.lang
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-06-07 13:47:50.000000 myokit-1.35.3/myokit/_bin/install-lin/x-abf.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      246 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/install-lin/x-cellml.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      247 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/_bin/install-lin/x-myokit.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      275 2023-06-07 13:47:50.000000 myokit-1.35.3/myokit/_bin/install-lin/x-wcp.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.655508 myokit-1.35.3/myokit/_bin/install-win/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1025 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_bin/install-win/menu.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.655508 myokit-1.35.3/myokit/_bin/sundials-win-vs/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1758 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/LICENSE
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.643508 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.656508 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/cvodes/
+-rw-r--r--   0 michael   (1000) michael   (1000)    27506 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     2427 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    12344 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.656508 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/nvector/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8934 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.658508 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5785 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     8997 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    13330 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     1024 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    10283 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     9385 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5420 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     9190 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    12559 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5165 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     1266 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.658508 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sunlinsol/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2983 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.658508 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sunmatrix/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3647 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.661508 myokit-1.35.3/myokit/_bin/sundials-win-vs/lib/
+-rw-r--r--   0 michael   (1000) michael   (1000)   677888 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll
+-rw-r--r--   0 michael   (1000) michael   (1000)   169196 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib
+-rw-r--r--   0 michael   (1000) michael   (1000)   160768 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll
+-rw-r--r--   0 michael   (1000) michael   (1000)    59576 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib
+-rw-r--r--   0 michael   (1000) michael   (1000)    11987 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/_config.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    89061 2023-07-18 23:19:29.000000 myokit-1.35.3/myokit/_datablock.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    75844 2023-07-26 20:57:13.000000 myokit-1.35.3/myokit/_datalog.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11060 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_err.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   103962 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_expressions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8948 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_io.py
+-rw-r--r--   0 michael   (1000) michael   (1000)   193516 2023-07-26 10:23:11.000000 myokit-1.35.3/myokit/_model_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      726 2023-07-26 20:58:33.000000 myokit-1.35.3/myokit/_myokit_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    74065 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_parsing.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4410 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_progress.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    30595 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/_protocol.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.663508 myokit-1.35.3/myokit/_sim/
+-rw-r--r--   0 michael   (1000) michael   (1000)    13412 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_sim/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    19156 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/_sim/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    18908 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/_sim/cable.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    38785 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/_sim/cmodel.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    15775 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_sim/cmodel.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4047 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_sim/compiler.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     2664 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_sim/compiler.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    72435 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/_sim/cvodessim.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    43186 2023-07-18 22:48:59.000000 myokit-1.35.3/myokit/_sim/cvodessim.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15446 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_sim/differential.hpp
+-rw-r--r--   0 michael   (1000) michael   (1000)    47444 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/_sim/fiber_tissue.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    50792 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/_sim/fiber_tissue.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8012 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_sim/jacobian.cpp
+-rw-r--r--   0 michael   (1000) michael   (1000)    12957 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_sim/jacobian.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    32352 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_sim/mcl.h
+-rw-r--r--   0 michael   (1000) michael   (1000)     5037 2023-06-25 10:43:52.000000 myokit-1.35.3/myokit/_sim/opencl.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    16446 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_sim/opencl.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46541 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/_sim/openclsim.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    19360 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_sim/openclsim.cl
+-rw-r--r--   0 michael   (1000) michael   (1000)    69159 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/_sim/openclsim.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29888 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/_sim/pacing.h
+-rw-r--r--   0 michael   (1000) michael   (1000)    10914 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_sim/rhs.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     7392 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_sim/rhs.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1720 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/_sim/sundials.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     2972 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_sim/sundials.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4602 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/_system.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29849 2023-07-12 17:16:09.000000 myokit-1.35.3/myokit/_unit.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3066 2023-07-14 13:14:46.000000 myokit-1.35.3/myokit/float.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.663508 myokit-1.35.3/myokit/formats/
+-rw-r--r--   0 michael   (1000) michael   (1000)    26714 2023-07-14 10:16:32.000000 myokit-1.35.3/myokit/formats/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.663508 myokit-1.35.3/myokit/formats/ansic/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3347 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/ansic/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3566 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/ansic/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5361 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/ansic/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.664508 myokit-1.35.3/myokit/formats/ansic/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11965 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/ansic/template/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     6044 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/ansic/template/euler.c
+-rw-r--r--   0 michael   (1000) michael   (1000)    14244 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/ansic/template/sim.c
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.664508 myokit-1.35.3/myokit/formats/axon/
+-rw-r--r--   0 michael   (1000) michael   (1000)      538 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/axon/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    75937 2023-07-26 10:23:11.000000 myokit-1.35.3/myokit/formats/axon/_abf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    10543 2023-07-12 17:16:09.000000 myokit-1.35.3/myokit/formats/axon/_atf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      826 2023-07-12 17:16:09.000000 myokit-1.35.3/myokit/formats/axon/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.664508 myokit-1.35.3/myokit/formats/cellml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1466 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cellml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2719 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cellml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2283 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cellml/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2229 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cellml/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.665508 myokit-1.35.3/myokit/formats/cellml/v1/
+-rw-r--r--   0 michael   (1000) michael   (1000)      608 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cellml/v1/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59011 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cellml/v1/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    43554 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cellml/v1/_parser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15055 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cellml/v1/_writer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.665508 myokit-1.35.3/myokit/formats/cellml/v2/
+-rw-r--r--   0 michael   (1000) michael   (1000)      598 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cellml/v2/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59012 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cellml/v2/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29536 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cellml/v2/_parser.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11994 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cellml/v2/_writer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.665508 myokit-1.35.3/myokit/formats/channelml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      443 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/channelml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    14605 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/channelml/_importer.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.665508 myokit-1.35.3/myokit/formats/cpp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      526 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cpp/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      421 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cpp/_ewriter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.666508 myokit-1.35.3/myokit/formats/cuda/
+-rw-r--r--   0 michael   (1000) michael   (1000)      816 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cuda/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4472 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cuda/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2059 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cuda/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.666508 myokit-1.35.3/myokit/formats/cuda/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8863 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/cuda/template/kernel.cu
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.666508 myokit-1.35.3/myokit/formats/easyml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      836 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/easyml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3482 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/easyml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15771 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/easyml/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.666508 myokit-1.35.3/myokit/formats/heka/
+-rw-r--r--   0 michael   (1000) michael   (1000)      761 2023-07-14 10:16:32.000000 myokit-1.35.3/myokit/formats/heka/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1154 2023-07-14 10:16:32.000000 myokit-1.35.3/myokit/formats/heka/_importer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    94849 2023-07-26 20:57:13.000000 myokit-1.35.3/myokit/formats/heka/_patchmaster.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.666508 myokit-1.35.3/myokit/formats/html/
+-rw-r--r--   0 michael   (1000) michael   (1000)      457 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/html/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2343 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/html/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6606 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/html/_flatten.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.667508 myokit-1.35.3/myokit/formats/latex/
+-rw-r--r--   0 michael   (1000) michael   (1000)      682 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/latex/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6690 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/latex/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5117 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/latex/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.667508 myokit-1.35.3/myokit/formats/mathml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      637 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/mathml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    12194 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/mathml/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    34289 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/mathml/_parser.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.667508 myokit-1.35.3/myokit/formats/matlab/
+-rw-r--r--   0 michael   (1000) michael   (1000)      695 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/matlab/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3172 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/matlab/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2868 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/matlab/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.667508 myokit-1.35.3/myokit/formats/matlab/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)      528 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/formats/matlab/template/constants.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      374 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/formats/matlab/template/ifthenelse.m
+-rw-r--r--   0 michael   (1000) michael   (1000)     2095 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/matlab/template/main.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      861 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/formats/matlab/template/model.m
+-rw-r--r--   0 michael   (1000) michael   (1000)      461 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/formats/matlab/template/model_wrapper.m
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.668508 myokit-1.35.3/myokit/formats/opencl/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6962 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/opencl/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5261 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/opencl/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3903 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/opencl/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.668508 myokit-1.35.3/myokit/formats/opencl/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11633 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/opencl/template/cable.c
+-rw-r--r--   0 michael   (1000) michael   (1000)     8158 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/opencl/template/kernel.cl
+-rw-r--r--   0 michael   (1000) michael   (1000)     9018 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/opencl/template/minilog.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1042 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/formats/opencl/template/plot.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      162 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/opencl/template/test.sh
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.668508 myokit-1.35.3/myokit/formats/python/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1049 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/python/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6751 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/python/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      969 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/python/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.668508 myokit-1.35.3/myokit/formats/python/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)    10311 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/python/template/sim.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.669508 myokit-1.35.3/myokit/formats/sbml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      653 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/sbml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    59396 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/sbml/_api.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      987 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/sbml/_importer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29181 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/sbml/_parser.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.669508 myokit-1.35.3/myokit/formats/stan/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2877 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/stan/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3102 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/stan/_ewriter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3745 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/stan/_exporter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.669508 myokit-1.35.3/myokit/formats/stan/template/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5305 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/stan/template/cell.stan
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       92 2023-02-05 15:45:10.000000 myokit-1.35.3/myokit/formats/stan/template/run.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.669508 myokit-1.35.3/myokit/formats/sympy/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1638 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/sympy/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6758 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/sympy/_ereader.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4875 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/sympy/_ewriter.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.670508 myokit-1.35.3/myokit/formats/wcp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      254 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/wcp/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    17751 2023-07-26 10:23:11.000000 myokit-1.35.3/myokit/formats/wcp/_wcp.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.670508 myokit-1.35.3/myokit/formats/xml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      445 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/xml/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1494 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/xml/_exporter.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      393 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/formats/xml/_split.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.671508 myokit-1.35.3/myokit/gui/
+-rw-r--r--   0 michael   (1000) michael   (1000)     6154 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/gui/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    49529 2023-07-19 10:57:19.000000 myokit-1.35.3/myokit/gui/datablock_viewer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    32561 2023-07-18 22:48:59.000000 myokit-1.35.3/myokit/gui/datalog_viewer.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8588 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/gui/explorer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)   108238 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/gui/ide.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2157 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/gui/progress.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    52418 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/gui/source.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6072 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/gui/vargrapher.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.671508 myokit-1.35.3/myokit/lib/
+-rw-r--r--   0 michael   (1000) michael   (1000)      216 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/lib/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    23859 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/lib/deps.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    28056 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/lib/guess.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    46678 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/lib/hh.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    67773 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/lib/markov.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4408 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/lib/multi.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    13874 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/lib/plots.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4552 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/pacing.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8230 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/pype.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.677508 myokit-1.35.3/myokit/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)     7752 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2738 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/tests/ansic_event_based_pacing.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1250 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/tests/ansic_time_series_pacing.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.679508 myokit-1.35.3/myokit/tests/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3022 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/tests/data/beeler-1977-model-compare-a.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2889 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/data/beeler-1977-model-compare-b.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3137 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/tests/data/beeler-1977-model.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/beeler-1977-protocol.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/beeler-1977-script.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3287 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/tests/data/beeler-1977-units.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     5091 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/data/clancy-1999-fitting.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3128 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/conditional.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6067 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/tests/data/cv1d.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/cv1d.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)    23916 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/decker-2009.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)    18350 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/decker.model
+-rw-r--r--   0 michael   (1000) michael   (1000)    10416 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/dn-1985-normalised.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      800 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/dom-markov.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.679508 myokit-1.35.3/myokit/tests/data/formats/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8192 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/abf-protocol.pro
+-rw-r--r--   0 michael   (1000) michael   (1000)    98376 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/abf-v1.abf
+-rw-r--r--   0 michael   (1000) michael   (1000)    44544 2023-07-12 17:16:09.000000 myokit-1.35.3/myokit/tests/data/formats/abf-v2.abf
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.680508 myokit-1.35.3/myokit/tests/data/formats/cellml/
+-rw-r--r--   0 michael   (1000) michael   (1000)      188 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/cellml/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)    59093 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/cellml/br-1977-dot.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    58593 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/cellml/br-1977.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)   117223 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/cellml/corrias.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)   221953 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/cellml/decker-2009.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1595 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/cellml/documentation.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/cellml/invalid-file.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    44837 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml
+-rw-r--r--   0 michael   (1000) michael   (1000)    44947 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.682508 myokit-1.35.3/myokit/tests/data/formats/channelml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2648 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      557 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2702 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      549 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2369 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1258 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1539 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1402 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1338 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1290 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1289 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1374 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1373 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)      675 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1398 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1317 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.683508 myokit-1.35.3/myokit/tests/data/formats/sbml/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8719 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     9801 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)    31408 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/sbml/HodgkinHuxley.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/sbml/LICENSE
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.683508 myokit-1.35.3/myokit/tests/data/formats/sbml/model/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2149 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2952 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1226 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.683508 myokit-1.35.3/myokit/tests/data/formats/sbml/result/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2457 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/sbml/result/00001-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     2206 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/sbml/result/00004-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     1131 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/sbml/result/01103-results.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)    25600 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/formats/wcp-file.wcp
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.690508 myokit-1.35.3/myokit/tests/data/io/
+-rw-r--r--   0 michael   (1000) michael   (1000)      735 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad1d-1-not-enough-files.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109429 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad1d-2-no-header.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   104768 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad1d-3-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad1d-4-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109458 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad1d-5-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1549 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad1d-6-time-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1584 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad1d-7-0d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   109483 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad1d-8-1d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)      739 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad2d-1-not-enough-files.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346240 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad2d-2-no-header.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   333091 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad2d-3-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     3026 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad2d-4-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346257 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad2d-5-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1553 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad2d-6-time-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1588 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad2d-7-0d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/bad2d-8-2d-too-short.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)      623 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/badlog-1-no-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1281 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/badlog-2-no-structure.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/badlog-3-not-a-zip.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/badlog-4-invalid-n-fields.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/badlog-5-invalid-data-size.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1457 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/badlog-6-bad-data-type.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     1458 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/badlog-7-not-enough-data.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     6031 2023-06-07 13:48:59.000000 myokit-1.35.3/myokit/tests/data/io/block2d.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)   346276 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/block2d.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-1-empty.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-10-just-spaces.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)        2 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-11-just-a-semicolon.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      104 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-12-bad-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-13-header-with-empty-1.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-14-header-with-empty-2.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      105 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-15-header-with-empty-3.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-16-wrong-columns-in-data.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-17-non-float-data.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      112 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-2-windows.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      103 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-3-old-mac.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      107 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-4-empty-lines.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-5-semicolons.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      119 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-6-open-string.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-7-empty-lines-2.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      100 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-8-unquoted-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      114 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog-9-double-quoted-header.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/datalog.csv
+-rw-r--r--   0 michael   (1000) michael   (1000)     1421 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/io/goodlog.zip
+-rw-r--r--   0 michael   (1000) michael   (1000)     4992 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/lr-1991-dep.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2315 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/lr-1991-fitting.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4571 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/lr-1991-testing.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6136 2023-07-26 10:23:11.000000 myokit-1.35.3/myokit/tests/data/lr-1991.mmt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.690508 myokit-1.35.3/myokit/tests/data/multi/
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/multi/beeler-1977-protocol.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      290 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/multi/beeler-1977-script.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/multi/beeler-no-name.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     6013 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/multi/lr-1991.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)      109 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/multi/not-a-model.csv
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.690508 myokit-1.35.3/myokit/tests/data/multi/subdir/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3008 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/multi/subdir/beeler-no-name.mmt
+-rw-r--r--   0 michael   (1000) michael   (1000)     3754 2023-06-07 13:48:23.000000 myokit-1.35.3/myokit/tests/data/noble-1962.mmt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    22536 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_aux.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    56981 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_cellml_v1_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    41869 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_cellml_v1_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    12532 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_cellml_v1_writer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    73319 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_cellml_v2_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    26345 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_cellml_v2_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10977 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_cellml_v2_writer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4058 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_cmodel.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      476 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_compiler_detection.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14096 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_component.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11511 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_config.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    52565 2023-07-18 23:19:29.000000 myokit-1.35.3/myokit/tests/test_datablock.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    91648 2023-07-26 20:57:13.000000 myokit-1.35.3/myokit/tests/test_datalog.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    60654 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_dependency_checking.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)   138508 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_expressions.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4882 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_float.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4236 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_formats.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    32603 2023-07-13 10:36:29.000000 myokit-1.35.3/myokit/tests/test_formats_axon.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    19078 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_formats_cellml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6703 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_formats_channelml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    11358 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_formats_easyml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     9169 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_formats_exporters.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    40800 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_formats_expression_writers.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3539 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_formats_html.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1531 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_formats_importers.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    37444 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_formats_mathml_content.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8726 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_formats_mathml_presentation.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    17298 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_formats_opencl.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4672 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_formats_sbml.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10324 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_formats_sympy.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7658 2023-07-13 10:36:31.000000 myokit-1.35.3/myokit/tests/test_formats_wcp.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14334 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_io.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1821 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_jacobian_calculator.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1767 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_jacobian_tracer.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7476 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_lib_deps.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    42333 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_lib_guess.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    31014 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_lib_hh.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    39983 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_lib_markov.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5145 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_lib_multi.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6062 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_lib_plots.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2829 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_meta.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    84972 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_model.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    16720 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_model_building.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3834 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_opencl_info.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8193 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_pacing_factory.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     6504 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/tests/test_pacing_system_c.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3637 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/tests/test_pacing_system_py.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    50865 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_parsing.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2762 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_progress_reporters.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    15092 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_protocol.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    12565 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_protocol_floating_point.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2318 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_protocol_time_series.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2402 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_pype.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     7353 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_quantity.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3452 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_rhs_benchmarker.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    71633 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_sbml_api.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    54542 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_sbml_parser.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    19281 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/tests/test_simulation_1d.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    44343 2023-07-25 10:53:10.000000 myokit-1.35.3/myokit/tests/test_simulation_cvodes.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1853 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_simulation_cvodes_from_disk.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    36596 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/tests/test_simulation_fiber_tissue.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    14033 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_simulation_log_interval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    60162 2023-07-11 14:14:16.000000 myokit-1.35.3/myokit/tests/test_simulation_opencl.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3005 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_simulation_opencl_log_interval.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    20114 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_simulation_opencl_vs_cvode.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5216 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_simulation_opencl_vs_sim1d.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      562 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_system_info.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10358 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_tools.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    13635 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_unit.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1721 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_user_functions.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    33331 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tests/test_variable.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    16868 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/tools.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8503 2023-06-25 10:52:15.000000 myokit-1.35.3/myokit/units.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-26 21:00:29.647508 myokit-1.35.3/myokit.egg-info/
+-rw-rw-r--   0 michael   (1000) michael   (1000)     5059 2023-07-26 21:00:29.000000 myokit-1.35.3/myokit.egg-info/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)    15109 2023-07-26 21:00:29.000000 myokit-1.35.3/myokit.egg-info/SOURCES.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-07-26 21:00:29.000000 myokit-1.35.3/myokit.egg-info/dependency_links.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)       48 2023-07-26 21:00:29.000000 myokit-1.35.3/myokit.egg-info/entry_points.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        1 2023-01-04 14:18:38.000000 myokit-1.35.3/myokit.egg-info/not-zip-safe
+-rw-rw-r--   0 michael   (1000) michael   (1000)      176 2023-07-26 21:00:29.000000 myokit-1.35.3/myokit.egg-info/requires.txt
+-rw-rw-r--   0 michael   (1000) michael   (1000)        7 2023-07-26 21:00:29.000000 myokit-1.35.3/myokit.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-07-26 21:00:29.691508 myokit-1.35.3/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     3183 2023-06-25 10:52:15.000000 myokit-1.35.3/setup.py
```

### Comparing `myokit-1.35.2/LICENSE.txt` & `myokit-1.35.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/PKG-INFO` & `myokit-1.35.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myokit
-Version: 1.35.2
+Version: 1.35.3
 Summary: A simple interface to cardiac cellular electrophysiology
 Home-page: http://myokit.org
 Author: Michael Clerx
 Author-email: michael@myokit.org
 License: BSD 3-clause license
 Project-URL: Bug Tracker, https://github.com/MichaelClerx/myokit/issues
 Project-URL: Documentation, http://docs.myokit.org
```

### Comparing `myokit-1.35.2/README.md` & `myokit-1.35.3/README.md`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/__init__.py` & `myokit-1.35.3/myokit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,18 +362,22 @@
 
 # Model api
 from ._model_api import ( # noqa
     check_name,
     Component,
     Equation,
     EquationList,
+    MetaDataContainer,
     Model,
     ModelPart,
+    ObjectWithMetaData,
     UserFunction,
     Variable,
+    VarOwner,
+    VarProvider,
 )
 
 # Expressions
 from ._expressions import (  # noqa
     Abs,
     ACos,
     And,
@@ -501,14 +505,15 @@
     ProgressPrinter,
     ProgressReporter,
     Timeout,
 )
 
 # Data logging
 from ._datalog import (     # noqa
+    ColumnMetaData,
     DataLog,
     _dimco,
     LoggedVariableInfo,
     prepare_log,
     split_key,
 )
 from ._datablock import (   # noqa
```

### Comparing `myokit-1.35.2/myokit/__main__.py` & `myokit-1.35.3/myokit/__main__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_aux.py` & `myokit-1.35.3/myokit/_aux.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/example.mmt` & `myokit-1.35.3/myokit/_bin/example.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/find.png` & `myokit-1.35.3/myokit/_bin/gui/find.png`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-128.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-128.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-16.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-16.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-24.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-24.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-256.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-256.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-32.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-32.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-48.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-48.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-64.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-64.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer-96.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer-96.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer.ico` & `myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer.ico`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-datablock-viewer.png` & `myokit-1.35.3/myokit/_bin/gui/icon-datablock-viewer.png`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-ide-128.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-ide-128.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-ide-16.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-ide-16.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-ide-24.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-ide-24.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-ide-256.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-ide-256.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-ide-32.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-ide-32.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-ide-48.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-ide-48.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-ide-64.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-ide-64.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-ide-96.xpm` & `myokit-1.35.3/myokit/_bin/gui/icon-ide-96.xpm`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-ide.ico` & `myokit-1.35.3/myokit/_bin/gui/icon-ide.ico`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/icon-ide.png` & `myokit-1.35.3/myokit/_bin/gui/icon-ide.png`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/new.png` & `myokit-1.35.3/myokit/_bin/gui/new.png`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/open.png` & `myokit-1.35.3/myokit/_bin/gui/open.png`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/gui/save.png` & `myokit-1.35.3/myokit/_bin/gui/save.png`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/install-lin/myokit.lang` & `myokit-1.35.3/myokit/_bin/install-lin/myokit.lang`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/install-win/menu.json` & `myokit-1.35.3/myokit/_bin/install-win/menu.json`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/LICENSE` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/LICENSE`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/cvodes/cvodes.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_direct.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/cvodes/cvodes_ls.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_config.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_export.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_linearsolver.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_matrix.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_nonlinearsolver.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sundials/sundials_version.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sunlinsol/sunlinsol_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/include/sunmatrix/sunmatrix_dense.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.dll`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/lib/sundials_cvodes.lib`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.dll`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib` & `myokit-1.35.3/myokit/_bin/sundials-win-vs/lib/sundials_nvecserial.lib`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_config.py` & `myokit-1.35.3/myokit/_config.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_datablock.py` & `myokit-1.35.3/myokit/_datablock.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_datalog.py` & `myokit-1.35.3/myokit/_datalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #
 # Functions relating to the DataLog class for storing time series data.
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
+import array
+import json
 import os
 import re
 import sys
-import array
 
 import numpy as np
 
 from collections import OrderedDict
 
 import myokit
 
@@ -78,36 +79,57 @@
 
         # Create a clone of d
         e = myokit.DataLog(d)
 
         # Create a DataLog based on a dictionary
         d = myokit.DataLog({'time':[1, 2, 3], 'data':[2, 4, 5]}, time='time')
 
+    A DataLog can contain meta data, consisting of key-value pairs where
+    ``key`` must be a valid myokit name, and ``value`` can be any string. Meta
+    data for the log as a whole is stored in the property ``meta``, which is a
+    :class:`myokit.MetaDataContainer`. Meta data specific to columns in stored
+    in the property ``cmeta``, which is a :class:`ColumnMetaData` object with
+    an entry for every column::
+
+        d = myokit.DataLog()
+        d.meta['datetime'] = '2023-07-21 15:57'
+        d['data'] = [1, 2, 3]
+        d.cmeta['data']['units'] = 'pA'
+
     Arguments:
 
     ``other``
         A DataLog to clone or a dictionary to use as basis.
     ``time``
         The log key to use for the time variable. When cloning a log, adding
         the ``time`` argument will overwrite the cloned value.
 
     """
 
     def __init__(self, other=None, time=None):
         if other is None:
-            # Create new
             super().__init__()
             self._time = None
+            self.meta = myokit.MetaDataContainer()
+            self.cmeta = ColumnMetaData()
+        elif isinstance(other, DataLog):
+            super().__init__()
+            for k, v in other.items():
+                # Don't use the overwritten setitem, which calls _add
+                super().__setitem__(k, v)
+            self._time = other._time
+            self.meta = myokit.MetaDataContainer(other.meta)
+            self.cmeta = ColumnMetaData(other.cmeta)
         else:
-            # Clone
-            super().__init__(other)
-            try:
-                self._time = str(other._time)
-            except Exception:
-                self._time = None
+            self._time = None
+            self.meta = myokit.MetaDataContainer()
+            self.cmeta = ColumnMetaData()
+            super().__init__(other)  # Let dict do the conversion
+
+        # Set time key, allow overruling when cloning
         if time is not None:
             self.set_time_key(time)
 
     def apd(self, v='membrane.V', threshold=-70):
         """
         Calculates one or more Action Potential Durations (APDs) in a single
         cell's membrane potential.
@@ -189,35 +211,47 @@
         """
         return myokit.DataBlock2d.from_log(self)
 
     def clone(self, numpy=False):
         """
         Returns a deep clone of this log.
 
-        All lists in the log will be duplicated, but the list contents are
+        All arrays in the log will be copied, but the array contents are
         assumed to be numerical (and thereby immutable) and won't be cloned.
 
-        A log with numpy arrays instead of lists can be created by setting
+        A log with numpy arrays instead of arrays can be created by setting
         ``numpy=True``.
         """
+        # Copy data
         log = DataLog()
-        log._time = self._time
         if numpy:
             for k, v in self.items():
                 log[str(k)] = np.array(v, copy=True, dtype=float)
         else:
+            typecode = 'd'
+            for v in self.values():
+                if isinstance(v, array.array):
+                    typecode = v.typecode
+                break
             for k, v in self.items():
-                log[str(k)] = list(v)
+                log[str(k)] = array.array(typecode, v)
+
+        # Copy meta data
+        log._time = self._time
+        log.meta = myokit.MetaDataContainer(self.meta)
+        log.cmeta = ColumnMetaData(self.cmeta)
         return log
 
     def __contains__(self, key):
         return super().__contains__(self._parse_key(key))
 
     def __delitem__(self, key):
-        return super().__delitem__(self._parse_key(key))
+        key = self._parse_key(key)
+        super().__delitem__(key)
+        self.cmeta._remove(key)
 
     def extend(self, other):
         """
         Returns a copy of this log, extended with the data of another.
 
         Both logs must have the same keys and the same time key. The added data
         must be from later time points than in the log being extended.
@@ -525,17 +559,27 @@
                 body = f.getinfo('data.bin')
             except KeyError:
                 raise myokit.DataLogReadError('Invalid log file format.')
             try:
                 head = f.getinfo('structure.txt')
             except KeyError:
                 raise myokit.DataLogReadError('Invalid log file format.')
+
             # Read file contents
             head = f.read(head).decode(ENC)
             body = f.read(body)
+
+            # Read meta data
+            try:
+                meta = f.getinfo('data.bin-metadata.json')
+            except KeyError:
+                meta = None
+            if meta is not None:
+                meta = f.read(meta)
+
         except zipfile.BadZipfile:
             raise myokit.DataLogReadError('Unable to read log: bad zip file.')
         except zipfile.LargeZipFile:    # pragma: no cover
             raise myokit.DataLogReadError(
                 'Unable to read log: zip file requires zip64 support and this'
                 ' has not been enabled on this system.')
         finally:
@@ -556,26 +600,42 @@
             # Note, this field doesn't have to be present in the log!
             log._time = time
         fields = [x for x in head]
         if len(fields) != n:
             raise myokit.DataLogReadError(
                 'Invalid number of fields specified.')
 
+        # Read meta data, if any
+        # Do this before big data conversion operation below, so that we can
+        # fail early.
+        if meta:
+            # Add temporary entries for every field
+            for field in fields:
+                log[field] = tuple()
+
+            # Read meta data
+            try:
+                meta = json.loads(meta)
+            except json.JSONDecodeError as e:   # pragma: no cover
+                raise myokit.DataLogReadError(
+                    'Invalid meta data JSON file: {e}.')
+            DataLog._load_meta_json(meta, log)
+
         # Get size of each entry on disk
         if data_size < 0:
             raise myokit.DataLogReadError(
                 'Invalid data size: ' + str(data_size) + '.')
         try:
             data_size *= dsize[data_type]
         except KeyError:
             raise myokit.DataLogReadError(
                 'Invalid data type: "' + data_type + '".')
 
         # Parse read data
-        fraction = 1.0 / len(fields)
+        fraction = 1 / len(fields)
         start, end = 0, 0
         nbody = len(body)
         try:
             if progress:
                 progress.enter(msg)
             for k, field in enumerate(fields):
                 if progress and not progress.update(k * fraction):
@@ -773,22 +833,90 @@
                 if np.all(y > 0):
                     log.set_time_key(key)
                     break
 
             # Return log
             return log
 
+    @staticmethod
+    def _load_meta_json(meta, log):
+        """
+        Takes a JSON object, attempts to obtain meta data from it and adds it
+        to the given ``log``.
+        """
+        # Check context
+        context = meta.get('@context', None)
+        if context != 'http://www.w3.org/ns/csvw':
+            raise myokit.DataLogReadError(
+                f'Invalid meta data file context: "{context}"')
+
+        # TODO: Check URL? Allow multiple schemas? Alternative syntax?
+
+        # Easier errors
+        def read(parent, key, value_type, parent_str=None):
+            try:
+                value = parent[key]
+            except KeyError:
+                p = '' if parent_str is None else f' inside "{parent_str}"'
+                raise myokit.DataLogReadError(
+                    f'Invalid meta data file: missing "{key}"{p}.')
+            if type(value) != value_type:
+                raise myokit.DataLogReadError(
+                    f'Invalid meta data file: expecting {key} of type'
+                    f' {value_type}, found {type(value)}.')
+            return value
+
+        # Search for Myokit key value pairs
+        def myokit_pairs(parent, container):
+            for key, value in parent.items():
+                if key.startswith('myokit:'):
+                    if type(value) is not str:
+                        raise myokit.DataLogReadError(
+                            'Invalid meta data file: All fields starting with'
+                            ' "myokit:" must have string values, found'
+                            f' {type(value)} for "{key}".')
+                    container[key[7:]] = value
+
+        # Get table schema, read column meta data
+        schema = read(meta, 'tableSchema', dict)
+        columns = read(schema, 'columns', list, 'tableSchema')
+        names = []
+        for column in columns:
+            # Check column exists, get cmeta
+            name = read(column, 'titles', str, 'column')
+            names.append(name)
+            try:
+                cmeta = log.cmeta[name]
+            except KeyError:
+                raise myokit.DataLogReadError(
+                    f'Invalid meta data file: unknown column: "{name}"')
+
+            # Read column meta data
+            myokit_pairs(column, cmeta)
+
+        # Check all columns were listed
+        if len(names) < len(log):
+            raise myokit.DataLogReadError(
+                'Incomplete meta data file: expected table schema with'
+                f' {len(log)} columns, but found {len(names)}.')
+
+        # Read global meta data
+        myokit_pairs(meta, log.meta)
+
     def npview(self):
         """
         Returns a ``DataLog`` with numpy array views of this log's data.
         """
+        # Create log, copy time key
         log = DataLog()
-        log._time = self._time
         for k, v in self.items():
             log[k] = np.asarray(v)
+        log._time = self._time
+        log.meta = myokit.MetaDataContainer(self.meta)
+        log.cmeta = ColumnMetaData(self.cmeta)
         return log
 
     def _parse_key(self, key):
         """
         Parses a key used for __getitem__, __setitem__, __delitem__ and
         __contains__.
         """
@@ -934,34 +1062,39 @@
             ar = array.array(dtype, v)
             if sys.byteorder == 'big':  # pragma: no cover
                 ar.byteswap()
             body_str.append(ar.tobytes())
         head_str = '\n'.join(head_str)
         body_str = b''.join(body_str)
 
-        # 2018-07-15: Wondering why I chose body-head-readme ordering now...
+        # Get meta data json, or None
+        meta_json = self._save_meta_json('data.bin')
 
         # Write
         head = zipfile.ZipInfo('structure.txt')
         head.compress_type = zipfile.ZIP_DEFLATED
         body = zipfile.ZipInfo('data.bin')
         body.compress_type = zipfile.ZIP_DEFLATED
-        read = zipfile.ZipInfo('readme.txt')
-        read.compress_type = zipfile.ZIP_DEFLATED
+        readme = zipfile.ZipInfo('readme.txt')
+        readme.compress_type = zipfile.ZIP_DEFLATED
+        meta = zipfile.ZipInfo('data.bin-metadata.json')
+        meta.compress_type = zipfile.ZIP_DEFLATED
         with zipfile.ZipFile(filename, 'w') as f:
             f.writestr(body, body_str)
             f.writestr(head, head_str.encode(enc))
-            f.writestr(read, README_SAVE_BIN.encode(enc))
+            f.writestr(readme, README_SAVE_BIN.encode(enc))
+            if meta_json is not None:
+                f.writestr(meta, json.dumps(meta_json, indent=2).encode(enc))
 
     def save_csv(
             self, filename, precision=myokit.DOUBLE_PRECISION, order=None,
-            delimiter=',', header=True):
+            delimiter=',', header=True, meta=False):
         """
         Writes this ``DataLog`` to a CSV file, following the syntax
-        outlined in RFC 4180 and with a header indicating the field names.
+        outlined in RFC 4180, and with a header indicating the field names.
 
         The resulting file will consist of:
 
           - A header line containing the names of all logged variables,
             separated by commas. If present, the time variable will be the
             first entry on the line. The remaining keys are ordered using a
             natural sort order.
@@ -988,14 +1121,17 @@
             spaces set ``delimiter=' '``, for tabs: ``delimiter='\\t'``. Note
             that some delimiters (for example '\\n' or '1234') will produce an
             unreadable or invalid csv file.
         ``header``
             Set this to ``False`` to avoid adding a header to the file. Note
             that Myokit will no longer be able to read the written csv file
             without this header.
+        ``meta``
+            Set this to ``True`` to store any meta data in a csv-on-the-web
+            JSON file named ``filename + '-metadata.json'``.
 
         *A note about locale settings*: On Windows systems with a locale
         setting that uses the comma as a decimal separator, importing CSV files
         into Microsoft Excel can be troublesome. To correctly import a CSV,
         either (1) Change your locale settings to use "." as a decimal
         separator or (2) Use the import wizard under Data > Get External Data
         to manually specify the correct separator and delimiter.
@@ -1044,19 +1180,14 @@
                 for key, dat in sorted(
                         self.items(),
                         key=lambda i: myokit.tools.natural_sort_key(i[0])):
                     if key != self._time:
                         keys.append(key)
                         data.append(dat)
 
-            # Number of entries
-            m = len(keys)
-            if m == 0:
-                return
-
             # Get length of entries
             n = self.length()
 
             # Write header
             if header:
                 line = []
                 for key in keys:
@@ -1068,23 +1199,64 @@
             data = [iter(x) for x in data]
             for i in range(0, n):
                 line = []
                 for d in data:
                     line.append(fmat(next(d)))
                 f.write((delimiter.join(line) + eol).encode('ascii'))
 
+        # Write meta data file
+        if meta:
+            meta_json = self._save_meta_json(filename)
+            if meta_json:
+                with open(f'{filename}-metadata.json', 'w') as f:
+                    json.dump(meta_json, f, indent=2)
+
+    def _save_meta_json(self, data_file_path):
+        """
+        Creates an object that can be passed to ``json.dump``, containing the
+        meta data for this DataLog and referencing the data file
+        ``data_file_path``.
+
+        If there is no meta data in the log, ``None`` is returned.
+        """
+        if len(self.meta) == 0:
+            if (len(x) == 0 for x in self.cmeta.values()):
+                return None
+
+        meta = {}
+        meta['@context'] = 'http://www.w3.org/ns/csvw'
+        meta['url'] = os.path.basename(data_file_path)
+
+        # Add table schema and column meta data
+        columns = []
+        for key, cmeta in self.cmeta.items():
+            column = {'titles': key, 'datatype': 'double'}
+            for k, v in cmeta.items():
+                column[f'myokit:{k}'] = v
+            columns.append(column)
+        meta['tableSchema'] = {'columns': columns}
+
+        # Add data log meta data
+        for k, v in self.meta.items():
+            meta[f'myokit:{k}'] = v
+
+        return meta
+
     def set_time_key(self, key):
         """
         Sets the key under which the time data is stored.
         """
         self._time = None if key is None else str(key)
 
     def __setitem__(self, key, value):
-        return super().__setitem__(
-            self._parse_key(key), value)
+        n = len(self)
+        key = self._parse_key(key)
+        super().__setitem__(key, value)
+        if len(self) > n:
+            self.cmeta._add(key)
 
     def split(self, value):
         """
         Splits the log into a part before and after the time ``value``::
 
             s = myokit.Simulation(m, p)
             d = s.run(1000)
@@ -1526,14 +1698,47 @@
         out.append('  dimension: ' + str(self._dimension))
         out.append('  size: ' + ', '.join([str(x) for x in self._size]))
         out.append('  keys:')
         out.extend(['    ' + x for x in self._keys])
         return '\n'.join(out)
 
 
+class ColumnMetaData(dict):
+    """
+    Contains meta data for each column in a :class:`DataLog`.
+
+    This class is managed by a :class:`DataLog`, which will ensure that it
+    contains a :class:`MetaDataContainer` for each column in the data log.
+    """
+    def __init__(self, other=None):
+        super().__init__()
+
+        if isinstance(other, ColumnMetaData):
+            s = super()
+            for key, value in other.items():
+                s.__setitem__(key, myokit.MetaDataContainer(value))
+        elif other is not None:
+            raise ValueError(
+                'Argument `other` must be a ColumnMetaData or None.')
+
+    def __delitem__(self, key):
+        raise ValueError(
+            'Entries in column meta data should be managed by a DataLog')
+
+    def __setitem__(self, key, value):
+        raise ValueError(
+            'Entries in column meta data should be managed by a DataLog')
+
+    def _add(self, key):
+        super().__setitem__(key, myokit.MetaDataContainer())
+
+    def _remove(self, key):
+        super().__delitem__(key)
+
+
 def prepare_log(
         log, model, dims=None, global_vars=None, if_empty=myokit.LOG_NONE,
         allowed_classes=myokit.LOG_ALL, precision=myokit.DOUBLE_PRECISION):
     """
     Returns a :class:`DataLog` for simulation classes based on a ``log``
     argument passed in by the user. The model the simulations will be based on
     should be passed in as ``model``.
@@ -1617,39 +1822,43 @@
         global_vars = []
     else:
         for var in global_vars:
             try:
                 v = model.get(var)
             except KeyError:
                 raise ValueError(
-                    'Unknown variable specified in global_vars <'
-                    + str(var) + '>.')
+                    f'Unknown variable specified in global_vars <{var}>.')
             if v.is_state():
                 raise ValueError('State cannot be global variable.')
 
     # Function to check if variable is allowed (doesn't handle derivatives)
     def check_if_allowed_class(var):
         if var.is_constant():
             raise ValueError(
-                'This log does not support constants, got <'
-                + str(var) + '>.')
+                f'This log does not support constants, got <{var}>.')
         elif var.is_state():
             if not myokit.LOG_STATE & allowed_classes:
                 raise ValueError(
-                    'This log does not support state variables, got <'
-                    + str(var) + '>.')
+                    f'This log does not support state variables, got <{var}>.')
         elif var.is_bound():
             if not myokit.LOG_BOUND & allowed_classes:
                 raise ValueError(
-                    'This log does not support bound variables, got <'
-                    + str(var) + '>.')
+                    f'This log does not support bound variables, got <{var}>.')
         elif not myokit.LOG_INTER & allowed_classes:
-            raise ValueError(
-                'This log does not support intermediary variables, got <'
-                + str(var) + '>.')
+            raise ValueError('This log does not support intermediary'
+                             f' variables, got <{var}>.')
+
+    # Function to add meta data about variables
+    def add_meta(log, key, var, time_unit=None):
+        m = log.cmeta[key]
+        u = var.unit()
+        if u is not None:
+            if time_unit is not None:
+                u = u / time_unit
+            m['unit'] = str(u)
 
     #
     # First option, no log argument given, use the "if_empty" option
     #
 
     if log is None:
         # Check if if_empty matches allowed_classes
@@ -1670,80 +1879,93 @@
 
         # Log argument given as flag
         flag = log
         log = myokit.DataLog()
         if flag == myokit.LOG_ALL:
             flag = allowed_classes
 
+        # Time variable and unit
+        time = model.time()
+        time_unit = time.unit()
+
         if myokit.LOG_STATE & flag:
 
             # Check if allowed
             if not (myokit.LOG_STATE & allowed_classes):
                 raise ValueError('This log does not support state variables.')
 
             # Add states
             for s in model.states():
                 name = s.qname()
                 for c in dcombos:
-                    log[c + name] = array.array(typecode)
+                    key = c + name
+                    log[key] = array.array(typecode)
+                    add_meta(log, key, s)
             flag -= myokit.LOG_STATE
 
         if myokit.LOG_BOUND & flag:
 
             # Check if allowed
             if not (myokit.LOG_BOUND & allowed_classes):
                 raise ValueError('This log does not support bound variables.')
 
             # Add bound variables
             for label, var in model.bindings():
                 name = var.qname()
                 if name in global_vars:
                     log[name] = array.array(typecode)
+                    add_meta(log, name, var)
                 else:
                     for c in dcombos:
-                        log[c + name] = array.array(typecode)
+                        key = c + name
+                        log[key] = array.array(typecode)
+                        add_meta(log, key, var)
             flag -= myokit.LOG_BOUND
 
         if myokit.LOG_INTER & flag:
 
             # Check if allowed
             if not (myokit.LOG_INTER & allowed_classes):
                 raise ValueError(
                     'This log does not support intermediary variables.')
 
             # Add intermediary variables
             for var in model.variables(inter=True, deep=True):
                 name = var.qname()
                 if name in global_vars:
                     log[name] = array.array(typecode)
+                    add_meta(log, name, var)
                 else:
                     for c in dcombos:
-                        log[c + name] = array.array(typecode)
+                        key = c + name
+                        log[key] = array.array(typecode)
+                        add_meta(log, key, var)
             flag -= myokit.LOG_INTER
 
         if myokit.LOG_DERIV & flag:
 
             # Check if allowed
             if not (myokit.LOG_DERIV & allowed_classes):
                 raise ValueError('This log does not support time-derivatives.')
 
             # Add state derivatives
             for var in model.states():
                 name = var.qname()
                 for c in dcombos:
-                    log['dot(' + c + name + ')'] = array.array(typecode)
+                    key = f'dot({c}{name})'
+                    log[key] = array.array(typecode)
+                    add_meta(log, key, var, time_unit)
             flag -= myokit.LOG_DERIV
 
         if flag != 0:
             raise ValueError('One or more unknown flags given as log.')
 
         # Set time variable
-        time = model.time().qname()
-        if time in log:
-            log.set_time_key(time)
+        if time.qname() in log:
+            log.set_time_key(time.qname())
 
         # Return
         return log
 
     #
     # Third option, a dict or DataLog is given. Test if it's suitable for this
     # simulation.
@@ -1777,86 +1999,81 @@
             # Split of index / name
             kdims, kname = split_key(key)
 
             # Test name-key
             try:
                 var = model.get(kname)
             except KeyError:
-                raise ValueError(
-                    'Unknown variable <' + str(kname) + '> in log.')
+                raise ValueError(f'Unknown variable <{kname}> in log.')
 
             # Check if in class of allowed variables
             if deriv:
                 if not myokit.LOG_DERIV & allowed_classes:
                     raise ValueError(
-                        'This log does not support derivatives, got <'
-                        + key + '>.')
+                        f'This log does not support derivatives, got <{key}>.')
                 if not var.is_state():
-                    raise ValueError(
-                        'Cannot log time derivative of non-state <'
-                        + var.qname() + '>.')
+                    raise ValueError('Cannot log time derivative of non-state'
+                                     f' <{var.qname()}>.')
             else:
                 check_if_allowed_class(var)
 
             # Check dimensions
             if kdims:
 
                 # Raise error if global
                 if kname in global_vars:
-                    raise ValueError(
-                        'Cannot specify a cell index for global logging'
-                        ' variable <' + str(kname) + '>.')
+                    raise ValueError('Cannot specify a cell index for global'
+                                     f' logging variable <{kname}>.')
 
                 # Test dim key
                 if kdims not in dcombos:
-                    raise ValueError(
-                        'Invalid index <' + str(kdims) + '> in log.')
+                    raise ValueError(f'Invalid index <{kdims}> in log.')
 
             elif dims:
 
                 # Raise error if non-global variable is used in multi-cell log
                 if kname not in global_vars:
-                    raise ValueError(
-                        'DataLog contains non-indexed entry for'
-                        ' cell-specific variable <' + str(kname) + '>.')
+                    raise ValueError('DataLog contains non-indexed entry for'
+                                     f' cell-specific variable <{kname}>.')
 
         # Check dict values can be appended to
         m = 'append'
         for v in log.values():
             if not (hasattr(v, m) and callable(getattr(v, m))):
-                raise ValueError(
-                    'Logging dict must map qnames to objects'
-                    ' that support the append() method.')
+                raise ValueError('Logging dict must map qnames to objects'
+                                 ' that support the append() method.')
 
         # Return
         return log
 
     #
     # Fourth option, a sequence of variable names, either global or local.
     #
 
     # Check if list interface works
     # If not, then raise exception
     try:
         if len(log) > 0:
             log[0]
     except Exception:
-        raise ValueError(
-            'Argument `log` has unexpected type. Expecting None, integer flag,'
-            ' sequence of names, dict or DataLog.')
+        raise ValueError('Argument `log` has unexpected type. Expecting None,'
+                         ' integer flag, sequence of names, dict or DataLog.')
 
     if isinstance(log, str):
-        raise ValueError(
-            'String passed in as `log` argument, should be list'
-            ' or other sequence containing strings.')
+        raise ValueError('String passed in as `log` argument, should be list'
+                         ' or other sequence containing strings.')
+
+    # Time variable and unit
+    time = model.time()
+    time_unit = time.unit()
 
     # Parse log argument as list
     lst = log
     log = myokit.DataLog()
-    checked_knames = set()
+    checked_knames = {}
     for key in lst:
 
         # Allow variable objects and LhsExpressions
         if isinstance(key, myokit.Variable):
             key = key.qname()
         elif isinstance(key, myokit.LhsExpression):
             key = str(key)
@@ -1866,67 +2083,67 @@
         if deriv:
             key = key[4:-1]
 
         # Split off cell indexes
         kdims, kname = split_key(key)
 
         # Don't re-test multi-dim vars
-        if kname not in checked_knames:
+        try:
+            var = checked_knames[kname]
+        except KeyError:
 
             # Test if name key points to valid variable
             try:
                 var = model.get(kname)
             except KeyError:
-                raise ValueError(
-                    'Unknown variable <' + str(kname) + '> in list.')
+                raise ValueError(f'Unknown variable <{kname}> in list.')
 
             # Check if in class of allowed variables
             if deriv:
                 if not myokit.LOG_DERIV & allowed_classes:
                     raise ValueError(
-                        'This log does not support derivatives, got <'
-                        + key + '>.')
+                        f'This log does not support derivatives, got <{key}>.')
 
                 if not var.is_state():
-                    raise ValueError(
-                        'Cannot log time derivative of non-state <'
-                        + var.qname() + '>.')
+                    raise ValueError('Cannot log time derivative of non-state'
+                                     f' <{var.qname()}>.')
             else:
                 check_if_allowed_class(var)
-            checked_knames.add(kname)
+            checked_knames[kname] = var
 
         # Add key to log
         if kdims:
 
             # Raise error if global
             if kname in global_vars:
-                raise ValueError(
-                    'Cannot specify a cell index for global logging variable'
-                    ' <' + str(kname) + '>.')
+                raise ValueError('Cannot specify a cell index for global'
+                                 f' logging variable <{kname}>.')
 
             # Test dim key
             if kdims not in dcombos:
-                raise ValueError(
-                    'Invalid index <' + str(kdims) + '> in list.')
+                raise ValueError(f'Invalid index <{kdims}> in list.')
 
-            key = kdims + kname if not deriv else 'dot(' + kdims + kname + ')'
+            key = kdims + kname if not deriv else f'dot({kdims}{kname})'
             log[key] = array.array(typecode)
+            add_meta(log, key, var, time_unit if deriv else None)
 
         else:
 
             if kname in global_vars:
-                key = kname if not deriv else 'dot(' + kname + ')'
+                key = kname if not deriv else f'dot({kname})'
                 log[key] = array.array(typecode)
+                add_meta(log, key, var, time_unit if deriv else None)
             else:
                 for c in dcombos:
-                    key = c + kname if not deriv else 'dot(' + c + kname + ')'
+                    key = c + kname if not deriv else f'dot({c}{kname})'
                     log[key] = array.array(typecode)
+                    add_meta(log, key, var, time_unit if deriv else None)
 
     # Set time variable
-    time = model.time().qname()
+    time = time.qname()
     if time in log:
         log.set_time_key(time)
 
     # Return
     return log
 
 
@@ -1975,7 +2192,8 @@
     the original entry.
     """
     m = ID_NAME_PATTERN.match(key, 0)
     if m:
         return key[:m.end()], key[m.end():]
     else:
         return '', key
+
```

### Comparing `myokit-1.35.2/myokit/_err.py` & `myokit-1.35.3/myokit/_err.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_expressions.py` & `myokit-1.35.3/myokit/_expressions.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_io.py` & `myokit-1.35.3/myokit/_io.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_model_api.py` & `myokit-1.35.3/myokit/_model_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,16 +39,25 @@
             'The name <' + str(name) + '> is a reserved keyword.')
 
     return name
 
 
 class MetaDataContainer(dict):
     """
-    Dictionary that stores meta-data.
+    Dictionary that stores string meta-data.
+
+    Each key must be a valid Myokit name (so start with at least one letter,
+    and contain only letters, numbers, and underscores), or a series of valid
+    Myokit names separated by colons (``:``). Values can be any string.
+
+    A MetaDataContainer can be cloned using
+    ``clone = MetaDataContainer(original)``.
     """
+    # Note: Cloning doesn't need to be deep, as keys and values are both
+    # immutable strings.
 
     def __getitem__(self, key):
         # Check key
         if META.match(key) is None:
             raise myokit.InvalidMetaDataNameError(
                 'The key <' + str(key) + '>'
                 ' is not a valid meta-data property identifier.')
@@ -61,15 +70,15 @@
         if META.match(key) is None:
             raise myokit.InvalidMetaDataNameError(
                 'The key <' + str(key) + '>'
                 ' is not a valid meta-data property identifier.')
         super().__setitem__(key, item)
 
 
-class ObjectWithMeta:
+class ObjectWithMetaData:
     """
     Base class for objects with meta data.
 
     Meta-data properties are all stored in a dict and should be string:string
     mappings.
     """
 
@@ -106,15 +115,15 @@
                 for line in v.split(eol):
                     b.write(pre + line + eol)
                 b.write(pre + '"""\n')
             else:
                 b.write(key + v + eol)
 
 
-class ModelPart(ObjectWithMeta):
+class ModelPart(ObjectWithMetaData):
     """
     Base class for model parts.
     """
 
     def __init__(self, parent, name):
         """
         Creates a new ModelPart
@@ -737,15 +746,15 @@
                 raise myokit.UnresolvedReferenceError(name, sa(name))
             try:
                 return comp[vname]
             except KeyError:
                 raise myokit.UnresolvedReferenceError(name, sa(name))
 
 
-class Model(ObjectWithMeta, VarProvider):
+class Model(ObjectWithMetaData, VarProvider):
     """
     Represents an electrophysiological cell model, structured in components.
 
     Components can be added to the model using :meth:`add_component()`. Access
     to a model's component is provided through the :meth:`get()` method and
     :meth:`components()`.
```

### Comparing `myokit-1.35.2/myokit/_myokit_version.py` & `myokit-1.35.3/myokit/_myokit_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Version as a tuple (major, minor, revision)
 #  - Changes to major are rare
 #  - Changes to minor indicate new features, possible slight backwards
 #    incompatibility
 #  - Changes to revision indicate bugfixes, tiny new features
 #  - There is no significance to odd/even numbers
-__version_tuple__ = 1, 35, 2
+__version_tuple__ = 1, 35, 3
 
 # String version of the version number
 __version__ = '.'.join([str(x) for x in __version_tuple__])
 if not __release__:  # pragma: no cover
     __version_tuple__ += ('dev', )
     __version__ += '.dev'
```

### Comparing `myokit-1.35.2/myokit/_parsing.py` & `myokit-1.35.3/myokit/_parsing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_progress.py` & `myokit-1.35.3/myokit/_progress.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_protocol.py` & `myokit-1.35.3/myokit/_protocol.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/__init__.py` & `myokit-1.35.3/myokit/_sim/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/cable.c` & `myokit-1.35.3/myokit/_sim/cable.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/cable.py` & `myokit-1.35.3/myokit/_sim/cable.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/cmodel.h` & `myokit-1.35.3/myokit/_sim/cmodel.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/cmodel.py` & `myokit-1.35.3/myokit/_sim/cmodel.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/compiler.c` & `myokit-1.35.3/myokit/_sim/compiler.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/compiler.py` & `myokit-1.35.3/myokit/_sim/compiler.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/cvodessim.c` & `myokit-1.35.3/myokit/_sim/cvodessim.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/cvodessim.py` & `myokit-1.35.3/myokit/_sim/cvodessim.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/differential.hpp` & `myokit-1.35.3/myokit/_sim/differential.hpp`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/fiber_tissue.c` & `myokit-1.35.3/myokit/_sim/fiber_tissue.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/fiber_tissue.py` & `myokit-1.35.3/myokit/_sim/fiber_tissue.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/jacobian.cpp` & `myokit-1.35.3/myokit/_sim/jacobian.cpp`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/jacobian.py` & `myokit-1.35.3/myokit/_sim/jacobian.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/mcl.h` & `myokit-1.35.3/myokit/_sim/mcl.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/opencl.c` & `myokit-1.35.3/myokit/_sim/opencl.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/opencl.py` & `myokit-1.35.3/myokit/_sim/opencl.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/openclsim.c` & `myokit-1.35.3/myokit/_sim/openclsim.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/openclsim.cl` & `myokit-1.35.3/myokit/_sim/openclsim.cl`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/openclsim.py` & `myokit-1.35.3/myokit/_sim/openclsim.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/pacing.h` & `myokit-1.35.3/myokit/_sim/pacing.h`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/rhs.c` & `myokit-1.35.3/myokit/_sim/rhs.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/rhs.py` & `myokit-1.35.3/myokit/_sim/rhs.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/sundials.c` & `myokit-1.35.3/myokit/_sim/sundials.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_sim/sundials.py` & `myokit-1.35.3/myokit/_sim/sundials.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_system.py` & `myokit-1.35.3/myokit/_system.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/_unit.py` & `myokit-1.35.3/myokit/_unit.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/float.py` & `myokit-1.35.3/myokit/float.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/__init__.py` & `myokit-1.35.3/myokit/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/ansic/__init__.py` & `myokit-1.35.3/myokit/formats/ansic/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/ansic/_ewriter.py` & `myokit-1.35.3/myokit/formats/ansic/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/ansic/_exporter.py` & `myokit-1.35.3/myokit/formats/ansic/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/ansic/template/cable.c` & `myokit-1.35.3/myokit/formats/ansic/template/cable.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/ansic/template/euler.c` & `myokit-1.35.3/myokit/formats/ansic/template/euler.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/ansic/template/sim.c` & `myokit-1.35.3/myokit/formats/ansic/template/sim.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/axon/__init__.py` & `myokit-1.35.3/myokit/formats/axon/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/axon/_abf.py` & `myokit-1.35.3/myokit/formats/axon/_abf.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,18 @@
 
     - Protocol (D/A) conversion is only supported for "episodic stimulation"
       with constant valued steps (so e.g. no ramps) and without "user lists".
     - Protocols with more than one sampling rate are not supported.
     - The publicly available information on the ABF format is not great, so
       there will be several other issues and shortcomings.
 
+    When an :class:`AbfFile` is created, the file at ``filepath`` is read in
+    its entirety and the file handle is closed. No try-catch or ``with``
+    statements are required.
+
     Arguments:
 
     ``filepath``
         The path to load the data from. Data will be read into memory
         immediately upon construction.
     ``is_protocol_file``
         If set to ``True``, no attempt to read A/D data will be made and only
@@ -883,14 +887,15 @@
             # Create and populate sweep
             sweep = self._sweeps[i_sweep]
             for i in range(self._n_adc):
                 c = Channel(self)
                 c._data = part[:, i]    # Actually store the data
                 c._rate = rate
                 c._start = start
+                c._is_reconstruction = False
 
                 if self._version < 2:
                     j = h['nADCSamplingSeq'][i]
 
                     c._name = h['sADCChannelName'][j]
                     c._index = int(h['nADCPtoLChannelMap'][j])
                     c._unit = self._unit(h['sADCUnits'][j])
@@ -971,14 +976,15 @@
                     c._index = i_dac
                 else:
                     c._index = int(dinfo(i_dac, 'lDACChannelNameIndex'))
                 c._data = np.ones(ns) * dinfo(i_dac, 'fDACHoldingLevel')
                 c._rate = self._rate
                 c._start = start
                 c._unit = self._unit(dinfo(i_dac, 'sDACChannelUnits'))
+                c._is_reconstruction = True
 
                 # Find start of first epoch. This is defined as being at t=0
                 # but axon likes to add some samples before the first and after
                 # the last epoch. We can find out the number of samples using
                 # a procedure found in ABF v1's _GetHoldingLength()
                 if self._is_protocol_file:
                     i2 = 0
@@ -1208,28 +1214,60 @@
             nc = self._n_adc + (self._n_dac if include_da else 0)
             names = [c.name() for c in self._sweeps[0][:nc]]
         else:
             names = [f'{i}.channel' for i in range(self._n_adc)]
             if include_da:
                 names += [f'{i}.da' for i in range(self._n_dac)]
 
-        # Gather data and return
+        # Channel meta data adding function
+        def add_channel_meta(channel, cmeta):
+            if channel._is_reconstruction:
+                cmeta['channel_type'] = 'Reconstructed D/A signal'
+                cmeta['original_name'] = channel._name
+                cmeta['original_index'] = channel._index
+                cmeta['unit'] = channel._unit
+                if channel._type:  # pragma: no cover
+                    cmeta['DAC type'] = type_mode_names[channel._type]
+            else:
+                cmeta['channel_type'] = 'Recorded signal'
+                cmeta['original_name'] = channel._name
+                cmeta['original_index'] = channel._index
+                cmeta['unit'] = channel._unit
+                if channel._lopass:
+                    cmeta['low_pass_Hz'] = channel._lopass
+                if channel._cm:
+                    cmeta['Cm_pF'] = channel._cm
+                if channel._rs:   # pragma: no cover
+                    cmeta['Rs'] = channel._rs
+
+        # Gather data
         t = self._sweeps[0][0].times()
         if not join_sweeps:
             log['time'] = t
+            log.cmeta['time']['unit'] = myokit.units.s
             for i_sweep, sweep in enumerate(self._sweeps):
                 for channel, name in zip(sweep, names):
-                    log[name, i_sweep] = channel.values()
+                    name = f'{i_sweep}.{name}'
+                    log[name] = channel.values()
+                    add_channel_meta(channel, log.cmeta[name])
         else:
             log['time'] = np.concatenate(
                 [t + i * self._sweep_start_to_start for i in range(ns)])
+            log.cmeta['time']['unit'] = myokit.units.s
             for i_channel, name in enumerate(names):
                 log[name] = np.concatenate(
                     [sweep[i_channel].values() for sweep in self._sweeps])
+                add_channel_meta(self._sweeps[0][i_channel], log.cmeta[name])
+
+        # Add meta data
         log.set_time_key('time')
+        log.meta['original_format'] = f'ABF {self._version_str}'
+        log.meta['recording_time'] = self._datetime
+        log.meta['acquisition_mode'] = acquisition_modes[self._mode]
+
         return log
 
     def matplotlib_figure(self):
         """ Creates and returns a matplotlib figure with this file's data. """
         import matplotlib.pyplot as plt
         f = plt.figure()
         plt.suptitle(self.filename())
@@ -1290,33 +1328,30 @@
 
         # Channel info
         if len(self._sweeps) > 0:
 
             # A/D recordings
             for i, c in enumerate(self._sweeps[0][:self._n_adc]):
                 out.append(f'A/D Channel {i}: "{c._name}"')
-                if c._type:  # pragma: no cover
-                    # Cover pragma: Don't have appropriate test file
-                    out.append(f'  Type: {type_mode_names[c._type]}')
                 out.append(f'  Unit: {c._unit}')
                 if c._lopass:
                     out.append(f'  Low-pass filter: {c._lopass} Hz')
                 if c._cm:
                     out.append(f'  Cm (telegraphed): {c._cm} pF')
                 if c._rs:   # pragma: no cover
                     # Cover pragma: Don't have appropriate test file
                     out.append(f'  Rs (telegraphed): {c._rs}')
 
             # Reconstructed D/A outputs
             for i, c in enumerate(self._sweeps[0][self._n_adc:]):
                 out.append(f'D/A Channel {i}: "{c._name}"')
+                out.append(f'  Unit: {c._unit}')
                 if c._type:  # pragma: no cover
                     # Cover pragma: Don't have appropriate test file
                     out.append('  Type: {type_mode_names[c._type]}')
-                out.append(f'  Unit: {c._unit}')
 
         # Add full header info
         if show_header:
             if self._strings:
                 dict_to_string(out, 'Strings', {'strings': self._strings})
             dict_to_string(out, 'file header', self._header)
 
@@ -1377,14 +1412,17 @@
     def __init__(self, parent_file):
         self._parent_file = parent_file  # The abf file this channel is from
         self._type = TYPE_UNKNOWN   # Type of recording
 
         # This channel's name
         self._name = None
 
+        # Is this a reconstructed D/A output?
+        self._is_reconstruction = None
+
         # This channel's index in the file. This is basically a name, and does
         # not correspond to e.g. its index in the ADC/DAC info or its index in
         # the sweep's list of channels.
         self._index = None
 
         # The units this channel's data is in
         self._unit = None
```

### Comparing `myokit-1.35.2/myokit/formats/axon/_atf.py` & `myokit-1.35.3/myokit/formats/axon/_atf.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/axon/_importer.py` & `myokit-1.35.3/myokit/formats/axon/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cellml/__init__.py` & `myokit-1.35.3/myokit/formats/cellml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cellml/_ewriter.py` & `myokit-1.35.3/myokit/formats/cellml/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cellml/_exporter.py` & `myokit-1.35.3/myokit/formats/cellml/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cellml/_importer.py` & `myokit-1.35.3/myokit/formats/cellml/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cellml/v1/__init__.py` & `myokit-1.35.3/myokit/formats/cellml/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cellml/v1/_api.py` & `myokit-1.35.3/myokit/formats/cellml/v1/_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cellml/v1/_parser.py` & `myokit-1.35.3/myokit/formats/cellml/v1/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cellml/v1/_writer.py` & `myokit-1.35.3/myokit/formats/cellml/v1/_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cellml/v2/__init__.py` & `myokit-1.35.3/myokit/formats/cellml/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cellml/v2/_api.py` & `myokit-1.35.3/myokit/formats/cellml/v2/_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cellml/v2/_parser.py` & `myokit-1.35.3/myokit/formats/cellml/v2/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cellml/v2/_writer.py` & `myokit-1.35.3/myokit/formats/cellml/v2/_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/channelml/_importer.py` & `myokit-1.35.3/myokit/formats/channelml/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cpp/__init__.py` & `myokit-1.35.3/myokit/formats/cpp/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cuda/__init__.py` & `myokit-1.35.3/myokit/formats/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cuda/_ewriter.py` & `myokit-1.35.3/myokit/formats/cuda/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cuda/_exporter.py` & `myokit-1.35.3/myokit/formats/cuda/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/cuda/template/kernel.cu` & `myokit-1.35.3/myokit/formats/cuda/template/kernel.cu`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/easyml/__init__.py` & `myokit-1.35.3/myokit/formats/easyml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/easyml/_ewriter.py` & `myokit-1.35.3/myokit/formats/easyml/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/easyml/_exporter.py` & `myokit-1.35.3/myokit/formats/easyml/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/heka/__init__.py` & `myokit-1.35.3/myokit/formats/heka/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/heka/_importer.py` & `myokit-1.35.3/myokit/formats/heka/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/heka/_patchmaster.py` & `myokit-1.35.3/myokit/formats/heka/_patchmaster.py`

 * *Files 2% similar despite different names*

```diff
@@ -699,23 +699,29 @@
         """
         Returns this series's :class:`AmplifierState`, containing meta data
         about the recording.
         """
         return self._amplifier_state
 
     def channel(self, channel_id, join_sweeps=False,
-                use_real_start_times=False):
+                use_real_start_times=False, ignore_zero_segment=True):
         """
         Implementation of :meth:`myokit.formats.SweepSource.channel`.
 
         Sweep starts in the Patchmaster format can be derived from the stimulus
         information (the intended start) or from the logged system time at the
         start of each sweep. Ideally these should be the same. By default the
         intended start times are used, but this can be changed to the system
         clock derived times by setting ``use_real_start_times=True``.
+
+        PatchMaster stimuli can specify a segment to use as the "zero segment".
+        Current measured in the latter part of this segment is measured and can
+        then be subtracted from the total signal. By default, this class does
+        not perform this zeroing, but this can be applied by setting
+        ``ignore_zero_segment`` to ``False``.
         """
         # Check channel id
         if isinstance(channel_id, str):
             channel_id = self._channel_names.index(channel_id)
         else:
             self._channel_names[channel_id]  # IndexError/TypeError to user
 
@@ -724,15 +730,15 @@
         if use_real_start_times:
             offset = self._sweep_starts_r
 
         # Gather data and return
         time, data = [], []
         for sweep, offset in zip(self, offsets):
             time.append(offset + sweep[channel_id].times())
-            data.append(sweep[channel_id].values())
+            data.append(sweep[channel_id].values(ignore_zero_segment))
         if join_sweeps:
             return (np.concatenate(time), np.concatenate(data))
         return time, data
 
     def channel_count(self):
         # Docstring in SweepSource
         return len(self._channel_names)
@@ -832,25 +838,31 @@
         return True
 
     def label(self):
         """ Returns this series's label. """
         return self._label
 
     def log(self, join_sweeps=False, use_names=False, include_da=True,
-            use_real_start_times=False):
+            use_real_start_times=False, ignore_zero_segment=True):
         """
         See :meth:`myokit.formats.SweepSource.log`.
 
         A D/A reconstruction will only be included if the stimulus type is
         supported, and if all segments are stored.
 
         Sweep starts in the Patchmaster format can be derived from the stimulus
         information (the intended start) or from the logged system time at the
         start of each sweep. This method uses the intended start times, but
         this can be changed by setting ``use_real_start_times=True``.
+
+        PatchMaster stimuli can specify a segment to use as the "zero segment".
+        Current measured in the latter part of this segment is measured and can
+        then be subtracted from the total signal. By default, this class does
+        not perform this zeroing, but this can be applied by setting
+        ``ignore_zero_segment`` to ``False``.
         """
 
         # Create log
         log = myokit.DataLog()
         ns = len(self)
         if ns == 0:  # pragma: no cover
             return log
@@ -870,32 +882,70 @@
         # Populate log
         if join_sweeps:
             # Join sweeps
             offsets = (self._sweep_starts_r if use_real_start_times
                        else self._sweep_starts_s)
             log['time'] = np.concatenate(
                 [offset + s[0].times() for s, offset in zip(self, offsets)])
+            log.cmeta['time']['unit'] = myokit.units.s
             for c, name in enumerate(channel_names):
                 log[name] = np.concatenate(
-                    [sweep[c].values() for sweep in self])
+                    [sweep[c].values(ignore_zero_segment) for sweep in self])
+                log.cmeta[name]['original_name'] = self._channel_names[c]
+                log.cmeta[name]['unit'] = self._channel_units[c]
             if include_da and len(da_names) == 1:
                 log[da_names[0]] = self.da(join_sweeps=True)[1]
+                log.cmeta[name]['original_name'] = self._da_names[0]
+                log.cmeta[name]['unit'] = self._da_units[0]
 
         else:
             # Individual sweeps
             log['time'] = self[0][0].times()
+            log.cmeta['time']['unit'] = myokit.units.s
             for i, sweep in enumerate(self):
                 for j, name in enumerate(channel_names):
-                    log[name, i] = sweep[j].values()
+                    name = f'{i}.{name}'
+                    log[name] = sweep[j].values(ignore_zero_segment)
+                    log.cmeta[name]['original_name'] = self._channel_names[j]
+                    log.cmeta[name]['unit'] = self._channel_units[j]
             if include_da and len(da_names) == 1:
                 _, vs = self.da(join_sweeps=False)
                 for i, v in enumerate(vs):
-                    log[da_names[0], i] = v
+                    name = f'{i}.{da_names[0]}'
+                    log[name] = v
+                    log.cmeta[name]['original_name'] = self._da_names[0]
+                    log.cmeta[name]['unit'] = self._da_units[0]
 
+        # Add meta data
         log.set_time_key('time')
+        a = self.amplifier_state()
+        log.meta['current_gain_mV_per_pA'] = a.current_gain()
+        log.meta['ljp_correction_mV'] = a.ljp()
+        log.meta['c_slow_compensation_pF'] = a.c_slow()
+        if a.c_fast_enabled():
+            log.meta['c_fast_compensation_enabled'] = 'true'
+            log.meta['c_fast_pF'] = a.c_fast()
+            log.meta['c_fast_tau_micro_s'] = a.c_fast_tau()
+        else:
+            log.meta['c_fast_compensation_enabled'] = 'false'
+        log.meta['r_series_MOhm'] = a.r_series()
+        if a.r_series_enabled():
+            log.meta['r_series_compensation_enabled'] = 'true'
+            log.meta['r_series_compensation_percent'] = round(
+                a.r_series_fraction() * 100, 1)
+        else:
+            log.meta['r_series_compensation_enabled'] = 'false'
+        if len(self) and len(self[0]):
+            t = self[0][0]
+            log.meta['r_pipette_MOhm'] = t.r_pipette()
+            log.meta['r_seal_MOhm'] = t.r_series()
+            log.meta['r_series_post_compensation_MOhm'] = \
+                t.r_series_remaining()
+            log.meta['c_slow_pF'] = t.c_slow()
+
         return log
 
     def meta_str(self, verbose=False):
         # Docstring in SweepSource
         out = []
 
         # Basic info
@@ -919,14 +969,15 @@
             else:
                 out.append(f'Incomplete recording: {len(self)} out of'
                            f' {self._intended_sweep_count} ran.')
 
         # Resistance, capacitance, etc.
         a = self.amplifier_state()
         out.append('Information from amplifier state:')
+        out.append('  Current gain: {a.current_gain()} mV/pA')
         if a.ljp():
             out.append('  LJP correction applied using'
                        f' LJP={round(a.ljp(), 4)} mV.')
         if a.c_fast_enabled():
             out.append(f'  C fast compensation: {a.c_fast()} pF,'
                        f' {round(a.c_fast_tau(), 4)} us.')
         else:
@@ -969,14 +1020,16 @@
             out.append(f'  {stim.sweep_count()} sweeps.')
             out.append(f'  Delay between sweeps: {stim.sweep_interval()} s.')
             out.append(f'  Sampling interval: {stim.sampling_interval()} s.')
             for i, ch in enumerate(stim):
                 out.append(f'  Channel {i}, in {ch.unit()}, amplifier in'
                            f' {ch.amplifier_mode()} mode.')
                 out.append(f'  Stimulus reconstruction: {ch.support_str()}.')
+                z = ch.zero_segment() or '0 (disabled)'
+                out.append(f'  Zero segment: {z}.')
                 for j, seg in enumerate(ch):
                     out.append(f'   Segment {j}, {seg.storage()}')
                     out.append(f'    {seg.segment_class()}, {seg}')
 
         return '\n'.join(out)
 
     def stimulus(self):
@@ -1134,15 +1187,16 @@
 #
 # See also manual 14.1.5 Trace
 #
 class Trace(TreeNode):
     """
     A trace from a :class:`Sweep`.
 
-    Data can be accessed via :meth:`values` (causing it to be read from disk).
+    Data can be accessed via :meth:`values`. Before calling this method, only
+    meta data will be read from disk.
 
     The number of data points can be accessed with :meth:`count_samples()` or
     ``len(trace)`` (this does not require reading anything from disk).
     """
     def __init__(self, parent):
         super().__init__(parent)
 
@@ -1154,14 +1208,15 @@
 
         # Raw data
         self._n = None              # Number of points
         self._data_pos = None       # Data offset (in bytes)
         self._data_type = None      # Data type (struct code)
         self._data_size = None      # Size of a point
         self._data_scale = None     # Scaling from raw to with-unit
+        self._data_zero = None      # Value during "zero segment"
         self._data_interleave_size = None  # 0 or more if interleaved
         self._data_interleave_skip = None  # distance to next block
 
         # Time
         self._t0 = None     # Trace start
         self._dt = None     # Sampling interval
 
@@ -1290,27 +1345,37 @@
         """ Recreates and returns a time vector for this trace. """
         return self._t0 + np.arange(self._n) * self._dt
 
     def time_unit(self):
         """ Returns a string version of the units on the time axis. """
         return myokit.units.s
 
-    def values(self):
-        """ Reads and returns this trace's data. """
+    def values(self, ignore_zero_offset=True):
+        """
+        Reads and returns this trace's data.
+
+        PatchMaster stimuli can specify a segment to use as the "zero segment".
+        Current measured in the latter part of this segment is measured and can
+        then be subtracted from the total signal. By default, this method does
+        not perform this zeroing, but it can be applied by setting
+        ``ignore_zero_segment`` to ``False``.
+        """
 
         if self._data_interleave_size == 0 or self._data_interleave_skip == 0:
             # Read continuous data
             d = np.memmap(self._handle, self._data_type, 'r',
                           offset=self._data_pos, shape=(self._n,))
         else:
             # Read interleaved data
             # points_per_block = self._data_interleave_size / self._data_size
             # n_blocks = np.ceil(self._n / points_per_block)
             raise NotImplementedError('Interleaved data is not supported.')
 
+        if ignore_zero_offset:
+            return d * self._data_scale
         return d * self._data_scale - self._data_zero
 
     def value_unit(self):
         """ Returns a string version of the units on the data axis. """
         return self._data_unit
 
 
@@ -1448,14 +1513,18 @@
     Describes the state of an amplifier used by PatchMaster.
     """
     def __init__(self, handle, reader):
 
         # Read properties
         i = handle.tell()
 
+        # Current gain (V/A)
+        handle.seek(i + 8)      # sCurrentGain = 8;  (* LONGREAL *)
+        self._current_gain = reader.read1('d')
+
         # Series resistance compensation
         handle.seek(i + 40)     # sRsFraction = 40; (* LONGREAL *)
         self._rs_fraction = reader.read1('d')
         handle.seek(i + 240)    # sRsOn = 240; (* BYTE *)
         self._rs_enabled = bool(reader.read1('b'))
 
         handle.seek(i + 88)    # sGSeries = 88; (* LONGREAL *)
@@ -1498,14 +1567,20 @@
 
     def c_slow(self):
         """
         Returns the capacitance (cF) used in slow capacitance correction.
         """
         return self._cs * 1e12
 
+    def current_gain(self):
+        """
+        The gain setting for current measurements, in mV/pA.
+        """
+        return self._current_gain * 1e-9
+
     def ljp(self):
         """
         Returns the liquid junction potential (LJP, in mV) used in the LJP
         correction.
 
         The LJP is defined as the potential of the bath with respect to the
         pipette (V_bath - V_pipette), and so will typically be a positive
@@ -1856,14 +1931,17 @@
 
         # Interpretation of "voltage" in segments
         self._holding = None
         self._use_stim_scale = None
         self._use_relative = None
         self._use_file_template = None
 
+        # Segment used to determine TrZeroData
+        self._zero_segment = None
+
     def _read_properties(self, handle, reader):
         # See TreeNode._read_properties
         start = handle.tell()
 
         handle.seek(start + 25)     # chAmplMode = 25; (* BYTE *)
         self._amplifier_mode = AmplifierMode(reader.read1('b'))
 
@@ -1873,14 +1951,17 @@
 
         handle.seek(start + 76)     # chStimToDacID = 76; (* SET16 *)
         flags = StimulusChannelDACFlags(reader.read('?' * 16))
         self._use_stim_scale = flags.use_stim_scale
         self._use_relative = flags.use_relative
         self._use_file_template = flags.use_file_template
 
+        handle.seek(start + 88)     # chZeroSeg =  88; (* INT32 *)
+        self._zero_segment = reader.read1('i')
+
         # Convert unit
         if self._unit == 'A':
             # It appears that segments stored as 'A' are in nA
             self._unit = myokit.units.nA
         elif self._unit == 'V':
             self._unit = myokit.units.V
         else:
@@ -2071,14 +2152,23 @@
         Note that, unlike :meth:`sweep_durations`, this method takes storage
         into account.
         """
         return np.sum(
             np.array([s.samples(sweep_count, dt) for s in self]),
             axis=0)
 
+    def zero_segment(self):
+        """
+        Returns the index of the segment to use for "zero offset subtraction".
+
+        Counting starts at 1, a zero segment of 0 indicates subtraction is
+        disabled.
+        """
+        return self._zero_segment
+
     def unit(self):
         """ Returns the units that this channel's output is in. """
         return self._unit
 
 
 #
 # From StimFile_v9.txt
```

### Comparing `myokit-1.35.2/myokit/formats/html/_exporter.py` & `myokit-1.35.3/myokit/formats/html/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/html/_flatten.py` & `myokit-1.35.3/myokit/formats/html/_flatten.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/latex/__init__.py` & `myokit-1.35.3/myokit/formats/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/latex/_ewriter.py` & `myokit-1.35.3/myokit/formats/latex/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/latex/_exporter.py` & `myokit-1.35.3/myokit/formats/latex/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/mathml/__init__.py` & `myokit-1.35.3/myokit/formats/mathml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/mathml/_ewriter.py` & `myokit-1.35.3/myokit/formats/mathml/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/mathml/_parser.py` & `myokit-1.35.3/myokit/formats/mathml/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/matlab/__init__.py` & `myokit-1.35.3/myokit/formats/matlab/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/matlab/_ewriter.py` & `myokit-1.35.3/myokit/formats/matlab/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/matlab/_exporter.py` & `myokit-1.35.3/myokit/formats/matlab/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/matlab/template/constants.m` & `myokit-1.35.3/myokit/formats/matlab/template/constants.m`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/matlab/template/main.m` & `myokit-1.35.3/myokit/formats/matlab/template/main.m`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/matlab/template/model.m` & `myokit-1.35.3/myokit/formats/matlab/template/model.m`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/opencl/__init__.py` & `myokit-1.35.3/myokit/formats/opencl/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/opencl/_ewriter.py` & `myokit-1.35.3/myokit/formats/opencl/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/opencl/_exporter.py` & `myokit-1.35.3/myokit/formats/opencl/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/opencl/template/cable.c` & `myokit-1.35.3/myokit/formats/opencl/template/cable.c`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/opencl/template/kernel.cl` & `myokit-1.35.3/myokit/formats/opencl/template/kernel.cl`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/opencl/template/minilog.py` & `myokit-1.35.3/myokit/formats/opencl/template/minilog.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/opencl/template/plot.py` & `myokit-1.35.3/myokit/formats/opencl/template/plot.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/python/__init__.py` & `myokit-1.35.3/myokit/formats/python/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/python/_ewriter.py` & `myokit-1.35.3/myokit/formats/python/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/python/_exporter.py` & `myokit-1.35.3/myokit/formats/python/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/python/template/sim.py` & `myokit-1.35.3/myokit/formats/python/template/sim.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/sbml/__init__.py` & `myokit-1.35.3/myokit/formats/sbml/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/sbml/_api.py` & `myokit-1.35.3/myokit/formats/sbml/_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/sbml/_importer.py` & `myokit-1.35.3/myokit/formats/sbml/_importer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/sbml/_parser.py` & `myokit-1.35.3/myokit/formats/sbml/_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/stan/__init__.py` & `myokit-1.35.3/myokit/formats/stan/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/stan/_ewriter.py` & `myokit-1.35.3/myokit/formats/stan/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/stan/_exporter.py` & `myokit-1.35.3/myokit/formats/stan/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/stan/template/cell.stan` & `myokit-1.35.3/myokit/formats/stan/template/cell.stan`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/sympy/__init__.py` & `myokit-1.35.3/myokit/formats/sympy/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/sympy/_ereader.py` & `myokit-1.35.3/myokit/formats/sympy/_ereader.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/sympy/_ewriter.py` & `myokit-1.35.3/myokit/formats/sympy/_ewriter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/formats/wcp/_wcp.py` & `myokit-1.35.3/myokit/formats/wcp/_wcp.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     WinWCP is a tool for recording electrophysiological data written by John
     Dempster of Strathclyde University. For more information, see
     https://documentation.help/WinWCP-V5.3.8/IDH_Topic750.htm
 
     WinWCP files contain a number of records ``NR``, each containing data from
     ``NC`` channels. Every channel has the same length, ``NP`` samples.
     Sampling happens at a fixed sampling rate.
+
+    When a :class:`WcpFile` is created, the file at ``path`` is read in its
+    entirety and the file handle is closed. No try-catch or ``with`` statements
+    are required.
     """
     def __init__(self, path):
         # The path to the file and its basename
         path = str(path)
         self._path = os.path.abspath(path)
         self._filename = os.path.basename(path)
 
@@ -318,24 +322,33 @@
         if not use_names:
             channel_names = [f'{i}.channel' for i in range(self._nc)]
 
         # Gather data and return
         if join_sweeps:
             log['time'] = np.concatenate(
                 [self._time + h['rtime'] for h in self._record_headers])
+            log.cmeta['time']['unit'] = self._time_unit
             for c, name in enumerate(channel_names):
                 log[name] = np.concatenate([r[c] for r in self._records])
+                log.cmeta[name]['unit'] = self._channel_units[c]
         else:
             # Return individual sweeps
             log['time'] = self._time
+            log.cmeta['time']['unit'] = self._time_unit
             for r, record in enumerate(self._records):
                 for c, name in enumerate(channel_names):
-                    log[name, r] = record[c]
+                    name = f'{r}.{name}'
+                    log[name] = record[c]
+                    log.cmeta[name]['unit'] = self._channel_units[c]
 
+        # Add meta data
         log.set_time_key('time')
+        log.meta['original_format'] = f'WinWCP {self._version_str}'
+        log.meta['recording_time'] = self._header['rtime']
+
         return log
 
     def matplotlib_figure(self):
         """ Creates and returns a matplotlib figure with this file's data. """
         import matplotlib.pyplot as plt
         f = plt.figure()
         axes = [f.add_subplot(self._nc, 1, 1 + i) for i in range(self._nc)]
```

### Comparing `myokit-1.35.2/myokit/formats/xml/_exporter.py` & `myokit-1.35.3/myokit/formats/xml/_exporter.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/gui/__init__.py` & `myokit-1.35.3/myokit/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/gui/datablock_viewer.py` & `myokit-1.35.3/myokit/gui/datablock_viewer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/gui/datalog_viewer.py` & `myokit-1.35.3/myokit/gui/datalog_viewer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/gui/explorer.py` & `myokit-1.35.3/myokit/gui/explorer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/gui/ide.py` & `myokit-1.35.3/myokit/gui/ide.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/gui/progress.py` & `myokit-1.35.3/myokit/gui/progress.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/gui/source.py` & `myokit-1.35.3/myokit/gui/source.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/gui/vargrapher.py` & `myokit-1.35.3/myokit/gui/vargrapher.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/lib/deps.py` & `myokit-1.35.3/myokit/lib/deps.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/lib/guess.py` & `myokit-1.35.3/myokit/lib/guess.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/lib/hh.py` & `myokit-1.35.3/myokit/lib/hh.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/lib/markov.py` & `myokit-1.35.3/myokit/lib/markov.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/lib/multi.py` & `myokit-1.35.3/myokit/lib/multi.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/lib/plots.py` & `myokit-1.35.3/myokit/lib/plots.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/pacing.py` & `myokit-1.35.3/myokit/pacing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/pype.py` & `myokit-1.35.3/myokit/pype.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/__init__.py` & `myokit-1.35.3/myokit/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/ansic_event_based_pacing.py` & `myokit-1.35.3/myokit/tests/ansic_event_based_pacing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/ansic_time_series_pacing.py` & `myokit-1.35.3/myokit/tests/ansic_time_series_pacing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/beeler-1977-model-compare-a.mmt` & `myokit-1.35.3/myokit/tests/data/beeler-1977-model-compare-a.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/beeler-1977-model-compare-b.mmt` & `myokit-1.35.3/myokit/tests/data/beeler-1977-model-compare-b.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/beeler-1977-model.mmt` & `myokit-1.35.3/myokit/tests/data/beeler-1977-model.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/beeler-1977-units.mmt` & `myokit-1.35.3/myokit/tests/data/beeler-1977-units.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/clancy-1999-fitting.mmt` & `myokit-1.35.3/myokit/tests/data/clancy-1999-fitting.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/conditional.mmt` & `myokit-1.35.3/myokit/tests/data/conditional.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/cv1d.mmt` & `myokit-1.35.3/myokit/tests/data/cv1d.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/cv1d.zip` & `myokit-1.35.3/myokit/tests/data/cv1d.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/decker-2009.mmt` & `myokit-1.35.3/myokit/tests/data/decker-2009.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/decker.model` & `myokit-1.35.3/myokit/tests/data/decker.model`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/dn-1985-normalised.mmt` & `myokit-1.35.3/myokit/tests/data/dn-1985-normalised.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/dom-markov.mmt` & `myokit-1.35.3/myokit/tests/data/dom-markov.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/abf-protocol.pro` & `myokit-1.35.3/myokit/tests/data/formats/abf-protocol.pro`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/abf-v1.abf` & `myokit-1.35.3/myokit/tests/data/formats/abf-v1.abf`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/abf-v2.abf` & `myokit-1.35.3/myokit/tests/data/formats/abf-v2.abf`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/cellml/br-1977-dot.cellml` & `myokit-1.35.3/myokit/tests/data/formats/cellml/br-1977-dot.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/cellml/br-1977.cellml` & `myokit-1.35.3/myokit/tests/data/formats/cellml/br-1977.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/cellml/corrias.cellml` & `myokit-1.35.3/myokit/tests/data/formats/cellml/corrias.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/cellml/decker-2009.cellml` & `myokit-1.35.3/myokit/tests/data/formats/cellml/decker-2009.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/cellml/documentation.cellml` & `myokit-1.35.3/myokit/tests/data/formats/cellml/documentation.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml` & `myokit-1.35.3/myokit/tests/data/formats/cellml/lr-1991-exported-1.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml` & `myokit-1.35.3/myokit/tests/data/formats/cellml/lr-1991-exported-2.cellml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-00-valid-file.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-01-wrong-root.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-02-no-channel-type.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-03-overlapping-name.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-04-no-cvr.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-05-two-cvrs.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-06-no-q10.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-07-three-transitions.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-08-no-closed-to-open.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-09-no-open-to-closed.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-10-tco-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-11-toc-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-12-no-steady-state.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-13-no-time-course.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-14-inf-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-15-tau-bad-expression.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-16-no-gates.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-17-invalid-name.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml` & `myokit-1.35.3/myokit/tests/data/formats/channelml/ch-18-c-style-if.channelml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml` & `myokit-1.35.3/myokit/tests/data/formats/sbml/00004-sbml-l2v1-modified.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml` & `myokit-1.35.3/myokit/tests/data/formats/sbml/00004-sbml-l3v2-modified.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/sbml/HodgkinHuxley.xml` & `myokit-1.35.3/myokit/tests/data/formats/sbml/HodgkinHuxley.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml` & `myokit-1.35.3/myokit/tests/data/formats/sbml/model/00001-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml` & `myokit-1.35.3/myokit/tests/data/formats/sbml/model/00004-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml` & `myokit-1.35.3/myokit/tests/data/formats/sbml/model/01103-sbml-l3v2.xml`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/sbml/result/00001-results.csv` & `myokit-1.35.3/myokit/tests/data/formats/sbml/result/00001-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/sbml/result/00004-results.csv` & `myokit-1.35.3/myokit/tests/data/formats/sbml/result/00004-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/sbml/result/01103-results.csv` & `myokit-1.35.3/myokit/tests/data/formats/sbml/result/01103-results.csv`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/formats/wcp-file.wcp` & `myokit-1.35.3/myokit/tests/data/formats/wcp-file.wcp`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad1d-1-not-enough-files.zip` & `myokit-1.35.3/myokit/tests/data/io/bad1d-1-not-enough-files.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad1d-2-no-header.zip` & `myokit-1.35.3/myokit/tests/data/io/bad1d-2-no-header.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad1d-3-no-data.zip` & `myokit-1.35.3/myokit/tests/data/io/bad1d-3-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad1d-4-not-a-zip.zip` & `myokit-1.35.3/myokit/tests/data/io/bad1d-4-not-a-zip.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad1d-5-bad-data-type.zip` & `myokit-1.35.3/myokit/tests/data/io/bad1d-5-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad1d-6-time-too-short.zip` & `myokit-1.35.3/myokit/tests/data/io/bad1d-6-time-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad1d-7-0d-too-short.zip` & `myokit-1.35.3/myokit/tests/data/io/bad1d-7-0d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad1d-8-1d-too-short.zip` & `myokit-1.35.3/myokit/tests/data/io/bad1d-8-1d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad2d-1-not-enough-files.zip` & `myokit-1.35.3/myokit/tests/data/io/bad2d-1-not-enough-files.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad2d-2-no-header.zip` & `myokit-1.35.3/myokit/tests/data/io/bad2d-2-no-header.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad2d-3-no-data.zip` & `myokit-1.35.3/myokit/tests/data/io/bad2d-3-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad2d-4-not-a-zip.zip` & `myokit-1.35.3/myokit/tests/data/io/bad2d-4-not-a-zip.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad2d-5-bad-data-type.zip` & `myokit-1.35.3/myokit/tests/data/io/bad2d-5-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad2d-6-time-too-short.zip` & `myokit-1.35.3/myokit/tests/data/io/bad2d-6-time-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad2d-7-0d-too-short.zip` & `myokit-1.35.3/myokit/tests/data/io/bad2d-7-0d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/bad2d-8-2d-too-short.zip` & `myokit-1.35.3/myokit/tests/data/io/bad2d-8-2d-too-short.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/badlog-1-no-data.zip` & `myokit-1.35.3/myokit/tests/data/io/badlog-1-no-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/badlog-2-no-structure.zip` & `myokit-1.35.3/myokit/tests/data/io/badlog-2-no-structure.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/badlog-4-invalid-n-fields.zip` & `myokit-1.35.3/myokit/tests/data/io/badlog-4-invalid-n-fields.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/badlog-5-invalid-data-size.zip` & `myokit-1.35.3/myokit/tests/data/io/badlog-5-invalid-data-size.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/badlog-6-bad-data-type.zip` & `myokit-1.35.3/myokit/tests/data/io/badlog-6-bad-data-type.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/badlog-7-not-enough-data.zip` & `myokit-1.35.3/myokit/tests/data/io/badlog-7-not-enough-data.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/block2d.mmt` & `myokit-1.35.3/myokit/tests/data/io/block2d.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/block2d.zip` & `myokit-1.35.3/myokit/tests/data/io/block2d.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/io/goodlog.zip` & `myokit-1.35.3/myokit/tests/data/io/goodlog.zip`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/lr-1991-dep.mmt` & `myokit-1.35.3/myokit/tests/data/lr-1991-dep.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/lr-1991-fitting.mmt` & `myokit-1.35.3/myokit/tests/data/lr-1991-fitting.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/lr-1991-testing.mmt` & `myokit-1.35.3/myokit/tests/data/lr-1991-testing.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/lr-1991.mmt` & `myokit-1.35.3/myokit/tests/data/lr-1991.mmt`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
     desc: Plateau Potassium current
 
 # Slow inward Calcium current
 [ica]
 use membrane.V as V
 dot(Ca_i) =  -1e-4 * ICa + 0.07 * (1e-4 - Ca_i)
     desc: Intracellular Calcium concentration
+    in [mM]
 E = 7.7 - 13.0287 * log(Ca_i / cell.Ca_o)
     desc: Nernst potential
     in [mV]
 dot(d) =  alpha * (1 - d) - beta * d
     alpha = 0.095 * exp(-0.01 * (V - 5)) / (1 + exp(-0.072 * (V - 5)))
     beta  = 0.07 * exp(-0.017 * (V + 44)) / (1 + exp(0.05 * (V + 44)))
 dot(f) =  alpha * (1-f) - beta * f
```

### Comparing `myokit-1.35.2/myokit/tests/data/multi/beeler-no-name.mmt` & `myokit-1.35.3/myokit/tests/data/multi/beeler-no-name.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/multi/lr-1991.mmt` & `myokit-1.35.3/myokit/tests/data/multi/lr-1991.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/multi/subdir/beeler-no-name.mmt` & `myokit-1.35.3/myokit/tests/data/multi/subdir/beeler-no-name.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/data/noble-1962.mmt` & `myokit-1.35.3/myokit/tests/data/noble-1962.mmt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_aux.py` & `myokit-1.35.3/myokit/tests/test_aux.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_cellml_v1_api.py` & `myokit-1.35.3/myokit/tests/test_cellml_v1_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_cellml_v1_parser.py` & `myokit-1.35.3/myokit/tests/test_cellml_v1_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_cellml_v1_writer.py` & `myokit-1.35.3/myokit/tests/test_cellml_v1_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_cellml_v2_api.py` & `myokit-1.35.3/myokit/tests/test_cellml_v2_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_cellml_v2_parser.py` & `myokit-1.35.3/myokit/tests/test_cellml_v2_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_cellml_v2_writer.py` & `myokit-1.35.3/myokit/tests/test_cellml_v2_writer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_cmodel.py` & `myokit-1.35.3/myokit/tests/test_cmodel.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_component.py` & `myokit-1.35.3/myokit/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_config.py` & `myokit-1.35.3/myokit/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_datablock.py` & `myokit-1.35.3/myokit/tests/test_datablock.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_datalog.py` & `myokit-1.35.3/myokit/tests/test_datalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 #
 # Tests the DataLog class
 #
 # This file is part of Myokit.
 # See http://myokit.org for copyright, sharing, and licensing details.
 #
+import array
+import json
 import os
 import unittest
 
 import numpy as np
 
 import myokit
 
@@ -20,19 +22,135 @@
     CancellingReporter,
     WarningCollector,
 )
 
 # Extra output
 debug = False
 
+CSV_META = """
+{
+  "@context": "http://www.w3.org/ns/csvw",
+  "url": "test.csv",
+  "tableSchema": {
+    "columns": [
+      {
+        "titles": "a.b",
+        "datatype": "double"
+      },
+      {
+        "titles": "c.d",
+        "datatype": "double",
+        "myokit:extra": "This is the best column"
+      },
+      {
+        "titles": "e.f",
+        "datatype": "double"
+      }
+    ]
+  },
+  "myokit:test": "A nice sandwich",
+  "myokit:number": "4",
+  "myokit:one:two": "5"
+}
+""".strip()
+
 
 class DataLogTest(unittest.TestCase):
     """
     Tests the DataLog's functions.
     """
+    def test_apd(self):
+        # Test the apd method.
+
+        # Very coarse check
+        d = myokit.DataLog(time='time')
+        d['time'] = np.linspace(0, 10, 11)
+        d['v'] = np.ones(10) * -85
+        d['v'][1:3] = 40
+        d['v'][6:9] = 40
+        apds = d.apd(v='v')
+        self.assertEqual(len(apds), 2)
+        self.assertTrue(apds['start'][0] > 0)
+        self.assertTrue(apds['start'][0] < 1)
+        self.assertTrue(apds['duration'][0] > 2.5)
+        self.assertTrue(apds['duration'][0] < 3.0)
+        self.assertTrue(apds['start'][1] > 5)
+        self.assertTrue(apds['start'][1] < 6)
+        self.assertTrue(apds['duration'][1] > 3.5)
+        self.assertTrue(apds['duration'][1] < 4.0)
+
+        # Check with threshold equal to V
+        apds = d.apd(v='v', threshold=-85)
+        self.assertEqual(len(apds['start']), 1)
+        self.assertEqual(apds['start'][0], 5)
+        self.assertEqual(apds['duration'][0], 4)
+
+        # Check against example model
+        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+        s = myokit.Simulation(m, p)
+        s.set_tolerance(1e-8, 1e-8)
+        d, apds1 = s.run(
+            2000, log=['engine.time', 'membrane.V'],
+            log_interval=0.005,
+            apd_variable='membrane.V', apd_threshold=-70)
+        apds2 = d.apd(threshold=-70)
+        self.assertEqual(len(apds1['start']), 2)
+        self.assertEqual(len(apds2['start']), 2)
+        self.assertAlmostEqual(1, apds1['start'][0] / apds2['start'][0])
+        self.assertAlmostEqual(1, apds1['start'][1] / apds2['start'][1])
+        self.assertAlmostEqual(1, apds1['duration'][0] / apds2['duration'][0])
+        self.assertAlmostEqual(1, apds1['duration'][1] / apds2['duration'][1])
+
+    def test_clone(self):
+        # Test cloning via constructor and clone() method
+
+        # Obtain a log from a simulation
+        m, p, _ = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
+        s = myokit.Simulation(m, p)
+        d1 = s.run(100, log=myokit.LOG_BOUND + myokit.LOG_STATE)
+        d1.meta['yes'] = 'no'
+
+        # Clone via constructor
+        d2 = myokit.DataLog(d1)
+        self.assertEqual(len(d1), len(d2))
+        self.assertEqual(d1.keys(), d2.keys())
+        for v1, v2 in zip(d1.values(), d2.values()):
+            self.assertEqual(v1, v2)
+            self.assertTrue(v1 is v2)   # Constructor clone is not deep!
+            self.assertEqual(type(v2), array.array)
+        self.assertIn('yes', d2.meta)
+        self.assertEqual(d2.meta['yes'], 'no')
+        for k in d2:
+            self.assertIn(k, d2.cmeta)
+        self.assertIn('unit', d2.cmeta['ica.Ca_i'])
+        self.assertEqual(d2.cmeta['ica.Ca_i']['unit'], '[mM]')
+
+        # Clone via clone()
+        d2 = d1.clone()
+        self.assertEqual(len(d1), len(d2))
+        self.assertEqual(d1.keys(), d2.keys())
+        for v1, v2 in zip(d1.values(), d2.values()):
+            self.assertEqual(v1, v2)
+            self.assertFalse(v1 is v2)
+            self.assertEqual(type(v2), array.array)
+        self.assertIn('yes', d2.meta)
+        self.assertEqual(d2.meta['yes'], 'no')
+        self.assertEqual(d2.cmeta['ica.Ca_i']['unit'], '[mM]')
+
+        # Clone via clone(numpy=True)
+        d2 = d1.clone(numpy=True)
+        self.assertEqual(len(d1), len(d2))
+        self.assertEqual(d1.keys(), d2.keys())
+        for v1, v2 in zip(d1.values(), d2.values()):
+            self.assertEqual(list(v1), list(v2))
+            self.assertFalse(v1 is v2)
+            self.assertEqual(type(v2), np.ndarray)
+        self.assertIn('yes', d2.meta)
+        self.assertEqual(d2.meta['yes'], 'no')
+        self.assertEqual(d2.cmeta['ica.Ca_i']['unit'], '[mM]')
 
     def test_extend(self):
         # Test the extend function.
 
         d1 = myokit.DataLog(time='time')
         v1 = [10, 9, 10, -1, -1, -1]
         v2 = [12, 2, 43, 31, 2, 7]
@@ -149,14 +267,57 @@
         self.assertEqual(x.find_after(10), 2)
         self.assertEqual(x.find_after(13), 3)
         self.assertEqual(x.find_after(15), 3)
         self.assertEqual(x.find_after(19), 4)
         self.assertEqual(x.find_after(20), 4)
         self.assertEqual(x.find_after(21), 5)
 
+    def test_fold(self):
+        # Test the fold() method.
+
+        d = myokit.DataLog(time='time')
+        d['time'] = list(range(100))
+        d['x'] = list(np.arange(100) * 3)
+
+        # Test without discarding remainder
+        d2 = d.fold(30, discard_remainder=False)
+        self.assertEqual(set(d2.keys()), set([
+            'time', '0.x', '1.x', '2.x', '3.x']))
+
+        # Test with discarding remainder
+        d = d.npview()
+        d2 = d.fold(30)
+        self.assertEqual(set(d2.keys()), set([
+            'time', '0.x', '1.x', '2.x']))
+        self.assertEqual(len(d2['time']), 30)
+        self.assertEqual(len(d2['0.x']), 30)
+        self.assertEqual(len(d2['1.x']), 30)
+        self.assertEqual(len(d2['2.x']), 30)
+        self.assertTrue(np.all(d2['time'] == d['time'][:30]))
+        self.assertTrue(np.all(d2['0.x'] == d['x'][:30]))
+        self.assertTrue(np.all(d2['1.x'] == d['x'][30:60]))
+        self.assertTrue(np.all(d2['2.x'] == d['x'][60:90]))
+
+    def test_has_nan(self):
+        # Test the has_nan() method, which checks if the _final_ value in any
+        # field is NaN.
+
+        d = myokit.DataLog(time='time')
+        d['time'] = list(range(100))
+        d['x'] = list(np.arange(100) * 3)
+        d['y'] = list(np.arange(100) * 3)
+        d['z'] = list(np.arange(100) * 3)
+        self.assertFalse(d.has_nan())
+        d['x'][-3] = float('nan')
+        self.assertFalse(d.has_nan())
+        d['x'][-1] = float('inf')
+        self.assertFalse(d.has_nan())
+        d['x'][-1] = float('nan')
+        self.assertTrue(d.has_nan())
+
     def test_indexing(self):
         # Test the indexing overrides in the simulation log.
 
         d = myokit.DataLog()
         d['x'] = 'y'
         self.assertEqual(d['x'], 'y')
         d['1.2.membrane.V'] = 'a bear'
@@ -375,14 +536,306 @@
         # 2-d
         e = d.clone()
         e['0.0.m.v'] = e['1.0.m.v'] = e['0.1.m.v'] = e['1.1.m.v'] = v
         self.assertEqual(
             e.keys_like('m.v'),
             ['0.0.m.v', '0.1.m.v', '1.0.m.v', '1.1.m.v'])
 
+    def test_length(self):
+        # Test the length() method, that counts the length of the log's
+        # entries.
+
+        d = myokit.DataLog(time='time')
+        self.assertEqual(d.length(), 0)
+        d['time'] = list(np.arange(100) * 3)
+        self.assertEqual(d.length(), 100)
+        d['x'] = list(np.arange(100) * 3)
+        self.assertEqual(d.length(), 100)
+
+    def test_load_errors(self):
+        # Test if the correct load errors are raised.
+
+        # Missing data file
+        path = os.path.join(DIR_IO, 'badlog-1-no-data.zip')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'log file format', myokit.DataLog.load,
+            path)
+
+        # Missing structure file
+        path = os.path.join(DIR_IO, 'badlog-2-no-structure.zip')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'log file format', myokit.DataLog.load,
+            path)
+
+        # Not a zip
+        path = os.path.join(DIR_IO, 'badlog-3-not-a-zip.zip')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'bad zip file', myokit.DataLog.load, path)
+
+        # Wrong number of fields
+        path = os.path.join(DIR_IO, 'badlog-4-invalid-n-fields.zip')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'number of fields', myokit.DataLog.load,
+            path)
+
+        # Negative data size
+        path = os.path.join(DIR_IO, 'badlog-5-invalid-data-size.zip')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'Invalid data size', myokit.DataLog.load,
+            path)
+
+        # Unknown data type
+        path = os.path.join(DIR_IO, 'badlog-6-bad-data-type.zip')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'Invalid data type', myokit.DataLog.load,
+            path)
+
+        # Not enough data
+        path = os.path.join(DIR_IO, 'badlog-7-not-enough-data.zip')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'larger data', myokit.DataLog.load, path)
+
+    def test_load_meta(self):
+        # Tests error handling in meta data loading.
+
+        # Should really be done by mocking up a zip file instead of testing the
+        # private interface...
+
+        # Create log for which CSV_META is appropriate
+        org = myokit.DataLog()
+        org['a.b'] = [1, 2, 3]
+        org['c.d'] = [4, 5, 6]
+        org['e.f'] = [7, 8, 9]
+
+        # Test loading
+        log = org.clone()
+        meta = json.loads(CSV_META)
+        myokit.DataLog._load_meta_json(meta, log)
+        self.assertIn('test', log.meta)
+        self.assertEqual(log.meta['test'], 'A nice sandwich')
+        self.assertIn('number', log.meta)
+        self.assertEqual(log.meta['number'], '4')
+        self.assertIn('one:two', log.meta)
+        self.assertEqual(log.meta['one:two'], '5')
+        self.assertIn('extra', log.cmeta['c.d'])
+        self.assertEqual(log.cmeta['c.d']['extra'], 'This is the best column')
+
+        # Invalid context (not a csv-on-the-web)
+        meta['@context'] = 'jippie'
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'Invalid meta data file context',
+            myokit.DataLog._load_meta_json, meta, log)
+        del meta['@context']
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'Invalid meta data file context',
+            myokit.DataLog._load_meta_json, meta, log)
+
+        # Missing required key other than context
+        meta = json.loads(CSV_META)
+        del meta['tableSchema']['columns']
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'missing "columns" inside "tableSchema"',
+            myokit.DataLog._load_meta_json, meta, log)
+        del meta['tableSchema']
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'missing "tableSchema"',
+            myokit.DataLog._load_meta_json, meta, log)
+
+        # Wrong type
+        meta['tableSchema'] = [1, 2, 3]
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'expecting tableSchema of type',
+            myokit.DataLog._load_meta_json, meta, log)
+
+        # Non-string value
+        meta = json.loads(CSV_META)
+        meta['myokit:tosti'] = 123
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'starting with "myokit:" must have',
+            myokit.DataLog._load_meta_json, meta, log)
+
+        # Missing column
+        del meta['myokit:tosti']
+        meta['tableSchema']['columns'] = meta['tableSchema']['columns'][1:]
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'expected table schema with 3 columns',
+            myokit.DataLog._load_meta_json, meta, log)
+
+        # Extra column
+        meta = json.loads(CSV_META)
+        meta['tableSchema']['columns'].append(
+            {'titles': 'Bert', 'datatype': 'double'})
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'unknown column: "Bert"',
+            myokit.DataLog._load_meta_json, meta, log)
+
+    def test_load_with_progress(self):
+        # Test loading with a progress reporter.
+
+        p = TestReporter()
+        path = os.path.join(DIR_IO, 'goodlog.zip')
+        self.assertFalse(p.entered)
+        self.assertFalse(p.exited)
+        self.assertFalse(p.updated)
+        d = myokit.DataLog.load(path, progress=p)
+        self.assertTrue(p.entered)
+        self.assertTrue(p.exited)
+        self.assertTrue(p.updated)
+        self.assertEqual(type(d), myokit.DataLog)
+
+        p = CancellingReporter(1)
+        d = myokit.DataLog.load(path, progress=p)
+        self.assertIsNone(d)
+
+    def test_load_csv_errors(self):
+        # Test for errors during csv loading.
+
+        # Test errory file, with comments etc., should work fine!
+        path = os.path.join(DIR_IO, 'datalog.csv')
+        d = myokit.DataLog.load_csv(path).npview()
+        self.assertEqual(set(d.keys()), set(['time', 'v']))
+        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
+        self.assertTrue(np.all(d['v'] == 10 * (1 + np.arange(6))))
+
+        # Empty file
+        path = os.path.join(DIR_IO, 'datalog-1-empty.csv')
+        d = myokit.DataLog.load_csv(path)
+        self.assertEqual(set(d.keys()), set())
+
+        # Test windows line endings
+        path = os.path.join(DIR_IO, 'datalog-2-windows.csv')
+        d = myokit.DataLog.load_csv(path).npview()
+        self.assertEqual(set(d.keys()), set(['time', 'v']))
+        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
+        self.assertTrue(np.all(d['v'] == 10 * (1 + np.arange(6))))
+
+        # Test old mac line endings
+        path = os.path.join(DIR_IO, 'datalog-3-old-mac.csv')
+        d = myokit.DataLog.load_csv(path).npview()
+        self.assertEqual(set(d.keys()), set(['time', 'v']))
+        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
+        self.assertTrue(np.all(d['v'] == 10 * (1 + np.arange(6))))
+
+        # Test empty lines at end
+        path = os.path.join(DIR_IO, 'datalog-4-empty-lines.csv')
+        d = myokit.DataLog.load_csv(path).npview()
+        self.assertEqual(set(d.keys()), set(['time', 'v']))
+        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
+        self.assertTrue(np.all(d['v'] == 10 * (1 + np.arange(6))))
+
+        # Test semicolons at end of each line
+        path = os.path.join(DIR_IO, 'datalog-5-semicolons.csv')
+        d = myokit.DataLog.load_csv(path).npview()
+        self.assertEqual(set(d.keys()), set(['time', 'v']))
+        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
+        self.assertTrue(np.all(d['v'] == 10 * (1 + np.arange(6))))
+
+        # Test unterminated string
+        path = os.path.join(DIR_IO, 'datalog-6-open-string.csv')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'inside quoted', myokit.DataLog.load_csv,
+            path)
+
+        # Test empty lines between data
+        path = os.path.join(DIR_IO, 'datalog-7-empty-lines-2.csv')
+        d = myokit.DataLog.load_csv(path)
+        self.assertEqual(set(d.keys()), set(['time', 'v']))
+        self.assertTrue(np.all(d['time'] == np.arange(1, 7)))
+        self.assertTrue(np.all(d['v'] == 10 * (np.arange(1, 7))))
+
+        # Test unquoted field names
+        path = os.path.join(DIR_IO, 'datalog-8-unquoted-header.csv')
+        d = myokit.DataLog.load_csv(path).npview()
+        self.assertEqual(set(d.keys()), set(['time', 'v']))
+        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
+        self.assertTrue(np.all(d['v'] == 10 * (1 + np.arange(6))))
+
+        # Test double-quoted field names
+        path = os.path.join(DIR_IO, 'datalog-9-double-quoted-header.csv')
+        d = myokit.DataLog.load_csv(path).npview()
+        self.assertEqual(set(d.keys()), set(['time', 'v"quote"']))
+        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
+        self.assertTrue(np.all(d['v"quote"'] == 10 * (1 + np.arange(6))))
+
+        # Test file with just some spaces (one line)
+        path = os.path.join(DIR_IO, 'datalog-10-just-spaces.csv')
+        d = myokit.DataLog.load_csv(path).npview()
+        self.assertEqual(set(d.keys()), set())
+
+        # Test file with just some spaces (one line)
+        path = os.path.join(DIR_IO, 'datalog-11-just-a-semicolon.csv')
+        d = myokit.DataLog.load_csv(path).npview()
+        self.assertEqual(set(d.keys()), set())
+
+        # Test header "abc"x"adc"
+        path = os.path.join(DIR_IO, 'datalog-12-bad-header.csv')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'Expecting double quote',
+            myokit.DataLog.load_csv, path)
+
+        # Test empty field "" in header
+        path = os.path.join(DIR_IO, 'datalog-13-header-with-empty-1.csv')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'Empty field', myokit.DataLog.load_csv,
+            path)
+
+        # Test empty field "x",,"y" in header
+        path = os.path.join(DIR_IO, 'datalog-14-header-with-empty-2.csv')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'Empty field', myokit.DataLog.load_csv,
+            path)
+
+        # Test empty field "time","v", in header
+        path = os.path.join(DIR_IO, 'datalog-15-header-with-empty-3.csv')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'Empty field', myokit.DataLog.load_csv,
+            path)
+
+        # Test wrong field count in data
+        path = os.path.join(DIR_IO, 'datalog-16-wrong-columns-in-data.csv')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'Wrong number of columns',
+            myokit.DataLog.load_csv, path)
+
+        # Test non-float data
+        path = os.path.join(DIR_IO, 'datalog-17-non-float-data.csv')
+        self.assertRaisesRegex(
+            myokit.DataLogReadError, 'Unable to convert',
+            myokit.DataLog.load_csv, path)
+
+    def test_npview(self):
+        # Tests the npview() method
+
+        d = myokit.DataLog()
+        d['tammy'] = [7, 8, 9]
+        d['tommy'] = [4, 5, 6]
+        d['timmy'] = [1, 2, 3]
+        d.set_time_key('timmy')
+        d.meta['best_meta'] = 'super_value'
+        d.cmeta['tammy']['stand:by'] = 'your man'
+
+        e = d.npview()
+        self.assertFalse(d is e)
+        self.assertEqual(len(d), len(e))
+        self.assertIsInstance(d['tammy'], list)
+        self.assertIsInstance(d['tommy'], list)
+        self.assertIsInstance(d['timmy'], list)
+        self.assertIsInstance(e['tammy'], np.ndarray)
+        self.assertIsInstance(e['tommy'], np.ndarray)
+        self.assertIsInstance(e['timmy'], np.ndarray)
+        self.assertEqual(d['tammy'], list(e['tammy']))
+        self.assertEqual(d['tommy'], list(e['tommy']))
+        self.assertEqual(d['timmy'], list(e['timmy']))
+        self.assertEqual(len(d.meta), len(e.meta))
+        self.assertIn('tammy', e.cmeta)
+        self.assertEqual(len(d.cmeta['tammy']), len(e.cmeta['tammy']))
+        self.assertIn('stand:by', e.cmeta['tammy'])
+        self.assertEqual(
+            d.cmeta['tammy']['stand:by'], e.cmeta['tammy']['stand:by'])
+
     def test_prepare_log_0d(self):
         # Test the `prepare_log` method for single-cell simulations.
 
         # Test multi-cell log preparing
         from myokit import prepare_log
         m = myokit.load_model(
             os.path.join(DIR_DATA, 'lr-1991-testing.mmt'))
@@ -1166,20 +1619,54 @@
             ['0.0.engine.time'], m, (2, 1), global_vars=['engine.time'])
 
         # Invalid index for variable in list
         self.assertRaisesRegex(
             ValueError, 'Invalid index', prepare_log, ['3.3.membrane.V'], m,
             (2, 1))
 
+    def test_regularize(self):
+        # Test the deprecated regularize() method.
+
+        d = myokit.DataLog(time='time')
+        d['time'] = np.log(np.linspace(1, 25, 100))
+        d['values'] = np.linspace(1, 25, 100)
+
+        has_scipy = True
+        with WarningCollector() as w:
+            try:
+                e = d.regularize(dt=0.5)
+            except ImportError:
+                has_scipy = False
+        self.assertIn('eprecated', w.text())
+        if not has_scipy:
+            return
+
+        self.assertEqual(len(e['time']), 7)
+        x = np.array([0, 0.5, 1, 1.5, 2, 2.5, 3])
+        self.assertTrue(np.all(e['time'] == x))
+        for i, y in enumerate(x):
+            self.assertTrue(np.abs(np.exp(y) - e['values'][i]) < 0.02)
+
+        # test setting tmin and tmax
+        with WarningCollector() as w:
+            e = d.regularize(dt=0.5, tmin=0.4, tmax=2.6)
+        self.assertEqual(len(e['time']), 5)
+        x = np.array([0.4, 0.9, 1.4, 1.9, 2.4])
+        self.assertTrue(np.all(e['time'] == x))
+        for i, y in enumerate(x):
+            self.assertTrue(np.abs(np.exp(y) - e['values'][i]) < 0.02)
+
     def test_save(self):
         # Test saving in binary format.
 
         d = myokit.DataLog()
         d['a.b'] = np.arange(0, 100, dtype=np.float32)
         d['c.d'] = np.sqrt(np.arange(0, 100) * 1.2)
+        d.meta['one'] = 1
+        d.cmeta['a.b']['two'] = 2
 
         # Test saving with double precision
         with TemporaryDirectory() as td:
             fname = td.path('test.bin')
             d.save(fname)
             e = myokit.DataLog.load(fname)
             self.assertFalse(d is e)
@@ -1194,14 +1681,20 @@
             self.assertTrue(isinstance(d['a.b'][0], np.float32))
             self.assertTrue(isinstance(d['c.d'][0], float))
             self.assertTrue(isinstance(e['a.b'][0], float))
             self.assertTrue(isinstance(e['c.d'][0], float))
             self.assertEqual(e['a.b'].typecode, 'd')
             self.assertEqual(e['c.d'].typecode, 'd')
 
+            # Test that meta data was loaded too
+            self.assertIn('one', e.meta)
+            self.assertEqual(e.meta['one'], '1')
+            self.assertIn('two', e.cmeta['a.b'])
+            self.assertEqual(e.cmeta['a.b']['two'], '2')
+
         # Test saving with single precision
         d = myokit.DataLog()
         d.set_time_key('c.d')
         d['a.b'] = np.arange(0, 100, dtype=np.float32)
         d['c.d'] = np.sqrt(np.arange(0, 100, dtype=np.float32) * 1.2)
         with TemporaryDirectory() as td:
             fname = td.path('test.bin')
@@ -1222,81 +1715,20 @@
             self.assertTrue(isinstance(e['c.d'][0], float))
             self.assertEqual(e['a.b'].typecode, 'f')
             self.assertEqual(e['c.d'].typecode, 'f')
             self.assertEqual(e.time_key(), 'c.d')
             self.assertTrue(np.all(e.time() == d.time()))
             self.assertTrue(np.all(e.time() == d['c.d']))
 
-    def test_load_errors(self):
-        # Test if the correct load errors are raised.
-
-        # Missing data file
-        path = os.path.join(DIR_IO, 'badlog-1-no-data.zip')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'log file format', myokit.DataLog.load,
-            path)
-
-        # Missing structure file
-        path = os.path.join(DIR_IO, 'badlog-2-no-structure.zip')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'log file format', myokit.DataLog.load,
-            path)
-
-        # Not a zip
-        path = os.path.join(DIR_IO, 'badlog-3-not-a-zip.zip')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'bad zip file', myokit.DataLog.load, path)
-
-        # Wrong number of fields
-        path = os.path.join(DIR_IO, 'badlog-4-invalid-n-fields.zip')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'number of fields', myokit.DataLog.load,
-            path)
-
-        # Negative data size
-        path = os.path.join(DIR_IO, 'badlog-5-invalid-data-size.zip')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'Invalid data size', myokit.DataLog.load,
-            path)
-
-        # Unknown data type
-        path = os.path.join(DIR_IO, 'badlog-6-bad-data-type.zip')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'Invalid data type', myokit.DataLog.load,
-            path)
-
-        # Not enough data
-        path = os.path.join(DIR_IO, 'badlog-7-not-enough-data.zip')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'larger data', myokit.DataLog.load, path)
-
-    def test_load_with_progress(self):
-        # Test loading with a progress reporter.
-
-        p = TestReporter()
-        path = os.path.join(DIR_IO, 'goodlog.zip')
-        self.assertFalse(p.entered)
-        self.assertFalse(p.exited)
-        self.assertFalse(p.updated)
-        d = myokit.DataLog.load(path, progress=p)
-        self.assertTrue(p.entered)
-        self.assertTrue(p.exited)
-        self.assertTrue(p.updated)
-        self.assertEqual(type(d), myokit.DataLog)
-
-        p = CancellingReporter(1)
-        d = myokit.DataLog.load(path, progress=p)
-        self.assertIsNone(d)
-
     def test_save_csv(self):
         # Test saving as csv.
 
         d = myokit.DataLog()
 
-        # Note: a.b and e.f are both non-decreaing, could be taken for time!
+        # Note: a.b and e.f are both non-decreasing, could be taken for time!
         d['a.b'] = np.arange(0, 100)
         d['c.d'] = np.sqrt(np.arange(0, 100) * 1.2)
         d['e.f'] = np.arange(0, 100) + 1
         with TemporaryDirectory() as td:
             fname = td.path('test.csv')
             d.save_csv(fname)
             e = myokit.DataLog.load_csv(fname)
@@ -1315,28 +1747,22 @@
         # Now set time key
         d.set_time_key('a.b')
         with TemporaryDirectory() as td:
             fname = td.path('test.csv')
             d.save_csv(fname)
             e = myokit.DataLog.load_csv(fname)
             self.assertEqual(e.time()[0], d['a.b'][0])
-
-        # Now set time key
         d.set_time_key('e.f')
         with TemporaryDirectory() as td:
             fname = td.path('test.csv')
             d.save_csv(fname)
             e = myokit.DataLog.load_csv(fname)
             self.assertEqual(e.time()[0], d['e.f'][0])
 
         # Test saving with single precision
-        d = myokit.DataLog(time='a.b')
-        d['a.b'] = np.arange(0, 100)
-        d['c.d'] = np.sqrt(np.arange(0, 100) * 1.2)
-        d['e.f'] = np.arange(0, 100) + 1
         d = d.npview()
         with TemporaryDirectory() as td:
             fname = td.path('test.csv')
             d.save_csv(fname, precision=myokit.SINGLE_PRECISION)
             e = myokit.DataLog.load_csv(fname).npview()
             self.assertEqual(len(d), len(e))
             self.assertIn('a.b', e)
@@ -1344,18 +1770,14 @@
             self.assertNotIn('a.d', e)
             self.assertEqual(len(d['a.b']), len(e['a.b']))
             self.assertEqual(len(d['c.d']), len(e['c.d']))
             self.assertTrue(np.all(np.abs(d['a.b'] - e['a.b']) < 1e-6))
             self.assertTrue(np.all(np.abs(d['c.d'] - e['c.d']) < 1e-6))
 
         # Test saving with python string formats
-        d = myokit.DataLog(time='a.b')
-        d['a.b'] = np.arange(0, 100)
-        d['c.d'] = np.sqrt(np.arange(0, 100) * 1.2)
-        d['e.f'] = np.arange(0, 100) + 1
         with TemporaryDirectory() as td:
             fname = td.path('test.csv')
             d.save_csv(fname, precision=None)
             e = myokit.DataLog.load_csv(fname)
             self.assertEqual(len(d), len(e))
             self.assertIn('a.b', e)
             self.assertIn('c.d', e)
@@ -1367,18 +1789,14 @@
 
         # Test invalid precision arguments
         with TemporaryDirectory() as td:
             fname = td.path('test.csv')
             self.assertRaises(ValueError, d.save_csv, fname, 'ernie')
 
         # Test saving with a fixed order
-        d = myokit.DataLog(time='a.b')
-        d['a.b'] = np.arange(0, 100)
-        d['c.d'] = np.sqrt(np.arange(0, 100) * 1.2)
-        d['e.f'] = np.arange(0, 100) + 1
         with TemporaryDirectory() as td:
             fname = td.path('test.csv')
             d.save_csv(fname, order=['a.b', 'c.d', 'e.f'])
             with open(fname, 'r', newline=None) as f:
                 header = f.readline()
             self.assertEqual(header, '"a.b","c.d","e.f"\n')
 
@@ -1422,129 +1840,56 @@
         d = myokit.DataLog()
         with TemporaryDirectory() as td:
             fname = td.path('test.csv')
             d.save_csv(fname)
             e = myokit.DataLog.load_csv(fname)
             self.assertEqual(len(e.keys()), 0)
 
-    def test_load_csv_errors(self):
-        # Test for errors during csv loading.
-
-        # Test errory file, with comments etc., should work fine!
-        path = os.path.join(DIR_IO, 'datalog.csv')
-        d = myokit.DataLog.load_csv(path).npview()
-        self.assertEqual(set(d.keys()), set(['time', 'v']))
-        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
-        self.assertTrue(np.all(d['v'] == 10 * (1 + np.arange(6))))
-
-        # Empty file
-        path = os.path.join(DIR_IO, 'datalog-1-empty.csv')
-        d = myokit.DataLog.load_csv(path)
-        self.assertEqual(set(d.keys()), set())
-
-        # Test windows line endings
-        path = os.path.join(DIR_IO, 'datalog-2-windows.csv')
-        d = myokit.DataLog.load_csv(path).npview()
-        self.assertEqual(set(d.keys()), set(['time', 'v']))
-        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
-        self.assertTrue(np.all(d['v'] == 10 * (1 + np.arange(6))))
-
-        # Test old mac line endings
-        path = os.path.join(DIR_IO, 'datalog-3-old-mac.csv')
-        d = myokit.DataLog.load_csv(path).npview()
-        self.assertEqual(set(d.keys()), set(['time', 'v']))
-        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
-        self.assertTrue(np.all(d['v'] == 10 * (1 + np.arange(6))))
-
-        # Test empty lines at end
-        path = os.path.join(DIR_IO, 'datalog-4-empty-lines.csv')
-        d = myokit.DataLog.load_csv(path).npview()
-        self.assertEqual(set(d.keys()), set(['time', 'v']))
-        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
-        self.assertTrue(np.all(d['v'] == 10 * (1 + np.arange(6))))
-
-        # Test semicolons at end of each line
-        path = os.path.join(DIR_IO, 'datalog-5-semicolons.csv')
-        d = myokit.DataLog.load_csv(path).npview()
-        self.assertEqual(set(d.keys()), set(['time', 'v']))
-        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
-        self.assertTrue(np.all(d['v'] == 10 * (1 + np.arange(6))))
-
-        # Test unterminated string
-        path = os.path.join(DIR_IO, 'datalog-6-open-string.csv')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'inside quoted', myokit.DataLog.load_csv,
-            path)
-
-        # Test empty lines between data
-        path = os.path.join(DIR_IO, 'datalog-7-empty-lines-2.csv')
-        d = myokit.DataLog.load_csv(path)
-        self.assertEqual(set(d.keys()), set(['time', 'v']))
-        self.assertTrue(np.all(d['time'] == np.arange(1, 7)))
-        self.assertTrue(np.all(d['v'] == 10 * (np.arange(1, 7))))
-
-        # Test unquoted field names
-        path = os.path.join(DIR_IO, 'datalog-8-unquoted-header.csv')
-        d = myokit.DataLog.load_csv(path).npview()
-        self.assertEqual(set(d.keys()), set(['time', 'v']))
-        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
-        self.assertTrue(np.all(d['v'] == 10 * (1 + np.arange(6))))
-
-        # Test double-quoted field names
-        path = os.path.join(DIR_IO, 'datalog-9-double-quoted-header.csv')
-        d = myokit.DataLog.load_csv(path).npview()
-        self.assertEqual(set(d.keys()), set(['time', 'v"quote"']))
-        self.assertTrue(np.all(d['time'] == (1 + np.arange(6))))
-        self.assertTrue(np.all(d['v"quote"'] == 10 * (1 + np.arange(6))))
-
-        # Test file with just some spaces (one line)
-        path = os.path.join(DIR_IO, 'datalog-10-just-spaces.csv')
-        d = myokit.DataLog.load_csv(path).npview()
-        self.assertEqual(set(d.keys()), set())
-
-        # Test file with just some spaces (one line)
-        path = os.path.join(DIR_IO, 'datalog-11-just-a-semicolon.csv')
-        d = myokit.DataLog.load_csv(path).npview()
-        self.assertEqual(set(d.keys()), set())
-
-        # Test header "abc"x"adc"
-        path = os.path.join(DIR_IO, 'datalog-12-bad-header.csv')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'Expecting double quote',
-            myokit.DataLog.load_csv, path)
-
-        # Test empty field "" in header
-        path = os.path.join(DIR_IO, 'datalog-13-header-with-empty-1.csv')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'Empty field', myokit.DataLog.load_csv,
-            path)
+        # Test saving CSV with meta data
+        d = myokit.DataLog()
+        d.set_time_key('a.b')
+        d['a.b'] = np.arange(0, 100)
+        d['c.d'] = np.sqrt(np.arange(0, 100) * 1.2)
+        d['e.f'] = np.arange(0, 100) + 1
+        d.meta['test'] = 'A nice sandwich'
+        d.meta['number'] = 4
+        d.meta['one:two'] = 5
+        d.cmeta['c.d']['extra'] = 'This is the best column'
 
-        # Test empty field "x",,"y" in header
-        path = os.path.join(DIR_IO, 'datalog-14-header-with-empty-2.csv')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'Empty field', myokit.DataLog.load_csv,
-            path)
+        with TemporaryDirectory() as td:
+            fname = td.path('test.csv')
+            d.save_csv(fname, meta=True)
 
-        # Test empty field "time","v", in header
-        path = os.path.join(DIR_IO, 'datalog-15-header-with-empty-3.csv')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'Empty field', myokit.DataLog.load_csv,
-            path)
+            e = myokit.DataLog.load_csv(fname)
+            self.assertEqual(len(d), len(e))
+            self.assertIn('a.b', e)
+            self.assertIn('c.d', e)
+            self.assertNotIn('a.d', e)
+            self.assertEqual(len(d['a.b']), len(e['a.b']))
+            self.assertEqual(len(d['c.d']), len(e['c.d']))
+            self.assertEqual(list(d['a.b']), list(e['a.b']))
+            self.assertEqual(list(d['c.d']), list(e['c.d']))
 
-        # Test wrong field count in data
-        path = os.path.join(DIR_IO, 'datalog-16-wrong-columns-in-data.csv')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'Wrong number of columns',
-            myokit.DataLog.load_csv, path)
+            self.maxDiff = None
+            meta_path = td.path('test.csv-metadata.json')
+            self.assertTrue(os.path.exists(meta_path))
+            with open(meta_path, 'r') as f:
+                self.assertEqual(f.read(), CSV_META)
+
+        # Test no meta data is written is none is set
+        del d.meta['test']
+        del d.meta['number']
+        del d.meta['one:two']
+        del d.cmeta['c.d']['extra']
 
-        # Test non-float data
-        path = os.path.join(DIR_IO, 'datalog-17-non-float-data.csv')
-        self.assertRaisesRegex(
-            myokit.DataLogReadError, 'Unable to convert',
-            myokit.DataLog.load_csv, path)
+        with TemporaryDirectory() as td:
+            fname = td.path('test.csv')
+            d.save_csv(fname, meta=True)
+            meta_path = td.path('test.csv-metadata.json')
+            self.assertFalse(os.path.exists(meta_path))
 
     def test_split(self):
         # Test the split function.
 
         var1 = 'engine.toom'
         var2 = 'membrane.V'
         x = myokit.DataLog({
@@ -1769,14 +2114,32 @@
 
         # Test larger period than log data
         d['x'] = [4, 5, 6, 7]
         e = d.split_periodic(100)
         self.assertEqual(set(d.keys()), set(e.keys()))
         self.assertFalse(d is e)
 
+    def test_time(self):
+        # Test the time() method.
+
+        d = myokit.DataLog(time='t')
+        t = [1, 2, 3]
+        d['t'] = t
+        self.assertIs(d['t'], t)
+
+        # Test non-existing time key
+        d = myokit.DataLog(time='t')
+        self.assertRaisesRegex(
+            myokit.InvalidDataLogError, 'Invalid key', d.time)
+
+        # Test no time key
+        d = myokit.DataLog()
+        self.assertRaisesRegex(
+            myokit.InvalidDataLogError, 'No time', d.time)
+
     def test_trim(self):
         # Test the trim() method.
 
         d = myokit.DataLog()
         d.set_time_key('t')
         d['t'] = t = [0, 0.1, 0.2, 0.3, 0.4]
         d['a'] = a = [1, 2, 3, 4, 5]
@@ -2040,207 +2403,14 @@
         d['y'] = [4, 5, 6]
         d.validate()
         d['z'] = [7, 8, 9]
         d.validate()
         d['x'].append(1)
         self.assertRaises(myokit.InvalidDataLogError, d.validate)
 
-    def test_apd(self):
-        # Test the apd method.
-
-        # Very coarse check
-        d = myokit.DataLog(time='time')
-        d['time'] = np.linspace(0, 10, 11)
-        d['v'] = np.ones(10) * -85
-        d['v'][1:3] = 40
-        d['v'][6:9] = 40
-        apds = d.apd(v='v')
-        self.assertEqual(len(apds), 2)
-        self.assertTrue(apds['start'][0] > 0)
-        self.assertTrue(apds['start'][0] < 1)
-        self.assertTrue(apds['duration'][0] > 2.5)
-        self.assertTrue(apds['duration'][0] < 3.0)
-        self.assertTrue(apds['start'][1] > 5)
-        self.assertTrue(apds['start'][1] < 6)
-        self.assertTrue(apds['duration'][1] > 3.5)
-        self.assertTrue(apds['duration'][1] < 4.0)
-
-        # Check with threshold equal to V
-        apds = d.apd(v='v', threshold=-85)
-        self.assertEqual(len(apds['start']), 1)
-        self.assertEqual(apds['start'][0], 5)
-        self.assertEqual(apds['duration'][0], 4)
-
-        # Check against example model
-        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
-        s = myokit.Simulation(m, p)
-        s.set_tolerance(1e-8, 1e-8)
-        d, apds1 = s.run(
-            2000, log=['engine.time', 'membrane.V'],
-            log_interval=0.005,
-            apd_variable='membrane.V', apd_threshold=-70)
-        apds2 = d.apd(threshold=-70)
-        self.assertEqual(len(apds1['start']), 2)
-        self.assertEqual(len(apds2['start']), 2)
-        self.assertAlmostEqual(1, apds1['start'][0] / apds2['start'][0])
-        self.assertAlmostEqual(1, apds1['start'][1] / apds2['start'][1])
-        self.assertAlmostEqual(1, apds1['duration'][0] / apds2['duration'][0])
-        self.assertAlmostEqual(1, apds1['duration'][1] / apds2['duration'][1])
-
-    def test_clone(self):
-        # Test data log cloning.
-
-        m, p, x = myokit.load(os.path.join(DIR_DATA, 'lr-1991.mmt'))
-        s = myokit.Simulation(m, p)
-        d1 = s.run(100, log=myokit.LOG_BOUND + myokit.LOG_STATE).npview()
-        d2 = d1.clone()
-
-        # Check keys are the same
-        self.assertEqual(d1.keys(), d2.keys())
-
-        # Check the values are the same, but not the same objects
-        for k, v in d1.items():
-            self.assertTrue(np.all(v == d2[k]))
-            self.assertFalse(v is d2[k])
-            self.assertTrue(type(d2[k]) == list)
-
-        # Check cloning as numpy arrays
-        d2 = d1.clone(numpy=True)
-        self.assertEqual(d1.keys(), d2.keys())
-        for k, v in d1.items():
-            self.assertTrue(np.all(v == d2[k]))
-            self.assertFalse(v is d2[k])
-            self.assertTrue(type(d2[k]) == np.ndarray)
-
-    def test_fold(self):
-        # Test the fold() method.
-
-        d = myokit.DataLog(time='time')
-        d['time'] = list(range(100))
-        d['x'] = list(np.arange(100) * 3)
-
-        # Test without discarding remainder
-        d2 = d.fold(30, discard_remainder=False)
-        self.assertEqual(set(d2.keys()), set([
-            'time', '0.x', '1.x', '2.x', '3.x']))
-
-        # Test with discarding remainder
-        d = d.npview()
-        d2 = d.fold(30)
-        self.assertEqual(set(d2.keys()), set([
-            'time', '0.x', '1.x', '2.x']))
-        self.assertEqual(len(d2['time']), 30)
-        self.assertEqual(len(d2['0.x']), 30)
-        self.assertEqual(len(d2['1.x']), 30)
-        self.assertEqual(len(d2['2.x']), 30)
-        self.assertTrue(np.all(d2['time'] == d['time'][:30]))
-        self.assertTrue(np.all(d2['0.x'] == d['x'][:30]))
-        self.assertTrue(np.all(d2['1.x'] == d['x'][30:60]))
-        self.assertTrue(np.all(d2['2.x'] == d['x'][60:90]))
-
-    def test_has_nan(self):
-        # Test the has_nan() method, which checks if the _final_ value in any
-        # field is NaN.
-
-        d = myokit.DataLog(time='time')
-        d['time'] = list(range(100))
-        d['x'] = list(np.arange(100) * 3)
-        d['y'] = list(np.arange(100) * 3)
-        d['z'] = list(np.arange(100) * 3)
-        self.assertFalse(d.has_nan())
-        d['x'][-3] = float('nan')
-        self.assertFalse(d.has_nan())
-        d['x'][-1] = float('inf')
-        self.assertFalse(d.has_nan())
-        d['x'][-1] = float('nan')
-        self.assertTrue(d.has_nan())
-
-    def test_length(self):
-        # Test the length() method, that counts the length of the log's
-        # entries.
-
-        d = myokit.DataLog(time='time')
-        self.assertEqual(d.length(), 0)
-        d['time'] = list(np.arange(100) * 3)
-        self.assertEqual(d.length(), 100)
-        d['x'] = list(np.arange(100) * 3)
-        self.assertEqual(d.length(), 100)
-
-    def test_regularize(self):
-        # Test the deprecated regularize() method.
-
-        d = myokit.DataLog(time='time')
-        d['time'] = np.log(np.linspace(1, 25, 100))
-        d['values'] = np.linspace(1, 25, 100)
-
-        has_scipy = True
-        with WarningCollector() as w:
-            try:
-                e = d.regularize(dt=0.5)
-            except ImportError:
-                has_scipy = False
-        self.assertIn('eprecated', w.text())
-        if not has_scipy:
-            return
-
-        self.assertEqual(len(e['time']), 7)
-        x = np.array([0, 0.5, 1, 1.5, 2, 2.5, 3])
-        self.assertTrue(np.all(e['time'] == x))
-        for i, y in enumerate(x):
-            self.assertTrue(np.abs(np.exp(y) - e['values'][i]) < 0.02)
-
-        # test setting tmin and tmax
-        with WarningCollector() as w:
-            e = d.regularize(dt=0.5, tmin=0.4, tmax=2.6)
-        self.assertEqual(len(e['time']), 5)
-        x = np.array([0.4, 0.9, 1.4, 1.9, 2.4])
-        self.assertTrue(np.all(e['time'] == x))
-        for i, y in enumerate(x):
-            self.assertTrue(np.abs(np.exp(y) - e['values'][i]) < 0.02)
-
-    def test_time(self):
-        # Test the time() method.
-
-        d = myokit.DataLog(time='t')
-        t = [1, 2, 3]
-        d['t'] = t
-        self.assertIs(d['t'], t)
-
-        # Test non-existing time key
-        d = myokit.DataLog(time='t')
-        self.assertRaisesRegex(
-            myokit.InvalidDataLogError, 'Invalid key', d.time)
-
-        # Test no time key
-        d = myokit.DataLog()
-        self.assertRaisesRegex(
-            myokit.InvalidDataLogError, 'No time', d.time)
-
-    def test_variable_info_errors(self):
-        # Test errors raised during variable info checking.
-
-        # Test mismatched dimensions (1d versus 2d)
-        d = myokit.DataLog(time='t')
-        d['t'] = [1, 2, 3, 4]
-        d['0.v'] = [1, 2, 3, 4]
-        d['1.1.v'] = [1, 2, 3, 4]
-        self.assertRaisesRegex(
-            RuntimeError, 'Different dimensions', d.variable_info)
-        # Note: Valid log, so not an InvalidDataLogError
-
-        # Test "irregular data": can't be arranged in a rectangular grid
-        d = myokit.DataLog(time='t')
-        d['t'] = [1, 2, 3, 4]
-        d['0.0.v'] = [1, 2, 3, 4]
-        d['0.2.v'] = [1, 2, 3, 4]
-        d['1.0.v'] = [1, 2, 3, 4]
-        d['1.1.v'] = [1, 2, 3, 4]
-        self.assertRaisesRegex(RuntimeError, 'Irregular', d.variable_info)
-        # Note: Valid log, so not an InvalidDataLogError
-
     def test_variable_info(self):
         # Test if correct variable info is returned.
 
         d = myokit.DataLog(time='t')
         # Odd grid
         d['0.0.v'] = [0, 1, 2, 3]
         d['0.2.v'] = [1, 2, 3, 4]
@@ -2286,14 +2456,84 @@
         self.assertEqual(v.size(), (3, 2))
         self.assertEqual(w.size(), (3, 2))
 
         # Check name
         self.assertEqual(v.name(), 'v')
         self.assertEqual(w.name(), 'w')
 
+    def test_variable_info_errors(self):
+        # Test errors raised during variable info checking.
+
+        # Test mismatched dimensions (1d versus 2d)
+        d = myokit.DataLog(time='t')
+        d['t'] = [1, 2, 3, 4]
+        d['0.v'] = [1, 2, 3, 4]
+        d['1.1.v'] = [1, 2, 3, 4]
+        self.assertRaisesRegex(
+            RuntimeError, 'Different dimensions', d.variable_info)
+        # Note: Valid log, so not an InvalidDataLogError
+
+        # Test "irregular data": can't be arranged in a rectangular grid
+        d = myokit.DataLog(time='t')
+        d['t'] = [1, 2, 3, 4]
+        d['0.0.v'] = [1, 2, 3, 4]
+        d['0.2.v'] = [1, 2, 3, 4]
+        d['1.0.v'] = [1, 2, 3, 4]
+        d['1.1.v'] = [1, 2, 3, 4]
+        self.assertRaisesRegex(RuntimeError, 'Irregular', d.variable_info)
+        # Note: Valid log, so not an InvalidDataLogError
+
+
+class ColumnMetaDataTest(unittest.TestCase):
+    """ Tests for the ColumnMetaData class. """
+
+    def test_set_and_del(self):
+        # Both are "disabled": Should only be handled by parent DataLog
+
+        m = myokit.ColumnMetaData()
+        self.assertEqual(list(m.keys()), [])
+        with self.assertRaisesRegex(ValueError, 'managed by a DataLog'):
+            m['x'] = 123
+        self.assertEqual(list(m.keys()), [])
+        m._add('x')
+        self.assertEqual(list(m.keys()), ['x'])
+        self.assertEqual(type(m['x']), myokit.MetaDataContainer)
+        with self.assertRaisesRegex(ValueError, 'managed by a DataLog'):
+            m['x'] = 123
+        with self.assertRaisesRegex(ValueError, 'managed by a DataLog'):
+            del m['x']
+        self.assertEqual(list(m.keys()), ['x'])
+        m._remove('x')
+        self.assertEqual(list(m.keys()), [])
+
+    def test_clone(self):
+        # Test cloning via constructor
+
+        m = myokit.ColumnMetaData()
+        m._add('x')
+        m._add('y')
+        self.assertFalse(m['x'] is m['y'])
+        m['x']['keyx1'] = 'value1'
+        m['y']['keyy1'] = 15
+        m2 = myokit.ColumnMetaData(m)
+        self.assertFalse(m2 is m)
+        self.assertIn('x', m2)
+        self.assertEqual(len(m2['x']), 1)
+        self.assertIn('keyx1', m2['x'])
+        self.assertEqual(m2['x']['keyx1'], 'value1')
+        self.assertIn('y', m2)
+        self.assertEqual(len(m2['y']), 1)
+        self.assertIn('keyy1', m2['y'])
+        self.assertEqual(m2['y']['keyy1'], '15')
+        self.assertFalse(m2['x'] is m['x'])
+        self.assertFalse(m2['y'] is m['y'])
+
+        with self.assertRaisesRegex(ValueError, 'ColumnMetaData or None'):
+            myokit.ColumnMetaData({})
+
 
 if __name__ == '__main__':
     print('Add -v for more debug output')
     import sys
     if '-v' in sys.argv:
         debug = True
     unittest.main()
```

### Comparing `myokit-1.35.2/myokit/tests/test_dependency_checking.py` & `myokit-1.35.3/myokit/tests/test_dependency_checking.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_expressions.py` & `myokit-1.35.3/myokit/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_float.py` & `myokit-1.35.3/myokit/tests/test_float.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats.py` & `myokit-1.35.3/myokit/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_axon.py` & `myokit-1.35.3/myokit/tests/test_formats_axon.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_cellml.py` & `myokit-1.35.3/myokit/tests/test_formats_cellml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_channelml.py` & `myokit-1.35.3/myokit/tests/test_formats_channelml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_easyml.py` & `myokit-1.35.3/myokit/tests/test_formats_easyml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_exporters.py` & `myokit-1.35.3/myokit/tests/test_formats_exporters.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_expression_writers.py` & `myokit-1.35.3/myokit/tests/test_formats_expression_writers.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_html.py` & `myokit-1.35.3/myokit/tests/test_formats_html.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_importers.py` & `myokit-1.35.3/myokit/tests/test_formats_importers.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_mathml_content.py` & `myokit-1.35.3/myokit/tests/test_formats_mathml_content.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_mathml_presentation.py` & `myokit-1.35.3/myokit/tests/test_formats_mathml_presentation.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_opencl.py` & `myokit-1.35.3/myokit/tests/test_formats_opencl.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_sbml.py` & `myokit-1.35.3/myokit/tests/test_formats_sbml.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_sympy.py` & `myokit-1.35.3/myokit/tests/test_formats_sympy.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_formats_wcp.py` & `myokit-1.35.3/myokit/tests/test_formats_wcp.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_io.py` & `myokit-1.35.3/myokit/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_jacobian_calculator.py` & `myokit-1.35.3/myokit/tests/test_jacobian_calculator.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_jacobian_tracer.py` & `myokit-1.35.3/myokit/tests/test_jacobian_tracer.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_lib_deps.py` & `myokit-1.35.3/myokit/tests/test_lib_deps.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_lib_guess.py` & `myokit-1.35.3/myokit/tests/test_lib_guess.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_lib_hh.py` & `myokit-1.35.3/myokit/tests/test_lib_hh.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_lib_markov.py` & `myokit-1.35.3/myokit/tests/test_lib_markov.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_lib_multi.py` & `myokit-1.35.3/myokit/tests/test_lib_multi.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_lib_plots.py` & `myokit-1.35.3/myokit/tests/test_lib_plots.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_meta.py` & `myokit-1.35.3/myokit/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_model.py` & `myokit-1.35.3/myokit/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_model_building.py` & `myokit-1.35.3/myokit/tests/test_model_building.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_opencl_info.py` & `myokit-1.35.3/myokit/tests/test_opencl_info.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_pacing_factory.py` & `myokit-1.35.3/myokit/tests/test_pacing_factory.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_pacing_system_c.py` & `myokit-1.35.3/myokit/tests/test_pacing_system_c.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_pacing_system_py.py` & `myokit-1.35.3/myokit/tests/test_pacing_system_py.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_parsing.py` & `myokit-1.35.3/myokit/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_progress_reporters.py` & `myokit-1.35.3/myokit/tests/test_progress_reporters.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_protocol.py` & `myokit-1.35.3/myokit/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_protocol_floating_point.py` & `myokit-1.35.3/myokit/tests/test_protocol_floating_point.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_protocol_time_series.py` & `myokit-1.35.3/myokit/tests/test_protocol_time_series.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_pype.py` & `myokit-1.35.3/myokit/tests/test_pype.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_quantity.py` & `myokit-1.35.3/myokit/tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_rhs_benchmarker.py` & `myokit-1.35.3/myokit/tests/test_rhs_benchmarker.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_sbml_api.py` & `myokit-1.35.3/myokit/tests/test_sbml_api.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_sbml_parser.py` & `myokit-1.35.3/myokit/tests/test_sbml_parser.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_simulation_1d.py` & `myokit-1.35.3/myokit/tests/test_simulation_1d.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_simulation_cvodes.py` & `myokit-1.35.3/myokit/tests/test_simulation_cvodes.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_simulation_cvodes_from_disk.py` & `myokit-1.35.3/myokit/tests/test_simulation_cvodes_from_disk.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_simulation_fiber_tissue.py` & `myokit-1.35.3/myokit/tests/test_simulation_fiber_tissue.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_simulation_log_interval.py` & `myokit-1.35.3/myokit/tests/test_simulation_log_interval.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_simulation_opencl.py` & `myokit-1.35.3/myokit/tests/test_simulation_opencl.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_simulation_opencl_log_interval.py` & `myokit-1.35.3/myokit/tests/test_simulation_opencl_log_interval.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_simulation_opencl_vs_cvode.py` & `myokit-1.35.3/myokit/tests/test_simulation_opencl_vs_cvode.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_simulation_opencl_vs_sim1d.py` & `myokit-1.35.3/myokit/tests/test_simulation_opencl_vs_sim1d.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_system_info.py` & `myokit-1.35.3/myokit/tests/test_system_info.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_tools.py` & `myokit-1.35.3/myokit/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_unit.py` & `myokit-1.35.3/myokit/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_user_functions.py` & `myokit-1.35.3/myokit/tests/test_user_functions.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tests/test_variable.py` & `myokit-1.35.3/myokit/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/tools.py` & `myokit-1.35.3/myokit/tools.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit/units.py` & `myokit-1.35.3/myokit/units.py`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/myokit.egg-info/PKG-INFO` & `myokit-1.35.3/myokit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myokit
-Version: 1.35.2
+Version: 1.35.3
 Summary: A simple interface to cardiac cellular electrophysiology
 Home-page: http://myokit.org
 Author: Michael Clerx
 Author-email: michael@myokit.org
 License: BSD 3-clause license
 Project-URL: Bug Tracker, https://github.com/MichaelClerx/myokit/issues
 Project-URL: Documentation, http://docs.myokit.org
```

### Comparing `myokit-1.35.2/myokit.egg-info/SOURCES.txt` & `myokit-1.35.3/myokit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `myokit-1.35.2/setup.py` & `myokit-1.35.3/setup.py`

 * *Files identical despite different names*

