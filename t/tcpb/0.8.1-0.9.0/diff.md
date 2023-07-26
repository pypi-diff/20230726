# Comparing `tmp/tcpb-0.8.1.tar.gz` & `tmp/tcpb-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcpb-0.8.1.tar", last modified: Sat Feb 26 04:00:40 2022, max compression
+gzip compressed data, was "tcpb-0.9.0.tar", last modified: Fri Mar 11 03:28:22 2022, max compression
```

## Comparing `tcpb-0.8.1.tar` & `tcpb-0.9.0.tar`

### file list

```diff
@@ -1,51 +1,50 @@
--rw-r--r--   0        0        0      237 2022-01-28 00:37:36.850896 tcpb-0.8.1/.flake8
--rw-r--r--   0        0        0     2031 2022-01-28 00:37:36.850896 tcpb-0.8.1/.gitignore
--rw-r--r--   0        0        0     1033 2022-02-26 03:59:50.248512 tcpb-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      198 2022-01-28 00:37:55.325802 tcpb-0.8.1/.vscode/settings.json
--rw-r--r--   0        0        0     4431 2022-02-26 03:59:50.248512 tcpb-0.8.1/CHANGELOG.md
--rw-r--r--   0        0        0     2745 2022-01-28 00:37:36.854895 tcpb-0.8.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1079 2022-01-28 00:37:36.854895 tcpb-0.8.1/LICENSE
--rw-r--r--   0        0        0      615 2022-01-28 00:37:36.854895 tcpb-0.8.1/README.md
--rwxr-xr-x   0        0        0     1035 2022-01-28 00:37:36.854895 tcpb-0.8.1/build_conda_pkgs.sh
--rw-r--r--   0        0        0     1012 2022-02-26 03:59:50.248512 tcpb-0.8.1/docs/usage.md
--rw-r--r--   0        0        0      747 2022-02-26 03:59:50.248512 tcpb-0.8.1/examples/basic_energy.py
--rwxr-xr-x   0        0        0     2145 2022-02-26 03:59:50.252512 tcpb-0.8.1/examples/ci_overlap_example.py
--rwxr-xr-x   0        0        0     1284 2022-02-26 03:59:50.252512 tcpb-0.8.1/examples/cisno_casci_example.py
--rwxr-xr-x   0        0        0     1190 2022-02-26 03:59:50.252512 tcpb-0.8.1/examples/fomo_casci_example.py
--rw-r--r--   0        0        0     1318 2022-02-26 03:59:50.248512 tcpb-0.8.1/examples/frontend_example.py
--rwxr-xr-x   0        0        0     1637 2022-02-26 03:59:50.252512 tcpb-0.8.1/examples/guess_reuse_example.py
--rw-r--r--   0        0        0     1382 2022-02-26 03:59:50.248512 tcpb-0.8.1/examples/guess_reuse_tcfe.py
--rw-r--r--   0        0        0      845 2022-02-26 03:59:50.248512 tcpb-0.8.1/examples/molden_file.py
--rwxr-xr-x   0        0        0     1466 2022-02-26 03:59:50.252512 tcpb-0.8.1/examples/sa_casscf_example.py
--rwxr-xr-x   0        0        0     1610 2022-02-26 03:59:50.252512 tcpb-0.8.1/examples/tddft_example.py
--rwxr-xr-x   0        0        0     1603 2022-02-26 03:59:50.252512 tcpb-0.8.1/examples/verbose_example.py
--rw-r--r--   0        0        0      475 2022-01-28 00:37:36.854895 tcpb-0.8.1/meta.yaml
--rw-r--r--   0        0        0      198 2022-01-28 00:37:36.854895 tcpb-0.8.1/mypy.ini
--rw-r--r--   0        0        0     1686 2022-02-26 03:59:50.248512 tcpb-0.8.1/pyproject.toml
--rwxr-xr-x   0        0        0      203 2022-02-26 03:59:50.248512 tcpb-0.8.1/scripts/format.sh
--rw-r--r--   0        0        0      135 2022-02-26 03:59:50.248512 tcpb-0.8.1/tcpb/__init__.py
--rw-r--r--   0        0        0    42676 2022-02-26 03:59:50.248512 tcpb-0.8.1/tcpb/clients.py
--rw-r--r--   0        0        0      323 2022-02-26 03:59:50.248512 tcpb-0.8.1/tcpb/config.py
--rw-r--r--   0        0        0      990 2022-02-26 03:59:50.248512 tcpb-0.8.1/tcpb/exceptions.py
--rw-r--r--   0        0        0     7205 2022-01-28 00:37:36.854895 tcpb-0.8.1/tcpb/molden_constructor.py
--rw-r--r--   0        0        0     2612 2022-01-28 00:37:36.854895 tcpb-0.8.1/tcpb/serial_utils.py
--rw-r--r--   0        0        0     6196 2022-02-24 01:28:05.267468 tcpb-0.8.1/tcpb/terachem_server.proto
--rw-r--r--   0        0        0    65777 2022-01-28 00:37:55.325802 tcpb-0.8.1/tcpb/terachem_server_pb2.py
--rw-r--r--   0        0        0    24581 2022-01-28 00:37:55.325802 tcpb-0.8.1/tcpb/terachem_server_pb2.pyi
--rw-r--r--   0        0        0     8247 2022-02-26 03:59:50.248512 tcpb-0.8.1/tcpb/utils.py
--rw-r--r--   0        0        0        0 2022-01-28 00:37:36.854895 tcpb-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-01-28 00:37:36.854895 tcpb-0.8.1/tests/answers/__init__.py
--rw-r--r--   0        0        0     6588 2022-01-28 00:37:36.854895 tcpb-0.8.1/tests/answers/ci_overlap.py
--rw-r--r--   0        0        0     4666 2022-01-28 00:37:36.854895 tcpb-0.8.1/tests/answers/cisno_casci.py
--rw-r--r--   0        0        0     1593 2022-01-28 00:37:36.854895 tcpb-0.8.1/tests/answers/cisno_casci_result.pbmsg
--rw-r--r--   0        0        0     5029 2022-01-28 00:37:36.854895 tcpb-0.8.1/tests/answers/fomo_casci.py
--rw-r--r--   0        0        0     2144 2022-02-26 03:59:50.248512 tcpb-0.8.1/tests/conftest.py
--rw-r--r--   0        0        0     2706 2022-01-28 00:37:55.325802 tcpb-0.8.1/tests/test_ci_overlap.py
--rw-r--r--   0        0        0     3014 2022-02-26 03:59:50.248512 tcpb-0.8.1/tests/test_cisno_casci.py
--rw-r--r--   0        0        0     4574 2022-01-28 00:37:55.325802 tcpb-0.8.1/tests/test_data/water.molden
--rw-r--r--   0        0        0       85 2022-01-28 00:37:36.854895 tcpb-0.8.1/tests/test_data/water_angstrom.pb
--rw-r--r--   0        0        0       91 2022-01-28 00:37:36.854895 tcpb-0.8.1/tests/test_data/water_bohr.pb
--rw-r--r--   0        0        0     1388 2022-01-28 00:37:36.854895 tcpb-0.8.1/tests/test_fomo_casci.py
--rw-r--r--   0        0        0     2650 2022-02-26 03:59:50.248512 tcpb-0.8.1/tests/test_keywords.py
--rw-r--r--   0        0        0     4331 2022-02-26 03:59:50.248512 tcpb-0.8.1/tests/test_utils.py
--rw-r--r--   0        0        0     2291 1970-01-01 00:00:00.000000 tcpb-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      237 2022-03-03 21:40:39.373503 tcpb-0.9.0/.flake8
+-rw-r--r--   0        0        0     2031 2022-03-03 21:40:39.373503 tcpb-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1033 2022-03-03 21:40:39.373503 tcpb-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      198 2022-03-03 21:40:39.373503 tcpb-0.9.0/.vscode/settings.json
+-rw-r--r--   0        0        0     5073 2022-03-11 03:27:52.624642 tcpb-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2745 2022-03-03 21:40:39.373503 tcpb-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1079 2022-03-03 21:40:39.373503 tcpb-0.9.0/LICENSE
+-rw-r--r--   0        0        0      615 2022-03-03 21:40:39.373503 tcpb-0.9.0/README.md
+-rwxr-xr-x   0        0        0     1035 2022-03-03 21:40:39.373503 tcpb-0.9.0/build_conda_pkgs.sh
+-rw-r--r--   0        0        0     1012 2022-03-03 21:40:39.373503 tcpb-0.9.0/docs/usage.md
+-rw-r--r--   0        0        0      747 2022-03-03 21:40:39.373503 tcpb-0.9.0/examples/basic_energy.py
+-rwxr-xr-x   0        0        0     2145 2022-03-03 21:40:39.373503 tcpb-0.9.0/examples/ci_overlap_example.py
+-rwxr-xr-x   0        0        0     1284 2022-03-03 21:40:39.373503 tcpb-0.9.0/examples/cisno_casci_example.py
+-rwxr-xr-x   0        0        0     1190 2022-03-03 21:40:39.373503 tcpb-0.9.0/examples/fomo_casci_example.py
+-rw-r--r--   0        0        0     1318 2022-03-11 02:03:36.809683 tcpb-0.9.0/examples/frontend_example.py
+-rwxr-xr-x   0        0        0     1637 2022-03-03 21:40:39.373503 tcpb-0.9.0/examples/guess_reuse_example.py
+-rw-r--r--   0        0        0     1382 2022-03-03 21:40:39.373503 tcpb-0.9.0/examples/guess_reuse_tcfe.py
+-rwxr-xr-x   0        0        0     1466 2022-03-03 21:40:39.373503 tcpb-0.9.0/examples/sa_casscf_example.py
+-rwxr-xr-x   0        0        0     1610 2022-03-03 21:40:39.373503 tcpb-0.9.0/examples/tddft_example.py
+-rwxr-xr-x   0        0        0     1603 2022-03-03 21:40:39.373503 tcpb-0.9.0/examples/verbose_example.py
+-rw-r--r--   0        0        0      475 2022-03-03 21:40:39.373503 tcpb-0.9.0/meta.yaml
+-rw-r--r--   0        0        0      198 2022-03-03 21:40:39.373503 tcpb-0.9.0/mypy.ini
+-rw-r--r--   0        0        0     1710 2022-03-11 03:27:52.624642 tcpb-0.9.0/pyproject.toml
+-rwxr-xr-x   0        0        0      203 2022-03-11 03:27:52.624642 tcpb-0.9.0/scripts/format.sh
+-rw-r--r--   0        0        0      135 2022-03-11 03:27:52.624642 tcpb-0.9.0/tcpb/__init__.py
+-rw-r--r--   0        0        0    43287 2022-03-11 03:27:52.624642 tcpb-0.9.0/tcpb/clients.py
+-rw-r--r--   0        0        0      374 2022-03-11 03:27:52.624642 tcpb-0.9.0/tcpb/config.py
+-rw-r--r--   0        0        0      990 2022-03-03 21:40:39.377503 tcpb-0.9.0/tcpb/exceptions.py
+-rw-r--r--   0        0        0     2612 2022-03-03 21:40:39.377503 tcpb-0.9.0/tcpb/serial_utils.py
+-rw-r--r--   0        0        0     6196 2022-03-03 21:40:39.377503 tcpb-0.9.0/tcpb/terachem_server.proto
+-rw-r--r--   0        0        0    65777 2022-03-03 21:40:39.377503 tcpb-0.9.0/tcpb/terachem_server_pb2.py
+-rw-r--r--   0        0        0    24593 2022-03-11 03:27:52.624642 tcpb-0.9.0/tcpb/terachem_server_pb2.pyi
+-rw-r--r--   0        0        0     7663 2022-03-11 03:27:52.624642 tcpb-0.9.0/tcpb/utils.py
+-rw-r--r--   0        0        0        0 2022-03-03 21:40:39.377503 tcpb-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-03 21:40:39.377503 tcpb-0.9.0/tests/answers/__init__.py
+-rw-r--r--   0        0        0     6588 2022-03-03 21:40:39.377503 tcpb-0.9.0/tests/answers/ci_overlap.py
+-rw-r--r--   0        0        0     4666 2022-03-03 21:40:39.377503 tcpb-0.9.0/tests/answers/cisno_casci.py
+-rw-r--r--   0        0        0     1593 2022-03-03 21:40:39.377503 tcpb-0.9.0/tests/answers/cisno_casci_result.pbmsg
+-rw-r--r--   0        0        0     5029 2022-03-03 21:40:39.377503 tcpb-0.9.0/tests/answers/fomo_casci.py
+-rw-r--r--   0        0        0     2596 2022-03-11 03:27:52.624642 tcpb-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0     2706 2022-03-03 21:40:39.377503 tcpb-0.9.0/tests/test_ci_overlap.py
+-rw-r--r--   0        0        0     3014 2022-03-10 20:33:26.710425 tcpb-0.9.0/tests/test_cisno_casci.py
+-rw-r--r--   0        0        0     4574 2022-03-03 21:40:39.377503 tcpb-0.9.0/tests/test_data/water.molden
+-rw-r--r--   0        0        0       85 2022-03-03 21:40:39.377503 tcpb-0.9.0/tests/test_data/water_angstrom.pb
+-rw-r--r--   0        0        0       91 2022-03-03 21:40:39.377503 tcpb-0.9.0/tests/test_data/water_bohr.pb
+-rw-r--r--   0        0        0     1633 2022-03-11 03:27:52.624642 tcpb-0.9.0/tests/test_fomo_casci.py
+-rw-r--r--   0        0        0     8156 2022-03-11 03:27:52.624642 tcpb-0.9.0/tests/test_frontend_client.py
+-rw-r--r--   0        0        0     2143 2022-03-11 03:27:52.624642 tcpb-0.9.0/tests/test_keywords.py
+-rw-r--r--   0        0        0     4331 2022-03-03 21:40:39.377503 tcpb-0.9.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 tcpb-0.9.0/PKG-INFO
```

### Comparing `tcpb-0.8.1/.gitignore` & `tcpb-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/.pre-commit-config.yaml` & `tcpb-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/CHANGELOG.md` & `tcpb-0.9.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,16 +4,43 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
 ### Added
 
