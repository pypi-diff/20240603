# Comparing `tmp/offtracker-2.7.10.zip` & `tmp/offtracker-2.7.8.zip`

## zipinfo {}

```diff
@@ -1,35 +1,34 @@
-Zip file size: 3850710 bytes, number of entries: 33
-drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-03 22:08 offtracker-2.7.10/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-03 22:08 offtracker-2.7.10/offtracker/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-03 22:08 offtracker-2.7.10/offtracker.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-03 22:08 offtracker-2.7.10/scripts/
--rw-rw-rw-  2.0 fat    34523 b- defN 23-Mar-13 21:12 offtracker-2.7.10/LICENSE.txt
--rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-24 14:02 offtracker-2.7.10/MANIFEST.in
--rw-rw-rw-  2.0 fat     6858 b- defN 24-Jun-03 22:08 offtracker-2.7.10/PKG-INFO
--rw-rw-rw-  2.0 fat     6384 b- defN 24-Jun-03 22:07 offtracker-2.7.10/README.md
--rw-rw-rw-  2.0 fat       42 b- defN 24-Jun-03 22:08 offtracker-2.7.10/setup.cfg
--rw-rw-rw-  2.0 fat     1620 b- defN 24-Jun-02 23:48 offtracker-2.7.10/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 24-Jun-03 22:08 offtracker-2.7.10/offtracker/mapping/
--rw-rw-rw-  2.0 fat    25177 b- defN 24-Jun-03 17:37 offtracker-2.7.10/offtracker/X_offplot.py
--rw-rw-rw-  2.0 fat    16733 b- defN 24-Jan-24 00:39 offtracker-2.7.10/offtracker/X_offtracker.py
--rw-rw-rw-  2.0 fat     6628 b- defN 23-Dec-06 08:38 offtracker-2.7.10/offtracker/X_sequence.py
--rw-rw-rw-  2.0 fat     2422 b- defN 24-Jun-03 17:25 offtracker-2.7.10/offtracker/_version.py
--rw-rw-rw-  2.0 fat       62 b- defN 23-Oct-27 10:48 offtracker-2.7.10/offtracker/__init__.py
--rw-rw-rw-  2.0 fat     1016 b- defN 23-Jan-11 16:41 offtracker-2.7.10/offtracker/mapping/1.1_bed2fr_v4.5.py
--rw-rw-rw-  2.0 fat      825 b- defN 22-Oct-26 18:17 offtracker-2.7.10/offtracker/mapping/1.3_bdg_normalize_v4.0.py
--rw-rw-rw-  2.0 fat  9552920 b- defN 23-May-01 22:09 offtracker-2.7.10/offtracker/mapping/bedGraphToBigWig
--rw-rw-rw-  2.0 fat    11686 b- defN 22-May-05 11:59 offtracker-2.7.10/offtracker/mapping/hg38.chrom.sizes
--rw-rw-rw-  2.0 fat     1405 b- defN 22-Nov-15 15:31 offtracker-2.7.10/offtracker/mapping/mm10.chrom.sizes
--rw-rw-rw-  2.0 fat    92947 b- defN 24-Jan-04 21:44 offtracker-2.7.10/offtracker/mapping/offtracker_blacklist_hg38.merged.bed
--rw-rw-rw-  2.0 fat   139585 b- defN 24-Jan-02 23:08 offtracker-2.7.10/offtracker/mapping/offtracker_blacklist_mm10.merged.bed
--rw-rw-rw-  2.0 fat     8229 b- defN 24-Jan-23 16:27 offtracker-2.7.10/offtracker/mapping/Snakefile_offtracker
--rw-rw-rw-  2.0 fat        1 b- defN 24-Jun-03 22:08 offtracker-2.7.10/offtracker.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat     6858 b- defN 24-Jun-03 22:08 offtracker-2.7.10/offtracker.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat       41 b- defN 24-Jun-03 22:08 offtracker-2.7.10/offtracker.egg-info/requires.txt
--rw-rw-rw-  2.0 fat      796 b- defN 24-Jun-03 22:08 offtracker-2.7.10/offtracker.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat       11 b- defN 24-Jun-03 22:08 offtracker-2.7.10/offtracker.egg-info/top_level.txt
--rw-rw-rw-  2.0 fat    20229 b- defN 24-Jun-03 21:49 offtracker-2.7.10/scripts/offtracker_analysis.py
--rw-rw-rw-  2.0 fat    15156 b- defN 23-Dec-06 22:13 offtracker-2.7.10/scripts/offtracker_candidates.py
--rw-rw-rw-  2.0 fat     4185 b- defN 23-Dec-21 14:37 offtracker-2.7.10/scripts/offtracker_config.py
--rw-rw-rw-  2.0 fat     1528 b- defN 24-Jun-03 17:34 offtracker-2.7.10/scripts/offtracker_plot.py
-33 files, 9957920 bytes uncompressed, 3845300 bytes compressed:  61.4%
+Zip file size: 3846813 bytes, number of entries: 32
+drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-21 14:47 offtracker-2.7.8/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-21 14:47 offtracker-2.7.8/offtracker/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-21 14:47 offtracker-2.7.8/offtracker.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-21 14:47 offtracker-2.7.8/scripts/
+-rw-rw-rw-  2.0 fat    34523 b- defN 23-Mar-13 21:12 offtracker-2.7.8/LICENSE.txt
+-rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-24 14:02 offtracker-2.7.8/MANIFEST.in
+-rw-rw-rw-  2.0 fat     4521 b- defN 24-Mar-21 14:47 offtracker-2.7.8/PKG-INFO
+-rw-rw-rw-  2.0 fat     4091 b- defN 24-Mar-21 14:45 offtracker-2.7.8/README.md
+-rw-rw-rw-  2.0 fat       42 b- defN 24-Mar-21 14:47 offtracker-2.7.8/setup.cfg
+-rw-rw-rw-  2.0 fat     1543 b- defN 24-Mar-21 14:46 offtracker-2.7.8/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-21 14:47 offtracker-2.7.8/offtracker/mapping/
+-rw-rw-rw-  2.0 fat    24371 b- defN 24-Feb-18 21:47 offtracker-2.7.8/offtracker/X_offplot.py
+-rw-rw-rw-  2.0 fat    16733 b- defN 24-Jan-24 00:39 offtracker-2.7.8/offtracker/X_offtracker.py
+-rw-rw-rw-  2.0 fat     6628 b- defN 23-Dec-06 08:38 offtracker-2.7.8/offtracker/X_sequence.py
+-rw-rw-rw-  2.0 fat     2296 b- defN 24-Feb-03 22:00 offtracker-2.7.8/offtracker/_version.py
+-rw-rw-rw-  2.0 fat       62 b- defN 23-Oct-27 10:48 offtracker-2.7.8/offtracker/__init__.py
+-rw-rw-rw-  2.0 fat     1016 b- defN 23-Jan-11 16:41 offtracker-2.7.8/offtracker/mapping/1.1_bed2fr_v4.5.py
+-rw-rw-rw-  2.0 fat      825 b- defN 22-Oct-26 18:17 offtracker-2.7.8/offtracker/mapping/1.3_bdg_normalize_v4.0.py
+-rw-rw-rw-  2.0 fat  9552920 b- defN 23-May-01 22:09 offtracker-2.7.8/offtracker/mapping/bedGraphToBigWig
+-rw-rw-rw-  2.0 fat    11686 b- defN 22-May-05 11:59 offtracker-2.7.8/offtracker/mapping/hg38.chrom.sizes
+-rw-rw-rw-  2.0 fat     1405 b- defN 22-Nov-15 15:31 offtracker-2.7.8/offtracker/mapping/mm10.chrom.sizes
+-rw-rw-rw-  2.0 fat    92947 b- defN 24-Jan-04 21:44 offtracker-2.7.8/offtracker/mapping/offtracker_blacklist_hg38.merged.bed
+-rw-rw-rw-  2.0 fat   139585 b- defN 24-Jan-02 23:08 offtracker-2.7.8/offtracker/mapping/offtracker_blacklist_mm10.merged.bed
+-rw-rw-rw-  2.0 fat     8229 b- defN 24-Jan-23 16:27 offtracker-2.7.8/offtracker/mapping/Snakefile_offtracker
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Mar-21 14:47 offtracker-2.7.8/offtracker.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat     4521 b- defN 24-Mar-21 14:47 offtracker-2.7.8/offtracker.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat       41 b- defN 24-Mar-21 14:47 offtracker-2.7.8/offtracker.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat      769 b- defN 24-Mar-21 14:47 offtracker-2.7.8/offtracker.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Mar-21 14:47 offtracker-2.7.8/offtracker.egg-info/top_level.txt
+-rw-rw-rw-  2.0 fat    19559 b- defN 24-Feb-22 21:27 offtracker-2.7.8/scripts/offtracker_analysis.py
+-rw-rw-rw-  2.0 fat    15156 b- defN 23-Dec-06 22:13 offtracker-2.7.8/scripts/offtracker_candidates.py
+-rw-rw-rw-  2.0 fat     4185 b- defN 23-Dec-21 14:37 offtracker-2.7.8/scripts/offtracker_config.py
+32 files, 9947719 bytes uncompressed, 3841631 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -1,100 +1,97 @@
-Filename: offtracker-2.7.10/
+Filename: offtracker-2.7.8/
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/
+Filename: offtracker-2.7.8/offtracker/
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker.egg-info/
+Filename: offtracker-2.7.8/offtracker.egg-info/
 Comment: 
 
-Filename: offtracker-2.7.10/scripts/
+Filename: offtracker-2.7.8/scripts/
 Comment: 
 
-Filename: offtracker-2.7.10/LICENSE.txt
+Filename: offtracker-2.7.8/LICENSE.txt
 Comment: 
 
-Filename: offtracker-2.7.10/MANIFEST.in
+Filename: offtracker-2.7.8/MANIFEST.in
 Comment: 
 
-Filename: offtracker-2.7.10/PKG-INFO
+Filename: offtracker-2.7.8/PKG-INFO
 Comment: 
 
-Filename: offtracker-2.7.10/README.md
+Filename: offtracker-2.7.8/README.md
 Comment: 
 
-Filename: offtracker-2.7.10/setup.cfg
+Filename: offtracker-2.7.8/setup.cfg
 Comment: 
 
-Filename: offtracker-2.7.10/setup.py
+Filename: offtracker-2.7.8/setup.py
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/mapping/
+Filename: offtracker-2.7.8/offtracker/mapping/
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/X_offplot.py
+Filename: offtracker-2.7.8/offtracker/X_offplot.py
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/X_offtracker.py
+Filename: offtracker-2.7.8/offtracker/X_offtracker.py
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/X_sequence.py
+Filename: offtracker-2.7.8/offtracker/X_sequence.py
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/_version.py
+Filename: offtracker-2.7.8/offtracker/_version.py
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/__init__.py
+Filename: offtracker-2.7.8/offtracker/__init__.py
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/mapping/1.1_bed2fr_v4.5.py
+Filename: offtracker-2.7.8/offtracker/mapping/1.1_bed2fr_v4.5.py
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/mapping/1.3_bdg_normalize_v4.0.py
+Filename: offtracker-2.7.8/offtracker/mapping/1.3_bdg_normalize_v4.0.py
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/mapping/bedGraphToBigWig
+Filename: offtracker-2.7.8/offtracker/mapping/bedGraphToBigWig
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/mapping/hg38.chrom.sizes
+Filename: offtracker-2.7.8/offtracker/mapping/hg38.chrom.sizes
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/mapping/mm10.chrom.sizes
+Filename: offtracker-2.7.8/offtracker/mapping/mm10.chrom.sizes
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/mapping/offtracker_blacklist_hg38.merged.bed
+Filename: offtracker-2.7.8/offtracker/mapping/offtracker_blacklist_hg38.merged.bed
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/mapping/offtracker_blacklist_mm10.merged.bed
+Filename: offtracker-2.7.8/offtracker/mapping/offtracker_blacklist_mm10.merged.bed
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker/mapping/Snakefile_offtracker
+Filename: offtracker-2.7.8/offtracker/mapping/Snakefile_offtracker
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker.egg-info/dependency_links.txt
+Filename: offtracker-2.7.8/offtracker.egg-info/dependency_links.txt
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker.egg-info/PKG-INFO
+Filename: offtracker-2.7.8/offtracker.egg-info/PKG-INFO
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker.egg-info/requires.txt
+Filename: offtracker-2.7.8/offtracker.egg-info/requires.txt
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker.egg-info/SOURCES.txt
+Filename: offtracker-2.7.8/offtracker.egg-info/SOURCES.txt
 Comment: 
 
-Filename: offtracker-2.7.10/offtracker.egg-info/top_level.txt
+Filename: offtracker-2.7.8/offtracker.egg-info/top_level.txt
 Comment: 
 
-Filename: offtracker-2.7.10/scripts/offtracker_analysis.py
+Filename: offtracker-2.7.8/scripts/offtracker_analysis.py
 Comment: 
 
-Filename: offtracker-2.7.10/scripts/offtracker_candidates.py
+Filename: offtracker-2.7.8/scripts/offtracker_candidates.py
 Comment: 
 
-Filename: offtracker-2.7.10/scripts/offtracker_config.py
-Comment: 
-
-Filename: offtracker-2.7.10/scripts/offtracker_plot.py
+Filename: offtracker-2.7.8/scripts/offtracker_config.py
 Comment: 
 
 Zip file comment:
```

