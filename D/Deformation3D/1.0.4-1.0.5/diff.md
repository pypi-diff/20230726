# Comparing `tmp/Deformation3D-1.0.4-py3-none-any.whl.zip` & `tmp/Deformation3D-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 469884 bytes, number of entries: 10
+Zip file size: 470102 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx      162 b- defN 23-Jul-26 01:05 Deformation3D/__init__.py
 -rwxrwxr-x  2.0 unx  1227224 b- defN 23-Jul-26 01:05 Deformation3D/deform.cpython-38-x86_64-linux-gnu.so
--rw-rw-r--  2.0 unx     4066 b- defN 23-Jul-26 01:14 Deformation3D/deformation3d.py
--rw-rw-r--  2.0 unx     1720 b- defN 23-Jul-26 01:05 Deformation3D/demo.py
+-rw-rw-r--  2.0 unx     4142 b- defN 23-Jul-26 01:26 Deformation3D/deformation3d.py
+-rw-rw-r--  2.0 unx     1736 b- defN 23-Jul-26 02:08 Deformation3D/demo.py
 -rw-rw-r--  2.0 unx    33494 b- defN 23-Jul-26 01:05 Deformation3D/generate_vox.py
--rw-rw-r--  2.0 unx    29068 b- defN 23-Jul-26 01:05 Deformation3D/obj_2_points.py
--rw-rw-r--  2.0 unx      367 b- defN 23-Jul-26 01:14 Deformation3D-1.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-26 01:14 Deformation3D-1.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Jul-26 01:14 Deformation3D-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      852 b- defN 23-Jul-26 01:14 Deformation3D-1.0.4.dist-info/RECORD
-10 files, 1297059 bytes uncompressed, 468428 bytes compressed:  63.9%
+-rw-rw-r--  2.0 unx    30553 b- defN 23-Jul-26 02:53 Deformation3D/obj_2_points.py
+-rw-rw-r--  2.0 unx      367 b- defN 23-Jul-26 02:56 Deformation3D-1.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-26 02:56 Deformation3D-1.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Jul-26 02:56 Deformation3D-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      852 b- defN 23-Jul-26 02:56 Deformation3D-1.0.5.dist-info/RECORD
+10 files, 1298636 bytes uncompressed, 468646 bytes compressed:  63.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: Deformation3D/generate_vox.py
 Comment: 
 
 Filename: Deformation3D/obj_2_points.py
 Comment: 
 
-Filename: Deformation3D-1.0.4.dist-info/METADATA
+Filename: Deformation3D-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: Deformation3D-1.0.4.dist-info/WHEEL
+Filename: Deformation3D-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: Deformation3D-1.0.4.dist-info/top_level.txt
+Filename: Deformation3D-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: Deformation3D-1.0.4.dist-info/RECORD
+Filename: Deformation3D-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Deformation3D/deformation3d.py

```diff
@@ -53,45 +53,47 @@
         try:
             # 使用 os.rmdir() 删除空文件夹
             os.rmdir(dir)
             print(f"空文件夹 {dir} 已成功删除。")
         except OSError as e:
             print(f"删除文件夹 {dir} 时出现错误：{e}")
 
-def get_models_pcd(out_dir, vega_dir, transform_axis=True, normal=False):
+
+def get_models_pcd(out_dir, vega_dir, remove_outlier=True, transform_axis=True, normal=False):
     """
     从模型中恢复点云数据
     :param out_dir:
     :param vega_dir: vega文件 /home/xxx/datasets/vega/
+    :param remove_outlier: 去除噪点
     :param transform_axis:
     :param normal:
     :return:
     """
     out_obj_dir = os.path.join(out_dir, "obj")
     out_src_dir = os.path.join(out_dir, "src")
     out_data_dir = os.path.join(out_dir, "data")
     os.makedirs(out_src_dir, exist_ok=True)
     os.makedirs(out_data_dir, exist_ok=True)
 
     for one_item in os.listdir(out_obj_dir):
-        if not os.path.isdir(one_item):
-            continue
         item_obj_dir = os.path.join(out_obj_dir, one_item)
+        if not os.path.isdir(item_obj_dir):
+            continue
         for one_vertices in os.listdir(item_obj_dir):
             if one_vertices[-12:-4] == "vertices":
                 txt_name = one_vertices[:-13]
                 try:
                     # 恢复点云数据
                     restore_one_point_cloud(item_obj_dir, vega_dir, out_src_dir, txt_name)
                     # 删除 vertices、elements
                     os.remove(os.path.join(item_obj_dir, f"{txt_name}_vertices.txt"))
                     os.remove(os.path.join(item_obj_dir, f"{txt_name}_elements.txt"))
                     # 去除异常数据
                     clear_pcd(out_src_dir, out_data_dir, f"{txt_name}.txt",
-                              remove_outlier=True, transform_axis=transform_axis, normal=normal)
+                              remove_outlier=remove_outlier, transform_axis=transform_axis, normal=normal)
                     os.remove(os.path.join(out_src_dir, f"{txt_name}.txt"))
                 except FileNotFoundError:
                     print("文件不存在，无法删除。")
                 except OSError as e:
                     print(f"删除文件时出现错误：{e}")
                 except:
                     print("其他错误")
```

