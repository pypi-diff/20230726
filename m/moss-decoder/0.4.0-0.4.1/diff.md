# Comparing `tmp/moss_decoder-0.4.0.tar.gz` & `tmp/moss_decoder-0.4.1.tar.gz`

## Comparing `moss_decoder-0.4.0.tar` & `moss_decoder-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 moss_decoder-0.4.0/Cargo.toml
--rw-r--r--   0     1001      123      601 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/.CERN-gitlab-ci.yml
--rw-r--r--   0     1001      123     2835 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      714 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/.gitignore
--rw-r--r--   0     1001      123      757 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0     1001      123     2800 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/README.md
--rw-r--r--   0     1001      123      560 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/moss_decoder.pyi
--rw-r--r--   0     1001      123      641 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/pyproject.toml
--rw-r--r--   0     1001      123  4458776 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/python310.dll
--rw-r--r--   0     1001      123     8390 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/src/lib.rs
--rw-r--r--   0     1001      123     1880 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/src/moss_protocol/moss_hit.rs
--rw-r--r--   0     1001      123     1843 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/src/moss_protocol/moss_packet.rs
--rw-r--r--   0     1001      123     1668 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/src/moss_protocol.rs
--rwxr-xr-x   0     1001      123      427 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/bench_dev_vs_prod.sh
--rw-r--r--   0     1001      123     7098 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/integration.py
--rw-r--r--   0     1001      123     4858 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/integration_test.rs
--rw-r--r--   0     1001      123  9582576 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/moss_noise.raw
--rwxr-xr-x   0     1001      123     1156 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/performance_dev_py.sh
--rwxr-xr-x   0     1001      123      820 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/performance_prod_py.sh
--rw-r--r--   0     1001      123      895 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/tests/utils.sh
--rw-r--r--   0     1001      123     8066 2023-07-25 14:51:03.000000 moss_decoder-0.4.0/Cargo.lock
--rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 moss_decoder-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 moss_decoder-0.4.1/Cargo.toml
+-rw-r--r--   0     1001      123      591 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/.CERN-gitlab-ci.yml
+-rw-r--r--   0     1001      123     2835 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      714 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/.gitignore
+-rw-r--r--   0     1001      123      757 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0     1001      123     2800 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/README.md
+-rw-r--r--   0     1001      123      560 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/moss_decoder.pyi
+-rw-r--r--   0     1001      123      641 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/pyproject.toml
+-rw-r--r--   0     1001      123  4458776 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/python310.dll
+-rw-r--r--   0     1001      123     8969 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/src/lib.rs
+-rw-r--r--   0     1001      123     1880 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/src/moss_protocol/moss_hit.rs
+-rw-r--r--   0     1001      123     1843 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/src/moss_protocol/moss_packet.rs
+-rw-r--r--   0     1001      123     1674 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/src/moss_protocol.rs
+-rwxr-xr-x   0     1001      123      427 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/tests/bench_dev_vs_prod.sh
+-rw-r--r--   0     1001      123     7098 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/tests/integration.py
+-rw-r--r--   0     1001      123     5822 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/tests/integration_test.rs
+-rw-r--r--   0     1001      123  9582576 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/tests/moss_noise.raw
+-rwxr-xr-x   0     1001      123     1156 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/tests/performance_dev_py.sh
+-rwxr-xr-x   0     1001      123      820 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/tests/performance_prod_py.sh
+-rw-r--r--   0     1001      123      895 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/tests/utils.sh
+-rw-r--r--   0     1001      123     8066 2023-07-26 07:22:16.000000 moss_decoder-0.4.1/Cargo.lock
+-rw-r--r--   0        0        0     3354 1970-01-01 00:00:00.000000 moss_decoder-0.4.1/PKG-INFO
```

### Comparing `moss_decoder-0.4.0/Cargo.toml` & `moss_decoder-0.4.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "moss_decoder"
-version = "0.4.0"
+version = "0.4.1"
 edition = "2021"
 authors = ["Marc Beck König <mbkj@tutamail.com>"]
 license = "MIT OR Apache-2.0"
 description = "Python module providing a decoder for the MOSS chip protocol."
 categories = ["python-module"]
```

### Comparing `moss_decoder-0.4.0/.CERN-gitlab-ci.yml` & `moss_decoder-0.4.1/.CERN-gitlab-ci.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 variables:
-    DOCKER_REGISTRY: "gitlab-registry.cern.ch/alice-its3-wp3/moss-testing/docker/python-rust"
+    DOCKER_REGISTRY: "gitlab-registry.cern.ch/alice-its3-wp3/moss-testing/docker"
 
 stages:
     - build
 
 default:
     before_script:
         - hostname -I