## Comparing `offtracker-2.7.10/LICENSE.txt` & `offtracker-2.7.8/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `offtracker-2.7.10/setup.py` & `offtracker-2.7.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,14 +45,11 @@
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     url=URL,
     python_requires=REQUIRES_PYTHON,
     packages=find_packages(),
     package_data={'offtracker': ['mapping/*']},
-    scripts = ['scripts/offtracker_config.py',
-               'scripts/offtracker_candidates.py',
-               'scripts/offtracker_analysis.py',
-               'scripts/offtracker_plot.py'],
+    scripts = ['scripts/offtracker_config.py','scripts/offtracker_candidates.py','scripts/offtracker_analysis.py'],
     install_requires=REQUIRED,
     include_package_data=True
 )
```

## Comparing `offtracker-2.7.10/offtracker/X_offplot.py` & `offtracker-2.7.8/offtracker/X_offplot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,30 @@
-
-import pandas as pd
-import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.patches as patches
-from matplotlib import rcParams
-# 和用 plt.rcParams or matplotlib.rcParams 是一样的
-dict_rc = {
-    'pdf.fonttype': 42,
-    'font.family': ['Arial']
-}
-rcParams.update(dict_rc)
+import pandas as pd
+import numpy as np
 
-# 2024.06.03. offtable 添加 threshold 分界线，默认为 None，常用的是 2
-def offtable(offtargets, target_guide,  length_pam = 3, 
+def offtable(offtargets, target_guide, 
                          col_seq='best_target', col_score='track_score', col_mismatch='mismatch', col_loc='target_location',
                          title=None, font='Arial', font_size=9, 
-                         box_size_x=15, box_size_y=20, box_gap=1, threshold=None,
-                         x_offset=15, y_offset=35, dpi=300, savefig=None):
+                         box_size_x=15, box_size_y=20, box_gap=1,
+                         x_offset=15, y_offset=35, dpi=200, savefig=None):
     # Facecolor
     color_dict = {
         'A': 'lightgreen',
         'T': 'lightblue',
         'C': 'lightcoral',
         'G': 'lightgoldenrodyellow',
         'N': 'lightgrey',
         '—': 'orange',
         '-': 'orange'
     }
 
     # If offtargets is a DataFrame, convert to list of dictionaries
     if isinstance(offtargets, pd.DataFrame):