## Deformation3D/demo.py

```diff
@@ -4,36 +4,36 @@
 import numpy as np
 
 from Deformation3D import prepare_vega_files, deform_models, get_models_pcd
 # Deformation3D.hello()
 
 
 config_filepath = "../configs/corn_vox.configs"
-txt_filepath = "demo/XY335-7-3-4.txt"
-vega_dir = "veg/"
-out_dir = "txt/"
+txt_filepath = "../demo/XY335-7-5-8.txt"
+vega_dir = "../demo/veg/"
+out_dir = "../demo/txt/"
 leaf_num = 7
-new_num = 10
+new_num = 1
 integrator_times = 20
 
 min_base_force = np.array([
-    [-8, -8, -100],  # stem
+    [-8, -8, -40],  # stem
     [-400, -400, -400],  # leaf 1
     [-400, -400, -400],  # leaf 2
     [-400, -400, -400],  # leaf 3
     [-400, -400, -400],  # leaf 4
     [-400, -400, -400],  # leaf 5
     [-400, -400, -400],  # leaf 6
     [-400, -400, -400],  # leaf 7
     [-400, -400, -400],  # leaf 8
     [-400, -400, -400],  # leaf 9
 ])
 
 max_base_force = np.array([
-    [8, 8, -100],  # stem
+    [8, 8, -40],  # stem
     [400, 400, 400],  # leaf 1
     [400, 400, 400],  # leaf 2
     [400, 400, 400],  # leaf 3
     [400, 400, 400],  # leaf 4
     [400, 400, 400],  # leaf 5
     [400, 400, 400],  # leaf 6
     [400, 400, 400],  # leaf 7
```

## Deformation3D/obj_2_points.py

