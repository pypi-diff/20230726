# Comparing `tmp/pyone-6.6.2.tar.gz` & `tmp/pyone-6.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyone-6.6.2.tar", last modified: Tue May 30 17:18:23 2023, max compression
+gzip compressed data, was "pyone-6.6.3.tar", last modified: Tue Jul 25 17:35:33 2023, max compression
```

## Comparing `pyone-6.6.2.tar` & `pyone-6.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-05-30 17:18:23.854967 pyone-6.6.2/
--rw-rw-r--   0 one       (1001) one       (1001)      889 2023-05-30 17:18:23.854967 pyone-6.6.2/PKG-INFO
-drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-05-30 17:18:23.850967 pyone-6.6.2/pyone/
--rw-r--r--   0 one       (1001) one       (1001)    11256 2023-05-30 17:01:42.000000 pyone-6.6.2/pyone/__init__.py
--rw-r--r--   0 one       (1001) one       (1001)     5898 2023-05-30 17:01:42.000000 pyone-6.6.2/pyone/acl.py
-drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-05-30 17:18:23.850967 pyone-6.6.2/pyone/bindings/
--rw-rw-r--   0 one       (1001) one       (1001)   115076 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone/bindings/__init__.py
--rw-rw-r--   0 one       (1001) one       (1001)  2625409 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone/bindings/supbind.py
--rw-r--r--   0 one       (1001) one       (1001)     3278 2023-05-30 17:01:42.000000 pyone-6.6.2/pyone/helpers.py
--rw-r--r--   0 one       (1001) one       (1001)      929 2023-05-30 17:01:42.000000 pyone-6.6.2/pyone/server.py
--rw-r--r--   0 one       (1001) one       (1001)     7039 2023-05-30 17:01:42.000000 pyone-6.6.2/pyone/tester.py
--rw-r--r--   0 one       (1001) one       (1001)     5023 2023-05-30 17:01:42.000000 pyone-6.6.2/pyone/util.py
-drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-05-30 17:18:23.850967 pyone-6.6.2/pyone.egg-info/
--rw-rw-r--   0 one       (1001) one       (1001)      889 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone.egg-info/PKG-INFO
--rw-rw-r--   0 one       (1001) one       (1001)      299 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone.egg-info/SOURCES.txt
--rw-rw-r--   0 one       (1001) one       (1001)        1 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone.egg-info/dependency_links.txt
--rw-rw-r--   0 one       (1001) one       (1001)       89 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone.egg-info/requires.txt
--rw-rw-r--   0 one       (1001) one       (1001)        6 2023-05-30 17:18:23.000000 pyone-6.6.2/pyone.egg-info/top_level.txt
--rw-rw-r--   0 one       (1001) one       (1001)       38 2023-05-30 17:18:23.854967 pyone-6.6.2/setup.cfg
--rw-r--r--   0 one       (1001) one       (1001)     2495 2023-05-30 17:01:42.000000 pyone-6.6.2/setup.py
+drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-07-25 17:35:33.112224 pyone-6.6.3/
+-rw-rw-r--   0 one       (1001) one       (1001)      889 2023-07-25 17:35:33.112224 pyone-6.6.3/PKG-INFO
+drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-07-25 17:35:33.108224 pyone-6.6.3/pyone/
+-rw-r--r--   0 one       (1001) one       (1001)    11256 2023-07-25 17:29:39.000000 pyone-6.6.3/pyone/__init__.py
+-rw-r--r--   0 one       (1001) one       (1001)     5898 2023-07-25 17:29:39.000000 pyone-6.6.3/pyone/acl.py
+drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-07-25 17:35:33.108224 pyone-6.6.3/pyone/bindings/
+-rw-rw-r--   0 one       (1001) one       (1001)   115093 2023-07-25 17:35:32.000000 pyone-6.6.3/pyone/bindings/__init__.py
+-rw-rw-r--   0 one       (1001) one       (1001)  2626276 2023-07-25 17:35:32.000000 pyone-6.6.3/pyone/bindings/supbind.py
+-rw-r--r--   0 one       (1001) one       (1001)     3278 2023-07-25 17:29:39.000000 pyone-6.6.3/pyone/helpers.py
+-rw-r--r--   0 one       (1001) one       (1001)      929 2023-07-25 17:29:39.000000 pyone-6.6.3/pyone/server.py
+-rw-r--r--   0 one       (1001) one       (1001)     7039 2023-07-25 17:29:39.000000 pyone-6.6.3/pyone/tester.py
+-rw-r--r--   0 one       (1001) one       (1001)     5023 2023-07-25 17:29:39.000000 pyone-6.6.3/pyone/util.py
+drwxrwxr-x   0 one       (1001) one       (1001)        0 2023-07-25 17:35:33.108224 pyone-6.6.3/pyone.egg-info/
+-rw-rw-r--   0 one       (1001) one       (1001)      889 2023-07-25 17:35:33.000000 pyone-6.6.3/pyone.egg-info/PKG-INFO
+-rw-rw-r--   0 one       (1001) one       (1001)      299 2023-07-25 17:35:33.000000 pyone-6.6.3/pyone.egg-info/SOURCES.txt
+-rw-rw-r--   0 one       (1001) one       (1001)        1 2023-07-25 17:35:33.000000 pyone-6.6.3/pyone.egg-info/dependency_links.txt
+-rw-rw-r--   0 one       (1001) one       (1001)       89 2023-07-25 17:35:33.000000 pyone-6.6.3/pyone.egg-info/requires.txt
+-rw-rw-r--   0 one       (1001) one       (1001)        6 2023-07-25 17:35:33.000000 pyone-6.6.3/pyone.egg-info/top_level.txt
+-rw-rw-r--   0 one       (1001) one       (1001)       38 2023-07-25 17:35:33.112224 pyone-6.6.3/setup.cfg
+-rw-r--r--   0 one       (1001) one       (1001)     2495 2023-07-25 17:29:39.000000 pyone-6.6.3/setup.py
```

### Comparing `pyone-6.6.2/PKG-INFO` & `pyone-6.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyone
-Version: 6.6.2
+Version: 6.6.3
 Summary: Python Bindings for OpenNebula XML-RPC API
 Home-page: http://opennebula.io
 Author: Rafael del Valle
 Author-email: rvalle@privaz.io
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: PyOne is an implementation of OpenNebula XML-RPC
                 bindings in Python. It works as a proxy over the XML-RPC api and