-        if threshold is not None:
-            n_positive = sum(offtargets[col_score]>=threshold)
         offtargets = offtargets.to_dict(orient='records')
 
     # Configuration
     # title=None
     # font='Arial'
     # font_size = 9
     # box_size_x = 15 # 一个碱基图形的宽度
@@ -107,26 +96,19 @@
 
         # Annotations for score, mismatches, and location coordinates
         ax.text(x_offset + (len(target_guide) + 2) * box_size_x, y + box_size_y / 2, round(seq[col_score],2), ha='center', va='center', family=font, fontsize=font_size)
         #ax.text(x_offset + (len(target_guide) + 7) * box_size_x, y + box_size_y / 2, "Target" if seq[col_mismatch] == 0 else seq[col_mismatch], ha='center', va='center', family=font, fontsize=font_size, color='red' if seq[col_mismatch] == 0 else 'black')
         ax.text(x_offset + (len(target_guide) + 4) * box_size_x, y + box_size_y / 2, seq[col_loc], ha='left', va='center', family=font, fontsize=font_size)
 
     # add a vertical line to indicate the PAM
-    x_line = x_offset + (len(target_guide) - length_pam) * box_size_x
+    x_line = x_offset + (len(target_guide) - 3) * box_size_x
     y_start = y_offset # + box_size_y / 2 
     y_end = y_start + (len(offtargets)+1) * (box_size_y + box_gap)
     ax.vlines(x=x_line, ymin=y_start, ymax=y_end, color='indianred', linestyle='--')
 