```diff
@@ -719,28 +719,55 @@
     corn_data = np.loadtxt(filepath)
     leaf_num = int(np.max(corn_data[:, -1]))
     corn_list = []
     corn_np = None
     # 区域生长分割
     if remove_outlier:
         for i in range(leaf_num + 1):
+            #  茎 不处理顶部，大于茎长（z）1/2的不处理，只处理下面的，然后拼接
             point_index = np.where(i == corn_data[:-1])[0]
             points = corn_data[point_index]
-            pcd = o3d.geometry.PointCloud()
-            pcd.points = o3d.utility.Vector3dVector(points[:, :3])
-            res = pcd.remove_statistical_outlier(100, 1)  # 目标点周围的邻居数, 标准偏差比率
-            # 欧式聚类
-            pcd1 = res[0]
-            # DBSCAN 聚类
-            pcd2 = dbscan_cluster(pcd1)
-            points_r = np.asarray(pcd2.points)
-            label = np.ones(points_r.shape[0]) * i
-            point_xyzl = np.concatenate([points_r, label.reshape(-1, 1)], axis=1)
-            corn_list.append(point_xyzl)
-            del pcd, pcd1, pcd2
+            if i == 0:
+                z_max = np.max(points[:, 2])
+                bottom_mask = points[:, 2] < z_max/2
+                bottom_points = points[bottom_mask]
+                top_points = points[~bottom_mask]
+                pcd = o3d.geometry.PointCloud()
+                pcd.points = o3d.utility.Vector3dVector(bottom_points[:, :3])
+                res = pcd.remove_statistical_outlier(100, 1)  # 目标点周围的邻居数, 标准偏差比率
+                # 欧式聚类
+                pcd1 = res[0]
+                # DBSCAN 聚类
+                pcd2 = dbscan_cluster(pcd1)
+                points_b_r = np.asarray(pcd2.points)
+                points_r = np.r_[top_points[:, :3], points_b_r]
+                label = np.ones(points_r.shape[0]) * i
+                point_xyzl = np.concatenate([points_r, label.reshape(-1, 1)], axis=1)
+                corn_list.append(point_xyzl)
+                del pcd, pcd1, pcd2
+            else:
+                z_min = np.min(points[:, 2])
+                z_max = np.max(points[:, 2])
+                z_bottom = z_min + (z_max - z_min) / 5
+                bottom_mask = points[:, 2] < z_bottom
+                bottom_points = points[bottom_mask]
+                top_points = points[~bottom_mask]
+                pcd = o3d.geometry.PointCloud()
+                pcd.points = o3d.utility.Vector3dVector(bottom_points[:, :3])
+                res = pcd.remove_statistical_outlier(100, 1)  # 目标点周围的邻居数, 标准偏差比率
+                # 欧式聚类
+                pcd1 = res[0]
+                # DBSCAN 聚类
+                pcd2 = dbscan_cluster(pcd1)
+                points_b_r = np.asarray(pcd2.points)
+                points_r = np.r_[top_points[:, :3], points_b_r]
+                label = np.ones(points_r.shape[0]) * i
+                point_xyzl = np.concatenate([points_r, label.reshape(-1, 1)], axis=1)
+                corn_list.append(point_xyzl)
+                del pcd, pcd1, pcd2
         corn_np = np.concatenate(corn_list, axis=0)
         np.random.shuffle(corn_np)
         # corn_np = np.array(corn_list[0])
     if corn_np is None:
         corn_np = corn_data
     # if len(corn_np) < len(corn_data) * 0.6 or len(corn_np) < 4096:
     #     print("error:  ", name)
```

## Comparing `Deformation3D-1.0.4.dist-info/RECORD` & `Deformation3D-1.0.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Deformation3D/__init__.py,sha256=bZH3Jmx9iTImatccGVBXpyAb2S5CX5s-pFki-W852gE,162
 Deformation3D/deform.cpython-38-x86_64-linux-gnu.so,sha256=-IRZp_mJ6Lje0rqiBziB_4tlAS2UnMZukNsDrencHVo,1227224
-Deformation3D/deformation3d.py,sha256=gdg-nFYFbv9Jyr7t0VQC66-leHlhaz4RaIhB-vS0qm8,4066
-Deformation3D/demo.py,sha256=VEvt9_l4rRqGEHYzVlz_cBfFE5GYaH-1u2feAqBl5UY,1720
+Deformation3D/deformation3d.py,sha256=QWy40HxxWi46bjMkvgm0puKlb_P_-SkqU6BMU0qC9SM,4142
+Deformation3D/demo.py,sha256=KlHzS2L_u0vhCl-RcNCUjaAfwmsxuXTeIBBHy6gfPLI,1736
 Deformation3D/generate_vox.py,sha256=ejXU3e_kXKoRG7Q3ve4Lh0T2p-ge3thnn7rIuA38hfc,33494
-Deformation3D/obj_2_points.py,sha256=KzkXIL5sGp25tcju49xjTHCUMv7aDskLC9l4auDyx8w,29068
-Deformation3D-1.0.4.dist-info/METADATA,sha256=nxoZOTIvy2gkUtJ_tJQtE0WqHT9FvI-5wPRIfREEhLY,367
-Deformation3D-1.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-Deformation3D-1.0.4.dist-info/top_level.txt,sha256=l4eGNK_-VK-Iw06-p8j3hwvxKAHYIStX3HyrXwGaevY,14
-Deformation3D-1.0.4.dist-info/RECORD,,
+Deformation3D/obj_2_points.py,sha256=OS304UyY3A-SIx-ebRLoZ1fxCaobDsQarkaE7Z2_mwI,30553
+Deformation3D-1.0.5.dist-info/METADATA,sha256=ey-f3Oxft5kVUxzvpTQY2bfxRLezWvgAcuH-koKUxyE,367
+Deformation3D-1.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+Deformation3D-1.0.5.dist-info/top_level.txt,sha256=l4eGNK_-VK-Iw06-p8j3hwvxKAHYIStX3HyrXwGaevY,14
+Deformation3D-1.0.5.dist-info/RECORD,,
```