```

### Comparing `pyone-6.6.2/pyone/__init__.py` & `pyone-6.6.3/pyone/__init__.py`

 * *Files identical despite different names*

### Comparing `pyone-6.6.2/pyone/acl.py` & `pyone-6.6.3/pyone/acl.py`

 * *Files identical despite different names*

### Comparing `pyone-6.6.2/pyone/bindings/__init__.py` & `pyone-6.6.3/pyone/bindings/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python
 
 #
-# Generated Tue May 30 17:18:23 2023 by generateDS.py version 2.41.5.
-# Python 3.8.10 (default, Mar 13 2023, 10:26:41)  [GCC 9.4.0]
+# Generated Tue Jul 25 17:35:32 2023 by generateDS.py version 2.42.2.
+# Python 3.8.10 (default, May 26 2023, 14:05:08)  [GCC 9.4.0]
 #
 # Command line options:
 #   ('-q', '')
 #   ('-f', '')
 #   ('-o', 'pyone/bindings/supbind.py')
 #   ('-s', 'pyone/bindings/__init__.py')
 #   ('--super', 'supbind')
 #   ('--external-encoding', 'utf-8')
 #   ('--silence', '')
 #
 # Command line arguments:
 #   ../../../share/doc/xsd/index.xsd
 #
 # Command line:
-#   /home/one/init-build-jenkins.bmbySM/one/src/oca/python/bin/generateDS -q -f -o "pyone/bindings/supbind.py" -s "pyone/bindings/__init__.py" --super="supbind" --external-encoding="utf-8" --silence ../../../share/doc/xsd/index.xsd
+#   /home/one/init-build-jenkins.DOlnm8/one/src/oca/python/bin/generateDS -q -f -o "pyone/bindings/supbind.py" -s "pyone/bindings/__init__.py" --super="supbind" --external-encoding="utf-8" --silence ../../../share/doc/xsd/index.xsd
 #
 # Current working directory (os.getcwd()):
 #   python
 #
 
 import os
 import sys
@@ -1660,16 +1660,16 @@
     def __init__(self, ID=None, UID=None, GID=None, UNAME=None, GNAME=None, NAME=None, LAST_POLL=None, STATE=None, LCM_STATE=None, RESCHED=None, STIME=None, ETIME=None, DEPLOY_ID=None, TEMPLATE=None, MONITORING=None, USER_TEMPLATE=None, HISTORY_RECORDS=None, **kwargs_):
         super(VMType92Sub, self).__init__(ID, UID, GID, UNAME, GNAME, NAME, LAST_POLL, STATE, LCM_STATE, RESCHED, STIME, ETIME, DEPLOY_ID, TEMPLATE, MONITORING, USER_TEMPLATE, HISTORY_RECORDS,  **kwargs_)
 supermod.VMType92.subclass = VMType92Sub
 # end class VMType92Sub
 
 
 class TEMPLATEType93Sub(TemplatedType, supermod.TEMPLATEType93):