-- `TCFrontEndClient` to enable access to the files written by TeraChem and upload input files for TeraChem, in particulat `c0` files as initial wavefunction guesses.
-  - Configuration parameters for controlling TCFrontEndClient behavior are
+### Changed
+
+### Removed
+
+## [0.9.0]
+
+### Added
+
+- Configuration parameters for controlling `TCFrontEndClient` behavior:
+
+  1. `native_files`: list[str] - List of natives files to collect. If none passed, all files will be collected.
+
+- Tests for `TCFrontEndClient` file put/get behaviors.
+
+### Changed
+
+- Refactored `TCFrontEndClient`
+
+### Removed
+
+- Construction of molden file from protocol buffer outputs. Molden files can now be requested directly from the Frontend client.
+
+## [0.8.1]
+
+### Added
+
+- `TCFrontEndClient` to enable access to the files written by TeraChem and upload input files for TeraChem, in particular `c0` files as initial wavefunction guesses.
+
+  - Configuration parameters for controlling `TCFrontEndClient` behavior are
     found in AtomicInput.extras['tcfe:config'] and include:
     1. `c0` | `ca0` and `cb0`: `bytes` - Binary files to use as an initial guess
        wavefunction
     2. `scratch_messy`: `bool` - If `True` client will not delete files on server
        after a computation
     3. `uploads_messy`: `bool` - If `True` client will not delete uploaded c0
        file(s) after a computation
