# Comparing `tmp/hades-core-0.0.1.tar.gz` & `tmp/hades-core-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hades-core-0.0.1.tar", last modified: Sun Jul 23 12:53:50 2023, max compression
+gzip compressed data, was "hades-core-0.0.2.tar", last modified: Wed Jul 26 14:07:14 2023, max compression
```

## Comparing `hades-core-0.0.1.tar` & `hades-core-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 12:53:50.343142 hades-core-0.0.1/
--rw-rw-rw-   0        0        0    11558 2023-07-14 08:35:39.000000 hades-core-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    15924 2023-07-23 12:53:50.342143 hades-core-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1788 2023-07-23 11:03:53.000000 hades-core-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 12:53:50.285143 hades-core-0.0.1/hades/
--rw-rw-rw-   0        0        0        0 2023-07-23 10:52:09.000000 hades-core-0.0.1/hades/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:53:50.301143 hades-core-0.0.1/hades/core/
--rw-rw-rw-   0        0        0     1057 2023-07-23 11:05:08.000000 hades-core-0.0.1/hades/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:53:50.304143 hades-core-0.0.1/hades/core/backtesting/
--rw-rw-rw-   0        0        0        0 2023-07-22 02:15:06.000000 hades-core-0.0.1/hades/core/backtesting/__init__.py
--rw-rw-rw-   0        0        0     2403 2023-07-21 13:33:51.000000 hades-core-0.0.1/hades/core/config.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:53:50.310143 hades-core-0.0.1/hades/core/exchange/
--rw-rw-rw-   0        0        0        0 2023-07-23 04:45:11.000000 hades-core-0.0.1/hades/core/exchange/__init__.py
--rw-rw-rw-   0        0        0    10610 2023-07-23 11:13:21.000000 hades-core-0.0.1/hades/core/exchange/binance.py
--rw-rw-rw-   0        0        0    11565 2023-07-23 11:13:45.000000 hades-core-0.0.1/hades/core/exchange/okx.py
--rw-rw-rw-   0        0        0      879 2023-07-23 11:04:06.000000 hades-core-0.0.1/hades/core/executor.py
--rw-rw-rw-   0        0        0     1295 2023-07-23 11:04:17.000000 hades-core-0.0.1/hades/core/messager.py
--rw-rw-rw-   0        0        0     1292 2023-07-21 13:34:06.000000 hades-core-0.0.1/hades/core/model.py
--rw-rw-rw-   0        0        0     2280 2023-07-23 11:04:28.000000 hades-core-0.0.1/hades/core/strategy.py
-drwxrwxrwx   0        0        0        0 2023-07-23 12:53:50.339145 hades-core-0.0.1/hades_core.egg-info/
--rw-rw-rw-   0        0        0    15924 2023-07-23 12:53:50.000000 hades-core-0.0.1/hades_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-07-23 12:53:50.000000 hades-core-0.0.1/hades_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 12:53:50.000000 hades-core-0.0.1/hades_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-23 12:53:50.000000 hades-core-0.0.1/hades_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-23 12:53:50.000000 hades-core-0.0.1/hades_core.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5492 2023-07-23 12:52:28.000000 hades-core-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-23 12:53:50.343142 hades-core-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:14.928542 hades-core-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 14:07:03.000000 hades-core-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-07-26 14:07:14.928542 hades-core-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-26 14:07:03.000000 hades-core-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:14.928542 hades-core-0.0.2/hades/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:14.928542 hades-core-0.0.2/hades/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:14.928542 hades-core-0.0.2/hades/core/backtesting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/backtesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:14.928542 hades-core-0.0.2/hades/core/exchange/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/exchange/binance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11279 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/exchange/okx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/messager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-26 14:07:03.000000 hades-core-0.0.2/hades/core/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:07:14.928542 hades-core-0.0.2/hades_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14855 2023-07-26 14:07:14.000000 hades-core-0.0.2/hades_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-26 14:07:14.000000 hades-core-0.0.2/hades_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:07:14.000000 hades-core-0.0.2/hades_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-26 14:07:14.000000 hades-core-0.0.2/hades_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 14:07:14.000000 hades-core-0.0.2/hades_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-26 14:07:03.000000 hades-core-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:07:14.928542 hades-core-0.0.2/setup.cfg
```

### Comparing `hades-core-0.0.1/LICENSE` & `hades-core-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `hades-core-0.0.1/PKG-INFO` & `hades-core-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,297 +1,262 @@
-Metadata-Version: 2.1
-Name: hades-core
-Version: 0.0.1
-Summary: cryptocurrency trading bot
-Author-email: Gary Guo <gary.guo.china@gmail.com>
-Maintainer-email: Gary Guo <gary.guo.china@gmail.com>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: Homepage, https://github.com/hades-trading/hades-core
-Keywords: okx,binance,cryptocurrency
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## Hades Bot
-
-binance/okx based, currently it can only support real time Tick/Bar/Order/Position live update and monitor. In `bot/strategies/sample` , created a simple strategy, doing nothing but send notification 
-![alt text](./doc/screenshot.png "Screen Shot")
-## How to start
-
-### 1. Setup Environment
-
-```shell
-python -m venv runtime
-runtime\Scripts\activate
-pip install -r requirements.txt
-# if requirements.txt not work
-pip3 install python-okx websockets requests binance-futures-connector schedule "uvicorn[standard]" fastapi pandas
-```
-
-### 2. Change Configuration
-
-copy `example.conf` and rename to `app.conf` , change parameter
-
-```ini
-[binance]
-apiKey           = apiKey
-secretKey        = secretKey
-
-[okx]
-apiKey           = apiKey
-secretKey        = secretKey
-passphrase       = passphrase
-ws_private       = wss://wsaws.okx.com:8443/ws/v5/private
-ws_public        = wss://wsaws.okx.com:8443/ws/v5/public
-ws_business      = wss://wsaws.okx.com:8443/ws/v5/business
-domain           = https://aws.okx.com
-useServerTime    = False
-
-[notification]
-token            = token
-prefix           = prefix
-period           = 8-23
-```
-
-### 3. Strategy
-implement your own Strategy (extends Strategy) and replace the strategy in `main.py`
-
-```shell
-python main.py
-```
-
-### 4. Deploy to PROD
-
-#### 4.1 Create /app and execute git clone
-
-```shell
-sudo -s
-mkdir /app
-chown user:user /app
-cd /app
-git clone git@github.com:Icefoxes/trading-bot.git .
-```
-#### 4.2 setup supervisor
-
-```shell
-pip3 install supervisor
-echo_supervisord_conf > /etc/supervisord.conf
-echo bot.ini >> /etc/supervisord.conf
-supervisord -c /etc/supervisord.conf
-supervisorctl start bot
-```
-
-## Planned feature
-- backtesting
-- ui to show backtesting
+Metadata-Version: 2.1
+Name: hades-core
+Version: 0.0.2
+Summary: cryptocurrency trading bot
+Author-email: Gary Guo <gary.guo.china@gmail.com>
+Maintainer-email: Gary Guo <gary.guo.china@gmail.com>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: Homepage, https://github.com/hades-trading/hades-core
+Keywords: okx,binance,cryptocurrency
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## Hades Bot
+
+binance/okx based, currently it can only support real time Tick/Bar/Order/Position live update and monitor. In `bot/strategies/sample` , created a simple strategy, doing nothing but send notification 
+![alt text](./doc/screenshot.png "Screen Shot")
+## How to start
+
+### 1. Setup Environment
+
+```shell
+python -m venv runtime
+runtime\Scripts\activate
+pip install -r requirements.txt
+# if requirements.txt not work
+pip3 install python-okx websockets requests binance-futures-connector
+```
+
+### 2. Change Configuration
+
+copy `example.conf` and rename to `app.conf` , change parameter
+
+```ini
+[binance]
+apiKey           = apiKey
+secretKey        = secretKey
+
+[okx]
+apiKey           = apiKey
+secretKey        = secretKey
+passphrase       = passphrase
+ws_private       = wss://wsaws.okx.com:8443/ws/v5/private
+ws_public        = wss://wsaws.okx.com:8443/ws/v5/public
+ws_business      = wss://wsaws.okx.com:8443/ws/v5/business
+domain           = https://aws.okx.com
+useServerTime    = False
+
+[notification]
+token            = token
+prefix           = prefix
+period           = 8-23
+```
```

