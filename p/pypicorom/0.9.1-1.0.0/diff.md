# Comparing `tmp/pypicorom-0.9.1.tar.gz` & `tmp/pypicorom-1.0.0.tar.gz`

## Comparing `pypicorom-0.9.1.tar` & `pypicorom-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 pypicorom-0.9.1/local_dependencies/picolink/Cargo.toml
--rw-r--r--   0     1001      123    12985 2023-07-15 05:39:16.000000 pypicorom-0.9.1/local_dependencies/picolink/src/lib.rs
--rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 pypicorom-0.9.1/Cargo.toml
--rw-r--r--   0     1001      123      325 2023-07-15 05:39:16.000000 pypicorom-0.9.1/.env/pyvenv.cfg
--rw-r--r--   0     1001      123     2807 2023-07-15 05:39:16.000000 pypicorom-0.9.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-07-15 05:39:16.000000 pypicorom-0.9.1/.gitignore
--rw-r--r--   0     1001      123      370 2023-07-15 05:39:16.000000 pypicorom-0.9.1/pyproject.toml
--rw-r--r--   0     1001      123     5066 2023-07-15 05:39:16.000000 pypicorom-0.9.1/src/lib.rs
--rw-r--r--   0     1001      123    12290 2023-07-15 05:39:24.000000 pypicorom-0.9.1/Cargo.lock
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pypicorom-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 pypicorom-1.0.0/local_dependencies/picolink/Cargo.toml
+-rw-r--r--   0     1001      123    13197 2023-07-26 17:50:34.000000 pypicorom-1.0.0/local_dependencies/picolink/src/lib.rs
+-rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 pypicorom-1.0.0/Cargo.toml
+-rw-r--r--   0     1001      123      325 2023-07-26 17:50:34.000000 pypicorom-1.0.0/.env/pyvenv.cfg
+-rw-r--r--   0     1001      123     2807 2023-07-26 17:50:34.000000 pypicorom-1.0.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-07-26 17:50:34.000000 pypicorom-1.0.0/.gitignore
+-rw-r--r--   0     1001      123      370 2023-07-26 17:50:34.000000 pypicorom-1.0.0/pyproject.toml
+-rw-r--r--   0     1001      123     5224 2023-07-26 17:50:34.000000 pypicorom-1.0.0/src/lib.rs
+-rw-r--r--   0     1001      123    12291 2023-07-26 17:50:38.000000 pypicorom-1.0.0/Cargo.lock
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pypicorom-1.0.0/PKG-INFO
```

### Comparing `pypicorom-0.9.1/local_dependencies/picolink/src/lib.rs` & `pypicorom-1.0.0/local_dependencies/picolink/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     CommitFlash = 12,
     CommitDone = 13,
 
     CommsStart = 80,
     CommsEnd = 81,
     CommsData = 82,
 
+    Identify = 0xf8,
     Error = 0xfe,
     Debug = 0xff,
 }
 
 #[derive(Clone, Debug)]
 pub enum ReqPacket {
     Ident,
@@ -45,14 +46,15 @@
     MaskGet,
     Write(Vec<u8>),
     Read,
     CommitFlash,
     CommsStart(u32),
     CommsEnd,
     CommsData(Vec<u8>),
+    Identify,
 }
 
 impl ReqPacket {
     fn encode(self) -> Result<Vec<u8>> {
         let (kind, payload) = match self.clone() {
             ReqPacket::Ident => (PacketKind::IdentReq, vec![]),
             ReqPacket::IdentSet(name) => (PacketKind::IdentSet, name.as_bytes().to_vec()),
@@ -64,14 +66,15 @@
             ReqPacket::MaskGet => (PacketKind::MaskGet, vec![]),
             ReqPacket::Write(data) => (PacketKind::Write, data),
             ReqPacket::Read => (PacketKind::Read, vec![]),
             ReqPacket::CommitFlash => (PacketKind::CommitFlash, vec![]),
             ReqPacket::CommsStart(addr) => (PacketKind::CommsStart, addr.to_le_bytes().to_vec()),
             ReqPacket::CommsEnd => (PacketKind::CommsEnd, vec![]),
             ReqPacket::CommsData(data) => (PacketKind::CommsData, data),
+            ReqPacket::Identify => (PacketKind::Identify, vec![]),
         };
 
         if payload.len() > 30 {
             return Err(anyhow!("{:?} request packet payload too large", self));
         }
 
         let mut data = Vec::with_capacity(32);
@@ -373,14 +376,19 @@
                 RespPacket::CommitDone => Some(()),
                 _ => None,
             },
             Duration::from_secs(5),
         )
     }
 