@@ -16,15 +16,15 @@
 
 build-centos:
     stage: build
     when: manual
     needs: []
     dependencies: []
     cache: []
-    image: ${DOCKER_REGISTRY}/fpga-lint
+    image: ${DOCKER_REGISTRY}/python-rust
     script:
         - python -m pip install maturin
         - maturin build --release
     artifacts:
         name: "${CI_COMMIT_SHA}"
         paths:
         - $CI_PROJECT_DIR/target/
```

### Comparing `moss_decoder-0.4.0/.github/workflows/CI.yml` & `moss_decoder-0.4.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/.gitignore` & `moss_decoder-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/.pre-commit-config.yaml` & `moss_decoder-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/README.md` & `moss_decoder-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/moss_decoder.pyi` & `moss_decoder-0.4.1/moss_decoder.pyi`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/pyproject.toml` & `moss_decoder-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/python310.dll` & `moss_decoder-0.4.1/python310.dll`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/src/lib.rs` & `moss_decoder-0.4.1/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -94,22 +94,20 @@
 
     if byte_cnt < 6 {
         return Err(PyValueError::new_err(
             "Received less than the minimum event size",
         ));
     }
 
-    let (moss_packet, trailer_idx) = if let Ok((moss_packet, trailer_idx)) = raw_decode_event(bytes)
-    {
-        (moss_packet, trailer_idx)
-    } else {
-        return Err(PyAssertionError::new_err("No MOSS Packets in event"));
-    };
-
-    Ok((moss_packet, trailer_idx))
+    match raw_decode_event(bytes) {
+        Ok((moss_packet, trailer_idx)) => Ok((moss_packet, trailer_idx)),
+        Err(e) => Err(PyAssertionError::new_err(format!(
+            "No MOSS packet found: {e}",
+        ))),
+    }
 }
 
 /// Decodes a single MOSS event into a [MossPacket] and the index of the trailer byte.
 /// This function does not return an error if no MOSS packet is found, instead the last_trailer_idx is returned as 0.
 /// In the case no MOSS packet is found, the a `MossPacket` is still returned with default values which is unit ID 0
 /// and no hits, but this result is invalid and should be discarded.
 #[pyfunction]
@@ -174,15 +172,15 @@
         Err(PyAssertionError::new_err("No MOSS Packets in events"))
     } else {
         Ok(moss_packets)
     }
 }
 
 /// Decodes a single MOSS event into a [MossPacket] and the index of the trailer byte (Rust only)
-fn raw_decode_event(bytes: &[u8]) -> Result<(MossPacket, usize), ()> {
+fn raw_decode_event(bytes: &[u8]) -> std::io::Result<(MossPacket, usize)> {
     let mut moss_packet = MossPacket {
         unit_id: INVALID_NO_HEADER_SEEN, // placeholder
         hits: Vec::new(),
     };
 
     let mut trailer_idx = 0;
     let mut current_region: u8 = 0xff; // placeholder
@@ -232,15 +230,31 @@
                 debug_assert!(is_moss_packet);
                 moss_packet.hits.last_mut().unwrap().column |= (*byte & 0x3F) as u16;
                 // col position [5:0]
             }
             MossWord::Delimiter => {
                 debug_assert!(!is_moss_packet);
             }
+            MossWord::ProtocolError => {
+                let describe_decode_state = if is_moss_packet {
+                    "in MOSS packet"
+                } else {
+                    "before header seen"
+                };
+                return Err(std::io::Error::new(
+                    std::io::ErrorKind::InvalidData,
+                    format!(
+                        "Protocol error {describe_decode_state}, at index {i} with byte {byte:#X} "
+                    ),
+                ));
+            }
         }
     }
     if moss_packet.unit_id == INVALID_NO_HEADER_SEEN || trailer_idx == 0 {
-        Err(())
+        Err(std::io::Error::new(
+            std::io::ErrorKind::NotFound,
+            "No MOSS packet found",
+        ))
     } else {
         Ok((moss_packet, trailer_idx))
     }
 }
```

### Comparing `moss_decoder-0.4.0/src/moss_protocol/moss_hit.rs` & `moss_decoder-0.4.1/src/moss_protocol/moss_hit.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/src/moss_protocol/moss_packet.rs` & `moss_decoder-0.4.1/src/moss_protocol/moss_packet.rs`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/src/moss_protocol.rs` & `moss_decoder-0.4.1/src/moss_protocol.rs`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     UnitFrameHeader,
     UnitFrameTrailer,
     RegionHeader,
     Data0,
     Data1,
     Data2,
     Delimiter,
