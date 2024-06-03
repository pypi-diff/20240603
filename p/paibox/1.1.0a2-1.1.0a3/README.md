# Comparing `tmp/paibox-1.1.0a2.tar.gz` & `tmp/paibox-1.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paibox-1.1.0a2.tar", max compression
+gzip compressed data, was "paibox-1.1.0a3.tar", max compression
```

## Comparing `paibox-1.1.0a2.tar` & `paibox-1.1.0a3.tar`

### file list

```diff
@@ -1,48 +1,47 @@
--rw-r--r--   0        0        0     1371 2024-05-21 11:46:16.796567 paibox-1.1.0a2/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-05-21 11:46:16.796567 paibox-1.1.0a2/LICENSE
--rw-r--r--   0        0        0      958 2024-05-21 11:46:16.796567 paibox-1.1.0a2/README.md
--rw-r--r--   0        0        0    37145 2024-05-21 11:46:16.800567 paibox-1.1.0a2/docs/Guide-of-PAIBox.md
--rw-r--r--   0        0        0     2816 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/__init__.py
--rw-r--r--   0        0        0      150 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/__init__.py
--rw-r--r--   0        0        0      394 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/checker.py
--rw-r--r--   0        0        0    16085 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/conf_template.py
--rw-r--r--   0        0        0     2079 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/constrs.py
--rw-r--r--   0        0        0     3112 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/context.py
--rw-r--r--   0        0        0    20470 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/graphs.py
--rw-r--r--   0        0        0     1228 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/graphs_types.py
--rw-r--r--   0        0        0    24207 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/mapper.py
--rw-r--r--   0        0        0    25600 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/placement.py
--rw-r--r--   0        0        0    21588 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/routing.py
--rw-r--r--   0        0        0    12062 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/backend/segment_utils.py
--rw-r--r--   0        0        0    10304 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/base.py
--rw-r--r--   0        0        0     5168 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/collector.py
--rw-r--r--   0        0        0      143 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/__init__.py
--rw-r--r--   0        0        0    30230 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/functional.py
--rw-r--r--   0        0        0    12086 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/modules.py
--rw-r--r--   0        0        0       25 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/neuron/__init__.py
--rw-r--r--   0        0        0    18494 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/neuron/base.py
--rw-r--r--   0        0        0     5632 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/neuron/neurons.py
--rw-r--r--   0        0        0      775 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/neuron/utils.py
--rw-r--r--   0        0        0     5238 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/projection.py
--rw-r--r--   0        0        0       88 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/synapses/__init__.py
--rw-r--r--   0        0        0    12804 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/synapses/base.py
--rw-r--r--   0        0        0      714 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/synapses/conv_types.py
--rw-r--r--   0        0        0    20753 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/synapses/conv_utils.py
--rw-r--r--   0        0        0     9036 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/synapses/synapses.py
--rw-r--r--   0        0        0    15277 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/components/synapses/transforms.py
--rw-r--r--   0        0        0     1704 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/context.py
--rw-r--r--   0        0        0     1791 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/exceptions.py
--rw-r--r--   0        0        0     7091 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/mixin.py
--rw-r--r--   0        0        0     1567 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/naming.py
--rw-r--r--   0        0        0     5322 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/network.py
--rw-r--r--   0        0        0      417 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/node.py
--rw-r--r--   0        0        0      115 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/simulator/__init__.py
--rw-r--r--   0        0        0     7793 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/simulator/encoder.py
--rw-r--r--   0        0        0     1230 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/simulator/probe.py
--rw-r--r--   0        0        0     6932 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/simulator/simulator.py
--rw-r--r--   0        0        0     1571 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/simulator/utils.py
--rw-r--r--   0        0        0      400 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/tools.py
--rw-r--r--   0        0        0     2239 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/types.py
--rw-r--r--   0        0        0     3164 2024-05-21 11:46:16.804567 paibox-1.1.0a2/paibox/utils.py
--rw-r--r--   0        0        0     2241 2024-05-21 11:46:16.804567 paibox-1.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 paibox-1.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1371 2024-06-03 07:10:42.286971 paibox-1.1.0a3/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-06-03 07:10:42.286971 paibox-1.1.0a3/LICENSE
+-rw-r--r--   0        0        0      983 2024-06-03 07:10:42.286971 paibox-1.1.0a3/README.md
+-rw-r--r--   0        0        0    39555 2024-06-03 07:10:42.286971 paibox-1.1.0a3/docs/Guide-of-PAIBox.md
+-rw-r--r--   0        0        0     2884 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/__init__.py
+-rw-r--r--   0        0        0      150 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/backend/__init__.py
+-rw-r--r--   0        0        0      394 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/backend/checker.py
+-rw-r--r--   0        0        0    16074 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/backend/conf_template.py
+-rw-r--r--   0        0        0     2076 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/backend/constrs.py
+-rw-r--r--   0        0        0     3100 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/backend/context.py
+-rw-r--r--   0        0        0    32934 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/backend/graphs.py
+-rw-r--r--   0        0        0     1486 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/backend/graphs_types.py
+-rw-r--r--   0        0        0    26429 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/backend/mapper.py
+-rw-r--r--   0        0        0    25691 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/backend/placement.py
+-rw-r--r--   0        0        0    22084 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/backend/routing.py
+-rw-r--r--   0        0        0    12077 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/backend/segment_utils.py
+-rw-r--r--   0        0        0    10303 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/base.py
+-rw-r--r--   0        0        0     5146 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/collector.py
+-rw-r--r--   0        0        0      143 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/__init__.py
+-rw-r--r--   0        0        0    34306 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/functional.py
+-rw-r--r--   0        0        0    13352 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/modules.py
+-rw-r--r--   0        0        0       25 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/neuron/__init__.py
+-rw-r--r--   0        0        0    17945 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/neuron/base.py
+-rw-r--r--   0        0        0     8410 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/neuron/neurons.py
+-rw-r--r--   0        0        0     1672 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/neuron/utils.py
+-rw-r--r--   0        0        0     5643 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/projection.py
+-rw-r--r--   0        0        0       81 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/synapses/__init__.py
+-rw-r--r--   0        0        0    13370 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/synapses/base.py
+-rw-r--r--   0        0        0      707 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/synapses/conv_types.py
+-rw-r--r--   0        0        0    21424 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/synapses/conv_utils.py
+-rw-r--r--   0        0        0     9562 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/synapses/synapses.py
+-rw-r--r--   0        0        0    17128 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/components/synapses/transforms.py
+-rw-r--r--   0        0        0     1698 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/context.py
+-rw-r--r--   0        0        0     1791 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/exceptions.py
+-rw-r--r--   0        0        0     7140 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/mixin.py
+-rw-r--r--   0        0        0     1567 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/naming.py
+-rw-r--r--   0        0        0     5336 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/network.py
+-rw-r--r--   0        0        0      220 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/node.py
+-rw-r--r--   0        0        0       63 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/simulator/__init__.py
+-rw-r--r--   0        0        0     7793 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/simulator/encoder.py
+-rw-r--r--   0        0        0     8054 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/simulator/simulator.py
+-rw-r--r--   0        0        0     1564 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/simulator/utils.py
+-rw-r--r--   0        0        0      400 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/tools.py
+-rw-r--r--   0        0        0      845 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/types.py
+-rw-r--r--   0        0        0     4227 2024-06-03 07:10:42.294971 paibox-1.1.0a3/paibox/utils.py
+-rw-r--r--   0        0        0     1980 2024-06-03 07:10:42.298972 paibox-1.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 paibox-1.1.0a3/PKG-INFO
```

### Comparing `paibox-1.1.0a2/CHANGELOG.md` & `paibox-1.1.0a3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a2/LICENSE` & `paibox-1.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a2/README.md` & `paibox-1.1.0a3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 # PAIBox
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIBox/blob/master/pyproject.toml">
-        <img src="https://img.shields.io/pypi/pyversions/paibox">
+        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/paibox">
     </a>