@@ -81,15 +108,17 @@
 
 ## 0.5.x - Long long ago
 
 ### Added
 
 - All of Stefan's original code.
 
-[unreleased]: https://github.com/mtzgroup/tcpb-client/compare/0.8.0...HEAD
+[unreleased]: https://github.com/mtzgroup/tcpb-client/compare/0.9.0...HEAD
+[0.9.0]: https://github.com/mtzgroup/tcpb-client/releases/tag/0.9.0
+[0.8.1]: https://github.com/mtzgroup/tcpb-client/releases/tag/0.8.1
 [0.8.0]: https://github.com/mtzgroup/tcpb-client/releases/tag/0.8.0
 [0.7.2]: https://github.com/mtzgroup/tcpb-client/releases/tag/0.7.2
 [0.7.1]: https://github.com/mtzgroup/tcpb-client/releases/tag/0.7.1
 [0.7.0]: https://github.com/mtzgroup/tcpb-client/releases/tag/0.7.0
 [r0.6.0]: https://github.com/mtzgroup/tcpb-client/releases/tag/r0.6.0
 [r0.5.3]: https://github.com/mtzgroup/tcpb-client/releases/tag/r0.5.3
 [r0.5.2]: https://github.com/mtzgroup/tcpb-client/releases/tag/r0.5.2