+    ProtocolError,
 }
 
 impl MossWord {
     const IDLE: u8 = 0xFF; // 1111_1111 (default)
     const UNIT_FRAME_HEADER: u8 = 0b1101_0000; // 1101_<unit_id[3:0]>
     const UNIT_FRAME_TRAILER: u8 = 0b1110_0000; // 1110_0000
     const REGION_HEADER: u8 = 0b1100_0000; // 1100_00_<region_id[1:0]>
@@ -33,11 +34,11 @@
             Self::UNIT_FRAME_TRAILER => MossWord::UnitFrameTrailer,
             six_msb if six_msb & 0xFC == Self::REGION_HEADER => MossWord::RegionHeader,
             four_msb if four_msb & 0xF0 == Self::UNIT_FRAME_HEADER => MossWord::UnitFrameHeader,
             Self::DELIMITER => Self::Delimiter,
             two_msb if two_msb & 0b1100_0000 == Self::DATA_0 => MossWord::Data0,
             two_msb if two_msb & 0b1100_0000 == Self::DATA_1 => MossWord::Data1,
             two_msb if two_msb & 0b1100_0000 == Self::DATA_2 => MossWord::Data2,
-            val => unreachable!("Unreachable: {val}"),
+            _ => MossWord::ProtocolError,
         }
     }
 }
```

### Comparing `moss_decoder-0.4.0/tests/integration.py` & `moss_decoder-0.4.1/tests/integration.py`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/tests/integration_test.rs` & `moss_decoder-0.4.1/tests/integration_test.rs`

 * *Files 10% similar despite different names*

```diff
@@ -100,14 +100,39 @@
         0b0101_1000, // row 3
         0b1000_0011, // col 3
         IDLE,
         UNIT_FRAME_TRAILER,
     ]
 }
 
+fn fake_event_protocol_error() -> Vec<u8> {
+    vec![
+        UNIT_FRAME_HEADER_0,
+        IDLE,
+        IDLE,
+        REGION_HEADER_0,
+        // Hit row 2, col 8
+        0x00,
+        0xF0, // Protocol error
+        0x88,
+        REGION_HEADER_1,
+        // Hit row 301, col 433
+        0x25,
+        0x6E,
+        0xB1,
+        REGION_HEADER_2,
+        REGION_HEADER_3,
+        // Hit row 2, col 8
+        0x00,
+        0x50,
+        0x88,
+        UNIT_FRAME_TRAILER,
+    ]
+}
+
 #[test]
 fn test_decoding_single_event() {
     //
     let event = fake_event_simple();
 
     let (packet, last_trailer_idx) = decode_event(&event).unwrap();
 
@@ -202,7 +227,26 @@
     assert_eq!(
         packets.len(),
         100000,
         "Expected 100k packets, got {}",
         packets.len()
     );
 }
+
+#[test]
+fn test_decode_protocol_error() {
+    pyo3::prepare_freethreaded_python();
+
+    let event = fake_event_protocol_error();
+
+    match decode_event(&event) {
+        Ok(_) => {
+            panic!("This packet has a protocol error, but it was not detected!")
+        }
+        Err(e) if e.to_string().contains("Protocol error") => {
+            println!("Got expected error: {e}");
+        }
+        Err(e) => {
+            panic!("Got unexpected error: {e}");
+        }
+    }
+}
```

### Comparing `moss_decoder-0.4.0/tests/moss_noise.raw` & `moss_decoder-0.4.1/tests/moss_noise.raw`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/tests/performance_dev_py.sh` & `moss_decoder-0.4.1/tests/performance_dev_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/tests/performance_prod_py.sh` & `moss_decoder-0.4.1/tests/performance_prod_py.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/tests/utils.sh` & `moss_decoder-0.4.1/tests/utils.sh`

 * *Files identical despite different names*

### Comparing `moss_decoder-0.4.0/Cargo.lock` & `moss_decoder-0.4.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "moss_decoder"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "pretty_assertions",
  "pyo3",
 ]
 
 [[package]]
 name = "once_cell"
```

### Comparing `moss_decoder-0.4.0/PKG-INFO` & `moss_decoder-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moss_decoder
-Version: 0.4.0
+Version: 0.4.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python package implemented in Rust to decode MOSS readout data
 Author: Marc Beck König
 Author-email: marc.beck.konig@cern.ch
 Maintainer-email: Marc Beck König <marc.beck.konig@cern.ch>
```

