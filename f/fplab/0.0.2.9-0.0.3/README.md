# Comparing `tmp/fplab-0.0.2.9.tar.gz` & `tmp/fplab-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fplab-0.0.2.9.tar", last modified: Wed May  1 02:39:30 2024, max compression
+gzip compressed data, was "fplab-0.0.3.tar", last modified: Mon Jun  3 13:46:00 2024, max compression
```

## Comparing `fplab-0.0.2.9.tar` & `fplab-0.0.3.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.233081 fplab-0.0.2.9/
--rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.2.9/LICENSE.txt
--rw-rw-rw-   0        0        0      523 2024-05-01 02:39:30.233081 fplab-0.0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      862 2024-04-06 15:56:56.000000 fplab-0.0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.125388 fplab-0.0.2.9/fplab/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.9/fplab/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.154546 fplab-0.0.2.9/fplab/enhancement/
--rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.2.9/fplab/enhancement/__init__.py
--rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.2.9/fplab/enhancement/frequency.py
--rw-rw-rw-   0        0        0     4907 2024-04-26 16:08:32.000000 fplab-0.0.2.9/fplab/enhancement/spatial.py
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.154546 fplab-0.0.2.9/fplab/generation/
--rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.2.9/fplab/generation/__init__.py
--rw-rw-rw-   0        0        0     9898 2024-04-27 05:54:42.000000 fplab-0.0.2.9/fplab/generation/distortion.py
--rw-rw-rw-   0        0        0     3304 2024-04-26 16:52:24.000000 fplab-0.0.2.9/fplab/generation/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.154546 fplab-0.0.2.9/fplab/intrinsic/
--rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.2.9/fplab/intrinsic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.170166 fplab-0.0.2.9/fplab/intrinsic/frequency/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.9/fplab/intrinsic/frequency/__init__.py
--rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.2.9/fplab/intrinsic/frequency/projection.py
--rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.2.9/fplab/intrinsic/frequency/tools.py
--rw-rw-rw-   0        0        0     3116 2024-04-07 04:59:12.000000 fplab-0.0.2.9/fplab/intrinsic/frequency/transform.py
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.185792 fplab-0.0.2.9/fplab/intrinsic/mask/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.9/fplab/intrinsic/mask/__init__.py
--rw-rw-rw-   0        0        0      855 2024-04-06 15:25:34.000000 fplab-0.0.2.9/fplab/intrinsic/mask/mask.py
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.185792 fplab-0.0.2.9/fplab/intrinsic/multiple/
--rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.2.9/fplab/intrinsic/multiple/__init__.py
--rw-rw-rw-   0        0        0     6990 2024-04-07 05:24:47.000000 fplab-0.0.2.9/fplab/intrinsic/multiple/transform.py
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.201818 fplab-0.0.2.9/fplab/intrinsic/orientation/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.9/fplab/intrinsic/orientation/__init__.py
--rw-rw-rw-   0        0        0     9285 2024-05-01 02:37:08.000000 fplab-0.0.2.9/fplab/intrinsic/orientation/gradient.py
--rw-rw-rw-   0        0        0     6215 2024-04-07 04:39:10.000000 fplab-0.0.2.9/fplab/intrinsic/orientation/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.201818 fplab-0.0.2.9/fplab/intrinsic/skeleton/
--rw-rw-rw-   0        0        0        0 2024-04-06 15:22:02.000000 fplab-0.0.2.9/fplab/intrinsic/skeleton/__init__.py
--rw-rw-rw-   0        0        0     1752 2024-04-06 16:14:50.000000 fplab-0.0.2.9/fplab/intrinsic/skeleton/skeleton.py
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.201818 fplab-0.0.2.9/fplab/matching/
--rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.2.9/fplab/matching/__init__.py
--rw-rw-rw-   0        0        0     6956 2024-03-30 03:40:09.000000 fplab-0.0.2.9/fplab/matching/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.217455 fplab-0.0.2.9/fplab/minutiae/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.9/fplab/minutiae/__init__.py
--rw-rw-rw-   0        0        0     6782 2024-04-14 14:52:02.000000 fplab-0.0.2.9/fplab/minutiae/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.233081 fplab-0.0.2.9/fplab/tools/
--rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.2.9/fplab/tools/__init__.py
--rw-rw-rw-   0        0        0    13732 2024-04-06 14:10:17.000000 fplab-0.0.2.9/fplab/tools/array.py
--rw-rw-rw-   0        0        0     5367 2024-04-06 14:01:28.000000 fplab-0.0.2.9/fplab/tools/image.py
--rw-rw-rw-   0        0        0    15076 2024-04-06 09:13:19.000000 fplab-0.0.2.9/fplab/tools/nbis.py
--rw-rw-rw-   0        0        0    15788 2024-04-06 14:10:17.000000 fplab-0.0.2.9/fplab/tools/tensor.py
-drwxrwxrwx   0        0        0        0 2024-05-01 02:39:30.138901 fplab-0.0.2.9/fplab.egg-info/
--rw-rw-rw-   0        0        0      523 2024-05-01 02:39:30.000000 fplab-0.0.2.9/fplab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2024-05-01 02:39:30.000000 fplab-0.0.2.9/fplab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 02:39:30.000000 fplab-0.0.2.9/fplab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-01 02:39:30.000000 fplab-0.0.2.9/fplab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 02:39:30.233081 fplab-0.0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      801 2024-05-01 02:35:48.000000 fplab-0.0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.167638 fplab-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2024-03-31 02:38:30.000000 fplab-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      521 2024-06-03 13:46:00.167638 fplab-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      862 2024-04-06 15:56:56.000000 fplab-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.013628 fplab-0.0.3/fplab/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.3/fplab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.047095 fplab-0.0.3/fplab/enhancement/
+-rw-rw-rw-   0        0        0        0 2024-03-31 08:36:57.000000 fplab-0.0.3/fplab/enhancement/__init__.py
+-rw-rw-rw-   0        0        0     4472 2024-03-31 08:36:57.000000 fplab-0.0.3/fplab/enhancement/frequency.py
+-rw-rw-rw-   0        0        0     4907 2024-04-26 16:08:32.000000 fplab-0.0.3/fplab/enhancement/spatial.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.064336 fplab-0.0.3/fplab/generation/
+-rw-rw-rw-   0        0        0        0 2024-04-02 15:51:38.000000 fplab-0.0.3/fplab/generation/__init__.py
+-rw-rw-rw-   0        0        0     9898 2024-04-27 05:54:42.000000 fplab-0.0.3/fplab/generation/distortion.py
+-rw-rw-rw-   0        0        0     3304 2024-04-26 16:52:24.000000 fplab-0.0.3/fplab/generation/tools.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.065339 fplab-0.0.3/fplab/intrinsic/
+-rw-rw-rw-   0        0        0        0 2024-03-23 06:49:44.000000 fplab-0.0.3/fplab/intrinsic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.088450 fplab-0.0.3/fplab/intrinsic/frequency/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.3/fplab/intrinsic/frequency/__init__.py
+-rw-rw-rw-   0        0        0     7577 2024-03-31 08:36:57.000000 fplab-0.0.3/fplab/intrinsic/frequency/projection.py
+-rw-rw-rw-   0        0        0    10795 2024-03-31 08:36:57.000000 fplab-0.0.3/fplab/intrinsic/frequency/tools.py
+-rw-rw-rw-   0        0        0     3116 2024-04-07 04:59:12.000000 fplab-0.0.3/fplab/intrinsic/frequency/transform.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.097776 fplab-0.0.3/fplab/intrinsic/mask/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.3/fplab/intrinsic/mask/__init__.py
+-rw-rw-rw-   0        0        0      855 2024-04-06 15:25:34.000000 fplab-0.0.3/fplab/intrinsic/mask/mask.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.106389 fplab-0.0.3/fplab/intrinsic/multiple/
+-rw-rw-rw-   0        0        0        0 2024-03-23 07:06:33.000000 fplab-0.0.3/fplab/intrinsic/multiple/__init__.py
+-rw-rw-rw-   0        0        0     6990 2024-04-07 05:24:47.000000 fplab-0.0.3/fplab/intrinsic/multiple/transform.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.122362 fplab-0.0.3/fplab/intrinsic/orientation/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.3/fplab/intrinsic/orientation/__init__.py
+-rw-rw-rw-   0        0        0     9285 2024-05-01 02:37:08.000000 fplab-0.0.3/fplab/intrinsic/orientation/gradient.py
+-rw-rw-rw-   0        0        0     6215 2024-04-07 04:39:10.000000 fplab-0.0.3/fplab/intrinsic/orientation/tools.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.130800 fplab-0.0.3/fplab/intrinsic/skeleton/
+-rw-rw-rw-   0        0        0        0 2024-04-06 15:22:02.000000 fplab-0.0.3/fplab/intrinsic/skeleton/__init__.py
+-rw-rw-rw-   0        0        0     1752 2024-04-06 16:14:50.000000 fplab-0.0.3/fplab/intrinsic/skeleton/skeleton.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.134234 fplab-0.0.3/fplab/matching/
+-rw-rw-rw-   0        0        0        0 2024-03-29 01:34:29.000000 fplab-0.0.3/fplab/matching/__init__.py
+-rw-rw-rw-   0        0        0    12309 2024-06-03 12:09:16.000000 fplab-0.0.3/fplab/matching/mcc.py
+-rw-rw-rw-   0        0        0     7080 2024-06-03 11:45:19.000000 fplab-0.0.3/fplab/matching/tools.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.141963 fplab-0.0.3/fplab/minutiae/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.3/fplab/minutiae/__init__.py
+-rw-rw-rw-   0        0        0     6782 2024-04-14 14:52:02.000000 fplab-0.0.3/fplab/minutiae/tools.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.165458 fplab-0.0.3/fplab/tools/
+-rw-rw-rw-   0        0        0        0 2024-03-02 09:02:14.000000 fplab-0.0.3/fplab/tools/__init__.py
+-rw-rw-rw-   0        0        0    13732 2024-04-06 14:10:17.000000 fplab-0.0.3/fplab/tools/array.py
+-rw-rw-rw-   0        0        0     5588 2024-06-03 07:49:05.000000 fplab-0.0.3/fplab/tools/image.py
+-rw-rw-rw-   0        0        0    15075 2024-06-03 04:25:06.000000 fplab-0.0.3/fplab/tools/nbis.py
+-rw-rw-rw-   0        0        0    15788 2024-04-06 14:10:17.000000 fplab-0.0.3/fplab/tools/tensor.py
+drwxrwxrwx   0        0        0        0 2024-06-03 13:46:00.031649 fplab-0.0.3/fplab.egg-info/
+-rw-rw-rw-   0        0        0      521 2024-06-03 13:45:59.000000 fplab-0.0.3/fplab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1080 2024-06-03 13:45:59.000000 fplab-0.0.3/fplab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 13:45:59.000000 fplab-0.0.3/fplab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-06-03 13:45:59.000000 fplab-0.0.3/fplab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-03 13:46:00.168823 fplab-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      799 2024-06-03 12:05:29.000000 fplab-0.0.3/setup.py
```

### Comparing `fplab-0.0.2.9/LICENSE.txt` & `fplab-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/PKG-INFO` & `fplab-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.2.9
+Version: 0.0.3
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.2.9/README.md` & `fplab-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/enhancement/frequency.py` & `fplab-0.0.3/fplab/enhancement/frequency.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/enhancement/spatial.py` & `fplab-0.0.3/fplab/enhancement/spatial.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/generation/distortion.py` & `fplab-0.0.3/fplab/generation/distortion.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/generation/tools.py` & `fplab-0.0.3/fplab/generation/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/intrinsic/frequency/projection.py` & `fplab-0.0.3/fplab/intrinsic/frequency/projection.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/intrinsic/frequency/tools.py` & `fplab-0.0.3/fplab/intrinsic/frequency/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/intrinsic/frequency/transform.py` & `fplab-0.0.3/fplab/intrinsic/frequency/transform.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/intrinsic/mask/mask.py` & `fplab-0.0.3/fplab/intrinsic/mask/mask.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/intrinsic/multiple/transform.py` & `fplab-0.0.3/fplab/intrinsic/multiple/transform.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/intrinsic/orientation/gradient.py` & `fplab-0.0.3/fplab/intrinsic/orientation/gradient.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/intrinsic/orientation/tools.py` & `fplab-0.0.3/fplab/intrinsic/orientation/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/intrinsic/skeleton/skeleton.py` & `fplab-0.0.3/fplab/intrinsic/skeleton/skeleton.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/matching/tools.py` & `fplab-0.0.3/fplab/matching/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     rk表示匹配分数阈值，可以为一维数组或整数"""
     if isinstance(rk, int):
         ranks = np.linspace(score.min(), score.max(), rk)
     elif isinstance(rk, np.ndarray):
         ranks = rk
     else:
         ranks = np.linspace(score.min(), score.max(), num=8)
-    ranks = np.round(ranks, 2)
+    ranks = np.round(ranks, 5)
     out = {}
     genuine, imposter = [], []
     for i in range(score.shape[0]):
         p_list = paired_list[i]
         for j in range(score.shape[1]):
             if j in p_list:
                 genuine.append(score[i, j])
@@ -112,20 +112,21 @@
                     "average": round((pf_ft_r+pt_ff_r)/2, 2)}
         difference.append(np.abs(pf_ft_r-pt_ff_r))
         average.append((pf_ft_r+pt_ff_r)/2)
     eer = average[np.argmin(np.array(difference))]
     return out, eer, genuine, imposter
 
 
-def analyse_score(score, p_dirs, g_dirs, script_stem, rk_i=None, rk_v=None, j_func=None, **kwargs):
+def analyse_score(score, p_dirs, g_dirs, script_stem, rk_i=None, rk_v=None, j_func=None, need_eer=False, **kwargs):
     """分析匹配矩阵score
     score是匹配器产生的匹配分数矩阵，行对应目标指纹，列对应库指纹
     p_dirs和g_dirs是目标指纹和库指纹的地址列表，分别与score的行列对应
     script_stem是所有生成的文本文件的前缀，需要为字符串形式
     rk_i，rk_v分别表示识别的rank-n和匹配的分数阈值，可以为一维数组或整数