-    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.1.0a2">
-        <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox?color=orange">
+    <a href="https://pypi.org/project/paibox/">
+        <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/paibox?color=pink">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIBox">
-      <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIBox/master?color=red">
+        <img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIBox?color=orange">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIBox/master">
-	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIBox/master.svg" alt="pre-commit.ci status">
+        <img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/PAICookers/PAIBox/master.svg">
     </a>
 </p>
 
 👉 用户使用指南：[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
 
 高效编写测试项目指南：[Guide-of-Test](docs/Guide-of-Test.md)
```

#### html2text {}

```diff
@@ -1,7 +1,5 @@
                                    # PAIBox
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_a_i_b_o_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
- _v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_?_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/
-    _g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
+_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_C_o_d_e_F_a_c_t_o_r_ _G_r_a_d_e_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
 ð ç¨æ·ä½¿ç¨æåï¼[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
 é«æç¼åæµè¯é¡¹ç®æåï¼[Guide-of-Test](docs/Guide-of-Test.md)
 [Changelog](./CHANGELOG.md)
```

### Comparing `paibox-1.1.0a2/docs/Guide-of-PAIBox.md` & `paibox-1.1.0a3/docs/Guide-of-PAIBox.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,139 +1,126 @@
 <div align="center">
 
 # PAIBox使用指南
 
 </div>
 
-## 快速上手
+## 安装
 
-PAIBox使用 `pyproject.toml` 管理依赖。若使用Poetry：
-
-```bash
-poetry install
-```
-
-或者采用开发版环境
-
-```bash
-poetry install --with dev
-```
-
-若使用conda等，则手动安装如下依赖至Python虚拟环境：
+请安装如下依赖：
 
 ```toml
-python = "^3.8"
+python = "^3.9"
 pydantic = "^2.0"
-numpy = "^1.24.0"
-paicorelib = "^1.1.1"
-orjson = "^3.10.1" # Optional
+numpy = "^1.26.0"
+paicorelib = "^1.1.4"
 ```
 
-通过pip安装PAIBox：
+可选依赖：
 
-```bash
-pip install paibox
+```toml
+orjson = "^3.10.0"
 ```
 
-添加 `--pre` 或克隆 `dev` 分支以使用开发版
+或者从Github克隆，由此下载的PAIBox将包含测试文件、文档等。
 
 ```bash
-git clone -b dev https://github.com/PAICookers/PAIBox.git
+git clone https://github.com/PAICookers/PAIBox.git
 cd PAIBox
 ```
 
 可查看版本号以确认安装：
 
 ```python
 import paibox as pb
 
 print(pb.__version__)
 >>> x.y.z
 ```
 
 ## 基本组件
 
-PAIBox提供**神经元**与**突触**作为基本组件，用于搭建神经网络。
+PAIBox 提供**神经元**与**突触**作为基本组件，用于搭建神经网络。
 
 结合**输入节点**，可以对输入数据进行脉冲编码，并传入网络中进行仿真推理。
 
 ### 神经元
 
-PAIBox提供了多种类型的神经元模型，能够实现各种特殊的功能。
+PAIBox 提供了多种类型的神经元模型，能够实现各种特殊的功能。
 
 神经元均支持 `delay`，`tick_wait_start`，`tick_wait_end`，`keep_shape`，`unrolling_factor` 参数。
 
 ⚠️ 神经元初始膜电位为0。
 
 #### IF
 
-IF神经元实现了经典的“积分发射”模型，其调用方式及参数如下：
+IF 神经元实现了经典的“积分发射”模型，其调用方式及参数如下：
 
 ```python
 import paibox as pb
 
-n1 = pb.IF(shape=10, threshold=127, reset_v=0, keep_shape=False, delay=1, tick_wait_start=1, tick_wait_end=0, name='n1')
+n1 = pb.IF(shape=10, threshold=127, reset_v=0, neg_threshold=-100, keep_shape=False, delay=1, tick_wait_start=1, tick_wait_end=0, name='n1')
 ```
 
 其中：
 
 - `shape`：代表神经元组的尺寸，其形式可以是整形标量、元组或列表。
 - `threshold`：神经元阈值，其形式为整数。
-- `reset_v`：神经元的重置膜电位。
+- `reset_v`：神经元的复位电位，可选参数。当指定时，神经元在发放后，进行硬复位( `v = resetv` )；当未指定时，进行软复位( `v -= pos_threshold` )。默认进行软复位。
+- `neg_threshold`：负阈值，神经元膜电位所允许的最小值，必须是非正整数。当未指定时，默认为硬件所允许的最小负整数。
 - `delay`：设定神经元输出的延迟。默认为1，即本时间步的计算结果，**下一时间步**传递至后继节点。
 - `tick_wait_start`：设定神经元启动时间。神经元将在第 `T` 个时间步时启动。0表示不启动。默认为1。
 - `tick_wait_end`：设定神经元持续工作时长。神经元将持续工作 `T` 个时间步。0表示**持续工作**。默认为0。
 - `unrolling_factor`：该参数与后端流程相关。展开因子表示神经元将被展开，部署至更多的物理核上，以降低延迟并提高吞吐率。
 - `keep_shape`：是否在仿真记录数据时保持尺寸信息，默认为 `False`。实际进行运算的尺寸仍视为一维。
 - `name`：神经元的名称。可选参数。
 
 #### LIF
 
-LIF神经元实现了“泄露-积分-发射”神经元模型，其调用方式及参数如下：
+LIF 神经元实现了“泄露-积分-发射”神经元模型，其调用方式及参数如下：
 
 ```python
-n1 = pb.LIF(shape=128, threshold=127, reset_v=0, leak_v=-1, keep_shape=False, name='n1')
+n1 = pb.LIF(shape=128, threshold=127, reset_v=0, leak_v=-1, neg_threshold=0, keep_shape=False, name='n1')
+n2 = pb.LIF(shape=128, threshold=10, reset_v=1, bias=-1, keep_shape=True, name='n2')
 ```
 
-- `leak_v`：LIF神经元的泄露值（有符号）。其他参数含义与IF神经元相同。
+- `leak_v`：LIF 神经元的泄露值，有符号数。
+- `bias`：偏置，有符号数。当指定偏置时，神经元将使用该值作为其泄露值，并**在阈值比较前泄露**，从而实现“偏置”的效果。此时，`leak_v` 将被忽略。在未指定偏置时，神经元先阈值比较后泄露。
+- 其他参数含义与 IF 相同。
 
 #### Tonic Spiking
 
-Tonic Spiking神经元可以实现对持续脉冲刺激的周期性反应。
+Tonic Spiking 神经元可以实现对持续脉冲刺激的周期性反应。
 
 ```python
 n1 = pb.TonicSpiking(shape=128, fire_step=3, keep_shape=False, name='n1')
 ```
 
-- `fire_step`：发放周期，每接收到 `N` 次刺激后发放脉冲。
+- `fire_step`：发放时间，每接收到 `N` 次刺激后发放脉冲。
 
 #### Phasic Spiking
 
-Phasic Spiking神经元可以实现，在接受一定数量脉冲后发放，然后保持静息状态，不再发放。
+Phasic Spiking 神经元可以实现，在接受一定数量脉冲后发放，然后保持静息状态，不再发放。
 
 ```python
-n1 = pb.PhasicSpiking(shape=128, time_to_fire=3, neg_floor=10, keep_shape=False, name='n1')
+n1 = pb.PhasicSpiking(shape=128, fire_step=3, neg_floor=-10, keep_shape=False, name='n1')
 ```
 
-- `time_to_fire`：发放时间。
-- `neg_floor`：地板阈值，静息时的膜电位为其负值。
-
-#### Always1Neuron
-
-Always1神经元在工作期间持续输出1。
+- `fire_step`：发放时间，每接收到 `N` 次刺激后发放脉冲。
+- `neg_floor`：地板阈值，有符号负数。当发放脉冲后，膜电位将永远保持在地板阈值。
 
 #### Spiking Relu
 
-SNN模式下，具有Relu功能的神经元。当输入为1，则输出为1；输入为0，则输出为0。
+SNN 模式下，具有 Relu 功能的神经元。当输入为1，则输出为1；输入为非正整数，输出为0。
 
 ### 突触
 
-#### 全连接
+#### 全连接 FullConn
 
-PAIBox中，突触用于连接不同神经元组，并包含了连接关系以及权重信息。以全连接类型的突触为实例：
+PAIBox 中，突触用于连接不同神经元组，并包含了连接关系以及权重信息。以全连接类型的突触为实例：
 
 ```python
 s1= pb.FullConn(source=n1, dest=n2, weights=weight1, conn_type=pb.SynConnType.All2All, name='s1')
 ```
 
 其中：
 
@@ -144,17 +131,14 @@
 - `name`：可选，为该对象命名。
 
 突触表达的是两个神经元组之间的连接关系。PAIBox提供了三种主要的连接关系表达：
 
 - `All2All`：全连接
 - `One2One`：单对单连接
 - `Identity`：恒等映射，同单对单连接，权重为缩放因子标量
-- `MatConn`：普通的矩阵连接
-
-通常情况下，`MatConn` 适合所有的连接关系，而 `All2All`、`One2One` 则提供了对于特殊连接更为方便的表达。
 
 ##### All2All 全连接
 
 对于全连接，其权重 `weights` 有两种输入类型：
 
 - 标量：默认为1。例如，设置为 `X`，则权重矩阵实际为元素均为 `X` 的 `N1*N2` 矩阵。
 - 矩阵：尺寸为 `N1*N2` 的矩阵。
@@ -174,15 +158,14 @@
 
   print(s1.weights)
   >>>
   2
   ```
 
   其权重以标量的形式储存。
-
 - 数组：尺寸要求为 `(N2,)`，可以自定义每组对应神经元之间的连接权重。如下例所示，设置 `weights` 为 `[1, 2, 3, 4, 5]`，
 
   ```python
   n1 = pb.IF(shape=5, threshold=1)
   n2 = pb.IF(shape=5, threshold=1)
   s1 = pb.FullConn(source=n1, dest=n2, conn_type=pb.SynConnType.One2One, weights=np.arange(1, 6, dtype=np.int8), name='s1')
 
@@ -197,17 +180,38 @@
 
   其权重实际上为 `N*N` 矩阵，其中 `N` 为前向/后向神经元组数目。
 
 ##### Identity 恒等映射
 
 具有缩放因子的单对单连接，即 `One2One` 中权重项为标量的特殊情况。
 
-##### MatConn 一般连接
+#### 2D矩阵乘法 MatMul2d
+
+专门用于表示二维矩阵乘法， $y=x\cdot w$ 或 $y=x^T\cdot w$
+
+- 例如，输入尺寸为 `(n, k)` ，权重尺寸为 `(k, m)`，输出尺寸为 `(n, m)`
+- 当输入尺寸为 `(k, n)` 时，会**自动进行转置**
+- 输入维度最大为2维
+- 当输入维度小于2维，将自动补齐，即 `(N, )` 补齐为 `(1, N)`
+
+```python
+n1 = pb.IF(shape=(8, 16), threshold=1)
+n2 = pb.IF(shape=(8, 10), threshold=1)
+s1 = pb.MatMul2d(source=n1, dest=n2, weights=np.ones((16, 10), dtype=np.int8))
+```
+
+⚠️ 不要与 `FullConn` 混淆。`FullConn` 需要传入 `N*M` 矩阵，其中 `N` 为前向神经元组数目，`M` 为后向神经元组数目。而 `MatMul2d` 中传入的矩阵尺寸并非 `N*M` ，它最终将展开为 `N*M` 矩阵。如下式所示，由于输入/输出数据在芯片中只能以一维表示，因此，它在芯片中的实现为：
 
-普通的神经元连接类型，仅可以通过矩阵设置其权重 `weights`。
+$$
+\begin{bmatrix}x_{11}&x_{12}&x_{13}\\x_{21}&x_{22}&x_{23}\end{bmatrix}\cdot\begin{bmatrix}w_{11}&w_{12}\\w_{21}&w_{22}\\w_{31}&w_{32}\end{bmatrix}=\begin{bmatrix}y_{11}&y_{12}\\y_{21}&y_{22}\end{bmatrix}
+$$
+
+$$
+\begin{bmatrix}x_{11}\\x_{12}\\x_{13}\\x_{21}\\x_{22}\\x_{23}\end{bmatrix}\cdot\begin{bmatrix}w_{11}&w_{12}&0&0\\w_{21}&w_{22}&0&0\\w_{31}&w_{32}&0&0\\0&0&w_{11}&w_{12}\\0&0&w_{21}&w_{22}\\0&0&w_{31}&w_{32}\end{bmatrix}=\begin{bmatrix}y_{11}&y_{12}&y_{21}&y_{22}\end{bmatrix}
+$$
 
 #### 1D卷积
 
 全展开形式1D卷积为全连接突触的一种特殊表达。需**严格指定**输入神经元的尺寸与维度、卷积核权重、卷积核维度顺序与步长。对于输出神经元的具体尺寸不做严格要求。
 
 - `kernel`：卷积核权重。
 - `stride`：步长，标量。默认为1。
@@ -219,16 +223,14 @@
 n1 = pb.IF(shape=(8, 28), threshold=1)      # Input feature map: (8, 28)
 n2 = pb.IF(shape=(16, 26), threshold=1)     # Output feature map: (16, 26)
 kernel = np.random.randint(-128, 128, size=(16, 8, 3), dtype=np.int8) # OIL
 
 conv1d = pb.Conv1d(n1, n2, kernel=kernel, stride=1, padding=0, kernel_order="OIL", name="conv1d_1")
 ```
 
-⚠️ `padding` 目前不支持，默认为0。
-
 #### 2D卷积
 
 全展开形式2D卷积为全连接突触的一种特殊表达。需**严格指定**输入神经元的尺寸与维度、卷积核权重、卷积核维度顺序与步长。对于输出神经元的具体尺寸不做严格要求。
 
 - `kernel`：卷积核权重。
 - `stride`：步长，标量或元组格式。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。默认为1。
 - `padding`：填充，可以为标量或元组。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。
@@ -283,15 +285,15 @@
 kernel = np.random.randint(-128, 128, size=(16, 8, 3, 3), dtype=np.int8) # OIHW
 
 convt2d = pb.ConvTranspose2d(n1, n2, kernel=kernel, stride=2, padding=1, output_padding=0, kernel_order="OIHW", name="convt2d_1")
 ```
 
 ### 编码器
 
-PAIBox提供了有状态与无状态编码器。其中，有状态编码器是指编码过程与时间有关，将输入数据编码到一段时间窗口内。而无状态编码器是指编码过程与时间无关，每个时间步，都可以根据输入数据进行编码。
+PAIBox 提供了有状态与无状态编码器。其中，有状态编码器是指编码过程与时间有关，将输入数据编码到一段时间窗口内。而无状态编码器是指编码过程与时间无关，每个时间步，都可以根据输入数据进行编码。
 
 ⚠️ 请注意，我们只提供较为简单的编码器，以便用户在不依赖外部库的条件下实现基本编码操作；如果需要更复杂的编码，请直接使用。
 
 #### 无状态编码器
 
 ##### 泊松编码
 
@@ -308,15 +310,15 @@
     out_spike[t] = pe(x)
 ```
 
 通过调用该编码器，将需编码数据传入，即可得到编码后结果。
 
 ##### 直接编码
 
-直接编码使用2D卷积进行特征提取，经过LIF神经元进行编码 。`Conv2dEncoder` 使用示例如下：
+直接编码使用2D卷积进行特征提取，经过 LIF 神经元进行编码 。`Conv2dEncoder` 使用示例如下：
 
 ```python
 kernel = np.random.uniform(-1, 1, size=(1, 3, 3, 3)).astype(np.float32) # OIHW
 stride = (1, 1)
 padding = (1, 1)
 de = pb.simulator.Conv2dEncoder(
     kernel,
@@ -342,19 +344,19 @@
 - `kernel_order`：指定卷积核维度顺序为 `OIHW` 或 `IOHW` 排列。
 - `tau`：膜电位时间常数。
 - `decay_input`：输入是否也会参与衰减。
 - `v_threshold`：阈值电平。
 - `v_reset`：复位电平。
 - 待编码数据维度顺序仅支持 `CHW`。
 
-其中，所使用的LIF为SpikingJelly内的 `SimpleLIFNode`。具体原理参见：[SpikingJelly/SimpleLIFNode](https://spikingjelly.readthedocs.io/zh-cn/latest/sub_module/spikingjelly.activation_based.neuron.html#spikingjelly.activation_based.neuron.SimpleLIFNode)。如果需要使用更复杂的编码，请直接使用。
+其中，所使用的 LIF 为 SpikingJelly 内的 `SimpleLIFNode`。具体原理参见：[SpikingJelly/SimpleLIFNode](https://spikingjelly.readthedocs.io/zh-cn/latest/sub_module/spikingjelly.activation_based.neuron.html#spikingjelly.activation_based.neuron.SimpleLIFNode)。如果需要使用更复杂的编码，请直接使用。
 
 #### 有状态编码器
 
-有状态编码器类别较多。PAIBox提供了几种有状态编码器：周期编码器 `PeriodicEncoder`、延迟编码器 `LatencyEncoder` 。
+有状态编码器类别较多。PAIBox 提供了几种有状态编码器：周期编码器 `PeriodicEncoder`、延迟编码器 `LatencyEncoder` 。
 
 ##### 周期编码器
 
 它以一段脉冲序列为输入，将其循环地在每一个时间步输出。以下为一个简单实例：
 
 ```python
 # 定义一段脉冲序列
@@ -389,15 +391,15 @@
     out_spike[t] = le(x)
 ```
 
 具体编码原理参见：[SpikingJelly/延迟编码器](https://spikingjelly.readthedocs.io/zh-cn/latest/activation_based/2_encoding.html#id5)
 
 ### 输入节点
 
-为了支持多样的数据输入形式，同时标明网络模型的输入节点，PAIBox设计了输入节点这一组件。
+为了支持多样的数据输入形式，同时标明网络模型的输入节点，PAIBox 设计了输入节点这一组件。
 
 输入节点可以使用以下方法定义：
 
 ```python
 inp = pb.InputProj(input=1, shape_out=(4, 4), keep_shape=True, name='inp1')
 ```
 
@@ -519,15 +521,15 @@
     [3 3 3 3]]
 ```
 
 当仿真时间不同时，输出结果也不同，表明输入节点的输出与时间步相关。
 
 #### 编码器类型输入
 
-PAIBox提供了一些常用编码器，编码器内部实现了 `__call__` 方法，因此可作为输入节点的输入使用。在作为输入节点的输入使用时，它与一般函数做为输入节点的输入使用存在差别。
+PAIBox 提供了一些常用编码器，编码器内部实现了 `__call__` 方法，因此可作为输入节点的输入使用。在作为输入节点的输入使用时，它与一般函数做为输入节点的输入使用存在差别。
 
 在例化 `InputProj` 时，输入节点的输入为编码器。在运行时，还需要通过设置 `inp.input`，**向输入节点输入待编码数据**，节点内部将完成编码并输出。以泊松编码器为例：
 
 ```python
 pe = pb.simulator.PoissonEncoder()                          # 例化泊松编码器
 inp = pb.InputProj(pe, shape_out=(4, 4), keep_shape=True)   # 例化输入节点
 input_data = np.random.rand(4, 4).astype(np.float32)        # 生成归一化数据
@@ -557,15 +559,15 @@
 - 该模块完成运算后的输出效果，则表现为一个具有独立输出能力的“神经元”，其输出接口的设计完全符合神经元的标准形式。这意味着其输出脉冲可作为后继突触的输入。
 - 后端构建时，模块将拆分成一或多个神经元节点与突触。所构建的基础组件尺寸由模块连接的操作数尺寸决定。
 
 功能模块均支持 `delay`，`tick_wait_start`，`tick_wait_end`，`keep_shape` 参数。
 
 ### 逻辑运算
 
-逻辑运算模块实现了 `numpy` 中的位逻辑运算操作（例如 `&` 与 `numpy.bitwise_and` 等），可对接收到的一或多个输出脉冲进行逻辑运算，并产生脉冲输出。PAIBox提供了逻辑与、或、非、异或：`BitwiseAND`，`BitwiseOR`，`BitwiseNOT`，`BitwiseXOR`。以位与为例：
+逻辑运算模块实现了 `numpy` 中的位逻辑运算操作（例如 `&` 与 `numpy.bitwise_and` 等），可对接收到的一或多个输出脉冲进行逻辑运算，并产生脉冲输出。PAIBox 提供了逻辑与、或、非、异或：`BitwiseAND`，`BitwiseOR`，`BitwiseNOT`，`BitwiseXOR`。以位与为例：
 
 ```python
 import paibox as pb
 
 class Net(pb.DynSysGroup):
     def __init__(self):
         super().__init__()
@@ -599,34 +601,43 @@
 ```
 
 其中：
 
 - `neuron`：进行延迟输出的神经元。
 - `chain_level`：延迟链的级数，即延迟的时间步。注意，这与 `delay` 含义不同：延迟链内部会建立多级神经元（类似buffer），以实现数据的延迟传递，而 `delay` 会使得神经元输出寄存的位置延后，后继节点的启动时间需要提前，这将导致其在前级**有效输出**前就进行了计算。
 
-### 平均/最大池化
+### 2D平均/最大池化
 
-目前仅提供2D池化：`SpikingAvgPool2d`、`SpikingMaxPool2d`。以平均池化为例：
+目前仅提供2D池化：`SpikingAvgPool2d`、`SpikingMaxPool2d`。以最大池化为例：
 
 ```python
 ksize = (3, 3)
 stride = None # default is ksize
 n1 = pb.SpikingRelu(shape, tick_wait_start=1)
-pool2d = pb.SpikingAvgPool2d(n1, ksize, None, tick_wait_start=2)
-n2 = pb.SpikingRelu(pool2d.shape_out, delay=1, tick_wait_start=3)
-s3 = pb.FullConn(pool2d, n2, conn_type=pb.SynConnType.One2One)
+p2d = pb.SpikingMaxPool2d(n1, ksize, stride=None, padding=(1,1), tick_wait_start=2)
+n2 = pb.SpikingRelu(p2d.shape_out, delay=1, tick_wait_start=3)
+s3 = pb.FullConn(p2d, n2, conn_type=pb.SynConnType.One2One)
 ```
 
 其中：
 
 - `neuron`：待池化的神经元。
 - `kernel_size`：池化窗口的尺寸，标量或元组格式。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。
 - `stride`：步长，可选参数，标量或元组格式，默认为 `None`，即池化窗口的尺寸。
+- `padding`：填充，可以为标量或元组。当为标量时，对应为 `(x, x)`；当为元组时，则对应为 `(x, y)`。默认为0。
 - 神经元维度顺序仅支持 `CHW`。
 
+对于平均池化 `SpikingAvgPool2d`，它还有如下参数可配置：
+
+- `threshold`：平均池化的比较阈值，芯片需要通过神经元的阈值比较间接地实现除法。当不指定时，阈值为 $\text{round}(\text{kernel\_size}/2)$。池化窗口的输入做累加后与该阈值进行比较，可等价于平均池化的操作，即 $o_j=\sum^{k-1}_{i=0}x_{ij} >= \text{threshold}$，其中 $k$ 为池化窗口尺寸，$x_{ij}$ 为每个池化窗口内的输入特征图元素，$o_j$ 为第 $j$ 个输出特征图元素。
+
+### \*2D平均池化（与膜电位相关）
+
+这是 `SpikingAvgPool2d` 的另一种实现形式。`SpikingAvgPool2d` 在每个时间步上的运算**不会造成膜电位积累**（当未发放时），因此，可以说它与时间步无关。而该平均池化实现，当未发放时，**会造成膜电位积累**，因此与时间步相关。调用 `SpikingAvgPool2dWithV`，参数与前述 `SpikingAvgPool2d` 相同。
+
 ### 脉冲加、减
 
 脉冲加减法与数的加减法存在差异。对脉冲进行加减，运算结果将在较长时间步上体现。例如，在 `T=1` 时刻两神经元均输出1，则将在 `T=2,3` 时刻产生输出脉冲。以下为脉冲加减法运算示例。其中，输入为 `T=12` 脉冲序列，输出为 `T=20` 脉冲序列。
 
 ```python
 inpa = np.array([1, 0, 0, 1, 0, 0, 0, 0, 1, 1, 1, 1], np.bool_)
 inpb = np.array([0, 0, 1, 1, 0, 0, 0, 1, 0, 0, 1, 0], np.bool_)
@@ -648,17 +659,19 @@
 
 其中：
 
 - `neuron_a`：第一个操作数。
 - `neuron_b`：第二个操作数。在减法中作被减数。
 - `overflow_strict`：是否严格检查运算结果溢出。如果启用，则在仿真中，当脉冲加、减运算结果溢出时将报错。默认为 `False`。
 
-### 转置
+### 2D/3D转置
 
-PAIBox提供了转置模块 `Transpose2d`，`Transpose3d`，用于实现二维、三维矩阵的转置。对于转置，需要**指定**输入神经元的尺寸、转置顺序（仅三维转置需要）。使用方法与逻辑运算模块相同：
+⚠️ 即将弃用
+
+PAIBox 提供了转置模块 `Transpose2d`，`Transpose3d`，用于实现二维、三维矩阵的转置。对于转置，需要**指定**输入神经元的尺寸、转置顺序（仅三维转置需要）。使用方法与逻辑运算模块相同：
 
 ```python
 n1 = pb.IF((32, 16), 1, 0, delay=1, tick_wait_start=1)
 t2d = pb.Transpose2d(n1, tick_wait_start=2)
 
 n2 = pb.IF((32, 16, 24), 1, 0, delay=1, tick_wait_start=1)
 t3d = pb.Transpose3d(n2, axes=(1, 2, 0), tick_wait_start=2)
@@ -667,15 +680,15 @@
 其中：
 
 - `neuron`：待转置其输出脉冲的神经元。对于二维转置，支持输入尺寸为1或2维；对于三维转置，支持输入尺寸为2或3维。尺寸不足时，自动补1。
 - `axes`：（仅三维转置）如果指定，则必须是包含 `[0,1,…,N-1]` 排列的元组或列表，其中 `N` 是矩阵的轴（维度）数。返回数组的第 `i` 轴将对应于输入的编号为 `axes[i]` 的轴。若未指定，则默认为 `range(N)[::-1]`，这将反转轴的顺序。具体参数含义参见：[numpy.transpose](https://numpy.org/doc/1.26/reference/generated/numpy.transpose.html#numpy.transpose)
 
 ## 网络模型
 
-在PAIBox中，可以通过继承 `DynSysGroup`（或 `Network`）来实现，并在其中例化基础组件与功能模块，完成网络模型的构建。以一个简单的两层全连接网络为例：
+在 PAIBox 中，可以通过继承 `DynSysGroup`（或 `Network`）来实现，并在其中例化基础组件与功能模块，完成网络模型的构建。以一个简单的两层全连接网络为例：
 
 <p align="center">
     <img src="images/Guide-基础网络搭建-全连接网络示例.png" alt="基础网络搭建-全连接网络示例" style="zoom:50%">
 </p>
 
 ### 网络构建
 
@@ -694,15 +707,15 @@
         self.n2 = pb.IF(10, threshold=128, reset_v=0, tick_wait_start=2)
         self.fc1 = pb.FullConn(self.i1, self.n1, weights=weight1, conn_type=pb.SynConnType.All2All)
         self.fc2 = pb.FullConn(self.n1, self.n2, weights=weight2, conn_type=pb.SynConnType.All2All)
 ```
 
 ### 容器类型
 
-PAIBox提供 `NodeList`、`NodeDict` 容器类型，可批量化操作网络基本组件。例如，
+PAIBox 提供 `NodeList`、`NodeDict` 容器类型，可批量化操作网络基本组件。例如，
 
 ```python
 import paibox as pb
 l1 = pb.NodeList()
 
 for i in range(5):
     l1.append(pb.IF(10, threshold=5, reset_v=0))
@@ -810,15 +823,15 @@
 - 神经元：脉冲输出 `spike` 、基于硬件寄存器的**输出** `output`（大小为 `256*N` ）、特征图形式的脉冲输出 `feature_map `、膜电位 `voltage`。
 - 突触：输出 `output`。
 
 ### 仿真机理
 
 在设置完探针后，可为每个输入节点单独输入数据，并进行仿真。仿真结束后可通过 `sim.data[...]` 读取探针监测的数据。
 
-PAIBox仿真器的仿真行为与实际硬件保持一致，在全局时间步 `T>0` 时，网络模型才开始工作。即在例化仿真器时若指定 `start_time_zero=False`，得到的仿真数据 `sim.data[probe1][0]` 为 `T=1` 时刻的模型输出。若指定 `start_time_zero=True`，则仿真数据 `sim.data[probe1][0]` 为 `T=0` 时刻的模型输出（初态）。
+PAIBox 仿真器的仿真行为与实际硬件保持一致，在全局时间步 `T>0` 时，网络模型才开始工作。即在例化仿真器时若指定 `start_time_zero=False`，得到的仿真数据 `sim.data[probe1][0]` 为 `T=1` 时刻的模型输出。若指定 `start_time_zero=True`，则仿真数据 `sim.data[probe1][0]` 为 `T=0` 时刻的模型输出（初态）。
 
 ```python
 # 准备输入数据
 input_data = np.random.rand(28, 28).astype(np.float32)
 input_data2 = np.random.rand(28, 28).astype(np.float32)
 
 fcnet.inp.input = input_data
@@ -837,58 +850,59 @@
 调用 `run` 运行仿真，其中：
 
 - `duration`：指定仿真时间步长。请注意，仿真时需要计算网络的最长路径(delay)，并计入仿真步长中以获取有效的输出。
 - `reset`：是否对网络模型中组件进行复位。默认为 `False`。这可实现在一次仿真的不同时间步，输入不同的数据。
 
 ## 编译、映射与导出
 
-模型映射将完成网络拓扑解析、映射、分配路由坐标、生成配置文件或帧数据，并最终导出为 `.bin` 或 `.npy` 格式交换文件等一系列工作。
+模型映射将完成网络拓扑解析、分割、路由坐标分配、配置信息与帧文件导出等一系列工作。
 
-例化 `Mapper`，传入所构建的网络模型，进行编译，最后导出帧即可。
+例化 `Mapper`，传入所构建的网络模型，编译，最后导出。
 
 ```python
 mapper = pb.Mapper()
 mapper.build(fcnet)
 graph_info = mapper.compile(weight_bit_optimization=True, grouping_optim_target="both")
-mapper.export(write_to_file=True, fp="./debug/", format="bin", split_by_coord=False, export_core_params=False)
+mapper.export(write_to_file=True, fp="./debug/", format="bin", split_by_coord=False, export_core_params=False, use_hw_sim=True)
 
 graph_info.n_core_required
 >>> 999
 
 # Clear all the results
 mapper.clear()
 ```
 
 其中，编译时有如下参数可指定：
 
-- `weight_bit_optimization`: 是否对权重精度进行优化处理。这将使得声明时为 INT8 的权重根据实际值当作更小的精度处理（当权重的值均在 [-8, 7] 之间，则可当作 INT4 进行处理）。默认由后端配置项内对应**编译选项**指定（默认开启）。
-- `grouping_optim_target`：指定神经元分组的优化目标，可以为 `"latency"`，`"core"` 或 `"both"`，分别代表以延时/吞吐率、占用核资源为优化目标、或二者兼顾。默认由后端配置项内对应**编译选项**指定（默认为 `both`）。
+- `weight_bit_optimization`: 是否对权重精度进行优化处理。这将使得声明时为 INT8 的权重根据实际值当作更小的精度处理（当权重的值均在 [-8, 7] 之间，则可当作 INT4 进行处理）。默认开启。
+- `grouping_optim_target`：指定神经元分组的优化目标，可以为 `"latency"`，`"core"` 或 `"both"`，分别代表以延时/吞吐率、占用核资源为优化目标、或二者兼顾。默认 `both`。
 - 同时，该方法将返回字典形式的编译后网络的信息。
 
 导出时有如下参数可指定：
 
 - `write_to_file`: 是否将配置帧导出为文件。默认为 `True`。
 - `fp`：导出目录。若未指定，则默认为后端配置选项 `build_directory` 所设置的目录（当前工作目录）。
 - `format`：导出交换文件格式，可以为 `bin`、`npy` 或 `txt`。默认为 `bin`。
 - `split_by_coord`：是否将配置帧以每个核坐标进行分割，由此生成的配置帧文件命名形如"config_core1"、"config_core2"。默认为 `False`，即最终导出为一个文件。
-- `export_core_params`: 是否导出实际使用核参数至json文件，以直观显示实际使用核的配置信息。默认为 `False`。
+- `export_core_params`：是否导出实际使用核参数至 json 文件，以直观显示实际使用核的配置信息。默认为 `False`。
+- `use_hw_sim`：是否使用硬件仿真器。若使用，将额外导出 `bin` 格式的配置帧文件。
 
 同时，该方法将返回模型的配置项字典 `GraphInfo`，包括：
 
 - `input`：输入节点信息字典。
 - `output`：输出目的地信息字典。
 - `memebers`：中间层所在物理核的配置项字典。
 - `inherent_timestep`：网络的最长时间步。
 - `n_core_required`：网络**需要**的物理核数目。
 - `n_core_occupied`：网络**实际占用**的物理核数目。
 - `extras`：其他额外的网络信息字典，例如，编译后的网络名称。
 
 ### 后端配置项
 
-与后端相关的配置项由 `BACKEND_CONFIG` 统一保存与访问，例如上述**编译选项**、`build_directory`、`target_chip_addr` 等。如下所示，对常用的配置项进行读取与修改：
+与后端相关的配置项由 `BACKEND_CONFIG` 统一保存与访问，例如 `build_directory`、`target_chip_addr` 等。如下所示，对常用的配置项进行读取与修改：
 
 1. 本地芯片地址 `target_chip_addr`，支持**多芯片配置**。
 
    ```python
    # Read
    BACKEND_CONFIG.target_chip_addr
    >>> [Coord(0, 0)]
@@ -909,31 +923,19 @@
    >>> Coord(1, 0)
 
    # Modify
    BACKEND_CONFIG.output_chip_addr = (2, 0)
    # or
    BACKEND_CONFIG.test_chip_addr = (2, 0)
    ```
-
    ⚠️ 请确保输出芯片地址不与本地芯片地址重叠。
 
 3. 编译后配置信息等文件输出目录路径 `output_dir`，默认为用户当前工作目录
 
    ```python
    # Read
    BACKEND_CONFIG.output_dir
    >>> Path.cwd() # Default is your current working directory
 
    # Modify
-   BACKEND_CONFIG.output_dir = "path/to/myoutput"
-   ```
-
-4. 编译选项
-
-   ```python
-   # Set cflag for enabling weight precision optimization
-   set_cflag(enable_wp_opt=True, cflag="This is a cflag.")
-
-   # Read
-   BACKEND_CONFIG.cflag
-   >>> {"enable_wp_opt": True, "cflag": "This is a cflag."}
+   BACKEND_CONFIG.output_dir = "path/to/my/output"
    ```
```

### Comparing `paibox-1.1.0a2/paibox/__init__.py` & `paibox-1.1.0a3/paibox/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,31 +5,32 @@
 from .components.functional import BitwiseAND as BitwiseAND
 from .components.functional import BitwiseNOT as BitwiseNOT
 from .components.functional import BitwiseOR as BitwiseOR
 from .components.functional import BitwiseXOR as BitwiseXOR
 from .components.functional import DelayChain as DelayChain
 from .components.functional import SpikingAdd as SpikingAdd
 from .components.functional import SpikingAvgPool2d as SpikingAvgPool2d
+from .components.functional import SpikingAvgPool2dWithV as SpikingAvgPool2dWithV
 from .components.functional import SpikingMaxPool2d as SpikingMaxPool2d
 from .components.functional import SpikingSub as SpikingSub
 from .components.functional import Transpose2d as Transpose2d
 from .components.functional import Transpose3d as Transpose3d
 from .components.neuron.neurons import IF as IF
 from .components.neuron.neurons import LIF as LIF
-from .components.neuron.neurons import Always1Neuron as Always1Neuron
 from .components.neuron.neurons import PhasicSpiking as PhasicSpiking
 from .components.neuron.neurons import SpikingRelu as SpikingRelu
 from .components.neuron.neurons import TonicSpiking as TonicSpiking
 from .components.projection import InputProj as InputProj
-from .components.synapses import GeneralConnType as SynConnType
+from .components.synapses import ConnType as SynConnType
 from .components.synapses.synapses import Conv1d as Conv1d
 from .components.synapses.synapses import Conv2d as Conv2d
 from .components.synapses.synapses import ConvTranspose1d as ConvTranspose1d
 from .components.synapses.synapses import ConvTranspose2d as ConvTranspose2d
 from .components.synapses.synapses import FullConn as FullConn
+from .components.synapses.synapses import MatMul2d as MatMul2d
 from .components.synapses.synapses import NoDecay as NoDecay
 from .context import FRONTEND_ENV as FRONTEND_ENV
 from .network import DynSysGroup as DynSysGroup
 from .network import Network as Network
 from .node import NodeDict as NodeDict
 from .node import NodeList as NodeList
 from .simulator import Probe as Probe
@@ -39,15 +40,15 @@
     __version__ = version("paibox")
 except Exception:
     __version__ = None
 
 from paibox import tools
 
 # Minimum required version of paicorelib
-__plib_minimum_version__ = "1.0.0"
+__plib_minimum_version__ = "1.1.4"
 
 try:
     import paicorelib as plib
 
     if hasattr(plib, "get_version"):  # For plib <= 0.0.12
         raise ImportError(
             tools.PLIB_UPDATE_INTRO.format(
```

### Comparing `paibox-1.1.0a2/paibox/backend/conf_template.py` & `paibox-1.1.0a3/paibox/backend/conf_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
 from pathlib import Path
-from typing import Any, ClassVar, Dict, List, NamedTuple, TypedDict
+from typing import Any, ClassVar, NamedTuple, TypedDict
 
 import numpy as np
 from numpy.typing import NDArray
 from paicorelib import (
     LCN_EX,
     AxonCoord,
     ChipCoord,
@@ -93,20 +93,20 @@
     max_pooling_en: MaxPoolingEnable
     tick_wait_start: int
     tick_wait_end: int
     snn_mode_en: SNNModeEnable
     target_lcn: LCN_EX
     test_chip_addr: Coord
 
-    def export(self) -> Dict[str, Any]:
+    def export(self) -> dict[str, Any]:
         return ParamsReg.model_validate(self._asdict(), strict=True).model_dump(
             by_alias=True
         )
 
-    def __json__(self) -> Dict[str, Any]:
+    def __json__(self) -> dict[str, Any]:
         """Dump the configs into json for debugging."""
         dict_ = self.export()
 
         for var in self._extra_params:
             dict_[var] = getattr(self, var)
 
         return dict_
@@ -114,30 +114,30 @@
 
 class NeuronDest(NamedTuple):
     """Information of neuron destination (axon address information)."""
 
     _extra_params = ("tick_relative", "addr_axon")
     """Extra parameters for debugging."""
 
-    tick_relative: List[int]
-    addr_axon: List[int]
+    tick_relative: list[int]
+    addr_axon: list[int]
     addr_core_x: int
     addr_core_y: int
     addr_core_x_ex: int
     addr_core_y_ex: int
     addr_chip_x: int
     addr_chip_y: int
 
-    def export(self) -> Dict[str, Any]:
+    def export(self) -> dict[str, Any]:
         dest_info = NeuronDestInfo.model_validate(self._asdict(), strict=True)
         dict_ = dest_info.model_dump(by_alias=True)
 
         return dict_
 
-    def __json__(self) -> Dict[str, Any]:
+    def __json__(self) -> dict[str, Any]:
         """Dump the configs into json for debugging."""
         dict_ = self.export()
 
         for var in self._extra_params:
             dict_[var] = getattr(self, var)
 
         return dict_
@@ -166,30 +166,30 @@
         "n_neuron",
         "addr_ram",
         "addr_offset",
     )
     """Extra parameters for debugging."""
 
     n_neuron: int
-    addr_ram: List[int]
+    addr_ram: list[int]
     """RAM Address of neurons"""
     addr_offset: int
     "RAM starting address(offset)"
     neuron_attrs: NeuronAttrs
     neuron_dest_info: NeuronDestInfo
 
     @classmethod
     def encapsulate(
         cls,
         neuron: NeuDyn,
         n_neuron: int,
-        addr_ram: List[int],
+        addr_ram: list[int],
         addr_offset: int,
-        axon_coords: List[AxonCoord],
-        dest_core_coords: List[Coord],
+        axon_coords: list[AxonCoord],
+        dest_core_coords: list[Coord],
         dest_chip_coord: Coord,
     ):
         """Build the `NeuronConfig`.
 
         Args:
             - neuron: the target `NeuDyn`.
             - addr_ram: assigned RAM address of the target neuron.
@@ -220,24 +220,24 @@
             n_neuron,
             addr_ram,
             addr_offset,
             attrs,
             neuron_dest_info,
         )
 
-    def export(self) -> Dict[str, Any]:
+    def export(self) -> dict[str, Any]:
         dict_ = self.neuron_attrs.model_dump(
             by_alias=True,
             # exclude={"dest_info": self.params_ram.dest_info._exclude_vars},
         )
         dict_.update(self.neuron_dest_info.model_dump(by_alias=True))
 
         return dict_
 
-    def __json__(self) -> Dict[str, Any]:
+    def __json__(self) -> dict[str, Any]:
         """Dump the configs into json for debugging."""
         dict_ = self.export()
 
         for var in self._extra_params:
             dict_[var] = getattr(self, var)
 
         return dict_
@@ -246,45 +246,45 @@
 class CorePlmConfig(NamedTuple):
     _extra_params = ()
     """Extra parameters for debugging."""
 
     random_seed: int
     weight_ram: NDArray[np.uint64]
     params_reg: ParamsReg
-    neuron_configs: Dict[NeuDyn, NeuronConfig]
+    neuron_configs: dict[NeuDyn, NeuronConfig]
 
     @classmethod
     def encapsulate(
         cls,
         random_seed: int,
         weight_ram: NDArray[np.uint64],
         core_config: CoreConfig,
-        neuron_configs: Dict[NeuDyn, NeuronConfig],
+        neuron_configs: dict[NeuDyn, NeuronConfig],
     ):
         return cls(
             random_seed,
             weight_ram,
             ParamsReg.model_validate(core_config._asdict(), strict=True),
             neuron_configs,
         )
 
-    def export(self) -> Dict[str, Any]:
+    def export(self) -> dict[str, Any]:
         dict_ = {
             "name": self.params_reg.name,
             "random_seed": self.random_seed,
             "neuron_rams": dict(),
             **self.params_reg.model_dump(by_alias=True),
         }
 
         for neu, neu_config in self.neuron_configs.items():
             dict_["neuron_rams"][neu.name] = neu_config.export()
 
         return dict_
 
-    def __json__(self) -> Dict[str, Any]:
+    def __json__(self) -> dict[str, Any]:
         """Dump the configs into json for debugging."""
         dict_ = self.export()
 
         for var in self._extra_params:
             dict_[var] = getattr(self, var)
 
         return dict_
@@ -303,18 +303,18 @@
             cls._default_seed,
             cls._default_zero_wram,
             ParamsReg.model_validate(core_config._asdict(), strict=True),
             cls._default_neuron_conf,
         )
 
 
-InputNodeConf: TypeAlias = Dict[NodeName, NeuronDest]
-OutputDestConf: TypeAlias = Dict[NodeName, Dict[CoordAddr, NeuronDestInfo]]
-CorePlmConfInChip: TypeAlias = Dict[Coord, CorePlmConfig]
-CorePlmConf: TypeAlias = Dict[ChipCoord, CorePlmConfInChip]
+InputNodeConf: TypeAlias = dict[NodeName, NeuronDest]
+OutputDestConf: TypeAlias = dict[NodeName, dict[CoordAddr, NeuronDestInfo]]
+CorePlmConfInChip: TypeAlias = dict[Coord, CorePlmConfig]
+CorePlmConf: TypeAlias = dict[ChipCoord, CorePlmConfInChip]
 
 
 class GraphInfo(TypedDict):
     """Information of compiled graph.
 
     TODO Optimize the data structure
     """
@@ -323,47 +323,47 @@
     output: OutputDestConf
     members: CorePlmConf
     inherent_timestep: int
     n_core_required: int
     """The actual used cores."""
     n_core_occupied: int
     """The occupied cores, including used & wasted."""
-    extras: NotRequired[Dict[str, Any]]
+    extras: NotRequired[dict[str, Any]]
 
 
 def gen_config_frames_by_coreconf(
     config_dict: CorePlmConf,
     write_to_file: bool,
     fp: Path,
     split_by_coord: bool,
-    formats: List[str],
-) -> Dict[Coord, FrameArrayType]:
+    formats: list[str],
+) -> dict[Coord, FrameArrayType]:
     """Generate configuration frames by given the `CorePlmConfig`.
 
     Args:
         - config_dict: the dictionary of configurations.
         - write_to_file: whether to write frames to file.
         - fp: If `write_to_file` is `True`, specify the path.
         - split_by_coord: whether to split the generated frames file by the core coordinates.
-        - format: a list of formats to export.
+        - formats: a list of formats to export.
     """
 
     def _write_to_f(name: str, array: FrameArrayType) -> None:
         for format in formats:
             _fp = fp / (name + f".{format}")
             if format == "npy":
                 np2npy(_fp, array)
             elif format == "bin":
                 np2bin(_fp, array)
             else:
                 np2txt(_fp, array)
 
     _default_rid = RId(0, 0)
-    _debug_dict: Dict[Coord, Dict[str, Any]] = dict()
-    frame_arrays_on_core: Dict[Coord, FrameArrayType] = dict()
+    _debug_dict: dict[Coord, dict[str, Any]] = dict()
+    frame_arrays_on_core: dict[Coord, FrameArrayType] = dict()
 
     for chip_coord, conf_in_chip in config_dict.items():
         for core_coord, v in conf_in_chip.items():
             # 1. Only one config frame type I for each physical core.
             config_frame_type1 = OfflineFrameGen.gen_config_frame1(
                 chip_coord, core_coord, _default_rid, v.random_seed
             )
@@ -448,15 +448,15 @@
                 list(frame_arrays_on_core.values()), dtype=FRAME_DTYPE, casting="no"
             )
             _write_to_f(f"config_cores_all", f)
 
     return frame_arrays_on_core
 
 
-def export_core_params_json(core_conf: Dict[Coord, CoreConfig], fp: Path) -> None:
+def export_core_params_json(core_conf: dict[Coord, CoreConfig], fp: Path) -> None:
     _valid_conf = {str(k): v.export() for k, v in core_conf.items()}
 
     if _use_orjson:
         with open(fp / _BACKEND_CONTEXT["core_conf_json"], "wb") as f:
             f.write(
                 orjson.dumps(
                     _valid_conf,
@@ -492,15 +492,15 @@
                 )
             )
     else:
         with open(fp / _BACKEND_CONTEXT["output_conf_json"], "w") as f:
             json.dump(output_conf_info, f, indent=2, cls=PAIConfigJsonEncoder)
 
 
-def export_neuconf_json(neuron_conf: Dict[NeuDyn, NeuronConfig], full_fp: Path) -> None:
+def export_neuconf_json(neuron_conf: dict[NeuDyn, NeuronConfig], full_fp: Path) -> None:
     _valid_conf = {k.name: v.export() for k, v in neuron_conf.items()}
 
     if _use_orjson:
         with open(full_fp, "wb") as f:
             f.write(orjson.dumps(_valid_conf, option=orjson.OPT_INDENT_2))
     else:
         with open(full_fp, "w") as f:
```

### Comparing `paibox-1.1.0a2/paibox/backend/constrs.py` & `paibox-1.1.0a3/paibox/backend/constrs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 import sys
 from collections import defaultdict
-from typing import ClassVar, Dict, FrozenSet, List, Sequence, Tuple
+from collections.abc import Sequence
+from typing import ClassVar
 
 from .graphs_types import NodeName, NodeType
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
-BoundedConstrType: TypeAlias = List[FrozenSet[NodeName]]
+BoundedConstrType: TypeAlias = list[frozenset[NodeName]]
 
 
 class Constraints:
     pass
 
 
 class GraphNodeConstrs(Constraints):
-    BOUNDED_CONSTRS: ClassVar[List[List[NodeName]]] = []
-    CONFLICTED_CONSTRS: ClassVar[Dict[NodeName, Tuple[NodeName, ...]]] = defaultdict(
+    BOUNDED_CONSTRS: ClassVar[list[list[NodeName]]] = []
+    CONFLICTED_CONSTRS: ClassVar[dict[NodeName, tuple[NodeName, ...]]] = defaultdict(
         tuple
     )
 
     @classmethod
     def clear(cls) -> None:
         cls.BOUNDED_CONSTRS = []
         cls.CONFLICTED_CONSTRS = {}
 
     @classmethod
     def add_node_constr(
         cls,
         *,
         bounded: Sequence[NodeName] = (),
-        conflicted: Dict[NodeName, Sequence[NodeName]] = {},
+        conflicted: dict[NodeName, Sequence[NodeName]] = {},
     ):
         """Add constraints to a node."""
         if len(bounded) > 0:
             cls.BOUNDED_CONSTRS.append(list(bounded))
 
         if conflicted:
             for k, v in conflicted.items():
                 cls.CONFLICTED_CONSTRS[k] = tuple(v)
 
     @staticmethod
-    def tick_wait_attr_constr(raw_nodes: List[NodeType]) -> List[List[int]]:
+    def tick_wait_attr_constr(raw_nodes: list[NodeType]) -> list[list[int]]:
         """Check whether the neurons to be assigned to a group are "equal" after\
             automatic inference.
 
         NOTE: Check attributes `tick_wait_start` & `tick_wait_end`. For those   \
             neurons with different attributes, they need to be separated.
 
         Return: returen the group of indices.
```

### Comparing `paibox-1.1.0a2/paibox/backend/context.py` & `paibox-1.1.0a3/paibox/backend/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Any, Dict, List, Union
+from typing import Any, Union
 
 from paicorelib import ChipCoord, Coord, CoordLike, to_coord
 from paicorelib.coordinate import to_coords
 
 from paibox.context import _Context
 from paibox.utils import merge_unique_ordered
 
@@ -30,19 +30,19 @@
     }
 
     def __init__(self) -> None:
         super().__init__()
         self.update(self._default)
 
     @property
-    def target_chip_addr(self) -> List[ChipCoord]:
+    def target_chip_addr(self) -> list[ChipCoord]:
         return self["target_chip_addr"]
 
     @target_chip_addr.setter
-    def target_chip_addr(self, addr: Union[CoordLike, List[CoordLike]]) -> None:
+    def target_chip_addr(self, addr: Union[CoordLike, list[CoordLike]]) -> None:
         if isinstance(addr, list):
             self["target_chip_addr"] = to_coords(addr)
         else:
             self["target_chip_addr"] = [to_coord(addr)]
 
     def add_chip_addr(self, *chip_addrs: CoordLike) -> None:
         # Maintain the order. We may take advantage of the priority
@@ -79,15 +79,15 @@
         return self["build_directory"]
 
     @output_dir.setter
     def output_dir(self, p: Union[str, Path]) -> None:
         self["build_directory"] = Path(p)
 
     @property
-    def cflags(self) -> Dict[str, Any]:
+    def cflags(self) -> dict[str, Any]:
         """Compilation options."""
         return self["cflags"]
 
     def set_default(self) -> None:
         self.clear_all()
         self.update(self._default)
```

### Comparing `paibox-1.1.0a2/paibox/backend/graphs_types.py` & `paibox-1.1.0a3/paibox/backend/graphs_types.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+from dataclasses import dataclass
 from enum import Enum, auto, unique
 from typing import NamedTuple, Union
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
@@ -32,26 +33,36 @@
 
 
 @unique
 class NodePosition(Enum):
     """Charactor of a node in the directed graph."""
 
     MEMBER = auto()
-    """As a member layer."""
     INPUT = auto()
-    """As an input node."""
     OUTPUT = auto()
-    """As an output node."""
 
 
-class NodeDegree(NamedTuple):
+_DEGREE_UNSET = -1  # XXX: or 0?
+
+
+@dataclass
+class NodeDegree:
     """In/Out-degree of a node in the directed graph."""
 
-    in_degree: int = 0
-    out_degree: int = 0
+    in_degree: int = _DEGREE_UNSET
+    out_degree: int = _DEGREE_UNSET
+
+    def __copy__(self) -> "NodeDegree":
+        return self.__deepcopy__()
+
+    def __deepcopy__(self) -> "NodeDegree":
+        return NodeDegree(self.in_degree, self.out_degree)
+
+    def copy(self) -> "NodeDegree":
+        return self.__deepcopy__()
 
 
 class NodeAttr(NamedTuple):
     node: NodeType
     position: NodePosition
     degree: NodeDegree
```

### Comparing `paibox-1.1.0a2/paibox/backend/mapper.py` & `paibox-1.1.0a3/paibox/backend/mapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 from collections import defaultdict
+from collections.abc import Sequence
 from copy import copy
 from pathlib import Path
-from typing import Any, Dict, List, Literal, Optional, Union
+from typing import Any, Literal, Optional, Union
 
 from paicorelib import Coord, CoordOffset, HwConfig, get_replication_id
 
 from paibox.base import NeuDyn, SynSys
 from paibox.exceptions import ConfigInvalidError, ResourceError
 from paibox.network import DynSysGroup
 
@@ -19,41 +20,46 @@
     OutputDestConf,
     export_core_params_json,
     export_input_conf_json,
     export_output_conf_json,
     gen_config_frames_by_coreconf,
 )
 from .context import _BACKEND_CONTEXT, set_cflag
-from .graphs import PAIGraph, convert2routing_groups, get_node_degrees
-from .graphs_types import NodeDegree, SourceNodeType
+from .graphs import (
+    PAIGraph,
+    convert2routing_groups,
+    get_node_degrees,
+    get_succ_cb_by_node,
+)
+from .graphs_types import NodeDegree, NodeType, SourceNodeType
 from .placement import CoreBlock, aligned_coords, max_lcn_of_cb
 from .routing import RoutingGroup, RoutingRoot
 from .segment_utils import NeuSeg
 
 __all__ = ["Mapper"]
 
 
 class Mapper:
     graph = PAIGraph()
     graph_info: GraphInfo
 
     def __init__(self) -> None:
-        self.core_blocks: List[CoreBlock] = []
+        self.core_blocks: list[CoreBlock] = []
         """List for core blocks in the network."""
-        self.succ_core_blocks: Dict[CoreBlock, List[CoreBlock]] = defaultdict(list)
-        self.input_core_blocks: Dict[SourceNodeType, List[CoreBlock]] = defaultdict(
+        self.succ_core_blocks: dict[CoreBlock, list[CoreBlock]] = defaultdict(list)
+        self.input_core_blocks: dict[SourceNodeType, list[CoreBlock]] = defaultdict(
             list
         )
         """List of input core blocks for each input node."""
 
-        self.degrees_of_cb: Dict[CoreBlock, NodeDegree] = defaultdict(NodeDegree)
-        self.routing_groups: List[RoutingGroup] = []
+        self.degrees_of_cb: dict[CoreBlock, NodeDegree] = defaultdict(NodeDegree)
+        self.routing_groups: list[RoutingGroup] = []
 
         self.core_plm_config: CorePlmConf = defaultdict(dict)
-        self.core_params: Dict[Coord, CoreConfig] = dict()
+        self.core_params: dict[Coord, CoreConfig] = dict()
         """The dictionary of core parameters."""
 
         self.n_core_required = 0
         self.n_core_occupied = 0
         self.routing_tree = RoutingRoot(chip_list=_BACKEND_CONTEXT["target_chip_addr"])
 
         self.clear()
@@ -72,14 +78,17 @@
         self.n_core_required = 0
         self.n_core_occupied = 0
 
         # Set default cflags
         _BACKEND_CONTEXT.cflags.clear()
         set_cflag(enable_wp_opt=True)
         set_cflag(grouping_optim_target="both")
+        set_cflag(no_twisted_branch=True)
+        set_cflag(multicast_optim=False)
+        set_cflag(multicast_optim_nodes=())
 
     def build(self, *networks: DynSysGroup, **build_options) -> None:
         """Build the directed graph based on given networks. More than one networks in one graph is supported.
 
         Args:
             - networks: one or many `DynSysGroup`.
 
@@ -89,130 +98,193 @@
 
         # Filter & check the constraints to nodes.
         self.graph.build(*networks, **build_options)
 
     def compile(
         self,
         *,
-        weight_bit_optimization: Optional[bool] = None,
-        grouping_optim_target: Optional[Literal["latency", "core", "both"]] = None,
+        weight_bit_optimization: bool = True,
+        grouping_optim_target: Literal["latency", "core", "both"] = "both",
+        no_twisted_branch: bool = True,
+        multicast_optim: Union[bool, Sequence[NodeType]] = False,
     ) -> GraphInfo:
         """Compile the network with optimization options.
 
         Args:
             - weight_bit_optimization: whether to optimize weight precision. For example, weights declared as   \
                 INT8 are treated as smaller precision based on their actual values (when the weight are all     \
                 between [-8, 7], they can be treated as INT4). By default, it is specified by the corresponding \
-                compile option in the backend configuration item (enabled by default).
+                compile option in the backend configuration item. Default is true.
             - grouping_optim_target: specify the optimization goal of neuron grouping, which can be `latency`,  \
                 `core` or `both`, which respectively represent the optimization goal of delay/throughput,       \
                 occupied cores, or both. The default is specified by the corresponding compilation option in the\
-                backend configuration item (`both` by default).
+                backend configuration item. Default is 'both'.
+            - no_twisted_branch: when parsing the network topology, whether or not to prohibit intersecting     \
+                branch structures will cause such structures to be processed. For example:
 
-        Return: network information after compilation in dictionary format.
-        """
-        if weight_bit_optimization is not None:
-            set_cflag(enable_wp_opt=weight_bit_optimization)
+                I -> A -> B -> C
+                       ------>
 
-        if grouping_optim_target is not None:
-            set_cflag(grouping_optim_target=grouping_optim_target)
+                The out-degree of node A is > 1, and its successor node C has an in-degree > 1. If `no_twisted_branch`    \
+                is true, A will be copied & denoted as A', whose forward connection is preserved.
 
-        """1. Check whether the PAIGraph has built."""
-        self._build_check()
+                I -> A -> B -> C
+                  -> A'------>
+
+                Default is true.
+
+            - multicast_optim (in dev): whether to perform multicast optimization. If true, the optimization is \
+                performed on all nodes in the network. If a node list is passed, the optimization is attempted  \
+                on the specified nodes only. Default is false.
+                TODO A description of it is to be added
 
-        """2. Set global compilation flags."""
+        Return: network information after compilation in dictionary format.
+        """
+        set_cflag(enable_wp_opt=weight_bit_optimization)
+        set_cflag(grouping_optim_target=grouping_optim_target)
+        set_cflag(no_twisted_branch=no_twisted_branch)
+
+        # True, to optimize all nodes. A sequence, to optimize specified nodes
+        if isinstance(multicast_optim, bool):
+            set_cflag(multicast_optim=multicast_optim)
+        elif isinstance(multicast_optim, Sequence):
+            _mul_optim_nodes = tuple(node.name for node in multicast_optim)
+
+            if any(node not in self.graph._raw_nodes for node in _mul_optim_nodes):
+                raise ValueError("not all specified nodes are in the graph.")
+
+            set_cflag(multicast_optim=True)
+            set_cflag(multicast_optim_nodes=_mul_optim_nodes)
+
+        """Preperation.
+            1. Check whether the PAIGraph has built.
+            2. Set global compilation flags.
+        """
+        self._build_check()
         self._set_global_cflags()
 
-        """3. Build core blocks."""
+        """Untwist the branch nodes if flag is on."""
+        if no_twisted_branch:
+            self.untwist_branch_nodes()
+
+        """Build core blocks."""
         self.build_core_blocks()
 
-        """4. Adjust the LCN extension of each core block."""
+        """Adjust the LCN extension of each core block."""
         self.lcn_ex_adjustment()
 
-        """5. Core coordinate assignment."""
+        """Group the axons of core block."""
+        self.cb_axon_grouping()
+
+        # Generate routing_groups for gh_multicast_optim
+        self.routing_groups = convert2routing_groups(
+            self.succ_core_blocks, self.degrees_of_cb, self.input_core_blocks
+        )
+
+        """Core coordinate assignment."""
         self.coord_assign()
 
-        """6. Allocate the core blocks to the `CorePlacement`."""
+        """Allocate the core blocks to the core placments."""
         self.core_allocation()
 
-        """7. Export parameters."""
+        """Export configurations."""
         return self.config_export()
 
+    def untwist_branch_nodes(self) -> None:
+        self.graph.untwist_branch_nodes()
+        self.graph.topo_support_check()
+
     def build_core_blocks(self) -> None:
         """Build core blocks based on grouped edges.
 
         Description: Group all edges & build `CoreBlock` based on the grouped edges.
         """
-        grouped_edges, routing_groups_id = self.graph.group_edges()
+        # TODO Before the compilation, add graph check, such as:
+        # check the node degree: _DEGREE_UNSET, ...
+        grouped_edges, rg_id = self.graph.group_edges()
 
         if sys.version_info >= (3, 10):
-            for syns, routing_id in zip(grouped_edges, routing_groups_id, strict=True):
+            for syns, routing_id in zip(grouped_edges, rg_id, strict=True):
                 self.core_blocks.append(
                     CoreBlock.build(*syns, seed=0, routing_id=routing_id)
                 )
         else:
-            if len(grouped_edges) != len(routing_groups_id):
+            if len(grouped_edges) != len(rg_id):
                 raise ValueError(
                     f"the length of grouped edges & routing groups id are not equal, "
-                    f"{len(grouped_edges)} != {len(routing_groups_id)}"
+                    f"{len(grouped_edges)} != {len(rg_id)}"
                 )
 
-            for syns, routing_id in zip(grouped_edges, routing_groups_id):
+            for syns, routing_id in zip(grouped_edges, rg_id):
                 self.core_blocks.append(CoreBlock.build(*syns, routing_id=routing_id))
 
-        for cb in self.core_blocks:
-            succ_cbs = list(
-                filter(
-                    lambda succ_cb: any(d for d in cb.dest if d in succ_cb.source),
-                    self.core_blocks,
-                )
-            )
-            self.succ_core_blocks[cb].extend(succ_cbs)
+        for cur_cb in self.core_blocks:
+            succ_cbs = []
+            # cur_cb == cb is possible
+            for cb in self.core_blocks:
+                if any(d for d in cur_cb.dest if d in cb.source):
+                    succ_cbs.append(cb)
+
+            self.succ_core_blocks[cur_cb] = succ_cbs
 
         for inode in self.graph.inodes.values():
             # TODO How to prevent this situation: there is input node & predecessor nodes
             # in a certain core blocks.
 
             # Disconnected input nodes will not be recorded.
-            succ_cb = [cb for cb in self.core_blocks if inode in cb.source]
+            succ_cb = get_succ_cb_by_node(inode, self.core_blocks)
             if len(succ_cb) > 0:
                 self.input_core_blocks[inode] = succ_cb
 
         self.degrees_of_cb = get_node_degrees(self.succ_core_blocks)
 
     def lcn_ex_adjustment(self) -> None:
-        """Adjust the LCN extension of each core block."""
+        """Adjust the LCN of each core block & set target LCN."""
         # In the absence of the above complex situations, the following judgment is useless.
         # But it'd be better to add this lcn adjustment.
         for input_cbs in self.input_core_blocks.values():
             if len(input_cbs) > 1:
                 max_lcn_ex = max_lcn_of_cb(input_cbs)
                 # Adjust the `lcn_ex` of the input core blocks for each input node
                 for g in input_cbs:
                     g.lcn_ex = max_lcn_ex
 
         for cb in self.core_blocks:
-            succ_cb = self.succ_core_blocks[cb]
+            succ_cbs = self.succ_core_blocks[cb]
 
-            if len(succ_cb) > 1:
-                max_lcn_ex = max_lcn_of_cb(succ_cb)
+            if len(succ_cbs) > 1:
+                max_lcn_ex = max_lcn_of_cb(succ_cbs)
                 # Adjust the `lcn_ex` of the following core blocks
-                for g in succ_cb:
-                    g.lcn_ex = max_lcn_ex
+                for _cb in succ_cbs:
+                    _cb.lcn_ex = max_lcn_ex
 
                 # Adjust `target_lcn` of itself & lock
                 cb.target_lcn = max_lcn_ex
-                cb.lcn_locked = True
-            elif len(succ_cb) == 1:
+            elif len(succ_cbs) == 1:
                 # Adjust `target_lcn` of itself & lock
-                cb.target_lcn = succ_cb[0].lcn_ex
-                cb.lcn_locked = True
-            else:
-                # Doesn't have following core blocks
-                cb.lcn_locked = True
+                cb.target_lcn = succ_cbs[0].lcn_ex
+
+            cb._lcn_locked = True
+
+    def cb_axon_grouping(self) -> None:
+        """The axons are grouped after the LCN has been modified & locked."""
+        for cb in self.core_blocks:
+            cb.group_axons()
+
+        for i in range(len(self.routing_groups)):
+            routing_group = self.routing_groups[i]
+
+    def graph_optimization(self) -> None:
+        optimized = self.graph.graph_optimization(self.core_blocks, self.routing_groups)
+        if optimized:
+            self.core_blocks.clear()
+            self.succ_core_blocks.clear()
+            self._build_check()
+            self.build_core_blocks()
+            self.lcn_ex_adjustment()
 
     def coord_assign(self) -> None:
         """Assign the coordinate of each `CorePlacement`.
 
         NOTE: The neurons in each core block must be grouped first to determine the \
             #N of cores required, and then the routing coordinates can be assigned.
         """
@@ -230,25 +302,22 @@
             raise ResourceError(
                 CORE_RESOURCE_OUT_OF_RANGE_TEXT.format(n_avail_cores, n_core_required)
             )
 
         self.n_core_required = n_core_required
 
         # Generate routing groups by given the list of core blocks.
-        routing_groups = convert2routing_groups(
-            self.succ_core_blocks, self.degrees_of_cb, self.input_core_blocks
-        )
-        for rg in routing_groups:
+        for rg in self.routing_groups:
             self.routing_tree.insert_routing_group(rg)
 
-        self.routing_groups = routing_groups
-
         # Calculate the consumption of occupied physical cores.
         if (
-            n_core_occupied := sum(rg.get_n_core_occupied() for rg in routing_groups)
+            n_core_occupied := sum(
+                rg.get_n_core_occupied() for rg in self.routing_groups
+            )
         ) > n_avail_cores:
             raise ResourceError(
                 CORE_RESOURCE_OUT_OF_RANGE_TEXT.format(n_avail_cores, n_core_occupied)
             )
 
         self.n_core_occupied = n_core_occupied
 
@@ -311,15 +380,15 @@
             "inp2_1": {...} # as input node #2
         }
         """
         input_nodes_info = dict()
 
         # Traverse input core blocks
         for inode, input_cbs in self.input_core_blocks.items():
-            dest_coords: List[Coord] = []
+            dest_coords: list[Coord] = []
 
             assert all(input_cbs[0].chip_coord == cb.chip_coord for cb in input_cbs)
             for cb in input_cbs:  # Do not use iterative generation.
                 dest_coords.extend(cb.core_coords)
 
             dest_rid = get_replication_id(dest_coords)
 
@@ -437,95 +506,80 @@
                 dest_cb_of_nseg = self._find_dest_cb_by_nseg(neu_seg, member_onode_cb)
 
                 if len(dest_cb_of_nseg) > 0:
                     assert _cb_routable(self.routing_groups, dest_cb_of_nseg)
                     core_plm.export_neu_config(neu_seg, dest_cb_of_nseg)
                 else:
                     offset_idx = o_nodes.index(neu_seg.parent)
-
-                    if hasattr(CoordOffset, "from_offset"):
-                        # For paicorelib > 0.0.13
-                        cur_ocoord = ocoord + CoordOffset.from_offset(offset_idx)
-                    else:
-                        # For paicorelib <= 0.0.13
-                        cur_ocoord = ocoord + CoordOffset(
-                            offset_idx // 32, offset_idx % 32
-                        )
-
+                    cur_ocoord = ocoord + CoordOffset.from_offset(offset_idx)
                     output_axon_offset = core_plm.export_neu_config(
                         neu_seg,
                         output_core_coord=cur_ocoord,
                         axon_addr_offset=output_axon_offset,
                     )
                     output_dest_info[neu_seg.parent.name][core_plm.coord.address] = (
                         core_plm.neu_configs[neu_seg.parent].neuron_dest_info
                     )
 
         # Add the offset as the starting coordinate of the next output node
-        return cur_ocoord + CoordOffset(1, 0)
+        return cur_ocoord + CoordOffset.from_offset(1)
 
     def _onode_cb_config_export(
         self, onode_cb: CoreBlock, output_dest_info: OutputDestConf, ocoord: Coord
     ) -> Coord:
         """Export configuration information for core blocks that are pure output."""
         cur_ocoord = ocoord
         output_axon_offset = 0
         o_nodes = [d for d in onode_cb.dest if d in self.graph.onodes.values()]
 
         for core_plm in onode_cb.core_placements.values():
             for neu_seg in core_plm.neu_segs_of_cplm:
                 # Get the output coordinate of this neu_seg
                 offset_idx = o_nodes.index(neu_seg.parent)
-
-                if hasattr(CoordOffset, "from_offset"):
-                    # For paicorelib > 0.0.13
-                    cur_ocoord = ocoord + CoordOffset.from_offset(offset_idx)
-                else:
-                    # For paicorelib <= 0.0.13
-                    cur_ocoord = ocoord + CoordOffset(offset_idx // 32, offset_idx % 32)
-
+                cur_ocoord = ocoord + CoordOffset.from_offset(offset_idx)
                 output_axon_offset = core_plm.export_neu_config(
                     neu_seg,
                     output_core_coord=cur_ocoord,
                     axon_addr_offset=output_axon_offset,
                 )
                 output_dest_info[neu_seg.parent.name][core_plm.coord.address] = (
                     core_plm.neu_configs[neu_seg.parent].neuron_dest_info
                 )
 
-        return cur_ocoord
+        # Add the offset as the starting coordinate of the next output node
+        return cur_ocoord + CoordOffset.from_offset(1)
 
     def export(
         self,
         write_to_file: bool = True,
         *,
         fp: Optional[Union[str, Path]] = None,
         format: Literal["txt", "bin", "npy"] = "bin",
         split_by_coord: bool = False,
         export_core_params: bool = False,
         use_hw_sim: bool = True,
-    ) -> Dict[Coord, Any]:
+    ) -> dict[Coord, Any]:
         """Generate configuration frames & export to file.
 
         Args:
             - write_to_file: whether to write frames into file.
             - fp: If `write_to_file` is `True`, specify the output path.
             - format: `txt`, `bin`, or `npy`. `bin` is recommended.
             - split_by_coord: whether to split the generated frames file by the core coordinates.
             - export_core_params: whether to export the parameters of occupied cores.
-            - use_hw_sim: whether to use hardware simulator. If use, '.txt' will be exported.
+            - use_hw_sim: whether to use hardware simulator. If use, '.bin' will be exported.
 
         Return: a dictionary of configurations.
         """
         if format not in ("bin", "npy", "txt"):
             raise ValueError(f"format {format} is not supported.")
 
         formats = [format]
         if use_hw_sim:
-            formats.append("txt")
+            formats.append("bin")
 
         formats = list(set(formats))
 
         _fp = _fp_check(fp)
         config_dict = gen_config_frames_by_coreconf(
             self.graph_info["members"],
             write_to_file,
@@ -577,33 +631,33 @@
                     f"Address width:    {axon_segment.addr_width}\n"
                     f"Address offset:   {axon_segment.addr_offset}"
                 )
 
     def _build_check(self) -> None:
         return self.graph.build_check()
 
-    def _find_dest_cb_by_nseg(self, neu_seg: NeuSeg, cb: CoreBlock) -> List[CoreBlock]:
+    def _find_dest_cb_by_nseg(self, neu_seg: NeuSeg, cb: CoreBlock) -> list[CoreBlock]:
         succ_cbs = self.succ_core_blocks[cb]
         dest_cb_of_nseg = [cb for cb in succ_cbs if neu_seg.parent in cb.source]
 
         return dest_cb_of_nseg
 
 
-def group_by(dict_: Dict, keyfunc=lambda item: item):
+def group_by(dict_: dict, keyfunc=lambda item: item):
     """Groups the given list or dictionary by the value returned by ``keyfunc``."""
     d = defaultdict(list)
 
     for item in dict_.values():
         d[keyfunc(item)].append(item)
 
     return d
 
 
 def _cb_routable(
-    routing_group: List[RoutingGroup], core_blocks: List[CoreBlock]
+    routing_group: list[RoutingGroup], core_blocks: list[CoreBlock]
 ) -> bool:
     if len(core_blocks) == 1:
         return True
 
     for rg in routing_group:
         if core_blocks[0] in rg:
             return all(cb in rg for cb in core_blocks)
```

### Comparing `paibox-1.1.0a2/paibox/backend/placement.py` & `paibox-1.1.0a3/paibox/backend/placement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import sys
 import warnings
-from dataclasses import field
 from functools import cached_property
-from typing import ClassVar, Dict, List, Literal, Optional, Tuple, overload
+from typing import ClassVar, Literal, Optional, overload
 
 import numpy as np
 from numpy.typing import NDArray
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
@@ -22,15 +21,16 @@
     CoreModeDict,
     HwConfig,
     HwCore,
     MaxPoolingEnable,
 )
 from paicorelib import WeightPrecision as WP
 
-from paibox.base import NeuDyn, PAIBoxObject, SynSys
+from paibox.base import NeuDyn, PAIBoxObject
+from paibox.components import FullConnectedSyn
 from paibox.exceptions import GraphBuildError, ResourceError, TruncationWarning
 from paibox.types import WeightType
 from paibox.utils import check_attr_same, count_unique_elem
 
 from .conf_template import CoreConfig, CorePlmConfig, EmptyCorePlmConfig, NeuronConfig
 from .context import _BACKEND_CONTEXT
 from .graphs_types import DestNodeType, SourceNodeType
@@ -40,28 +40,33 @@
     NeuSegOfCorePlm,
     aligned_coords,
     get_axon_segments,
     get_neu_segments,
 )
 
 WeightRamType: TypeAlias = NDArray[np.uint64]  # uint64 weights mapped in weight RAM
+_COORD_UNSET = 0
 
 
 class CoreAbstract(HwCore, PAIBoxObject):
-    SUPPORTED_MODE: ClassVar[Tuple[CoreMode, ...]] = (CoreMode.MODE_SNN,)
+    SUPPORTED_MODE: ClassVar[tuple[CoreMode, ...]] = (CoreMode.MODE_SNN,)
     """Supported core modes."""
 
 
 class CoreBlock(CoreAbstract):
     """Core Block for `MODE_SNN` ONLY."""
 
     RUNTIME_MODE: ClassVar[CoreMode] = CoreMode.MODE_SNN
 
     def __init__(
-        self, *parents: SynSys, routing_id: int, seed: int, name: Optional[str] = None
+        self,
+        *parents: FullConnectedSyn,
+        routing_id: int,
+        seed: int,
+        name: Optional[str] = None,
     ) -> None:
         """Core blocks in SNN mode.
 
         Args:
             - parents: the parent synapses.
             - routing_id: id of routing group.
             - seed: random seed. Default value is 0.
@@ -75,61 +80,61 @@
 
         self.seed = seed
         """Random seed, legal integer, no more than uint64."""
 
         self.target_lcn = LCN_EX.LCN_1X
         """The target(destination core block) LCN."""
 
-        self.lcn_locked = False
+        self._lcn_locked = False
         """Used to indicate whether `lcn_ex` has been adjusted."""
 
-        self.core_coords: List[Coord] = list()
+        self.core_coords: list[Coord] = list()
         """Assigned core coordinates."""
 
-        self.chip_coord: ChipCoord = Coord(0, 0)  # default
+        self.chip_coord: ChipCoord = Coord(_COORD_UNSET, _COORD_UNSET)
         """A core block must be placed on a chip."""
 
-        self.core_placements: Dict[Coord, CorePlacement] = dict()
+        self.core_placements: dict[Coord, CorePlacement] = dict()
         """Core placements."""
 
         # Segment the group of axons.
-        self.axon_segments: Dict[SourceNodeType, AxonSegment] = get_axon_segments(
-            self.axons, self.n_timeslot, self.n_fanin_max
-        )
+        self.axon_segments: dict[SourceNodeType, AxonSegment] = dict()
         """A dictionary of segments of each axon(source node)."""
 
         self.neuron_segs_of_cb: NeuSegOfCoreBlock = []
         """Neuron segments in the core block. Each element in the list \
             represents the neuron segments in core placement(physical core).
         """
 
     def group_neurons(
         self, optim_target: Literal["latency", "core", "both"] = "both"
     ) -> None:
         """Group the neurons to determine the #N of cores required."""
-        if not self.lcn_locked:
-            raise GraphBuildError("Group the neurons after lcn_ex is locked.")
+        if not self._lcn_locked:
+            raise GraphBuildError("group the neurons after 'lcn_ex' is locked.")
 
         self.neuron_segs_of_cb = get_neu_segments(
             self.dest,
             self.neuron_capacity,
-            _neuron_repl_prop(self.n_weight_bits, self.n_timeslot),
+            neuron_repl_prop(self.n_weight_bits, self.n_timeslot),
             optim_target,
         )
 
     def core_plm_alloc(self) -> None:
         """Allocate `CoreBlock` to physical cores."""
-        if not self.lcn_locked:
-            raise GraphBuildError("Allocate core placements after lcn_ex is locked.")
+        if not self._lcn_locked:
+            raise GraphBuildError("allocate core placements after 'lcn_ex' is locked.")
 
         for i, coord in enumerate(self.core_coords):
             # assert self.get_raw_weight_of_coord(i)[0].shape[0] == self.n_axon
             self.core_placements[coord] = CorePlacement.build(self, i)
 
-    def _get_syn_of(self, src: SourceNodeType, dest: DestNodeType) -> Optional[SynSys]:
+    def _get_syn_of(
+        self, src: SourceNodeType, dest: DestNodeType
+    ) -> Optional[FullConnectedSyn]:
         for syn in self.obj:
             if syn.source == src and syn.dest == dest:
                 return syn
 
         return None
 
     def _n_axon2lcn_ex(self) -> LCN_EX:
@@ -156,32 +161,32 @@
 
     def copy(self):
         raise NotImplementedError
 
     """Interfaces"""
 
     @property
-    def obj(self) -> Tuple[SynSys, ...]:
+    def obj(self) -> tuple[FullConnectedSyn, ...]:
         return self._parents
 
     @property
-    def shape(self) -> Tuple[int, int]:
+    def shape(self) -> tuple[int, int]:
         return (count_unique_elem(self.source), count_unique_elem(self.dest))
 
     @property
-    def source(self) -> List[SourceNodeType]:
+    def source(self) -> list[SourceNodeType]:
         """Ordered unique source nodes."""
         return list(set([parent.source for parent in self.obj]))
 
     @property
-    def axons(self) -> List[SourceNodeType]:
+    def axons(self) -> list[SourceNodeType]:
         return self.source
 
     @property
-    def dest(self) -> List[DestNodeType]:
+    def dest(self) -> list[DestNodeType]:
         """Ordered unique destination nodes."""
         return list(set([parent.dest for parent in self.obj]))
 
     def n_axon_of(self, index: int) -> int:
         """Get the #N of axons of `index`-th source neuron."""
         return self.axons[index].num_out
 
@@ -235,15 +240,15 @@
         """Set or adjust the `lcn_ex` & lock."""
         if lcn_ex > LCN_EX.LCN_64X:
             raise ResourceError(
                 f"required LCN extension out of range {LCN_EX.LCN_64X} ({lcn_ex})."
             )
 
         self._lcn_ex = lcn_ex
-        self.lcn_locked = True
+        self._lcn_locked = True
 
     @property
     def n_timeslot(self) -> int:
         return 1 << self.lcn_ex
 
     @property
     def tws(self) -> int:
@@ -278,19 +283,19 @@
         )
 
     @property
     def n_neuron(self) -> int:
         return sum(d.num_in for d in self.dest)
 
     @property
-    def unrolling_factor(self) -> List[int]:
+    def unrolling_factor(self) -> list[int]:
         return [d.unrolling_factor for d in self.dest]
 
     @property
-    def n_neuron_of_plm(self) -> List[int]:
+    def n_neuron_of_plm(self) -> list[int]:
         """A list of the #N of neurons on each `CorePlacement`.
 
         FIXME Different in SNN/ANN RUNTIME_MODE.
         """
         if len(self.core_coords) == 0:
             raise GraphBuildError(f"do this after coordinates assignment.")
 
@@ -299,19 +304,27 @@
         assert [] not in self.neuron_segs_of_cb  # TODO if it never happens, remove it.
 
         return [
             sum(seg.n_neuron for seg in neuron_segs)
             for neuron_segs in self.neuron_segs_of_cb
         ]
 
+    def group_axons(self) -> None:
+        if not self._lcn_locked:
+            raise GraphBuildError("get axon segments after 'lcn_ex' is locked.")
+
+        self.axon_segments = get_axon_segments(
+            self.axons, self.n_timeslot, self.n_fanin_max
+        )
+
     @cached_property
-    def raw_weight_of_dest(self) -> List[WeightType]:
+    def raw_weight_of_dest(self) -> list[WeightType]:
         """Merge and then split the weight matrix according to the grouping of neurons."""
         # The concatenated weight for each destination node.
-        w_of_neurons: List[WeightType] = []
+        w_of_neurons: list[WeightType] = []
 
         for d in self.dest:
             # The weights for each destination node.
             w_of_dest = []
 
             for s in self.source:
                 if syn := self._get_syn_of(s, d):
@@ -327,17 +340,17 @@
         assert all(
             w_of_neurons[0].shape[0] == w_of_neuron.shape[0]
             for w_of_neuron in w_of_neurons
         )
 
         return w_of_neurons
 
-    def get_raw_weight_of_coord(self, idx: int) -> List[WeightType]:
+    def get_raw_weight_of_coord(self, idx: int) -> list[WeightType]:
         """Get the raw weight of a coordinate(on each `CorePlacement`)."""
-        w_of_neu_segs: List[WeightType] = []
+        w_of_neu_segs: list[WeightType] = []
 
         for neu_seg in self.neuron_segs_of_cb[idx]:
             w_of_dest = self.raw_weight_of_dest[self.dest.index(neu_seg.parent)]
             w_of_neu_seg = w_of_dest[:, neu_seg.segment.index].copy()
             w_of_neu_seg.setflags(write=False)
             w_of_neu_segs.append(w_of_neu_seg)
 
@@ -353,51 +366,51 @@
         return f"<{self.name} of target '{self.obj}'>"
 
     def _obj_repr(self) -> str:
         """The representation of the names of target objects."""
         return ", ".join(n.name for n in self.obj)
 
     @classmethod
-    def build(cls, *synapses: SynSys, routing_id: int, seed: int = 0):
+    def build(cls, *synapses: FullConnectedSyn, routing_id: int, seed: int = 0):
         """Group synapses & build `CoreBlock`."""
         # FIXME where does the parameter check do?
         if seed > (1 << 64) - 1:
             warnings.warn(
                 f"random seed {seed} is too large, truncated into 64 bits.",
                 TruncationWarning,
             )
 
         return cls(*synapses, routing_id=routing_id, seed=seed)
 
     @classmethod
-    def export_core_plm_config(cls, cb: "CoreBlock") -> Dict[Coord, CoreConfig]:
+    def export_core_plm_config(cls, cb: "CoreBlock") -> dict[Coord, CoreConfig]:
         """Export the parameters of the core into a dictionary."""
         cb_config = dict()
 
         for coord, core_plm in cb.core_placements.items():
             cb_config[coord] = CorePlacement.export_param_config(core_plm)
 
         return cb_config
 
 
 class CorePlacement(CoreAbstract):
     """The divided synapse placed on a single CORE."""
 
-    WEIGHT_RAM_SHAPE: ClassVar[Tuple[int, int]] = (
+    WEIGHT_RAM_SHAPE: ClassVar[tuple[int, int]] = (
         HwConfig.N_FANIN_PER_DENDRITE_SNN,
         HwConfig.N_DENDRITE_MAX_SNN,
     )
     """SNN mode ONLY."""
 
     def __init__(
         self,
         parent: CoreBlock,
         routing_coord: Coord,
         n_neuron: int,
-        raw_weights: List[WeightType],
+        raw_weights: list[WeightType],
         neu_segs_of_cplm: NeuSegOfCorePlm,
         name: Optional[str] = None,
     ) -> None:
         """
         Arguments:
             - parent: the parent core block.
             - idx: The index number where this object is located.
@@ -413,26 +426,26 @@
 
         self.n_neuron = n_neuron
 
         self._weights_folded = self._fold_raw_weights(raw_weights)
         """The folded weights."""
 
         self.neu_segs_of_cplm = neu_segs_of_cplm
-        self.neu_configs: Dict[NeuDyn, NeuronConfig] = dict()
+        self.neu_configs: dict[NeuDyn, NeuronConfig] = dict()
 
     @classmethod
     def build(cls, parent: CoreBlock, idx: int):
         coord = parent.core_coords[idx]
         n_neuron = parent.n_neuron_of_plm[idx]
         neu_segs_of_cplm = parent.neuron_segs_of_cb[idx]
         raw_weights = parent.get_raw_weight_of_coord(idx)
 
         return cls(parent, coord, n_neuron, raw_weights, neu_segs_of_cplm)
 
-    def _fold_raw_weights(self, raw_weights: List[WeightType]) -> WeightType:
+    def _fold_raw_weights(self, raw_weights: list[WeightType]) -> WeightType:
         """Fold the weights into LCN-sized blocks."""
         w_folded_list = []
         w_folded_of_axon_segs = []
         n_fold = self.n_timeslot
 
         if self.lcn_ex == LCN_EX.LCN_1X:
             w_folded = np.hstack(raw_weights, dtype=np.int8)
@@ -566,30 +579,30 @@
             _BACKEND_CONTEXT.test_chip_addr,    # test_chip_addr
         )
         # fmt: on
         return cb_config
 
     @overload
     def export_neu_config(
-        self, neu_seg: NeuSeg, axon_dests: List[CoreBlock]
+        self, neu_seg: NeuSeg, axon_dests: list[CoreBlock]
     ) -> None: ...
 
     @overload
     def export_neu_config(
         self,
         neu_seg: NeuSeg,
         *,
         output_core_coord: Coord,
         axon_addr_offset: int,
     ) -> int: ...
 
     def export_neu_config(
         self,
         neu_seg: NeuSeg,
-        axon_dests: Optional[List[CoreBlock]] = None,
+        axon_dests: Optional[list[CoreBlock]] = None,
         output_core_coord: Optional[Coord] = None,
         axon_addr_offset: Optional[int] = None,
     ) -> Optional[int]:
         """Export the neuron configuration."""
         if isinstance(axon_dests, list):
             axon_coords = aligned_coords(
                 neu_seg.segment.index,
@@ -652,15 +665,15 @@
         )
 
     @property
     def mode(self) -> CoreMode:
         return self.parent.RUNTIME_MODE
 
     @property
-    def shape(self) -> Tuple[int, int]:
+    def shape(self) -> tuple[int, int]:
         return (count_unique_elem(self.source), count_unique_elem(self.dest))
 
     @property
     def weight_precision(self) -> WP:
         return self.parent.weight_precision
 
     @property
@@ -689,18 +702,18 @@
 
     @property
     def twe(self) -> int:
         return self.parent.twe
 
     @property
     def n_dendrite(self) -> int:
-        return self.n_neuron * _neuron_repl_prop(self.n_weight_bits, self.n_timeslot)
+        return self.n_neuron * neuron_repl_prop(self.n_weight_bits, self.n_timeslot)
 
     @property
-    def source(self) -> List[SourceNodeType]:
+    def source(self) -> list[SourceNodeType]:
         return self.parent.source
 
     @property
     def dest(self):
         """The destination nodes within it.
 
         NOTE: This attribute is different from the one of its parent.
@@ -758,31 +771,22 @@
         return EmptyCorePlmConfig.encapsulate(core_param)
 
     @classmethod
     def build(cls, coord: Coord):
         return cls(coord)
 
     @property
-    def n_core_required(self):
+    def n_core_required(self) -> int:
         return 1
 
 
-def max_lcn_of_cb(cb: List[CoreBlock]) -> LCN_EX:
+def max_lcn_of_cb(cb: list[CoreBlock]) -> LCN_EX:
     """Find the max LCN extenion of previous grouped synapses"""
     return max(cb, key=lambda cb: cb.lcn_ex).lcn_ex
 
 
-def _neuron_repl_prop(nbits: int, ntimeslot: int) -> int:
+def neuron_repl_prop(nbits: int, ntimeslot: int) -> int:
     """Get the proportion of neuron replication.
 
     scale = nbits(1 << wp) * n_timeslot(1 << lcn_ex)
     """
     return nbits * ntimeslot
-
-
-class CoreMapper:
-    """Manage to group, combine & place the network into the chip.
-
-    TODO Integrate all the info of building the map.
-    """
-
-    core_blocks: List[CoreBlock] = field(default_factory=list)
```

### Comparing `paibox-1.1.0a2/paibox/backend/routing.py` & `paibox-1.1.0a3/paibox/backend/routing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Dict, Iterator, List, Optional, Sequence, final
+from collections.abc import Iterator, Sequence
+from typing import Any, Optional, Union, final
 
 from paicorelib import ChipCoord, Coord, HwConfig
 from paicorelib.routing_defs import ROUTING_DIRECTIONS_IDX as DIREC_IDX
 from paicorelib.routing_defs import RoutingCoord, RoutingCost
 from paicorelib.routing_defs import RoutingDirection as Direction
 from paicorelib.routing_defs import RoutingLevel as Level
 from paicorelib.routing_defs import RoutingStatus as Status
@@ -42,15 +43,15 @@
             - children: the children of the cluster.
             - d: the direction of the cluster, relative to its parent.
             - item: the data hanging on the cluster.
             - tag: a tag for user to identify.
             - status: the status of the cluster. Only for L0-level leaves.
         """
         self.level = level
-        self.children: Dict[Direction, RoutingCluster] = dict()
+        self.children: dict[Direction, RoutingCluster] = dict()
         self.d = direction
         self.item = data
         self.tag = tag
         self.include_online = include_online
 
         # Only set the attribute for L0-level cluster.
         if self.level == Level.L0:
@@ -96,24 +97,24 @@
         return False
 
     def add_child_to(
         self, child: "RoutingCluster", d: Direction, check_hit_online: bool = False
     ) -> bool:
         """Add a child cluster to a certain `direction`."""
         if self.level - child.level != 1:
-            raise ValueError(f"Cannot skip more than 1 level.")
+            raise ValueError(f"cannot skip more than 1 level.")
 
         if d in self:
             return False
 
-        if d == Direction.X1Y1:
+        if d == Direction.X1Y1 or self.level in (Level.L1, Level.L2):
             if self.include_online and check_hit_online:
                 return False
             else:
-                child.include_online = True
+                child.include_online = self.include_online
 
         # child.direction = d. Already done in `self[d]`(__setitem__).
         self[d] = child
 
         return True
 
     def remove_child(
@@ -122,15 +123,15 @@
         revert_direc: Direction = Direction.ANY,
         strict: bool = False,
     ) -> Optional["RoutingCluster"]:
         child = self.children.pop(d, None)
 
         if child is None:
             if strict:
-                raise RoutingError(f"Removed child of {d} from {self} failed.")
+                raise RoutingError(f"removed child of {d} from {self} failed.")
             else:
                 return None
 
         # Revert the properties that were modified in the previous insertion.
         child.include_online = False
         child.d = revert_direc
 
@@ -159,26 +160,26 @@
         sub_cluster = self[path[0]]
 
         if len(path) > 1:
             return sub_cluster.find_cluster_by_path(path[1:])
         else:
             return sub_cluster
 
-    def get_routing_path(self, cluster: "RoutingCluster") -> Optional[List[Direction]]:
+    def get_routing_path(self, cluster: "RoutingCluster") -> Optional[list[Direction]]:
         """Return a direction path from L4 to the level of `cluster`.
 
         Args:
             - cluster: the cluster with level <= `self.level`.
 
         Return:
             - A list of `Direction` from L4 to L0.
         """
         if cluster.level > self.level:
             raise ValueError(
-                f"Cannot get routing path because the level cluster is higher."
+                f"cannot get routing path because the level cluster is higher."
             )
 
         if cluster.level == self.level:
             if cluster != self:
                 return None
 
             return []
@@ -251,15 +252,15 @@
 
         if subtree.level == self.level:
             sub_n_child = len(subtree.children)
             if self.n_child_avail() < sub_n_child:
                 return False
 
             if sub_n_child == 1:
-                self.add_child(subtree[Direction.X0Y0], check_hit_online)
+                return self.add_child(subtree[Direction.X0Y0], check_hit_online)
 
             elif sub_n_child == 2:
                 n_cur_child = len(self.children)
                 hit_online = False
 
                 for i in range(sub_n_child):
                     success = self.add_child_to(
@@ -288,14 +289,15 @@
                 self[Direction.X1Y1].include_online = True
 
             else:
                 raise ValueError(f"the number of {sub_n_child} child is invalid.")
 
             return True
 
+        # subtree.level < self.level
         if not self.is_empty():
             for d in DIREC_IDX:
                 if d in self:
                     flag = self[d].add_subtree(subtree, check_hit_online)
                     if flag:
                         return True
 
@@ -364,15 +366,15 @@
         if not L1_cluster.add_child(cluster):
             raise RoutingError(f"add child to L1 cluster failed.")
 
         return cluster
 
     def find_lx_clusters(
         self, lx: Level, n_child_avail_low: int = 0
-    ) -> List["RoutingCluster"]:
+    ) -> list["RoutingCluster"]:
         """Find all clusters at a `lx` level with at least `n_child_avail_low` child clusters."""
         if lx > self.level:
             return []
 
         clusters = []
 
         def dfs_preorder(root: RoutingCluster) -> None:
@@ -385,15 +387,15 @@
             for d in DIREC_IDX:
                 if d in root:
                     dfs_preorder(root[d])
 
         dfs_preorder(self)
         return clusters
 
-    def find_leaf_at_level(self, lx: Level) -> List["RoutingCluster"]:
+    def find_leaf_at_level(self, lx: Level) -> list["RoutingCluster"]:
         """Find clusters with no child at the `lx` level."""
         if lx == Level.L0:
             return []
 
         return self.find_lx_clusters(lx, self.node_capacity)
 
     def breadth_of_lx(self, lx: Level) -> int:
@@ -420,31 +422,31 @@
         return d in self.children
 
     @property
     def node_capacity(self) -> int:
         return HwConfig.N_SUB_ROUTING_NODE if self.level > Level.L0 else 0
 
 
-class RoutingGroup(List[CoreBlock]):
+class RoutingGroup(list[CoreBlock]):
     """Core blocks located within a routing group are routable.
 
     NOTE: Axon groups within a routing group are the same.
     """
 
     def __init__(self, *cb: CoreBlock) -> None:
         self.core_blocks = list(cb)
-        self.assigned_coords: List[Coord] = []
+        self.assigned_coords: list[Coord] = []
         """Assigned core coordinates in the routing group"""
-        self.wasted_coords: List[Coord] = []
+        self.wasted_coords: list[Coord] = []
         """Wasted core coordinates in routing group"""
-        self.wasted_core_plm: Dict[Coord, EmptyCorePlacement] = {}
+        self.wasted_core_plm: dict[Coord, EmptyCorePlacement] = {}
         """Wasted core placements"""
 
     def assign(
-        self, assigned: List[Coord], wasted: List[Coord], chip_coord: Coord
+        self, assigned: list[Coord], wasted: list[Coord], chip_coord: Coord
     ) -> None:
         self.assigned_coords = assigned
         self.wasted_coords = wasted
 
         # Assign the coordinates to each core block inside the routing group.
         cur_i = 0
         for cb in self:
@@ -508,15 +510,15 @@
             )
 
         return self[0].chip_coord
 
 
 @final
 class RoutingRoot:
-    def __init__(self, chip_list: List[ChipCoord], **kwargs) -> None:
+    def __init__(self, chip_list: list[ChipCoord], **kwargs) -> None:
         """Initialize a routing quadtree root."""
         self.chip_list = chip_list
         # Every L5 routing cluster is unique in each chip root.
         self.chip_roots = [
             RoutingCluster(Level.L5, include_online=True) for _ in range(len(chip_list))
         ]
 
@@ -566,14 +568,16 @@
             else:
                 l0 = routing_cluster.add_L0_for_placing(
                     status=Status.OCCUPIED, tag=f"{id(routing_group)}_{i}"
                 )
                 wasted.append(l0)
 
         # If #N of wasted cores > 16, it won't hit online L2 cluster.
+        # XXX 'check_hit_online' conditions could be more precise, but
+        # there is no clear benefit to doing so at the moment.
         check_hit_online = len(wasted) <= HwConfig.N_CORE_ONLINE
 
         # Add the sub-tree to the root.
         flag = False
         # TODO For now, use sequential attempt.
         for chip_coord, chip_root in zip(self.chip_list, self.chip_roots):
             flag = chip_root.add_subtree(routing_cluster, check_hit_online)
@@ -603,19 +607,25 @@
 
         return True
 
     def clear(self) -> None:
         for root in self:
             root.clear()
 
-    def breadth_of_lx_at(self, lx: Level, chip_idx: int) -> int:
-        return self[chip_idx].breadth_of_lx(lx)
+    def breadth_of_lx(self, lx: Union[Level, int], chip_idx: int = -1) -> int:
+        """Get the breadth of the given level at chip root #idx.
 
-    def breadth_of_lx(self, lx: Level) -> int:
-        return sum(chip_root.breadth_of_lx(lx) for chip_root in self)
+        Args:
+            - lx: the level to find.
+            - chip_idx: the chip root index. If it is -1, return the sum of the breadth on all roots.
+        """
+        if chip_idx == -1:
+            return sum(chip_root.breadth_of_lx(Level(lx)) for chip_root in self)
+
+        return self[chip_idx].breadth_of_lx(Level(lx))
 
     def __getitem__(self, index: int) -> RoutingCluster:
         return self.chip_roots[index]
 
     def __iter__(self) -> Iterator[RoutingCluster]:
         return self.chip_roots.__iter__()
```

### Comparing `paibox-1.1.0a2/paibox/backend/segment_utils.py` & `paibox-1.1.0a3/paibox/backend/segment_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import warnings
+from collections.abc import Sequence
 from functools import partial
 from math import ceil
-from typing import Dict, List, Literal, NamedTuple, Sequence
+from typing import Literal, NamedTuple
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
 from paicorelib import AxonCoord, AxonSegment, NeuronSegment
@@ -30,20 +31,20 @@
         return self.segment.n_addr
 
     def __str__(self) -> str:
         return f"NeuSeg {self.parent.name} at offset {self.segment.addr_offset}"
 
 
 NeuSlice: TypeAlias = slice
-NeuSegOfCorePlm: TypeAlias = List[NeuSeg]
-NeuSegOfCoreBlock: TypeAlias = List[NeuSegOfCorePlm]
+NeuSegOfCorePlm: TypeAlias = list[NeuSeg]
+NeuSegOfCoreBlock: TypeAlias = list[NeuSegOfCorePlm]
 
 
 def _place_seperately(
-    seg_slices_dict: Dict[NeuDyn, List[NeuSlice]], repl_prop: int
+    seg_slices_dict: dict[NeuDyn, list[NeuSlice]], repl_prop: int
 ) -> NeuSegOfCoreBlock:
     neu_segs_of_cb = []
 
     for neu, seg_slices in seg_slices_dict.items():
         neu_segs_of_cb.extend(
             [
                 [NeuSeg(neu, NeuronSegment(seg_slice, 0, repl_prop))]
@@ -54,40 +55,40 @@
     return neu_segs_of_cb
 
 
 def _coarse_group(
     neu: NeuDyn,
     capacity: int,
     load_type: Literal["average", "max_capacity"],
-) -> List[NeuSlice]:
+) -> list[NeuSlice]:
     """Group neurons with 'average' or 'maximum capacity' load type.
 
     NOTE: Group neuron seperately, like [N1], [N2], ..., [Nn]. For each neuron, \
         take unrolling factor into consideration, then distribute the neuron to \
         the cores evently.
 
         #N of cores required of nx = ceil(Ni / capacity) * uf
         Average load of nx = ceil(nx / (#N of cores required of nx))
     """
 
-    def _average_load(n: int, n_part: int) -> List[int]:
+    def _average_load(n: int, n_part: int) -> list[int]:
         """Distribute #num into #n_part parts evently."""
         quotient = ceil(n / n_part)
         rest = n - (n_part - 1) * quotient
 
         return [quotient] * (n_part - 1) + [rest]
 
-    def _max_capacity_load(n: int) -> List[int]:
+    def _max_capacity_load(n: int) -> list[int]:
         nonlocal capacity
         n_part = ceil(n / capacity)
         rest = n - (n_part - 1) * capacity
 
         return [capacity] * (n_part - 1) + [rest]
 
-    neu_seg_slices: List[NeuSlice] = []
+    neu_seg_slices: list[NeuSlice] = []
     n_neuron = neu.num_out
 
     if load_type == "average":
         n_core_required = ceil(n_neuron / capacity) * neu.unrolling_factor
         dist = _average_load(n_neuron, n_core_required)
     else:
         dist = _max_capacity_load(n_neuron)
@@ -97,15 +98,15 @@
         neu_seg_slices.append(NeuSlice(_sum, _sum + d, 1))
         _sum += d
 
     return neu_seg_slices
 
 
 def _get_nsg_opt_core(
-    seg_slices_dict: Dict[NeuDyn, List[NeuSlice]], capacity: int, repl_prop: int
+    seg_slices_dict: dict[NeuDyn, list[NeuSlice]], capacity: int, repl_prop: int
 ) -> NeuSegOfCoreBlock:
     neu_segs_of_cb: NeuSegOfCoreBlock = []  # The final result
     raise_warning = False
 
     for neu in seg_slices_dict:
         if neu.unrolling_factor > 1:
             neu.unrolling_factor = 1
@@ -174,36 +175,36 @@
 
     backtrack(0, 0, [])
 
     return neu_segs_of_cb
 
 
 def _get_neu_slices(
-    neu_groups: List[NeuDyn],
+    neu_groups: list[NeuDyn],
     capacity: int,
     load_type: Literal["average", "max_capacity"],
-) -> Dict[NeuDyn, List[NeuSlice]]:
+) -> dict[NeuDyn, list[NeuSlice]]:
     """Group the neuron groups by category with load balancing optimization.
 
     NOTE: Use load balancing optimization automatically.
     """
-    seg_slices_dict: Dict[NeuDyn, List[NeuSlice]] = dict()
+    seg_slices_dict: dict[NeuDyn, list[NeuSlice]] = dict()
 
     for neu in neu_groups:
         seg_slices_dict[neu] = _coarse_group(neu, capacity, load_type)
 
     return seg_slices_dict
 
 
 _get_neu_slices_opt_core = partial(_get_neu_slices, load_type="max_capacity")
 _get_neu_slices_opt_latency = partial(_get_neu_slices, load_type="average")
 
 
 def _dense_reorganized(
-    seg_slices_dict: Dict[NeuDyn, List[NeuSlice]], capacity: int, repl_prop: int
+    seg_slices_dict: dict[NeuDyn, list[NeuSlice]], capacity: int, repl_prop: int
 ) -> NeuSegOfCoreBlock:
     """Reorganize densely. Based on the result of 'latency' method, use greedy algorithm to \
         reorganize the incomplete neuron segments for saving cores.
     """
 
     def _find_neu_in_segs_of_cplm(neu: NeuDyn, seg_of_cplm: NeuSegOfCorePlm) -> bool:
         return any(neu == s.parent for s in seg_of_cplm)
@@ -251,15 +252,15 @@
                 neu_seg = NeuSeg(neu, NeuronSegment(seg_slice, 0, repl_prop))
                 neu_segs_of_cb.append([neu_seg])
 
     return neu_segs_of_cb
 
 
 def get_neu_segments(
-    neu_groups: List[NeuDyn],
+    neu_groups: list[NeuDyn],
     capacity: int,
     repl_prop: int,
     optim_target: Literal["latency", "core", "both"],
 ) -> NeuSegOfCoreBlock:
     """Get the neuron segments with a optimization strategy.
 
     Args:
@@ -280,15 +281,15 @@
             return _place_seperately(seg_slices_dict, repl_prop)
         else:
             return _dense_reorganized(seg_slices_dict, capacity, repl_prop)
 
 
 def get_axon_segments(
     axons: Sequence[SourceNodeType], tr_max: int, fan_in_max: int
-) -> Dict[SourceNodeType, AxonSegment]:
+) -> dict[SourceNodeType, AxonSegment]:
     """Divide axons into segments by group to fit the hardware constraints.
 
     Args:
         - axons: The axons to be segmented.
         - tr_max: The maximum value of the time slot(=n_timeslot).
         - fan_in_max: The value of fan-in per dendrite(=N_FANIN_PER_DENDRITE_XNN).
 
@@ -325,15 +326,15 @@
         axon_segments[axon] = segment
 
     return axon_segments
 
 
 def aligned_coords(
     neu_index: NeuSlice, axon_seg: AxonSegment, delay: int, dest_n_timeslot: int
-) -> List[AxonCoord]:
+) -> list[AxonCoord]:
     """Find the axon segments aligned with the index of neuron segment.
 
     The length of axon coordinates is the same as `neu_index`.
     """
     axon_coords = []
     addr_width = axon_seg.addr_width
     addr_offset = axon_seg.addr_offset
```

### Comparing `paibox-1.1.0a2/paibox/base.py` & `paibox-1.1.0a3/paibox/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import sys
-from typing import Any, ClassVar, Dict, List, Literal, Optional, Set, Tuple
+from typing import Any, ClassVar, Literal, Optional
 
 import numpy as np
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
@@ -11,19 +11,20 @@
 from paicorelib import WeightPrecision as WP
 
 from .collector import Collector
 from .mixin import ReceiveInputProj, StatusMemory, TimeRelatedNode
 from .naming import get_unique_name, is_name_unique
 from .node import NodeDict, NodeList
 from .types import WeightType
+from .utils import arg_check_pos
 
 __all__ = []
 
 
-_IdPathType: TypeAlias = Tuple[int, int]
+_IdPathType: TypeAlias = tuple[int, int]
 
 
 class PAIBoxObject:
     _excluded_vars = ()
     __avoid_name_conflict__: ClassVar[bool] = False
 
     def __init__(self, name: Optional[str] = None) -> None:
@@ -87,15 +88,15 @@
     def _find_nodes(
         self,
         method: Literal["absolute", "relative"] = "absolute",
         level: int = -1,
         include_self: bool = True,
         find_recursive: bool = False,
         _lid: int = 0,
-        _paths: Optional[Set[_IdPathType]] = None,
+        _paths: Optional[set[_IdPathType]] = None,
         _iter_termination: bool = False,
     ) -> Collector[str, "PAIBoxObject"]:
         if _paths is None:
             _paths = set()
 
         gather = Collector()
 
@@ -110,14 +111,16 @@
                 return gather
         else:
             if (level > -1) and (_lid >= level):
                 return gather
 
         iter_termi = True  # iteration termination flag
 
+        from .simulator import Probe
+
         def _find_nodes_absolute() -> None:
             nonlocal gather, nodes, iter_termi
 
             for v in self.__dict__.values():
                 if isinstance(v, PAIBoxObject):
                     iter_termi = False
                     _add_node2(self, v, _paths, gather, nodes)
@@ -140,14 +143,16 @@
                         level=level,
                         include_self=include_self,
                         find_recursive=find_recursive,
                         _lid=_lid + 1,
                         _paths=_paths,
                         _iter_termination=iter_termi,
                     )
+                    if not isinstance(v, Probe)
+                    else {}
                 )
 
         def _find_nodes_relative() -> None:
             nonlocal gather, nodes, iter_termi
 
             for k, v in self.__dict__.items():
                 if isinstance(v, PAIBoxObject):
