# Comparing `tmp/Deformation3D-1.7.6-py3-none-any.whl.zip` & `tmp/Deformation3D-1.7.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 479726 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      224 b- defN 23-Nov-28 09:53 Deformation3D/__init__.py
--rwxrwxr-x  2.0 unx  1251792 b- defN 23-Nov-28 09:53 Deformation3D/deform.cpython-38-x86_64-linux-gnu.so
--rw-rw-r--  2.0 unx     8339 b- defN 23-Nov-28 09:53 Deformation3D/deformation3d.py
--rw-rw-r--  2.0 unx     1817 b- defN 23-Nov-28 09:53 Deformation3D/demo.py
--rw-rw-r--  2.0 unx    42954 b- defN 23-Nov-28 09:54 Deformation3D/generate_vox.py
--rw-rw-r--  2.0 unx    34218 b- defN 23-Nov-28 09:53 Deformation3D/obj_2_points.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Nov-28 09:54 Deformation3D-1.7.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Nov-28 09:54 Deformation3D-1.7.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Nov-28 09:54 Deformation3D-1.7.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      852 b- defN 23-Nov-28 09:54 Deformation3D-1.7.6.dist-info/RECORD
-10 files, 1340698 bytes uncompressed, 478270 bytes compressed:  64.3%
+Zip file size: 479787 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      224 b- defN 24-Jun-03 03:27 Deformation3D/__init__.py
+-rwxrwxr-x  2.0 unx  1251792 b- defN 24-Jun-03 03:27 Deformation3D/deform.cpython-38-x86_64-linux-gnu.so
+-rw-rw-r--  2.0 unx     8402 b- defN 24-Jun-03 03:33 Deformation3D/deformation3d.py
+-rw-rw-r--  2.0 unx     1817 b- defN 24-Jun-03 03:27 Deformation3D/demo.py
+-rw-rw-r--  2.0 unx    42995 b- defN 24-Jun-03 03:33 Deformation3D/generate_vox.py
+-rw-rw-r--  2.0 unx    34432 b- defN 24-Jun-03 03:33 Deformation3D/obj_2_points.py
+-rw-rw-r--  2.0 unx      396 b- defN 24-Jun-03 03:34 Deformation3D-1.7.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Jun-03 03:34 Deformation3D-1.7.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 24-Jun-03 03:34 Deformation3D-1.7.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      852 b- defN 24-Jun-03 03:34 Deformation3D-1.7.7.dist-info/RECORD
+10 files, 1341016 bytes uncompressed, 478331 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: Deformation3D/generate_vox.py
 Comment: 
 
 Filename: Deformation3D/obj_2_points.py
 Comment: 
 
-Filename: Deformation3D-1.7.6.dist-info/METADATA
+Filename: Deformation3D-1.7.7.dist-info/METADATA
 Comment: 
 
-Filename: Deformation3D-1.7.6.dist-info/WHEEL
+Filename: Deformation3D-1.7.7.dist-info/WHEEL
 Comment: 
 
-Filename: Deformation3D-1.7.6.dist-info/top_level.txt
+Filename: Deformation3D-1.7.7.dist-info/top_level.txt
 Comment: 
 
-Filename: Deformation3D-1.7.6.dist-info/RECORD
+Filename: Deformation3D-1.7.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Deformation3D/deformation3d.py

```diff
@@ -94,15 +94,15 @@
             os.rmdir(dir)
             print(f"空文件夹 {dir} 已成功删除。")
         except OSError as e:
             print(f"删除文件夹 {dir} 时出现错误：{e}")
 
 
 def get_models_pcd(out_dir, vega_dir, outlier_th=100, outlier_e=1, remove_outlier=True, transform_axis=True,
-                   normal=False, rgb=False, semantic=False, post_process=True):
+                   normal=False, rgb=False, semantic=False, post_process=True, dbscan=False):
     """
     从模型中恢复点云数据
     :param out_dir:
     :param vega_dir: vega文件 /home/xxx/datasets/vega/
     :param outlier_th: 去除噪点 阈值
     :param outlier_e: 去除噪点 阈值
     :param remove_outlier: 去除噪点
@@ -131,15 +131,16 @@
                     # 删除 vertices、elements
                     os.remove(os.path.join(item_obj_dir, f"{txt_name}_vertices.txt"))
                     os.remove(os.path.join(item_obj_dir, f"{txt_name}_elements.txt"))
                     # 去除异常数据
                     if post_process:
                         clear_pcd(out_src_dir, out_data_dir, f"{txt_name}.txt", outlier_th=outlier_th,
                                   outlier_e=outlier_e,
-                                  remove_outlier=remove_outlier, transform_axis=transform_axis, normal=normal)
+                                  remove_outlier=remove_outlier, transform_axis=transform_axis, normal=normal,
+                                  dbscan=dbscan)
                         os.remove(os.path.join(out_src_dir, f"{txt_name}.txt"))
                 except FileNotFoundError:
                     print("文件不存在，无法删除。")
                 except OSError as e:
                     print(f"删除文件时出现错误：{e}")
                 except:
                     print("其他错误")
```

## Deformation3D/generate_vox.py