```

### Comparing `tcpb-0.8.1/CONTRIBUTING.md` & `tcpb-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/LICENSE` & `tcpb-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/README.md` & `tcpb-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/build_conda_pkgs.sh` & `tcpb-0.9.0/build_conda_pkgs.sh`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/docs/usage.md` & `tcpb-0.9.0/docs/usage.md`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/examples/basic_energy.py` & `tcpb-0.9.0/examples/basic_energy.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/examples/ci_overlap_example.py` & `tcpb-0.9.0/examples/ci_overlap_example.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/examples/cisno_casci_example.py` & `tcpb-0.9.0/examples/cisno_casci_example.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/examples/fomo_casci_example.py` & `tcpb-0.9.0/examples/fomo_casci_example.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/examples/frontend_example.py` & `tcpb-0.9.0/examples/frontend_example.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/examples/guess_reuse_example.py` & `tcpb-0.9.0/examples/guess_reuse_example.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/examples/guess_reuse_tcfe.py` & `tcpb-0.9.0/examples/guess_reuse_tcfe.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/examples/sa_casscf_example.py` & `tcpb-0.9.0/examples/sa_casscf_example.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/examples/tddft_example.py` & `tcpb-0.9.0/examples/tddft_example.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/examples/verbose_example.py` & `tcpb-0.9.0/examples/verbose_example.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/pyproject.toml` & `tcpb-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
   "flake8 >=3.8.4",
   "pre-commit >= 2.9.3",
   "autoflake >= 1.4",
 ]
 test = [
   "pytest >=6.2.1",
   "pytest-cov >=2.10.1,<3.0.0",
+  "pytest-mock>=3.6.1",
   "coverage >=5.3.1,<6.0",
   "mypy ==0.790",
   "black >=20.8b1,<21.0b0",
   "isort >=5.7.0,<6.0.0",
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `tcpb-0.8.1/tcpb/clients.py` & `tcpb-0.9.0/tcpb/clients.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """
 
 import logging
 import socket
 import struct
 import warnings
 from time import sleep
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 from uuid import uuid4
 
 import httpx
 import numpy as np
 from qcelemental.models.results import (
     AtomicInput,
     AtomicResult,
@@ -30,15 +30,14 @@
 
 from tcpb.utils import atomic_input_to_job_input, job_output_to_atomic_result
 
 # Import the Protobuf messages generated from the .proto file
 from . import terachem_server_pb2 as pb
 from .config import settings
 from .exceptions import ServerError
-from .molden_constructor import tcpb_imd_fields2molden_string
 
 logger = logging.getLogger(__name__)
 
 
 class TCProtobufClient:
     """Connect and communicate with a TeraChem instance running in Protocol Buffer server mode
     (i.e. TeraChem was started with the -s|--server flag)
@@ -413,17 +412,14 @@
                         np.array(
                             output.cis_transition_dipoles[4 * i : 4 * i + 3],
                             dtype=np.float64,
                         )
                     )
                 results["cis_transition_dipoles"] = tDips
 
-        if len(output.compressed_mo_vector):
-            results["molden"] = tcpb_imd_fields2molden_string(output)
-
         # Save results for user access later
         self.prev_results = results
 
         # Wipe state
         self.curr_job_dir = None
         self.curr_job_scr_dir = None
         self.curr_job_id = None
@@ -843,44 +839,45 @@
             packet = header + msg_str
             self.intracefile.write(packet)
 
         return recv_pb
 
 
 class TCFrontEndClient(TCProtobufClient):
-    """Client for interating with TeraChem FrontEnd.
+    """Client for interacting with TeraChem FrontEnd.
 
-    TeraChem FrontEnd proxies calls to a TeraChem Protocol Buffer Server and provides
-    access to the underlying files created by TeraChem from a compute job.
+    TeraChemFrontEndClient communicates with a TeraChem Protocol Buffer Server for
+    QC compute jobs and with a file server to get/put files to the server. A file may
+    be put to the server e.g., to use as an initial wave function guess, or any output
+    file retrieved after a computation.
     """
 
     def __init__(
         self,
         host: str = "127.0.0.1",
         port: int = 11111,
         frontend_port: int = 80,
+        frontend_host: Optional[str] = None,
         uploads_prefix: str = "uploads",
         debug=False,
         trace=False,
     ):
+        self.frontend_host = frontend_host or host
         self.frontend_port = frontend_port
         self.uploads_prefix = uploads_prefix
 
         super().__init__(host, port, debug, trace)
 
     def _request(self, method: str, path: str, **kwargs) -> httpx.Response:
         """Main method for sending requests to the TCFrontEnd file server"""
 
-        if path.startswith("/"):
-            raise ValueError("Path cannot start with '/'")
-
         with httpx.Client() as client:
             res = client.request(
                 method.upper(),
-                f"http://{self.host}:{self.frontend_port}/{path}",
+                f"http://{self.frontend_host}:{self.frontend_port}/{path}",
                 **kwargs,
             )
         res.raise_for_status()
         return res
 
     def ls(self, path: str = "/") -> List[Dict[str, str]]:
         """List directories on TeraChem Server
@@ -941,14 +938,15 @@
             found in AtomicInput.extras['tcfe:config'] and include:
                 1. 'c0' | 'ca0 and cb0': Binary files to use as an initial guess
                     wavefunction
                 2. 'scratch_messy': bool If True client will not delete files on server
                     after a computation
                 3. 'uploads_messy': bool If True client will not delete uploaded c0
                     file(s) after a computation
+                4. 'native_files': list[str] of filesnames to collect
 
         Parameters:
             atomic_input: AtomicInput object specifying the computation
         """
         # Do pre-compute work
         atomic_input = self._pre_compute_tasks(atomic_input)
         # Send calculation to TCPBS
@@ -975,15 +973,15 @@
             if "c0" in tcfe_config:
                 path = self.put("c0", tcfe_config["c0"])
 
             else:
                 # ca0 and cb0 both exist
                 ca0_path = self.put("ca0", tcfe_config["ca0"])
                 cb0_path = self.put("cb0", tcfe_config["cb0"])
-                path = f"{ca0_path} {cb0_path}"
+                path = f"{ca0_path} {cb0_path}"  # TC wants two, space separated paths
 
             # 'keywords' will exist because AtomicInput defaults it to {} if empty
             ai_dict["keywords"]["guess"] = path
 
         return AtomicInput(**ai_dict)
 
     def _post_compute_tasks(self, result: AtomicResult) -> AtomicResult:
@@ -999,41 +997,59 @@
         job_dir = result.extras[settings.extras_job_kwarg]["job_dir"]
 
         # dict for modifying attributes
         result_dict = result.dict()
 
         # Retreive tc.out if requested
         if result.protocols.stdout:
-            req = self._request("GET", f"{job_dir}/tc.out")
-            result_dict["stdout"] = req.text
+            result_dict["stdout"] = self.get(f"{job_dir}/tc.out").decode()
 
         # Retrieve native_files if requested (files produced by TeraChem that don't fit
         # cleanly into the QCSchema json)
         if result.protocols.native_files in {NativeFilesProtocolEnum.all}:
-            # Assume no native_files added previously
-            result_dict["native_files"] = {}
-
-            # Collect Files; "all" is shorthand for the files collected below
-            orb1a_path = result.extras[settings.extras_job_kwarg]["orb1afile"]
-            orb1a_name = orb1a_path.split("/")[-1]
-            req = self._request("GET", orb1a_path)
-            result_dict["native_files"][orb1a_name] = req.content
-
-            orb1b_path = result.extras[settings.extras_job_kwarg]["orb1bfile"]
-            if orb1b_path:
-                orb1b_name = orb1b_path.split("/")[-1]
-                req = self._request("GET", orb1b_path)
-                result_dict["native_files"][orb1b_name] = req.content
+            self._collect_files(result_dict)
 
         # Cleanup uploads
         if self.uploads_prefix in result.keywords.get(
             "guess", ""
         ) and not tcfe_config.get("uploads_messy"):
             # Files were uploaded and put in "guess" keyword; also no request to maintain files
             for path in result.keywords["guess"].split():
-                req = self._request("DELETE", f"{path}")
+                self._request("DELETE", f"{path}")
 
         # Cleanup Scratch Directory
         if not tcfe_config.get("scratch_messy"):
             self._request("DELETE", f"{job_dir}/")
 
         return AtomicResult(**result_dict)
+
+    def _collect_files(self, result_dict: Dict[str, Any]) -> None:
+        """Collects requested native_files.
+
+        Parameters:
+            result_dict: Dictionary representation of an AtomicResult
+
+        Returns:
+            None: Modified result dictionary in place
+        """
+        tcfe_config = result_dict["extras"].get(settings.tcfe_config_kwarg, {})
+        scr_dir = result_dict["extras"][settings.extras_job_kwarg]["job_scr_dir"]
+
+        # Assume no native_files added previously
+        result_dict[settings.tcfe_config_native_files] = {}
+
+        if not tcfe_config.get("native_files"):
+            # Specific files not requested, return all
+            tcfe_config[settings.tcfe_config_native_files] = [
+                file_desc["name"]
+                for file_desc in self.ls(scr_dir)
+                if file_desc["type"] == "file"
+            ]
+
+        for output_file in tcfe_config[settings.tcfe_config_native_files]:
+            data = self.get(f"{scr_dir}/{output_file}")
+            try:
+                data = data.decode()
+            except UnicodeDecodeError:
+                # File is binary
+                pass
+            result_dict[settings.tcfe_config_native_files][output_file] = data
```

### Comparing `tcpb-0.8.1/tcpb/exceptions.py` & `tcpb-0.9.0/tcpb/exceptions.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/tcpb/serial_utils.py` & `tcpb-0.9.0/tcpb/serial_utils.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/tcpb/terachem_server.proto` & `tcpb-0.9.0/tcpb/terachem_server.proto`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/tcpb/terachem_server_pb2.py` & `tcpb-0.9.0/tcpb/terachem_server_pb2.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/tcpb/terachem_server_pb2.pyi` & `tcpb-0.9.0/tcpb/terachem_server_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -97,21 +97,23 @@
         self, oneof_group: typing_extensions.Literal["job_status", b"job_status"]
     ) -> typing_extensions.Literal["accepted", "working", "completed"]: ...
 
 global___Status = Status
 
 class Mol(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+
     class _UnitType(
         google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[UnitType.V],
         builtins.type,
     ):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
         ANGSTROM = Mol.UnitType.V(0)
         BOHR = Mol.UnitType.V(1)
+
     class UnitType(metaclass=_UnitType):
         V = typing.NewType("V", builtins.int)
     ANGSTROM = Mol.UnitType.V(0)
     BOHR = Mol.UnitType.V(1)
 
     ATOMS_FIELD_NUMBER: builtins.int
     XYZ_FIELD_NUMBER: builtins.int
@@ -162,31 +164,34 @@
         ],
     ) -> None: ...
 
 global___Mol = Mol
 
 class JobInput(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
+
     class _RunType(
         google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[RunType.V],
         builtins.type,
     ):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
         ENERGY = JobInput.RunType.V(0)
         GRADIENT = JobInput.RunType.V(1)
         COUPLING = JobInput.RunType.V(14)
         TDCI = JobInput.RunType.V(16)
         CI_VEC_OVERLAP = JobInput.RunType.V(19)
+
     class RunType(metaclass=_RunType):
         V = typing.NewType("V", builtins.int)
     ENERGY = JobInput.RunType.V(0)
     GRADIENT = JobInput.RunType.V(1)
     COUPLING = JobInput.RunType.V(14)
     TDCI = JobInput.RunType.V(16)
     CI_VEC_OVERLAP = JobInput.RunType.V(19)
+
     class _MethodType(
         google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[MethodType.V],
         builtins.type,
     ):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
         HF = JobInput.MethodType.V(0)
         CASE = JobInput.MethodType.V(2)
@@ -211,14 +216,15 @@
         CAMB3LYP = JobInput.MethodType.V(19)
         B97 = JobInput.MethodType.V(20)
         WB97 = JobInput.MethodType.V(21)
         WB97X = JobInput.MethodType.V(22)
         WB97XD3 = JobInput.MethodType.V(23)
         GFNXTB = JobInput.MethodType.V(24)
         GFN2XTB = JobInput.MethodType.V(25)
+
     class MethodType(metaclass=_MethodType):
         V = typing.NewType("V", builtins.int)
     HF = JobInput.MethodType.V(0)
     CASE = JobInput.MethodType.V(2)
     SVWN1 = JobInput.MethodType.V(3)
     SVWN3 = JobInput.MethodType.V(4)
     SVWN5 = JobInput.MethodType.V(5)
@@ -240,57 +246,63 @@
     CAMB3LYP = JobInput.MethodType.V(19)
     B97 = JobInput.MethodType.V(20)
     WB97 = JobInput.MethodType.V(21)
     WB97X = JobInput.MethodType.V(22)
     WB97XD3 = JobInput.MethodType.V(23)
     GFNXTB = JobInput.MethodType.V(24)
     GFN2XTB = JobInput.MethodType.V(25)
+
     class _ImdType(
         google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[ImdType.V],
         builtins.type,
     ):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
         NOT_IMD = JobInput.ImdType.V(0)
         IMD_NEW_CONDITION = JobInput.ImdType.V(1)
         IMD_CONTINUE = JobInput.ImdType.V(2)
         IMD_HESSIAN = JobInput.ImdType.V(3)
+
     class ImdType(metaclass=_ImdType):
         V = typing.NewType("V", builtins.int)
     NOT_IMD = JobInput.ImdType.V(0)
     IMD_NEW_CONDITION = JobInput.ImdType.V(1)
     IMD_CONTINUE = JobInput.ImdType.V(2)
     IMD_HESSIAN = JobInput.ImdType.V(3)
+
     class _ImdOrbitalType(
         google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[ImdOrbitalType.V],
         builtins.type,
     ):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
         NO_ORBITAL = JobInput.ImdOrbitalType.V(0)
         ALPHA_ORBITAL = JobInput.ImdOrbitalType.V(1)
         BETA_ORBITAL = JobInput.ImdOrbitalType.V(2)
         ALPHA_DENSITY = JobInput.ImdOrbitalType.V(3)
         BETA_DENSITY = JobInput.ImdOrbitalType.V(4)
         WHOLE_C = JobInput.ImdOrbitalType.V(5)
+
     class ImdOrbitalType(metaclass=_ImdOrbitalType):
         V = typing.NewType("V", builtins.int)
     NO_ORBITAL = JobInput.ImdOrbitalType.V(0)
     ALPHA_ORBITAL = JobInput.ImdOrbitalType.V(1)
     BETA_ORBITAL = JobInput.ImdOrbitalType.V(2)
     ALPHA_DENSITY = JobInput.ImdOrbitalType.V(3)
     BETA_DENSITY = JobInput.ImdOrbitalType.V(4)
     WHOLE_C = JobInput.ImdOrbitalType.V(5)
+
     class _ImdAdditionalOption(
         google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[
             ImdAdditionalOption.V
         ],
         builtins.type,
     ):
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor = ...
         IMD_NORMAL_MD = JobInput.ImdAdditionalOption.V(0)
         IMD_MECI_OPT_GRADIENT = JobInput.ImdAdditionalOption.V(1)
+
     class ImdAdditionalOption(metaclass=_ImdAdditionalOption):
         V = typing.NewType("V", builtins.int)
     IMD_NORMAL_MD = JobInput.ImdAdditionalOption.V(0)
     IMD_MECI_OPT_GRADIENT = JobInput.ImdAdditionalOption.V(1)
 
     MOL_FIELD_NUMBER: builtins.int
     RUN_FIELD_NUMBER: builtins.int
```

### Comparing `tcpb-0.8.1/tcpb/utils.py` & `tcpb-0.9.0/tcpb/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     AtomicResultProperties,
     Provenance,
     WavefunctionProperties,
 )
 
 from . import terachem_server_pb2 as pb
 from .config import settings