@@ -162,25 +167,26 @@
                     for k2, v2 in v.items():
                         if isinstance(v2, PAIBoxObject):
                             iter_termi = False
                             _add_node1(self, f"{k}.{k2}", v2, _paths, gather, nodes)
 
             # finding nodes recursively
             for k1, v1 in nodes:
-                for k2, v2 in v1._find_nodes(
-                    method=method,
-                    level=level,
-                    include_self=include_self,
-                    find_recursive=find_recursive,
-                    _lid=_lid + 1,
-                    _paths=_paths,
-                    _iter_termination=iter_termi,
-                ).items():
-                    if k2:
-                        gather[f"{k1}.{k2}"] = v2
+                if not isinstance(v1, Probe):
+                    for k2, v2 in v1._find_nodes(
+                        method=method,
+                        level=level,
+                        include_self=include_self,
+                        find_recursive=find_recursive,
+                        _lid=_lid + 1,
+                        _paths=_paths,
+                        _iter_termination=iter_termi,
+                    ).items():
+                        if k2:
+                            gather[f"{k1}.{k2}"] = v2
 
         nodes = []
 
         if method == "absolute":
             _find_nodes_absolute()
         else:
             _find_nodes_relative()
@@ -188,32 +194,32 @@
         return gather
 
 
 def _add_node1(
     obj: Any,
     k: str,
     v: PAIBoxObject,
-    _paths: Set[_IdPathType],
+    _paths: set[_IdPathType],
     gather: Collector[str, PAIBoxObject],
-    nodes: List[Tuple[str, PAIBoxObject]],
+    nodes: list[tuple[str, PAIBoxObject]],
 ) -> None:
     path = (id(obj), id(v))
 
     if path not in _paths:
         _paths.add(path)
         gather[k] = v
         nodes.append((k, v))
 
 
 def _add_node2(
     obj: Any,
     v: PAIBoxObject,
-    _paths: Set[_IdPathType],
+    _paths: set[_IdPathType],
     gather: Collector[str, PAIBoxObject],
-    nodes: List[PAIBoxObject],
+    nodes: list[PAIBoxObject],
 ) -> None:
     path = (id(obj), id(v))
 
     if path not in _paths:
         _paths.add(path)
         gather[v.name] = v
         nodes.append(v)