### Comparing `hades-core-0.0.1/hades/core/__init__.py` & `hades-core-0.0.2/hades/core/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import logging
-
-from hades.core.config import TradeBotConf
-from hades.core.messager import Messager
-from hades.core.model import Order, Position, Tick, Bar, Balance, Trade
-from hades.core.strategy import Strategy, Exchange, Subscriber, ExchangeEnum
-from hades.core.exchange.binance import BinanceUMSubscriber
-from hades.core.exchange.okx import OkxSubscriber
-from hades.core.executor import TradeExecutor
-
-
-logging.basicConfig(filename='log.txt',
-                    format='%(asctime)s - %(levelname)s - %(name)s - %(funcName)s - %(message)s',
-                    level=logging.INFO)
-
-logging.getLogger('okx.websocket.WsClientProtocol').setLevel(logging.ERROR)
-
-__all__ = ['TradeBotConf',
-           'Messager',
-           'Strategy',
-           'Exchange',
-           'Subscriber',
-           'ExchangeEnum',
-           'BinanceUMSubscriber',
-           'OkxSubscriber',
-           'TradeExecutor',
-           'Order',
-           'Position',
-           'Tick',
-           'Bar',
-           'Trade',
-           'Balance']
-
+import logging
+
+from hades.core.config import TradeBotConf
+from hades.core.messager import Messager
+from hades.core.model import Order, Position, Tick, Bar, Balance, Trade
+from hades.core.strategy import Strategy, Exchange, Subscriber, ExchangeEnum
+from hades.core.exchange.binance import BinanceUMSubscriber
+from hades.core.exchange.okx import OkxSubscriber
+from hades.core.executor import TradeExecutor
+
+
+logging.basicConfig(filename='log.txt',
+                    format='%(asctime)s - %(levelname)s - %(name)s - %(funcName)s - %(message)s',
+                    level=logging.INFO)
+
+logging.getLogger('okx.websocket.WsClientProtocol').setLevel(logging.ERROR)
+
+__all__ = ['TradeBotConf',
+           'Messager',
+           'Strategy',
+           'Exchange',
+           'Subscriber',
+           'ExchangeEnum',
+           'BinanceUMSubscriber',
+           'OkxSubscriber',
+           'TradeExecutor',
+           'Order',
+           'Position',
+           'Tick',
+           'Bar',
+           'Trade',
+           'Balance']
+
```

### Comparing `hades-core-0.0.1/hades/core/config.py` & `hades-core-0.0.2/hades/core/config.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from configparser import ConfigParser
-from os import path
-import os
-
-BINANCE_API_KEY      = 'BINANCE_API_KEY'
-BINANCE_SECRET_KEY   = 'BINANCE_SECRET_KEY'
-
-NOTIFICATION_TOKEN  = 'NOTIFICATION_TOKEN'
-NOTIFICATION_PREFIX = 'NOTIFICATION_PREFIX'
-NOTIFICATION_PERIOD = 'NOTIFICATION_PERIOD'
-
-class TradeBotConf:
-    def __init__(self, conf: ConfigParser = None) -> None:
-        if not conf:
-            self.binance               = {}
-            self.binance['apiKey']     = os.environ.get(BINANCE_API_KEY)
-            self.binance['secretKey']  = os.environ.get(BINANCE_SECRET_KEY)
-            self.token                 = os.environ.get(NOTIFICATION_TOKEN)
-            self.prefix                = os.environ.get(NOTIFICATION_PREFIX)
-            self.period                = os.environ.get(NOTIFICATION_PERIOD)
-        else:
-            if conf.has_section('okx'):
-                self.okx                   = {}
-                self.okx['apiKey']         = conf['okx']['apiKey']
-                self.okx['secretKey']      = conf['okx']['secretKey']
-                self.okx['passphrase']     = conf['okx']['passphrase']
-                self.okx['ws_private']     = conf['okx']['ws_private']
-                self.okx['ws_public']      = conf['okx']['ws_public']
-                self.okx['ws_business']    = conf['okx']['ws_business']
-                self.okx['domain']         = conf['okx']['domain']
-                self.okx['useServerTime']  = conf.getboolean('okx', 'useServerTime')
-            if conf.has_section('binance'):
-                self.binance               = {}
-                self.binance['apiKey']     = conf['binance']['apiKey']
-                self.binance['secretKey']  = conf['binance']['secretKey']
-            if conf.has_section('notification'):
-                self.token                 = conf['notification']['token']
-                self.prefix                = conf['notification']['prefix']
-                self.period                = conf['notification']['period']
-        
-    
-    @staticmethod
-    def load():
-        parser = ConfigParser()
-        ROOT_DIR = os.path.abspath(os.curdir)
-        conf_file = path.join(ROOT_DIR, 'app.conf')
-        if path.exists(conf_file):
-            parser.read(conf_file, encoding='UTF-8')
-            return TradeBotConf(parser)
-        else:
-            return TradeBotConf()
+from configparser import ConfigParser
+from os import path
+import os
+
+BINANCE_API_KEY      = 'BINANCE_API_KEY'
+BINANCE_SECRET_KEY   = 'BINANCE_SECRET_KEY'
+
+NOTIFICATION_TOKEN  = 'NOTIFICATION_TOKEN'
+NOTIFICATION_PREFIX = 'NOTIFICATION_PREFIX'
+NOTIFICATION_PERIOD = 'NOTIFICATION_PERIOD'
+
+class TradeBotConf:
+    def __init__(self, conf: ConfigParser = None) -> None:
+        if not conf:
+            self.binance               = {}
+            self.binance['apiKey']     = os.environ.get(BINANCE_API_KEY)
+            self.binance['secretKey']  = os.environ.get(BINANCE_SECRET_KEY)
+            self.token                 = os.environ.get(NOTIFICATION_TOKEN)
+            self.prefix                = os.environ.get(NOTIFICATION_PREFIX)
+            self.period                = os.environ.get(NOTIFICATION_PERIOD)
+        else:
+            if conf.has_section('okx'):
+                self.okx                   = {}
+                self.okx['apiKey']         = conf['okx']['apiKey']
+                self.okx['secretKey']      = conf['okx']['secretKey']
+                self.okx['passphrase']     = conf['okx']['passphrase']
+                self.okx['ws_private']     = conf['okx']['ws_private']
+                self.okx['ws_public']      = conf['okx']['ws_public']
+                self.okx['ws_business']    = conf['okx']['ws_business']
+                self.okx['domain']         = conf['okx']['domain']
+                self.okx['useServerTime']  = conf.getboolean('okx', 'useServerTime')
+            if conf.has_section('binance'):
+                self.binance               = {}
+                self.binance['apiKey']     = conf['binance']['apiKey']
+                self.binance['secretKey']  = conf['binance']['secretKey']
+            if conf.has_section('notification'):
+                self.token                 = conf['notification']['token']
+                self.prefix                = conf['notification']['prefix']
+                self.period                = conf['notification']['period']
+        
+    
+    @staticmethod
+    def load():
+        parser = ConfigParser()
+        ROOT_DIR = os.path.abspath(os.curdir)
+        conf_file = path.join(ROOT_DIR, 'app.conf')
+        if path.exists(conf_file):
+            parser.read(conf_file, encoding='UTF-8')
+            return TradeBotConf(parser)
+        else:
+            return TradeBotConf()
```

### Comparing `hades-core-0.0.1/hades/core/exchange/okx.py` & `hades-core-0.0.2/hades/core/exchange/okx.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,286 +1,286 @@
-
-import asyncio
-import websockets
-from okx.websocket import WsUtils
-import okx.Trade as Trade
-import okx.Account as Account
-import okx.MarketData as Market
-
-from typing import List
-from datetime import datetime
-import json
-import logging
-
-from hades.core import TradeBotConf, Strategy, Exchange, Subscriber, Order, Position, Balance, Tick, Bar
-
-
-class OkxExchangeClient(Exchange):
-    def __init__(self,  conf: TradeBotConf) -> None:
-        self.conf = {
-            'api_key': conf.okx['apiKey'],
-            'api_secret_key': conf.okx['secretKey'],
-            'domain': conf.okx['domain'],
-            'passphrase': conf.okx['passphrase'],
-            'flag': '0'
-        }
-        self.tradeApi = Trade.TradeAPI(**self.conf)
-        self.accountApi = Account.AccountAPI(**self.conf)
-        self.marketApi = Market.MarketAPI(**self.conf)
-    # Account Info
-    def get_positions(self) -> List[Position]:
-        response = self.accountApi.get_positions()
-        if response.get('code') == '0' and response.get('data') and len(response['data']) > 0:
-            return to_okx_position(response['data']) 
-        return []
-
-    def get_balance(self):
-        return self.accountApi.get_account_balance()
-    # Trade Info
-    def get_orders(self) -> List[Order]:
-        response = self.tradeApi.get_order_list()
-        if response.get('code') == '0' and response.get('data') and len(response['data']) > 0:
-            return to_okx_order(response['data']) 
-        return []
-    
-    def place_buy_order(self, symbol: str, size: float, price: float):
-        return self.tradeApi.place_order(instId=symbol, tdMode='isolated', side='buy', sz=str(size), px=str(price), ordType='post_only')
-    
-    def place_sell_order(self, symbol: str, size: float, price: float):
-        return self.tradeApi.place_order(instId=symbol, tdMode='isolated', side='sell', sz=str(size), px=str(price), ordType='post_only')
-    
-    def cancel_order(self, orderId: str, symbol: str):
-        return self.tradeApi.cancel_order(instId=symbol, ordId=orderId)
-    
-    def close_position(self, symbol: str):
-        return self.tradeApi.close_positions(instId=symbol, mgnMode='isolated')
-
-    # get latest 100 bar
-    def get_candlesticks(self, symbol: str, bar: str = '1m', limit: int = 100) -> List[Bar]:
-        response = self.marketApi.get_candlesticks(instId=symbol, bar=bar, limit=str(limit))
-        if response.get('code') == '0' and response.get('data') and len(response['data']) > 0:
-            return to_okx_bar(response['data']) 
-        return []
-    
-
-def to_okx_tick(data: dict) -> List[Tick]:
-    ticks = []
-    ticks.append(Tick(
-        symbol=data['instId'],
-        price=float(data['last']),
-        timestmap = datetime.fromtimestamp(int(data['ts']) / 1000)
-    ))
-    return ticks
-
-
-def to_okx_position(data: List[dict]) -> List[Position]:
-    positions = []
-    for record in data:
-        positions.append(Position(
-            symbol=record.get('instId'),
-            instrumentType=record.get('instType'),
-            side=record.get('posSide'),
-            quantity=float(record.get('pos')),
-            unrealized_profit=round(float(record.get('upl')), 2),
-            unrealized_profit_ratio = round(float(record.get('uplRatio')) * 100, 2) ,
-            mode=record.get('mgnMode'),
-            price=float(record.get('avgPx')),
-            timestamp=datetime.fromtimestamp(int(record['cTime']) / 1000)
-        ))
-    return positions
-   
-
-def to_okx_bar(records: List[str]) -> List[Bar]:
-    bars: List[Bar] = []
-    for record in records:
-        timestamp, open, high, low, close, vol, _, _, _ = record
-        bars.append(Bar(
-            timestamp=datetime.fromtimestamp(int(timestamp) / 1000),
-            open=float(open),
-            high=float(high),
-            low=float(low),
-            close=float(close),
-            vol=float(vol),
-        )) 
-    return bars
-
-
-def to_okx_order(records: List[dict]) -> List[Order]:
-    orders = []
-    for data in records:
-        orders.append(Order(
-            orderId=data.get('ordId'),
-            orderType=data.get('ordType'),
-            symbol=data.get('instId'),
-            instrumentType=data.get('instType'),
-            price=float(data.get('px')),
-            status=data.get('state'),
-            side=data.get('side'),
-            quantity=0,
-            timestamp=datetime.fromtimestamp(int(data.get('cTime')) / 1000)
-        ))
-    return orders
-
-
-def to_okx_balance(records: dict) -> List[Balance]:
-    balance = []
-    if 'details' in records:
-        for record in records['details']:
-            if float(record.get('availBal')) != 0:
-                balance.append(Balance(asset=record['ccy'], availableBalance=float(record.get('availBal'))))
-    return balance
-
-
-class Subscription:
-    def __init__(self, channel: str, arg: dict, interval: int = 0) -> None:
-        self.channel = channel
-        self.arg = {
-            'channel': channel,
-            "extraParams": "{\"updateInterval\": INTERVAL}".replace('INTERVAL', str(interval)),
-            **arg
-        }
-
-    def __repr__(self) -> str:
-        return self.arg
-
-
-class OkxConnectionManager:
-    def __init__(self,
-                 uri: str,
-                 subscriptions: List[Subscription],
-                 conf: TradeBotConf = None,
-                 private: bool = False) -> None:
-        self.uri = uri
-        self.subscriptions = subscriptions
-        self.private = private
-        if private and conf:
-            self.conf = {
-                'apiKey': conf.okx['apiKey'],
-                'passphrase': conf.okx['passphrase'],
-                'secretKey': conf.okx['secretKey'],
-                'useServerTime': False
-            }
-
-    async def run(self):
-        async for conn in websockets.connect(self.uri):
-            try:
-                # login
-                if self.private and self.conf:
-                    payload = WsUtils.initLoginParams(**self.conf)
-                    await conn.send(payload.decode())
-                    await asyncio.sleep(3)
-                # subscribe
-                for sub in self.subscriptions:
-                    await conn.send(json.dumps({
-                        'op': 'subscribe',
-                        'args': [sub.arg]
-                    }))
-                async for message in conn:
-                    await self.handle_message(json.loads(message))
-            except websockets.ConnectionClosed:
-                logging.error(f"{','.join([sub.channel for sub in self.subscriptions])} reconnecting")
-                continue
-  
-    async def handle_message(self, message: dict):
-        if message.get('event'):
-            logging.info(f"{','.join([sub.channel for sub in self.subscriptions])} {json.dumps(message)}")
-
-
-class BalanceSubscribe(OkxConnectionManager):
-    def __init__(self, strategy: Strategy) -> None:
-        self.channel = 'account'
-        self.strategy = strategy
-        conf = TradeBotConf.load()
-        logging.info('init BalanceSubscribe')
-        super().__init__(conf.okx['ws_private'], [Subscription(self.channel, {'ccy': 'USDT'})], conf, True)
-
-    async def handle_message(self, message: dict):
-        await super().handle_message(message)
-        if message.get('arg', {}).get('channel') == self.channel and message.get('data'):
-            balance = to_okx_balance(message['data'][0])
-            self.strategy.on_balance_status(balance)
-        logging.info(f'[balance] {json.dumps(message)}')
-
-
-class OrderSubscriber(OkxConnectionManager):
-    def __init__(self, strategy: Strategy) -> None:
-        self.channel = 'orders'
-        self.strategy = strategy
-        conf = TradeBotConf.load()
-        logging.info('init OrderSubscriber')
-        super().__init__(conf.okx['ws_private'], [Subscription(self.channel, {'instType': self.strategy.instrumentType})], conf, True)
-
-    async def handle_message(self, message: dict):
-        await super().handle_message(message)
-        if message.get('arg', {}).get('channel') == self.channel and message.get('data'):
-            orders = to_okx_order(message['data'])
-            self.strategy.on_order_status(orders)
-        logging.info(f'[order] {json.dumps(message)}')
-
-
-class PositionSubscriber(OkxConnectionManager):
-    def __init__(self, strategy: Strategy) -> None:
-        self.channel = 'positions'
-        self.strategy = strategy
-        conf = TradeBotConf.load()
-        logging.info('init PositionSubscriber')
-        super().__init__(conf.okx['ws_private'], [Subscription(self.channel, {'instType': self.strategy.instrumentType}, interval=3)], conf, True)
-
-
-    async def handle_message(self, message: dict):
-        await super().handle_message(message)
-        if message.get('arg', {}).get('channel') == self.channel and message.get('data'):
-            positions = to_okx_position(message['data'])
-            self.strategy.on_position_status(positions)
-        logging.debug(f'[position] {json.dumps(message)}')
-
-
-class TickSubscriber(OkxConnectionManager):
-    def __init__(self, strategy: Strategy) -> None:
-        self.channel = 'tickers'
-        self.strategy = strategy
-        conf = TradeBotConf.load()
-        logging.info('init TickSubscriber')
-        super().__init__(conf.okx['ws_public'], [Subscription(self.channel, {'instId': sub}, interval=1) for sub in self.strategy.symbols])
-
-    async def handle_message(self, message: dict):
-        await super().handle_message(message)
-        if message.get('arg', {}).get('channel') == self.channel and message.get('data') and len(message.get('data')) > 0:
-            ticks = to_okx_tick(message['data'][0])
-            self.strategy.on_tick(ticks)
-        logging.debug(f'[tick] {json.dumps(message)}')
-
-
-class BarSubscriber(OkxConnectionManager):
-    def __init__(self, strategy: Strategy) -> None:
-        self.bar_types = set([f'candle{bar_type}' for bar_type in strategy.klines])
-        self.strategy = strategy
-        conf = TradeBotConf.load()
-        logging.info('init BarSubscriber')
-        subscriptions = []
-        for symbol in self.strategy.symbols:
-            for bar_type in self.bar_types:
-                logging.info(f'subscribe {bar_type}-{symbol}')
-                subscriptions.append(Subscription(f'{bar_type}', {'instId': symbol}, interval=1))
-        
-        super().__init__(conf.okx['ws_public'], subscriptions)
-
-    async def handle_message(self, message: dict):
-        await super().handle_message(message)
-        if message.get('arg', {}).get('channel', None) in self.bar_types and message.get('data') and len(message.get('data')) > 0:
-            bars = to_okx_bar(message['data'])
-            self.strategy.on_bar(bars)
-        logging.debug(f'[bar] {json.dumps(message)}')
-
-
-class OkxSubscriber(Subscriber):
-    def __init__(self, strategy: Strategy) -> None:
-        self.strategy = strategy
-        self.strategy.on_init_exchange(OkxExchangeClient(TradeBotConf.load()))
-    
-    
-    def run(self) -> List[asyncio.Future]:
-        return asyncio.gather(BalanceSubscribe(self.strategy).run(),
-                            OrderSubscriber(self.strategy).run(),
-                            BarSubscriber(self.strategy).run(),
-                            TickSubscriber(self.strategy).run(),
-                            PositionSubscriber(self.strategy).run())
+
+import asyncio
+import websockets
+from okx.websocket import WsUtils
+import okx.Trade as Trade
+import okx.Account as Account
+import okx.MarketData as Market
+
+from typing import List
+from datetime import datetime
+import json
+import logging
+
+from hades.core import TradeBotConf, Strategy, Exchange, Subscriber, Order, Position, Balance, Tick, Bar
+
+
+class OkxExchangeClient(Exchange):
+    def __init__(self,  conf: TradeBotConf) -> None:
+        self.conf = {
+            'api_key': conf.okx['apiKey'],
+            'api_secret_key': conf.okx['secretKey'],
+            'domain': conf.okx['domain'],
+            'passphrase': conf.okx['passphrase'],
+            'flag': '0'
+        }
+        self.tradeApi = Trade.TradeAPI(**self.conf)
+        self.accountApi = Account.AccountAPI(**self.conf)
+        self.marketApi = Market.MarketAPI(**self.conf)
+    # Account Info
+    def get_positions(self) -> List[Position]:
+        response = self.accountApi.get_positions()
+        if response.get('code') == '0' and response.get('data') and len(response['data']) > 0:
+            return to_okx_position(response['data']) 
+        return []
+
+    def get_balance(self):
+        return self.accountApi.get_account_balance()
+    # Trade Info
+    def get_orders(self) -> List[Order]:
+        response = self.tradeApi.get_order_list()
+        if response.get('code') == '0' and response.get('data') and len(response['data']) > 0:
+            return to_okx_order(response['data']) 
+        return []
+    
+    def place_buy_order(self, symbol: str, size: float, price: float):
+        return self.tradeApi.place_order(instId=symbol, tdMode='isolated', side='buy', sz=str(size), px=str(price), ordType='post_only')
+    
+    def place_sell_order(self, symbol: str, size: float, price: float):
+        return self.tradeApi.place_order(instId=symbol, tdMode='isolated', side='sell', sz=str(size), px=str(price), ordType='post_only')
+    
+    def cancel_order(self, orderId: str, symbol: str):
+        return self.tradeApi.cancel_order(instId=symbol, ordId=orderId)
+    
+    def close_position(self, symbol: str):
+        return self.tradeApi.close_positions(instId=symbol, mgnMode='isolated')
+
+    # get latest 100 bar
+    def get_candlesticks(self, symbol: str, bar: str = '1m', limit: int = 100) -> List[Bar]:
+        response = self.marketApi.get_candlesticks(instId=symbol, bar=bar, limit=str(limit))
+        if response.get('code') == '0' and response.get('data') and len(response['data']) > 0:
+            return to_okx_bar(response['data']) 
+        return []
+    
+
+def to_okx_tick(data: dict) -> List[Tick]:
+    ticks = []
+    ticks.append(Tick(
+        symbol=data['instId'],
+        price=float(data['last']),
+        timestmap = datetime.fromtimestamp(int(data['ts']) / 1000)
+    ))
+    return ticks
+
+
+def to_okx_position(data: List[dict]) -> List[Position]:
+    positions = []
+    for record in data:
+        positions.append(Position(
+            symbol=record.get('instId'),
+            instrumentType=record.get('instType'),
+            side=record.get('posSide'),
+            quantity=float(record.get('pos')),
+            unrealized_profit=round(float(record.get('upl')), 2),
+            unrealized_profit_ratio = round(float(record.get('uplRatio')) * 100, 2) ,
+            mode=record.get('mgnMode'),
+            price=float(record.get('avgPx')),
+            timestamp=datetime.fromtimestamp(int(record['cTime']) / 1000)
+        ))
+    return positions
+   
+
+def to_okx_bar(records: List[str]) -> List[Bar]:
+    bars: List[Bar] = []
+    for record in records:
+        timestamp, open, high, low, close, vol, _, _, _ = record
+        bars.append(Bar(
+            timestamp=datetime.fromtimestamp(int(timestamp) / 1000),
+            open=float(open),
+            high=float(high),
+            low=float(low),
+            close=float(close),
+            vol=float(vol),
+        )) 
+    return bars
+
+
+def to_okx_order(records: List[dict]) -> List[Order]:
+    orders = []
+    for data in records:
+        orders.append(Order(
+            orderId=data.get('ordId'),
+            orderType=data.get('ordType'),
+            symbol=data.get('instId'),
+            instrumentType=data.get('instType'),
+            price=float(data.get('px')),
+            status=data.get('state'),
+            side=data.get('side'),
+            quantity=0,
+            timestamp=datetime.fromtimestamp(int(data.get('cTime')) / 1000)
+        ))
+    return orders
+
+
+def to_okx_balance(records: dict) -> List[Balance]:
+    balance = []
+    if 'details' in records:
+        for record in records['details']:
+            if float(record.get('availBal')) != 0:
+                balance.append(Balance(asset=record['ccy'], availableBalance=float(record.get('availBal'))))
+    return balance
+
+
+class Subscription:
+    def __init__(self, channel: str, arg: dict, interval: int = 0) -> None:
+        self.channel = channel
+        self.arg = {
+            'channel': channel,
+            "extraParams": "{\"updateInterval\": INTERVAL}".replace('INTERVAL', str(interval)),
+            **arg
+        }
+
+    def __repr__(self) -> str:
+        return self.arg
+
+
+class OkxConnectionManager:
+    def __init__(self,
+                 uri: str,
+                 subscriptions: List[Subscription],
+                 conf: TradeBotConf = None,
+                 private: bool = False) -> None:
+        self.uri = uri
+        self.subscriptions = subscriptions
+        self.private = private
+        if private and conf:
+            self.conf = {
+                'apiKey': conf.okx['apiKey'],
+                'passphrase': conf.okx['passphrase'],
+                'secretKey': conf.okx['secretKey'],
+                'useServerTime': False
+            }
+
+    async def run(self):
+        async for conn in websockets.connect(self.uri):
+            try:
+                # login
+                if self.private and self.conf:
+                    payload = WsUtils.initLoginParams(**self.conf)
+                    await conn.send(payload.decode())
+                    await asyncio.sleep(3)
+                # subscribe
+                for sub in self.subscriptions:
+                    await conn.send(json.dumps({
+                        'op': 'subscribe',
+                        'args': [sub.arg]
+                    }))
+                async for message in conn:
+                    await self.handle_message(json.loads(message))
+            except websockets.ConnectionClosed:
+                logging.error(f"{','.join([sub.channel for sub in self.subscriptions])} reconnecting")
+                continue
+  
+    async def handle_message(self, message: dict):
+        if message.get('event'):
+            logging.info(f"{','.join([sub.channel for sub in self.subscriptions])} {json.dumps(message)}")
+
+
+class BalanceSubscribe(OkxConnectionManager):
+    def __init__(self, strategy: Strategy) -> None:
+        self.channel = 'account'
+        self.strategy = strategy
+        conf = TradeBotConf.load()
+        logging.info('init BalanceSubscribe')
+        super().__init__(conf.okx['ws_private'], [Subscription(self.channel, {'ccy': 'USDT'})], conf, True)
+
+    async def handle_message(self, message: dict):
+        await super().handle_message(message)
+        if message.get('arg', {}).get('channel') == self.channel and message.get('data'):
+            balance = to_okx_balance(message['data'][0])
+            self.strategy.on_balance_status(balance)
+        logging.info(f'[balance] {json.dumps(message)}')
+
+
+class OrderSubscriber(OkxConnectionManager):
+    def __init__(self, strategy: Strategy) -> None:
+        self.channel = 'orders'
+        self.strategy = strategy
+        conf = TradeBotConf.load()
+        logging.info('init OrderSubscriber')
+        super().__init__(conf.okx['ws_private'], [Subscription(self.channel, {'instType': self.strategy.instrumentType})], conf, True)
+
+    async def handle_message(self, message: dict):
+        await super().handle_message(message)
+        if message.get('arg', {}).get('channel') == self.channel and message.get('data'):
+            orders = to_okx_order(message['data'])
+            self.strategy.on_order_status(orders)
+        logging.info(f'[order] {json.dumps(message)}')
+
+
+class PositionSubscriber(OkxConnectionManager):
+    def __init__(self, strategy: Strategy) -> None:
+        self.channel = 'positions'
+        self.strategy = strategy
+        conf = TradeBotConf.load()
+        logging.info('init PositionSubscriber')
+        super().__init__(conf.okx['ws_private'], [Subscription(self.channel, {'instType': self.strategy.instrumentType}, interval=3)], conf, True)
+
+
+    async def handle_message(self, message: dict):
+        await super().handle_message(message)
+        if message.get('arg', {}).get('channel') == self.channel and message.get('data'):
+            positions = to_okx_position(message['data'])
+            self.strategy.on_position_status(positions)
+        logging.debug(f'[position] {json.dumps(message)}')
+
+
+class TickSubscriber(OkxConnectionManager):
+    def __init__(self, strategy: Strategy) -> None:
+        self.channel = 'tickers'
+        self.strategy = strategy
+        conf = TradeBotConf.load()
+        logging.info('init TickSubscriber')
+        super().__init__(conf.okx['ws_public'], [Subscription(self.channel, {'instId': sub}, interval=1) for sub in self.strategy.symbols])
+
+    async def handle_message(self, message: dict):
+        await super().handle_message(message)
+        if message.get('arg', {}).get('channel') == self.channel and message.get('data') and len(message.get('data')) > 0:
+            ticks = to_okx_tick(message['data'][0])
+            self.strategy.on_tick(ticks)
+        logging.debug(f'[tick] {json.dumps(message)}')
+
+
+class BarSubscriber(OkxConnectionManager):
+    def __init__(self, strategy: Strategy) -> None:
+        self.bar_types = set([f'candle{bar_type}' for bar_type in strategy.klines])
+        self.strategy = strategy
+        conf = TradeBotConf.load()
+        logging.info('init BarSubscriber')
+        subscriptions = []
+        for symbol in self.strategy.symbols:
+            for bar_type in self.bar_types:
+                logging.info(f'subscribe {bar_type}-{symbol}')
+                subscriptions.append(Subscription(f'{bar_type}', {'instId': symbol}, interval=1))
+        
+        super().__init__(conf.okx['ws_public'], subscriptions)
+
+    async def handle_message(self, message: dict):
+        await super().handle_message(message)
+        if message.get('arg', {}).get('channel', None) in self.bar_types and message.get('data') and len(message.get('data')) > 0:
+            bars = to_okx_bar(message['data'])
+            self.strategy.on_bar(bars)
+        logging.debug(f'[bar] {json.dumps(message)}')
+
+
+class OkxSubscriber(Subscriber):
+    def __init__(self, strategy: Strategy) -> None:
+        self.strategy = strategy
+        self.strategy.on_init_exchange(OkxExchangeClient(TradeBotConf.load()))
+    
+    
+    def run(self) -> List[asyncio.Future]:
+        return asyncio.gather(BalanceSubscribe(self.strategy).run(),
+                            OrderSubscriber(self.strategy).run(),
+                            BarSubscriber(self.strategy).run(),
+                            TickSubscriber(self.strategy).run(),
+                            PositionSubscriber(self.strategy).run())
```

### Comparing `hades-core-0.0.1/hades/core/executor.py` & `hades-core-0.0.2/hades/core/executor.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from hades.core import Strategy, BinanceUMSubscriber, OkxSubscriber, Subscriber, ExchangeEnum
-
-
-class TradeExecutor():
-    def __init__(self, strategy: Strategy, backtesting: bool, exchange:ExchangeEnum=ExchangeEnum.Binance) -> None:
-        self.backtesting = backtesting
-        self.strategy = strategy
-        self.exchange = exchange
-        self.subscriber = self.__get_subscriber(self.exchange)
-
-    async def execute(self):
-        await self.subscriber.run()
-
-    def __get_subscriber(self, exchange:ExchangeEnum) -> Subscriber:
-        if exchange == ExchangeEnum.Binance:
-            return BinanceUMSubscriber(self.strategy)
-        elif exchange == ExchangeEnum.OKX:
-            return OkxSubscriber(self.strategy)
-        raise  ValueError('current exchange does not support')
-    
-    def stop(self):
-        self.subscriber.stop()
-        
+from hades.core import Strategy, BinanceUMSubscriber, OkxSubscriber, Subscriber, ExchangeEnum
+
+
+class TradeExecutor():
+    def __init__(self, strategy: Strategy, backtesting: bool, exchange:ExchangeEnum=ExchangeEnum.Binance) -> None:
+        self.backtesting = backtesting
+        self.strategy = strategy
+        self.exchange = exchange
+        self.subscriber = self.__get_subscriber(self.exchange)
+
+    async def execute(self):
+        await self.subscriber.run()
+
+    def __get_subscriber(self, exchange:ExchangeEnum) -> Subscriber:
+        if exchange == ExchangeEnum.Binance:
+            return BinanceUMSubscriber(self.strategy)
+        elif exchange == ExchangeEnum.OKX:
+            return OkxSubscriber(self.strategy)
+        raise  ValueError('current exchange does not support')
+    
+    def stop(self):
+        self.subscriber.stop()
+
```

### Comparing `hades-core-0.0.1/hades/core/messager.py` & `hades-core-0.0.2/hades/core/messager.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from datetime import datetime
-import logging
-import requests
-from hades.core import TradeBotConf
-
-
-class Messager:
-    def __init__(self, conf: TradeBotConf) -> None:
-        self.prefix = conf.prefix
-        self.start, self.end = conf.period.split('-')
-        self.url = f'https://oapi.dingtalk.com/robot/send?access_token={conf.token}'
-        self.session = requests.session()
-        self.session.headers.update({
-            'Content-Type': 'application/json',
-        })
-        self.last_notify = None
-
-    def notify(self, text) -> bool:
-        data = {
-            'msgtype': 'text',
-            'text': {
-                'content': f'{self.prefix} {text}'
-            }
-        }
-        now = datetime.utcnow()
-        if now.hour >= int(self.start) and now.hour < int(self.end):
-            response = self.session.post(self.url, json=data)
-            return 'errmsg' in response.json() and response.json()['errmsg'] == 'ok'
-        else:
-            logging.info(f'message = {text} not sent')
-
-    def notify_with_interval(self, text, minute: int = 5) -> bool:
-        now = datetime.utcnow()
-        if not self.last_notify or (now - self.last_notify).seconds >= minute * 60:
-            self.last_notify = now
-            self.notify(text)
+from datetime import datetime
+import logging
+import requests
+from hades.core import TradeBotConf
+
+
+class Messager:
+    def __init__(self, conf: TradeBotConf) -> None:
+        self.prefix = conf.prefix
+        self.start, self.end = conf.period.split('-')
+        self.url = f'https://oapi.dingtalk.com/robot/send?access_token={conf.token}'
+        self.session = requests.session()
+        self.session.headers.update({
+            'Content-Type': 'application/json',
+        })
+        self.last_notify = None
+
+    def notify(self, text) -> bool:
+        data = {
+            'msgtype': 'text',
+            'text': {
+                'content': f'{self.prefix} {text}'
+            }
+        }
+        now = datetime.utcnow()
+        if now.hour >= int(self.start) and now.hour < int(self.end):
+            response = self.session.post(self.url, json=data)
+            return 'errmsg' in response.json() and response.json()['errmsg'] == 'ok'
+        else:
+            logging.info(f'message = {text} not sent')
+
+    def notify_with_interval(self, text, minute: int = 5) -> bool:
+        now = datetime.utcnow()
+        if not self.last_notify or (now - self.last_notify).seconds >= minute * 60:
+            self.last_notify = now
+            self.notify(text)
```

### Comparing `hades-core-0.0.1/hades/core/model.py` & `hades-core-0.0.2/hades/core/model.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from collections import namedtuple
-
-Tick = namedtuple('Tick', ['symbol', 'price', 'timestmap'])
-
-Bar = namedtuple('Bar', ['timestamp', 'open', 'high', 'low', 'close', 'vol'])
-
-Order = namedtuple('Orders', ['orderId', 'orderType', 'symbol', 
-                              'instrumentType', 'price', 
-                                'status', 'side', 'quantity', 'timestamp'])
-
-Position = namedtuple('Position', ['symbol', 'instrumentType', 
-                                   'side', 'quantity', 'unrealized_profit', 
-                                   'unrealized_profit_ratio', 'mode', 'price', 'timestamp'])
-
-Balance = namedtuple('Balance',['asset', 'availableBalance'])
-
-Trade = namedtuple('Trade', ['symbol', 
-                             'id', 
-                             'orderId', 
-                             'side', 
-                             'price', 
-                             'quantity',
-                             'realizedPnl',
-                             'marginAsset', 
-                             'quoteQty', 
-                             'commission', 
-                             'commissionToUSDT', 
-                             'commissionAsset', 
-                             'timestamp',
+from collections import namedtuple
+
+Tick = namedtuple('Tick', ['symbol', 'price', 'timestmap'])
+
+Bar = namedtuple('Bar', ['timestamp', 'open', 'high', 'low', 'close', 'vol'])
+
+Order = namedtuple('Orders', ['orderId', 'orderType', 'symbol', 
+                              'instrumentType', 'price', 
+                                'status', 'side', 'quantity', 'timestamp'])
+
+Position = namedtuple('Position', ['symbol', 'instrumentType', 
+                                   'side', 'quantity', 'unrealized_profit', 
+                                   'unrealized_profit_ratio', 'mode', 'price', 'timestamp'])
+
+Balance = namedtuple('Balance',['asset', 'availableBalance'])
+
+Trade = namedtuple('Trade', ['symbol', 
+                             'id', 
+                             'orderId', 
+                             'side', 
+                             'price', 
+                             'quantity',
+                             'realizedPnl',
+                             'marginAsset', 
+                             'quoteQty', 
+                             'commission', 
+                             'commissionToUSDT', 
+                             'commissionAsset', 
+                             'timestamp',
                              'maker'])
```

### Comparing `hades-core-0.0.1/hades_core.egg-info/PKG-INFO` & `hades-core-0.0.2/hades_core.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,297 +1,262 @@
-Metadata-Version: 2.1
-Name: hades-core
-Version: 0.0.1
-Summary: cryptocurrency trading bot
-Author-email: Gary Guo <gary.guo.china@gmail.com>
-Maintainer-email: Gary Guo <gary.guo.china@gmail.com>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: Homepage, https://github.com/hades-trading/hades-core
-Keywords: okx,binance,cryptocurrency
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## Hades Bot
-
-binance/okx based, currently it can only support real time Tick/Bar/Order/Position live update and monitor. In `bot/strategies/sample` , created a simple strategy, doing nothing but send notification 
-![alt text](./doc/screenshot.png "Screen Shot")
-## How to start
-
-### 1. Setup Environment
-
-```shell
-python -m venv runtime
-runtime\Scripts\activate
-pip install -r requirements.txt
-# if requirements.txt not work
-pip3 install python-okx websockets requests binance-futures-connector schedule "uvicorn[standard]" fastapi pandas
-```
-
-### 2. Change Configuration
-
-copy `example.conf` and rename to `app.conf` , change parameter
-
-```ini
-[binance]
-apiKey           = apiKey
-secretKey        = secretKey
-
-[okx]
-apiKey           = apiKey
-secretKey        = secretKey
-passphrase       = passphrase
-ws_private       = wss://wsaws.okx.com:8443/ws/v5/private
-ws_public        = wss://wsaws.okx.com:8443/ws/v5/public
-ws_business      = wss://wsaws.okx.com:8443/ws/v5/business
-domain           = https://aws.okx.com
-useServerTime    = False
-
-[notification]
-token            = token
-prefix           = prefix
-period           = 8-23
-```
-
-### 3. Strategy
-implement your own Strategy (extends Strategy) and replace the strategy in `main.py`
-
-```shell
-python main.py
-```
-
-### 4. Deploy to PROD
-
-#### 4.1 Create /app and execute git clone
-
-```shell
-sudo -s
-mkdir /app
-chown user:user /app
-cd /app
-git clone git@github.com:Icefoxes/trading-bot.git .
-```
-#### 4.2 setup supervisor
-
-```shell
-pip3 install supervisor
-echo_supervisord_conf > /etc/supervisord.conf
-echo bot.ini >> /etc/supervisord.conf
-supervisord -c /etc/supervisord.conf
-supervisorctl start bot
-```
-
-## Planned feature
-- backtesting
-- ui to show backtesting
+Metadata-Version: 2.1
+Name: hades-core
+Version: 0.0.2
+Summary: cryptocurrency trading bot
+Author-email: Gary Guo <gary.guo.china@gmail.com>
+Maintainer-email: Gary Guo <gary.guo.china@gmail.com>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: Homepage, https://github.com/hades-trading/hades-core
+Keywords: okx,binance,cryptocurrency
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## Hades Bot
+
+binance/okx based, currently it can only support real time Tick/Bar/Order/Position live update and monitor. In `bot/strategies/sample` , created a simple strategy, doing nothing but send notification 
+![alt text](./doc/screenshot.png "Screen Shot")
+## How to start
+
+### 1. Setup Environment
+
+```shell
+python -m venv runtime
+runtime\Scripts\activate
+pip install -r requirements.txt
+# if requirements.txt not work
+pip3 install python-okx websockets requests binance-futures-connector
+```
+
+### 2. Change Configuration
+
+copy `example.conf` and rename to `app.conf` , change parameter
+
+```ini
+[binance]
+apiKey           = apiKey
+secretKey        = secretKey
+
+[okx]
+apiKey           = apiKey
+secretKey        = secretKey
+passphrase       = passphrase
+ws_private       = wss://wsaws.okx.com:8443/ws/v5/private
+ws_public        = wss://wsaws.okx.com:8443/ws/v5/public
+ws_business      = wss://wsaws.okx.com:8443/ws/v5/business
+domain           = https://aws.okx.com
+useServerTime    = False
+
+[notification]
+token            = token
+prefix           = prefix
+period           = 8-23
+```
```

### Comparing `hades-core-0.0.1/pyproject.toml` & `hades-core-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-
-[project]
-# This is the name of your project. The first time you publish this
-# package, this name will be registered for you. It will determine how
-# users can install this project, e.g.:
-#
-# $ pip install sampleproject
-#
-# And where it will live on PyPI: https://pypi.org/project/sampleproject/
-name = "hades-core"
-
-# Versions should comply with PEP 440:
-# https://www.python.org/dev/peps/pep-0440/
-version = "0.0.1" 
-
-# This is a one-line description or tagline of what your project does. This
-# corresponds to the "Summary" metadata field:
-# https://packaging.python.org/specifications/core-metadata/#summary
-description = "cryptocurrency trading bot"  # Optional
-
-# This is an optional longer description of your project that represents
-# the body of text which users will see when they visit PyPI.
-#
-# Often, this is the same as your README, so you can just read it in from
-# that file directly (as we have already done above)
-#
-# This field corresponds to the "Description" metadata field:
-# https://packaging.python.org/specifications/core-metadata/#description-optional
-readme = "README.md" # Optional
-
-# Specify which Python versions you support. In contrast to the
-# 'Programming Language' classifiers above, 'pip install' will check this
-# and refuse to install the project if the version does not match. See
-# https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-requires-python = ">=3.7"
-
-# This is either text indicating the license for the distribution, or a file
-# that contains the license
-# https://packaging.python.org/en/latest/specifications/core-metadata/#license
-license = {file = "LICENSE"}
-
-# This field adds keywords for your project which will appear on the
-# project page. What does your project relate to?
-#
-# Note that this is a list of additional keywords, separated
-# by commas, to be used to assist searching for the distribution in a
-# larger catalog.
-keywords = ["okx", "binance", "cryptocurrency"] 
-
-# This should be your name or the name of the organization who originally
-# authored the project, and a valid email address corresponding to the name
-# listed.
-authors = [
-     {name = "Gary Guo", email = "gary.guo.china@gmail.com"},
-]
-
-# This should be your name or the names of the organization who currently
-# maintains the project, and a valid email address corresponding to the name
-# listed.
-maintainers = [
-    {name = "Gary Guo", email = "gary.guo.china@gmail.com"},
-]
-
-# Classifiers help users find your project by categorizing it.
-#
-# For a list of valid classifiers, see https://pypi.org/classifiers/
-classifiers = [  # Optional
-  # How mature is this project? Common values are
-  #   3 - Alpha
-  #   4 - Beta
-  #   5 - Production/Stable
-  "Development Status :: 3 - Alpha",
-
-  # Indicate who your project is intended for
-  "Intended Audience :: Developers",
-  "Topic :: Software Development :: Build Tools",
-
-  # Pick your license as you wish
-  "License :: OSI Approved :: MIT License",
-
-  # Specify the Python versions you support here. In particular, ensure
-  # that you indicate you support Python 3. These classifiers are *not*
-  # checked by "pip install". See instead "python_requires" below.
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: 3 :: Only",
-]
-
-# This field lists other packages that your project depends on to run.
-# Any package you put here will be installed by pip when your project is
-# installed, so they must be valid existing projects.
-#
-# For an analysis of this field vs pip's requirements files see:
-# https://packaging.python.org/discussions/install-requires-vs-requirements/
-dependencies = [ # Optional
-   "python-okx", 
-   "websockets", 
-   "requests", 
-   "binance-futures-connector"
-]
-
-# List additional groups of dependencies here (e.g. development
-# dependencies). Users will be able to install these using the "extras"
-# syntax, for example:
-#
-#   $ pip install sampleproject[dev]
-#
-# Similar to `dependencies` above, these must be valid existing
-# projects.
-[project.optional-dependencies] # Optional
-
-
-# List URLs that are relevant to your project
-#
-# This field corresponds to the "Project-URL" and "Home-Page" metadata fields:
-# https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
-# https://packaging.python.org/specifications/core-metadata/#home-page-optional
-#
-# Examples listed include a pattern for specifying where the package tracks
-# issues, where the source is hosted, where to say thanks to the package
-# maintainers, and where to support the project financially. The key is
-# what's used to render the link text on PyPI.
-[project.urls]  # Optional
-"Homepage" = "https://github.com/hades-trading/hades-core"
-
-[tool.setuptools.packages.find]
-exclude = ["tests*", "runtime*"]  # exclude packages matching these glob patterns (empty by default)
-
-[build-system]
-# These are the assumed default build requirements from pip:
-# https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
-requires = ["setuptools>=43.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[tool.bandit]
-exclude_dirs = ["build","dist","tests","runtime"]
+
+[project]
+# This is the name of your project. The first time you publish this
+# package, this name will be registered for you. It will determine how
+# users can install this project, e.g.:
+#
+# $ pip install sampleproject
+#
+# And where it will live on PyPI: https://pypi.org/project/sampleproject/
+name = "hades-core"
+
+# Versions should comply with PEP 440:
+# https://www.python.org/dev/peps/pep-0440/
+dynamic = ['version']
+
+# This is a one-line description or tagline of what your project does. This
+# corresponds to the "Summary" metadata field:
+# https://packaging.python.org/specifications/core-metadata/#summary
+description = "cryptocurrency trading bot"  # Optional
+
+# This is an optional longer description of your project that represents
+# the body of text which users will see when they visit PyPI.
+#
+# Often, this is the same as your README, so you can just read it in from
+# that file directly (as we have already done above)
+#
+# This field corresponds to the "Description" metadata field:
+# https://packaging.python.org/specifications/core-metadata/#description-optional
+readme = "README.md" # Optional
+
+# Specify which Python versions you support. In contrast to the
+# 'Programming Language' classifiers above, 'pip install' will check this
+# and refuse to install the project if the version does not match. See
+# https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
+requires-python = ">=3.7"
+
+# This is either text indicating the license for the distribution, or a file
+# that contains the license
+# https://packaging.python.org/en/latest/specifications/core-metadata/#license
+license = {file = "LICENSE"}
+
+# This field adds keywords for your project which will appear on the
+# project page. What does your project relate to?
+#
+# Note that this is a list of additional keywords, separated
+# by commas, to be used to assist searching for the distribution in a
+# larger catalog.
+keywords = ["okx", "binance", "cryptocurrency"] 
+
+# This should be your name or the name of the organization who originally
+# authored the project, and a valid email address corresponding to the name
+# listed.
+authors = [
+     {name = "Gary Guo", email = "gary.guo.china@gmail.com"},
+]
+
+# This should be your name or the names of the organization who currently
+# maintains the project, and a valid email address corresponding to the name
+# listed.
+maintainers = [
+    {name = "Gary Guo", email = "gary.guo.china@gmail.com"},
+]
+
+# Classifiers help users find your project by categorizing it.
+#
+# For a list of valid classifiers, see https://pypi.org/classifiers/
+classifiers = [  # Optional
+  # How mature is this project? Common values are
+  #   3 - Alpha
+  #   4 - Beta
+  #   5 - Production/Stable
+  "Development Status :: 3 - Alpha",
+
+  # Indicate who your project is intended for
+  "Intended Audience :: Developers",
+  "Topic :: Software Development :: Build Tools",
+
+  # Pick your license as you wish
+  "License :: OSI Approved :: MIT License",
+
+  # Specify the Python versions you support here. In particular, ensure
+  # that you indicate you support Python 3. These classifiers are *not*
+  # checked by "pip install". See instead "python_requires" below.
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3 :: Only",
+]
+
+# This field lists other packages that your project depends on to run.
+# Any package you put here will be installed by pip when your project is
+# installed, so they must be valid existing projects.
+#
+# For an analysis of this field vs pip's requirements files see:
+# https://packaging.python.org/discussions/install-requires-vs-requirements/
+dependencies = [ # Optional
+   "python-okx", 
+   "websockets", 
+   "requests", 
+   "binance-futures-connector"
+]
+
+# List additional groups of dependencies here (e.g. development
+# dependencies). Users will be able to install these using the "extras"
+# syntax, for example:
+#
+#   $ pip install sampleproject[dev]
+#
+# Similar to `dependencies` above, these must be valid existing
+# projects.
+[project.optional-dependencies] # Optional
+
+
+# List URLs that are relevant to your project
+#
+# This field corresponds to the "Project-URL" and "Home-Page" metadata fields:
+# https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
+# https://packaging.python.org/specifications/core-metadata/#home-page-optional
+#
+# Examples listed include a pattern for specifying where the package tracks
+# issues, where the source is hosted, where to say thanks to the package
+# maintainers, and where to support the project financially. The key is
+# what's used to render the link text on PyPI.
+[project.urls]  # Optional
+"Homepage" = "https://github.com/hades-trading/hades-core"
+
+[tool.setuptools.packages.find]
+exclude = ["tests*", "runtime*"]  # exclude packages matching these glob patterns (empty by default)
+
+[build-system]
+# These are the assumed default build requirements from pip:
+# https://pip.pypa.io/en/stable/reference/pip/#pep-517-and-518-support
+requires = ["setuptools>=43.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[tool.bandit]
+exclude_dirs = ["build","dist","tests","runtime"]
+
+[tool.setuptools.dynamic]
+version = {attr = "hades.__version__"}
```