-from .molden_constructor import tcpb_imd_fields2molden_string
 
 SUPPORTED_DRIVERS = {"ENERGY", "GRADIENT"}
 
 
 def atomic_input_to_job_input(atomic_input: AtomicInput) -> pb.JobInput:
     """Convert AtomicInput to JobInput"""
     # Don't mutate original atomic_input object
@@ -106,25 +105,14 @@
 
     else:
         raise ValueError(
             f"Unsupported driver: {atomic_input.driver.upper()}, supported drivers "
             f"include: {SUPPORTED_DRIVERS}"
         )
 
-    if atomic_input.keywords.get("molden"):
-        # Molden file was request
-        try:
-            molden_string = tcpb_imd_fields2molden_string(job_output)
-        except Exception:
-            # Don't know how this code will blow up, so except everything for now :/
-            # NOTE: mo_output will set imd_orbital_type to "WHOLE_C"
-            molden_string = "Unable to create molden output. Did you include the 'mo_output' keyword??"
-    else:
-        molden_string = None
-
     # Prepare AtomicInput to be base input for AtomicResult
     atomic_input_dict = atomic_input.dict()
     atomic_input_dict.pop("provenance", None)
 
     # Create AtomicResult as superset of AtomicInput values
     atomic_result = AtomicResult(
         **atomic_input_dict,
@@ -160,15 +148,14 @@
             settings.extras_job_kwarg: {
                 "job_dir": jo_dict.get("job_dir"),
                 "job_scr_dir": jo_dict.get("job_scr_dir"),
                 "server_job_id": jo_dict.get("server_job_id"),
                 "orb1afile": jo_dict.get("orb1afile"),
                 "orb1bfile": jo_dict.get("orb1bfile"),
             },
-            "molden": molden_string,
         }
     )
     return atomic_result
 
 
 def to_atomic_result_properties(job_output: pb.JobOutput) -> AtomicResultProperties:
     """Extract AtomicResultProperties from JobOutput protobuf message"""