@@ -234,20 +240,20 @@
     def update(self, *args, **kwargs):
         raise NotImplementedError
 
     def reset_state(self, *args, **kwargs):
         raise NotImplementedError
 
     @property
-    def shape_in(self) -> Tuple[int, ...]:
+    def shape_in(self) -> tuple[int, ...]:
         """Actual shape of input."""
         raise NotImplementedError
 
     @property
-    def shape_out(self) -> Tuple[int, ...]:
+    def shape_out(self) -> tuple[int, ...]:
         """Actual shape of output."""
         raise NotImplementedError
 
     @property
     def num_in(self) -> int:
         raise NotImplementedError
 
@@ -271,26 +277,23 @@
 
 
 class NeuDyn(DynamicSys, ReceiveInputProj, TimeRelatedNode):
     def __init__(self, name: Optional[str] = None) -> None:
         super().__init__(name)
         self.master_nodes = NodeDict()
 
-    def export_params(self) -> Dict[str, Any]:
+    def export_params(self) -> dict[str, Any]:
         """Export the parameters into dictionary."""
         params = {}
 
         for k, v in self.__dict__.items():
             if k in self._excluded_vars:
                 continue
 
-            if sys.version_info >= (3, 9):
-                params.update({k.removeprefix("_"): v})
-            else:
-                params.update({k.lstrip("_"): v})  # compatible for py3.8
+            params.update({k.removeprefix("_"): v})
 
         return params
 
     def is_working(self) -> bool:
         return (self.tick_wait_start > 0 and self.timestamp >= 0) and (
             self.tick_wait_end == 0 or self.timestamp + 1 <= self.tick_wait_end
         )
