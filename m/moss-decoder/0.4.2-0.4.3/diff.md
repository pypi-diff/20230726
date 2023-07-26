# Comparing `tmp/moss_decoder-0.4.2.tar.gz` & `tmp/moss_decoder-0.4.3.tar.gz`

## Comparing `moss_decoder-0.4.2.tar` & `moss_decoder-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 moss_decoder-0.4.2/Cargo.toml
--rw-r--r--   0     1001      123      633 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/.CERN-gitlab-ci.yml
--rw-r--r--   0     1001      123     2835 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      373 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/.github/workflows/bench-py.yml
--rw-r--r--   0     1001      123      404 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/.github/workflows/rust.yml
--rw-r--r--   0     1001      123      714 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/.gitignore
--rw-r--r--   0     1001      123      757 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     3100 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/README.md
--rw-r--r--   0     1001      123      560 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/moss_decoder.pyi
--rw-r--r--   0     1001      123      641 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/pyproject.toml
--rw-r--r--   0     1001      123  4458776 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/python310.dll
--rw-r--r--   0     1001      123     9630 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/src/lib.rs
--rw-r--r--   0     1001      123     1880 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/src/moss_protocol/moss_hit.rs
--rw-r--r--   0     1001      123     1843 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/src/moss_protocol/moss_packet.rs
--rw-r--r--   0     1001      123     1674 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/src/moss_protocol.rs
--rwxr-xr-x   0     1001      123      427 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/tests/bench_dev_vs_prod.sh
--rw-r--r--   0     1001      123     7098 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/tests/integration.py
--rw-r--r--   0     1001      123     6118 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/tests/integration_test.rs
--rw-r--r--   0     1001      123  9582576 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/tests/moss_noise.raw
--rwxr-xr-x   0     1001      123     1190 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/tests/performance_dev_py.sh
--rwxr-xr-x   0     1001      123      820 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/tests/performance_prod_py.sh
--rw-r--r--   0     1001      123      895 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/tests/utils.sh
--rw-r--r--   0     1001      123     8066 2023-07-26 14:43:56.000000 moss_decoder-0.4.2/Cargo.lock
--rw-r--r--   0        0        0     3654 1970-01-01 00:00:00.000000 moss_decoder-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 moss_decoder-0.4.3/Cargo.toml
+-rw-r--r--   0     1001      123      633 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/.CERN-gitlab-ci.yml
+-rw-r--r--   0     1001      123     2835 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      373 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/.github/workflows/bench-py.yml
+-rw-r--r--   0     1001      123      404 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/.github/workflows/rust.yml
+-rw-r--r--   0     1001      123      714 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/.gitignore
+-rw-r--r--   0     1001      123      757 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     3100 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/README.md
+-rw-r--r--   0     1001      123      874 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/moss_decoder.pyi
+-rw-r--r--   0     1001      123      641 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/pyproject.toml
+-rw-r--r--   0     1001      123  4458776 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/python310.dll
+-rw-r--r--   0     1001      123     9630 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/src/lib.rs
+-rw-r--r--   0     1001      123     1880 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/src/moss_protocol/moss_hit.rs
+-rw-r--r--   0     1001      123     1843 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/src/moss_protocol/moss_packet.rs
+-rw-r--r--   0     1001      123     1674 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/src/moss_protocol.rs
+-rwxr-xr-x   0     1001      123      427 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/bench_dev_vs_prod.sh
+-rw-r--r--   0     1001      123     7102 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/integration.py
+-rw-r--r--   0     1001      123     6118 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/integration_test.rs
+-rw-r--r--   0     1001      123  9582576 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/moss_noise.raw
+-rwxr-xr-x   0     1001      123     1190 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/performance_dev_py.sh
+-rwxr-xr-x   0     1001      123      820 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/performance_prod_py.sh
+-rw-r--r--   0     1001      123      895 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/tests/utils.sh
+-rw-r--r--   0     1001      123     8066 2023-07-26 15:05:22.000000 moss_decoder-0.4.3/Cargo.lock
+-rw-r--r--   0        0        0     3654 1970-01-01 00:00:00.000000 moss_decoder-0.4.3/PKG-INFO
```

### Comparing `moss_decoder-0.4.2/.CERN-gitlab-ci.yml` & `moss_decoder-0.4.3/.CERN-gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/.github/workflows/CI.yml` & `moss_decoder-0.4.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/.gitignore` & `moss_decoder-0.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/.pre-commit-config.yaml` & `moss_decoder-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/README.md` & `moss_decoder-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/pyproject.toml` & `moss_decoder-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/python310.dll` & `moss_decoder-0.4.3/python310.dll`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/src/lib.rs` & `moss_decoder-0.4.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/src/moss_protocol/moss_hit.rs` & `moss_decoder-0.4.3/src/moss_protocol/moss_hit.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/src/moss_protocol/moss_packet.rs` & `moss_decoder-0.4.3/src/moss_protocol/moss_packet.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/src/moss_protocol.rs` & `moss_decoder-0.4.3/src/moss_protocol.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/tests/integration.py` & `moss_decoder-0.4.3/tests/integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Integration tests. Uses the `moss_decoder` package
 from python and allows benchmarks."""
 import sys  # Don't want to depend on `argparse`
 import time
 from pathlib import Path
 import moss_decoder
-from moss_decoder import MossPacket, decode_event, MossHit
+from moss_decoder import MossPacket, MossHit
+from moss_decoder import decode_event, decode_event_noexcept
 
 FILE_PATH = Path("tests/moss_noise.raw")
 
 
 def read_bytes_from_file(file_path: Path) -> bytes:
     """Open file at `file_path` and read as binary, return `bytes`"""
     with open(file_path, "rb") as readout_file:
@@ -144,17 +145,15 @@
                 more_data = False
                 raise exc
 
     if noexcept is True:
         res = 1
         packets = []
         while res != 0:
-            packet, res = moss_decoder.decode_event_noexcept(
-                raw_bytes[last_trailer_idx:]
-            )
+            packet, res = decode_event_noexcept(raw_bytes[last_trailer_idx:])
             if res != 0:
                 last_trailer_idx = last_trailer_idx + res + 1
                 packets.append(packet)
 
     last_trailer_idx = last_trailer_idx - 1
 
     print(f"Decoded {len(packets)} packets")
```

### Comparing `moss_decoder-0.4.2/tests/integration_test.rs` & `moss_decoder-0.4.3/tests/integration_test.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/tests/moss_noise.raw` & `moss_decoder-0.4.3/tests/moss_noise.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/tests/performance_dev_py.sh` & `moss_decoder-0.4.3/tests/performance_dev_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/tests/performance_prod_py.sh` & `moss_decoder-0.4.3/tests/performance_prod_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/tests/utils.sh` & `moss_decoder-0.4.3/tests/utils.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.2/Cargo.lock` & `moss_decoder-0.4.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "moss_decoder"
-version = "0.4.2"
+version = "0.4.3"
 dependencies = [
  "pretty_assertions",
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
```

### Comparing `moss_decoder-0.4.2/PKG-INFO` & `moss_decoder-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moss_decoder
-Version: 0.4.2
+Version: 0.4.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python package implemented in Rust to decode MOSS readout data
 Author: Marc Beck König
 Author-email: marc.beck.konig@cern.ch
 Maintainer-email: Marc Beck König <marc.beck.konig@cern.ch>
```