```

### Comparing `tcpb-0.8.1/tests/answers/ci_overlap.py` & `tcpb-0.9.0/tests/answers/ci_overlap.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/tests/answers/cisno_casci.py` & `tcpb-0.9.0/tests/answers/cisno_casci.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/tests/answers/cisno_casci_result.pbmsg` & `tcpb-0.9.0/tests/answers/cisno_casci_result.pbmsg`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/tests/answers/fomo_casci.py` & `tcpb-0.9.0/tests/answers/fomo_casci.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/tests/conftest.py` & `tcpb-0.9.0/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from pathlib import Path
 from typing import Collection, Union
 
 import pytest
-from qcelemental.models import AtomicInput, Molecule
+from qcelemental.models import (
+    AtomicInput,
+    AtomicResult,
+    AtomicResultProperties,
+    Molecule,
+)
 from qcelemental.models.common_models import Model
 
 from tcpb import terachem_server_pb2 as pb
+from tcpb.config import settings as tcpb_settings
 
 
 @pytest.fixture
 def settings():
     yield {"tcpb_host": "localhost", "tcpb_port": 11111, "round_decimals": 6}
 
 
@@ -57,14 +63,26 @@
 
 @pytest.fixture(scope="function")
 def atomic_input(water):
     model = Model(method="B3LYP", basis="6-31g")
     return AtomicInput(molecule=water, model=model, driver="energy")
 
 
+@pytest.fixture(scope="function")
+def atomic_result(atomic_input):
+    result = AtomicResult(
+        **atomic_input.dict(),
+        return_result=123.123,
+        success=True,
+        properties=AtomicResultProperties(return_energy=123.123),
+    )
+    result.extras[tcpb_settings.extras_job_kwarg] = {"job_dir": "job_1"}
+    return result
+
+
 @pytest.fixture
 def job_output():
     """Return job_output protobuf message"""
     job_output_correct_answer = pb.JobOutput()
     with open(
         Path(__file__).parent / "answers" / "cisno_casci_result.pbmsg", "rb"
     ) as f:
```