+    need_eer是否输出eer
     j_func，**kwargs用于判断p_dirs和g_dirs的匹配项，使用方法见get_paired"""
     paired_list = get_paired(p_dirs, g_dirs, j_func=j_func, **kwargs)
     out_identify = analyse_score_identify(score, paired_list, rk=rk_i)
     out_verify, eer, genuine, imposter = analyse_score_verify(score, paired_list, rk=rk_v)
     paired_file = Path(script_stem) / 'paired_list.txt'
     analyse_file = Path(script_stem) / 'analyse.txt'
     analyse_fig = Path(script_stem) / 'verify_out.png'
@@ -151,8 +152,11 @@
         af.write(f"相等错误率：{eer}\n")
         af.write(f"score:\tpt_ft_n\tpf_ft_n\tpt_ff_n\tpf_ff_n\tpf_ft_r\tpt_ff_r\tdifference\taverage\n")
         for k, v in out_verify.items():
             af.write(f"{k}:\t{v['pt_ft_n']}\t{v['pf_ft_n']}\t{v['pt_ff_n']}\t{v['pf_ff_n']}\t"
                      f"{v['pf_ft_r']}\t{v['pt_ff_r']}\t{v['difference']}\t{v['average']}\n")
     plt.hist([genuine, imposter], 40, (score.min(), score.max()), density=True)
     plt.savefig(analyse_fig)
-    return out_identify, out_verify
+    if need_eer:
+        return out_identify, out_verify, eer
+    else:
+        return out_identify, out_verify
```

### Comparing `fplab-0.0.2.9/fplab/minutiae/tools.py` & `fplab-0.0.3/fplab/minutiae/tools.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/tools/array.py` & `fplab-0.0.3/fplab/tools/array.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab/tools/image.py` & `fplab-0.0.3/fplab/tools/image.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                 if 'Extensions:' in s2:
                     for s3 in s2.split(' '):
                         if '.' in s3:
                             ext.append(s3)
     return ext
 
 
-def get_data_dirs(data_folder_path, data_dirs, ext=None, top_flag=True):
+def get_data_dirs(data_folder_path, data_dirs, ext=None, top_flag=True, specified_content=None):
     """
     获得data_folder_path路径下的所有指定格式ext（默认为PIL库支持读取的所有格式）的文件的绝对路径字符串列表
     当top_flag为True时，会对输出字符串排序
     data_folder_path是一个Path对象, data_dirs是一个字符串列表，ext是一个字符串列表，top_flag为布尔值
     """
     if not ext:
         ext = get_support_extensions()
@@ -47,14 +47,20 @@
         data_folder_p = data_folder_path
     for path in data_folder_p.iterdir():
         if path.is_dir():
             data_dirs = get_data_dirs(path, data_dirs, ext=ext, top_flag=False)
         elif path.suffix in ext:
             data_dirs.append(str(path.absolute()))
     if top_flag:
+        if specified_content:
+            temp = []
+            for d in data_dirs:
+                if specified_content in d:
+                    temp.append(d)
+            data_dirs = temp
         data_dirs = sorted(data_dirs)
     return data_dirs
 
 
 def type_as(im, md="t", device=None):
     """将im转化为指定类型
     md可以为"t"（张量形式），"a"（数组形式）或是图像