-    def __init__(self, CPU=None, MEMORY=None, DISK=None, NIC=None, GRAPHICS=None, **kwargs_):
-        super(TEMPLATEType93Sub, self).__init__(CPU, MEMORY, DISK, NIC, GRAPHICS,  **kwargs_)
+    def __init__(self, CPU=None, MEMORY=None, VCPU=None, DISK=None, NIC=None, GRAPHICS=None, **kwargs_):
+        super(TEMPLATEType93Sub, self).__init__(CPU, MEMORY, VCPU, DISK, NIC, GRAPHICS,  **kwargs_)
 supermod.TEMPLATEType93.subclass = TEMPLATEType93Sub
 # end class TEMPLATEType93Sub
 
 
 class DISKTypeSub(TemplatedType, supermod.DISKType):
     def __init__(self, VCENTER_DS_REF=None, VCENTER_INSTANCE_ID=None, anytypeobjs_=None, **kwargs_):
         super(DISKTypeSub, self).__init__(VCENTER_DS_REF, VCENTER_INSTANCE_ID, anytypeobjs_,  **kwargs_)
```

### Comparing `pyone-6.6.2/pyone/bindings/supbind.py` & `pyone-6.6.3/pyone/bindings/supbind.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #
-# Generated Tue May 30 17:18:23 2023 by generateDS.py version 2.41.5.
-# Python 3.8.10 (default, Mar 13 2023, 10:26:41)  [GCC 9.4.0]
+# Generated Tue Jul 25 17:35:32 2023 by generateDS.py version 2.42.2.
+# Python 3.8.10 (default, May 26 2023, 14:05:08)  [GCC 9.4.0]
 #
 # Command line options:
 #   ('-q', '')
 #   ('-f', '')
 #   ('-o', 'pyone/bindings/supbind.py')
 #   ('-s', 'pyone/bindings/__init__.py')
 #   ('--super', 'supbind')
 #   ('--external-encoding', 'utf-8')
 #   ('--silence', '')
 #
 # Command line arguments:
 #   ../../../share/doc/xsd/index.xsd
 #
 # Command line:
-#   /home/one/init-build-jenkins.bmbySM/one/src/oca/python/bin/generateDS -q -f -o "pyone/bindings/supbind.py" -s "pyone/bindings/__init__.py" --super="supbind" --external-encoding="utf-8" --silence ../../../share/doc/xsd/index.xsd
+#   /home/one/init-build-jenkins.DOlnm8/one/src/oca/python/bin/generateDS -q -f -o "pyone/bindings/supbind.py" -s "pyone/bindings/__init__.py" --super="supbind" --external-encoding="utf-8" --silence ../../../share/doc/xsd/index.xsd
 #
 # Current working directory (os.getcwd()):
 #   python
 #
 
 import sys
 try:
@@ -39510,24 +39510,26 @@
 # end class VMType92
 
 
 class TEMPLATEType93(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, CPU=None, MEMORY=None, DISK=None, NIC=None, GRAPHICS=None, gds_collector_=None, **kwargs_):
+    def __init__(self, CPU=None, MEMORY=None, VCPU=None, DISK=None, NIC=None, GRAPHICS=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.CPU = CPU
         self.CPU_nsprefix_ = None
         self.MEMORY = MEMORY
         self.MEMORY_nsprefix_ = None
+        self.VCPU = VCPU
+        self.VCPU_nsprefix_ = None
         if DISK is None:
             self.DISK = []
         else:
             self.DISK = DISK
         self.DISK_nsprefix_ = None
         if NIC is None:
             self.NIC = []
@@ -39555,14 +39557,18 @@
         return self.CPU
     def set_CPU(self, CPU):
         self.CPU = CPU
     def get_MEMORY(self):
         return self.MEMORY
     def set_MEMORY(self, MEMORY):
         self.MEMORY = MEMORY
+    def get_VCPU(self):
+        return self.VCPU
+    def set_VCPU(self, VCPU):
+        self.VCPU = VCPU
     def get_DISK(self):
         return self.DISK
     def set_DISK(self, DISK):
         self.DISK = DISK
     def add_DISK(self, value):
         self.DISK.append(value)
     def insert_DISK_at(self, index, value):
@@ -39583,14 +39589,15 @@
         return self.GRAPHICS
     def set_GRAPHICS(self, GRAPHICS):
         self.GRAPHICS = GRAPHICS
     def has__content(self):
         if (
             self.CPU is not None or
             self.MEMORY is not None or
+            self.VCPU is not None or
             self.DISK or
             self.NIC or
             self.GRAPHICS is not None
         ):
             return True
         else:
             return False
@@ -39628,14 +39635,18 @@
             namespaceprefix_ = self.CPU_nsprefix_ + ':' if (UseCapturedNS_ and self.CPU_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sCPU>%s</%sCPU>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.CPU), input_name='CPU')), namespaceprefix_ , eol_))
         if self.MEMORY is not None:
             namespaceprefix_ = self.MEMORY_nsprefix_ + ':' if (UseCapturedNS_ and self.MEMORY_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sMEMORY>%s</%sMEMORY>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.MEMORY), input_name='MEMORY')), namespaceprefix_ , eol_))