-    # 2024.06.03. add a horizontal line to indicate the threshold
-    if threshold is not None:
-        thresh_x_start = x_offset
-        thresh_x_end = x_offset + len(target_guide) * box_size_x
-        thresh_y = y_offset + (n_positive+1) * (box_size_y + box_gap) - box_gap*0.5
-        ax.hlines(y=thresh_y, xmin=thresh_x_start, xmax=thresh_x_end, color='orange', linestyle='--')
-
     # Styling and save
     ax.set_xlim(0, width*1.1) # location 的文字太长了，所以要加长一点
     ax.set_ylim(height, 0)
     ax.axis('off')
 
     # # This will make the subplot(s) expand to fill the entire figure area, with no padding on any side. 
     # # In brief, make the plot bigger (not influence the font size)
```

## Comparing `offtracker-2.7.10/offtracker/X_offtracker.py` & `offtracker-2.7.8/offtracker/X_offtracker.py`

 * *Files identical despite different names*

## Comparing `offtracker-2.7.10/offtracker/X_sequence.py` & `offtracker-2.7.8/offtracker/X_sequence.py`

 * *Files identical despite different names*

## Comparing `offtracker-2.7.10/offtracker/_version.py` & `offtracker-2.7.8/offtracker/_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-__version__ = "2.7.10"
+__version__ = "2.7.8"
 # 2023.08.11. v1.1.0	adding a option for not normalizing the bw file
 # 2023.10.26. v1.9.0	prerelease for v2.0
 # 2023.10.27. v2.0.0	大更新，还没微调
