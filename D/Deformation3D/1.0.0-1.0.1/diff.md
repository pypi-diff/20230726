# Comparing `tmp/Deformation3D-1.0.0-py3-none-any.whl.zip` & `tmp/Deformation3D-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 469960 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      162 b- defN 23-Jul-25 12:06 Deformation3D/__init__.py
--rwxrwxr-x  2.0 unx  1227208 b- defN 23-Jul-25 12:06 Deformation3D/deform.cpython-38-x86_64-linux-gnu.so
--rw-rw-r--  2.0 unx     4005 b- defN 23-Jul-25 12:06 Deformation3D/deformation3d.py
--rw-rw-r--  2.0 unx     1720 b- defN 23-Jul-25 12:06 Deformation3D/demo.py
--rw-rw-r--  2.0 unx    33493 b- defN 23-Jul-25 12:06 Deformation3D/generate_vox.py
--rw-rw-r--  2.0 unx    29068 b- defN 23-Jul-25 12:06 Deformation3D/obj_2_points.py
--rw-rw-r--  2.0 unx      367 b- defN 23-Jul-25 12:20 Deformation3D-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 12:20 Deformation3D-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Jul-25 12:20 Deformation3D-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      852 b- defN 23-Jul-25 12:20 Deformation3D-1.0.0.dist-info/RECORD
-10 files, 1296981 bytes uncompressed, 468504 bytes compressed:  63.9%
+Zip file size: 469959 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      162 b- defN 23-Jul-25 23:14 Deformation3D/__init__.py
+-rwxrwxr-x  2.0 unx  1227208 b- defN 23-Jul-25 23:14 Deformation3D/deform.cpython-38-x86_64-linux-gnu.so
+-rw-rw-r--  2.0 unx     4005 b- defN 23-Jul-25 23:14 Deformation3D/deformation3d.py
+-rw-rw-r--  2.0 unx     1720 b- defN 23-Jul-25 23:14 Deformation3D/demo.py
+-rw-rw-r--  2.0 unx    33494 b- defN 23-Jul-25 23:18 Deformation3D/generate_vox.py
+-rw-rw-r--  2.0 unx    29068 b- defN 23-Jul-25 23:14 Deformation3D/obj_2_points.py
+-rw-rw-r--  2.0 unx      367 b- defN 23-Jul-25 23:18 Deformation3D-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 23:18 Deformation3D-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Jul-25 23:18 Deformation3D-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      852 b- defN 23-Jul-25 23:18 Deformation3D-1.0.1.dist-info/RECORD
+10 files, 1296982 bytes uncompressed, 468503 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: Deformation3D/generate_vox.py
 Comment: 
 
 Filename: Deformation3D/obj_2_points.py
 Comment: 
 
-Filename: Deformation3D-1.0.0.dist-info/METADATA
+Filename: Deformation3D-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: Deformation3D-1.0.0.dist-info/WHEEL
+Filename: Deformation3D-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: Deformation3D-1.0.0.dist-info/top_level.txt
+Filename: Deformation3D-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: Deformation3D-1.0.0.dist-info/RECORD
+Filename: Deformation3D-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Deformation3D/generate_vox.py

```diff
@@ -518,15 +518,15 @@
     # 材料
     '''
     质量密度
     杨氏模量越大，越不容易变形
     泊松比是指在材料的比例极限内，由均匀分布的纵向应力引起的横向应变与相应的纵向应变之比的值
     '''
     MATERIAL_name0 = "\n*MATERIAL STEM\n"
-    MATERIAL_value0 = "ENU, 1000, 100000, 0.01\n"
+    MATERIAL_value0 = "ENU, 1000, 1000000, 0.01\n"
 
     MATERIAL_name1 = "\n*MATERIAL LEAF\n"
     MATERIAL_value1 = "ENU, 1000, 10000000, 0.45\n"
 
     # 集合
     SET_name0 = "\n*SET set0\n"
     SET_value0 = ""
```

