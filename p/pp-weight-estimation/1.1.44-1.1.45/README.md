# Comparing `tmp/pp_weight_estimation-1.1.44.tar.gz` & `tmp/pp_weight_estimation-1.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pp_weight_estimation-1.1.44.tar", last modified: Mon Jun  3 01:20:05 2024, max compression
+gzip compressed data, was "pp_weight_estimation-1.1.45.tar", last modified: Mon Jun  3 01:41:43 2024, max compression
```

## Comparing `pp_weight_estimation-1.1.44.tar` & `pp_weight_estimation-1.1.45.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.312045 pp_weight_estimation-1.1.44/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.44/README.md
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/pp_weight_estimation/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/pp_weight_estimation/core/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/core/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     9980 2024-06-03 01:19:39.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/core/function_test.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     6799 2024-06-03 00:56:17.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/core/get_weight.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/core/gpt_support.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1992 2024-06-02 16:33:46.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/core/s3_io.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/pp_weight_estimation/utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/utils/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2092 2024-06-02 00:07:54.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/utils/slack_connect.py
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/utils/visulizer.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-06-03 01:19:56.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/version.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-03 01:20:05.000000 pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-06-03 01:20:05.000000 pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/SOURCES.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-06-03 01:20:05.000000 pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/dependency_links.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-06-03 01:20:05.000000 pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/requires.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-06-03 01:20:05.000000 pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/top_level.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.44/pyproject.toml
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/scripts/
--rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.44/scripts/weight_pred.py
--rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-06-03 01:20:05.312045 pp_weight_estimation-1.1.44/setup.cfg
--rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.44/setup.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/tests/
--rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.44/tests/test_function_test.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:41:43.112758 pp_weight_estimation-1.1.45/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-03 01:41:43.112758 pp_weight_estimation-1.1.45/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.45/README.md
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:41:43.108758 pp_weight_estimation-1.1.45/pp_weight_estimation/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.45/pp_weight_estimation/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:41:43.112758 pp_weight_estimation-1.1.45/pp_weight_estimation/core/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.45/pp_weight_estimation/core/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    10106 2024-06-03 01:41:21.000000 pp_weight_estimation-1.1.45/pp_weight_estimation/core/function_test.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     6802 2024-06-03 01:38:30.000000 pp_weight_estimation-1.1.45/pp_weight_estimation/core/get_weight.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.45/pp_weight_estimation/core/gpt_support.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1992 2024-06-02 16:33:46.000000 pp_weight_estimation-1.1.45/pp_weight_estimation/core/s3_io.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:41:43.112758 pp_weight_estimation-1.1.45/pp_weight_estimation/utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.45/pp_weight_estimation/utils/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2092 2024-06-02 00:07:54.000000 pp_weight_estimation-1.1.45/pp_weight_estimation/utils/slack_connect.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.45/pp_weight_estimation/utils/visulizer.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-06-03 01:41:33.000000 pp_weight_estimation-1.1.45/pp_weight_estimation/version.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:41:43.112758 pp_weight_estimation-1.1.45/pp_weight_estimation.egg-info/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-03 01:41:43.000000 pp_weight_estimation-1.1.45/pp_weight_estimation.egg-info/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-06-03 01:41:43.000000 pp_weight_estimation-1.1.45/pp_weight_estimation.egg-info/SOURCES.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-06-03 01:41:43.000000 pp_weight_estimation-1.1.45/pp_weight_estimation.egg-info/dependency_links.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-06-03 01:41:43.000000 pp_weight_estimation-1.1.45/pp_weight_estimation.egg-info/requires.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-06-03 01:41:43.000000 pp_weight_estimation-1.1.45/pp_weight_estimation.egg-info/top_level.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.45/pyproject.toml
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:41:43.108758 pp_weight_estimation-1.1.45/scripts/
+-rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.45/scripts/weight_pred.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-06-03 01:41:43.112758 pp_weight_estimation-1.1.45/setup.cfg
+-rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.45/setup.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:41:43.112758 pp_weight_estimation-1.1.45/tests/
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.45/tests/test_function_test.py
```

### Comparing `pp_weight_estimation-1.1.44/pp_weight_estimation/core/function_test.py` & `pp_weight_estimation-1.1.45/pp_weight_estimation/core/function_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,37 +124,37 @@
     use_input_groundtruth = 'input_groundtruth' in input_df.columns
 
     entries = []
     for _, row in input_df.iterrows():
         image_dict = split_filename(row['s3_image_path'])
         local_image_folder = path_to_save_images + image_dict['siteId'] + '/' + image_dict['food_item'] + '/'
         os.makedirs(local_image_folder, exist_ok=True)
