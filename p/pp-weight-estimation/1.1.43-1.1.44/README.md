# Comparing `tmp/pp_weight_estimation-1.1.43.tar.gz` & `tmp/pp_weight_estimation-1.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pp_weight_estimation-1.1.43.tar", last modified: Sun Jun  2 00:08:19 2024, max compression
+gzip compressed data, was "pp_weight_estimation-1.1.44.tar", last modified: Mon Jun  3 01:20:05 2024, max compression
```

## Comparing `pp_weight_estimation-1.1.43.tar` & `pp_weight_estimation-1.1.44.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-02 00:08:19.855676 pp_weight_estimation-1.1.43/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-02 00:08:19.855676 pp_weight_estimation-1.1.43/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.43/README.md
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-02 00:08:19.855676 pp_weight_estimation-1.1.43/pp_weight_estimation/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.43/pp_weight_estimation/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-02 00:08:19.855676 pp_weight_estimation-1.1.43/pp_weight_estimation/core/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.43/pp_weight_estimation/core/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    11113 2024-05-30 11:49:39.000000 pp_weight_estimation-1.1.43/pp_weight_estimation/core/function_test.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     6734 2024-05-30 11:49:39.000000 pp_weight_estimation-1.1.43/pp_weight_estimation/core/get_weight.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.43/pp_weight_estimation/core/gpt_support.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1993 2024-06-01 14:46:28.000000 pp_weight_estimation-1.1.43/pp_weight_estimation/core/s3_io.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-02 00:08:19.855676 pp_weight_estimation-1.1.43/pp_weight_estimation/utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.43/pp_weight_estimation/utils/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     2092 2024-06-02 00:07:54.000000 pp_weight_estimation-1.1.43/pp_weight_estimation/utils/slack_connect.py
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.43/pp_weight_estimation/utils/visulizer.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-06-02 00:08:01.000000 pp_weight_estimation-1.1.43/pp_weight_estimation/version.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-02 00:08:19.855676 pp_weight_estimation-1.1.43/pp_weight_estimation.egg-info/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-02 00:08:19.000000 pp_weight_estimation-1.1.43/pp_weight_estimation.egg-info/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-06-02 00:08:19.000000 pp_weight_estimation-1.1.43/pp_weight_estimation.egg-info/SOURCES.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-06-02 00:08:19.000000 pp_weight_estimation-1.1.43/pp_weight_estimation.egg-info/dependency_links.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-06-02 00:08:19.000000 pp_weight_estimation-1.1.43/pp_weight_estimation.egg-info/requires.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-06-02 00:08:19.000000 pp_weight_estimation-1.1.43/pp_weight_estimation.egg-info/top_level.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.43/pyproject.toml
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-02 00:08:19.855676 pp_weight_estimation-1.1.43/scripts/
--rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.43/scripts/weight_pred.py
--rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-06-02 00:08:19.855676 pp_weight_estimation-1.1.43/setup.cfg
--rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.43/setup.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-02 00:08:19.855676 pp_weight_estimation-1.1.43/tests/
--rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.43/tests/test_function_test.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.312045 pp_weight_estimation-1.1.44/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.44/README.md
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/pp_weight_estimation/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/pp_weight_estimation/core/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/core/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     9980 2024-06-03 01:19:39.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/core/function_test.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     6799 2024-06-03 00:56:17.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/core/get_weight.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/core/gpt_support.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1992 2024-06-02 16:33:46.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/core/s3_io.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/pp_weight_estimation/utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/utils/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     2092 2024-06-02 00:07:54.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/utils/slack_connect.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/utils/visulizer.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-06-03 01:19:56.000000 pp_weight_estimation-1.1.44/pp_weight_estimation/version.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-03 01:20:05.000000 pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-06-03 01:20:05.000000 pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/SOURCES.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-06-03 01:20:05.000000 pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/dependency_links.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-06-03 01:20:05.000000 pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/requires.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-06-03 01:20:05.000000 pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/top_level.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.44/pyproject.toml
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/scripts/
+-rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.44/scripts/weight_pred.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-06-03 01:20:05.312045 pp_weight_estimation-1.1.44/setup.cfg
+-rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.44/setup.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-03 01:20:05.308045 pp_weight_estimation-1.1.44/tests/
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.44/tests/test_function_test.py
```

### Comparing `pp_weight_estimation-1.1.43/pp_weight_estimation/core/function_test.py` & `pp_weight_estimation-1.1.44/pp_weight_estimation/core/function_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import transformers as t
 from PIL import Image
 import os
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 from mb_utils.src import logging
-from pp_weight_estimation.core.get_weight import get_seg, get_final_mask, get_final_img, get_histogram, get_val
+from pp_weight_estimation.core.get_weight import get_seg, get_final_mask, get_final_img, get_histogram, get_val, split_filename
 from pp_weight_estimation.core.s3_io import get_client, download_image
 from pp_weight_estimation.core.gpt_support import get_count