+        if self.VCPU is not None:
+            namespaceprefix_ = self.VCPU_nsprefix_ + ':' if (UseCapturedNS_ and self.VCPU_nsprefix_) else ''
+            showIndent(outfile, level, pretty_print)
+            outfile.write('<%sVCPU>%s</%sVCPU>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.VCPU), input_name='VCPU')), namespaceprefix_ , eol_))
         for DISK_ in self.DISK:
             namespaceprefix_ = self.DISK_nsprefix_ + ':' if (UseCapturedNS_ and self.DISK_nsprefix_) else ''
             DISK_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='DISK', pretty_print=pretty_print)
         for NIC_ in self.NIC:
             namespaceprefix_ = self.NIC_nsprefix_ + ':' if (UseCapturedNS_ and self.NIC_nsprefix_) else ''
             NIC_.export(outfile, level, namespaceprefix_, namespacedef_='', name_='NIC', pretty_print=pretty_print)
         if self.GRAPHICS is not None:
@@ -39664,14 +39675,20 @@
             self.CPU_nsprefix_ = child_.prefix
         elif nodeName_ == 'MEMORY':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'MEMORY')
             value_ = self.gds_validate_string(value_, node, 'MEMORY')
             self.MEMORY = value_
             self.MEMORY_nsprefix_ = child_.prefix
+        elif nodeName_ == 'VCPU':
+            value_ = child_.text
+            value_ = self.gds_parse_string(value_, node, 'VCPU')
+            value_ = self.gds_validate_string(value_, node, 'VCPU')
+            self.VCPU = value_
+            self.VCPU_nsprefix_ = child_.prefix
         elif nodeName_ == 'DISK':
             obj_ = DISKType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.DISK.append(obj_)
             obj_.original_tagname_ = 'DISK'
         elif nodeName_ == 'NIC':
             obj_ = NICType.factory(parent_object_=self)
```

### Comparing `pyone-6.6.2/pyone/helpers.py` & `pyone-6.6.3/pyone/helpers.py`

 * *Files identical despite different names*

### Comparing `pyone-6.6.2/pyone/server.py` & `pyone-6.6.3/pyone/server.py`

 * *Files identical despite different names*

### Comparing `pyone-6.6.2/pyone/tester.py` & `pyone-6.6.3/pyone/tester.py`

 * *Files identical despite different names*

### Comparing `pyone-6.6.2/pyone/util.py` & `pyone-6.6.3/pyone/util.py`

 * *Files identical despite different names*

### Comparing `pyone-6.6.2/pyone.egg-info/PKG-INFO` & `pyone-6.6.3/pyone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyone
-Version: 6.6.2
+Version: 6.6.3
 Summary: Python Bindings for OpenNebula XML-RPC API
 Home-page: http://opennebula.io
 Author: Rafael del Valle
 Author-email: rvalle@privaz.io
 License: http://www.apache.org/licenses/LICENSE-2.0
 Description: PyOne is an implementation of OpenNebula XML-RPC
                 bindings in Python. It works as a proxy over the XML-RPC api and
```

### Comparing `pyone-6.6.2/setup.py` & `pyone-6.6.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     'requests'
 ]
 
 # include future in python2
 if sys.version_info[0] < 3:
     install_requires.append('future')
 
-version = '6.6.2'
+version = '6.6.3'
 
 # mark pre-release
 v1 = int(version.split('.')[1])
 v2 = int(version.split('.')[2])
 
 if v1 >= 90 or v2 >= 90:
     pyone_version = version + 'rc1'
```