### Comparing `tcpb-0.8.1/tests/test_ci_overlap.py` & `tcpb-0.9.0/tests/test_ci_overlap.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/tests/test_cisno_casci.py` & `tcpb-0.9.0/tests/test_cisno_casci.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/tests/test_data/water.molden` & `tcpb-0.9.0/tests/test_data/water.molden`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/tests/test_fomo_casci.py` & `tcpb-0.9.0/tests/test_fomo_casci.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+import pytest
+
 from tcpb import TCProtobufClient as TCPBClient
 
 from .answers import fomo_casci
 from .conftest import _round
 
 
+@pytest.mark.skip(
+    "Fails for reasons internal to TeraChem. It appears this method causes TeraChem (or the PBS?) to return"
+    "vastly different results than previously. See https://github.com/mtzgroup/terachem/issues/139"
+)
 def test_fomo_casci(settings, ethylene):
 
     with TCPBClient(host=settings["tcpb_host"], port=settings["tcpb_port"]) as TC:
         options = {
             "method": "hf",
             "basis": "6-31g**",
             "atoms": ethylene["atoms"],
```

### Comparing `tcpb-0.8.1/tests/test_keywords.py` & `tcpb-0.9.0/tests/test_keywords.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,28 +3,14 @@
 import pytest
 from numpy import ndarray
 from qcelemental.models import AtomicInput
 
 from tcpb import TCProtobufClient as TCPBClient
 
 
-def test_molden_file_creation(settings, atomic_input, test_data_dir):
-    # Add molden keywords
-    atomic_input.keywords.update({"mo_output": True, "molden": True})
-    with TCPBClient(settings["tcpb_host"], settings["tcpb_port"]) as TC:
-        result = TC.compute(atomic_input)
-
-    with open(test_data_dir / "water.molden") as f:
-        correct_molden = f.read()
-
-    with open("output.molden", "w") as f:
-        f.write(result.extras["molden"])
-    assert result.extras["molden"] == correct_molden
-
-
 @pytest.mark.skip(
     reason="You can see in the tc.in/out files the convergence is set correctly. Yes a"
     "looser convergence doesn't always produce a shorter computation time."
 )
 def test_convthre(settings, atomic_input):
     atomic_input.keywords["convthre"] = 3.0e-5
     with TCPBClient(settings["tcpb_host"], settings["tcpb_port"]) as client:
```

### Comparing `tcpb-0.8.1/tests/test_utils.py` & `tcpb-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tcpb-0.8.1/PKG-INFO` & `tcpb-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcpb
-Version: 0.8.1
+Version: 0.9.0
 Summary: Protobuf client for TeraChem server mode
 Home-page: https://github.com/mtzgroup/tcpb-client
 Author: Colton Hicks
 Author-email: mtzgroupadmin@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
@@ -28,14 +28,15 @@
 Requires-Dist: qcelemental>=0.24.0
 Requires-Dist: httpx>=0.22.0
 Requires-Dist: flake8 >=3.8.4 ; extra == "dev"
 Requires-Dist: pre-commit >= 2.9.3 ; extra == "dev"
 Requires-Dist: autoflake >= 1.4 ; extra == "dev"
 Requires-Dist: pytest >=6.2.1 ; extra == "test"
 Requires-Dist: pytest-cov >=2.10.1,<3.0.0 ; extra == "test"
+Requires-Dist: pytest-mock>=3.6.1 ; extra == "test"
 Requires-Dist: coverage >=5.3.1,<6.0 ; extra == "test"
 Requires-Dist: mypy ==0.790 ; extra == "test"
 Requires-Dist: black >=20.8b1,<21.0b0 ; extra == "test"
 Requires-Dist: isort >=5.7.0,<6.0.0 ; extra == "test"
 Provides-Extra: dev
 Provides-Extra: test
```