-# 2023.10.28. v2.1.0	修复bug，增加计算信号长度的功能
-# 2023.10.28. v2.2.0	修复bug，改变计算信号长度的算法
-# 2023.10.29. v2.3.0	增加 overall signal 计算
-# 2023.11.01. v2.3.1	增加 signal_only 选项
-# 2023.11.02. v2.3.2	修改 sample signal 和 group mean 的计算顺序
-# 2023.11.04. v2.3.3	修复 overall score 标准化时排序错误的问题
-# 2023.11.05. v2.3.4	修复判断单边溢出信号时的列名选取错误
-# 2023.11.13. v2.3.5	微调 track score
-# 2023.12.05. v2.3.6	candidates 增加 cleavage site，修正 alignment 有 deletion 会错位的 bug
-# 2023.12.05. v2.3.7	用 cleavage site 代替 midpoint # 还没改完
-# 2023.12.07. v2.3.8	df_score 增加 df_exp, df_ctr 各自列。修复没 df_ctr 时的 bug。track score 用 proximal
-# 2023.12.09. v2.4.0	为了兼顾 proximal 和 overall，当 normalized overall signal 高于 2 时，增加 overall signal 的加分
-# 2023.12.09. v2.5.0	尝试新的加权位置
-# 2023.12.10. v2.6.0	加入 trackseq v4 的计算分支，即考虑 Region 内的 positive_pct，避免短而尖锐的信号
-# 2023.12.10. v2.6.1	有些非特异信号数值很大，如果在 control 组是大负数，可能导致减 control 后假高信号，因此给负数一个 clip
-# 2023.12.30. v2.7.0	增加 X_offplot 模块，用于绘图
-# 2023.12.31. v2.7.1	control 的负数值 clip 由 -5 改为 -1，进一步减少假阳性。另外不加 overall 了
-# 2024.01.01. v2.7.2	权重改为 proximal + pct = 1 + 1. 防信号外溢假阳性标准由<0改为<=0
-# 2024.01.02. v2.7.3	flank regions 默认值改为 1000 2000 3000 5000。之前 control 的负数值 clip 相当于直接在 final score，现在改为每个单独 clip 后重新算 score，默认值为 CtrClip=-0.5
-# 2024.01.03. v2.7.4	更新了 blacklist.bed
-# 2024.01.04. v2.7.5	更新了 hg38 blacklist.bed
-# 2024.01.12. v2.7.6	修复小bug，输出 fdr 改为 <0.05。
-# 2024.01.23. v2.7.7	Snakefile_offtracker: add --fixedStep to bigwigCompare for not merging neighbouring bins with equal values.
-# 2024.02.01. v2.7.8	逐步添加 X_offplot.py 功能
-# 2024.06.02. v2.7.9	添加 offtracker_plot.py
-# 2024.06.03. v2.7.10	修复 bugs，offtable 添加 threshold = 2 的分界
+# 2023.10.28. v2.1.0 修复bug，增加计算信号长度的功能
+# 2023.10.28. v2.2.0 修复bug，改变计算信号长度的算法
+# 2023.10.29. v2.3.0 增加 overall signal 计算
+# 2023.11.01. v2.3.1 增加 signal_only 选项
+# 2023.11.02. v2.3.2 修改 sample signal 和 group mean 的计算顺序
+# 2023.11.04. v2.3.3 修复 overall score 标准化时排序错误的问题
+# 2023.11.05. v2.3.4 修复判断单边溢出信号时的列名选取错误
+# 2023.11.13. v2.3.5 微调 track score
+# 2023.12.05. v2.3.6 candidates 增加 cleavage site，修正 alignment 有 deletion 会错位的 bug
+# 2023.12.05. v2.3.7 用 cleavage site 代替 midpoint # 还没改完
+# 2023.12.07. v2.3.8 df_score 增加 df_exp, df_ctr 各自列。修复没 df_ctr 时的 bug。track score 用 proximal
+# 2023.12.09. v2.4.0 为了兼顾 proximal 和 overall，当 normalized overall signal 高于 2 时，增加 overall signal 的加分
+# 2023.12.09. v2.5.0 尝试新的加权位置
+# 2023.12.10. v2.6.0 加入 trackseq v4 的计算分支，即考虑 Region 内的 positive_pct，避免短而尖锐的信号
+# 2023.12.10. v2.6.1 有些非特异信号数值很大，如果在 control 组是大负数，可能导致减 control 后假高信号，因此给负数一个 clip
+# 2023.12.30. v2.7.0 增加 X_offplot 模块，用于绘图
+# 2023.12.31. v2.7.1 control 的负数值 clip 由 -5 改为 -1，进一步减少假阳性。另外不加 overall 了
+# 2024.01.01. v2.7.2 权重改为 proximal + pct = 1 + 1. 防信号外溢假阳性标准由<0改为<=0
+# 2024.01.02. v2.7.3 flank regions 默认值改为 1000 2000 3000 5000。之前 control 的负数值 clip 相当于直接在 final score，现在改为每个单独 clip 后重新算 score，默认值为 CtrClip=-0.5
+# 2024.01.03. v2.7.4 更新了 blacklist.bed
+# 2024.01.04. v2.7.5 更新了 hg38 blacklist.bed
+# 2024.01.12. v2.7.6 修复小bug，输出 fdr 改为 <0.05。
+# 2024.01.23. v2.7.7 Snakefile_offtracker: add --fixedStep to bigwigCompare for not merging neighbouring bins with equal values.
+# 2024.02.01. v2.7.8 逐步添加 X_offplot.py 功能
```

## Comparing `offtracker-2.7.10/offtracker/mapping/1.1_bed2fr_v4.5.py` & `offtracker-2.7.8/offtracker/mapping/1.1_bed2fr_v4.5.py`

 * *Files identical despite different names*

## Comparing `offtracker-2.7.10/offtracker/mapping/1.3_bdg_normalize_v4.0.py` & `offtracker-2.7.8/offtracker/mapping/1.3_bdg_normalize_v4.0.py`

 * *Files identical despite different names*

## Comparing `offtracker-2.7.10/offtracker/mapping/bedGraphToBigWig` & `offtracker-2.7.8/offtracker/mapping/bedGraphToBigWig`

 * *Files identical despite different names*

## Comparing `offtracker-2.7.10/offtracker/mapping/hg38.chrom.sizes` & `offtracker-2.7.8/offtracker/mapping/hg38.chrom.sizes`

 * *Files identical despite different names*

## Comparing `offtracker-2.7.10/offtracker/mapping/mm10.chrom.sizes` & `offtracker-2.7.8/offtracker/mapping/mm10.chrom.sizes`

 * *Files identical despite different names*

## Comparing `offtracker-2.7.10/offtracker/mapping/offtracker_blacklist_hg38.merged.bed` & `offtracker-2.7.8/offtracker/mapping/offtracker_blacklist_hg38.merged.bed`

 * *Files identical despite different names*

## Comparing `offtracker-2.7.10/offtracker/mapping/offtracker_blacklist_mm10.merged.bed` & `offtracker-2.7.8/offtracker/mapping/offtracker_blacklist_mm10.merged.bed`

 * *Files identical despite different names*

## Comparing `offtracker-2.7.10/offtracker/mapping/Snakefile_offtracker` & `offtracker-2.7.8/offtracker/mapping/Snakefile_offtracker`

 * *Files identical despite different names*

## Comparing `offtracker-2.7.10/offtracker.egg-info/SOURCES.txt` & `offtracker-2.7.8/offtracker.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -18,9 +18,8 @@
 offtracker/mapping/bedGraphToBigWig
 offtracker/mapping/hg38.chrom.sizes
 offtracker/mapping/mm10.chrom.sizes
 offtracker/mapping/offtracker_blacklist_hg38.merged.bed
 offtracker/mapping/offtracker_blacklist_mm10.merged.bed
 scripts/offtracker_analysis.py
 scripts/offtracker_candidates.py