+    pub fn identify(&mut self) -> Result<()> {
+        self.send(ReqPacket::Identify)?;
+        Ok(())
+    }
+
     pub fn poll_comms(&mut self, outgoing: Option<Vec<u8>>) -> Result<Vec<u8>> {
         let mut incoming = Vec::new();
         if let Some(outgoing) = outgoing {
             for chunk in outgoing.chunks(30) {
                 while let Some(pkt) = self.recv(Instant::now())? {
                     match pkt {
                         RespPacket::CommsData(data) => {
```

### Comparing `pypicorom-0.9.1/.github/workflows/CI.yml` & `pypicorom-1.0.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pypicorom-0.9.1/.gitignore` & `pypicorom-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pypicorom-0.9.1/src/lib.rs` & `pypicorom-1.0.0/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,21 @@
     /// Commit the current ROM data to flash memory
     fn commit(&mut self) -> PyResult<()> {
         self.comms_inactive()?;
 
         Ok(self.link.commit_rom()?)
     }
 
+    /// Ask PicoROM to identify itself
+    fn identify(&mut self) -> PyResult<()> {
+        self.comms_inactive()?;
+
+        Ok(self.link.identify()?)
+    }
+
     /// Upload ROM data
     #[pyo3(signature = (data, mask=0x3ffff), text_signature = "(data, mask=0x3ffff, /)")]
     fn upload(&mut self, data: &[u8], mask: u32) -> PyResult<()> {
         self.comms_inactive()?;
 
         self.link.upload(data, mask, |_| {})?;
```

### Comparing `pypicorom-0.9.1/Cargo.lock` & `pypicorom-1.0.0/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.71"
+version = "1.0.72"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+checksum = "3b13c32d80ecc7ab747b80c3784bce54ee8a7a0cc4fbda9bf4cda2cf6fe90854"
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
@@ -133,22 +133,22 @@
 name = "num-derive"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e6a0fd4f737c707bd9086cc16c925f294943eb62eb71499e9fd4cf71f8b9f4e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.26",
+ "syn 2.0.27",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.18.0"
@@ -176,27 +176,27 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "picolink"
-version = "0.9.0"
+version = "1.0.0"
 dependencies = [
  "anyhow",
  "num-derive",
  "num-traits",
  "serialport",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.64"
+version = "1.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
+checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.19.1"
@@ -256,25 +256,25 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pypicorom"
-version = "0.9.1"
+version = "1.0.0"
 dependencies = [
  "picolink",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.29"
+version = "1.0.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
+checksum = "50f3b39ccfb720540debaa0164757101c08ecb8d326b15358ce76a62c7e85965"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.3.5"
@@ -311,17 +311,17 @@
 name = "regex-syntax"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5ea92a5b6195c6ef2a0295ea818b312502c6fc94dde986c5553242e18fd4ce2"
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serialport"
 version = "4.2.2-alpha.0"
 source = "git+https://github.com/wickerwaka/serialport-rs.git?rev=c14ea8611834c39390a02f0eec3efb51fc576712#c14ea8611834c39390a02f0eec3efb51fc576712"
 dependencies = [
  "CoreFoundation-sys",
@@ -356,34 +356,34 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.26"
+version = "2.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "45c3457aacde3c65315de5031ec191ce46604304d2446e803d71ade03308d970"
+checksum = "b60f673f44a8255b9c8c657daf66a596d435f2da81a555b06dc644d080ba45e0"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.9"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22049a19f4a68748a168c0fc439f9516686aa045927ff767eca0a85101fb6e73"
+checksum = "301abaae475aa91687eb82514b328ab47a211a533026cb25fc3e519b86adfc3c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
```