@@ -309,18 +312,15 @@
 
     @property
     def unrolling_factor(self) -> int:
         return self._uf
 
     @unrolling_factor.setter
     def unrolling_factor(self, factor: int) -> None:
-        if factor < 1:
-            raise ValueError(f"'unrolling_factor' must be positive, but got {factor}.")
-
-        self._uf = factor
+        self._uf = arg_check_pos(factor, "'unrolling_factor'")
 
 
 class SynSys(DynamicSys):
     CFLAG_ENABLE_WP_OPTIMIZATION: ClassVar[bool] = True
     """Compilation flag for weight precision optimization."""
 
     @property
```

### Comparing `paibox-1.1.0a2/paibox/collector.py` & `paibox-1.1.0a3/paibox/collector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,18 @@
-from typing import (
-    Callable,
-    Dict,
-    MutableMapping,
-    Sequence,
-    Type,
-    TypeVar,
-    Union,
-    overload,
-)
+from collections.abc import Callable, MutableMapping, Sequence
+from typing import TypeVar, Union, overload
 
 _T = TypeVar("_T")
 _KT = TypeVar("_KT")
 _VT = TypeVar("_VT")
 
 # XXX: use collections.UserDict[_KT, _VT] in 3.9+
 
 
-class Collector(Dict[_KT, _VT]):
+class Collector(dict[_KT, _VT]):
     def __setitem__(self, key, value) -> None:
         if key in self:
             if id(self[key]) != id(value):
                 raise ValueError(
                     f"mame '{key}' conflicts: same name for {value} & {self[key]}."
                 )
 
@@ -118,42 +110,42 @@
                 if k not in gather:
                     raise KeyError(f"key '{k}' not found. Removed failed.")
 
                 gather.pop(k)
 
         return gather
 
-    def subset(self, obj_type: Type[_T]) -> "Collector[_KT, _T]":
+    def subset(self, obj_type: type[_T]) -> "Collector[_KT, _T]":
         gather = Collector()
 
         for k, v in self.items():
             if isinstance(v, obj_type):
                 gather[k] = v
 
         return gather
 
-    def not_subset(self, obj_type: Type[_T]) -> "Collector[_KT, _VT]":
+    def not_subset(self, obj_type: type[_T]) -> "Collector[_KT, _VT]":
         gather = type(self)()
 
         for k, v in self.items():
             if not isinstance(v, obj_type):
                 gather[k] = v
 
         return gather
 
-    def include(self, *types: Type[_T]) -> "Collector[_KT, _T]":
+    def include(self, *types: type[_T]) -> "Collector[_KT, _T]":
         gather = Collector()
 
         for k, v in self.items():
             if isinstance(v, types):
                 gather[k] = v
 
         return gather
 
-    def exclude(self, *types: Type[_T]) -> "Collector[_KT, _VT]":
+    def exclude(self, *types: type[_T]) -> "Collector[_KT, _VT]":
         gather = type(self)()
 
         for k, v in self.items():
             if not isinstance(v, types):
                 gather[k] = v
 
         return gather
```

### Comparing `paibox-1.1.0a2/paibox/components/functional.py` & `paibox-1.1.0a3/paibox/components/functional.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,62 @@
-import warnings
+import sys
+from collections.abc import Sequence
 from functools import partial
-from typing import Literal, Optional, Sequence, Tuple, Union
+from typing import Literal, Optional, Union
 
 import numpy as np
 from numpy.typing import NDArray
-from paicorelib import LCM, NTM, RM, TM
+from paicorelib import NTM, RM, TM
 
 from paibox.base import NeuDyn, NodeList
-from paibox.exceptions import FunctionalError, PAIBoxWarning, ShapeError
+from paibox.exceptions import PAIBoxDeprecationWarning, ShapeError
 from paibox.network import DynSysGroup
 from paibox.types import SpikeType, VoltageType
-from paibox.utils import as_shape, shape2num
+from paibox.utils import arg_check_non_neg, as_shape, shape2num, typical_round
 
 from .modules import (
     BuiltComponentType,
     FunctionalModule,
     FunctionalModule2to1,
     FunctionalModule2to1WithV,
+    FunctionalModuleWithV,
     TransposeModule,
 )
 from .neuron import Neuron
 from .neuron.neurons import *
-from .neuron.utils import VJT_MIN_LIMIT, _is_vjt_overflow
+from .neuron.utils import vjt_overflow
 from .projection import InputProj
-from .synapses import FullConnSyn
-from .synapses import GeneralConnType as GConnType
+from .synapses import ConnType, FullConnSyn
 from .synapses.conv_types import _Size2Type
 from .synapses.conv_utils import _fm_ndim2_check, _pair
-from .synapses.transforms import _Pool2dForward
+from .synapses.transforms import Conv2dForward, _Pool2dForward
+
+if sys.version_info >= (3, 13):
+    from warnings import deprecated
+else:
+    from typing_extensions import deprecated
 
 __all__ = [
     "BitwiseAND",
     "BitwiseNOT",
     "BitwiseOR",
     "BitwiseXOR",
     "DelayChain",
     "SpikingAdd",
     "SpikingAvgPool2d",
+    "SpikingAvgPool2dWithV",
     "SpikingMaxPool2d",
     "SpikingSub",
     "Transpose2d",
     "Transpose3d",
 ]
 
 
 _L_SADD = 1  # Literal value for spiking addition.
 _L_SSUB = -1  # Literal value for spiking subtraction.
-VJT_OVERFLOW_ERROR_TEXT = "Membrane potential overflow causes spiking addition errors."
 
 
 class BitwiseAND(FunctionalModule2to1):
     inherent_delay = 0
 
     def __init__(
         self,
@@ -84,47 +90,47 @@
     def spike_func(self, x1: SpikeType, x2: SpikeType, **kwargs) -> SpikeType:
         return x1 & x2
 
     def build(self, network: DynSysGroup, **build_options) -> BuiltComponentType:
         # 1. Instantiate neurons & synapses & connect the source
         n1_and = Neuron(
             self.shape_out,
-            leak_comparison=LCM.LEAK_BEFORE_COMP,
+            neg_threshold=0,
             leak_v=-1,
             delay=self.delay_relative,
             tick_wait_start=self.tick_wait_start,
             tick_wait_end=self.tick_wait_end,
             keep_shape=self.keep_shape,
             name=f"n0_{self.name}",
         )
 
         syn1 = FullConnSyn(
             self.module_intf.operands[0],
             n1_and,
             1,
-            conn_type=GConnType.One2One,
+            conn_type=ConnType.One2One,
             name=f"s0_{self.name}",
         )
         syn2 = FullConnSyn(
             self.module_intf.operands[1],
             n1_and,
             1,
-            conn_type=GConnType.One2One,
+            conn_type=ConnType.One2One,
             name=f"s1_{self.name}",
         )
 
         generated = [n1_and, syn1, syn2]
 
         # 2. Connect the source of all backward synapses to output neuron.
         for syn in self.module_intf.output:
             syn.source = n1_and
 
         # 3. Add the components to the network & remove the module itself.
         network._add_components(*generated)
-        # network._remove_components(self)
+        network._remove_components(self)
 
         return generated
 
 
 class BitwiseNOT(FunctionalModule):
     inherent_delay = 0
 
@@ -156,40 +162,41 @@
             **kwargs,
         )
 
     def spike_func(self, x1: SpikeType, **kwargs) -> SpikeType:
         return ~x1
 
     def build(self, network: DynSysGroup, **build_options) -> BuiltComponentType:
-        n1_not = Neuron(
+        n1_not = LIF(
             self.shape_out,
-            leak_comparison=LCM.LEAK_BEFORE_COMP,
-            leak_v=-1,
+            threshold=1,
+            neg_threshold=0,
+            leak_v=1,
             delay=self.delay_relative,
             tick_wait_start=self.tick_wait_start,
             tick_wait_end=self.tick_wait_end,
             keep_shape=self.keep_shape,
             name=f"n0_{self.name}",
         )
 
         syn1 = FullConnSyn(
             self.module_intf.operands[0],
             n1_not,
             weights=-1,
-            conn_type=GConnType.One2One,
+            conn_type=ConnType.One2One,
             name=f"s0_{self.name}",
         )
 
         generated = [n1_not, syn1]
 
         for syns in self.module_intf.output:
             syns.source = n1_not
 
         network._add_components(*generated)
-        # network._remove_components(self)
+        network._remove_components(self)
 
         return generated
 
 
 class BitwiseOR(FunctionalModule2to1):
     inherent_delay = 0
 
@@ -225,32 +232,32 @@
             name=f"n0_{self.name}",
         )
 
         syn1 = FullConnSyn(
             self.module_intf.operands[0],
             n1_or,
             1,
-            conn_type=GConnType.One2One,
+            conn_type=ConnType.One2One,
             name=f"s0_{self.name}",
         )
         syn2 = FullConnSyn(
             self.module_intf.operands[1],
             n1_or,
             1,
-            conn_type=GConnType.One2One,
+            conn_type=ConnType.One2One,
             name=f"s1_{self.name}",
         )
 
         generated = [n1_or, syn1, syn2]
 
         for syns in self.module_intf.output:
             syns.source = n1_or
 
         network._add_components(*generated)
-        # network._remove_components(self)
+        network._remove_components(self)
 
         return generated
 
 
 class BitwiseXOR(FunctionalModule2to1):
     inherent_delay = 1
 
@@ -292,52 +299,52 @@
 
         identity = np.identity(self.num_out, dtype=np.int8)
         # weight of syn1, (-1*(N,), 1*(N,))
         syn1 = FullConnSyn(
             self.module_intf.operands[0],
             n1_aux,
             weights=np.hstack([-1 * identity, identity], casting="safe", dtype=np.int8),
-            conn_type=GConnType.MatConn,
+            conn_type=ConnType.All2All,
             name=f"s0_{self.name}",
         )
         # weight of syn2, (1*(N,), -1*(N,))
         syn2 = FullConnSyn(
             self.module_intf.operands[1],
             n1_aux,
             weights=np.hstack([identity, -1 * identity], casting="safe", dtype=np.int8),
-            conn_type=GConnType.MatConn,
+            conn_type=ConnType.All2All,
             name=f"s1_{self.name}",
         )
 
         # The shape of n2 is (N,) or (h1, w1).
         n2_xor = SpikingRelu(
             self.shape_out,
             delay=self.delay_relative,
-            tick_wait_start=self.tick_wait_start + 1,
+            tick_wait_start=n1_aux.tick_wait_start + 1,
             tick_wait_end=self.tick_wait_end,
             keep_shape=self.keep_shape,
             name=f"n1_{self.name}",
         )
 
         # weight of syn3, identity matrix with shape (2N, N)
         syn3 = FullConnSyn(
             n1_aux,
             n2_xor,
-            weights=np.vstack([identity, -1 * identity], casting="safe", dtype=np.int8),
-            conn_type=GConnType.MatConn,
+            weights=np.vstack([identity, identity], casting="safe", dtype=np.int8),
+            conn_type=ConnType.All2All,
             name=f"s2_{self.name}",
         )
 
         generated = [n1_aux, n2_xor, syn1, syn2, syn3]
 
         for syns in self.module_intf.output:
             syns.source = n2_xor
 
         network._add_components(*generated)