-scripts/offtracker_config.py
-scripts/offtracker_plot.py
+scripts/offtracker_config.py
```

## Comparing `offtracker-2.7.10/scripts/offtracker_analysis.py` & `offtracker-2.7.8/scripts/offtracker_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     parser = argparse.ArgumentParser()
     parser.description='Analyze the Tracking-seq data.'
     parser.add_argument('-f','--folder'  , type=str, required=True,    nargs='+', help='Directory of the data folder.' )
     parser.add_argument('--seqfolder'    , type=str, required=True,    help='folder containing df_candidate created by offtracker_cadidates.py.')
     parser.add_argument('--name'         , type=str, required=True,    help='custom name of the sgRNA' )
     parser.add_argument('--exp'          , type=str, default='all',    nargs='+', help='A substring mark in the name of experimental samples. The default is to use all samples other than control' )
     parser.add_argument('--control'      , type=str, default='none',   nargs='+', help='A substring mark in the name of control samples. The default is no control. "others" for all samples other than --exp.' )
-    parser.add_argument('--fdr'          , type=int, default=0.05,     help='FDR threshold for the final result. Default is 0.05.')
     parser.add_argument('--smooth'       , type=int, default=1,        help='Smooth strength for the signal.')
     parser.add_argument('--window'       , type=int, default=3,        help='Window size for smoothing the signal.')
     parser.add_argument('--binsize'      , type=int, default=100,      help='Window size for smoothing the signal.')
     parser.add_argument('--flank_max'    , type=int, default=100000,   help='Maximun flanking distance from the candidate site.')
     parser.add_argument('--flank_regions', type=int, default=[1000,2000,3000,5000], nargs='+',help='flanking regions for calculating signal.')
     parser.add_argument('--SeqScorePower', type=float, default=4,      help='The seq score power' )
     parser.add_argument('--CtrClip'      , type=float, default=-0.5,     help='The lower clip for control samples' )