-from urllib.parse import urlparse
 from typing import List,Dict,Union
-import cv2
 import yaml
 import boto3
+from datetime import datetime
 
 logger = logging.logger 
 #model_checkpoint = '/Users/test/test1/mit-segformer-s' 
 #model = t.TFSegformerForSemanticSegmentation.from_pretrained(model_checkpoint)
 
 __all__ = ["load_color_values", "process_pipeline"]
 
@@ -75,14 +74,16 @@
     """
     config = load_config(config_path)
 
     input_csv_path = config['data']['input_csv_path']
     gt_csv_path = config['data']['gt_csv_path']
     val_color_csv_path = config['data']['val_color_csv_path']
     path_to_save_images = config['data']['path_to_save_images']
+    if path_to_save_images[-1] != '/':
+        path_to_save_images += '/'
     
     save_plots = config['results'].get('save_plots', False)
     final_mask_vals = config['results'].get('final_mask_vals', 50)
     mask_val = config['results'].get('model_val', 0.08)
     new_bg_removal = config['results'].get('background_removal', True)
     equalizer_items = config['results'].get('equalizer_items')
 
@@ -96,19 +97,22 @@
     gpt_response = config['gpt_res'].get('gpt_response', False)
     gpt_token = config['gpt_res'].get('gpt_token', None)
     gpt_model = config['gpt_res'].get('gpt_model', None)
     gpt_prompt = config['gpt_res'].get('gpt_prompt', None)
     gpt_file_path = config['gpt_res'].get('gpt_file_path', None)
     gpt_api_key = config['gpt_res']['gpt_api_key']
 
+    todays_date = "{:%Y_%m_%d}".format(datetime.now())
+
+
     model = t.TFSegformerForSemanticSegmentation.from_pretrained(model_path)  
 
     #might have to be change this
-    session = boto3.Session(profile_name=profile)
-    client = session.client('s3')
+    session = boto3.Session()
+    client = session.client(profile)
 
     color_dict = load_color_values(val_color_csv_path)
     groundtruth_df = pd.read_csv(gt_csv_path)
     input_df = pd.read_csv(input_csv_path)
     input_df['mask'] = ''
     input_df['final_image'] = ''
     input_df['pixel_count'] = 0
@@ -117,95 +121,83 @@
     input_df['error'] = 0.0
     input_df['success'] = False
 
     use_input_groundtruth = 'input_groundtruth' in input_df.columns
 
     entries = []
     for _, row in input_df.iterrows():
-        local_image_path = row['s3_image_path']
+        image_dict = split_filename(row['s3_image_path'])
+        local_image_folder = path_to_save_images + image_dict['siteId'] + '/' + image_dict['food_item'] + '/'
+        os.makedirs(local_image_folder, exist_ok=True)
+        local_image_path = path_to_save_images + image_dict['siteId'] + '/' + image_dict['food_item'] + '/' + image_dict['image']
+        img_temp = download_image(bucket, row['s3_image_path'], client)
+        if img_temp is None:
+            if logger:
+                logger.error(f"Error downloading image {row['s3_image_path']}. Skipping image.")
+            continue
+        else:
+            img_temp.save(local_image_path)
         site_id = row['site_id']
         taxonomy_code = row['taxonomy_code']
         food_item = row['food_item']
         input_groundtruth = row['input_groundtruth'] if use_input_groundtruth else 0
         if local_image_path and site_id and taxonomy_code:
             composed_key = f"{site_id}_{taxonomy_code}"
-            entries.append((site_id, local_image_path, composed_key, taxonomy_code))
+            entries.append((site_id, local_image_path, composed_key, taxonomy_code,local_image_folder))
     
     if not entries:
         if logger:
             logger.error("No valid entries found in the CSV file")
         raise ValueError("No valid entries found in the CSV file")
     
     results = []
-    for index, (site_id, local_image_path, composed_key, taxonomy_code) in enumerate(entries):
+    for index, (site_id, local_image_path, composed_key, taxonomy_code,local_image_folder) in enumerate(entries):
         try:
             if composed_key not in color_dict:
                 if logger:
                     logger.error(f"No color found for key {composed_key}. Skipping image {local_image_path}.")
                 input_df.at[index, 'success'] = False
                 continue
             colors = color_dict[composed_key]
         
-            site_dir = os.path.join(path_to_save_images, 'images' , site_id)
-            os.makedirs(site_dir, exist_ok=True)
-        
-            original_filename = os.path.basename(local_image_path)
-            save_filename, _ = os.path.splitext(os.path.basename(local_image_path))
-            download_path = os.path.join(site_dir, original_filename)
-        
-            if logger:
-                logger.info(f"Processing image: {local_image_path}")
-
-            image = download_image(bucket, local_image_path, client)
-            image.save(download_path)
-            ori_img = cv2.imread(download_path)
-
-            masked_img = get_seg(local_image_path, model, mask_val=mask_val, resize=True, new_bg_removal=new_bg_removal, equalize=True)
+            if taxonomy_code in equalizer_items:
+                equalizer = True
+            else:
+                equalizer = False
+            masked_img = get_seg(local_image_path, model, mask_val=mask_val, resize=True, new_bg_removal=new_bg_removal, equalizer=equalizer)
 
-            final_mask = None
             for color in colors:
-                mask = get_final_mask(ori_img, masked_img, color=color, val=final_mask_vals, logger=logger)
-                if final_mask is None:
-                    final_mask = mask
-                else:
-                    final_mask = cv2.bitwise_or(final_mask, mask)
-
-            masks_dir = os.path.join(path_to_save_images, 'masks')
-            os.makedirs(masks_dir, exist_ok=True)
-            mask_save_path = os.path.join(masks_dir, f"{save_filename}_mask_{final_mask_vals}.png")
-            mask_image = Image.fromarray(final_mask.astype(np.uint8))
-            mask_image.save(mask_save_path)
-            input_df.at[index, 'mask'] = mask_save_path
-
-            new_final_img = get_final_img(masked_img, final_mask, mask_val=mask_val)
-
-            final_images_dir = os.path.join(path_to_save_images, 'final_image')
-            os.makedirs(final_images_dir, exist_ok=True)
-            final_img_save_path = os.path.join(final_images_dir, f"{save_filename}_final.png")
-            final_image = Image.fromarray(new_final_img.astype(np.uint8))
-            final_image.save(final_img_save_path)
-            input_df.at[index, 'final_image'] = final_img_save_path
+                final_mask = get_final_mask(local_image_path, masked_img, color=color, val=final_mask_vals, logger=logger)
+
+            # if save_plots:
+            #     mask_image = Image.fromarray(final_mask.astype(np.uint8))
+            #     mask_image_path = local_image_folder + f"{food_item}_mask_{final_mask_vals}.png"
+            #     mask_image.save(mask_image_path)
+            #     input_df.at[index, 'mask'] = mask_image_path
+            # else:
+            #     input_df.at[index, 'mask'] = ''
 
-            final_image_np = np.array(final_image)
+            new_final_img = get_final_img(local_image_path, final_mask)  ## saving final mask with the image
+            if save_plots:
+                final_image_path = local_image_folder + f"{food_item}_final_mask.png"
+                new_final_img.save(final_image_path)
+                input_df.at[index, 'mask'] = final_image_path
+            else:
+                input_df.at[index, 'mask'] = ''
 
-            new_histogram, bin_edges = get_histogram(final_image_np)
+            new_histogram, _ = get_histogram(new_final_img)
 
             pixel_count = new_histogram[-1]
             pixel_count = pixel_count.astype(int)
             input_df.at[index, 'pixel_count'] = pixel_count
 
             if save_plots:
-                plots_dir = os.path.join(path_to_save_images, 'image_plots')
-                os.makedirs(plots_dir, exist_ok=True)
-                
-                hist_plot_path = os.path.join(plots_dir, f"{save_filename}_hist_plot.png")
-                input_df.at[index, 'histogram'] = hist_plot_path             
-                plt.savefig(hist_plot_path)
-                plt.close()
-            else:
+                plt.figure()
+                plt.plot(new_histogram)
+                plt.savefig(local_image_folder + f"{food_item}_histogram.png")
                 plt.close()
 
             reference_row = groundtruth_df[groundtruth_df['taxonomy_code'] == taxonomy_code]
             if not reference_row.empty:
                 reference_pixel_count = reference_row.iloc[0]['reference_pixel_count']
                 groundtruth_weight = reference_row.iloc[0]['groundtruth']
 
@@ -230,31 +222,16 @@
             results.append((masked_img, final_mask, new_final_img, new_histogram, pred_w2, error, gpt_result, gpt_error))
         except Exception as e:
             if logger:
                 logger.error(f"Error processing image {local_image_path}: {e}")
             input_df.at[index, 'success'] = False
             continue
     
-    output_csv_dir = os.path.join(path_to_save_images, 'csv', site_id, 'output_csv')
+    output_csv_dir = path_to_save_images + 'output_csv/'
     os.makedirs(output_csv_dir, exist_ok=True)
-    output_csv_path = os.path.join(output_csv_dir, "output.csv")
+    output_csv_path = os.path.join(output_csv_dir, f"output_{todays_date}.csv")
     input_df.to_csv(output_csv_path, index=False)
 
     if logger:
         logger.info(f"Processing complete. Output saved to {output_csv_path}")
         
     return output_csv_path, results
-
-
-# add logger - done
-# error if there is not taxcode and skip that image - done
-# column to output with failure or success -done
-# new csv with refrence image and groundtruth, and histogram pixel inside segmentation, model-checkpoint - done
-# download to GH2  particular location - done
-# save everything mask(save the 50 val in the name of file as _50) histogram and final image - done 
-# save everything locally - done
-# save the plots locally only when input is given add plot boolean input to process_pipeline at images_plot folder - done
-# yaml file for inputs -done
-# write the _mask after the name - done
-# s3cmd ls s3://pp-image-capture-processed-useast1-prod/siteId=33263/mealService=b514a5da-2bcf-4330-8a3c-f17e7f85a922/
-# get-repsonse -> get-image -> download image -> 
-# aslo csv files
```

### Comparing `pp_weight_estimation-1.1.43/pp_weight_estimation/core/get_weight.py` & `pp_weight_estimation-1.1.44/pp_weight_estimation/core/get_weight.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,24 +135,25 @@
         logger.info(upper_bound)
         logger.info(lower_bound)
     final_img = cv2.inRange(masked_img, np.array(lower_bound), np.array(upper_bound))
 
     if show:
         f, (axarr,axarr2) = plt.subplots(1,2,figsize=(15,15),gridspec_kw={'wspace':0.1, 'hspace':0.1},squeeze=True)
         axarr.imshow(final_img)
-        masked_image = np.copy(ori_img)
+        masked_image = np.copy(Image.open(ori_img))
+        #masked_image = np.copy(ori_img)
         masked_image[final_img<= 0.5] = 0
         axarr2.imshow(masked_image)
     return final_img
 
 def get_final_img(img,mask,mask_val=0.3):
     """
     Function to get the final image
     """
-    new_masked_image = np.copy(img)
+    new_masked_image = np.copy(Image.open(img))
     new_masked_image[mask<= mask_val] = 0
     return new_masked_image
     
 def get_histogram(img,show=False,logger=None):
     """
     Function to get the histogram of the image
     """
```

### Comparing `pp_weight_estimation-1.1.43/pp_weight_estimation/core/gpt_support.py` & `pp_weight_estimation-1.1.44/pp_weight_estimation/core/gpt_support.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.43/pp_weight_estimation/core/s3_io.py` & `pp_weight_estimation-1.1.44/pp_weight_estimation/core/s3_io.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -69,8 +69,8 @@
     """
     Downloads an image from S3
     """
     if client is None:
         client = get_client()
     response = get_response(client, bucket, key)
     return get_image(response)
-    
+
```

### Comparing `pp_weight_estimation-1.1.43/pp_weight_estimation/utils/slack_connect.py` & `pp_weight_estimation-1.1.44/pp_weight_estimation/utils/slack_connect.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.43/pp_weight_estimation.egg-info/SOURCES.txt` & `pp_weight_estimation-1.1.44/pp_weight_estimation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.43/setup.py` & `pp_weight_estimation-1.1.44/setup.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.43/tests/test_function_test.py` & `pp_weight_estimation-1.1.44/tests/test_function_test.py`

 * *Files identical despite different names*