-        # network._remove_components(self)
+        network._remove_components(self)
 
         return generated
 
 
 class DelayChain(FunctionalModule):
     def __init__(
         self,
@@ -362,15 +369,16 @@
             shape_out = (neuron.num_out,)
 
         if chain_level < 1:
             raise ValueError(
                 f"the level of delay chain must be positive, but got {chain_level}."
             )
 
-        self.inherent_delay = chain_level
+        self.chain_level = chain_level
+        self.inherent_delay = chain_level - 1
 
         super().__init__(
             neuron,
             shape_out=shape_out,
             keep_shape=keep_shape,
             name=name,
             **kwargs,
@@ -380,60 +388,60 @@
         return x1
 
     def build(self, network: DynSysGroup, **build_options) -> BuiltComponentType:
         n_delaychain = NodeList()
         s_delaychain = NodeList()
 
         # Delay chain of length #D.
-        for i in range(self.inherent_delay - 1):
+        for i in range(self.chain_level - 1):
             n_delay = SpikingRelu(
                 self.shape_out,
                 tick_wait_start=self.tick_wait_start + i,
                 tick_wait_end=self.tick_wait_end,
                 delay=1,
                 name=f"n{i}_{self.name}",
             )
             n_delaychain.append(n_delay)
 
         # delay = delay_relative for output neuron
         n_out = SpikingRelu(
             self.shape_out,
-            tick_wait_start=self.tick_wait_start + i,
+            tick_wait_start=self.tick_wait_start + i + 1,
             tick_wait_end=self.tick_wait_end,
             delay=self.delay_relative,
-            name=f"n{self.inherent_delay-1}_{self.name}",
+            name=f"n{i+1}_{self.name}",
         )
         n_delaychain.append(n_out)  # Must append to the last.
 
         syn_in = FullConnSyn(
             self.module_intf.operands[0],
             n_delaychain[0],
             1,
-            conn_type=GConnType.One2One,
+            conn_type=ConnType.One2One,
             name=f"s0_{self.name}",
         )
 
-        for i in range(self.inherent_delay - 1):
+        for i in range(self.chain_level - 1):
             s_delay = FullConnSyn(
                 n_delaychain[i],
                 n_delaychain[i + 1],
                 1,
-                conn_type=GConnType.One2One,
+                conn_type=ConnType.One2One,
                 name=f"s{i+1}_{self.name}",
             )
 
             s_delaychain.append(s_delay)
 
         generated = [*n_delaychain, syn_in, *s_delaychain]
 
         for syns in self.module_intf.output:
             syns.source = n_out
 
         network._add_components(*generated)
-        # network._remove_components(self)
+        network._remove_components(self)
 
         return generated
 
 
 class SpikingAdd(FunctionalModule2to1WithV):
     inherent_delay = 0
 
@@ -456,15 +464,15 @@
                 raised if the result overflows during simulation.
 
         NOTE: the inherent delay of the module is 0.
         """
         self.overflow_strict = overflow_strict
         super().__init__(neuron_a, neuron_b, keep_shape=keep_shape, name=name, **kwargs)
 
-    def spike_func(self, vjt: VoltageType, **kwargs) -> Tuple[SpikeType, VoltageType]:
+    def spike_func(self, vjt: VoltageType, **kwargs) -> tuple[SpikeType, VoltageType]:
         """Simplified neuron computing mechanism as the operator function."""
         return _spike_func_sadd_ssub(vjt)
 
     def synaptic_integr(
         self, x1: SpikeType, x2: SpikeType, vjt_pre: VoltageType
     ) -> VoltageType:
         return _sum_inputs_sadd_ssub(
@@ -472,95 +480,171 @@
         )
 
     def build(self, network: DynSysGroup, **build_options) -> BuiltComponentType:
         n1_sadd = Neuron(
             self.shape_out,
             reset_mode=RM.MODE_LINEAR,
             neg_thres_mode=NTM.MODE_SATURATION,
+            neg_threshold=0,
             delay=self.delay_relative,
             tick_wait_start=self.tick_wait_start,
             tick_wait_end=self.tick_wait_end,
             keep_shape=self.keep_shape,
             name=f"n0_{self.name}",
         )
 
         syn1 = FullConnSyn(
             self.module_intf.operands[0],
             n1_sadd,
             1,
-            conn_type=GConnType.One2One,
+            conn_type=ConnType.One2One,
             name=f"s0_{self.name}",
         )
         syn2 = FullConnSyn(
             self.module_intf.operands[1],
             n1_sadd,
             1,
-            conn_type=GConnType.One2One,
+            conn_type=ConnType.One2One,
             name=f"s1_{self.name}",
         )
 
         generated = [n1_sadd, syn1, syn2]
 
         for syns in self.module_intf.output:
             syns.source = n1_sadd
 
         network._add_components(*generated)
-        # network._remove_components(self)
+        network._remove_components(self)
+
+        return generated
+
+
+class _SpikingPool2dWithV(FunctionalModuleWithV):
+    inherent_delay = 0
+
+    def __init__(
+        self,
+        neuron: Union[NeuDyn, InputProj],
+        kernel_size: _Size2Type,
+        stride: Optional[_Size2Type] = None,
+        padding: _Size2Type = 0,
+        pos_thres: Optional[int] = None,
+        keep_shape: bool = True,
+        name: Optional[str] = None,
+        **kwargs,
+    ) -> None:
+        """Basic 2d spiking pooling."""
+        # C,H,W
+        cin, ih, iw = _fm_ndim2_check(neuron.shape_out, "CHW")
+
+        _ksize = _pair(kernel_size)
+        _kernel = np.ones((cin, cin, *_ksize), dtype=np.int8)
+        _stride = _pair(stride) if stride is not None else _ksize
+        _padding = _pair(padding)
+
+        oh = (ih + 2 * _padding[0] - _ksize[0]) // _stride[0] + 1
+        ow = (iw + 2 * _padding[1] - _ksize[1]) // _stride[1] + 1
+
+        if keep_shape:
+            shape_out = (cin, oh, ow)
+        else:
+            shape_out = (cin * oh * ow,)
+
+        if isinstance(pos_thres, int):
+            self.pos_thres = arg_check_non_neg(pos_thres, "positive threshold")
+        else:
+            self.pos_thres = typical_round(shape2num(_ksize) / 2)
+
+        self.tfm = Conv2dForward((ih, iw), (oh, ow), _kernel, _stride, _padding)
+
+        super().__init__(
+            neuron,
+            shape_out=shape_out,
+            keep_shape=keep_shape,
+            name=name,
+            **kwargs,
+        )
+
+    def spike_func(self, vjt: VoltageType, **kwargs) -> tuple[SpikeType, VoltageType]:
+        return _spike_func_avg_pool(vjt, self.pos_thres)
+
+    def synaptic_integr(self, x1: SpikeType, vjt_pre: VoltageType) -> VoltageType:
+        return vjt_overflow((vjt_pre + self.tfm(x1).ravel()).astype(np.int32))
+
+    def build(self, network: DynSysGroup, **build_options) -> BuiltComponentType:
+        n1_ap2d = IF(
+            self.shape_out,
+            threshold=self.pos_thres,
+            reset_v=0,
+            delay=self.delay_relative,
+            tick_wait_start=self.tick_wait_start,
+            tick_wait_end=self.tick_wait_end,
+            keep_shape=self.keep_shape,
+            name=f"n0_{self.name}",
+        )
+
+        syn1 = FullConnSyn(
+            self.module_intf.operands[0],
+            n1_ap2d,
+            weights=self.tfm.connectivity.astype(np.bool_),
+            conn_type=ConnType.All2All,
+            name=f"s0_{self.name}",
+        )
+
+        generated = [n1_ap2d, syn1]
+
+        for syns in self.module_intf.output:
+            syns.source = n1_ap2d
+
+        network._add_components(*generated)
+        network._remove_components(self)
 
         return generated
 
 
 class _SpikingPool2d(FunctionalModule):
     inherent_delay = 0
 
     def __init__(
         self,
         neuron: Union[NeuDyn, InputProj],
         kernel_size: _Size2Type,
         pool_type: Literal["avg", "max"],
         stride: Optional[_Size2Type] = None,
-        # padding: _Size2Type = 0,
+        padding: _Size2Type = 0,
+        threshold: Optional[int] = None,
         # fm_order: _Order3d = "CHW",
         keep_shape: bool = True,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
-        """2d pooling for spike.
-
-        Args:
-            - neuron: of which the pooling will be performed.
-            - kernel_size: the size of the window to take a max over.
-            - pool_type: type of pooling, "avg" or "max".
-            - stride: the stride of the window. Default value is `kernel_size`.
-
-        NOTE: the inherent delay of the module is 0.
-        """
+        """Basic 2d spiking pooling."""
         if pool_type not in ("avg", "max"):
             raise ValueError("type of pooling must be 'avg' or 'max'.")
 
         # if fm_order not in ("CHW", "HWC"):
         #     raise ValueError("feature map order must be 'CHW' or 'HWC'.")
 
         # C,H,W
         cin, ih, iw = _fm_ndim2_check(neuron.shape_out, "CHW")
 
         _ksize = _pair(kernel_size)
         _stride = _pair(stride) if stride is not None else _ksize
-        _padding = _pair(0)
+        _padding = _pair(padding)
 
         oh = (ih + 2 * _padding[0] - _ksize[0]) // _stride[0] + 1
         ow = (iw + 2 * _padding[1] - _ksize[1]) // _stride[1] + 1
 
         if keep_shape:
             shape_out = (cin, oh, ow)
         else:
             shape_out = (cin * oh * ow,)
 
         self.tfm = _Pool2dForward(
-            cin, (ih, iw), (oh, ow), _ksize, _stride, _padding, pool_type
+            cin, (ih, iw), (oh, ow), _ksize, _stride, _padding, pool_type, threshold
         )
 
         super().__init__(
             neuron,
             shape_out=shape_out,
             keep_shape=keep_shape,
             name=name,
@@ -568,75 +652,108 @@
         )
 
     def spike_func(self, x1: SpikeType, **kwargs) -> SpikeType:
         return self.tfm(x1)
 
     def build(self, network: DynSysGroup, **build_options) -> BuiltComponentType:
         if self.tfm.pool_type == "avg":
-            n1_mp = Neuron(
+            n1_p2d = Neuron(
                 self.shape_out,
-                leak_comparison=LCM.LEAK_BEFORE_COMP,
-                leak_v=-(shape2num(self.tfm.ksize) // 2),
+                leak_v=1 - self.tfm.threshold,
+                neg_threshold=0,
                 delay=self.delay_relative,
                 tick_wait_start=self.tick_wait_start,
                 tick_wait_end=self.tick_wait_end,
                 keep_shape=self.keep_shape,
             )
         else:  # "max"
-            n1_mp = SpikingRelu(
+            n1_p2d = SpikingRelu(
                 self.shape_out,
                 delay=self.delay_relative,
                 tick_wait_start=self.tick_wait_start,
                 tick_wait_end=self.tick_wait_end,
                 keep_shape=self.keep_shape,
                 name=f"n0_{self.name}",
             )
 
         syn1 = FullConnSyn(
             self.module_intf.operands[0],
-            n1_mp,
+            n1_p2d,
             weights=self.tfm.connectivity.astype(np.bool_),
-            conn_type=GConnType.MatConn,
+            conn_type=ConnType.All2All,
             name=f"s0_{self.name}",
         )
 
-        generated = [n1_mp, syn1]
+        generated = [n1_p2d, syn1]
 
         for syns in self.module_intf.output:
-            syns.source = n1_mp
+            syns.source = n1_p2d
 
         network._add_components(*generated)
-        # network._remove_components(self)
+        network._remove_components(self)
 
         return generated
 
 
 class SpikingAvgPool2d(_SpikingPool2d):
     def __init__(
         self,
         neuron: Union[NeuDyn, InputProj],
         kernel_size: _Size2Type,
         stride: Optional[_Size2Type] = None,
-        # padding: _Size2Type = 0,
+        padding: _Size2Type = 0,
+        threshold: Optional[int] = None,
         # fm_order: _Order3d = "CHW",
         *,
         keep_shape: bool = True,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
         """2d average pooling for spike. The input feature map is in 'CHW' order by default.
 
         Args:
             - neuron: the target neuron to be pooled.
             - kernel_size: the size of the window to take a max over.
             - stride: the stride of the window. Default value is `kernel_size`.
+            - padding: the amount of zero-padding applied to the input. It can be a scalar or a tuple of 2  \
+                integers.
+            - threshold: if specified, the pooling result is o = (sum of the pooling window > threshold).   \
+                Otherwise the threshold is kernel_size // 2.
 
         NOTE: the inherent delay of the module is 0.
         """
-        super().__init__(neuron, kernel_size, "avg", stride, keep_shape, name, **kwargs)
+        super().__init__(
+            neuron,
+            kernel_size,
+            "avg",
+            stride,
+            padding,
+            threshold,
+            keep_shape,
+            name,
+            **kwargs,
+        )
+
+
+class SpikingAvgPool2dWithV(_SpikingPool2dWithV):
+    def __init__(
+        self,
+        neuron: Union[NeuDyn, InputProj],
+        kernel_size: _Size2Type,
+        stride: Optional[_Size2Type] = None,
+        padding: _Size2Type = 0,
+        threshold: Optional[int] = None,
+        *,
+        keep_shape: bool = True,
+        name: Optional[str] = None,
+        **kwargs,
+    ) -> None:
+        super().__init__(
+            neuron, kernel_size, stride, padding, threshold, keep_shape, name, **kwargs
+        )
 
 
 class SpikingMaxPool2d(_SpikingPool2d):
     """
     XXX: By enabling `MaxPoolingEnable` in neurons, the max pooling function can also be implemented.       \
         However, since the second-level cache of the input buffer before the physical core is in 144*8bit   \
         format, it is extremely wasteful when the input data is 1bit (i.e., spike). Therefore, we still     \
@@ -644,31 +761,42 @@
     """
 
     def __init__(
         self,
         neuron: Union[NeuDyn, InputProj],
         kernel_size: _Size2Type,
         stride: Optional[_Size2Type] = None,
-        # padding: _Size2Type = 0,
+        padding: _Size2Type = 0,
         # fm_order: _Order3d = "CHW",
         *,
         keep_shape: bool = True,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
         """2d max pooling for spike.
 
         Args:
             - neuron: the target neuron to be pooled.
             - kernel_size: the size of the window to take a max over.
             - stride: the stride of the window. Default value is `kernel_size`.
+            - padding: the amount of zero-padding applied to the input. It can be a scalar or a tuple of 2  \
+                integers.
 
         NOTE: the inherent delay of the module is 0.
         """
-        super().__init__(neuron, kernel_size, "max", stride, keep_shape, name, **kwargs)
+        super().__init__(
+            neuron,
+            kernel_size,
+            "max",
+            stride,
+            padding,
+            keep_shape=keep_shape,
+            name=name,
+            **kwargs,
+        )
 
 
 class SpikingSub(FunctionalModule2to1WithV):
     inherent_delay = 0
 
     def __init__(
         self,
@@ -689,64 +817,67 @@
                 raised if the result overflows during simulation.
 
         NOTE: the inherent delay of the module is 0.
         """
         self.overflow_strict = overflow_strict
         super().__init__(neuron_a, neuron_b, keep_shape=keep_shape, name=name, **kwargs)
 
-    def spike_func(self, vjt: VoltageType, **kwargs) -> Tuple[SpikeType, VoltageType]:
+    def spike_func(self, vjt: VoltageType, **kwargs) -> tuple[SpikeType, VoltageType]:
         """Simplified neuron computing mechanism to generate output spike."""
         return _spike_func_sadd_ssub(vjt)
 
     def synaptic_integr(
         self, x1: SpikeType, x2: SpikeType, vjt_pre: VoltageType
     ) -> VoltageType:
         return _sum_inputs_sadd_ssub(
             x1, x2, vjt_pre, _L_SSUB, strict=self.overflow_strict
         )
 
     def build(self, network: DynSysGroup, **build_options) -> BuiltComponentType:
         n1_ssub = Neuron(
             self.shape_out,
-            neg_threshold=VJT_MIN_LIMIT,
             reset_mode=RM.MODE_LINEAR,
             neg_thres_mode=NTM.MODE_SATURATION,
             delay=self.delay_relative,
             tick_wait_start=self.tick_wait_start,
             tick_wait_end=self.tick_wait_end,
             keep_shape=self.keep_shape,
             name=f"n0_{self.name}",
         )
 
         syn1 = FullConnSyn(
             self.module_intf.operands[0],
             n1_ssub,
             1,
-            conn_type=GConnType.One2One,
+            conn_type=ConnType.One2One,
             name=f"s0_{self.name}",
         )
         syn2 = FullConnSyn(
             self.module_intf.operands[1],
             n1_ssub,
             weights=-1,
-            conn_type=GConnType.One2One,
+            conn_type=ConnType.One2One,
             name=f"s1_{self.name}",
         )
 
         generated = [n1_ssub, syn1, syn2]
 
         for syns in self.module_intf.output:
             syns.source = n1_ssub
 
         network._add_components(*generated)
-        # network._remove_components(self)
+        network._remove_components(self)
 
         return generated
 
 
+@deprecated(
+    "'Transpose2d' will be removed in a future version. Use 'MatMul2d' instead.",
+    category=PAIBoxDeprecationWarning,
+)
 class Transpose2d(TransposeModule):
     def __init__(
         self,
         neuron: Union[NeuDyn, InputProj],
         *,
         keep_shape: bool = True,
         name: Optional[str] = None,
@@ -770,42 +901,46 @@
 
     def spike_func(self, x1: SpikeType, **kwargs) -> SpikeType:
         _x1 = x1.reshape(self.shape_in)
 
         return _x1.T
 
     def build(self, network: DynSysGroup, **build_options) -> BuiltComponentType:
-        n1_t2d = Neuron(
+        n1_t2d = SpikingRelu(
             self.shape_out,
             delay=self.delay_relative,
             tick_wait_start=self.tick_wait_start,
             tick_wait_end=self.tick_wait_end,
             keep_shape=self.keep_shape,
             name=f"n0_{self.name}",
         )
 
         syn1 = FullConnSyn(
             self.module_intf.operands[0],
             n1_t2d,
             weights=_transpose2d_mapping(self.shape_in),
-            conn_type=GConnType.MatConn,
+            conn_type=ConnType.All2All,
             name=f"s0_{self.name}",
         )
 
         generated = [n1_t2d, syn1]
 
         for syns in self.module_intf.output:
             syns.source = n1_t2d
 
         network._add_components(*generated)
-        # network._remove_components(self)
+        network._remove_components(self)
 
         return generated
 
 
+@deprecated(
+    "'Transpose3d' will be removed in a future version. Use 'MatMul2d' instead.",
+    category=PAIBoxDeprecationWarning,
+)
 class Transpose3d(TransposeModule):
     def __init__(
         self,
         neuron: Union[NeuDyn, InputProj],
         axes: Optional[Sequence[int]] = None,
         *,
         keep_shape: bool = True,
@@ -834,92 +969,100 @@
 
     def spike_func(self, x1: SpikeType, **kwargs) -> SpikeType:
         _x1 = x1.reshape(self.shape_in)
 
         return _x1.transpose(self.axes)
 
     def build(self, network: DynSysGroup, **build_options) -> BuiltComponentType:
-        n1_t3d = Neuron(
+        n1_t3d = SpikingRelu(
             self.shape_out,
             delay=self.delay_relative,
             tick_wait_start=self.tick_wait_start,
             tick_wait_end=self.tick_wait_end,
             keep_shape=self.keep_shape,
             name=f"n0_{self.name}",
         )
 
         syn1 = FullConnSyn(
             self.module_intf.operands[0],
             n1_t3d,
             weights=_transpose3d_mapping(self.shape_in, self.axes),
-            conn_type=GConnType.MatConn,
+            conn_type=ConnType.All2All,
             name=f"s0_{self.name}",
         )
 
         generated = [n1_t3d, syn1]
 
         for syns in self.module_intf.output:
             syns.source = n1_t3d
 
         network._add_components(*generated)
-        # network._remove_components(self)
+        network._remove_components(self)
 
         return generated
 
 
-def _spike_func_sadd_ssub(vjt: VoltageType) -> Tuple[SpikeType, VoltageType]:
+def _spike_func_sadd_ssub(vjt: VoltageType) -> tuple[SpikeType, VoltageType]:
     """Function `spike_func()` in spiking addition & subtraction."""
     # Fire
     thres_mode = np.where(
         vjt >= 1,
         TM.EXCEED_POSITIVE,
         np.where(vjt < 0, TM.EXCEED_NEGATIVE, TM.NOT_EXCEEDED),
     )
     spike = np.equal(thres_mode, TM.EXCEED_POSITIVE)
     # Reset
     v_reset = np.where(thres_mode == TM.EXCEED_POSITIVE, vjt - 1, vjt)
 
     return spike, v_reset
 
 
+def _spike_func_avg_pool(
+    vjt: VoltageType, pos_thres: int
+) -> tuple[SpikeType, VoltageType]:
+    """Function `spike_func()` in spiking addition & subtraction."""
+    # Fire
+    thres_mode = np.where(
+        vjt >= pos_thres,
+        TM.EXCEED_POSITIVE,
+        np.where(vjt < 0, TM.EXCEED_NEGATIVE, TM.NOT_EXCEEDED),
+    )
+    spike = np.equal(thres_mode, TM.EXCEED_POSITIVE)
+    # Reset
+    v_reset = np.where(thres_mode == TM.EXCEED_POSITIVE, 0, vjt)
+
+    return spike, v_reset
+
+
 def _sum_inputs_sadd_ssub(
     x1: SpikeType,
     x2: SpikeType,
     vjt_pre: VoltageType,
     add_or_sub: Literal[1, -1],
     strict: bool,
 ) -> VoltageType:
     """Function `sum_input()` for spiking addition & subtraction."""
-    # Charge
     incoming_v = (vjt_pre + x1 * 1 + x2 * add_or_sub).astype(np.int32)
-
-    # NOTE: In most cases, membrane potential overflow won't occur, otherwise the result is incorrect.
-    if _is_vjt_overflow(incoming_v):
-        if strict:
-            raise FunctionalError(VJT_OVERFLOW_ERROR_TEXT)
-        else:
-            warnings.warn(VJT_OVERFLOW_ERROR_TEXT, PAIBoxWarning)
-
-    return incoming_v
+    return vjt_overflow(incoming_v, strict)
 
 
-def _shape_check(shape: Tuple[int, ...], ndim: int) -> Tuple[int, ...]:
+def _shape_check(shape: tuple[int, ...], ndim: int) -> tuple[int, ...]:
     if len(shape) > ndim:
         raise ShapeError(
             f"expected shape to have dimensions <= {ndim}, but got {len(shape)}."
         )
 
     return as_shape(shape, min_dim=ndim)
 
 
 _shape_ndim2_check = partial(_shape_check, ndim=2)
 _shape_ndim3_check = partial(_shape_check, ndim=3)
 
 
-def _transpose2d_mapping(op_shape: Tuple[int, ...]) -> NDArray[np.bool_]:
+def _transpose2d_mapping(op_shape: tuple[int, ...]) -> NDArray[np.bool_]:
     """Get the mapping matrix for transpose of 2d array.
 
     Argument:
         - op_shape: the shape of matrix to be transposed, flattened in (X,Y) order.
 
     Return: transposed index matrix with shape (X*Y, Y*X).
     """
@@ -929,15 +1072,15 @@
     for idx in np.ndindex(op_shape):
         mt[idx[0] * op_shape[1] + idx[1], idx[1] * op_shape[0] + idx[0]] = 1
 
     return mt
 
 
 def _transpose3d_mapping(
-    op_shape: Tuple[int, ...], axes: Tuple[int, ...]
+    op_shape: tuple[int, ...], axes: tuple[int, ...]
 ) -> NDArray[np.bool_]:
     """Get the mapping matrix for transpose of 3d array.
 
     Argument:
         - op_shape: the shape of matrix to be transposed, flattened in (X,Y,Z) order.
         - axes: If specified, it must be a tuple or list which contains a permutation of [0, 1, …, N-1]     \
             where N is the number of axes of a.
```

### Comparing `paibox-1.1.0a2/paibox/components/modules.py` & `paibox-1.1.0a3/paibox/components/modules.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 import sys
 import typing
 from collections import deque
+from collections.abc import Sequence
 from dataclasses import dataclass, field
-from typing import ClassVar, List, Optional, Sequence, Tuple, Union
+from typing import ClassVar, Optional, Union
 
 import numpy as np
 from paicorelib import TM, HwConfig
 
-from paibox.base import NeuDyn, SynSys
+from paibox.base import NeuDyn
 from paibox.exceptions import NotSupportedError, RegisterError, ShapeError
 from paibox.types import SpikeType, VoltageType
 from paibox.utils import check_elem_unique, shape2num
 
 from .projection import InputProj
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
 if typing.TYPE_CHECKING:
     from paibox.network import DynSysGroup
 
+    from .synapses import FullConnectedSyn
+
 __all__ = ["BuildingModule"]
 
-MultiInputsType: TypeAlias = List[SpikeType]  # Type of inputs of `NeuModule`.
-BuiltComponentType: TypeAlias = List[Union[SynSys, NeuDyn]]
+MultiInputsType: TypeAlias = list[SpikeType]  # Type of inputs of `NeuModule`.
+BuiltComponentType: TypeAlias = list[Union["FullConnectedSyn", NeuDyn]]
 
 
 @dataclass
 class ModuleIntf:
     """Module interface. The interface of the module stores the information about where the module  \
         gets input and where it outputs. This information will be used when building the module.
     """
 
-    operands: List[Union[NeuDyn, InputProj]] = field(default_factory=list)
+    operands: list[Union[NeuDyn, InputProj]] = field(default_factory=list)
     """TODO can operands be a `NeuModule`?"""
-    output: List[SynSys] = field(default_factory=list)
+    output: list["FullConnectedSyn"] = field(default_factory=list)
     """A list of synapses."""
 
     @property
     def num_in(self) -> int:
         return sum(op.num_out for op in self.operands)
 
     @property
@@ -59,19 +62,19 @@
         """Register operands to the interface."""
         self.module_intf.operands.extend(op)
 
     def unregister_operand(self, op: Union[NeuDyn, InputProj]) -> None:
         """Remove a operand from the interface."""
         self.module_intf.operands.remove(op)
 
-    def register_output(self, syn: SynSys) -> None:
+    def register_output(self, syn: "FullConnectedSyn") -> None:
         """Register the output synapses."""
         self.module_intf.output.append(syn)
 
-    def unregister_output(self, syn: SynSys) -> None:
+    def unregister_output(self, syn: "FullConnectedSyn") -> None:
         """Remove an output synapses."""
         self.module_intf.output.remove(syn)
 
     @property
     def n_op(self) -> int:
         return len(self.module_intf.operands)
 
@@ -113,16 +116,19 @@
         """Function used to describe getting inputs of the module."""
         raise NotImplementedError
 
     def spike_func(self, *args, **kwargs):
         """Function used to describe generating output spike of the module."""
         raise NotImplementedError
 
+    def is_outputing(self) -> bool:
+        return (self.timestamp - self.inherent_delay) >= 0
+
     @property
-    def source(self) -> List[Union[NeuDyn, InputProj]]:
+    def source(self) -> list[Union[NeuDyn, InputProj]]:
         return self.module_intf.operands
 
     @property
     def dest(self):
         return self  # will be deprecated at anytime in the future.
 
     @property
@@ -139,15 +145,15 @@
     """Basic functional module. Only used in SNN mode."""
 
     n_return = 1
 
     def __init__(
         self,
         *operands: Union[NeuDyn, InputProj],
-        shape_out: Tuple[int, ...],
+        shape_out: tuple[int, ...],
         keep_shape: bool,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
         kwargs.setdefault("delay", 1)
         kwargs.setdefault("tick_wait_start", 1)
         kwargs.setdefault("tick_wait_end", 0)
@@ -192,15 +198,15 @@
         else:
             _init_synin = []
 
         self.set_memory(
             "synin_deque", deque(_init_synin, maxlen=1 + self.inherent_delay)
         )
 
-    def get_inputs(self) -> MultiInputsType:
+    def get_inputs(self) -> None:
         synin = []
 
         for op in self.module_intf.operands:
             # Retrieve the spike at index `timestamp` of the dest neurons
             if self.is_working():
                 if isinstance(op, InputProj):
                     synin.append(op.output.copy())
@@ -209,36 +215,38 @@
                     synin.append(op.output[idx].copy())
             else:
                 # Retrieve 0 to the dest neurons if it is not working
                 synin.append(np.zeros_like(op.spike))
 
         self.synin_deque.append(synin)  # Append to the right of the deque.
 
-        return self.synin_deque.popleft()  # Pop the left of the deque.
-
     def update(self, *args, **kwargs) -> Optional[SpikeType]:
         if not self.is_working():
             self._inner_spike = np.zeros((self.num_out,), dtype=np.bool_)
             return None
 
-        synin = self.get_inputs()
-        self._inner_spike = self.spike_func(*synin).ravel()
+        self.get_inputs()
 
-        idx = (self.timestamp + self.delay_relative - 1) % HwConfig.N_TIMESLOT_MAX
-        self.delay_registers[idx] = self._inner_spike.copy()
+        if self.is_outputing():
+            synin = self.synin_deque.popleft()  # Pop the left of the deque.
+            self._inner_spike = self.spike_func(*synin).ravel()
+            idx = (
+                self.timestamp - self.inherent_delay + self.delay_relative - 1
+            ) % HwConfig.N_TIMESLOT_MAX
+            self.delay_registers[idx] = self._inner_spike.copy()
 
         return self._inner_spike
 
     @property
     def shape_in(self):
         # TODO Return a tuple (shape_in_of_op1, shape_in_of_op2, ...)?
         raise NotImplementedError
 
     @property
-    def shape_out(self) -> Tuple[int, ...]:
+    def shape_out(self) -> tuple[int, ...]:
         return self._shape_out
 
     @property
     def num_in(self) -> int:
         return self.module_intf.num_in
 
     @property
@@ -253,14 +261,18 @@
     def spike(self) -> SpikeType:
         return self._inner_spike
 
     @property
     def feature_map(self) -> SpikeType:
         return self._inner_spike.reshape(self.varshape)
 
+    @property
+    def varshape(self) -> tuple[int, ...]:
+        return self.shape_out if self.keep_shape else (self.num_out,)
+
 
 class FunctionalModule2to1(FunctionalModule):
     """Functional module with two operands."""
 
     def __init__(
         self,
         neuron_a: Union[NeuDyn, InputProj],
@@ -270,47 +282,35 @@
         **kwargs,
     ) -> None:
         if neuron_a.num_out != neuron_b.num_out:
             raise ShapeError(
                 f"two operands must have the same size: {neuron_a.num_out} != {neuron_b.num_out}."
             )
 
-        if keep_shape:
-            if neuron_a.shape_out != neuron_b.shape_out:
-                raise ShapeError(
-                    f"two operands must have the same shape: {neuron_a.shape_out} != {neuron_b.shape_out}.\n"
-                    f"When two operands have different shapes, set 'keep_shape=False' and the output will "
-                    f"not retain shape information."
-                )
-
-            _shape_out = neuron_a.shape_out
-        else:
-            _shape_out = (neuron_a.num_out,)
-
         super().__init__(
             neuron_a,
             neuron_b,
-            shape_out=_shape_out,
+            shape_out=_shape_check2(neuron_a, neuron_b, keep_shape),
             keep_shape=keep_shape,
             name=name,
             **kwargs,
         )
 
     @property
-    def varshape(self) -> Tuple[int, ...]:
+    def varshape(self) -> tuple[int, ...]:
         return self.shape_out if self.keep_shape else (self.num_out,)
 
 
 class TransposeModule(FunctionalModule):
     inherent_delay = 0
 
     def __init__(
         self,
         neuron: Union[NeuDyn, InputProj],
-        shape_in: Tuple[int, ...],
+        shape_in: tuple[int, ...],
         axes: Optional[Sequence[int]] = None,
         keep_shape: bool = True,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
         if axes is None:
             axes = range(len(shape_in))[::-1]
@@ -331,53 +331,98 @@
         self._shape_in = shape_in
         self.axes = axes
         super().__init__(
             neuron, shape_out=shape_out, keep_shape=keep_shape, name=name, **kwargs
         )
 
     @property
-    def shape_in(self) -> Tuple[int, ...]:
+    def shape_in(self) -> tuple[int, ...]:
         return self._shape_in
 
 
-class FunctionalModule2to1WithV(FunctionalModule2to1):
+class FunctionalModuleWithV(FunctionalModule):
     """Functional module with two operands.
 
-    NOTE: Compared to `FunctionalModule2to1`, The difference is that we also take the \
-        membrane potential voltage(vjt) into consideration.
+    NOTE: Compared to `FunctionalModule`, the difference is that it takes the \
+        membrane potential voltage into consideration.
     """
 
     def __init__(
         self,
-        neuron_a: Union[NeuDyn, InputProj],
-        neuron_b: Union[NeuDyn, InputProj],
+        *operands: Union[NeuDyn, InputProj],
+        shape_out: tuple[int, ...],
         keep_shape: bool = False,
         name: Optional[str] = None,
         **kwargs,
     ) -> None:
-        super().__init__(neuron_a, neuron_b, keep_shape, name, **kwargs)
-
+        super().__init__(
+            *operands, shape_out=shape_out, keep_shape=keep_shape, name=name, **kwargs
+        )
         self.set_memory("_vjt", np.zeros((self.num_out,), dtype=np.int32))
         self.thres_mode = np.full((self.num_out,), TM.NOT_EXCEEDED, dtype=np.uint8)
 
     def synaptic_integr(self, *args, **kwargs) -> VoltageType:
         """Functions used to describe synaptic integration of the module."""
         raise NotImplementedError
 
     def update(self, *args, **kwargs) -> Optional[SpikeType]:
         if not self.is_working():
             self._inner_spike = np.zeros((self.num_out,), dtype=np.bool_)
             return None
 
-        synin = self.get_inputs()
-        incoming_v = self.synaptic_integr(*synin, self._vjt)
-        _is, self._vjt = self.spike_func(incoming_v)
-        self._inner_spike = _is.ravel()
+        self.get_inputs()
 
-        idx = (self.timestamp + self.delay_relative - 1) % HwConfig.N_TIMESLOT_MAX
-        self.delay_registers[idx] = self._inner_spike.copy()
+        if self.is_outputing():
+            synin = self.synin_deque.popleft()  # Pop the left of the deque.
+            incoming_v = self.synaptic_integr(*synin, self._vjt)
+            _is, self._vjt = self.spike_func(incoming_v)
+            self._inner_spike = _is.ravel()
+
+            idx = (
+                self.timestamp - self.inherent_delay + self.delay_relative - 1
+            ) % HwConfig.N_TIMESLOT_MAX
+            self.delay_registers[idx] = self._inner_spike.copy()
 
         return self._inner_spike
 
     @property
     def voltage(self) -> VoltageType:
         return self._vjt.reshape(self.varshape)
+
+
+class FunctionalModule2to1WithV(FunctionalModuleWithV):
+    def __init__(
+        self,
+        neuron_a: Union[NeuDyn, InputProj],
+        neuron_b: Union[NeuDyn, InputProj],
+        keep_shape: bool = False,
+        name: Optional[str] = None,
+        **kwargs,
+    ) -> None:
+        super().__init__(
+            neuron_a,
+            neuron_b,
+            shape_out=_shape_check2(neuron_a, neuron_b, keep_shape),
+            keep_shape=keep_shape,
+            name=name,
+            **kwargs,
+        )
+
+
+def _shape_check2(
+    neuron_a: Union[NeuDyn, InputProj],
+    neuron_b: Union[NeuDyn, InputProj],
+    keep_shape: bool,
+) -> tuple[int, ...]:
+    if keep_shape:
+        if neuron_a.shape_out != neuron_b.shape_out:
+            raise ShapeError(
+                f"two operands must have the same shape: {neuron_a.shape_out} != {neuron_b.shape_out}. "
+                f"When two operands have different shapes, set 'keep_shape=False' and the output will "
+                f"not retain shape information."
+            )
+
+        shape_out = neuron_a.shape_out
+    else:
+        shape_out = (neuron_a.num_out,)
+
+    return shape_out
```

### Comparing `paibox-1.1.0a2/paibox/components/neuron/base.py` & `paibox-1.1.0a3/paibox/components/neuron/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional, Tuple
+from typing import Any, Optional
 
 import numpy as np
 from numpy.typing import NDArray
 from paicorelib import (
     LCM,
     LDM,
     LIM,
@@ -13,17 +13,23 @@
     HwConfig,
     MaxPoolingEnable,
     SpikeWidthFormat,
 )
 
 from paibox.base import NeuDyn
 from paibox.types import Shape, SpikeType, VoltageType
-from paibox.utils import as_shape, shape2num
+from paibox.utils import (
+    arg_check_non_neg,
+    arg_check_non_pos,
+    arg_check_pos,
+    as_shape,
+    shape2num,
+)
 
-from .utils import _vjt_overflow
+from .utils import NEG_THRES_MIN, vjt_overflow
 
 __all__ = ["Neuron"]
 
 
 class MetaNeuron:
     """Meta neuron"""
 
@@ -38,14 +44,15 @@
         neg_threshold: int,
         pos_threshold: int,
         leak_direction: LDM,
         leak_integration_mode: LIM,
         leak_v: int,
         synaptic_integration_mode: SIM,
         bit_truncation: int,
+        overflow_strict: bool,
         keep_shape: bool = False,
     ) -> None:
         """Stateless attributes. Scalar."""
         # Basic attributes.
         self.keep_shape = keep_shape
         self._shape = as_shape(shape)
         self._n_neuron = shape2num(self._shape)
@@ -69,17 +76,18 @@
         self._spike_width_format: SpikeWidthFormat
         self._pool_max_en: MaxPoolingEnable
 
         # Auxiliary attributes or variables.
         self._thres_mask: int = (1 << threshold_mask_bits) - 1
         self.thres_mode = self.init_param(TM.NOT_EXCEEDED).astype(np.uint8)
         self._v_th_rand = self.init_param(0).astype(np.int32)
+        self.overflow_strict = overflow_strict
 
     def _neuronal_charge(
-        self, incoming_v: VoltageType, vjt_pre: VoltageType
+        self, incoming_v: VoltageType, vjt_pre: VoltageType, strict: bool = False
     ) -> VoltageType:
         r"""1. Synaptic integration.
 
         Description:
             _rho_w_ij: Random synaptic integration enable, 0 or 1.
 
             If synaptic integration mode is deterministic, then
@@ -91,21 +99,21 @@
 
         if self.synaptic_integration_mode is SIM.MODE_STOCHASTIC:
             raise NotImplementedError(
                 f"mode {SIM.MODE_STOCHASTIC.name} is not implemented."
             )
         else:
             if incoming_v.ndim == 2:
-                _v = incoming_v.sum(axis=1).astype(np.int32)
+                _v = incoming_v.sum(axis=1, dtype=np.int32)
             else:
                 _v = incoming_v
 
-        v_charged = np.add(vjt_pre, _v).astype(np.int32)
+        v_charged = np.add(vjt_pre, _v, dtype=np.int32)
 
-        return _vjt_overflow(v_charged)  # Handle with overflow here
+        return vjt_overflow(v_charged, strict)  # Handle with overflow here
 
     def _neuronal_leak(self, vjt: VoltageType) -> VoltageType:
         r"""2. Leak integration.
 
         2.1 Leak direction, forward or reversal.
             If leak direction is `MODE_FORWARD`, the `_ld` is 1, else is \sgn{`vjt`}.
 
@@ -124,15 +132,15 @@
 
         if self.leak_direction is LDM.MODE_FORWARD:
             _ld = np.ones((self._n_neuron,), dtype=np.bool_)
         else:
             _ld = np.sign(vjt)
 
         if self.leak_integration_mode is LIM.MODE_DETERMINISTIC:
-            v_leaked = np.add(vjt, _ld * self.leak_v).astype(np.int32)
+            v_leaked = np.add(vjt, _ld * self.leak_v, dtype=np.int32)
         else:
             raise NotImplementedError(
                 f"mode {LIM.MODE_STOCHASTIC.name} is not implemented."
             )
             # _F = 1 if abs(self.leak_v) >= _rho_j_lambda else 0
             # sgn_leak_v = fn_sgn(self.leak_v, 0)
             # self.vjt = np.add(self.vjt, sgn_leak_v * _F * _ld).astype(np.int32)
@@ -313,18 +321,18 @@
     def _aux_post_hook(self) -> None:
         """Post-hook after the entire activation."""
         # Reset the auxiliary threshold mode.
         self.thres_mode = self.init_param(TM.NOT_EXCEEDED).astype(np.uint8)
 
     def update(
         self, incoming_v: VoltageType, vjt_pre: VoltageType
-    ) -> Tuple[SpikeType, VoltageType, NDArray[np.uint8]]:
+    ) -> tuple[SpikeType, VoltageType, NDArray[np.uint8]]:
         """Update at one time step."""
         # 1. Charge
-        v_charged = self._neuronal_charge(incoming_v, vjt_pre)
+        v_charged = self._neuronal_charge(incoming_v, vjt_pre, self.overflow_strict)
 
         # 2. Leak & fire
         if self.leak_comparison is LCM.LEAK_BEFORE_COMP:
             v_leaked = self._neuronal_leak(v_charged)
             spike = self._neuronal_fire(v_leaked)
         else:
             spike = self._neuronal_fire(v_charged)
@@ -338,106 +346,78 @@
 
         return spike, v_reset, _debug_thres_mode
 
     def init_param(self, param: Any) -> np.ndarray:
         return np.full((self._n_neuron,), param)
 
     @property
-    def varshape(self) -> Tuple[int, ...]:
+    def varshape(self) -> tuple[int, ...]:
         return self._shape if self.keep_shape else (self._n_neuron,)
 
     @property
     def bias(self) -> int:
-        """Signed 30-bit. ANN mode only."""
         return self.leak_v
 
 
 class Neuron(MetaNeuron, NeuDyn):
     _excluded_vars = (
         "vjt",
         "vj",
         "y",
-        "threshold_mode",
+        "thres_mode",
         "spike",
-        "v_th_rand",
+        "_v_th_rand",
         "_spike_width_format",
         "_pool_max_en",
         "master_nodes",
     )
 
+    _n_copied = 0
+    """Counter of copies."""
+
     def __init__(
         self,
         shape: Shape,
         reset_mode: RM = RM.MODE_NORMAL,
         reset_v: int = 0,
-        leak_comparison: LCM = LCM.LEAK_AFTER_COMP,
+        leak_comparison: LCM = LCM.LEAK_BEFORE_COMP,
         threshold_mask_bits: int = 0,
         neg_thres_mode: NTM = NTM.MODE_RESET,
-        neg_threshold: int = 0,
+        neg_threshold: int = NEG_THRES_MIN,
         pos_threshold: int = 1,
         leak_direction: LDM = LDM.MODE_FORWARD,
         leak_integration_mode: LIM = LIM.MODE_DETERMINISTIC,
         leak_v: int = 0,
         synaptic_integration_mode: SIM = SIM.MODE_DETERMINISTIC,
         bit_truncation: int = 0,
         *,
         delay: int = 1,
         tick_wait_start: int = 1,
         tick_wait_end: int = 0,
         unrolling_factor: int = 1,
+        overflow_strict: bool = False,
         keep_shape: bool = False,
         name: Optional[str] = None,
     ) -> None:
-        if neg_threshold > 0:
-            raise ValueError(
-                f"negative threshold must be non-positive, but got {neg_threshold}."
-            )
-
-        if pos_threshold < 0:
-            raise ValueError(
-                f"positive threshold must be non-negative, but got {pos_threshold}."
-            )
-
-        if bit_truncation < 0:
-            raise ValueError(
-                f"bit of tuncation must be non-negative, but got {bit_truncation}."
-            )
-
-        if delay < 1:
-            raise ValueError(f"'delay' must be positive, but got {delay}.")
-
-        if tick_wait_start < 0:
-            raise ValueError(
-                f"'tick_wait_start' must be non-negative, but got {tick_wait_start}."
-            )
-
-        if tick_wait_end < 0:
-            raise ValueError(
-                f"'tick_wait_end' must be non-negative, but got {tick_wait_end}."
-            )
-
-        if unrolling_factor < 1:
-            raise ValueError(
-                f"'unrolling_factor' must be positive, but got {unrolling_factor}."
-            )
-
         super().__init__(
             shape,
             reset_mode,
             reset_v,
             leak_comparison,
             threshold_mask_bits,
             neg_thres_mode,
-            (-neg_threshold),  # In `MetaNeuron`, it is unsgined.
-            pos_threshold,
+            # In `MetaNeuron`, it is unsigned.
+            (-arg_check_non_pos(neg_threshold, "negative threshold")),
+            arg_check_non_neg(pos_threshold, "positive threshold"),
             leak_direction,
             leak_integration_mode,
             leak_v,
             synaptic_integration_mode,
-            bit_truncation,
+            arg_check_non_neg(bit_truncation, "bit of tuncation"),
+            overflow_strict,
             keep_shape,
         )
         super(MetaNeuron, self).__init__(name)
 
         """Stateful attributes. Vector."""
         # Initial vjt is fixed at 0.
         self.set_memory("_vjt", self.init_param(0).astype(np.int32))
@@ -456,21 +436,18 @@
         self.set_memory(
             "delay_registers",
             np.zeros(
                 (HwConfig.N_TIMESLOT_MAX,) + self._inner_spike.shape, dtype=np.bool_
             ),
         )
 
-        self._delay = delay
-        self._tws = tick_wait_start
-        self._twe = tick_wait_end
-        self._uf = unrolling_factor
-
-        """Counter of copies."""
-        self._n_copied = 0
+        self._delay = arg_check_pos(delay, "'delay'")
+        self._tws = arg_check_non_neg(tick_wait_start, "'tick_wait_start'")
+        self._twe = arg_check_non_neg(tick_wait_end, "'tick_wait_end'")
+        self._uf = arg_check_pos(unrolling_factor, "'unrolling_factor'")
 
     def __len__(self) -> int:
         return self._n_neuron
 
     def __call__(
         self, x: Optional[np.ndarray] = None, *args, **kwargs
     ) -> Optional[SpikeType]:
@@ -517,15 +494,15 @@
         return Neuron(
             self._shape,
             self.reset_mode,
             self.reset_v,
             self.leak_comparison,
             self.threshold_mask_bits,
             self.neg_thres_mode,
-            self.neg_threshold,
+            (-1) * self.neg_threshold,
             self.pos_threshold,
             self.leak_direction,
             self.leak_integration_mode,
             self.leak_v,
             self.synaptic_integration_mode,
             self.bit_truncation,
             delay=self.delay_relative,
@@ -536,19 +513,19 @@
             name=f"{self.name}_copied_{self._n_copied}",
         )
 
     def copy(self) -> "Neuron":
         return self.__deepcopy__()
 
     @property
-    def shape_in(self) -> Tuple[int, ...]:
+    def shape_in(self) -> tuple[int, ...]:
         return self._shape
 
     @property
-    def shape_out(self) -> Tuple[int, ...]:
+    def shape_out(self) -> tuple[int, ...]:
         return self._shape
 
     @property
     def num_in(self) -> int:
         return self._n_neuron
 
     @property
```

### Comparing `paibox-1.1.0a2/paibox/components/projection.py` & `paibox-1.1.0a3/paibox/components/projection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
 import sys
-from typing import Callable, Optional, Tuple, Union
+from collections.abc import Callable
+from typing import Optional, Union
 
 import numpy as np
 
 if sys.version_info >= (3, 10):
     from typing import ParamSpec
 else:
     from typing_extensions import ParamSpec
@@ -65,21 +66,31 @@
 
         self.set_memory("_inner_spike", np.zeros((self.num_out,), dtype=np.bool_))
 
     def update(self, **kwargs) -> SpikeType:
         _spike = self._get_neumeric_input(**kwargs)
 
         if isinstance(_spike, (int, np.bool_, np.integer)):
-            self._inner_spike = np.full((self.num_out,), _spike, dtype=np.bool_)
+            # XXX In order to simplify the situation where one neuron is connected to
+            # multiple axons in the simulation (the actual input node output size is 8),
+            # one input node is temporarily allowed to output 8 bits of data.
+            if isinstance(_spike, (np.bool_, np.integer)):
+                _dtype = _spike.dtype
+            else:
+                _dtype = np.int8
+
+            self._inner_spike = np.full((self.num_out,), _spike, dtype=_dtype)
+
         elif isinstance(_spike, np.ndarray):
             if shape2num(_spike.shape) != self.num_out:
                 raise ShapeError(
                     f"cannot reshape output value from {_spike.shape} to ({self.num_out},)."
                 )
-            self._inner_spike = _spike.ravel().astype(np.bool_)
+            self._inner_spike = _spike.ravel()
+
         else:
             # should never be reached
             raise TypeError(
                 f"expected type int, np.bool_, np.integer or np.ndarray, "
                 f"but got {_spike}, type {type(_spike)}."
             )
 
@@ -99,31 +110,31 @@
 
         elif self._func_input is None:
             return self._num_input
         else:
             return _call_with_ctx(self._func_input, self._num_input, **kwargs)
 
     @property
-    def varshape(self) -> Tuple[int, ...]:
+    def varshape(self) -> tuple[int, ...]:
         return self.shape_out if self.keep_shape else (self.num_out,)
 
     @property
     def num_in(self) -> int:
         return 0
 
     @property
     def num_out(self) -> int:
         return shape2num(self._shape)
 
     @property
-    def shape_in(self) -> Tuple[int, ...]:
+    def shape_in(self) -> tuple[int, ...]:
         return (0,)
 
     @property
-    def shape_out(self) -> Tuple[int, ...]:
+    def shape_out(self) -> tuple[int, ...]:
         return self._shape
 
     @property
     def input(self):
         return self._get_neumeric_input()
 
     @input.setter
```

### Comparing `paibox-1.1.0a2/paibox/components/synapses/base.py` & `paibox-1.1.0a3/paibox/components/synapses/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import ClassVar, Optional, Tuple, Union
+from typing import ClassVar, Optional, Union
 
 import numpy as np
 from paicorelib import HwConfig
 from paicorelib import WeightPrecision as WP
 
 from paibox.base import NeuDyn, SynSys
 from paibox.exceptions import RegisterError, ShapeError
@@ -11,151 +11,174 @@
 from ..modules import BuildingModule
 from ..neuron import Neuron
 from ..projection import InputProj
 from .conv_types import _KOrder3d, _KOrder4d
 from .conv_utils import _fm_ndim1_check, _fm_ndim2_check
 from .transforms import (
     AllToAll,
+    ConnType,
     Conv1dForward,
     Conv2dForward,
     ConvTranspose1dForward,
     ConvTranspose2dForward,
+    Identity,
+    MaskedLinear,
+    OneToOne,
+    Transform,
 )
-from .transforms import GeneralConnType as GConnType
-from .transforms import Identity, MaskedLinear, OneToOne, Transform
 
 RIGISTER_MASTER_KEY_FORMAT = "{0}.output"
 
 
 def _check_equal(num_in: int, num_out: int) -> int:
     if num_in != num_out:
         raise ShapeError(
             f"the number of source & destination neurons must be equal: {num_in} != {num_out}."
         )
 
     return num_in
 
 
-class Synapses:
+class FullConnectedSyn(SynSys):
+    comm: Transform
+    _n_copied: int = 0
+    """Counter of copies."""
+
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
-        dest: NeuDyn,
-        subclass_syn_name: str,
+        target: NeuDyn,
+        name: Optional[str] = None,
     ) -> None:
+        super().__init__(name)
+
         self._source = source
-        self._target = dest
-        self._child_syn_name = subclass_syn_name
-        """The name of subclass `FullConnectedSyn`."""
+        self._target = target
+
+        self.set_memory("_synout", np.zeros((self.num_out,), dtype=np.int32))
+
+        # Register itself with the master nodes of target.
+        target.register_master(RIGISTER_MASTER_KEY_FORMAT.format(self.name), self)
+
+        # If the source is `BuildingModule`, register itself with its module interface.
+        if isinstance(source, BuildingModule):
+            source.register_output(self)
+
+    def __call__(self, *args, **kwargs) -> SynOutType:
+        return self.update(*args, **kwargs)
+
+    def update(self, spike: Optional[np.ndarray] = None, *args, **kwargs) -> SynOutType:
+        # Retrieve the spike at index `timestamp` of the dest neurons
+        if self.dest.is_working():
+            if isinstance(self.source, InputProj):
+                synin = self.source.output.copy() if spike is None else spike
+            else:
+                idx = self.dest.timestamp % HwConfig.N_TIMESLOT_MAX
+                synin = self.source.output[idx].copy() if spike is None else spike
+        else:
+            # Retrieve 0 to the dest neurons if it is not working
+            synin = np.zeros_like(self.source.spike)
+
+        self._synout = self.comm(synin).ravel().astype(np.int32)
+        return self._synout
+
+    def reset_state(self, *args, **kwargs) -> None:
+        # TODO Add other initialization methods in the future.
+        self.reset_memory()  # Call reset of `StatusMemory`.
+
+    def __copy__(self) -> "FullConnSyn":
+        return self.__deepcopy__()
+
+    def __deepcopy__(self, memo=None, _nil=[]) -> "FullConnSyn":
+        self._n_copied += 1
+
+        return FullConnSyn(
+            self.source,
+            self.dest,
+            self.connectivity,
+            ConnType.All2All,
+            f"{self.name}_copied_{self._n_copied}",
+        )
+
+    def copy(
+        self,
+        source: Optional[Union[NeuDyn, InputProj]] = None,
+        target: Optional[NeuDyn] = None,
+    ) -> "FullConnSyn":
+        copied = self.__copy__()
+        if isinstance(source, (NeuDyn, InputProj)):
+            copied.source = source
+
+        if isinstance(target, NeuDyn):
+            copied.target = target
+
+        return copied
 
     @property
     def source(self) -> Union[NeuDyn, InputProj]:
         return self._source
 
     @source.setter
     def source(self, source: Union[NeuDyn, InputProj]) -> None:
         """Set a new source neuron."""
         if source.num_out != self.num_in:
             raise RegisterError(
-                f"the number of source neurons before and after the change"
-                f"is not equal: {source.num_out} != {self.num_in}."
+                f"the number of source neurons before and after the change "
+                f"is not equal, {source.num_out} != {self.num_in}."
             )
 
         self._source = source
 
     @property
-    def dest(self) -> NeuDyn:
+    def target(self) -> NeuDyn:
         return self._target
 
-    @dest.setter
-    def dest(self, dest: NeuDyn) -> None:
-        """Set a new destination neuron."""
-        if dest.num_in != self.num_out:
+    @target.setter
+    def target(self, target: NeuDyn) -> None:
+        """Set a new target neuron."""
+        if target.num_in != self.num_out:
             raise RegisterError(
-                f"the number of source neurons before and after the change"
-                f"is not equal: {dest.num_in} != {self.num_out}."
+                f"the number of source neurons before and after the change "
+                f"is not equal, {target.num_in} != {self.num_out}."
             )
 
-        self._target = dest
-        # FIXME Because the modification of the synapse destination neuron occurs in the backend,
-        # there's no need to register new dest again because simulation will not be done again (maybe).
-        # But does it mean that we need to make a copy of the original network and then pass it to
-        # the backend?
-        dest.register_master(
-            RIGISTER_MASTER_KEY_FORMAT.format(self._child_syn_name), self
+        self._target.unregister_master(self.name)
+
+        self._target = target
+        # Allow the same target to register again.
+        target.register_master(
+            RIGISTER_MASTER_KEY_FORMAT.format(self.name), self, strict=False
         )
 
     @property
-    def target(self) -> NeuDyn:
+    def dest(self) -> NeuDyn:
+        # TODO To maintain compatibility, the dest attribute is preserved.
+        # Will be removed in a future version.
         return self._target
 
+    @dest.setter
+    def dest(self, target: NeuDyn) -> None:
+        self.target = target
+
     @property
-    def shape_in(self) -> Tuple[int, ...]:
+    def shape_in(self) -> tuple[int, ...]:
         return self._source.shape_out
 
     @property
-    def shape_out(self) -> Tuple[int, ...]:
+    def shape_out(self) -> tuple[int, ...]:
         return self._target.shape_in
 
     @property
     def num_in(self) -> int:
         return self._source.num_out
 
     @property
     def num_out(self) -> int:
         return self._target.num_in
 
-
-class FullConnectedSyn(Synapses, SynSys):
-
-    comm: Transform
-
-    def __init__(
-        self,
-        source: Union[NeuDyn, InputProj],
-        dest: NeuDyn,
-        name: Optional[str] = None,
-    ) -> None:
-        super(Synapses, self).__init__(name)
-        super().__init__(source, dest, self.name)
-
-        self.set_memory("_synout", np.zeros((self.num_out,), dtype=np.int32))
-
-        # Register itself with the master nodes of destination.
-        dest.register_master(RIGISTER_MASTER_KEY_FORMAT.format(self.name), self)
-
-        # If the source is `BuildingModule`, register itself with its module interface.
-        if isinstance(source, BuildingModule):
-            source.register_output(self)
-
-    def __call__(self, *args, **kwargs) -> SynOutType:
-        return self.update(*args, **kwargs)
-
-    def update(self, spike: Optional[np.ndarray] = None, *args, **kwargs) -> SynOutType:
-        # Retrieve the spike at index `timestamp` of the dest neurons
-        if self.dest.is_working():
-            if isinstance(self.source, InputProj):
-                synin = self.source.output.copy() if spike is None else spike
-            else:
-                idx = self.dest.timestamp % HwConfig.N_TIMESLOT_MAX
-                synin = self.source.output[idx].copy() if spike is None else spike
-        else:
-            # Retrieve 0 to the dest neurons if it is not working
-            synin = np.zeros_like(self.source.spike)
-
-        self._synout = self.comm(synin).ravel().astype(np.int32)
-        return self._synout
-
-    def reset_state(self, *args, **kwargs) -> None:
-        # TODO Add other initialization methods in the future.
-        self.reset_memory()  # Call reset of `StatusMemory`.
-
-    def _set_comm(self, comm: Transform) -> None:
-        self.comm = comm
-
     @property
     def output(self) -> SynOutType:
         return self._synout
 
     @property
     def weights(self) -> WeightType:
         return self.comm.weights
@@ -170,52 +193,58 @@
         return self.comm.connectivity
 
 
 class FullConnSyn(FullConnectedSyn):
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
-        dest: NeuDyn,
+        target: NeuDyn,
         weights: DataArrayType,
-        conn_type: GConnType,
+        conn_type: ConnType,
         name: Optional[str] = None,
     ) -> None:
-        super().__init__(source, dest, name)
+        super().__init__(source, target, name)
 
-        if conn_type is GConnType.One2One:
+        if conn_type is ConnType.One2One:
             comm = OneToOne(_check_equal(self.num_in, self.num_out), weights)
-        elif conn_type is GConnType.Identity:
+        elif conn_type is ConnType.Identity:
             if not isinstance(weights, (int, np.bool_, np.integer)):
                 raise TypeError(
                     f"expected type int, np.bool_, np.integer, but got type {type(weights)}."
                 )
             comm = Identity(_check_equal(self.num_in, self.num_out), weights)
-        elif conn_type is GConnType.All2All:
+        elif conn_type is ConnType.All2All:
             comm = AllToAll((self.num_in, self.num_out), weights)
         else:  # MatConn
             if not isinstance(weights, np.ndarray):
                 raise TypeError(
                     f"expected type np.ndarray, but got type {type(weights)}."
                 )
-            comm = MaskedLinear((self.num_in, self.num_out), weights)
+            if len(self.shape_in) > 2:
+                raise ShapeError(
+                    f"Expect the shape of source to have no more than 2 dimensions, "
+                    f"but got {len(self.shape_in)}."
+                )
+
+            comm = MaskedLinear(self.shape_in, self.shape_out, weights)
 
-        self._set_comm(comm)
+        self.comm = comm
 
 
 class Conv1dSyn(FullConnectedSyn):
     _spatial_ndim: ClassVar[int] = 1
 
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: Neuron,
         kernel: np.ndarray,
-        stride: Tuple[int],
-        padding: Tuple[int],
-        dilation: Tuple[int],
+        stride: tuple[int],
+        padding: tuple[int],
+        dilation: tuple[int],
         order: _KOrder3d,
         name: Optional[str] = None,
     ) -> None:
         super().__init__(source, dest, name)
 
         if kernel.ndim != self._spatial_ndim + 2:
             raise ShapeError(
@@ -237,30 +266,28 @@
 
         if in_ch != in_channels:
             raise ShapeError(f"input channels mismatch: {in_ch} != {in_channels}.")
 
         if (_output_size := out_channels * out_l) != dest.num_in:
             raise ShapeError(f"Output size mismatch: {_output_size} != {dest.num_in}.")
 
-        comm = Conv1dForward((in_l,), (out_l,), _kernel, stride, padding)
-
-        self._set_comm(comm)
+        self.comm = Conv1dForward((in_l,), (out_l,), _kernel, stride, padding)
 
 
 class Conv2dSyn(FullConnectedSyn):
     _spatial_ndim: ClassVar[int] = 2
 
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: Neuron,
         kernel: np.ndarray,
-        stride: Tuple[int, int],
-        padding: Tuple[int, int],
-        dilation: Tuple[int, int],
+        stride: tuple[int, int],
+        padding: tuple[int, int],
+        dilation: tuple[int, int],
         order: _KOrder4d,
         name: Optional[str] = None,
     ) -> None:
         super().__init__(source, dest, name)
 
         if kernel.ndim != self._spatial_ndim + 2:
             raise ShapeError(
@@ -283,33 +310,36 @@
             1
         ] + 1
 
         if in_ch != in_channels:
             raise ShapeError(f"input channels mismatch: {in_ch} != {in_channels}.")
 
         if (_output_size := out_channels * out_h * out_w) != dest.num_in:
-            raise ShapeError(f"Output size mismatch: {_output_size} != {dest.num_in}.")
-
-        comm = Conv2dForward((in_h, in_w), (out_h, out_w), _kernel, stride, padding)
+            raise ShapeError(
+                f"Output size mismatch: {_output_size} ({out_channels}*{out_h}*{out_w}) "
+                f"!= {dest.num_in}."
+            )
 
-        self._set_comm(comm)
+        self.comm = Conv2dForward(
+            (in_h, in_w), (out_h, out_w), _kernel, stride, padding
+        )
 
 
 class ConvTranspose1dSyn(FullConnectedSyn):
     _spatial_ndim: ClassVar[int] = 1
 
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: Neuron,
         kernel: np.ndarray,
-        stride: Tuple[int],
-        padding: Tuple[int],
-        dilation: Tuple[int],
-        output_padding: Tuple[int],
+        stride: tuple[int],
+        padding: tuple[int],
+        dilation: tuple[int],
+        output_padding: tuple[int],
         order: _KOrder3d,
         name: Optional[str] = None,
     ) -> None:
         super().__init__(source, dest, name)
 
         if kernel.ndim != self._spatial_ndim + 2:
             raise ShapeError(
@@ -335,33 +365,31 @@
 
         if in_ch != in_channels:
             raise ShapeError(f"input channels mismatch: {in_ch} != {in_channels}.")
 
         if (_output_size := out_channels * out_l) != dest.num_in:
             raise ShapeError(f"Output size mismatch: {_output_size} != {dest.num_in}.")
 
-        comm = ConvTranspose1dForward(
+        self.comm = ConvTranspose1dForward(
             (in_l,), (out_l,), _kernel, stride, padding, output_padding
         )
 
-        self._set_comm(comm)
-
 
 class ConvTranspose2dSyn(FullConnectedSyn):
     _spatial_ndim: ClassVar[int] = 2
 
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: Neuron,
         kernel: np.ndarray,
-        stride: Tuple[int, int],
-        padding: Tuple[int, int],
-        dilation: Tuple[int, int],
-        output_padding: Tuple[int, int],
+        stride: tuple[int, int],
+        padding: tuple[int, int],
+        dilation: tuple[int, int],
+        output_padding: tuple[int, int],
         order: _KOrder4d,
         name: Optional[str] = None,
     ) -> None:
         super().__init__(source, dest, name)
 
         if kernel.ndim != self._spatial_ndim + 2:
             raise ShapeError(
@@ -394,12 +422,10 @@
 
         if in_ch != in_channels:
             raise ShapeError(f"input channels mismatch: {in_ch} != {in_channels}.")
 
         if (_output_size := out_channels * out_h * out_w) != dest.num_in:
             raise ShapeError(f"Output size mismatch: {_output_size} != {dest.num_in}.")
 
-        comm = ConvTranspose2dForward(
+        self.comm = ConvTranspose2dForward(
             (in_h, in_w), (out_h, out_w), _kernel, stride, padding, output_padding
         )
-
-        self._set_comm(comm)
```

### Comparing `paibox-1.1.0a2/paibox/components/synapses/conv_types.py` & `paibox-1.1.0a3/paibox/components/synapses/conv_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Literal, Tuple, TypeVar, Union
+from typing import Literal, TypeVar, Union
 
 T = TypeVar("T")
 
-_TupleAnyType = Union[T, Tuple[T, ...]]
-_Tuple1Type = Union[T, Tuple[T]]
-_Tuple2Type = Union[T, Tuple[T, T]]
-_Tuple3Type = Union[T, Tuple[T, T, T]]
+_TupleAnyType = Union[T, tuple[T, ...]]
+_Tuple1Type = Union[T, tuple[T]]
+_Tuple2Type = Union[T, tuple[T, T]]
+_Tuple3Type = Union[T, tuple[T, T, T]]
 
 _SizeAnyType = _TupleAnyType[int]
 _Size1Type = _Tuple1Type[int]
 _Size2Type = _Tuple2Type[int]
 _Size3Type = _Tuple3Type[int]
 
-SizeAnyType = Tuple[int, ...]
-Size1Type = Tuple[int]
-Size2Type = Tuple[int, int]
-Size3Type = Tuple[int, int, int]
+SizeAnyType = tuple[int, ...]
+Size1Type = tuple[int]
+Size2Type = tuple[int, int]
+Size3Type = tuple[int, int, int]
 
 _Order2d = Literal["CL", "LC"]  # Feature map order in 2d
 _Order3d = Literal["CHW", "HWC"]  # Feature map order in 3d
 _KOrder3d = Literal["OIL", "IOL"]  # Kernel order in 1d convolution
 _KOrder4d = Literal["OIHW", "IOHW"]  # Kernel order in 2d convolution
```

### Comparing `paibox-1.1.0a2/paibox/components/synapses/conv_utils.py` & `paibox-1.1.0a3/paibox/components/synapses/conv_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from collections.abc import Iterable
 from functools import partial
 from itertools import repeat
-from typing import Any, Iterable
+from typing import Any
 
 import numpy as np
 from numpy.typing import NDArray
 
 from paibox.exceptions import ShapeError
 from paibox.types import SpikeType, SynOutType, WeightType
 
@@ -155,14 +156,15 @@
                 w_unrolled_np[:, i * ow + j + o_ch * out_size] = t[o_ch].ravel()
 
     # Remove the part of the padding in the w_unrolled_no_padding
     # That is, remove useless weight in the w_unrolled_no_padding
     nih, niw = in_shape
     nin_size = nih * niw
     w_unrolled = np.zeros((cin * nin_size, cout * out_size), dtype=kernel.dtype)
+
     for i in range(cin):
         for j in range(nih):
             w_unrolled[i * nin_size + j * niw : i * nin_size + j * niw + niw, :] = (
                 w_unrolled_np[
                     i * in_size
                     + (padding[0] + j) * iw
                     + padding[1] : i * in_size
@@ -178,49 +180,69 @@
 
 def _pool2d_kernel_unroll(
     channels: int,
     in_shape: Size2Type,
     out_shape: Size2Type,
     ksize: Size2Type,
     stride: Size2Type,
-    # padding: Size2Type,
+    padding: Size2Type,
     # fm_order: str,
 ) -> WeightType:
     kh, kw = ksize
-    ih, iw = in_shape
+    ih = in_shape[0] + 2 * padding[0]
+    iw = in_shape[1] + 2 * padding[1]
     oh, ow = out_shape
     in_size = ih * iw
     out_size = oh * ow
 
-    w_unrolled = np.zeros((channels * in_size, channels * out_size), dtype=np.bool_)
+    w_unrolled_np = np.zeros((channels * in_size, channels * out_size), dtype=np.bool_)
 
     for i in range(oh):
         for j in range(ow):
             zeros_image = np.zeros((channels * ih, iw * channels), dtype=np.bool_)
             for i_ch in range(channels):
                 zeros_image[
                     (i * stride[0] + i_ch * ih) : (i * stride[0] + i_ch * ih) + kh,
                     (j * stride[1] + i_ch * iw) : (j * stride[1] + i_ch * iw) + kw,
                 ] = 1
 
             temp = zeros_image.reshape((channels * ih, channels, iw)).transpose(1, 0, 2)
 
             for o_ch in range(channels):
-                w_unrolled[:, i * ow + j + o_ch * oh * ow] = temp[o_ch].ravel()
+                w_unrolled_np[:, i * ow + j + o_ch * oh * ow] = temp[o_ch].ravel()
+
+    nih, niw = in_shape
+    nin_size = nih * niw
+    w_unrolled = np.zeros((channels * nin_size, channels * out_size), dtype=np.bool_)
+
+    for i in range(channels):
+        for j in range(nih):
+            w_unrolled[i * nin_size + j * niw : i * nin_size + j * niw + niw, :] = (
+                w_unrolled_np[
+                    i * in_size
+                    + (padding[0] + j) * iw
+                    + padding[1] : i * in_size
+                    + (padding[0] + j) * iw
+                    + padding[1]
+                    + niw,
+                    :,
+                ]
+            )
 
     return w_unrolled
 
 
 def _func_pool2d(
     x_chw: SpikeType,
     out_shape: Size2Type,
     ksize: Size2Type,
     stride: Size2Type,
     padding: Size2Type,
     type: str,
+    threshold: int,
 ) -> SpikeType:
     xcin, xh, xw = x_chw.shape
     kh, kw = ksize
     oh, ow = out_shape
     cout = xcin
 
     assert (xh + padding[0] * 2 - kh) // stride[0] + 1 == oh
@@ -250,16 +272,15 @@
                             c,
                             stride[0] * i : stride[0] * i + kh,
                             stride[1] * j : stride[1] * j + kw,
                         ]
                     )
 
     if type == "avg":
-        thres = kh * kw // 2 + 1
-        return out >= thres
+        return out >= threshold
     else:
         return out.astype(np.bool_)
 
 
 def _conv1d_faster(
     x_cl: NDArray[Any],
     out_shape: Size1Type,
```

### Comparing `paibox-1.1.0a2/paibox/components/synapses/synapses.py` & `paibox-1.1.0a3/paibox/components/synapses/synapses.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,61 +14,87 @@
     Conv2dSyn,
     ConvTranspose1dSyn,
     ConvTranspose2dSyn,
     FullConnSyn,
 )
 from .conv_types import _KOrder3d, _KOrder4d, _Size1Type, _Size2Type
 from .conv_utils import _pair, _single
-from .transforms import GeneralConnType as GConnType
+from .transforms import ConnType
 
 if sys.version_info >= (3, 13):
     from warnings import deprecated
 else:
     from typing_extensions import deprecated
 
-__all__ = ["FullConn", "Conv1d", "Conv2d", "ConvTranspose1d", "ConvTranspose2d"]
+__all__ = [
+    "FullConn",
+    "MatMul2d",
+    "Conv1d",
+    "Conv2d",
+    "ConvTranspose1d",
+    "ConvTranspose2d",
+]
 
 
 class FullConn(FullConnSyn):
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: NeuDyn,
         weights: DataArrayType = 1,
         *,
-        conn_type: GConnType = GConnType.MatConn,
+        conn_type: ConnType = ConnType.All2All,
         name: Optional[str] = None,
     ) -> None:
         """Full-connected synapses.
 
         Args:
             - source: source neuron.
             - dest: destination neuron.
             - weights: weights of the synapses. It can be a scalar or `np.ndarray`.
             - conn_type: the type of connection.
             - name: name of the full-connected synapses. Optional.
         """
-        super().__init__(source, dest, weights, conn_type, name)
+        super().__init__(source, dest, weights, conn_type, name=name)
 
 
 @deprecated(
     "'NoDecay' will be removed in a future version. Use 'FullConn' instead.",
     category=PAIBoxDeprecationWarning,
 )
-class NoDecay(FullConn):
+class NoDecay(FullConnSyn):
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
         dest: NeuDyn,
         weights: DataArrayType = 1,
         *,
-        conn_type: GConnType = GConnType.MatConn,
+        conn_type: ConnType = ConnType.All2All,
         name: Optional[str] = None,
     ) -> None:
-        super().__init__(source, dest, weights, conn_type=conn_type, name=name)
+        super().__init__(source, dest, weights, conn_type, name=name)
+
+
+class MatMul2d(FullConnSyn):
+    def __init__(
+        self,
+        source: Union[NeuDyn, InputProj],
+        dest: NeuDyn,
+        weights: np.ndarray,
+        name: Optional[str] = None,
+    ) -> None:
+        """MatMul2d synapses.
+
+        Args:
+            - source: source neuron.
+            - dest: destination neuron.
+            - weights: weights of the synapses.
+            - name: name of the matmul2d. Optional.
+        """
+        super().__init__(source, dest, weights, ConnType.MatConn, name)
 
 
 class Conv1d(Conv1dSyn):
     def __init__(
         self,
         source: Union[Neuron, InputProj],
         dest: Neuron,
```

### Comparing `paibox-1.1.0a2/paibox/components/synapses/transforms.py` & `paibox-1.1.0a3/paibox/components/synapses/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import warnings
 from enum import Enum, auto, unique
-from typing import Literal
+from typing import Literal, Optional
 
 import numpy as np
 from paicorelib import WeightPrecision as WP
 
 from paibox.exceptions import AutoOptimizationWarning, ShapeError
 from paibox.types import DataArrayType, IntScalarType, SpikeType, SynOutType, WeightType
-from paibox.utils import is_shape
+from paibox.utils import is_shape, shape2num, typical_round
 
-from .conv_types import Size1Type, Size2Type
+from .conv_types import Size1Type, Size2Type, SizeAnyType
 from .conv_utils import (
     _conv1d_faster,
     _conv1d_unroll,
     _conv2d_faster,
     _conv2d_unroll,
     _convtranspose1d_faster,
     _convtranspose1d_unroll,
@@ -40,22 +40,16 @@
 MIN_INT2 = np.int8(-2)
 MAX_INT4 = np.int8(7)
 MIN_INT4 = np.int8(-8)
 MAX_INT8 = np.iinfo(np.int8).max
 MIN_INT8 = np.iinfo(np.int8).min
 
 
-class ConnType(Enum):
-    """Basic connection enum type."""
-
-    pass
-
-
 @unique
-class GeneralConnType(ConnType):
+class ConnType(Enum):
     MatConn = auto()
     """General matrix connection."""
 
     One2One = auto()
     """One-to-one connection."""
 
     Identity = auto()
@@ -262,27 +256,77 @@
             self.weights
             if self.weights.ndim == 2
             else (self.weights * np.ones(self.conn_size, dtype=np.bool_))
         )
 
 
 class MaskedLinear(Transform):
-    def __init__(self, conn_size: Size2Type, weights: np.ndarray) -> None:
-        if not is_shape(weights, conn_size):
-            raise ShapeError(f"expected shape is {conn_size}, but got {weights.shape}.")
+    def __init__(
+        self, in_shape: SizeAnyType, out_shape: SizeAnyType, weights: np.ndarray
+    ) -> None:
+        self.in_shape = (1,) * (2 - len(in_shape)) + in_shape
+        self.out_shape = (1,) * (2 - len(out_shape)) + out_shape
+
+        if self.in_shape[0] == weights.shape[0]:
+            self.axes = (1, 0)
+        elif self.in_shape[1] == weights.shape[0]:
+            self.axes = (0, 1)
+        else:
+            raise ShapeError(
+                f"cannot do matmul between shape {in_shape} & {weights.shape}."
+            )
+
+        _in_shape = tuple(self.in_shape[i] for i in self.axes)
+
+        if (expected_oshape := _in_shape[:-1] + weights.shape[1:]) != self.out_shape:
+            raise ShapeError(
+                f"wrong output shape, expected {expected_oshape}, but got {self.out_shape}."
+            )
 
         super().__init__(weights)
 
     def __call__(self, x: SpikeType, *args, **kwargs) -> SynOutType:
-        # (N,) @ (N, M) -> (M,)
-        return x @ self.weights.astype(np.int32)
+        # (n?, k) @ (k, m?) -> (n?, m?)
+        _x = x.reshape(self.in_shape).transpose(self.axes)
+
+        return _x @ self.weights.astype(np.int32)
+
+    @staticmethod
+    def _matmul_unroll(
+        in_shape: SizeAnyType,
+        out_shape: SizeAnyType,
+        weights: WeightType,
+        axes: tuple[int, ...],
+    ) -> WeightType:
+        n_ishape = shape2num(in_shape)
+        n_oshape = shape2num(out_shape)
+        in_shape_t = tuple(in_shape[i] for i in axes)
+
+        w_unrolled = np.zeros((n_ishape, n_oshape), dtype=weights.dtype)
+
+        orig_idx = np.arange(n_ishape).reshape(in_shape_t)
+        mapping_tbl = orig_idx.transpose(np.argsort(axes)).ravel()
+
+        for i in range(in_shape_t[0]):
+            w_unrolled[
+                i * weights.shape[0] : (i + 1) * weights.shape[0],
+                i * weights.shape[1] : (i + 1) * weights.shape[1],
+            ] = weights
+
+        return w_unrolled[mapping_tbl]
 
     @property
     def connectivity(self):
-        return self.weights
+        return self._matmul_unroll(
+            self.in_shape, self.out_shape, self.weights, self.axes
+        )
+
+    @property
+    def is_T(self) -> bool:
+        return self.axes == (1, 0)
 
 
 class Conv1dForward(Transform):
     def __init__(
         self,
         in_shape: Size1Type,
         out_shape: Size1Type,
@@ -454,50 +498,61 @@
             self.stride,
             self.padding,
             self.output_padding,
         )
 
 
 class _Pool2dForward(Transform):
-    # DO NOT use in the `FullConnectedSyn`
     def __init__(
         self,
         channels: int,
         in_shape: Size2Type,
         out_shape: Size2Type,
         kernel_size: Size2Type,
         stride: Size2Type,
         padding: Size2Type,
         # fm_order: _Order3d,
         pool_type: Literal["avg", "max"],
+        threshold: Optional[int] = None,
     ) -> None:
         self.channels = channels
         self.in_shape = in_shape
         self.out_shape = out_shape
         self.ksize = kernel_size
         self.stride = stride
         self.padding = padding
         # self.fm_order = fm_order
         self.pool_type = pool_type
+        if isinstance(threshold, int):
+            self.threshold = threshold
+        else:
+            self.threshold = typical_round(shape2num(kernel_size) / 2)
 
-        super().__init__(np.asarray(1, dtype=np.int8))
+        super().__init__(1)
 
     def __call__(self, x: SpikeType, *args, **kwargs) -> SpikeType:
         # if self.fm_order == "HWC":
         #     # (N,) -> (H, W, C) -> (C, H, W)
         #     _x = x.reshape(self.in_shape + (self.channels,)).transpose(2, 0, 1)
         # else:
         _x = x.reshape((self.channels,) + self.in_shape)
 
         return _func_pool2d(
-            _x, self.out_shape, self.ksize, self.stride, self.padding, self.pool_type
+            _x,
+            self.out_shape,
+            self.ksize,
+            self.stride,
+            self.padding,
+            self.pool_type,
+            self.threshold,
         )
 
     @property
     def connectivity(self):
         return _pool2d_kernel_unroll(
             self.channels,
             self.in_shape,
             self.out_shape,
             self.ksize,
             self.stride,
+            self.padding,
         )
```

### Comparing `paibox-1.1.0a2/paibox/context.py` & `paibox-1.1.0a3/paibox/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Dict, TypeVar
+from typing import Any, TypeVar
 
 __all__ = ["FRONTEND_ENV"]
 
 
 _KT = TypeVar("_KT")
 _VT = TypeVar("_VT")
 
 # XXX: use collections.UserDict[_KT, _VT] in 3.9+
 
 
-class _Context(Dict[_KT, _VT]):
+class _Context(dict[_KT, _VT]):
     def load(self, key: Any, default: Any = None) -> Any:
         """Load the context by the `key`.
 
         Args:
             - key: the key to indicate the data.
             - default: the default value when `key` is not defined.
         """
```

### Comparing `paibox-1.1.0a2/paibox/exceptions.py` & `paibox-1.1.0a3/paibox/exceptions.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a2/paibox/mixin.py` & `paibox-1.1.0a3/paibox/mixin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+import typing
+from collections.abc import Sequence
 from copy import deepcopy
 from functools import wraps
-from typing import Any, Dict, Optional, Sequence, Type, TypeVar
+from typing import Any, Optional, TypeVar
 
 import numpy as np
 
 from .context import _FRONTEND_CONTEXT
 from .exceptions import RegisterError
 from .naming import get_unique_name
 from .node import NodeDict
 from .types import VoltageType
 
+if typing.TYPE_CHECKING:
+    from paibox.components import FullConnectedSyn
+
 _T = TypeVar("_T")
 
 
 def singleton(cls):
     instances = {}
 
     @wraps(cls)
@@ -77,18 +82,18 @@
         if isinstance(elem, PAIBoxObject):
             return elem._name
         else:
             return get_unique_name("ContainerElem")
 
     def elem_format(
         self,
-        child_type: Type[_T],
+        child_type: type[_T],
         *children_as_tuple: Sequence[_T],
-        **children_as_dict: Dict[Any, _T],
-    ) -> Dict[str, _T]:
+        **children_as_dict: dict[Any, _T],
+    ) -> dict[str, _T]:
         elems = dict()
 
         for child in children_as_tuple:
             if isinstance(child, child_type):
                 elems[self._get_elem_name(child)] = child
 
             elif isinstance(child, (list, tuple)):
@@ -122,27 +127,26 @@
 
     def add_elem(self, *elems, **elements) -> None:
         """Add elements as a dictionary"""
         self.children.update(self.elem_format(object, *elems, **elements))
 
 
 class ReceiveInputProj(MixIn):
-    master_nodes: NodeDict[str, Any]
+    master_nodes: NodeDict[str, "FullConnectedSyn"]
 
-    def register_master(self, key: str, master_target) -> None:
-        if key in self.master_nodes:
+    def register_master(
+        self, key: str, master_target: "FullConnectedSyn", strict: bool = True
+    ) -> None:
+        if key in self.master_nodes and strict:
             raise RegisterError(f"master node with key '{key}' already exists.")
 
         self.master_nodes[key] = master_target
 
-    def unregister_master(self, key: str, strict: bool = True) -> Optional[Any]:
-        if key in self.master_nodes:
-            return self.master_nodes.pop(key, None)
-        elif strict:
-            raise KeyError(f"key '{key}' not found in master nodes.")
+    def unregister_master(self, key: str) -> Optional["FullConnectedSyn"]:
+        return self.master_nodes.pop(key, None)
 
     def get_master_node(self, key: str) -> Optional[Any]:
         return self.master_nodes.get(key, None)
 
     def sum_inputs(self, *, init: VoltageType = 0, **kwargs) -> VoltageType:  # type: ignore
         # TODO Out is a np.ndarray right now, but it may be more than one type.
         output = init
```

### Comparing `paibox-1.1.0a2/paibox/naming.py` & `paibox-1.1.0a3/paibox/naming.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a2/paibox/network.py` & `paibox-1.1.0a3/paibox/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Optional, Type, Union
+from typing import Optional, Union
 
 import numpy as np
 from typing_extensions import TypeAlias
 
 from .base import DynamicSys, PAIBoxObject, SynSys
 from .collector import Collector
 from .components import NeuModule, Neuron, Projection
@@ -13,15 +13,15 @@
 __all__ = ["DynSysGroup", "Network"]
 
 
 class DynSysGroup(DynamicSys, Container):
     def __init__(
         self,
         *components_as_tuple,
-        component_type: Type = DynamicSys,
+        component_type: type = DynamicSys,
         name: Optional[str] = None,
         **components_as_dict,
     ) -> None:
         super().__init__(name)
         self.children = NodeDict(
             self.elem_format(component_type, *components_as_tuple, **components_as_dict)
         )
@@ -68,15 +68,15 @@
 
     def __call__(self, **kwargs) -> None:
         return self.update(**kwargs)
 
     @classmethod
     def build_fmodule(
         cls, network: "DynSysGroup", **build_options
-    ) -> Dict[NeuModule, BuiltComponentType]:
+    ) -> dict[NeuModule, BuiltComponentType]:
         generated = dict()
         modules = network.components.subset(NeuModule).unique()
 
         for module in modules.values():
             generated[module] = module.build(network, **build_options)
 
         return generated
@@ -97,14 +97,15 @@
     def _remove_components(self, *components: DynamicSys) -> None:
         """Remove components from the network."""
         for cpn in components:
             for tag, obj in self.__dict__.items():
                 if cpn is obj:
                     cpn.__gh_build_ignore__ = False
                     delattr(self, tag)
+                    break
 
     def _ignore_components(self, *components: DynamicSys) -> None:
         for cpn in components:
             if cpn in self.__dict__.values():
                 cpn.__gh_build_ignore__ = True
 
     @property
```

### Comparing `paibox-1.1.0a2/paibox/simulator/encoder.py` & `paibox-1.1.0a3/paibox/simulator/encoder.py`

 * *Files identical despite different names*

### Comparing `paibox-1.1.0a2/paibox/simulator/simulator.py` & `paibox-1.1.0a3/paibox/simulator/simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,59 @@
 import copy
 import warnings
-from typing import Any, Dict, List, Optional
+from typing import Any, Optional
 
 import numpy as np
 from numpy.typing import NDArray
 
 from paibox.base import DynamicSys, PAIBoxObject
 from paibox.context import _FRONTEND_CONTEXT
-from paibox.exceptions import SimulationError
+from paibox.exceptions import PAIBoxDeprecationWarning, SimulationError
 
-from .probe import Probe
+__all__ = ["Probe", "Simulator"]
 
-__all__ = ["Simulator"]
+
+class Probe(PAIBoxObject):
+    target: PAIBoxObject
+
+    def __init__(
+        self,
+        target: PAIBoxObject,
+        attr: str,
+        *,
+        name: Optional[str] = None,
+    ) -> None:
+        """
+        Arguments:
+            - target: the target that needs to be monitored.
+            - attr: the attribute that needs to be monitored.
+            - name: the name of the probe. Optional.
+        """
+        self.attr = attr
+        self._check_attr(target)
+
+        super().__init__(name)
+
+    def _check_attr(self, target: PAIBoxObject) -> None:
+        if not hasattr(target, self.attr):
+            raise AttributeError(
+                f"attribute '{self.attr}' not found in target {target}."
+            )
+
+        self.target = target
+
+    @property
+    def _label_txt(self) -> str:
+        return f"'{self.name}'" if hasattr(self, "name") else ""
+
+    def __str__(self) -> str:
+        return f"<Probe {self._label_txt} of '{self.attr}' of {self.target.name}>"
+
+    def __repr__(self) -> str:
+        return f"<Probe {self._label_txt} at 0x{id(self):x} of '{self.attr}' of {self.target.name}>"
 
 
 class Simulator(PAIBoxObject):
     def __init__(
         self,
         target: DynamicSys,
         start_time_zero: bool = False,
@@ -42,15 +80,15 @@
         self._start_time_zero = start_time_zero
         """Whether to start the simulation at time 0."""
 
         self._sim_data = dict()
         self._sim_data["ts"] = []  # Necessary key for recording timestamp
 
         self.data = _SimulationData(self._sim_data)
-        self.probes: List[Probe] = []
+        self.probes: list[Probe] = []
 
         self._add_inner_probes()
         self.reset()
 
     def run(self, duration: int, reset: bool = False, **kwargs) -> None:
         """
         Arguments:
@@ -59,15 +97,15 @@
             - kwargs：determined by the parameter format of the input node. It will be deprecated, \
                 please use 'FRONTEND_ENV.save()' instead.
         """
         if kwargs:
             warnings.warn(
                 "passing extra arguments through 'run()' will be deprecated. "
                 "Use 'FRONTEND_ENV.save()' instead.",
-                DeprecationWarning,
+                PAIBoxDeprecationWarning,
             )
 
         if duration < 1:
             raise SimulationError(f"duration must be positive, but got {duration}.")
 
         n_steps = self._get_nstep(duration)
         if n_steps < 1:
@@ -115,15 +153,15 @@
             self._update_probes()
 
     def _destroy_probes(self):
         self.probes.clear()
         self._sim_data.clear()
         self.data.reset()
 
-    def get_raw(self, probe: Probe) -> List[Any]:
+    def get_raw(self, probe: Probe) -> list[Any]:
         """Retrieve the raw data.
 
         Argument:
             - probe: the probe to retrieve.
             - t: retrieve the data at time `t`.
 
         NOTE: For faster access, use the attribute of `data`.
@@ -183,15 +221,15 @@
         """Timestamp of simulator. Simulation at this time is not finished."""
         return self._ts
 
 
 class _SimulationData(dict):
     """Data structure used to retrieve and access the simulation data."""
 
-    def __init__(self, raw: Dict[Probe, List[Any]]) -> None:
+    def __init__(self, raw: dict[Probe, list[Any]]) -> None:
         super().__init__()
         self.raw = raw
         self._cache = {}
 
     def __getitem__(self, key) -> Any:
         """
         Return simulation data for ``key`` object.
```

### Comparing `paibox-1.1.0a2/paibox/simulator/utils.py` & `paibox-1.1.0a3/paibox/simulator/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import Any, Tuple
+from typing import Any
 
 import numpy as np
 from numpy.typing import NDArray
 
-Size2Type = Tuple[int, int]
+Size2Type = tuple[int, int]
 
 
 """Faster Conv2d in FP32 format."""
 
 
 def _conv2d_faster_fp32(
     x_chw: NDArray[Any], kernel: NDArray[Any], stride: Size2Type, padding: Size2Type
```

### Comparing `paibox-1.1.0a2/paibox/utils.py` & `paibox-1.1.0a3/paibox/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Iterable, List, Sequence, Tuple
+from collections.abc import Iterable, Sequence
+from typing import Any, Optional
 
 import numpy as np
 
 from paibox.types import Shape
 
 """Handful utilities."""
 
@@ -31,15 +32,15 @@
     seen = set()
     for item in obj:
         seen.add(item)
 
     return len(seen)
 
 
-def merge_unique_ordered(list1: List[Any], list2: List[Any]) -> List[Any]:
+def merge_unique_ordered(list1: list[Any], list2: list[Any]) -> list[Any]:
     seen = set()
     result = []
 
     for item in list1 + list2:
         if item not in seen:
             seen.add(item)
             result.append(item)
@@ -78,15 +79,15 @@
         a = 1
         for b in shape:
             a *= b
 
         return a
 
 
-def as_shape(x, min_dim: int = 0) -> Tuple[int, ...]:
+def as_shape(x, min_dim: int = 0) -> tuple[int, ...]:
     """Return a tuple if `x` is iterable or `(x,)` if `x` is integer."""
     if is_integer(x):
         _shape = (int(x),)
     elif is_iterable(x):
         _shape = tuple(int(e) for e in x)
     else:
         raise ValueError(f"{x} cannot be safely converted to a shape.")
@@ -126,7 +127,46 @@
 
     return isinstance(obj, Iterable)
 
 
 def fn_sgn(a, b) -> int:
     """Signal function."""
     return 1 if a > b else -1 if a < b else 0
+
+
+def typical_round(number: float) -> int:
+    if number - int(number) < 0.5:
+        return int(number)
+    else:
+        return int(number) + 1
+
+
+def arg_check_pos(arg: int, desc: Optional[str] = None) -> int:
+    _desc = "value" if desc is None else f"{desc}"
+    if arg < 1:
+        raise ValueError(f"{_desc} must be positive, but got {arg}.")
+
+    return arg
+
+
+def arg_check_non_pos(arg: int, desc: Optional[str] = None) -> int:
+    _desc = "value" if desc is None else f"{desc}"
+    if arg > 0:
+        raise ValueError(f"{_desc} must be non-positive, but got {arg}.")
+
+    return arg
+
+
+def arg_check_neg(arg: int, desc: Optional[str] = None) -> int:
+    _desc = "value" if desc is None else f"{desc}"
+    if arg > -1:
+        raise ValueError(f"{_desc} must be negative, but got {arg}.")
+
+    return arg
+
+
+def arg_check_non_neg(arg: int, desc: Optional[str] = None) -> int:
+    _desc = "value" if desc is None else f"{desc}"
+    if arg < 0:
+        raise ValueError(f"{_desc} must be non-negative, but got {arg}.")
+
+    return arg
```

### Comparing `paibox-1.1.0a2/pyproject.toml` & `paibox-1.1.0a3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paibox"
-version = "1.1.0a2"
+version = "1.1.0a3"
 description = "Toolchain of PAICORE 2.0"
 authors = ["Ziru Pan <zrpan@stu.pku.edu.cn>"]
 maintainers = [
     "Hongtu Xia <hongtux@pku.edu.cn>",
     "Siyuan Gao <siyuan-gao@outlook.com>",
     "Zhaoyang Hao <hzyang2218@gmail.com>",
     "Ziru Pan <zrpan@stu.pku.edu.cn>",
@@ -16,64 +16,56 @@
 documentation = "https://github.com/PAICookers/PAIBox#readme"
 keywords = ["PAICORE 2.0", "PAIBox", "SNN", "Toolchain"]
 classifiers = [
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries",
 ]
 packages = [{ include = "paibox" }]
 
 # Includes the document
 include = ["docs/Guide-of-PAIBox.md", "CHANGELOG.md"]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 pydantic = "^2.0"
-numpy = "^1.24.0"
-paicorelib = "^1.1.2"
+numpy = "^1.26.0"
+paicorelib = "^1.1.4"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = { version = "^8.0.0", python = "^3.8" }
+pytest = "^8.0.0"
 pytest-md = "^0.2.0"
-torch = { version = "^2.2.1+cpu", optional = true, source = "torch-cpu" }
 paicorelib = {git = "https://github.com/PAICookers/PAIlib.git", rev = "dev"}
-orjson = "^3.10.1"
+orjson = "^3.10.0"
 
 
 [tool.poetry.group.dev.dependencies]
-orjson = "^3.10.1"
+orjson = "^3.10.0"
 
 
 [tool.pytest.ini_options]
-minversion = "7.0.0"
+minversion = "8.0.0"
 testpaths = ["tests"]
 
 
 [[tool.poetry.source]]
-name = "torch-cpu"
-url = "https://download.pytorch.org/whl/cpu"
-priority = "explicit"
-
-
-[[tool.poetry.source]]
 name = "tsinghua"
 url = "https://pypi.tuna.tsinghua.edu.cn/simple"
 priority = "primary"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `paibox-1.1.0a2/PKG-INFO` & `paibox-1.1.0a3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 Metadata-Version: 2.1
 Name: paibox
-Version: 1.1.0a2
+Version: 1.1.0a3
 Summary: Toolchain of PAICORE 2.0
 Home-page: https://github.com/PAICookers/PAIBox
 License: GPL-3.0-or-later
 Keywords: PAICORE 2.0,PAIBox,SNN,Toolchain
 Author: Ziru Pan
 Author-email: zrpan@stu.pku.edu.cn
 Maintainer: Hongtu Xia
 Maintainer-email: hongtux@pku.edu.cn
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: numpy (>=1.24.0,<2.0.0)
-Requires-Dist: paicorelib (>=1.1.2,<2.0.0)
+Requires-Dist: numpy (>=1.26.0,<2.0.0)
+Requires-Dist: paicorelib (>=1.1.4,<2.0.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Project-URL: Documentation, https://github.com/PAICookers/PAIBox#readme
 Project-URL: Repository, https://github.com/PAICookers/PAIBox
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # PAIBox
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIBox/blob/master/pyproject.toml">
-        <img src="https://img.shields.io/pypi/pyversions/paibox">
+        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/paibox">
     </a>
-    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.1.0a2">
-        <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox?color=orange">
+    <a href="https://pypi.org/project/paibox/">
+        <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/paibox?color=pink">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIBox">
-      <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIBox/master?color=red">
+        <img alt="CodeFactor Grade" src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIBox?color=orange">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIBox/master">
-	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIBox/master.svg" alt="pre-commit.ci status">
+        <img alt="pre-commit.ci status" src="https://results.pre-commit.ci/badge/github/PAICookers/PAIBox/master.svg">
     </a>
 </p>
 
 👉 用户使用指南：[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
 
 高效编写测试项目指南：[Guide-of-Test](docs/Guide-of-Test.md)
```

#### html2text {}

```diff
@@ -1,26 +1,23 @@
-Metadata-Version: 2.1 Name: paibox Version: 1.1.0a2 Summary: Toolchain of
+Metadata-Version: 2.1 Name: paibox Version: 1.1.0a3 Summary: Toolchain of
 PAICORE 2.0 Home-page: https://github.com/PAICookers/PAIBox License: GPL-3.0-
 or-later Keywords: PAICORE 2.0,PAIBox,SNN,Toolchain Author: Ziru Pan Author-
 email: zrpan@stu.pku.edu.cn Maintainer: Hongtu Xia Maintainer-email:
-hongtux@pku.edu.cn Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
+hongtux@pku.edu.cn Requires-Python: >=3.9,<4.0 Classifier: Intended Audience ::
 Science/Research Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
-Development :: Build Tools Classifier: Topic :: Software Development ::
-Libraries Requires-Dist: numpy (>=1.24.0,<2.0.0) Requires-Dist: paicorelib
-(>=1.1.2,<2.0.0) Requires-Dist: pydantic (>=2.0,<3.0) Project-URL:
-Documentation, https://github.com/PAICookers/PAIBox#readme Project-URL:
-Repository, https://github.com/PAICookers/PAIBox Description-Content-Type:
-text/markdown
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Build Tools Classifier: Topic ::
+Software Development :: Libraries Requires-Dist: numpy (>=1.26.0,<2.0.0)
+Requires-Dist: paicorelib (>=1.1.4,<2.0.0) Requires-Dist: pydantic (>=2.0,<3.0)
+Project-URL: Documentation, https://github.com/PAICookers/PAIBox#readme
+Project-URL: Repository, https://github.com/PAICookers/PAIBox Description-
+Content-Type: text/markdown
                                    # PAIBox
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_a_i_b_o_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
- _v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_?_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/
-    _g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
+_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_C_o_d_e_F_a_c_t_o_r_ _G_r_a_d_e_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
 ð ç¨æ·ä½¿ç¨æåï¼[Guide-of-PAIBox](docs/Guide-of-PAIBox.md)
 é«æç¼åæµè¯é¡¹ç®æåï¼[Guide-of-Test](docs/Guide-of-Test.md)
 [Changelog](./CHANGELOG.md)
```