```

### Comparing `fplab-0.0.2.9/fplab/tools/nbis.py` & `fplab-0.0.3/fplab/tools/nbis.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         temp_path = Path(temp_dir)
     else:
         temp_path = Path("temp_images")
     if temp_flag:
         temp_path.mkdir(parents=True, exist_ok=True)
     out = []
     with tqdm(total=len(im_dirs)) as pbar:
-        pbar.set_description("正在提取细节点:")
+        pbar.set_description("正在提取细节点")
         for im_dir in im_dirs:
             save_dir = im_dir.replace(root_dir, out_dir).split(".")[0]
             Path(save_dir).parent.mkdir(parents=True, exist_ok=True)
             if temp_flag:
                 im_d = change_image(Path(im_dir), sv_pt=temp_path, ext='.png', dpi=(500, 500), md="L")
                 im_d = str(im_d.absolute())
             else:
```

### Comparing `fplab-0.0.2.9/fplab/tools/tensor.py` & `fplab-0.0.3/fplab/tools/tensor.py`

 * *Files identical despite different names*

### Comparing `fplab-0.0.2.9/fplab.egg-info/PKG-INFO` & `fplab-0.0.3/fplab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fplab
-Version: 0.0.2.9
+Version: 0.0.3
 Summary: Python3 Package for Fingerprint Processing
 Author: Yurun Wang
 Author-email: wangyurun@mail.sdu.edu.cn
 License: MIT
 Keywords: python,fingerprint
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fplab-0.0.2.9/fplab.egg-info/SOURCES.txt` & `fplab-0.0.3/fplab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 fplab/intrinsic/multiple/transform.py
 fplab/intrinsic/orientation/__init__.py
 fplab/intrinsic/orientation/gradient.py
 fplab/intrinsic/orientation/tools.py
 fplab/intrinsic/skeleton/__init__.py
 fplab/intrinsic/skeleton/skeleton.py
 fplab/matching/__init__.py
+fplab/matching/mcc.py
 fplab/matching/tools.py
 fplab/minutiae/__init__.py
 fplab/minutiae/tools.py
 fplab/tools/__init__.py
 fplab/tools/array.py
 fplab/tools/image.py
 fplab/tools/nbis.py
```

### Comparing `fplab-0.0.2.9/setup.py` & `fplab-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2.9'
+VERSION = '0.0.3'
 DESCRIPTION = 'Python3 Package for Fingerprint Processing'
 LONG_DESCRIPTION = ('This is a python3 package for fingerprint processing,'
                     ' which can be used for fingerprint enhancement.')
 
 setup(
     name="fplab",
     version=VERSION,
```

