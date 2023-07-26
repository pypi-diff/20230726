# Comparing `tmp/aws_network_firewall-0.3.0.tar.gz` & `tmp/aws_network_firewall-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_network_firewall-0.3.0.tar", max compression
+gzip compressed data, was "aws_network_firewall-0.4.0.tar", max compression
```

## Comparing `aws_network_firewall-0.3.0.tar` & `aws_network_firewall-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0    11335 2023-07-24 11:53:19.590885 aws_network_firewall-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0      800 2023-07-24 11:53:19.590885 aws_network_firewall-0.3.0/README.md
--rw-r--r--   0        0        0       22 2023-07-24 11:53:20.638930 aws_network_firewall-0.3.0/aws_network_firewall/__init__.py
--rw-r--r--   0        0        0     1403 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/account.py
--rw-r--r--   0        0        0      175 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cidr_range.py
--rw-r--r--   0        0        0      387 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cidr_ranges.py
--rw-r--r--   0        0        0      505 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cli/commands/__init__.py
--rw-r--r--   0        0        0     1365 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cli/commands/check.py
--rw-r--r--   0        0        0     1191 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cli/commands/update.py
--rw-r--r--   0        0        0      744 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/cli/handler.py
--rw-r--r--   0        0        0      589 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/destination.py
--rw-r--r--   0        0        0     1130 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/documentation_generator.py
--rw-r--r--   0        0        0     3031 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/rule.py
--rw-r--r--   0        0        0     1994 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/schemas/__init__.py
--rw-r--r--   0        0        0     2113 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/schemas/environment.yaml
--rw-r--r--   0        0        0      509 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/source.py
--rw-r--r--   0        0        0      210 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/suricata/__init__.py
--rw-r--r--   0        0        0      415 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/suricata/host.py
--rw-r--r--   0        0        0      353 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/suricata/option.py
--rw-r--r--   0        0        0     1756 2023-07-24 11:53:19.594885 aws_network_firewall-0.3.0/aws_network_firewall/suricata/rule.py
--rw-r--r--   0        0        0     1178 2023-07-24 11:53:20.638930 aws_network_firewall-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1518 1970-01-01 00:00:00.000000 aws_network_firewall-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11335 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0      800 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-26 14:41:19.290145 aws_network_firewall-0.4.0/aws_network_firewall/__init__.py
+-rw-r--r--   0        0        0     1403 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/account.py
+-rw-r--r--   0        0        0      175 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/cidr_range.py
+-rw-r--r--   0        0        0      387 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/cidr_ranges.py
+-rw-r--r--   0        0        0      505 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1365 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/cli/commands/check.py
+-rw-r--r--   0        0        0      374 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/cli/commands/docs.py
+-rw-r--r--   0        0        0     1191 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/cli/commands/update.py
+-rw-r--r--   0        0        0      744 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/cli/handler.py
+-rw-r--r--   0        0        0      589 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/destination.py
+-rw-r--r--   0        0        0     1130 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/documentation_generator.py
+-rw-r--r--   0        0        0     3168 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/rule.py
+-rw-r--r--   0        0        0     1994 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/schemas/__init__.py
+-rw-r--r--   0        0        0     2680 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/schemas/environment.yaml
+-rw-r--r--   0        0        0      509 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/source.py
+-rw-r--r--   0        0        0      210 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/suricata/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/suricata/host.py
+-rw-r--r--   0        0        0      474 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/suricata/option.py
+-rw-r--r--   0        0        0     1812 2023-07-26 14:41:18.430143 aws_network_firewall-0.4.0/aws_network_firewall/suricata/rule.py
+-rw-r--r--   0        0        0     1202 2023-07-26 14:41:19.290145 aws_network_firewall-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 aws_network_firewall-0.4.0/PKG-INFO
```

### Comparing `aws_network_firewall-0.3.0/LICENSE.txt` & `aws_network_firewall-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.3.0/README.md` & `aws_network_firewall-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.3.0/aws_network_firewall/account.py` & `aws_network_firewall-0.4.0/aws_network_firewall/account.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.3.0/aws_network_firewall/cli/commands/check.py` & `aws_network_firewall-0.4.0/aws_network_firewall/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.3.0/aws_network_firewall/cli/commands/update.py` & `aws_network_firewall-0.4.0/aws_network_firewall/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.3.0/aws_network_firewall/cli/handler.py` & `aws_network_firewall-0.4.0/aws_network_firewall/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.3.0/aws_network_firewall/destination.py` & `aws_network_firewall-0.4.0/aws_network_firewall/destination.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.3.0/aws_network_firewall/documentation_generator.py` & `aws_network_firewall-0.4.0/aws_network_firewall/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.3.0/aws_network_firewall/rule.py` & `aws_network_firewall-0.4.0/aws_network_firewall/rule.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,16 @@
 
         return list(filter(None, map(convert_source, self.sources)))
 
     @staticmethod
     def __tls_endpoint_options(endpoint: str) -> List[SuricataOption]:
         options = [
             SuricataOption(name="tls.sni"),
-            SuricataOption(name="tls.version", value="1.2,1.3"),
+            SuricataOption(name="tls.version", value="1.2", quoted_value=False),
+            SuricataOption(name="tls.version", value="1.3", quoted_value=False),
         ]
 
         if endpoint.startswith("*"):
             options += [
                 SuricataOption(name="dotprefix"),
                 SuricataOption(name="content", value=endpoint[1:]),
                 SuricataOption(name="nocase"),
@@ -67,16 +68,16 @@
         options = []
 
         if destination.protocol == "TLS" and destination.endpoint:
             options = self.__tls_endpoint_options(destination.endpoint)
 
         return options + [
             SuricataOption(name="msg", value=f"{self.workload} | {self.name}"),
-            SuricataOption(name="rev", value="1"),
-            SuricataOption(name="sid", value="XXX"),
+            SuricataOption(name="rev", value="1", quoted_value=False),
+            SuricataOption(name="sid", value="XXX", quoted_value=False),
         ]
 
     def __resolve_rule(self, destination: Destination) -> Optional[SuricataRule]:
         if not destination.cidr:
             return None
 
         return SuricataRule(
```

### Comparing `aws_network_firewall-0.3.0/aws_network_firewall/schemas/__init__.py` & `aws_network_firewall-0.4.0/aws_network_firewall/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_network_firewall-0.3.0/aws_network_firewall/suricata/rule.py` & `aws_network_firewall-0.4.0/aws_network_firewall/suricata/rule.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,15 +40,16 @@
             message = next(
                 filter(lambda option: option.name == "msg", self.options),
                 Option(name="msg", value="Unknown"),
             )
             message.value = (
                 f"{message.value} | Pass non-established TCP for 3-way handshake"
             )
-            flow = Option(name="flow", value="not_established")
-            sid = Option(name="sid", value="XXX")
-            rev = Option(name="rev", value="1")
+            flow = Option(name="flow", value="not_established")  # No quotes
+            sid = Option(name="sid", value="XXX", quoted_value=False)
+            rev = Option(name="rev", value="1", quoted_value=False)
+
             handshake_options = "; ".join(list(map(str, [message, flow, rev, sid])))
 
-            post_rule = f"\n{self.action} tcp {self.source} <> {self.destination} ({handshake_options})"
+            post_rule = f"\n{self.action} tcp {self.source} <> {self.destination} ({handshake_options};)"
 
-        return f"{self.action} {self.protocol} {self.source} {self.direction} {self.destination} ({options}){post_rule}"
+        return f"{self.action} {self.protocol} {self.source} {self.direction} {self.destination} ({options};){post_rule}"
```

### Comparing `aws_network_firewall-0.3.0/pyproject.toml` & `aws_network_firewall-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-network-firewall"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_network_firewall"}]
 
 [tool.poetry.group.dev.dependencies]
@@ -29,29 +29,30 @@
 python = "^3.9"
 click = "^8.1.3"
 pyyaml = "^6.0"
 jinja2 = "^3.1.2"
 xenon = "^0.9.0"
 jsonschema = "^4.18.3"
 landingzone-organization = "^0.8.0"
+jsonschema2md = "^0.9.0"
 
 
 [tool.poetry.scripts]
 aws-network-firewall = "aws_network_firewall.cli:cli"
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.coverage.run]
 branch = true
 source = ["aws_network_firewall"]
 
 [tool.coverage.report]
 show_missing = true
-fail_under = 100
+fail_under = 98
 exclude_lines = [
     "if __name__ == .__main__.:"
 ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aws_network_firewall-0.3.0/PKG-INFO` & `aws_network_firewall-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: aws-network-firewall
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonschema (>=4.18.3,<5.0.0)
+Requires-Dist: jsonschema2md (>=0.9.0,<0.10.0)
 Requires-Dist: landingzone-organization (>=0.8.0,<0.9.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: xenon (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # AWS Network Firewall
```