@@ -46,15 +45,14 @@
 
     print(f'Runing offtracker verision: {offtracker.__version__}')
     # main parameters
     folders = args.folder
     sgRNA_name = args.name
     pattern_exp = args.exp
     pattern_ctr = args.control
-    fdr_thresh = args.fdr
     binsize = args.binsize
     flank_max = args.flank_max
     flank_regions = args.flank_regions
     smooth_times = args.smooth
     window_size = args.window
     seq_score_power = args.SeqScorePower
     n_threads  = args.thread
@@ -153,19 +151,16 @@
         if (os.path.isfile(output))&(not args.overwrite):
             print(output, 'exists, skipped')
             continue
         df_bdg = xseq.read_bed(a_file)
         df_bdg.columns = ['chr','start','end','residual']
         # 将 df_bdg 按照染色体分组
         sample_groups = df_bdg.groupby('chr')
-        # 2024.06.03. fix a bug that df_bdg has less chr than df_candidate
-        total_chr = df_bdg['chr'].unique()
-        df_candidate_sub_temp = df_candidate_sub[df_candidate_sub['chr'].isin(total_chr)]
         # 将 df_candidate_sub 按照染色体分组
-        candidate_groups = df_candidate_sub_temp.groupby('chr')
+        candidate_groups = df_candidate_sub.groupby('chr')
 
         # 定义一个空的列表，用于存储每个染色体的数据
         chrom_list = []
         # 遍历分组后的数据
         list_index = []
         for chr_name, chr_candidate in candidate_groups:
             # 获取当前染色体对应的 df_sample 数据