-        local_image_path = path_to_save_images + image_dict['siteId'] + '/' + image_dict['food_item'] + '/' + image_dict['image']
+        local_image_path = path_to_save_images + image_dict['siteId'] + '/' + image_dict['food_item'] + '/' + image_dict['image'] + '.jpeg'
         img_temp = download_image(bucket, row['s3_image_path'], client)
         if img_temp is None:
             if logger:
                 logger.error(f"Error downloading image {row['s3_image_path']}. Skipping image.")
             continue
         else:
             img_temp.save(local_image_path)
         site_id = row['site_id']
         taxonomy_code = row['taxonomy_code']
         food_item = row['food_item']
         input_groundtruth = row['input_groundtruth'] if use_input_groundtruth else 0
         if local_image_path and site_id and taxonomy_code:
             composed_key = f"{site_id}_{taxonomy_code}"
-            entries.append((site_id, local_image_path, composed_key, taxonomy_code,local_image_folder))
+            entries.append((site_id, local_image_path, composed_key, taxonomy_code,local_image_folder,image_dict['image']))
     
     if not entries:
         if logger:
             logger.error("No valid entries found in the CSV file")
         raise ValueError("No valid entries found in the CSV file")
     
     results = []
-    for index, (site_id, local_image_path, composed_key, taxonomy_code,local_image_folder) in enumerate(entries):
+    for index, (site_id, local_image_path, composed_key, taxonomy_code,local_image_folder,image_dict_name) in enumerate(entries):
         try:
             if composed_key not in color_dict:
                 if logger:
                     logger.error(f"No color found for key {composed_key}. Skipping image {local_image_path}.")
                 input_df.at[index, 'success'] = False
                 continue
             colors = color_dict[composed_key]
@@ -174,30 +174,30 @@
             #     mask_image.save(mask_image_path)
             #     input_df.at[index, 'mask'] = mask_image_path
             # else:
             #     input_df.at[index, 'mask'] = ''
 
             new_final_img = get_final_img(local_image_path, final_mask)  ## saving final mask with the image
             if save_plots:
-                final_image_path = local_image_folder + f"{food_item}_final_mask.png"
+                final_image_path = local_image_folder + f"{food_item}" + "/" + image_dict_name + "_" +todays_date  +"_final_mask.png"
                 new_final_img.save(final_image_path)
                 input_df.at[index, 'mask'] = final_image_path
             else:
                 input_df.at[index, 'mask'] = ''
 
             new_histogram, _ = get_histogram(new_final_img)
 
             pixel_count = new_histogram[-1]
             pixel_count = pixel_count.astype(int)
             input_df.at[index, 'pixel_count'] = pixel_count
 
             if save_plots:
                 plt.figure()
                 plt.plot(new_histogram)
-                plt.savefig(local_image_folder + f"{food_item}_histogram.png")
+                plt.savefig(local_image_folder + f"{food_item}/{image_dict_name}_{todays_date}_histogram.png")
                 plt.close()
 
             reference_row = groundtruth_df[groundtruth_df['taxonomy_code'] == taxonomy_code]
             if not reference_row.empty:
                 reference_pixel_count = reference_row.iloc[0]['reference_pixel_count']
                 groundtruth_weight = reference_row.iloc[0]['groundtruth']
```

### Comparing `pp_weight_estimation-1.1.44/pp_weight_estimation/core/get_weight.py` & `pp_weight_estimation-1.1.45/pp_weight_estimation/core/get_weight.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,9 +194,9 @@
     parts = file.split('/')
     if logger:
         logger.info(parts)
     return {
         'site_id': parts[1][7:],
         'meal_service': parts[2][12:],
         'food_item': parts[3][9:],
-        'image': parts[4][6:]
+        'image': parts[4][6:-12]
     }
```

### Comparing `pp_weight_estimation-1.1.44/pp_weight_estimation/core/gpt_support.py` & `pp_weight_estimation-1.1.45/pp_weight_estimation/core/gpt_support.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.44/pp_weight_estimation/core/s3_io.py` & `pp_weight_estimation-1.1.45/pp_weight_estimation/core/s3_io.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.44/pp_weight_estimation/utils/slack_connect.py` & `pp_weight_estimation-1.1.45/pp_weight_estimation/utils/slack_connect.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/SOURCES.txt` & `pp_weight_estimation-1.1.45/pp_weight_estimation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.44/setup.py` & `pp_weight_estimation-1.1.45/setup.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.44/tests/test_function_test.py` & `pp_weight_estimation-1.1.45/tests/test_function_test.py`

 * *Files identical despite different names*

