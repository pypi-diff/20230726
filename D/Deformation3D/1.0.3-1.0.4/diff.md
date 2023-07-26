# Comparing `tmp/Deformation3D-1.0.3-py3-none-any.whl.zip` & `tmp/Deformation3D-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 469865 bytes, number of entries: 10
+Zip file size: 469884 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx      162 b- defN 23-Jul-26 01:05 Deformation3D/__init__.py
 -rwxrwxr-x  2.0 unx  1227224 b- defN 23-Jul-26 01:05 Deformation3D/deform.cpython-38-x86_64-linux-gnu.so
--rw-rw-r--  2.0 unx     4005 b- defN 23-Jul-26 01:05 Deformation3D/deformation3d.py
+-rw-rw-r--  2.0 unx     4066 b- defN 23-Jul-26 01:14 Deformation3D/deformation3d.py
 -rw-rw-r--  2.0 unx     1720 b- defN 23-Jul-26 01:05 Deformation3D/demo.py
 -rw-rw-r--  2.0 unx    33494 b- defN 23-Jul-26 01:05 Deformation3D/generate_vox.py
 -rw-rw-r--  2.0 unx    29068 b- defN 23-Jul-26 01:05 Deformation3D/obj_2_points.py
--rw-rw-r--  2.0 unx      367 b- defN 23-Jul-26 01:05 Deformation3D-1.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-26 01:05 Deformation3D-1.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Jul-26 01:05 Deformation3D-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      852 b- defN 23-Jul-26 01:05 Deformation3D-1.0.3.dist-info/RECORD
-10 files, 1296998 bytes uncompressed, 468409 bytes compressed:  63.9%
+-rw-rw-r--  2.0 unx      367 b- defN 23-Jul-26 01:14 Deformation3D-1.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-26 01:14 Deformation3D-1.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Jul-26 01:14 Deformation3D-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      852 b- defN 23-Jul-26 01:14 Deformation3D-1.0.4.dist-info/RECORD
+10 files, 1297059 bytes uncompressed, 468428 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: Deformation3D/generate_vox.py
 Comment: 
 
 Filename: Deformation3D/obj_2_points.py
 Comment: 
 
-Filename: Deformation3D-1.0.3.dist-info/METADATA
+Filename: Deformation3D-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: Deformation3D-1.0.3.dist-info/WHEEL
+Filename: Deformation3D-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: Deformation3D-1.0.3.dist-info/top_level.txt
+Filename: Deformation3D-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: Deformation3D-1.0.3.dist-info/RECORD
+Filename: Deformation3D-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Deformation3D/deformation3d.py

```diff
@@ -69,14 +69,16 @@
     out_obj_dir = os.path.join(out_dir, "obj")
     out_src_dir = os.path.join(out_dir, "src")
     out_data_dir = os.path.join(out_dir, "data")
     os.makedirs(out_src_dir, exist_ok=True)
     os.makedirs(out_data_dir, exist_ok=True)
 
     for one_item in os.listdir(out_obj_dir):
+        if not os.path.isdir(one_item):
+            continue
         item_obj_dir = os.path.join(out_obj_dir, one_item)
         for one_vertices in os.listdir(item_obj_dir):
             if one_vertices[-12:-4] == "vertices":
                 txt_name = one_vertices[:-13]
                 try:
                     # 恢复点云数据
                     restore_one_point_cloud(item_obj_dir, vega_dir, out_src_dir, txt_name)
```

## Comparing `Deformation3D-1.0.3.dist-info/RECORD` & `Deformation3D-1.0.4.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Deformation3D/__init__.py,sha256=bZH3Jmx9iTImatccGVBXpyAb2S5CX5s-pFki-W852gE,162
 Deformation3D/deform.cpython-38-x86_64-linux-gnu.so,sha256=-IRZp_mJ6Lje0rqiBziB_4tlAS2UnMZukNsDrencHVo,1227224
-Deformation3D/deformation3d.py,sha256=ODD1zQMEC9cJJORiHy0hTUcrE2ZSKy1aXVBanDOllJA,4005
+Deformation3D/deformation3d.py,sha256=gdg-nFYFbv9Jyr7t0VQC66-leHlhaz4RaIhB-vS0qm8,4066
 Deformation3D/demo.py,sha256=VEvt9_l4rRqGEHYzVlz_cBfFE5GYaH-1u2feAqBl5UY,1720
 Deformation3D/generate_vox.py,sha256=ejXU3e_kXKoRG7Q3ve4Lh0T2p-ge3thnn7rIuA38hfc,33494
 Deformation3D/obj_2_points.py,sha256=KzkXIL5sGp25tcju49xjTHCUMv7aDskLC9l4auDyx8w,29068
-Deformation3D-1.0.3.dist-info/METADATA,sha256=YGahExkiPdwuIvq2erkwK8FOxYxMrNMoKu4TdHELzKQ,367
-Deformation3D-1.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-Deformation3D-1.0.3.dist-info/top_level.txt,sha256=l4eGNK_-VK-Iw06-p8j3hwvxKAHYIStX3HyrXwGaevY,14
-Deformation3D-1.0.3.dist-info/RECORD,,
+Deformation3D-1.0.4.dist-info/METADATA,sha256=nxoZOTIvy2gkUtJ_tJQtE0WqHT9FvI-5wPRIfREEhLY,367
+Deformation3D-1.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+Deformation3D-1.0.4.dist-info/top_level.txt,sha256=l4eGNK_-VK-Iw06-p8j3hwvxKAHYIStX3HyrXwGaevY,14
+Deformation3D-1.0.4.dist-info/RECORD,,
```