@@ -235,16 +230,15 @@
             # df_exp[cols_clip] = df_exp[cols_clip].clip(lower=-1)
             # df_group_signal = df_exp - df_ctr
             df_exp.columns = 'exp_' + df_exp.columns
             df_ctr.columns = 'ctr_' + df_ctr.columns
             df_score = pd.concat([df_score, df_exp, df_ctr], axis=1)
         else:
             df_score = pd.concat([df_score, df_exp], axis=1)
-        # 2024.06.03. 跑样例数据时，只有一个 chr6, 其他都是 nan, 不删除会导致后续计算出错
-        df_score = df_score.dropna().copy()
+        df_score = df_score.copy()
         df_score.to_csv(output)
     
     ##########################
     ## filter and normalize ##
     ##########################
     output = f'./temp/df_result_{outname}.csv'
     if (os.path.isfile(output))&(not args.overwrite):
@@ -341,18 +335,16 @@
         print('mean_score:{:.3f};std:{:.3f}'.format(mu,std))
         # pv and fdr
         df_result['pv'] = df_result[f'log2_track_score'].apply( lambda x: norm.sf(x,loc=mu,scale=std) )
         df_result['pv'].clip(lower=1e-320,inplace=True)
         df_result['fdr'] = offtracker.fdr(df_result['pv'])
         df_result['rank'] = range(1,len(df_result)+1)
         df_result.to_csv(output)        
-        # 2024.06.03. 以防 fdr<=fdr_thresh 滤掉了 track_score>=2 的位点
-        bool_fdr = df_result['fdr']<=fdr_thresh
-        bool_score = df_result['track_score']>=2
-        df_output = df_result[bool_fdr|bool_score].copy()
+
+        df_output = df_result[df_result['fdr']<=0.05].copy()
         if pattern_ctr != 'none':
             df_output = df_output[['target_location', 'best_strand','best_target','deletion','insertion','mismatch',
                                    'exp_L_length', 'exp_R_length','ctr_L_length','ctr_R_length','L_length','R_length','signal_length',
                                   'norm_best_seq_score','track_score', 'log2_track_score','fdr','rank']]
             df_output.columns = ['target_location', 'strand', 'target', 'deletion', 'insertion', 'mismatch', 
                                  'exp_L_length', 'exp_R_length','ctr_L_length','ctr_R_length','L_length','R_length','signal_length',
                                  'seq_score', 'track_score', 'log2_track_score','FDR', 'rank']
```

## Comparing `offtracker-2.7.10/scripts/offtracker_candidates.py` & `offtracker-2.7.8/scripts/offtracker_candidates.py`

 * *Files identical despite different names*

## Comparing `offtracker-2.7.10/scripts/offtracker_config.py` & `offtracker-2.7.8/scripts/offtracker_config.py`

 * *Files identical despite different names*