```diff
@@ -854,20 +854,21 @@
     :param vertices_label: 顶点 label
     :param filepath: 保存的文件名
     :param per_num: 每个叶子随机选取的顶点个数, -1 叶尖全部
     :return:
     """
     group_leaf = []
     vertices_label_list = np.array(vertices_label).astype(int)
-    n = vertices_label_list.max()
+    # n = vertices_label_list.max()
     # vis_point = []
     real_stem_bottom_index = None
     mid_stem_index_list = None
     # 叶
-    for i in range(0, n + 1):
+    unique_n = np.unique(vertices_label_list)
+    for i in unique_n:
         leaf_index_list = np.where(vertices_label_list == i)[0]
         # 叶子对应的顶点坐标
         leaf_points_list = []
         for leaf_index in leaf_index_list:
             value = vertices[leaf_index]
             leaf_points_list.append(value)
         leaf_points_arr = np.array(leaf_points_list)
```

## Deformation3D/obj_2_points.py

```diff
@@ -766,15 +766,15 @@
     normal = np.asarray(corn_cloud.normals)
     corn_xyz_normal_l = np.concatenate((corn_xyz, normal, corn_l), axis=1)
     del corn_cloud
     return corn_xyz_normal_l
 
 
 def clear_pcd(src_dir, target_dir, name, outlier_th=100, outlier_e=1, remove_outlier=True, transform_axis=True,
-              normal=False):
+              normal=False, dbscan=False):
     filepath = os.path.join(src_dir, name)
     corn_data = np.loadtxt(filepath)
     leaf_num = int(np.max(corn_data[:, -1]))
     corn_list = []
     corn_np = None
     # 区域生长分割
     if remove_outlier:
@@ -783,18 +783,22 @@
             i_corn_data = corn_data[point_index]
             pcd = o3d.geometry.PointCloud()
             pcd.points = o3d.utility.Vector3dVector(i_corn_data[:, :3])
             res = pcd.remove_statistical_outlier(outlier_th, outlier_e)  # 目标点周围的邻居数, 标准偏差比率
             # 欧式聚类
             pcd1 = res[0]
             # DBSCAN 聚类
-            pcd2, indexc = dbscan_cluster(pcd1)
-            points_r = np.asarray(pcd2.points)
-            # label = np.ones(points_r.shape[0]) * i
-            point_xyzl = np.concatenate([points_r, i_corn_data[:, 3:][res[1]][indexc]], axis=1)
+            if dbscan:
+                pcd2, indexc = dbscan_cluster(pcd1)
+                points_r = np.asarray(pcd2.points)
+                # label = np.ones(points_r.shape[0]) * i
+                point_xyzl = np.concatenate([points_r, i_corn_data[:, 3:][res[1]][indexc]], axis=1)
+            else:
+                points_r = np.asarray(pcd1.points)
+                point_xyzl = np.concatenate([points_r, i_corn_data[:, 3:][res[1]]], axis=1)
             corn_list.append(point_xyzl)
             del pcd, pcd1, pcd2
 
             # if i == 0:
             #     大于茎长（z）1/10的不处理，只处理下面的，然后拼接
             #     z_max = np.max(points[:, 2])
             #     bottom_mask = points[:, 2] < z_max/10
```

## Comparing `Deformation3D-1.7.6.dist-info/RECORD` & `Deformation3D-1.7.7.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Deformation3D/__init__.py,sha256=IMebni5OZruCJtlR6ov25b0dIk8UJ1GWkyV1wCYvg-4,224
 Deformation3D/deform.cpython-38-x86_64-linux-gnu.so,sha256=flMna9QAwkQL17QPNBP2A7xKi1k5z-f6GpxVY227B7k,1251792
-Deformation3D/deformation3d.py,sha256=pRdC45BWPaWAcDf4wTnqq_ZCbf54V3WTsT8vpgTMATI,8339
+Deformation3D/deformation3d.py,sha256=NZ3sEAli8hW9ojeq850JJmtobePJUypOok0eraQwkxA,8402
 Deformation3D/demo.py,sha256=4RiYtn54wzInYH2Bf4ssJAhY8nNbIqnjjDI20ohp-gg,1817
-Deformation3D/generate_vox.py,sha256=u1X0Kw0mg0fiJ6iGqQwUYpUfj80w3i7pvO4SFfsSTfY,42954
-Deformation3D/obj_2_points.py,sha256=DIK7m9mpSmbt92pSyXGz7OWQkSGOdDRvLcApBQNjKBA,34218
-Deformation3D-1.7.6.dist-info/METADATA,sha256=jb3648Hw5fW3HQ_GHtuLGFIpnQZE7GVu9vX7WRrlrgg,396
-Deformation3D-1.7.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-Deformation3D-1.7.6.dist-info/top_level.txt,sha256=l4eGNK_-VK-Iw06-p8j3hwvxKAHYIStX3HyrXwGaevY,14
-Deformation3D-1.7.6.dist-info/RECORD,,
+Deformation3D/generate_vox.py,sha256=qQq8ZO1dD0s0eWi-lRP_Vtv6wDd6EK5hSvB4JCjIITg,42995
+Deformation3D/obj_2_points.py,sha256=RfQg-egf_SGEHH0zIxQ6V1LlUycy5Q62Je7XW7J7SAg,34432
+Deformation3D-1.7.7.dist-info/METADATA,sha256=x3H9F9ZIkmusEfxpsly6h5qdZ9-UnqTvS9etaIoak0Y,396
+Deformation3D-1.7.7.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+Deformation3D-1.7.7.dist-info/top_level.txt,sha256=l4eGNK_-VK-Iw06-p8j3hwvxKAHYIStX3HyrXwGaevY,14
+Deformation3D-1.7.7.dist-info/RECORD,,
```

