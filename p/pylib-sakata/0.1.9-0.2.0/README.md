# Comparing `tmp/pylib-sakata-0.1.9.tar.gz` & `tmp/pylib-sakata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylib-sakata-0.1.9.tar", last modified: Wed Jul 20 09:00:00 2022, max compression
+gzip compressed data, was "pylib-sakata-0.2.0.tar", last modified: Mon Jun  3 15:11:47 2024, max compression
```

## Comparing `pylib-sakata-0.1.9.tar` & `pylib-sakata-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-07-20 09:00:00.221379 pylib-sakata-0.1.9/
--rw-rw-rw-   0        0        0     1091 2022-04-29 12:07:38.000000 pylib-sakata-0.1.9/LICENSE
--rw-rw-rw-   0        0        0    62397 2022-07-20 09:00:00.220378 pylib-sakata-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0    62057 2022-07-20 08:59:27.000000 pylib-sakata-0.1.9/README.md
--rw-rw-rw-   0        0        0       42 2022-07-20 09:00:00.221379 pylib-sakata-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      576 2022-07-20 08:59:48.000000 pylib-sakata-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-20 09:00:00.161379 pylib-sakata-0.1.9/src/
-drwxrwxrwx   0        0        0        0 2022-07-20 09:00:00.203379 pylib-sakata-0.1.9/src/pylib_sakata/
--rw-rw-rw-   0        0        0        0 2022-04-29 12:07:38.000000 pylib-sakata-0.1.9/src/pylib_sakata/__init__.py
--rw-rw-rw-   0        0        0    32607 2022-07-20 08:57:06.000000 pylib-sakata-0.1.9/src/pylib_sakata/ctrl.py
--rw-rw-rw-   0        0        0     8614 2022-05-22 12:50:33.000000 pylib-sakata-0.1.9/src/pylib_sakata/fft.py
--rw-rw-rw-   0        0        0      331 2022-04-29 12:07:38.000000 pylib-sakata-0.1.9/src/pylib_sakata/init.py
--rw-rw-rw-   0        0        0    11243 2022-05-28 17:38:19.000000 pylib-sakata-0.1.9/src/pylib_sakata/kinema.py
--rw-rw-rw-   0        0        0     3475 2022-05-02 05:12:25.000000 pylib-sakata-0.1.9/src/pylib_sakata/meas.py
--rw-rw-rw-   0        0        0     7485 2022-05-20 15:32:05.000000 pylib-sakata-0.1.9/src/pylib_sakata/plot.py
--rw-rw-rw-   0        0        0     2405 2022-04-29 12:07:38.000000 pylib-sakata-0.1.9/src/pylib_sakata/traj.py
-drwxrwxrwx   0        0        0        0 2022-07-20 09:00:00.219377 pylib-sakata-0.1.9/src/pylib_sakata.egg-info/
--rw-rw-rw-   0        0        0    62397 2022-07-20 09:00:00.000000 pylib-sakata-0.1.9/src/pylib_sakata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2022-07-20 09:00:00.000000 pylib-sakata-0.1.9/src/pylib_sakata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-20 09:00:00.000000 pylib-sakata-0.1.9/src/pylib_sakata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-07-20 09:00:00.000000 pylib-sakata-0.1.9/src/pylib_sakata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-03 15:11:47.252704 pylib-sakata-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2022-04-29 12:07:38.000000 pylib-sakata-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    64715 2024-06-03 15:11:47.252704 pylib-sakata-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    64415 2024-06-03 15:09:08.000000 pylib-sakata-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-03 15:11:47.252704 pylib-sakata-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      577 2024-06-03 15:08:45.000000 pylib-sakata-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 15:11:47.188655 pylib-sakata-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-06-03 15:11:47.232653 pylib-sakata-0.2.0/src/pylib_sakata/
+-rw-rw-rw-   0        0        0        0 2022-04-29 12:07:38.000000 pylib-sakata-0.2.0/src/pylib_sakata/__init__.py
+-rw-rw-rw-   0        0        0    32876 2024-06-03 14:50:12.000000 pylib-sakata-0.2.0/src/pylib_sakata/ctrl.py
+-rw-rw-rw-   0        0        0     8673 2024-02-15 15:56:29.000000 pylib-sakata-0.2.0/src/pylib_sakata/fft.py
+-rw-rw-rw-   0        0        0      331 2022-04-29 12:07:38.000000 pylib-sakata-0.2.0/src/pylib_sakata/init.py
+-rw-rw-rw-   0        0        0    11243 2022-05-28 17:38:19.000000 pylib-sakata-0.2.0/src/pylib_sakata/kinema.py
+-rw-rw-rw-   0        0        0     3932 2024-04-10 07:53:21.000000 pylib-sakata-0.2.0/src/pylib_sakata/meas.py
+-rw-rw-rw-   0        0        0     8025 2024-03-09 14:54:11.000000 pylib-sakata-0.2.0/src/pylib_sakata/plot.py
+-rw-rw-rw-   0        0        0    23911 2024-02-04 11:28:11.000000 pylib-sakata-0.2.0/src/pylib_sakata/traj.py
+drwxrwxrwx   0        0        0        0 2024-06-03 15:11:47.250654 pylib-sakata-0.2.0/src/pylib_sakata.egg-info/
+-rw-rw-rw-   0        0        0    64715 2024-06-03 15:11:47.000000 pylib-sakata-0.2.0/src/pylib_sakata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-06-03 15:11:47.000000 pylib-sakata-0.2.0/src/pylib_sakata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 15:11:47.000000 pylib-sakata-0.2.0/src/pylib_sakata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-03 15:11:47.000000 pylib-sakata-0.2.0/src/pylib_sakata.egg-info/top_level.txt
```

### Comparing `pylib-sakata-0.1.9/LICENSE` & `pylib-sakata-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylib-sakata-0.1.9/PKG-INFO` & `pylib-sakata-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: pylib-sakata
-Version: 0.1.9
+Version: 0.2.0
 Summary: Control system design and analysis package
 Home-page: https://github.com/Koichi-Sakata/pylib_sakata
 Author: Koichi Sakata
 Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-pylib-sakata User's Manual version-0.1.9
+pylib-sakata User's Manual version-0.2.0
 ===
 
-<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
-
 <!-- code_chunk_output -->
 
-- [pylib-sakata User's Manual version-0.1.9](#pylib-sakata-users-manual-version-019)
 - [1. Introduction](#1-introduction)
 - [2. Environment Setup](#2-environment-setup)
   - [2.1. Installation of Python](#21-installation-of-python)
   - [2.2. Installation  of required Python libraries](#22-installation--of-required-python-libraries)
   - [2.3. Installation of pylib-sakata](#23-installation-of-pylib-sakata)
   - [2.4. Installation of IDE for Python](#24-installation-of-ide-for-python)
     - [2.4.1. Visual Studio Code (VSCode)](#241-visual-studio-code-vscode)
@@ -32,15 +27,15 @@
       - [2.4.2.1. Installation of Spyder](#2421-installation-of-spyder)
       - [2.4.2.2. Initial setting of Spyder](#2422-initial-setting-of-spyder)
     - [2.4.3. PyCharm](#243-pycharm)
       - [2.4.3.1. Installation of PyCharm](#2431-installation-of-pycharm)
       - [2.4.3.2. Initial setting of PyCharm](#2432-initial-setting-of-pycharm)
     - [2.4.4. Comparison between  VSCode and Spyder and PyCharm](#244-comparison-between--vscode-and-spyder-and-pycharm)
   - [2.5. Getting started](#25-getting-started)
-- [3. pylib_sakata.ctrl](#3-pylib_sakatactrl)
+- [3. pylib\_sakata.ctrl](#3-pylib_sakatactrl)
   - [3.1. ZpkModel](#31-zpkmodel)
   - [3.2. tf](#32-tf)
   - [3.3. ss](#33-ss)
   - [3.4. zpk](#34-zpk)
   - [3.5. tf2ss](#35-tf2ss)
   - [3.6. tf2zpk](#36-tf2zpk)
   - [3.7. ss2tf](#37-ss2tf)
@@ -66,57 +61,60 @@
   - [3.27. pfopt](#327-pfopt)
   - [3.28. dob](#328-dob)
   - [3.29. zpetc](#329-zpetc)
   - [3.30. filt](#330-filt)
   - [3.31. minreal](#331-minreal)
   - [3.32. makeprmset](#332-makeprmset)
   - [3.33. defprmset](#333-defprmset)
-- [4. pylib_sakata.fft](#4-pylib_sakatafft)
+- [4. pylib\_sakata.fft](#4-pylib_sakatafft)
   - [4.1. FreqResp](#41-freqresp)
   - [4.2. fft](#42-fft)
-  - [4.3. fft_ave](#43-fft_ave)
+  - [4.3. fft\_ave](#43-fft_ave)
   - [4.4. tfestimate](#44-tfestimate)
   - [4.5. frdresize](#45-frdresize)
   - [4.6. frdsim](#46-frdsim)
-- [5. pylib_sakta.meas](#5-pylib_saktameas)
+- [5. pylib\_sakata.meas](#5-pylib_sakatameas)
   - [5.1. MeasData](#51-measdata)
   - [5.2. getcsvdata](#52-getcsvdata)
   - [5.3. gettxtdata](#53-gettxtdata)
   - [5.4. getmatdata](#54-getmatdata)
   - [5.5. getdata](#55-getdata)
   - [5.6. getdataindex](#56-getdataindex)
   - [5.7. measdata2frd](#57-measdata2frd)
-- [6. pylib_sakata.traj](#6-pylib_sakatatraj)
+- [6. pylib\_sakata.traj](#6-pylib_sakatatraj)
   - [6.1. TrajInf](#61-trajinf)
-  - [6.2. traj4th](#62-traj4th)
-- [7. pylib_sakata.plot](#7-pylib_sakataplot)
-  - [7.1. plot_xy](#71-plot_xy)
-  - [7.2. plot_tf](#72-plot_tf)
-  - [7.3. plot_tffrd](#73-plot_tffrd)
-  - [7.4. plot_nyquist](#74-plot_nyquist)
-  - [7.5. plot_nyquist_assistline](#75-plot_nyquist_assistline)
+  - [6.2. traj3rd](#62-traj3rd)
+  - [6.3. traj3rd2](#63-traj3rd2)
+  - [6.4. traj4th](#64-traj4th)
+  - [6.5. trajSinStep](#65-trajsinstep)
+- [7. pylib\_sakata.plot](#7-pylib_sakataplot)
+  - [7.1. plot\_xy](#71-plot_xy)
+  - [7.2. plot\_tf](#72-plot_tf)
+  - [7.3. plot\_tffrd](#73-plot_tffrd)
+  - [7.4. plot\_nyquist](#74-plot_nyquist)
+  - [7.5. plot\_nyquist\_assistline](#75-plot_nyquist_assistline)
   - [7.6. makefig](#76-makefig)
   - [7.7. savefig](#77-savefig)
   - [7.8. showfig](#78-showfig)
-- [8. pylib_sakata.init](#8-pylib_sakatainit)
-  - [8.1. close_all](#81-close_all)
-  - [8.2. clear_all](#82-clear_all)
+- [8. pylib\_sakata.init](#8-pylib_sakatainit)
+  - [8.1. close\_all](#81-close_all)
+  - [8.2. clear\_all](#82-clear_all)
 
 <!-- /code_chunk_output -->
 
-# 1. Introduction
+## 1. Introduction
 
-The pylib-sakata package is a set of python classes and functions that make the python-control package more convenient. This package provide practical level's tools to design controls and  to analysis of performance and stability of SISO LTI systems. These development environments are available on free.
+The pylib-sakata package is a set of python classes and functions that make the python-control package more convenient. This package provides practical level's tools to design controls and  to analysis of performance and stability of SISO LTI systems. These development environments are available on free.
 
-# 2. Environment Setup
+## 2. Environment Setup
 
-## 2.1. Installation of Python
+### 2.1. Installation of Python
 Python installation exe file can be downloaded [HERE](https://www.python.org/downloads/) for Windows. Check "Add Python 3.x to PATH" when you install Python.
 
-## 2.2. Installation  of required Python libraries
+### 2.2. Installation  of required Python libraries
 
 The pylib-sakata package requires [numpy](http://www.numpy.org), [scipy](http://www.scipy.org), [matplotlib](https://matplotlib.org), [pandas](https://pandas.pydata.org/), and [python-control](https://github.com/python-control/python-control). In addition, some routines require the [slycot](https://github.com/python-control/Slycot) library in order to implement more advanced features. 
 First, pip should be upgraded by the following command on the command prompt for Windows OS.
 ```shell
 python -m pip install --upgrade pip
 ```
 For Linux OS, pip can be upgraded by the following command on the shell.
@@ -129,89 +127,89 @@
 pip install scipy
 pip install matplotlib
 pip install pandas
 pip install control
 ```
 If those libraries can not be installed, please use pip3 instead of pip.
 
-## 2.3. Installation of pylib-sakata
+### 2.3. Installation of pylib-sakata
 
 The [pylib-sakata](https://github.com/Koichi-Sakata/pylib_sakata) package can be installed using pip using pip as following on the command prompt or on the shell.
 
 ```shell
 pip install pylib-sakata
 ```
 
-## 2.4. Installation of IDE for Python
+### 2.4. Installation of IDE for Python
 
 There are three recommended IDEs.
 
-### 2.4.1. Visual Studio Code (VSCode)
+#### 2.4.1. Visual Studio Code (VSCode)
 Although VSCode is actually an editor, it is available as Python IDE due to extensions. It is recommended to install it easily because of the versatility of extensions. The following figure shows VSCode IDE window.
 
 <img src="figure\vscode_disp.png" alt="vscode_disp" style="zoom: 33%;" />
 
-#### 2.4.1.1. Installation of VSCode
+##### 2.4.1.1. Installation of VSCode
 The latest version of VSCode installation exe file can be downloaded [HERE](https://code.visualstudio.com/) for Windows OS.
 For Linux OS, VSCode can be installed by the following command on the shell.
 ```shell
 $ sudo apt update 
 $ sudo apt install code
 ```
 
-#### 2.4.1.2. Initial setting of VSCode
+##### 2.4.1.2. Initial setting of VSCode
 1. Install Python extension for Visual Studio Code from extensions in the activity bar on the left side.
 1. Command (Ctrl+Shift+P) to open the command palette.
 1. Select your installed python.exe on  "Python: select interpreter".
 
-### 2.4.2. Spyder
+#### 2.4.2. Spyder
 Spyder is an IDE like MATLAB. If you are used to MATLAB, this IDE is recommended. The following figure shows Spyder IDE window.
 
 <img src="figure\spyder_disp.png" alt="spyder_disp" style="zoom: 33%;" />
 
-#### 2.4.2.1. Installation of Spyder
+##### 2.4.2.1. Installation of Spyder
 The latest version of Spyder installation exe file can be downloaded [HERE](https://www.spyder-ide.org/) for Windows OS.
 For Linux OS, Spyder can be installed by the following command on the shell.
 
 ```shell
 $ sudo apt update 
 $ sudo apt install spyder3
 ```
 
-#### 2.4.2.2. Initial setting of Spyder
+##### 2.4.2.2. Initial setting of Spyder
 1. Open Tools>Preferences>Python interpreter.
 1. Check "Use the following Python interpreter."
 1. Enter the path of your installed python.exe.
 1. Install spyder-kernels for your python version by the following command `pip install spyder-kernels==2.0.*` on the command prompt or on the shell.
 1. Reboot your PC.
 
-### 2.4.3. PyCharm
+#### 2.4.3. PyCharm
 Professional version is charged. Community version is free. Community version is enough for control system development. The following figure shows PyCharm window.
 
 <img src="figure\pycharm_disp.png" alt="spyder_disp" style="zoom: 33%;" />
 
-#### 2.4.3.1. Installation of PyCharm
+##### 2.4.3.1. Installation of PyCharm
 The latest version of PyCharm installation exe file can be downloaded [HERE](https://www.jetbrains.com/pycharm/download/). 
 
-#### 2.4.3.2. Initial setting of PyCharm
+##### 2.4.3.2. Initial setting of PyCharm
 It is not necessary.
 
-### 2.4.4. Comparison between  VSCode and Spyder and PyCharm
+#### 2.4.4. Comparison between  VSCode and Spyder and PyCharm
 
 |                    |        VSCode       |      Spyder       |     PyCharm       |
 | ------------------ | :-----------------: | :---------------: | :---------------: |
 | Cost               |        Free         |       Free        |    Free/Paid      |
 | Boot time          |        Fast         |       Slow        |       Normal      |
 | Processing speed   |        Fast         |       Normal      |       Normal      |
 | REPL mode          | need to switch REPL terminal  | Available | Available |
 | Variable Explorer  | Available on Jupyter terminal | Available (Class variables are invisible.) | Available |
 
 Spyder is more suitable than VSCode for early debugging. On the other hand, VSCode is stress-free than Spyder for late debugging you do not need to check inter states of variables. PyCharm is generally well-balanced. My recommendation is PyCharm.
 
-## 2.5. Getting started
+### 2.5. Getting started
 The pylib-sakata package can be imported as follows.
 ```python
 >>> import pylib_sakata
 ```
 This package consists of six modules as follows.
 1. **ctrl**: to design controllers and filters
 1. **fft**: to analysis FFT
@@ -228,17 +226,17 @@
 >>> from pylib_sakata import traj
 >>> from pylib_sakata import plot
 >>> from pylib_sakata import init
 ```
 
 Example codes are [HERE](https://github.com/Koichi-Sakata/pylib_sakata/tree/main/example).
 
-# 3. pylib_sakata.ctrl
+## 3. pylib_sakata.ctrl
 
-## 3.1. ZpkModel
+### 3.1. ZpkModel
 
 class pylib_sakata.ctrl.**ZpkModel**(*z, p, k, dt=0*)
 
 - Parameters:
   - z: zeros array of the LTI model
   - p: poles array of the LTI model
   - k: gain of the LTI model. Note: the gain is not system dc gain but coefficient of monic polynomials. This is different from the definition of dc gain in TransferFunction class.
@@ -295,15 +293,15 @@
 - \__**pow**__(*other*)
 	A zpk model to the power of x.
 
 - **feedback**(*other=1, sys='S'*)
 	Calculate the feedback system that consist of two zpk model (P: self and C: other).
 	sys: FB type (Optional), Default: 'S', Set in 'S': sensitivity function, 'T': complementary sensitivity function, 'SP': response from input disturbance to output
 
-## 3.2. tf
+### 3.2. tf
 
 pylib_sakata.ctrl.**tf**(*num, den, dt=0*)
 
 This function calls **tf** function in control library.
 
 - Parameters:
   - num: polynomial coefficients of the numerator of the LTI model
@@ -317,15 +315,15 @@
 >>> print(ctrl.tf([1., 2.], [3., 4., 5.]))
 
      s + 2
 ---------------
 3 s^2 + 4 s + 5
 ```
 
-## 3.3. ss
+### 3.3. ss
 
 pylib_sakata.ctrl.**ss**(*A, B, C, D, dt=0*)
 
 This function calls **ss** function in control library.
 
 - Parameters:
   - A, B, C, D: state space matrices
@@ -343,15 +341,15 @@
      [7.]]
 
 C = [[6. 8.]]
 
 D = [[9.]]
 ```
 
-## 3.4. zpk
+### 3.4. zpk
 
 pylib_sakata.ctrl.**zpk**(*z, p, k, dt=0*)
 
 - Parameters:
   - A, B, C, D: state space matrices
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
 - Returns:
@@ -362,21 +360,21 @@
 >>> ctrl.zpk([-1., -2.], [-3., -4., -5.], 2.)
 
       (s+1)(s+2)
 2 * ---------------
     (s+3)(s+4)(s+5)
 ```
 
-## 3.5. tf2ss
+### 3.5. tf2ss
 
-pylib_sakata.ctrl.**tf2ss**(*tf, form='reachable'*)
+pylib_sakata.ctrl.**tf2ss**(*tf, form=None*)
 
 - Parameters:
   - tf: instance of TransferFunction class
-  - form: canonical form (Optional), Default: reachable. You can select the canonical form in reachable, observable, and modal.
+  - form: canonical form (Optional), you can select the canonical form in 'reachable', 'observable', and 'modal'.
 - Returns:
   - out: instance of StateSpace class
 
 **Examples**
 ```python
 >>> Sys_tf = ctrl.tf([1., 2.], [3., 4., 5.])
 >>> print(ctrl.tf2ss(Sys_tf))
@@ -387,15 +385,15 @@
      [0.]]
 
 C = [[0.33333333 0.66666667]]
 
 D = [[0.]]
 ```
 
-## 3.6. tf2zpk
+### 3.6. tf2zpk
 
 pylib_sakata.ctrl.**tf2zpk**(*tf*)
 
 - Parameters:
   - tf: instance of TransferFunction class
 - Returns:
   - out: instance of ZpkModel class
@@ -407,15 +405,15 @@
 
                        (s+2)
 0.3333 * ----------------------------------
          (s+0.6667+1.106j)(s+0.6667-1.106j)
 ```
 
 
-## 3.7. ss2tf
+### 3.7. ss2tf
 
 pylib_sakata.ctrl.**ss2tf**(*ss*)
 
 - Parameters:
   - ss: instance of StateSpace class
 - Returns:
   - out: instance of TransferFunction class
@@ -426,15 +424,15 @@
 >>> print(ctrl.ss2tf(Sys_ss))
 
 9 s^2 + 113 s + 118
 -------------------
    s^2 + 3 s + 2
 ```
 
-## 3.8. ss2zpk
+### 3.8. ss2zpk
 
 pylib_sakata.ctrl.**ss2zpk**(*ss*)
 
 - Parameters:
   - ss: instance of StateSpace class
 - Returns:
   - out: instance of ZpkModel class
@@ -445,15 +443,15 @@
 >>> ctrl.ss2zpk(Sys_ss)
 
     (s+11.41)(s+1.149)
 9 * ------------------
         (s+2)(s+1)
 ```
 
-## 3.9. zpk2tf
+### 3.9. zpk2tf
 
 pylib_sakata.ctrl.**zpk2tf**(*zpk*)
 
 - Parameters:
   - zpk: instance of ZpkModel class
 - Returns:
   - out: instance of TransferFunction class
@@ -464,15 +462,15 @@
 >>> print(ctrl.zpk2tf(Sys_zpk))
 
     2 s^2 + 6 s + 4
 ------------------------
 s^3 + 12 s^2 + 47 s + 60
 ```
 
-## 3.10. zpk2ss
+### 3.10. zpk2ss
 
 pylib_sakata.ctrl.**zpk2ss**(*zpk, form='reachable'*)
 
 - Parameters:
   - zpk: instance of ZpkModel class
   - form: canonical form (Optional), Default: reachable. You can select the canonical form in reachable, observable, and modal.
 - Returns:
@@ -491,15 +489,15 @@
      [0.]]
 
 C = [[2. 6. 4.]]
 
 D = [[0.]]
 ```
 
-## 3.11. sys2frd
+### 3.11. sys2frd
 
 pylib_sakata.ctrl.**sys2frd**(*sys, freq*)
 
 - Parameters:
   - sys: LTI model (StateSpace or TransferFunction or ZpkModel)
   - freq: 1-D array frequency data [Hz]
 - Returns:
@@ -525,15 +523,15 @@
 freq = array([   1.            1.00069108    1.00138264 ...  998.61926487  999.30939397
  1000.        ])
 resp = array([1.89109027e-01-0.06951671j 1.89033162e-01-0.06962001j
  1.88957165e-01-0.0697232j  ... 4.57206511e-07-0.00031875j
  4.56575231e-07-0.00031853j 4.55944822e-07-0.00031831j])
 ```
 
-## 3.12. feedback
+### 3.12. feedback
 
 pylib_sakata.ctrl.**feedback**(*sysP, sysC, sys='S'*)
 
 This function is for calculating the feedback system that consist of two LTI model (P: plant and C: controller).
 
 - Parameters:
   - sysP: LTI model (StateSpace or TransferFunction or ZpkModel) of the plant
@@ -558,15 +556,15 @@
 >>> ctrl.feedback(P_zpk, C_zpk)
 
                      s(s+2)(s+2)s
 1 * -----------------------------------------------
     (s+1)(s+1-0.0001508j)(s+1+0.0001508j)(s+0.9998)
 ```
 
-## 3.13. frdfeedback
+### 3.13. frdfeedback
 
 pylib_sakata.ctrl.**frdfeedback**(*frdP, frdC, sys='S'*)
 
 This function is for calculating the feedback system that consist of two freqresp (P: plant and C: controller).
 
 - Parameters:
   - frdP: 1-D array complex data of the frequency response of the plant
@@ -586,15 +584,15 @@
 >>> C_frd = ctrl.tf2frd(C_tf, freq)
 >>> ctrl.frdfeedback(P_frd, C_frd)
 array([1.04746047+1.56990662e-02j, 1.04739933+1.56671729e-02j,
        1.04733826+1.56353434e-02j, ..., 1.00000005+1.61927479e-11j,
        1.00000005+1.61592227e-11j, 1.00000005+1.61257668e-11j])
 ```
 
-## 3.14. c2d
+### 3.14. c2d
 
 pylib_sakata.ctrl.**c2d**(*sysC, dt, method='tustin'*)
 
 The matched method of **c2d** in control library does not supported for pure integrals and pure derivatives because of dc gain inf error. This function solved this problem.
 
 - Parameters:
   - sysC: continuous time LTI model (StateSpace or TransferFunction or ZpkModel) of the plant
@@ -602,44 +600,40 @@
   - method: discretized method (Optional), Default: 'tustin', set a method in 'tustin', 'matched', 'zoh', and etc.
 - Returns:
   - out: discrete time LTI model (StateSpace or TransferFunction or ZpkModel) of the feedback system
 
 **Examples**
 ```python
 >>> C_tf = ctrl.tf([1., 3., 2.], [1., 3., 0.])
->>> print(ctrl.c2d_matched(C_tf, 0.001))
+>>> print(ctrl.c2d(C_tf, 0.001, 'matched'))
 
 z^2 - 1.997 z + 0.997
 ---------------------
 z^2 - 1.997 z + 0.997
 
 dt = 0.001
 ```
 ```python
 >>> C_zpk = ctrl.zpk([-1., -2.,], [0., -3.,], 1.)
->>> ctrl.c2d_matched(C_zpk, 0.001)
+>>> ctrl.c2d(C_zpk, 0.001, 'matched')
 
     (z-0.999)(z-0.998)
 1 * ------------------
       (z-1)(z-0.997)
 
 dt = 0.001
 ```
 
-## 3.15. pi
+### 3.15. pi
 
 pylib_sakata.ctrl.**pi**(*freq, zeta, L, R, dt=None, method='tustin'*)
 
 This function is for design of a PI controller.
-$$
-C_{PI}(s) = K_P + \frac{K_I}{s} = \frac{b_1s+b_0}{s}
-$$
-$$
-P(s) = \frac{1}{Ls+R}
-$$
+$$C_{PI}(s) = K_P + \frac{K_I}{s} = \frac{b_1s+b_0}{s}$$
+$$P(s) = \frac{1}{Ls+R}$$
 
 - Parameters:
   - freq: frequency[Hz] of the pole pair of the feedback system with the PI controller
   - zeta: damping of the pole pair of the feedback system with the PI controller
   - L: inductance[H] of the plant
   - R: resistance[$\Omega$] of the plant
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
@@ -661,25 +655,21 @@
 2844 z + 1104
 -------------
     z - 1
 
 dt = 0.001
 ```
 
-## 3.16. pd
+### 3.16. pd
 
 pylib_sakata.ctrl.**pd**(*freq1, freq2, zeta2, M, C, K, dt=None, method='tustin'*)
 
 This function is for design of a PD controller.
-$$
-C_{PID}(s) = K_P + \frac{K_D s}{\tau_D s+1} = \frac{b_1s+b_0}{s+a_1}
-$$
-$$
-P(s) = \frac{1}{Ms^2+Cs+K}
-$$
+$$C_{PD}(s) = K_P + \frac{K_D s}{\tau_D s+1} = \frac{b_1s+b_0}{s+a_0}$$
+$$P(s) = \frac{1}{Ms^2+Cs+K}$$
 
 - Parameters:
   - freq1: frequency[Hz] of the first pole of the feedback system with the PD controller
   - freq2: frequency[Hz] of the second pole pair of the feedback system with the PD controller
   - zeta2: damping of the second pole pair of the feedback system with the PD controller
   - M: mass[kg] of the plant
   - C: viscosity[N/(m/s)] of the plant
@@ -703,25 +693,21 @@
 1.653e+04 z - 1.607e+04
 -----------------------
       z - 0.8641
 
 dt = 0.001
 ```
 
-## 3.17. pid
+### 3.17. pid
 
 pylib_sakata.ctrl.**pid**(*freq1, zeta1, freq2, zeta2, M, C, K, dt=None, method='tustin'*)
 
 This function is for design of a PID controller.
-$$
-C_{PID}(s) = K_P + \frac{K_I}{s} + \frac{K_D s}{\tau_D s+1} = \frac{b_2s^2+b_1s+b_0}{s^2+a_1s}
-$$
-$$
-P(s) = \frac{1}{Ms^2+Cs+K}
-$$
+$$C_{PID}(s) = K_P + \frac{K_I}{s} + \frac{K_D s}{\tau_D s+1} = \frac{b_2s^2+b_1s+b_0}{s^2+a_1s}$$
+$$P(s) = \frac{1}{Ms^2+Cs+K}$$
 
 - Parameters:
   - freq1: frequency[Hz] of the first pole pair of the feedback system with the PID controller
   - zeta1: damping of the first pole pair of the feedback system with the PID controller
   - freq2: frequency[Hz] of the second pole pair of the feedback system with the PID controller
   - zeta2: damping of the second pole pair of the feedback system with the PID controller
   - M: mass[kg] of the plant
@@ -746,22 +732,20 @@
 3.32e+04 z^2 - 6.485e+04 z + 3.167e+04
 --------------------------------------
         z^2 - 1.811 z + 0.8111
 
 dt = 0.001
 ```
 
-## 3.18. pl1st
+### 3.18. pl1st
 
 pylib_sakata.ctrl.**pl1st**(*freq1, freq2, dt=None, method='tustin'*)
 
 This function is for design of a first order phase lead filter.
-$$
-F_{PL}(s) = \frac{f_2}{f_1} * \frac{s+2\pi f_1}{s+2\pi f_2}
-$$
+$$F_{PL}(s) = \frac{f_2}{f_1} * \frac{s+2\pi f_1}{s+2\pi f_2}$$
 
 - Parameters:
   - freq1: frequency[Hz] of numerator of the phase lead filter
   - freq2: frequency[Hz] of denominator of the phase lead filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
@@ -781,22 +765,20 @@
         (z-0.7285)
 1.761 * ----------
         (z-0.5219)
 
 dt = 0.001
 ```
 
-## 3.19. pl2nd
+### 3.19. pl2nd
 
 pylib_sakata.ctrl.**pl2nd**(*freq1, zeta1, freq2, zeta2, dt=None, method='tustin'*)
 
 This function is for design of a second order phase lead filter.
-$$
-F_{PL^2}(s) = \left( \frac{f_2}{f_1} \right)^2 * \frac{s^2+2\zeta_1 (2\pi f_1)s+(2\pi f_1)^2}{s^2+2\zeta_2 (2\pi f_2)s+(2\pi f_2)^2}
-$$
+$$F_{PL^2}(s) = \left( \frac{f_2}{f_1} \right)^2 * \frac{s^2+2\zeta_1 (2\pi f_1)s+(2\pi f_1)^2}{s^2+2\zeta_2 (2\pi f_2)s+(2\pi f_2)^2}$$
 
 - Parameters:
   - freq1: frequency[Hz] of numerator of the phase lead filter
   - zeta1: damping of numerator of the phase lead filter
   - freq2: frequency[Hz] of denominator of the phase lead filter
   - zeta2: damping of denominator of the phase lead filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
@@ -818,22 +800,20 @@
 1.618 z^2 - 2.536 z + 1.046
 ---------------------------
   z^2 - 1.172 z + 0.4283
 
 dt = 0.001
 ```
 
-## 3.20. lpf1st
+### 3.20. lpf1st
 
 pylib_sakata.ctrl.**lpf1st**(*freq, dt=None, method='tustin'*)
 
 This function is for design of a first order low pass filter.
-$$
-F_{LP}(s) = \frac{2\pi f}{s+2\pi f}
-$$
+$$F_{LP}(s) = \frac{2\pi f}{s+2\pi f}$$
 
 - Parameters:
   - freq: frequency[Hz] of the low pass filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
   - out: instance of TransferFunction class of the low pass filter
@@ -852,22 +832,20 @@
 0.2391 z + 0.2391
 -----------------
    z - 0.5219
 
 dt = 0.001
 ```
 
-## 3.21. lpf2nd
+### 3.21. lpf2nd
 
 pylib_sakata.ctrl.**lpf2nd**(*freq, zeta, dt=None, method='tustin'*)
 
 This function is for design of a second order low pass filter.
-$$
-F_{LP^2}(s) = \frac{(2\pi f)^2}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}
-$$
+$$F_{LP^2}(s) = \frac{(2\pi f)^2}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}$$
 
 - Parameters:
   - freq: frequency[Hz] of the low pass filter
   - zeta1: damping of the low pass filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
@@ -887,22 +865,20 @@
 0.06415 z^2 + 0.1283 z + 0.06415
 --------------------------------
      z^2 - 1.172 z + 0.4283
 
 dt = 0.001
 ```
 
-## 3.22. hpf1st
+### 3.22. hpf1st
 
 pylib_sakata.ctrl.**hpf1st**(*freq, dt=None, method='tustin'*)
 
 This function is for design of a first order high pass filter.
-$$
-F_{HP}(s) = 1 - F_{LP}(s) = \frac{s}{s+2\pi f}
-$$
+$$F_{HP}(s) = 1 - F_{LP}(s) = \frac{s}{s+2\pi f}$$
 
 - Parameters:
   - freq: frequency[Hz] of the high pass filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
   - out: instance of TransferFunction class of the high pass filter
@@ -921,22 +897,20 @@
 0.7609 z - 0.7609
 -----------------
    z - 0.5219
 
 dt = 0.001
 ```
 
-## 3.23. hpf2nd
+### 3.23. hpf2nd
 
 pylib_sakata.ctrl.**hpf2nd**(*freq, zeta, dt=None, method='tustin'*)
 
 This function is for design of a second order high pass filter.
-$$
-F_{HP^2}(s) = 1 - F_{LP^2}(s) = \frac{s^2+2\zeta (2\pi f)s}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}
-$$
+$$F_{HP^2}(s) = 1 - F_{LP^2}(s) = \frac{s^2+2\zeta (2\pi f)s}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}$$
 
 - Parameters:
   - freq: frequency[Hz] of the high pass filter
   - zeta1: damping of the high pass filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
@@ -956,22 +930,20 @@
 0.9358 z^2 - 1.3 z + 0.3641
 ---------------------------
   z^2 - 1.172 z + 0.4283
 
 dt = 0.001
 ```
 
-## 3.24. nf
+### 3.24. nf
 
 pylib_sakata.ctrl.**nf**(*freq, zeta, depth, dt=None, method='matched'*)
 
 This function is for design of notch filters.
-$$
-F_{notch}(s) = \frac{s^2+2d\zeta (2\pi f)s+(2\pi f)^2}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}
-$$
+$$F_{notch}(s) = \frac{s^2+2d\zeta (2\pi f)s+(2\pi f)^2}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}$$
 
 - Parameters:
   - freq: array of frequency[Hz] of the notch filters
   - zeta: array of damping of the notch filters
   - depth: array of depth of the notch filters (0 < depth < 1)
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'matched', set a method if dt > 0
@@ -990,22 +962,20 @@
 >>> ctrl.nf([100., 200., 300.], [0.02, 0.02, 0.02], [0.01, 0.01, 0.01], 0.001)
 array([TransferFunction(array([ 0.9876627 , -1.59787102,  0.9874145 ]), array([ 1.        , -1.59797428,  0.97518046]), 0.001),
        TransferFunction(array([ 0.97553399, -0.6027617 ,  0.97504375]), array([ 1.        , -0.60316088,  0.95097692]), 0.001),
        TransferFunction(array([0.96362486, 0.59532837, 0.96289858]), array([1.        , 0.59447771, 0.92737411]), 0.001)],
       dtype=object)
 ```
 
-## 3.25. pf
+### 3.25. pf
 
 pylib_sakata.ctrl.**pf**(*freq, zeta, k, phi, dt=None, method='tustin'*)
 
 This function is for design of peak filters ([resonant filters](https://ieeexplore.ieee.org/document/4291569)).
-$$
-F_{peak}(s) = \frac{k(s^2-\phi s)}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}
-$$
+$$F_{peak}(s) = \frac{k(s^2-\phi s)}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}$$
 
 - Parameters:
   - freq: array of frequency[Hz] of the peak filters
   - zeta: array of damping of the peak filters
   - k: array of peak width of the peak filters
   - phi: array of phase lead of the peak filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
@@ -1026,15 +996,15 @@
 >>> ctrl.pf([2., 3., 5.], [0.001, 0.001, 0.001], [-0.00025695, -0.00049616, 0.0003898], [860.21053991, 633.22924516, -1090.49879949], 0.001)
 array([TransferFunction(array([-0.00014643,  0.00051387, -0.00036745]), array([ 1.        , -1.99981696,  0.99997487]), 0.001),
        TransferFunction(array([-0.00033903,  0.00099221, -0.00065318]), array([ 1.        , -1.99960704,  0.9999623 ]), 0.001),
        TransferFunction(array([ 0.00060217, -0.00077938,  0.00017721]), array([ 1.        , -1.9989505 ,  0.99993719]), 0.001)],
       dtype=object)
 ```
 
-## 3.26. pfoptparam
+### 3.26. pfoptparam
 pylib_sakata.ctrl.**pfoptparam**(freq, zeta, depth, sysT)
 
 This function is for getting parameters of optimized peak filters ([resonant filters](https://ieeexplore.ieee.org/document/4291569)).
 
 - Parameters:
   - freq: array of frequency[Hz] of the peak filters
   - zeta: array of damping of the peak filters
@@ -1051,15 +1021,15 @@
 >>> Ps = ctrl.tf([1.], [2., 10., 0.])
 >>> Cs = ctrl.pid(10., 1., 10., 0.7, 2., 10., 0.)
 >>> ctrl.pfoptparam([2., 3., 5.], [0.001, 0.001, 0.001], [0.1, 0.1, 0.1], ctrl.feedback(Ps, Cs, sys='T'))
 The common pole-zeros of the zpk model have been deleted.
 ([2.0, 3.0, 5.0], [0.001, 0.001, 0.001], array([-0.00025695, -0.00049616,  0.0003898 ]), array([  860.21053991,   633.22924516, -1090.49879949]))
 ```
 
-## 3.27. pfopt
+### 3.27. pfopt
 
 pylib_sakata.ctrl.**pfopt**(*freq, zeta, depth, sysT, dt=None, method='tustin'*)
 
 This function is for design of optimized peak filters ([resonant filters](https://ieeexplore.ieee.org/document/4291569)).
 
 - Parameters:
   - freq: array of frequency[Hz] of the peak filters
@@ -1087,33 +1057,32 @@
 The common pole-zeros of the zpk model have been deleted.
 array([TransferFunction(array([ 0.0049857 , -0.00972818,  0.00474248]), array([ 1.        , -1.99981696,  0.99997487]), 0.001),
        TransferFunction(array([ 0.00740923, -0.01446026,  0.00705103]), array([ 1.        , -1.99960704,  0.9999623 ]), 0.001),
        TransferFunction(array([ 0.01227286, -0.02398427,  0.01171141]), array([ 1.        , -1.9989505 ,  0.99993719]), 0.001)],
       dtype=object)
 ```
 
-## 3.28. dob
+### 3.28. dob
 pylib_sakata.ctrl.**dob**(*freq, zeta, M, C, K, dt, nd = 0*)
 
 This function is for design of a discrete-time disturbance observer (DOB).
-$$
-\hat{d} = -z^{n_d} Q[z] u + Q[z] P^{-1}[z] y
-$$
+$$\hat{d} = -z^{-n_d} Q[z] u + Q[z] P^{-1}[z] y$$
+
 Here, it is defined that disturbance $d$ is injected in the system as plus sign.
 
 - Parameters:
   - freq: frequency[Hz] of the pole pair of the DOB
   - zeta: damping of the pole pair of the DOB
   - M: mass[kg] of the plant
   - C: viscosity[N/(m/s)] of the plant
   - K: stiffness[N/m] of the plant
   - dt: sampling time of the system
   - nd: sampling number of the dead-time of the system
 - Returns:
-  - DOBu: $z^{n_d} Q[z]$
+  - DOBu: $z^{-n_d} Q[z]$
   - DOBy: $Q[z] P^{-1}[z]$
 
 **Examples**
 ```python
 >>> DOBu, DOBy = ctrl.dob(5., 0.7, 1., 10., 0., 0.001, 1)
 >>> print(DOBu)
 
@@ -1128,15 +1097,15 @@
 970.3 z^2 - 1931 z + 960.7
 --------------------------
   z^2 - 1.956 z + 0.957
 
 dt = 0.001
 ```
 
-## 3.29. zpetc
+### 3.29. zpetc
 pylib_sakata.ctrl.**zpetc**(*Pz, dt, zerothr=0.99*)
 
 This function is for design of a zero phase error tracking controller ([ZPETC](https://engineering.purdue.edu/ME576/ZPETC_Tomizuka.pdf)).
 
 - Parameters:
   - Pz: instance of TransferFunction class of discrete-time LTI system
   - dt: sampling time of the system
@@ -1166,47 +1135,47 @@
 
 dt = 0.001
 
 >>> Nzpetc
 2
 ```
 
-## 3.30. filt
+### 3.30. filt
 pylib_sakata.ctrl.**filt**(*num, den, dt*)
 
 This function is to create transfer functions as rational expressions in $z^{-1}$ and to order the numerator and denominator terms in ascending powers of $z^{-1}$.
 
 - Parameters:
   - num: polynomial coefficients of the numerator of the discrete-time LTI model
   - den: polynomial coefficients of the denominator of the discrete-time LTI model
   - dt: sampling time of the discrete-time LTI model
 - Returns:
   - out: instance of TransferFunction class of ZPETC
 
-## 3.31. minreal
+### 3.31. minreal
 pylib_sakata.ctrl.**minreal**(*sys*)
 
 This function is to delete the common pole-zeros of the system.
 
 - Parameters:
   - sys: LTI model (StateSpace or TransferFunction or ZpkModel)
 - Returns:
   - out: LTI model whose the common pole-zeros were deleted
 
-## 3.32. makeprmset
+### 3.32. makeprmset
 pylib_sakata.ctrl.**makeprmset**(*path='.'*)
 
 This function is to create Cpp and header files of controller parameter sets
 
 - Parameters:
   - path: path to create Cpp and header files of controller parameter sets
 - Returns:
   - None
   
-## 3.33. defprmset
+### 3.33. defprmset
 pylib_sakata.ctrl.**defprmset**(*tfz, prmSetName, path='.', mode='a'*)
 
 - Parameters:
   - tfz: discrete time TransferFunction model
   - prmSetName: parameter set name of the following struct in Cpp
   - path: path to create Cpp and header files of controller parameter sets
   - mode: mode to open Cpp and header files
@@ -1232,17 +1201,17 @@
 	double	dA[4];
 	double	dB[4];
 	double	dInPre[3];
 	double	dOutPre[3];
 } TF3_INF;						// 3rd order TF information
 ```
 
-# 4. pylib_sakata.fft
+## 4. pylib_sakata.fft
 
-## 4.1. FreqResp
+### 4.1. FreqResp
 
 class pylib_sakata.fft.**FreqResp**(*freq, resp, dt=0*)
 
 - Parameters:
   - freq: 1-D array frequency data [Hz]
   - resp: 1-D array frequency response data [complex data]
   - dt: sampling time (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
@@ -1277,15 +1246,15 @@
 
 - \__**rtruediv**__(*other*)
 	Right divide two FRDs.
 
 - \__**pow**__(*other*)
 	A FRD to the power of x.
 
-## 4.2. fft
+### 4.2. fft
 
 pylib_sakata.fft.**fft**(*data, dt*)
 
 This function is for calculating FFT from 1-D array data.
 
 - Parameters:
   - data: 1-D array time response data
@@ -1302,25 +1271,25 @@
 >>> x = np.sin(2*np.pi*10.0*t) + np.sin(2*np.pi*50.0*t)
 >>> fft.fft(x, dt)
 (array([0.00000000e+00, 1.00010001e-01, 2.00020002e-01, ...,
        9.99799980e+02, 9.99899990e+02, 1.00000000e+03]), array([3.93463040e-17, 2.39600781e-06, 4.79322523e-06, ...,
        7.19286425e-06, 4.79322523e-06, 2.39600781e-06]))
 ```
 
-## 4.3. fft_ave
+### 4.3. fft_ave
 
 pylib_sakata.fft.**fft_ave**(*data, dt, windivnum=4, overlap=0.5*)
 
 This function is for calculating averaged FFT from 1-D array data.
 
 - Parameters:
   - data: 1-D array time response data
   - dt: sampling time of the time response data
   - windivnum: number of windows to divide the time response data
-  - overlap: overlap retio divided time response data (0 <= overlap < 1)
+  - overlap: overlap ratio divided time response data (0 <= overlap < 1)
 - Returns:
   - freq_data: 1-D array frequency data [Hz]
   - fft_data: 1-D array FFT data
 
 **Examples**
 ```python
 import numpy as np
@@ -1329,27 +1298,27 @@
 >>> x = np.sin(2*np.pi*10.0*t) + np.sin(2*np.pi*50.0*t)
 >>> fft.fft_ave(x, dt, 4, 0.5)
 (array([0.00000000e+00, 4.88519785e-01, 9.77039570e-01, ...,
        9.99022960e+02, 9.99511480e+02, 1.00000000e+03]), array([5.33388114e-05, 5.46444944e-05, 5.85999322e-05, ...,
        6.53498409e-05, 5.85999322e-05, 5.46444944e-05]))
 ```
 
-## 4.4. tfestimate
+### 4.4. tfestimate
 
 pylib_sakata.fft.**tfestimate**(*x, y, freq, dt, windivnum=4, overlap=0.5*)
 
 This function is for system identification from input and output time response data.
 
 - Parameters:
   - x: 1-D array time response data of input
   - y: 1-D array time response data of output
   - freq: 1-D array frequency data [Hz]
   - dt: sampling time of the time response data
   - windivnum: number of windows to divide the time response data
-  - overlap: overlap retio divided time response data (0 <= overlap < 1)
+  - overlap: overlap ratio divided time response data (0 <= overlap < 1)
 - Returns:
   - freqresp: instance of FreqResp class
   - coh: 1-D array coherence data
 
 **Examples**
 ```python
 >>> import numpy as np
@@ -1367,15 +1336,15 @@
 >>> fft.tfestimate(u, y, freq, dt)
 (array([-0.11586071-1.49076948e-01j, -0.11590257-1.49078279e-01j,
        -0.11594446-1.49079611e-01j, ..., -0.13155661-1.45847229e-01j,
        -0.14201211-1.03211830e-01j, -0.15745492-1.88460358e-14j]), array([0.77271576, 0.77244166, 0.7721674 , ..., 0.23080322, 0.32843388,
        0.43848208]))
 ```
 
-## 4.5. frdresize
+### 4.5. frdresize
 
 pylib_sakata.fft.**frdresize**(*freqresp, freq*)
 
 This function is for resizing a frequency response data.
 
 - Parameters:
   - freqresp: instance of FreqResp class
@@ -1395,57 +1364,57 @@
 freq = array([   1.            1.00069108    1.00138264 ...  998.61926487  999.30939397
  1000.        ])
 resp = array([-5.10821217e-03-5.65218353e-02j -5.10244172e-03-5.64813436e-02j
  -5.09666728e-03-5.64408239e-02j ... -5.64622394e-09-5.31301950e-05j
  -5.63759203e-09-5.30909366e-05j -5.62895416e-09-5.30516511e-05j])
 ```
 
-## 4.6. frdsim
+### 4.6. frdsim
 
 pylib_sakata.fft.**frdsim**(*freqresp, x, dt*)
 
 This function is for simulation steady time response data when a time-domain data is input to a system written by frequency response data.
-$$
-y(t) = \text{ifft}(\text{FreqResp}(\omega)\times\text{fft}(u(t)))
-$$
+$$y(t) = \text{ifft}(\text{FreqResp}(\omega)\times\text{fft}(u(t)))$$
 
 - Parameters:
   - freqresp: instance of FreqResp class
   - x: 1-D array time response data of input
   - dt: sampling time of the time response data
 - Returns:
+  - t: 1-D array time data [s]
   - y: 1-D array time response data of output
 
 **Examples**
 ```python
 >>> import numpy as np
 >>> freq = np.logspace(np.log10(1.), np.log10(1000.), 100, base=10)
 >>> Sys_tf = ctrl.tf([1., 2.], [3., 4., 5.])
 >>> freqresp = ctrl.sys2frd(Sys_tf, freq)
 >>> dt = 0.001
 >>> t = np.linspace(0.0, 10., int(10./dt))
 >>> x = np.sin(2*np.pi*10.0*t) + np.sin(2*np.pi*50.0*t)
 >>> fft.frdsim(freqresp, x, dt)
-array([-0.00635301, -0.00630568, -0.00612106, ..., -0.00610225,
-       -0.0062943 , -0.00634922])
+(array([0.000e+00, 1.000e-03, 2.000e-03, ..., 9.996e+00, 9.997e+00,
+       9.998e+00]), array([-0.00635301, -0.00630568, -0.00612106, ..., -0.00610225,
+       -0.0062943 , -0.00634922]))
 ```
 
-# 5. pylib_sakta.meas
+## 5. pylib_sakata.meas
 
-## 5.1. MeasData
+### 5.1. MeasData
 
-class pylib_sakata.meas.**MeasData**(*time, list, value, time, dt*)
+class pylib_sakata.meas.**MeasData**(*list, value, time, dt*)
 
 - Parameters:
-  - dataList: array of data list (*str*)
-  - dataValue: array of data value
+  - list: array of data list (*str*)
+  - value: array of data value
   - time: 1-D array time data [s]
   - dt: sampling time of the time response data
 
-## 5.2. getcsvdata
+### 5.2. getcsvdata
 
 pylib_sakata.meas.**getcsvdata**(*filePath*)
 
 This function is for getting measurement data from a csv file.
 
 - Parameters:
   - filePath: csv file path of measurement file
@@ -1453,15 +1422,15 @@
   - instance of MeasData class
 
 **Examples**
 ```python
 measdata = meas.getcsvdata('data\001-inject.csv')
 ```
 
-## 5.3. gettxtdata
+### 5.3. gettxtdata
 
 pylib_sakata.meas.**gettxtdata**(*filePath*)
 
 This function is for getting measurement data from a txt file.
 
 - Parameters:
   - filePath: txt file path of measurement file
@@ -1469,15 +1438,15 @@
   - instance of MeasData class
 
 **Examples**
 ```python
 measdata = meas.gettxtdata('data\001-inject.txt')
 ```
 
-## 5.4. getmatdata
+### 5.4. getmatdata
 
 pylib_sakata.meas.**getmatdata**(*filePath*)
 
 This function is for getting measurement data from a mat file.
 
 - Parameters:
   - filePath: mat file path of measurement file
@@ -1485,52 +1454,52 @@
   - instance of MeasData class
 
 **Examples**
 ```python
 measdata = meas.getmatdata('data\001-inject.mat')
 ```
 
-## 5.5. getdata
+### 5.5. getdata
 
 pylib_sakata.meas.**getdata**(*filePath*)
 
 This function is for getting measurement data from a file.
 
 - Parameters:
   - filePath: file path of measurement file (.csv, .txt, and .mat are supported.)
 - Returns:
   - instance of MeasData class
 
 **Examples**
 ```python
-measdata = meas.getmatdata('data\001-inject.csv')
+measdata = meas.getdata('data\001-inject.csv')
 ```
 ```python
-measdata = meas.getmatdata('data\001-inject.txt')
+measdata = meas.getdata('data\001-inject.txt')
 ```
 ```python
-measdata = meas.getmatdata('data\001-inject.mat')
+measdata = meas.getdata('data\001-inject.mat')
 ```
 
-## 5.6. getdataindex
+### 5.6. getdataindex
 
 pylib_sakata.meas.**getdataindex**(*measdata, dataName*)
 
 - Parameters:
   - measdata: instance of MeasData class
   - dataName: data name
 - Returns:
   - index: index of dataName
 
 **Examples**
 ```python
 index = meas.getdataindex(measdata, 'ServoOut')
 ```
 
-## 5.7. measdata2frd
+### 5.7. measdata2frd
 
 pylib_sakata.meas.**measdata2frd**(*filePath, inputName, outputName, flagName, freq, inputGain=1.0, outputGain=1.0, windivnum=4, overlap=0.5*)
 
 This function is for system identification from input and output time response data of measurement file.
 
 - Parameters:
   - filePath: file path of measurement file (.csv, .txt, and .mat are supported.)
@@ -1538,74 +1507,136 @@
   - outputName: output data name in the measurement file
   - flagName: flag data name in the measurement file
   - freq: 1-D array frequency data [Hz]
   - inputGain: inputdata gain (Optional), Default: 1.0, unit of input can be fixed by this parameter.
   - outputGain: outputdata gain (Optional), Default: 1.0, unit of output can be fixed by this parameter.
   - dt: sampling time of the time response data
   - windivnum: number of windows to divide the time response data
-  - overlap: overlap retio divided time response data (0 <= overlap < 1)
+  - overlap: overlap ratio divided time response data (0 <= overlap < 1)
 - Returns:
   - freqresp: instance of FreqResp class
   - coh: 1-D array coherence data
 
 **Examples**
 ```python
 import numpy as np
 freq = np.logspace(np.log10(1.), np.log10(1000.), 10000, base=10)
 freqresp, coh = measdata2frd('data\001-inject.csv', 'ServoOut', 'PosErrUm', 'FlagNoise', freq, 1., 1.e-6)
 ```
 
-# 6. pylib_sakata.traj
+## 6. pylib_sakata.traj
 
-## 6.1. TrajInf
+### 6.1. TrajInf
 
 class pylib_sakata.traj.**TrajInf**(*time, pos, vel, acc, T, dt*)
 
 - Parameters:
   - time: 1-D array time data [s]
   - pos: 1-D array position trajectory data [m]
   - vel: 1-D array velocity trajectory data [m/s]
   - acc: 1-D array acceleration trajectory data [m/s^2]
   - T: moving time [s]
   - dt: sampling time of the trajectory data
 
-## 6.2. traj4th
+### 6.2. traj3rd
 
-pylib_sakata.traj.**traj4th**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
+pylib_sakata.traj.**traj3rd**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)  
+
+This function is for generation of a 3rd order polynomial trajectory.
+
+- Parameters:
+  - posStart: start position of the trajectory
+  - posStep: step position of the trajectory
+  - velMax: maximum of velocity of the trajectory
+  - accAve: average of accelation (= decelation) of the trajectory
+  - dt: sampling time of the trajectory data.
+  - Tstay: time after the step moving
+- Returns:
+  - out: instance of TrajInf class of the 3rd order polynomial trajectory
+
+**Examples**
+```python
+traj = traj.traj3rd(0, 100, 100, 200, 0.001, 0.5)
+```
+
+### 6.3. traj3rd2
+
+pylib_sakata.traj.**traj3rd2**(*posStart, posStep, velMax, accAve, jerkRatio, dt, Tstay=0*)  
+
+This function is for generation of a 3rd order polynomial trajectory as trapezoidal accelaration trajectory.
+
+- Parameters:
+  - posStart: start position of the trajectory
+  - posStep: step position of the trajectory
+  - velMax: maximum of velocity of the trajectory
+  - accAve: average of accelation (= decelation) of the trajectory
+  - jerkRatio: ratio of jerk time per accelaration time (0 < jerkRatio <= 0.5)
+  - dt: sampling time of the trajectory data.
+  - Tstay: time after the step moving
+- Returns:
+  - out: instance of TrajInf class of the 3rd order polynomial trajectory
+
+**Examples**
+```python
+traj = traj.traj3rd2(0, 100, 100, 200, 0.001, 0.2, 0.5)
+```
+
+### 6.4. traj4th
+
+pylib_sakata.traj.**traj4th**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)  
+pylib_sakata.traj.**traj4th2**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
 
 This function is for generation of a 4th order polynomial trajectory.
 
 - Parameters:
   - posStart: start position of the trajectory
   - posStep: step position of the trajectory
   - velMax: maximum of velocity of the trajectory
   - accAve: average of accelation (= decelation) of the trajectory
   - dt: sampling time of the trajectory data.
+  - Tstay: time after the step moving
 - Returns:
   - out: instance of TrajInf class of the 4th order polynomial trajectory
 
 **Examples**
 ```python
 traj = traj.traj4th(0, 100, 100, 200, 0.001, 0.5)
+```
 
-fig = plot.makefig()
-ax1 = fig.add_subplot(311)
-ax2 = fig.add_subplot(312)
-ax3 = fig.add_subplot(313)
-plot.plot_xy(ax1, traj.time, traj.pos, ylabel='[m]', legend=['Pos'], title='TrajInf')
-plot.plot_xy(ax2, traj.time, traj.vel, ylabel='[m/s]', legend=['Vel'])
-plot.plot_xy(ax3, traj.time, traj.acc, xlabel='Time [s]', ylabel='[m/s^2]', legend=['Acc'])
-plot.savefig('time_traj.png')
+### 6.5. trajSinStep
+
+pylib_sakata.traj.**trajSinStep**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
+pylib_sakata.traj.**trajSinStep2**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
+pylib_sakata.traj.**trajSinStep3**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
+
+This function is for generation of a trajectory based on sine waves.
+
+- Parameters:
+  - posStart: start position of the trajectory
+  - posStep: step position of the trajectory
+  - velMax: maximum of velocity of the trajectory
+  - accAve: average of accelation (= decelation) of the trajectory
+  - dt: sampling time of the trajectory data.
+  - Tstay: time after the step moving
+- Returns:
+  - out: instance of TrajInf class of the trajectory based on sine waves
+
+**Examples**
+```python
+traj = traj.SinStep(0, 100, 100, 200, 0.001, 0.5)
 ```
 
-<img src="figure\time_traj.png" alt="vscode_disp" style="zoom: 80%;" />
+The comparison of these trajectories under the specification: posStep = 1, velMax = 1, accAve = 2 is shown as follows.
+
+<img src="figure\time_traj.png" alt="vscode_disp" style="zoom: 15%;" />
+<img src="figure\time_fft.png" alt="vscode_disp" style="zoom: 40%;" />
 
-# 7. pylib_sakata.plot
+## 7. pylib_sakata.plot
 
-## 7.1. plot_xy
+### 7.1. plot_xy
 
 pylib_sakata.plot.**plot_xy**(*ax, x, y, styl='-', col='b', width=1.5, alpha=1.0, xrange=None, yrange=None, xlabel=None, ylabel=None, legend=None, loc='best', title=None, xscale='linear', yscale='linear', labelouter=True*)
 
 This function is for drawing a 2-D figure from x and y data. You can select xy scale in linear type, log type and so on.
 
 - Parameters:
   - ax: handle of axis
@@ -1642,15 +1673,15 @@
 ax2 = fig2.add_subplot(312)
 ax3 = fig2.add_subplot(313)
 plot.plot_xy(ax1, fft_axis, chirp_fft, '-', 'm', 1.5, 1.0, freqrange, [0, 1.0], ylabel='Input [N]', legend=['Chirp'], title='Power spectrum density', xscale='log')
 plot.plot_xy(ax2, fft_axis, u_fft, '-', 'b', 1.5, 1.0, freqrange, [0, 0.1], ylabel='Input [N]', legend=['Servo Out'], xscale='log')
 plot.plot_xy(ax3, fft_axis, y_fft*1.0e6, '-', 'b', 1.5, 1.0, freqrange, [0, 20], xlabel='Frequency [Hz]', ylabel='Output [um]', legend=['Position'], xscale='log')
 ```
 
-## 7.2. plot_tf
+### 7.2. plot_tf
 
 pylib_sakata.plot.**plot_tf**(*ax_mag, ax_phase, sys, freq, styl='-', col='b', width=1.5, alpha=1.0, freqrange=None, magrange=None, legend=None, loc='best', title=None, labelouter=True*)
 
 This function is for drawing a Bode diagram from a LTI model.
 
 - Parameters:
   - ax_mag: handle of magnitude axis
@@ -1683,25 +1714,24 @@
 fig2 = plot.makefig()
 ax_mag = fig2.add_subplot(211)
 ax_phase = fig2.add_subplot(212)
 plot.plot_tf(ax_mag, ax_phase, T, freq, '-', 'm', 1.5, 1.0, title='Frequency response of complementary sensitivity function')
 plot.plot_tf(ax_mag, ax_phase, Tn, freq, '--', 'b', 1.5, 1.0, [1, 1000], [-60, 10], legend=['Measurement','Model'])
 ```
 
-## 7.3. plot_tffrd
+### 7.3. plot_tffrd
 
 pylib_sakata.plot.**plot_tffrd**(*ax_mag, ax_phase, freqresp, styl='-', col='b', width=1.5, alpha=1.0, freqrange=None, magrange=None, legend=None, loc='best', title=None, labelouter=True, ax_coh=None, coh=None*)
 
 This function is for drawing a Bode diagram from a frequency response data.
 
 - Parameters:
   - ax_mag: handle of magnitude axis
   - ax_phase: handle of phase axis, if you set as None, phase axis is skipped.
   - freqresp: instance of FreqResp class
-  - freq: 1-D array frequency data [Hz]
   - styl: line style (Optional), Default: '-', Select in '-' (solid), '--' (dashed), '.' (dotted), '-.' (dashdot)
   - col: line color (Optional), Default: 'b' (blue)
   - width: line width (Optional), Default: 1.5
   - alpha: transmittance of line, Default: 1.0, set from 0 to 1.0
   - freqrange: plot range of frequency-axis (Optional), Default: None, set as [freqmin, freqmax]
   - magrange: plot range of magnitude-axis (Optional), Default: None, set as [magmin, magmax]
   - legend: legend of data, Default: None, set a list of strings data
@@ -1734,15 +1764,15 @@
 fig3 = plot.makefig()
 ax_mag = fig2.add_subplot(211)
 ax_phase = fig2.add_subplot(212)
 plot.plot_tffrd(ax_mag, ax_phase, T_frd, '-', 'm', 1.5, 1.0, title='Frequency response of complementary sensitivity function')
 plot.plot_tffrd(ax_mag, ax_phase, Tn_frd, '--', 'b', 1.5, 1.0, [1, 1000], [-60, 10], legend=['Measurement','Model'])
 ```
 
-## 7.4. plot_nyquist
+### 7.4. plot_nyquist
 
 pylib_sakata.plot.**plot_nyquist**(*ax, freqresp, styl='-', col='b', width=1.5, alpha=1.0, xrange=None, yrange=None, legend=None, loc='best', title=None, labelouter=True*)
 
 This function is for drawing a Nyquist diagram from a frequency response data of a open loop system
 
 - Parameters:
   - ax: handle of axis
@@ -1764,15 +1794,15 @@
 ```python
 fig = plot.makefig()
 ax = fig.add_subplot(111)
 plot.plot_nyquist(ax, G_frd, '-', 'm', 1.5, 1.0, title='Nyquist Diagram')
 plot.plot_nyquist(ax, Gn_frd, '--', 'b', 1.5, 1.0, legend=['Measurement','Model'])
 ```
 
-## 7.5. plot_nyquist_assistline
+### 7.5. plot_nyquist_assistline
 
 pylib_sakata.plot.**plot_nyquist_assistline**(*ax*)
 
 This function is for drawing assist line of a Nyquist diagram.
 
 - Parameters:
   - ax: handle of axis
@@ -1780,32 +1810,33 @@
   - None
 
 **Examples**
 ```python
 plot.plot_nyquist_assistline(ax)
 ```
 
-## 7.6. makefig
+### 7.6. makefig
 
-pylib_sakata.plot.**makefig**(dpi=100, popwin=False)
+pylib_sakata.plot.**makefig**(dpi=100, figsize=(6, 4), popwin=False)
 
 This function will make a new figure handle.
 
 - Parameters:
   - dpi: dot per inch of figure (Optional), Default: 100
+  - figsize: set figure size (Optional), Default: (6, 4) which means 600x400 pixels
   - popwin: switch to fix the popup window of the figure (Optional), Default: False
 - Returns:
   - fig: figure handle
 
 **Examples**
 ```python
 fig = plot.makefig()
 ```
 
-## 7.7. savefig
+### 7.7. savefig
 
 pylib_sakata.plot.**savefig**(*figName*)
 
 This function will save a current figure.
 
 - Parameters:
   - figName: figure name for saving a current figure, set strings data
@@ -1813,43 +1844,41 @@
   - None
 
 **Examples**
 ```python
 plot.savefig('freq_P.png')
 ```
 
-## 7.8. showfig
+### 7.8. showfig
 
 pylib_sakata.plot.**showfig**()
 
 This function will call matplotlib.pyplot.show()
 
 **Examples**
 ```python
 showfig()
 ```
 
-# 8. pylib_sakata.init
+## 8. pylib_sakata.init
 
-## 8.1. close_all
+### 8.1. close_all
 
 pylib_sakata.init.**close_all**()
 
 This function is for closing current opened figures.
 
 **Examples**
 ```python
 close_all()
 ```
 
-## 8.2. clear_all
+### 8.2. clear_all
 
 pylib_sakata.init.**clear_all**()
 
 This function is for deleting all defined variables.
 
 **Examples**
 ```python
 clear_all()
 ```
-
-
```

### Comparing `pylib-sakata-0.1.9/README.md` & `pylib-sakata-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-pylib-sakata User's Manual version-0.1.9
+pylib-sakata User's Manual version-0.2.0
 ===
 
-<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
-
 <!-- code_chunk_output -->
 
-- [pylib-sakata User's Manual version-0.1.9](#pylib-sakata-users-manual-version-019)
 - [1. Introduction](#1-introduction)
 - [2. Environment Setup](#2-environment-setup)
   - [2.1. Installation of Python](#21-installation-of-python)
   - [2.2. Installation  of required Python libraries](#22-installation--of-required-python-libraries)
   - [2.3. Installation of pylib-sakata](#23-installation-of-pylib-sakata)
   - [2.4. Installation of IDE for Python](#24-installation-of-ide-for-python)
     - [2.4.1. Visual Studio Code (VSCode)](#241-visual-studio-code-vscode)
@@ -19,15 +16,15 @@
       - [2.4.2.1. Installation of Spyder](#2421-installation-of-spyder)
       - [2.4.2.2. Initial setting of Spyder](#2422-initial-setting-of-spyder)
     - [2.4.3. PyCharm](#243-pycharm)
       - [2.4.3.1. Installation of PyCharm](#2431-installation-of-pycharm)
       - [2.4.3.2. Initial setting of PyCharm](#2432-initial-setting-of-pycharm)
     - [2.4.4. Comparison between  VSCode and Spyder and PyCharm](#244-comparison-between--vscode-and-spyder-and-pycharm)
   - [2.5. Getting started](#25-getting-started)
-- [3. pylib_sakata.ctrl](#3-pylib_sakatactrl)
+- [3. pylib\_sakata.ctrl](#3-pylib_sakatactrl)
   - [3.1. ZpkModel](#31-zpkmodel)
   - [3.2. tf](#32-tf)
   - [3.3. ss](#33-ss)
   - [3.4. zpk](#34-zpk)
   - [3.5. tf2ss](#35-tf2ss)
   - [3.6. tf2zpk](#36-tf2zpk)
   - [3.7. ss2tf](#37-ss2tf)
@@ -53,57 +50,60 @@
   - [3.27. pfopt](#327-pfopt)
   - [3.28. dob](#328-dob)
   - [3.29. zpetc](#329-zpetc)
   - [3.30. filt](#330-filt)
   - [3.31. minreal](#331-minreal)
   - [3.32. makeprmset](#332-makeprmset)
   - [3.33. defprmset](#333-defprmset)
-- [4. pylib_sakata.fft](#4-pylib_sakatafft)
+- [4. pylib\_sakata.fft](#4-pylib_sakatafft)
   - [4.1. FreqResp](#41-freqresp)
   - [4.2. fft](#42-fft)
-  - [4.3. fft_ave](#43-fft_ave)
+  - [4.3. fft\_ave](#43-fft_ave)
   - [4.4. tfestimate](#44-tfestimate)
   - [4.5. frdresize](#45-frdresize)
   - [4.6. frdsim](#46-frdsim)
-- [5. pylib_sakta.meas](#5-pylib_saktameas)
+- [5. pylib\_sakata.meas](#5-pylib_sakatameas)
   - [5.1. MeasData](#51-measdata)
   - [5.2. getcsvdata](#52-getcsvdata)
   - [5.3. gettxtdata](#53-gettxtdata)
   - [5.4. getmatdata](#54-getmatdata)
   - [5.5. getdata](#55-getdata)
   - [5.6. getdataindex](#56-getdataindex)
   - [5.7. measdata2frd](#57-measdata2frd)
-- [6. pylib_sakata.traj](#6-pylib_sakatatraj)
+- [6. pylib\_sakata.traj](#6-pylib_sakatatraj)
   - [6.1. TrajInf](#61-trajinf)
-  - [6.2. traj4th](#62-traj4th)
-- [7. pylib_sakata.plot](#7-pylib_sakataplot)
-  - [7.1. plot_xy](#71-plot_xy)
-  - [7.2. plot_tf](#72-plot_tf)
-  - [7.3. plot_tffrd](#73-plot_tffrd)
-  - [7.4. plot_nyquist](#74-plot_nyquist)
-  - [7.5. plot_nyquist_assistline](#75-plot_nyquist_assistline)
+  - [6.2. traj3rd](#62-traj3rd)
+  - [6.3. traj3rd2](#63-traj3rd2)
+  - [6.4. traj4th](#64-traj4th)
+  - [6.5. trajSinStep](#65-trajsinstep)
+- [7. pylib\_sakata.plot](#7-pylib_sakataplot)
+  - [7.1. plot\_xy](#71-plot_xy)
+  - [7.2. plot\_tf](#72-plot_tf)
+  - [7.3. plot\_tffrd](#73-plot_tffrd)
+  - [7.4. plot\_nyquist](#74-plot_nyquist)
+  - [7.5. plot\_nyquist\_assistline](#75-plot_nyquist_assistline)
   - [7.6. makefig](#76-makefig)
   - [7.7. savefig](#77-savefig)
   - [7.8. showfig](#78-showfig)
-- [8. pylib_sakata.init](#8-pylib_sakatainit)
-  - [8.1. close_all](#81-close_all)
-  - [8.2. clear_all](#82-clear_all)
+- [8. pylib\_sakata.init](#8-pylib_sakatainit)
+  - [8.1. close\_all](#81-close_all)
+  - [8.2. clear\_all](#82-clear_all)
 
 <!-- /code_chunk_output -->
 
-# 1. Introduction
+## 1. Introduction
 
-The pylib-sakata package is a set of python classes and functions that make the python-control package more convenient. This package provide practical level's tools to design controls and  to analysis of performance and stability of SISO LTI systems. These development environments are available on free.
+The pylib-sakata package is a set of python classes and functions that make the python-control package more convenient. This package provides practical level's tools to design controls and  to analysis of performance and stability of SISO LTI systems. These development environments are available on free.
 
-# 2. Environment Setup
+## 2. Environment Setup
 
-## 2.1. Installation of Python
+### 2.1. Installation of Python
 Python installation exe file can be downloaded [HERE](https://www.python.org/downloads/) for Windows. Check "Add Python 3.x to PATH" when you install Python.
 
-## 2.2. Installation  of required Python libraries
+### 2.2. Installation  of required Python libraries
 
 The pylib-sakata package requires [numpy](http://www.numpy.org), [scipy](http://www.scipy.org), [matplotlib](https://matplotlib.org), [pandas](https://pandas.pydata.org/), and [python-control](https://github.com/python-control/python-control). In addition, some routines require the [slycot](https://github.com/python-control/Slycot) library in order to implement more advanced features. 
 First, pip should be upgraded by the following command on the command prompt for Windows OS.
 ```shell
 python -m pip install --upgrade pip
 ```
 For Linux OS, pip can be upgraded by the following command on the shell.
@@ -116,89 +116,89 @@
 pip install scipy
 pip install matplotlib
 pip install pandas
 pip install control
 ```
 If those libraries can not be installed, please use pip3 instead of pip.
 
-## 2.3. Installation of pylib-sakata
+### 2.3. Installation of pylib-sakata
 
 The [pylib-sakata](https://github.com/Koichi-Sakata/pylib_sakata) package can be installed using pip using pip as following on the command prompt or on the shell.
 
 ```shell
 pip install pylib-sakata
 ```
 
-## 2.4. Installation of IDE for Python
+### 2.4. Installation of IDE for Python
 
 There are three recommended IDEs.
 
-### 2.4.1. Visual Studio Code (VSCode)
+#### 2.4.1. Visual Studio Code (VSCode)
 Although VSCode is actually an editor, it is available as Python IDE due to extensions. It is recommended to install it easily because of the versatility of extensions. The following figure shows VSCode IDE window.
 
 <img src="figure\vscode_disp.png" alt="vscode_disp" style="zoom: 33%;" />
 
-#### 2.4.1.1. Installation of VSCode
+##### 2.4.1.1. Installation of VSCode
 The latest version of VSCode installation exe file can be downloaded [HERE](https://code.visualstudio.com/) for Windows OS.
 For Linux OS, VSCode can be installed by the following command on the shell.
 ```shell
 $ sudo apt update 
 $ sudo apt install code
 ```
 
-#### 2.4.1.2. Initial setting of VSCode
+##### 2.4.1.2. Initial setting of VSCode
 1. Install Python extension for Visual Studio Code from extensions in the activity bar on the left side.
 1. Command (Ctrl+Shift+P) to open the command palette.
 1. Select your installed python.exe on  "Python: select interpreter".
 
-### 2.4.2. Spyder
+#### 2.4.2. Spyder
 Spyder is an IDE like MATLAB. If you are used to MATLAB, this IDE is recommended. The following figure shows Spyder IDE window.
 
 <img src="figure\spyder_disp.png" alt="spyder_disp" style="zoom: 33%;" />
 
-#### 2.4.2.1. Installation of Spyder
+##### 2.4.2.1. Installation of Spyder
 The latest version of Spyder installation exe file can be downloaded [HERE](https://www.spyder-ide.org/) for Windows OS.
 For Linux OS, Spyder can be installed by the following command on the shell.
 
 ```shell
 $ sudo apt update 
 $ sudo apt install spyder3
 ```
 
-#### 2.4.2.2. Initial setting of Spyder
+##### 2.4.2.2. Initial setting of Spyder
 1. Open Tools>Preferences>Python interpreter.
 1. Check "Use the following Python interpreter."
 1. Enter the path of your installed python.exe.
 1. Install spyder-kernels for your python version by the following command `pip install spyder-kernels==2.0.*` on the command prompt or on the shell.
 1. Reboot your PC.
 
-### 2.4.3. PyCharm
+#### 2.4.3. PyCharm
 Professional version is charged. Community version is free. Community version is enough for control system development. The following figure shows PyCharm window.
 
 <img src="figure\pycharm_disp.png" alt="spyder_disp" style="zoom: 33%;" />
 
-#### 2.4.3.1. Installation of PyCharm
+##### 2.4.3.1. Installation of PyCharm
 The latest version of PyCharm installation exe file can be downloaded [HERE](https://www.jetbrains.com/pycharm/download/). 
 
-#### 2.4.3.2. Initial setting of PyCharm
+##### 2.4.3.2. Initial setting of PyCharm
 It is not necessary.
 
-### 2.4.4. Comparison between  VSCode and Spyder and PyCharm
+#### 2.4.4. Comparison between  VSCode and Spyder and PyCharm
 
 |                    |        VSCode       |      Spyder       |     PyCharm       |
 | ------------------ | :-----------------: | :---------------: | :---------------: |
 | Cost               |        Free         |       Free        |    Free/Paid      |
 | Boot time          |        Fast         |       Slow        |       Normal      |
 | Processing speed   |        Fast         |       Normal      |       Normal      |
 | REPL mode          | need to switch REPL terminal  | Available | Available |
 | Variable Explorer  | Available on Jupyter terminal | Available (Class variables are invisible.) | Available |
 
 Spyder is more suitable than VSCode for early debugging. On the other hand, VSCode is stress-free than Spyder for late debugging you do not need to check inter states of variables. PyCharm is generally well-balanced. My recommendation is PyCharm.
 
-## 2.5. Getting started
+### 2.5. Getting started
 The pylib-sakata package can be imported as follows.
 ```python
 >>> import pylib_sakata
 ```
 This package consists of six modules as follows.
 1. **ctrl**: to design controllers and filters
 1. **fft**: to analysis FFT
@@ -215,17 +215,17 @@
 >>> from pylib_sakata import traj
 >>> from pylib_sakata import plot
 >>> from pylib_sakata import init
 ```
 
 Example codes are [HERE](https://github.com/Koichi-Sakata/pylib_sakata/tree/main/example).
 
-# 3. pylib_sakata.ctrl
+## 3. pylib_sakata.ctrl
 
-## 3.1. ZpkModel
+### 3.1. ZpkModel
 
 class pylib_sakata.ctrl.**ZpkModel**(*z, p, k, dt=0*)
 
 - Parameters:
   - z: zeros array of the LTI model
   - p: poles array of the LTI model
   - k: gain of the LTI model. Note: the gain is not system dc gain but coefficient of monic polynomials. This is different from the definition of dc gain in TransferFunction class.
@@ -282,15 +282,15 @@
 - \__**pow**__(*other*)
 	A zpk model to the power of x.
 
 - **feedback**(*other=1, sys='S'*)
 	Calculate the feedback system that consist of two zpk model (P: self and C: other).
 	sys: FB type (Optional), Default: 'S', Set in 'S': sensitivity function, 'T': complementary sensitivity function, 'SP': response from input disturbance to output
 
-## 3.2. tf
+### 3.2. tf
 
 pylib_sakata.ctrl.**tf**(*num, den, dt=0*)
 
 This function calls **tf** function in control library.
 
 - Parameters:
   - num: polynomial coefficients of the numerator of the LTI model
@@ -304,15 +304,15 @@
 >>> print(ctrl.tf([1., 2.], [3., 4., 5.]))
 
      s + 2
 ---------------
 3 s^2 + 4 s + 5
 ```
 
-## 3.3. ss
+### 3.3. ss
 
 pylib_sakata.ctrl.**ss**(*A, B, C, D, dt=0*)
 
 This function calls **ss** function in control library.
 
 - Parameters:
   - A, B, C, D: state space matrices
@@ -330,15 +330,15 @@
      [7.]]
 
 C = [[6. 8.]]
 
 D = [[9.]]
 ```
 
-## 3.4. zpk
+### 3.4. zpk
 
 pylib_sakata.ctrl.**zpk**(*z, p, k, dt=0*)
 
 - Parameters:
   - A, B, C, D: state space matrices
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
 - Returns:
@@ -349,21 +349,21 @@
 >>> ctrl.zpk([-1., -2.], [-3., -4., -5.], 2.)
 
       (s+1)(s+2)
 2 * ---------------
     (s+3)(s+4)(s+5)
 ```
 
-## 3.5. tf2ss
+### 3.5. tf2ss
 
-pylib_sakata.ctrl.**tf2ss**(*tf, form='reachable'*)
+pylib_sakata.ctrl.**tf2ss**(*tf, form=None*)
 
 - Parameters:
   - tf: instance of TransferFunction class
-  - form: canonical form (Optional), Default: reachable. You can select the canonical form in reachable, observable, and modal.
+  - form: canonical form (Optional), you can select the canonical form in 'reachable', 'observable', and 'modal'.
 - Returns:
   - out: instance of StateSpace class
 
 **Examples**
 ```python
 >>> Sys_tf = ctrl.tf([1., 2.], [3., 4., 5.])
 >>> print(ctrl.tf2ss(Sys_tf))
@@ -374,15 +374,15 @@
      [0.]]
 
 C = [[0.33333333 0.66666667]]
 
 D = [[0.]]
 ```
 
-## 3.6. tf2zpk
+### 3.6. tf2zpk
 
 pylib_sakata.ctrl.**tf2zpk**(*tf*)
 
 - Parameters:
   - tf: instance of TransferFunction class
 - Returns:
   - out: instance of ZpkModel class
@@ -394,15 +394,15 @@
 
                        (s+2)
 0.3333 * ----------------------------------
          (s+0.6667+1.106j)(s+0.6667-1.106j)
 ```
 
 
-## 3.7. ss2tf
+### 3.7. ss2tf
 
 pylib_sakata.ctrl.**ss2tf**(*ss*)
 
 - Parameters:
   - ss: instance of StateSpace class
 - Returns:
   - out: instance of TransferFunction class
@@ -413,15 +413,15 @@
 >>> print(ctrl.ss2tf(Sys_ss))
 
 9 s^2 + 113 s + 118
 -------------------
    s^2 + 3 s + 2
 ```
 
-## 3.8. ss2zpk
+### 3.8. ss2zpk
 
 pylib_sakata.ctrl.**ss2zpk**(*ss*)
 
 - Parameters:
   - ss: instance of StateSpace class
 - Returns:
   - out: instance of ZpkModel class
@@ -432,15 +432,15 @@
 >>> ctrl.ss2zpk(Sys_ss)
 
     (s+11.41)(s+1.149)
 9 * ------------------
         (s+2)(s+1)
 ```
 
-## 3.9. zpk2tf
+### 3.9. zpk2tf
 
 pylib_sakata.ctrl.**zpk2tf**(*zpk*)
 
 - Parameters:
   - zpk: instance of ZpkModel class
 - Returns:
   - out: instance of TransferFunction class
@@ -451,15 +451,15 @@
 >>> print(ctrl.zpk2tf(Sys_zpk))
 
     2 s^2 + 6 s + 4
 ------------------------
 s^3 + 12 s^2 + 47 s + 60
 ```
 
-## 3.10. zpk2ss
+### 3.10. zpk2ss
 
 pylib_sakata.ctrl.**zpk2ss**(*zpk, form='reachable'*)
 
 - Parameters:
   - zpk: instance of ZpkModel class
   - form: canonical form (Optional), Default: reachable. You can select the canonical form in reachable, observable, and modal.
 - Returns:
@@ -478,15 +478,15 @@
      [0.]]
 
 C = [[2. 6. 4.]]
 
 D = [[0.]]
 ```
 
-## 3.11. sys2frd
+### 3.11. sys2frd
 
 pylib_sakata.ctrl.**sys2frd**(*sys, freq*)
 
 - Parameters:
   - sys: LTI model (StateSpace or TransferFunction or ZpkModel)
   - freq: 1-D array frequency data [Hz]
 - Returns:
@@ -512,15 +512,15 @@
 freq = array([   1.            1.00069108    1.00138264 ...  998.61926487  999.30939397
  1000.        ])
 resp = array([1.89109027e-01-0.06951671j 1.89033162e-01-0.06962001j
  1.88957165e-01-0.0697232j  ... 4.57206511e-07-0.00031875j
  4.56575231e-07-0.00031853j 4.55944822e-07-0.00031831j])
 ```
 
-## 3.12. feedback
+### 3.12. feedback
 
 pylib_sakata.ctrl.**feedback**(*sysP, sysC, sys='S'*)
 
 This function is for calculating the feedback system that consist of two LTI model (P: plant and C: controller).
 
 - Parameters:
   - sysP: LTI model (StateSpace or TransferFunction or ZpkModel) of the plant
@@ -545,15 +545,15 @@
 >>> ctrl.feedback(P_zpk, C_zpk)
 
                      s(s+2)(s+2)s
 1 * -----------------------------------------------
     (s+1)(s+1-0.0001508j)(s+1+0.0001508j)(s+0.9998)
 ```
 
-## 3.13. frdfeedback
+### 3.13. frdfeedback
 
 pylib_sakata.ctrl.**frdfeedback**(*frdP, frdC, sys='S'*)
 
 This function is for calculating the feedback system that consist of two freqresp (P: plant and C: controller).
 
 - Parameters:
   - frdP: 1-D array complex data of the frequency response of the plant
@@ -573,15 +573,15 @@
 >>> C_frd = ctrl.tf2frd(C_tf, freq)
 >>> ctrl.frdfeedback(P_frd, C_frd)
 array([1.04746047+1.56990662e-02j, 1.04739933+1.56671729e-02j,
        1.04733826+1.56353434e-02j, ..., 1.00000005+1.61927479e-11j,
        1.00000005+1.61592227e-11j, 1.00000005+1.61257668e-11j])
 ```
 
-## 3.14. c2d
+### 3.14. c2d
 
 pylib_sakata.ctrl.**c2d**(*sysC, dt, method='tustin'*)
 
 The matched method of **c2d** in control library does not supported for pure integrals and pure derivatives because of dc gain inf error. This function solved this problem.
 
 - Parameters:
   - sysC: continuous time LTI model (StateSpace or TransferFunction or ZpkModel) of the plant
@@ -589,44 +589,40 @@
   - method: discretized method (Optional), Default: 'tustin', set a method in 'tustin', 'matched', 'zoh', and etc.
 - Returns:
   - out: discrete time LTI model (StateSpace or TransferFunction or ZpkModel) of the feedback system
 
 **Examples**
 ```python
 >>> C_tf = ctrl.tf([1., 3., 2.], [1., 3., 0.])
->>> print(ctrl.c2d_matched(C_tf, 0.001))
+>>> print(ctrl.c2d(C_tf, 0.001, 'matched'))
 
 z^2 - 1.997 z + 0.997
 ---------------------
 z^2 - 1.997 z + 0.997
 
 dt = 0.001
 ```
 ```python
 >>> C_zpk = ctrl.zpk([-1., -2.,], [0., -3.,], 1.)
->>> ctrl.c2d_matched(C_zpk, 0.001)
+>>> ctrl.c2d(C_zpk, 0.001, 'matched')
 
     (z-0.999)(z-0.998)
 1 * ------------------
       (z-1)(z-0.997)
 
 dt = 0.001
 ```
 
-## 3.15. pi
+### 3.15. pi
 
 pylib_sakata.ctrl.**pi**(*freq, zeta, L, R, dt=None, method='tustin'*)
 
 This function is for design of a PI controller.
-$$
-C_{PI}(s) = K_P + \frac{K_I}{s} = \frac{b_1s+b_0}{s}
-$$
-$$
-P(s) = \frac{1}{Ls+R}
-$$
+$$C_{PI}(s) = K_P + \frac{K_I}{s} = \frac{b_1s+b_0}{s}$$
+$$P(s) = \frac{1}{Ls+R}$$
 
 - Parameters:
   - freq: frequency[Hz] of the pole pair of the feedback system with the PI controller
   - zeta: damping of the pole pair of the feedback system with the PI controller
   - L: inductance[H] of the plant
   - R: resistance[$\Omega$] of the plant
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
@@ -648,25 +644,21 @@
 2844 z + 1104
 -------------
     z - 1
 
 dt = 0.001
 ```
 
-## 3.16. pd
+### 3.16. pd
 
 pylib_sakata.ctrl.**pd**(*freq1, freq2, zeta2, M, C, K, dt=None, method='tustin'*)
 
 This function is for design of a PD controller.
-$$
-C_{PID}(s) = K_P + \frac{K_D s}{\tau_D s+1} = \frac{b_1s+b_0}{s+a_1}
-$$
-$$
-P(s) = \frac{1}{Ms^2+Cs+K}
-$$
+$$C_{PD}(s) = K_P + \frac{K_D s}{\tau_D s+1} = \frac{b_1s+b_0}{s+a_0}$$
+$$P(s) = \frac{1}{Ms^2+Cs+K}$$
 
 - Parameters:
   - freq1: frequency[Hz] of the first pole of the feedback system with the PD controller
   - freq2: frequency[Hz] of the second pole pair of the feedback system with the PD controller
   - zeta2: damping of the second pole pair of the feedback system with the PD controller
   - M: mass[kg] of the plant
   - C: viscosity[N/(m/s)] of the plant
@@ -690,25 +682,21 @@
 1.653e+04 z - 1.607e+04
 -----------------------
       z - 0.8641
 
 dt = 0.001
 ```
 
-## 3.17. pid
+### 3.17. pid
 
 pylib_sakata.ctrl.**pid**(*freq1, zeta1, freq2, zeta2, M, C, K, dt=None, method='tustin'*)
 
 This function is for design of a PID controller.
-$$
-C_{PID}(s) = K_P + \frac{K_I}{s} + \frac{K_D s}{\tau_D s+1} = \frac{b_2s^2+b_1s+b_0}{s^2+a_1s}
-$$
-$$
-P(s) = \frac{1}{Ms^2+Cs+K}
-$$
+$$C_{PID}(s) = K_P + \frac{K_I}{s} + \frac{K_D s}{\tau_D s+1} = \frac{b_2s^2+b_1s+b_0}{s^2+a_1s}$$
+$$P(s) = \frac{1}{Ms^2+Cs+K}$$
 
 - Parameters:
   - freq1: frequency[Hz] of the first pole pair of the feedback system with the PID controller
   - zeta1: damping of the first pole pair of the feedback system with the PID controller
   - freq2: frequency[Hz] of the second pole pair of the feedback system with the PID controller
   - zeta2: damping of the second pole pair of the feedback system with the PID controller
   - M: mass[kg] of the plant
@@ -733,22 +721,20 @@
 3.32e+04 z^2 - 6.485e+04 z + 3.167e+04
 --------------------------------------
         z^2 - 1.811 z + 0.8111
 
 dt = 0.001
 ```
 
-## 3.18. pl1st
+### 3.18. pl1st
 
 pylib_sakata.ctrl.**pl1st**(*freq1, freq2, dt=None, method='tustin'*)
 
 This function is for design of a first order phase lead filter.
-$$
-F_{PL}(s) = \frac{f_2}{f_1} * \frac{s+2\pi f_1}{s+2\pi f_2}
-$$
+$$F_{PL}(s) = \frac{f_2}{f_1} * \frac{s+2\pi f_1}{s+2\pi f_2}$$
 
 - Parameters:
   - freq1: frequency[Hz] of numerator of the phase lead filter
   - freq2: frequency[Hz] of denominator of the phase lead filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
@@ -768,22 +754,20 @@
         (z-0.7285)
 1.761 * ----------
         (z-0.5219)
 
 dt = 0.001
 ```
 
-## 3.19. pl2nd
+### 3.19. pl2nd
 
 pylib_sakata.ctrl.**pl2nd**(*freq1, zeta1, freq2, zeta2, dt=None, method='tustin'*)
 
 This function is for design of a second order phase lead filter.
-$$
-F_{PL^2}(s) = \left( \frac{f_2}{f_1} \right)^2 * \frac{s^2+2\zeta_1 (2\pi f_1)s+(2\pi f_1)^2}{s^2+2\zeta_2 (2\pi f_2)s+(2\pi f_2)^2}
-$$
+$$F_{PL^2}(s) = \left( \frac{f_2}{f_1} \right)^2 * \frac{s^2+2\zeta_1 (2\pi f_1)s+(2\pi f_1)^2}{s^2+2\zeta_2 (2\pi f_2)s+(2\pi f_2)^2}$$
 
 - Parameters:
   - freq1: frequency[Hz] of numerator of the phase lead filter
   - zeta1: damping of numerator of the phase lead filter
   - freq2: frequency[Hz] of denominator of the phase lead filter
   - zeta2: damping of denominator of the phase lead filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
@@ -805,22 +789,20 @@
 1.618 z^2 - 2.536 z + 1.046
 ---------------------------
   z^2 - 1.172 z + 0.4283
 
 dt = 0.001
 ```
 
-## 3.20. lpf1st
+### 3.20. lpf1st
 
 pylib_sakata.ctrl.**lpf1st**(*freq, dt=None, method='tustin'*)
 
 This function is for design of a first order low pass filter.
-$$
-F_{LP}(s) = \frac{2\pi f}{s+2\pi f}
-$$
+$$F_{LP}(s) = \frac{2\pi f}{s+2\pi f}$$
 
 - Parameters:
   - freq: frequency[Hz] of the low pass filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
   - out: instance of TransferFunction class of the low pass filter
@@ -839,22 +821,20 @@
 0.2391 z + 0.2391
 -----------------
    z - 0.5219
 
 dt = 0.001
 ```
 
-## 3.21. lpf2nd
+### 3.21. lpf2nd
 
 pylib_sakata.ctrl.**lpf2nd**(*freq, zeta, dt=None, method='tustin'*)
 
 This function is for design of a second order low pass filter.
-$$
-F_{LP^2}(s) = \frac{(2\pi f)^2}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}
-$$
+$$F_{LP^2}(s) = \frac{(2\pi f)^2}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}$$
 
 - Parameters:
   - freq: frequency[Hz] of the low pass filter
   - zeta1: damping of the low pass filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
@@ -874,22 +854,20 @@
 0.06415 z^2 + 0.1283 z + 0.06415
 --------------------------------
      z^2 - 1.172 z + 0.4283
 
 dt = 0.001
 ```
 
-## 3.22. hpf1st
+### 3.22. hpf1st
 
 pylib_sakata.ctrl.**hpf1st**(*freq, dt=None, method='tustin'*)
 
 This function is for design of a first order high pass filter.
-$$
-F_{HP}(s) = 1 - F_{LP}(s) = \frac{s}{s+2\pi f}
-$$
+$$F_{HP}(s) = 1 - F_{LP}(s) = \frac{s}{s+2\pi f}$$
 
 - Parameters:
   - freq: frequency[Hz] of the high pass filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
   - out: instance of TransferFunction class of the high pass filter
@@ -908,22 +886,20 @@
 0.7609 z - 0.7609
 -----------------
    z - 0.5219
 
 dt = 0.001
 ```
 
-## 3.23. hpf2nd
+### 3.23. hpf2nd
 
 pylib_sakata.ctrl.**hpf2nd**(*freq, zeta, dt=None, method='tustin'*)
 
 This function is for design of a second order high pass filter.
-$$
-F_{HP^2}(s) = 1 - F_{LP^2}(s) = \frac{s^2+2\zeta (2\pi f)s}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}
-$$
+$$F_{HP^2}(s) = 1 - F_{LP^2}(s) = \frac{s^2+2\zeta (2\pi f)s}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}$$
 
 - Parameters:
   - freq: frequency[Hz] of the high pass filter
   - zeta1: damping of the high pass filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
@@ -943,22 +919,20 @@
 0.9358 z^2 - 1.3 z + 0.3641
 ---------------------------
   z^2 - 1.172 z + 0.4283
 
 dt = 0.001
 ```
 
-## 3.24. nf
+### 3.24. nf
 
 pylib_sakata.ctrl.**nf**(*freq, zeta, depth, dt=None, method='matched'*)
 
 This function is for design of notch filters.
-$$
-F_{notch}(s) = \frac{s^2+2d\zeta (2\pi f)s+(2\pi f)^2}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}
-$$
+$$F_{notch}(s) = \frac{s^2+2d\zeta (2\pi f)s+(2\pi f)^2}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}$$
 
 - Parameters:
   - freq: array of frequency[Hz] of the notch filters
   - zeta: array of damping of the notch filters
   - depth: array of depth of the notch filters (0 < depth < 1)
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'matched', set a method if dt > 0
@@ -977,22 +951,20 @@
 >>> ctrl.nf([100., 200., 300.], [0.02, 0.02, 0.02], [0.01, 0.01, 0.01], 0.001)
 array([TransferFunction(array([ 0.9876627 , -1.59787102,  0.9874145 ]), array([ 1.        , -1.59797428,  0.97518046]), 0.001),
        TransferFunction(array([ 0.97553399, -0.6027617 ,  0.97504375]), array([ 1.        , -0.60316088,  0.95097692]), 0.001),
        TransferFunction(array([0.96362486, 0.59532837, 0.96289858]), array([1.        , 0.59447771, 0.92737411]), 0.001)],
       dtype=object)
 ```
 
-## 3.25. pf
+### 3.25. pf
 
 pylib_sakata.ctrl.**pf**(*freq, zeta, k, phi, dt=None, method='tustin'*)
 
 This function is for design of peak filters ([resonant filters](https://ieeexplore.ieee.org/document/4291569)).
-$$
-F_{peak}(s) = \frac{k(s^2-\phi s)}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}
-$$
+$$F_{peak}(s) = \frac{k(s^2-\phi s)}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}$$
 
 - Parameters:
   - freq: array of frequency[Hz] of the peak filters
   - zeta: array of damping of the peak filters
   - k: array of peak width of the peak filters
   - phi: array of phase lead of the peak filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
@@ -1013,15 +985,15 @@
 >>> ctrl.pf([2., 3., 5.], [0.001, 0.001, 0.001], [-0.00025695, -0.00049616, 0.0003898], [860.21053991, 633.22924516, -1090.49879949], 0.001)
 array([TransferFunction(array([-0.00014643,  0.00051387, -0.00036745]), array([ 1.        , -1.99981696,  0.99997487]), 0.001),
        TransferFunction(array([-0.00033903,  0.00099221, -0.00065318]), array([ 1.        , -1.99960704,  0.9999623 ]), 0.001),
        TransferFunction(array([ 0.00060217, -0.00077938,  0.00017721]), array([ 1.        , -1.9989505 ,  0.99993719]), 0.001)],
       dtype=object)
 ```
 
-## 3.26. pfoptparam
+### 3.26. pfoptparam
 pylib_sakata.ctrl.**pfoptparam**(freq, zeta, depth, sysT)
 
 This function is for getting parameters of optimized peak filters ([resonant filters](https://ieeexplore.ieee.org/document/4291569)).
 
 - Parameters:
   - freq: array of frequency[Hz] of the peak filters
   - zeta: array of damping of the peak filters
@@ -1038,15 +1010,15 @@
 >>> Ps = ctrl.tf([1.], [2., 10., 0.])
 >>> Cs = ctrl.pid(10., 1., 10., 0.7, 2., 10., 0.)
 >>> ctrl.pfoptparam([2., 3., 5.], [0.001, 0.001, 0.001], [0.1, 0.1, 0.1], ctrl.feedback(Ps, Cs, sys='T'))
 The common pole-zeros of the zpk model have been deleted.
 ([2.0, 3.0, 5.0], [0.001, 0.001, 0.001], array([-0.00025695, -0.00049616,  0.0003898 ]), array([  860.21053991,   633.22924516, -1090.49879949]))
 ```
 
-## 3.27. pfopt
+### 3.27. pfopt
 
 pylib_sakata.ctrl.**pfopt**(*freq, zeta, depth, sysT, dt=None, method='tustin'*)
 
 This function is for design of optimized peak filters ([resonant filters](https://ieeexplore.ieee.org/document/4291569)).
 
 - Parameters:
   - freq: array of frequency[Hz] of the peak filters
@@ -1074,33 +1046,32 @@
 The common pole-zeros of the zpk model have been deleted.
 array([TransferFunction(array([ 0.0049857 , -0.00972818,  0.00474248]), array([ 1.        , -1.99981696,  0.99997487]), 0.001),
        TransferFunction(array([ 0.00740923, -0.01446026,  0.00705103]), array([ 1.        , -1.99960704,  0.9999623 ]), 0.001),
        TransferFunction(array([ 0.01227286, -0.02398427,  0.01171141]), array([ 1.        , -1.9989505 ,  0.99993719]), 0.001)],
       dtype=object)
 ```
 
-## 3.28. dob
+### 3.28. dob
 pylib_sakata.ctrl.**dob**(*freq, zeta, M, C, K, dt, nd = 0*)
 
 This function is for design of a discrete-time disturbance observer (DOB).
-$$
-\hat{d} = -z^{n_d} Q[z] u + Q[z] P^{-1}[z] y
-$$
+$$\hat{d} = -z^{-n_d} Q[z] u + Q[z] P^{-1}[z] y$$
+
 Here, it is defined that disturbance $d$ is injected in the system as plus sign.
 
 - Parameters:
   - freq: frequency[Hz] of the pole pair of the DOB
   - zeta: damping of the pole pair of the DOB
   - M: mass[kg] of the plant
   - C: viscosity[N/(m/s)] of the plant
   - K: stiffness[N/m] of the plant
   - dt: sampling time of the system
   - nd: sampling number of the dead-time of the system
 - Returns:
-  - DOBu: $z^{n_d} Q[z]$
+  - DOBu: $z^{-n_d} Q[z]$
   - DOBy: $Q[z] P^{-1}[z]$
 
 **Examples**
 ```python
 >>> DOBu, DOBy = ctrl.dob(5., 0.7, 1., 10., 0., 0.001, 1)
 >>> print(DOBu)
 
@@ -1115,15 +1086,15 @@
 970.3 z^2 - 1931 z + 960.7
 --------------------------
   z^2 - 1.956 z + 0.957
 
 dt = 0.001
 ```
 
-## 3.29. zpetc
+### 3.29. zpetc
 pylib_sakata.ctrl.**zpetc**(*Pz, dt, zerothr=0.99*)
 
 This function is for design of a zero phase error tracking controller ([ZPETC](https://engineering.purdue.edu/ME576/ZPETC_Tomizuka.pdf)).
 
 - Parameters:
   - Pz: instance of TransferFunction class of discrete-time LTI system
   - dt: sampling time of the system
@@ -1153,47 +1124,47 @@
 
 dt = 0.001
 
 >>> Nzpetc
 2
 ```
 
-## 3.30. filt
+### 3.30. filt
 pylib_sakata.ctrl.**filt**(*num, den, dt*)
 
 This function is to create transfer functions as rational expressions in $z^{-1}$ and to order the numerator and denominator terms in ascending powers of $z^{-1}$.
 
 - Parameters:
   - num: polynomial coefficients of the numerator of the discrete-time LTI model
   - den: polynomial coefficients of the denominator of the discrete-time LTI model
   - dt: sampling time of the discrete-time LTI model
 - Returns:
   - out: instance of TransferFunction class of ZPETC
 
-## 3.31. minreal
+### 3.31. minreal
 pylib_sakata.ctrl.**minreal**(*sys*)
 
 This function is to delete the common pole-zeros of the system.
 
 - Parameters:
   - sys: LTI model (StateSpace or TransferFunction or ZpkModel)
 - Returns:
   - out: LTI model whose the common pole-zeros were deleted
 
-## 3.32. makeprmset
+### 3.32. makeprmset
 pylib_sakata.ctrl.**makeprmset**(*path='.'*)
 
 This function is to create Cpp and header files of controller parameter sets
 
 - Parameters:
   - path: path to create Cpp and header files of controller parameter sets
 - Returns:
   - None
   
-## 3.33. defprmset
+### 3.33. defprmset
 pylib_sakata.ctrl.**defprmset**(*tfz, prmSetName, path='.', mode='a'*)
 
 - Parameters:
   - tfz: discrete time TransferFunction model
   - prmSetName: parameter set name of the following struct in Cpp
   - path: path to create Cpp and header files of controller parameter sets
   - mode: mode to open Cpp and header files
@@ -1219,17 +1190,17 @@
 	double	dA[4];
 	double	dB[4];
 	double	dInPre[3];
 	double	dOutPre[3];
 } TF3_INF;						// 3rd order TF information
 ```
 
-# 4. pylib_sakata.fft
+## 4. pylib_sakata.fft
 
-## 4.1. FreqResp
+### 4.1. FreqResp
 
 class pylib_sakata.fft.**FreqResp**(*freq, resp, dt=0*)
 
 - Parameters:
   - freq: 1-D array frequency data [Hz]
   - resp: 1-D array frequency response data [complex data]
   - dt: sampling time (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
@@ -1264,15 +1235,15 @@
 
 - \__**rtruediv**__(*other*)
 	Right divide two FRDs.
 
 - \__**pow**__(*other*)
 	A FRD to the power of x.
 
-## 4.2. fft
+### 4.2. fft
 
 pylib_sakata.fft.**fft**(*data, dt*)
 
 This function is for calculating FFT from 1-D array data.
 
 - Parameters:
   - data: 1-D array time response data
@@ -1289,25 +1260,25 @@
 >>> x = np.sin(2*np.pi*10.0*t) + np.sin(2*np.pi*50.0*t)
 >>> fft.fft(x, dt)
 (array([0.00000000e+00, 1.00010001e-01, 2.00020002e-01, ...,
        9.99799980e+02, 9.99899990e+02, 1.00000000e+03]), array([3.93463040e-17, 2.39600781e-06, 4.79322523e-06, ...,
        7.19286425e-06, 4.79322523e-06, 2.39600781e-06]))
 ```
 
-## 4.3. fft_ave
+### 4.3. fft_ave
 
 pylib_sakata.fft.**fft_ave**(*data, dt, windivnum=4, overlap=0.5*)
 
 This function is for calculating averaged FFT from 1-D array data.
 
 - Parameters:
   - data: 1-D array time response data
   - dt: sampling time of the time response data
   - windivnum: number of windows to divide the time response data
-  - overlap: overlap retio divided time response data (0 <= overlap < 1)
+  - overlap: overlap ratio divided time response data (0 <= overlap < 1)
 - Returns:
   - freq_data: 1-D array frequency data [Hz]
   - fft_data: 1-D array FFT data
 
 **Examples**
 ```python
 import numpy as np
@@ -1316,27 +1287,27 @@
 >>> x = np.sin(2*np.pi*10.0*t) + np.sin(2*np.pi*50.0*t)
 >>> fft.fft_ave(x, dt, 4, 0.5)
 (array([0.00000000e+00, 4.88519785e-01, 9.77039570e-01, ...,
        9.99022960e+02, 9.99511480e+02, 1.00000000e+03]), array([5.33388114e-05, 5.46444944e-05, 5.85999322e-05, ...,
        6.53498409e-05, 5.85999322e-05, 5.46444944e-05]))
 ```
 
-## 4.4. tfestimate
+### 4.4. tfestimate
 
 pylib_sakata.fft.**tfestimate**(*x, y, freq, dt, windivnum=4, overlap=0.5*)
 
 This function is for system identification from input and output time response data.
 
 - Parameters:
   - x: 1-D array time response data of input
   - y: 1-D array time response data of output
   - freq: 1-D array frequency data [Hz]
   - dt: sampling time of the time response data
   - windivnum: number of windows to divide the time response data
-  - overlap: overlap retio divided time response data (0 <= overlap < 1)
+  - overlap: overlap ratio divided time response data (0 <= overlap < 1)
 - Returns:
   - freqresp: instance of FreqResp class
   - coh: 1-D array coherence data
 
 **Examples**
 ```python
 >>> import numpy as np
@@ -1354,15 +1325,15 @@
 >>> fft.tfestimate(u, y, freq, dt)
 (array([-0.11586071-1.49076948e-01j, -0.11590257-1.49078279e-01j,
        -0.11594446-1.49079611e-01j, ..., -0.13155661-1.45847229e-01j,
        -0.14201211-1.03211830e-01j, -0.15745492-1.88460358e-14j]), array([0.77271576, 0.77244166, 0.7721674 , ..., 0.23080322, 0.32843388,
        0.43848208]))
 ```
 
-## 4.5. frdresize
+### 4.5. frdresize
 
 pylib_sakata.fft.**frdresize**(*freqresp, freq*)
 
 This function is for resizing a frequency response data.
 
 - Parameters:
   - freqresp: instance of FreqResp class
@@ -1382,57 +1353,57 @@
 freq = array([   1.            1.00069108    1.00138264 ...  998.61926487  999.30939397
  1000.        ])
 resp = array([-5.10821217e-03-5.65218353e-02j -5.10244172e-03-5.64813436e-02j
  -5.09666728e-03-5.64408239e-02j ... -5.64622394e-09-5.31301950e-05j
  -5.63759203e-09-5.30909366e-05j -5.62895416e-09-5.30516511e-05j])
 ```
 
-## 4.6. frdsim
+### 4.6. frdsim
 
 pylib_sakata.fft.**frdsim**(*freqresp, x, dt*)
 
 This function is for simulation steady time response data when a time-domain data is input to a system written by frequency response data.
-$$
-y(t) = \text{ifft}(\text{FreqResp}(\omega)\times\text{fft}(u(t)))
-$$
+$$y(t) = \text{ifft}(\text{FreqResp}(\omega)\times\text{fft}(u(t)))$$
 
 - Parameters:
   - freqresp: instance of FreqResp class
   - x: 1-D array time response data of input
   - dt: sampling time of the time response data
 - Returns:
+  - t: 1-D array time data [s]
   - y: 1-D array time response data of output
 
 **Examples**
 ```python
 >>> import numpy as np
 >>> freq = np.logspace(np.log10(1.), np.log10(1000.), 100, base=10)
 >>> Sys_tf = ctrl.tf([1., 2.], [3., 4., 5.])
 >>> freqresp = ctrl.sys2frd(Sys_tf, freq)
 >>> dt = 0.001
 >>> t = np.linspace(0.0, 10., int(10./dt))
 >>> x = np.sin(2*np.pi*10.0*t) + np.sin(2*np.pi*50.0*t)
 >>> fft.frdsim(freqresp, x, dt)
-array([-0.00635301, -0.00630568, -0.00612106, ..., -0.00610225,
-       -0.0062943 , -0.00634922])
+(array([0.000e+00, 1.000e-03, 2.000e-03, ..., 9.996e+00, 9.997e+00,
+       9.998e+00]), array([-0.00635301, -0.00630568, -0.00612106, ..., -0.00610225,
+       -0.0062943 , -0.00634922]))
 ```
 
-# 5. pylib_sakta.meas
+## 5. pylib_sakata.meas
 
-## 5.1. MeasData
+### 5.1. MeasData
 
-class pylib_sakata.meas.**MeasData**(*time, list, value, time, dt*)
+class pylib_sakata.meas.**MeasData**(*list, value, time, dt*)
 
 - Parameters:
-  - dataList: array of data list (*str*)
-  - dataValue: array of data value
+  - list: array of data list (*str*)
+  - value: array of data value
   - time: 1-D array time data [s]
   - dt: sampling time of the time response data
 
-## 5.2. getcsvdata
+### 5.2. getcsvdata
 
 pylib_sakata.meas.**getcsvdata**(*filePath*)
 
 This function is for getting measurement data from a csv file.
 
 - Parameters:
   - filePath: csv file path of measurement file
@@ -1440,15 +1411,15 @@
   - instance of MeasData class
 
 **Examples**
 ```python
 measdata = meas.getcsvdata('data\001-inject.csv')
 ```
 
-## 5.3. gettxtdata
+### 5.3. gettxtdata
 
 pylib_sakata.meas.**gettxtdata**(*filePath*)
 
 This function is for getting measurement data from a txt file.
 
 - Parameters:
   - filePath: txt file path of measurement file
@@ -1456,15 +1427,15 @@
   - instance of MeasData class
 
 **Examples**
 ```python
 measdata = meas.gettxtdata('data\001-inject.txt')
 ```
 
-## 5.4. getmatdata
+### 5.4. getmatdata
 
 pylib_sakata.meas.**getmatdata**(*filePath*)
 
 This function is for getting measurement data from a mat file.
 
 - Parameters:
   - filePath: mat file path of measurement file
@@ -1472,52 +1443,52 @@
   - instance of MeasData class
 
 **Examples**
 ```python
 measdata = meas.getmatdata('data\001-inject.mat')
 ```
 
-## 5.5. getdata
+### 5.5. getdata
 
 pylib_sakata.meas.**getdata**(*filePath*)
 
 This function is for getting measurement data from a file.
 
 - Parameters:
   - filePath: file path of measurement file (.csv, .txt, and .mat are supported.)
 - Returns:
   - instance of MeasData class
 
 **Examples**
 ```python
-measdata = meas.getmatdata('data\001-inject.csv')
+measdata = meas.getdata('data\001-inject.csv')
 ```
 ```python
-measdata = meas.getmatdata('data\001-inject.txt')
+measdata = meas.getdata('data\001-inject.txt')
 ```
 ```python
-measdata = meas.getmatdata('data\001-inject.mat')
+measdata = meas.getdata('data\001-inject.mat')
 ```
 
-## 5.6. getdataindex
+### 5.6. getdataindex
 
 pylib_sakata.meas.**getdataindex**(*measdata, dataName*)
 
 - Parameters:
   - measdata: instance of MeasData class
   - dataName: data name
 - Returns:
   - index: index of dataName
 
 **Examples**
 ```python
 index = meas.getdataindex(measdata, 'ServoOut')
 ```
 
-## 5.7. measdata2frd
+### 5.7. measdata2frd
 
 pylib_sakata.meas.**measdata2frd**(*filePath, inputName, outputName, flagName, freq, inputGain=1.0, outputGain=1.0, windivnum=4, overlap=0.5*)
 
 This function is for system identification from input and output time response data of measurement file.
 
 - Parameters:
   - filePath: file path of measurement file (.csv, .txt, and .mat are supported.)
@@ -1525,74 +1496,136 @@
   - outputName: output data name in the measurement file
   - flagName: flag data name in the measurement file
   - freq: 1-D array frequency data [Hz]
   - inputGain: inputdata gain (Optional), Default: 1.0, unit of input can be fixed by this parameter.
   - outputGain: outputdata gain (Optional), Default: 1.0, unit of output can be fixed by this parameter.
   - dt: sampling time of the time response data
   - windivnum: number of windows to divide the time response data
-  - overlap: overlap retio divided time response data (0 <= overlap < 1)
+  - overlap: overlap ratio divided time response data (0 <= overlap < 1)
 - Returns:
   - freqresp: instance of FreqResp class
   - coh: 1-D array coherence data
 
 **Examples**
 ```python
 import numpy as np
 freq = np.logspace(np.log10(1.), np.log10(1000.), 10000, base=10)
 freqresp, coh = measdata2frd('data\001-inject.csv', 'ServoOut', 'PosErrUm', 'FlagNoise', freq, 1., 1.e-6)
 ```
 
-# 6. pylib_sakata.traj
+## 6. pylib_sakata.traj
 
-## 6.1. TrajInf
+### 6.1. TrajInf
 
 class pylib_sakata.traj.**TrajInf**(*time, pos, vel, acc, T, dt*)
 
 - Parameters:
   - time: 1-D array time data [s]
   - pos: 1-D array position trajectory data [m]
   - vel: 1-D array velocity trajectory data [m/s]
   - acc: 1-D array acceleration trajectory data [m/s^2]
   - T: moving time [s]
   - dt: sampling time of the trajectory data
 
-## 6.2. traj4th
+### 6.2. traj3rd
+
+pylib_sakata.traj.**traj3rd**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)  
+
+This function is for generation of a 3rd order polynomial trajectory.
+
+- Parameters:
+  - posStart: start position of the trajectory
+  - posStep: step position of the trajectory
+  - velMax: maximum of velocity of the trajectory
+  - accAve: average of accelation (= decelation) of the trajectory
+  - dt: sampling time of the trajectory data.
+  - Tstay: time after the step moving
+- Returns:
+  - out: instance of TrajInf class of the 3rd order polynomial trajectory
+
+**Examples**
+```python
+traj = traj.traj3rd(0, 100, 100, 200, 0.001, 0.5)
+```
+
+### 6.3. traj3rd2
+
+pylib_sakata.traj.**traj3rd2**(*posStart, posStep, velMax, accAve, jerkRatio, dt, Tstay=0*)  
 
-pylib_sakata.traj.**traj4th**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
+This function is for generation of a 3rd order polynomial trajectory as trapezoidal accelaration trajectory.
+
+- Parameters:
+  - posStart: start position of the trajectory
+  - posStep: step position of the trajectory
+  - velMax: maximum of velocity of the trajectory
+  - accAve: average of accelation (= decelation) of the trajectory
+  - jerkRatio: ratio of jerk time per accelaration time (0 < jerkRatio <= 0.5)
+  - dt: sampling time of the trajectory data.
+  - Tstay: time after the step moving
+- Returns:
+  - out: instance of TrajInf class of the 3rd order polynomial trajectory
+
+**Examples**
+```python
+traj = traj.traj3rd2(0, 100, 100, 200, 0.001, 0.2, 0.5)
+```
+
+### 6.4. traj4th
+
+pylib_sakata.traj.**traj4th**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)  
+pylib_sakata.traj.**traj4th2**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
 
 This function is for generation of a 4th order polynomial trajectory.
 
 - Parameters:
   - posStart: start position of the trajectory
   - posStep: step position of the trajectory
   - velMax: maximum of velocity of the trajectory
   - accAve: average of accelation (= decelation) of the trajectory
   - dt: sampling time of the trajectory data.
+  - Tstay: time after the step moving
 - Returns:
   - out: instance of TrajInf class of the 4th order polynomial trajectory
 
 **Examples**
 ```python
 traj = traj.traj4th(0, 100, 100, 200, 0.001, 0.5)
+```
 
-fig = plot.makefig()
-ax1 = fig.add_subplot(311)
-ax2 = fig.add_subplot(312)
-ax3 = fig.add_subplot(313)
-plot.plot_xy(ax1, traj.time, traj.pos, ylabel='[m]', legend=['Pos'], title='TrajInf')
-plot.plot_xy(ax2, traj.time, traj.vel, ylabel='[m/s]', legend=['Vel'])
-plot.plot_xy(ax3, traj.time, traj.acc, xlabel='Time [s]', ylabel='[m/s^2]', legend=['Acc'])
-plot.savefig('time_traj.png')
+### 6.5. trajSinStep
+
+pylib_sakata.traj.**trajSinStep**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
+pylib_sakata.traj.**trajSinStep2**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
+pylib_sakata.traj.**trajSinStep3**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
+
+This function is for generation of a trajectory based on sine waves.
+
+- Parameters:
+  - posStart: start position of the trajectory
+  - posStep: step position of the trajectory
+  - velMax: maximum of velocity of the trajectory
+  - accAve: average of accelation (= decelation) of the trajectory
+  - dt: sampling time of the trajectory data.
+  - Tstay: time after the step moving
+- Returns:
+  - out: instance of TrajInf class of the trajectory based on sine waves
+
+**Examples**
+```python
+traj = traj.SinStep(0, 100, 100, 200, 0.001, 0.5)
 ```
 
-<img src="figure\time_traj.png" alt="vscode_disp" style="zoom: 80%;" />
+The comparison of these trajectories under the specification: posStep = 1, velMax = 1, accAve = 2 is shown as follows.
+
+<img src="figure\time_traj.png" alt="vscode_disp" style="zoom: 15%;" />
+<img src="figure\time_fft.png" alt="vscode_disp" style="zoom: 40%;" />
 
-# 7. pylib_sakata.plot
+## 7. pylib_sakata.plot
 
-## 7.1. plot_xy
+### 7.1. plot_xy
 
 pylib_sakata.plot.**plot_xy**(*ax, x, y, styl='-', col='b', width=1.5, alpha=1.0, xrange=None, yrange=None, xlabel=None, ylabel=None, legend=None, loc='best', title=None, xscale='linear', yscale='linear', labelouter=True*)
 
 This function is for drawing a 2-D figure from x and y data. You can select xy scale in linear type, log type and so on.
 
 - Parameters:
   - ax: handle of axis
@@ -1629,15 +1662,15 @@
 ax2 = fig2.add_subplot(312)
 ax3 = fig2.add_subplot(313)
 plot.plot_xy(ax1, fft_axis, chirp_fft, '-', 'm', 1.5, 1.0, freqrange, [0, 1.0], ylabel='Input [N]', legend=['Chirp'], title='Power spectrum density', xscale='log')
 plot.plot_xy(ax2, fft_axis, u_fft, '-', 'b', 1.5, 1.0, freqrange, [0, 0.1], ylabel='Input [N]', legend=['Servo Out'], xscale='log')
 plot.plot_xy(ax3, fft_axis, y_fft*1.0e6, '-', 'b', 1.5, 1.0, freqrange, [0, 20], xlabel='Frequency [Hz]', ylabel='Output [um]', legend=['Position'], xscale='log')
 ```
 
-## 7.2. plot_tf
+### 7.2. plot_tf
 
 pylib_sakata.plot.**plot_tf**(*ax_mag, ax_phase, sys, freq, styl='-', col='b', width=1.5, alpha=1.0, freqrange=None, magrange=None, legend=None, loc='best', title=None, labelouter=True*)
 
 This function is for drawing a Bode diagram from a LTI model.
 
 - Parameters:
   - ax_mag: handle of magnitude axis
@@ -1670,25 +1703,24 @@
 fig2 = plot.makefig()
 ax_mag = fig2.add_subplot(211)
 ax_phase = fig2.add_subplot(212)
 plot.plot_tf(ax_mag, ax_phase, T, freq, '-', 'm', 1.5, 1.0, title='Frequency response of complementary sensitivity function')
 plot.plot_tf(ax_mag, ax_phase, Tn, freq, '--', 'b', 1.5, 1.0, [1, 1000], [-60, 10], legend=['Measurement','Model'])
 ```
 
-## 7.3. plot_tffrd
+### 7.3. plot_tffrd
 
 pylib_sakata.plot.**plot_tffrd**(*ax_mag, ax_phase, freqresp, styl='-', col='b', width=1.5, alpha=1.0, freqrange=None, magrange=None, legend=None, loc='best', title=None, labelouter=True, ax_coh=None, coh=None*)
 
 This function is for drawing a Bode diagram from a frequency response data.
 
 - Parameters:
   - ax_mag: handle of magnitude axis
   - ax_phase: handle of phase axis, if you set as None, phase axis is skipped.
   - freqresp: instance of FreqResp class
-  - freq: 1-D array frequency data [Hz]
   - styl: line style (Optional), Default: '-', Select in '-' (solid), '--' (dashed), '.' (dotted), '-.' (dashdot)
   - col: line color (Optional), Default: 'b' (blue)
   - width: line width (Optional), Default: 1.5
   - alpha: transmittance of line, Default: 1.0, set from 0 to 1.0
   - freqrange: plot range of frequency-axis (Optional), Default: None, set as [freqmin, freqmax]
   - magrange: plot range of magnitude-axis (Optional), Default: None, set as [magmin, magmax]
   - legend: legend of data, Default: None, set a list of strings data
@@ -1721,15 +1753,15 @@
 fig3 = plot.makefig()
 ax_mag = fig2.add_subplot(211)
 ax_phase = fig2.add_subplot(212)
 plot.plot_tffrd(ax_mag, ax_phase, T_frd, '-', 'm', 1.5, 1.0, title='Frequency response of complementary sensitivity function')
 plot.plot_tffrd(ax_mag, ax_phase, Tn_frd, '--', 'b', 1.5, 1.0, [1, 1000], [-60, 10], legend=['Measurement','Model'])
 ```
 
-## 7.4. plot_nyquist
+### 7.4. plot_nyquist
 
 pylib_sakata.plot.**plot_nyquist**(*ax, freqresp, styl='-', col='b', width=1.5, alpha=1.0, xrange=None, yrange=None, legend=None, loc='best', title=None, labelouter=True*)
 
 This function is for drawing a Nyquist diagram from a frequency response data of a open loop system
 
 - Parameters:
   - ax: handle of axis
@@ -1751,15 +1783,15 @@
 ```python
 fig = plot.makefig()
 ax = fig.add_subplot(111)
 plot.plot_nyquist(ax, G_frd, '-', 'm', 1.5, 1.0, title='Nyquist Diagram')
 plot.plot_nyquist(ax, Gn_frd, '--', 'b', 1.5, 1.0, legend=['Measurement','Model'])
 ```
 
-## 7.5. plot_nyquist_assistline
+### 7.5. plot_nyquist_assistline
 
 pylib_sakata.plot.**plot_nyquist_assistline**(*ax*)
 
 This function is for drawing assist line of a Nyquist diagram.
 
 - Parameters:
   - ax: handle of axis
@@ -1767,32 +1799,33 @@
   - None
 
 **Examples**
 ```python
 plot.plot_nyquist_assistline(ax)
 ```
 
-## 7.6. makefig
+### 7.6. makefig
 
-pylib_sakata.plot.**makefig**(dpi=100, popwin=False)
+pylib_sakata.plot.**makefig**(dpi=100, figsize=(6, 4), popwin=False)
 
 This function will make a new figure handle.
 
 - Parameters:
   - dpi: dot per inch of figure (Optional), Default: 100
+  - figsize: set figure size (Optional), Default: (6, 4) which means 600x400 pixels
   - popwin: switch to fix the popup window of the figure (Optional), Default: False
 - Returns:
   - fig: figure handle
 
 **Examples**
 ```python
 fig = plot.makefig()
 ```
 
-## 7.7. savefig
+### 7.7. savefig
 
 pylib_sakata.plot.**savefig**(*figName*)
 
 This function will save a current figure.
 
 - Parameters:
   - figName: figure name for saving a current figure, set strings data
@@ -1800,39 +1833,39 @@
   - None
 
 **Examples**
 ```python
 plot.savefig('freq_P.png')
 ```
 
-## 7.8. showfig
+### 7.8. showfig
 
 pylib_sakata.plot.**showfig**()
 
 This function will call matplotlib.pyplot.show()
 
 **Examples**
 ```python
 showfig()
 ```
 
-# 8. pylib_sakata.init
+## 8. pylib_sakata.init
 
-## 8.1. close_all
+### 8.1. close_all
 
 pylib_sakata.init.**close_all**()
 
 This function is for closing current opened figures.
 
 **Examples**
 ```python
 close_all()
 ```
 
-## 8.2. clear_all
+### 8.2. clear_all
 
 pylib_sakata.init.**clear_all**()
 
 This function is for deleting all defined variables.
 
 **Examples**
 ```python
```

### Comparing `pylib-sakata-0.1.9/setup.py` & `pylib-sakata-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (c) 2022 Koichi Sakata
+# Copyright (c) 2024 Koichi Sakata
 
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pylib-sakata",
-    version="0.1.9",
+    version="0.2.0",
     author="Koichi Sakata",
     author_email="",
     description="Control system design and analysis package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Koichi-Sakata/pylib_sakata",
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.8",
+    python_requires=">=3.11",
 )
```

### Comparing `pylib-sakata-0.1.9/src/pylib_sakata/ctrl.py` & `pylib-sakata-0.2.0/src/pylib_sakata/ctrl.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 import os
 import math
 import numpy as np
 from numpy.polynomial import polynomial
 import control
 from control import matlab
 from .fft import FreqResp
-
+import warnings
+warnings.simplefilter("ignore", np.ComplexWarning)
 
 class ZpkModel:
 
     def __init__(self, zeros, poles, gain, dt=0):
         # gain: not system dc gain but coefficient of monic polynomials!
         zeros = list(zeros)
         poles = list(poles)
@@ -263,23 +264,26 @@
     return matlab.ss(A, B, C, D, dt)
 
 
 def zpk(z, p, k, dt=0):
     return ZpkModel(z, p, k, dt)
 
 
-def tf2ss(tf, form='reachable'):
+def tf2ss(tf, form=None):
     # form: 'reachable' or 'observable' or 'modal'
-    ss, T = control.canonical_form(matlab.tf2ss(tf), form=form)
+    if form == None:
+        ss = matlab.tf2ss(tf)
+    else:
+        ss, T = control.canonical_form(matlab.tf2ss(tf), form=form)
     return ss
 
 
 def tf2zpk(tf):
-    zeros = tf.zero()
-    poles = tf.pole()
+    zeros = tf.zeros()
+    poles = tf.poles()
     gain = tf.num[0][0][0] / tf.den[0][0][0]
     dt = tf.dt
     zpk = ZpkModel(zeros, poles, gain, dt)
     return zpk
 
 
 def ss2tf(ss):
@@ -685,32 +689,36 @@
     zinv = tf([1], [1, 0], dt)
     numpoly = 0
     for i in range(len(num)):
         numpoly += num[i] * zinv ** i
     denpoly = 0
     for i in range(len(den)):
         denpoly += den[i] * zinv ** i
+    # return minreal(numpoly / denpoly)
     return minreal(numpoly / denpoly)
 
 
 def minreal(sys):
     if type(sys) == matlab.TransferFunction:
         return zpk2tf(tf2zpk(sys))
     elif type(sys) == matlab.StateSpace:
         return zpk2ss(ss2zpk(sys))
     else:
         return sys
 
 
-def makeprmset(path='.'):
-    path_cpp = path + '/gval_ctrlprm.cpp'
+def makeprmset(path='.', ftype='cpp'):
+    path_cpp = path + '/gval_ctrlprm.'+ ftype
     f = open(path_cpp, 'w')
-    f.write('#include "TcPch.h"\n')
-    f.write('#pragma hdrstop\n')
-    f.write('#include "head_ctrlprm.h"\n\n')
+    if ftype == 'cpp':
+        f.write('#include "TcPch.h"\n')
+        f.write('#pragma hdrstop\n')
+        f.write('#include "head_ctrlprm.h"\n\n')
+    elif ftype == 'c':
+        f.write('#include "head_common.h"\n\n')
 
     path_h = path + '/head_ctrlprm.h'
     f = open(path_h, 'w')
     f.write('#ifndef _HEAD_CTRLPRM_\n')
     f.write('#define _HEAD_CTRLPRM_\n\n')
     f.write('typedef struct {\n')
     f.write('	double	dA[2];\n')
@@ -729,21 +737,23 @@
     f.write('	double	dB[4];\n')
     f.write('	double	dInPre[3];\n')
     f.write('	double	dOutPre[3];\n')
     f.write('} TF3_INF;						// 3rd order TF information\n\n')
     f.write('#endif\n')
 
 
-def defprmset(tfz, prmSetName, path='.', mode='a'):
+def defprmset(tfz, prmSetName, path='.', ftype='cpp', mode='a'):
+    path_cpp = path + '/gval_ctrlprm.' + ftype
+    if isinstance(tfz, list):
+        tfz = np.array(tfz)
     if type(tfz).__module__ != 'numpy':
         num = tfz.num[0][0]
         den = tfz.den[0][0]
         if len(den) - len(num) > 0:
             num = np.concatenate([np.zeros(len(den) - len(num)), num])
-        path_cpp = path + '/gval_ctrlprm.cpp'
         f = open(path_cpp, mode)
         f.write('\n')
         if len(den) == 2:
             f.write('TF1_INF	')
             f.write(prmSetName)
             f.write(' = {\n')
             f.write('	{ ')
@@ -816,15 +826,14 @@
             f.write('extern TF3_INF	')
         f.write(prmSetName)
         f.write(';\n')
         f.write('\n#endif\n')
         f.close()
     else:
         if type(tfz[0]).__module__ != 'numpy':
-            path_cpp = path + '/gval_ctrlprm.cpp'
             f = open(path_cpp, mode)
             f.write('\n')
             den = tfz[0].den[0][0]
             if len(den) == 2:
                 f.write('TF1_INF	')
                 f.write(prmSetName)
                 f.write(' = {\n')
@@ -883,15 +892,14 @@
             elif len(den) == 4:
                 f.write('extern TF3_INF	')
             f.write(prmSetName)
             f.write(';\n')
             f.write('\n#endif\n')
             f.close()
         else:
-            path_cpp = path + '/gval_ctrlprm.cpp'
             f = open(path_cpp, mode)
             f.write('\n')
             den = tfz[0][0].den[0][0]
             if len(den) == 2:
                 f.write('TF1_INF	')
                 f.write(prmSetName)
                 f.write(' = {\n')
```

### Comparing `pylib-sakata-0.1.9/src/pylib_sakata/fft.py` & `pylib-sakata-0.2.0/src/pylib_sakata/fft.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     N_ave = int((Tlen - (Tfc * overlap)) / (Tfc * (1 - overlap)))  # data number for average
     data_array = []
     for i in range(N_ave):
         ps = int(x_ol * i)  # 切り出し位置をループ毎に更新
         data_array.append(data[ps:ps + framesize:1])  # 切り出し位置psからフレームサイズ分抽出して配列に追加
 
     # Hanning Window
-    han = signal.hanning(framesize)
+    han = signal.windows.hann(framesize)
     acf = 1 / (sum(han) / framesize)  # Amplitude Correction Factor
     for i in range(N_ave):
         data_array[i] = data_array[i] * han
 
     # FFT average
     fft_array = []
     for i in range(N_ave):
@@ -204,15 +204,16 @@
     # Mirror second-half part
     y_fft_flip = np.flip(np.conj(y_fft[1:len(y_fft)]))
     # Combine two parts
     y_fft_full = np.concatenate([y_fft, y_fft_flip])
 
     # Calculate time response of output
     y = np.real(np.fft.ifft(y_fft_full))
-    return y
+    t = np.linspace(0, (len(y) - 1) * dt, len(y))
+    return t, y
 
 
 def _floorpow2(x):
     # 2のべき乗に切り下げて丸め込み x>1
     return int(bin(1) + '0' * (len(bin(int(x))) - 3), base=2)
```

### Comparing `pylib-sakata-0.1.9/src/pylib_sakata/kinema.py` & `pylib-sakata-0.2.0/src/pylib_sakata/kinema.py`

 * *Files identical despite different names*

### Comparing `pylib-sakata-0.1.9/src/pylib_sakata/meas.py` & `pylib-sakata-0.2.0/src/pylib_sakata/meas.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,31 +33,40 @@
 
 
 def gettxtdata(filePath):
     """For example, data measured by PMAC"""
     f = open(filePath)
     line = f.readlines()
     f.close()
-    dataList = line[0].split()
-    dataValue = [[] for i in range(len(dataList))]
-    for n in range(len(dataList)):
-        dataline = []
-        for k in range(1, len(line)):
-            dataline.append(float(line[k].split()[n]))
-        dataValue[n] = np.array(dataline)
+    if (line[0].find('\t') == -1):
+        dataList = line[0][:-1].split('  ')
+        dataValue = [[] for i in range(len(dataList))]
+        for n in range(len(dataList)):
+            dataline = []
+            for k in range(1, len(line)):
+                dataline.append(float(line[k][:-1].split()[n]))
+            dataValue[n] = np.array(dataline)
+    else:
+        dataList = line[0][:-1].split('\t')[:-1]
+        dataValue = [[] for i in range(len(dataList))]
+        for n in range(len(dataList)):
+            dataline = []
+            for k in range(1, len(line)):
+                dataline.append(float(line[k][:-1].split(' \t')[:-1][n]))
+            dataValue[n] = np.array(dataline)
     dt = dataValue[0][1] - dataValue[0][0]
     t = np.linspace(0.0, len(dataValue[0]) * dt, int(len(dataValue[0])))
     return MeasData(dataList, dataValue, t, dt)
 
 
 def getmatdata(filePath):
     """For example, data measured by Matlab-base software"""
     matdata = io.loadmat(filePath)
     dataNum = len(matdata['dataY'][0])
-    Fs = matdata['samplefreq'][0][0]
+    Fs = matdata['samplefreq'][0][0] / matdata['downsample'][0][0]
     dt = 1.0/Fs
     dataList = [[] for i in range(dataNum)]
     dataValue = [[] for i in range(dataNum)]
     for k in range(dataNum):
         dataList[k] = matdata['dataY'][0][k][0][0]
         dataValue[k] = matdata['dataY'][0][k][1][0]
     t = np.linspace(0.0, len(dataValue[0]) * dt, int(len(dataValue[0])))
```

### Comparing `pylib-sakata-0.1.9/src/pylib_sakata/plot.py` & `pylib-sakata-0.2.0/src/pylib_sakata/plot.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 import numpy as np
 import matplotlib
 from control import matlab
 from matplotlib import pyplot as plt
 from .fft import FreqResp
 
+
 def plot_xy(ax, x, y, styl='-', col='b', width=1.5, alpha=1.0, xrange=None, yrange=None, xlabel=None, ylabel=None, legend=None, loc='best', title=None, xscale='linear', yscale='linear', labelouter=True):
     ax.set_xscale(xscale)
     ax.set_yscale(yscale)
     if xrange == None:
         xmin = min(x)
         xmax = max(x)
         xrange = [xmin, xmax]
@@ -29,15 +30,15 @@
         yrange = [ymin - 0.2*(ymax-ymin), ymax + 0.2*(ymax-ymin)]
     ax.set_xlim(xrange)
     ax.set_ylim(yrange)
     if xlabel != None:
         ax.set_xlabel(xlabel)
     if ylabel != None:
         ax.set_ylabel(ylabel)
-    ax.grid(b=True, which='both', axis='both')
+    ax.grid(visible=True, which='both', axis='both')
     # plot
     ax.plot(x, y, linestyle=styl, color=col, linewidth=width, alpha=alpha)
     # legend and title
     if legend != None:
         ax.legend(legend, loc=loc)
     if title != None:
         ax.set_title(title)
@@ -62,34 +63,39 @@
         magmax = max(magdb)
         magrange = [magmin - 0.2*(magmax-magmin), magmax + 0.2*(magmax-magmin)]
     ax_mag.set_xlim(freqrange)
     ax_mag.set_ylim(magrange)
     if ax_phase == None:
             ax_mag.set_xlabel('Frequency [Hz]')
     ax_mag.set_ylabel('Magnitude [dB]')
-    ax_mag.grid(b=True, which='both', axis='both')
+    ax_mag.grid(visible=True, which='both', axis='both')
     # mag plot
     ax_mag.plot(freq, magdb, linestyle=styl, color=col, linewidth=width, alpha=alpha)
     # legend and title
     if legend != None:
         ax_mag.legend(legend, loc=loc)
     if title != None:
         ax_mag.set_title(title)
     if labelouter == True:
         ax_mag.label_outer()
     
     if ax_phase != None:
         ax_phase.set_xscale('log')
         ax_phase.set_xlim(freqrange)
-        ax_phase.set_ylim(-200, 200)
+        # ax_phase.set_ylim(-200, 200)
+        ax_phase.set_ylim(-400, 40)
         ax_phase.set_xlabel('Frequency [Hz]')
         ax_phase.set_ylabel('Phase [deg]')
-        ax_phase.set_yticks([-180, -90, 0, 90, 180])
-        ax_phase.grid(b=True, which='both', axis='both')
+        # ax_phase.set_yticks([-180, -90, 0, 90, 180])
+        ax_phase.set_yticks([-360, -270, -180, -90, 0])
+        ax_phase.grid(visible=True, which='both', axis='both')
         # phase plot
+        for k in range(len(phasedeg)):
+            if phasedeg[k] > 0:
+                phasedeg[k] -= 360
         ax_phase.plot(freq, phasedeg, linestyle=styl, color=col, linewidth=width, alpha=alpha)
         if labelouter == True:
             ax_phase.label_outer()  
 
 
 def plot_tffrd(ax_mag, ax_phase, freqresp, styl='-', col='b', width=1.5, alpha=1.0, freqrange=None, magrange=None, legend=None, loc='best', title=None, labelouter=True, ax_coh=None, coh=None):
     mag = np.absolute(freqresp.resp)
@@ -107,46 +113,51 @@
         magmax = max(magdb)
         magrange = [magmin - 0.2*(magmax-magmin), magmax + 0.2*(magmax-magmin)]
     ax_mag.set_xlim(freqrange)
     ax_mag.set_ylim(magrange)
     if ax_phase == None and ax_coh == None:
             ax_mag.set_xlabel('Frequency [Hz]')
     ax_mag.set_ylabel('Magnitude [dB]')
-    ax_mag.grid(b=True, which='both', axis='both')
+    ax_mag.grid(visible=True, which='both', axis='both')
     # mag plot
     ax_mag.plot(freqresp.freq, magdb, linestyle=styl, color=col, linewidth=width, alpha=alpha)
     # legend and title
     if legend != None:
         ax_mag.legend(legend, loc=loc)
     if title != None:
         ax_mag.set_title(title)
     if labelouter == True:
         ax_mag.label_outer()
     
     if ax_phase != None:
         ax_phase.set_xscale('log')
         ax_phase.set_xlim(freqrange)
-        ax_phase.set_ylim(-200, 200)
+        # ax_phase.set_ylim(-200, 200)
+        ax_phase.set_ylim(-400, 40)
         if ax_coh == None:
             ax_phase.set_xlabel('Frequency [Hz]')
         ax_phase.set_ylabel('Phase [deg]')
-        ax_phase.set_yticks([-180, -90, 0, 90, 180])
-        ax_phase.grid(b=True, which='both', axis='both')
+        # ax_phase.set_yticks([-180, -90, 0, 90, 180])
+        ax_phase.set_yticks([-360, -270, -180, -90, 0])
+        ax_phase.grid(visible=True, which='both', axis='both')
         # phase plot
+        for k in range(len(phasedeg)):
+            if phasedeg[k] > 0:
+                phasedeg[k] -= 360
         ax_phase.plot(freqresp.freq, phasedeg, linestyle=styl, color=col, linewidth=width, alpha=alpha)
         if labelouter == True:
             ax_phase.label_outer()
         
     if ax_coh != None:
         ax_coh.set_xscale('log')
         ax_coh.set_xlim(freqrange)
         ax_coh.set_ylim(0, 1.2)
         ax_coh.set_xlabel('Frequency [Hz]')
         ax_coh.set_ylabel('Coherence [.]')
-        ax_coh.grid(b=True, which='both', axis='both')
+        ax_coh.grid(visible=True, which='both', axis='both')
         # coherence plot
         ax_coh.plot(freqresp.freq, coh, linestyle=styl, color=col, linewidth=width, alpha=alpha)
         if labelouter == True:
             ax_phase.label_outer()
 
 
 def plot_nyquist(ax, freqresp, styl='-', col='b', width=1.5, alpha=1.0, xrange=None, yrange=None, legend=None, loc='best', title=None, labelouter=True):
@@ -158,15 +169,15 @@
     if yrange == None:
         yrange = [-1.5, 1.5]
     ax.set_xlim(xrange)
     ax.set_ylim(yrange)
     ax.set_xlabel('Real')
     ax.set_ylabel('Imaginary')
     ax.set_aspect('equal', adjustable='box')
-    ax.grid(b=True, which='both', axis='both')
+    ax.grid(visible=True, which='both', axis='both')
     # plot
     ax.plot(x, y, linestyle=styl, color=col, linewidth=width, alpha=alpha)
     # legend and title
     if legend != None:
         ax.legend(legend, loc=loc)
     if title != None:
         ax.set_title(title)
@@ -180,22 +191,22 @@
     cy = np.cos(cir)
     # plot
     ax.plot(cx, cy, linestyle='-', color='gray', linewidth=0.5)
     ax.plot(0.5*cx-1, 0.5*cy, linestyle='-', color='gray', linewidth=0.5)
     ax.plot(-1.0, 0.0, marker='x', color='r')
     
     
-def makefig(dpi=100, popwin=False):
-    fig = plt.figure(dpi=dpi)
+def makefig(dpi=100, figsize=(6, 4), popwin=False):
+    fig = plt.figure(dpi=dpi, figsize=figsize)
     if popwin != False:
         mngr = plt.get_current_fig_manager()
         # to put it into the upper left corner for example:
-        mngr.window.setGeometry(50,250,640, 545)
+        mngr.window.geometry(str(figsize[0])+'00x'+str(figsize[1])+'00+0+0')
     return fig
 
 
 def savefig(figName):
-    plt.savefig(figName)
+    plt.savefig(figName, bbox_inches='tight')
 
 
 def showfig():
     plt.show()
```

### Comparing `pylib-sakata-0.1.9/src/pylib_sakata.egg-info/PKG-INFO` & `pylib-sakata-0.2.0/src/pylib_sakata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 Metadata-Version: 2.1
 Name: pylib-sakata
-Version: 0.1.9
+Version: 0.2.0
 Summary: Control system design and analysis package
 Home-page: https://github.com/Koichi-Sakata/pylib_sakata
 Author: Koichi Sakata
 Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.8
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-pylib-sakata User's Manual version-0.1.9
+pylib-sakata User's Manual version-0.2.0
 ===
 
-<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
-
 <!-- code_chunk_output -->
 
-- [pylib-sakata User's Manual version-0.1.9](#pylib-sakata-users-manual-version-019)
 - [1. Introduction](#1-introduction)
 - [2. Environment Setup](#2-environment-setup)
   - [2.1. Installation of Python](#21-installation-of-python)
   - [2.2. Installation  of required Python libraries](#22-installation--of-required-python-libraries)
   - [2.3. Installation of pylib-sakata](#23-installation-of-pylib-sakata)
   - [2.4. Installation of IDE for Python](#24-installation-of-ide-for-python)
     - [2.4.1. Visual Studio Code (VSCode)](#241-visual-studio-code-vscode)
@@ -32,15 +27,15 @@
       - [2.4.2.1. Installation of Spyder](#2421-installation-of-spyder)
       - [2.4.2.2. Initial setting of Spyder](#2422-initial-setting-of-spyder)
     - [2.4.3. PyCharm](#243-pycharm)
       - [2.4.3.1. Installation of PyCharm](#2431-installation-of-pycharm)
       - [2.4.3.2. Initial setting of PyCharm](#2432-initial-setting-of-pycharm)
     - [2.4.4. Comparison between  VSCode and Spyder and PyCharm](#244-comparison-between--vscode-and-spyder-and-pycharm)
   - [2.5. Getting started](#25-getting-started)
-- [3. pylib_sakata.ctrl](#3-pylib_sakatactrl)
+- [3. pylib\_sakata.ctrl](#3-pylib_sakatactrl)
   - [3.1. ZpkModel](#31-zpkmodel)
   - [3.2. tf](#32-tf)
   - [3.3. ss](#33-ss)
   - [3.4. zpk](#34-zpk)
   - [3.5. tf2ss](#35-tf2ss)
   - [3.6. tf2zpk](#36-tf2zpk)
   - [3.7. ss2tf](#37-ss2tf)
@@ -66,57 +61,60 @@
   - [3.27. pfopt](#327-pfopt)
   - [3.28. dob](#328-dob)
   - [3.29. zpetc](#329-zpetc)
   - [3.30. filt](#330-filt)
   - [3.31. minreal](#331-minreal)
   - [3.32. makeprmset](#332-makeprmset)
   - [3.33. defprmset](#333-defprmset)
-- [4. pylib_sakata.fft](#4-pylib_sakatafft)
+- [4. pylib\_sakata.fft](#4-pylib_sakatafft)
   - [4.1. FreqResp](#41-freqresp)
   - [4.2. fft](#42-fft)
-  - [4.3. fft_ave](#43-fft_ave)
+  - [4.3. fft\_ave](#43-fft_ave)
   - [4.4. tfestimate](#44-tfestimate)
   - [4.5. frdresize](#45-frdresize)
   - [4.6. frdsim](#46-frdsim)
-- [5. pylib_sakta.meas](#5-pylib_saktameas)
+- [5. pylib\_sakata.meas](#5-pylib_sakatameas)
   - [5.1. MeasData](#51-measdata)
   - [5.2. getcsvdata](#52-getcsvdata)
   - [5.3. gettxtdata](#53-gettxtdata)
   - [5.4. getmatdata](#54-getmatdata)
   - [5.5. getdata](#55-getdata)
   - [5.6. getdataindex](#56-getdataindex)
   - [5.7. measdata2frd](#57-measdata2frd)
-- [6. pylib_sakata.traj](#6-pylib_sakatatraj)
+- [6. pylib\_sakata.traj](#6-pylib_sakatatraj)
   - [6.1. TrajInf](#61-trajinf)
-  - [6.2. traj4th](#62-traj4th)
-- [7. pylib_sakata.plot](#7-pylib_sakataplot)
-  - [7.1. plot_xy](#71-plot_xy)
-  - [7.2. plot_tf](#72-plot_tf)
-  - [7.3. plot_tffrd](#73-plot_tffrd)
-  - [7.4. plot_nyquist](#74-plot_nyquist)
-  - [7.5. plot_nyquist_assistline](#75-plot_nyquist_assistline)
+  - [6.2. traj3rd](#62-traj3rd)
+  - [6.3. traj3rd2](#63-traj3rd2)
+  - [6.4. traj4th](#64-traj4th)
+  - [6.5. trajSinStep](#65-trajsinstep)
+- [7. pylib\_sakata.plot](#7-pylib_sakataplot)
+  - [7.1. plot\_xy](#71-plot_xy)
+  - [7.2. plot\_tf](#72-plot_tf)
+  - [7.3. plot\_tffrd](#73-plot_tffrd)
+  - [7.4. plot\_nyquist](#74-plot_nyquist)
+  - [7.5. plot\_nyquist\_assistline](#75-plot_nyquist_assistline)
   - [7.6. makefig](#76-makefig)
   - [7.7. savefig](#77-savefig)
   - [7.8. showfig](#78-showfig)
-- [8. pylib_sakata.init](#8-pylib_sakatainit)
-  - [8.1. close_all](#81-close_all)
-  - [8.2. clear_all](#82-clear_all)
+- [8. pylib\_sakata.init](#8-pylib_sakatainit)
+  - [8.1. close\_all](#81-close_all)
+  - [8.2. clear\_all](#82-clear_all)
 
 <!-- /code_chunk_output -->
 
-# 1. Introduction
+## 1. Introduction
 
-The pylib-sakata package is a set of python classes and functions that make the python-control package more convenient. This package provide practical level's tools to design controls and  to analysis of performance and stability of SISO LTI systems. These development environments are available on free.
+The pylib-sakata package is a set of python classes and functions that make the python-control package more convenient. This package provides practical level's tools to design controls and  to analysis of performance and stability of SISO LTI systems. These development environments are available on free.
 
-# 2. Environment Setup
+## 2. Environment Setup
 
-## 2.1. Installation of Python
+### 2.1. Installation of Python
 Python installation exe file can be downloaded [HERE](https://www.python.org/downloads/) for Windows. Check "Add Python 3.x to PATH" when you install Python.
 
-## 2.2. Installation  of required Python libraries
+### 2.2. Installation  of required Python libraries
 
 The pylib-sakata package requires [numpy](http://www.numpy.org), [scipy](http://www.scipy.org), [matplotlib](https://matplotlib.org), [pandas](https://pandas.pydata.org/), and [python-control](https://github.com/python-control/python-control). In addition, some routines require the [slycot](https://github.com/python-control/Slycot) library in order to implement more advanced features. 
 First, pip should be upgraded by the following command on the command prompt for Windows OS.
 ```shell
 python -m pip install --upgrade pip
 ```
 For Linux OS, pip can be upgraded by the following command on the shell.
@@ -129,89 +127,89 @@
 pip install scipy
 pip install matplotlib
 pip install pandas
 pip install control
 ```
 If those libraries can not be installed, please use pip3 instead of pip.
 
-## 2.3. Installation of pylib-sakata
+### 2.3. Installation of pylib-sakata
 
 The [pylib-sakata](https://github.com/Koichi-Sakata/pylib_sakata) package can be installed using pip using pip as following on the command prompt or on the shell.
 
 ```shell
 pip install pylib-sakata
 ```
 
-## 2.4. Installation of IDE for Python
+### 2.4. Installation of IDE for Python
 
 There are three recommended IDEs.
 
-### 2.4.1. Visual Studio Code (VSCode)
+#### 2.4.1. Visual Studio Code (VSCode)
 Although VSCode is actually an editor, it is available as Python IDE due to extensions. It is recommended to install it easily because of the versatility of extensions. The following figure shows VSCode IDE window.
 
 <img src="figure\vscode_disp.png" alt="vscode_disp" style="zoom: 33%;" />
 
-#### 2.4.1.1. Installation of VSCode
+##### 2.4.1.1. Installation of VSCode
 The latest version of VSCode installation exe file can be downloaded [HERE](https://code.visualstudio.com/) for Windows OS.
 For Linux OS, VSCode can be installed by the following command on the shell.
 ```shell
 $ sudo apt update 
 $ sudo apt install code
 ```
 
-#### 2.4.1.2. Initial setting of VSCode
+##### 2.4.1.2. Initial setting of VSCode
 1. Install Python extension for Visual Studio Code from extensions in the activity bar on the left side.
 1. Command (Ctrl+Shift+P) to open the command palette.
 1. Select your installed python.exe on  "Python: select interpreter".
 
-### 2.4.2. Spyder
+#### 2.4.2. Spyder
 Spyder is an IDE like MATLAB. If you are used to MATLAB, this IDE is recommended. The following figure shows Spyder IDE window.
 
 <img src="figure\spyder_disp.png" alt="spyder_disp" style="zoom: 33%;" />
 
-#### 2.4.2.1. Installation of Spyder
+##### 2.4.2.1. Installation of Spyder
 The latest version of Spyder installation exe file can be downloaded [HERE](https://www.spyder-ide.org/) for Windows OS.
 For Linux OS, Spyder can be installed by the following command on the shell.
 
 ```shell
 $ sudo apt update 
 $ sudo apt install spyder3
 ```
 
-#### 2.4.2.2. Initial setting of Spyder
+##### 2.4.2.2. Initial setting of Spyder
 1. Open Tools>Preferences>Python interpreter.
 1. Check "Use the following Python interpreter."
 1. Enter the path of your installed python.exe.
 1. Install spyder-kernels for your python version by the following command `pip install spyder-kernels==2.0.*` on the command prompt or on the shell.
 1. Reboot your PC.
 
-### 2.4.3. PyCharm
+#### 2.4.3. PyCharm
 Professional version is charged. Community version is free. Community version is enough for control system development. The following figure shows PyCharm window.
 
 <img src="figure\pycharm_disp.png" alt="spyder_disp" style="zoom: 33%;" />
 
-#### 2.4.3.1. Installation of PyCharm
+##### 2.4.3.1. Installation of PyCharm
 The latest version of PyCharm installation exe file can be downloaded [HERE](https://www.jetbrains.com/pycharm/download/). 
 
-#### 2.4.3.2. Initial setting of PyCharm
+##### 2.4.3.2. Initial setting of PyCharm
 It is not necessary.
 
-### 2.4.4. Comparison between  VSCode and Spyder and PyCharm
+#### 2.4.4. Comparison between  VSCode and Spyder and PyCharm
 
 |                    |        VSCode       |      Spyder       |     PyCharm       |
 | ------------------ | :-----------------: | :---------------: | :---------------: |
 | Cost               |        Free         |       Free        |    Free/Paid      |
 | Boot time          |        Fast         |       Slow        |       Normal      |
 | Processing speed   |        Fast         |       Normal      |       Normal      |
 | REPL mode          | need to switch REPL terminal  | Available | Available |
 | Variable Explorer  | Available on Jupyter terminal | Available (Class variables are invisible.) | Available |
 
 Spyder is more suitable than VSCode for early debugging. On the other hand, VSCode is stress-free than Spyder for late debugging you do not need to check inter states of variables. PyCharm is generally well-balanced. My recommendation is PyCharm.
 
-## 2.5. Getting started
+### 2.5. Getting started
 The pylib-sakata package can be imported as follows.
 ```python
 >>> import pylib_sakata
 ```
 This package consists of six modules as follows.
 1. **ctrl**: to design controllers and filters
 1. **fft**: to analysis FFT
@@ -228,17 +226,17 @@
 >>> from pylib_sakata import traj
 >>> from pylib_sakata import plot
 >>> from pylib_sakata import init
 ```
 
 Example codes are [HERE](https://github.com/Koichi-Sakata/pylib_sakata/tree/main/example).
 
-# 3. pylib_sakata.ctrl
+## 3. pylib_sakata.ctrl
 
-## 3.1. ZpkModel
+### 3.1. ZpkModel
 
 class pylib_sakata.ctrl.**ZpkModel**(*z, p, k, dt=0*)
 
 - Parameters:
   - z: zeros array of the LTI model
   - p: poles array of the LTI model
   - k: gain of the LTI model. Note: the gain is not system dc gain but coefficient of monic polynomials. This is different from the definition of dc gain in TransferFunction class.
@@ -295,15 +293,15 @@
 - \__**pow**__(*other*)
 	A zpk model to the power of x.
 
 - **feedback**(*other=1, sys='S'*)
 	Calculate the feedback system that consist of two zpk model (P: self and C: other).
 	sys: FB type (Optional), Default: 'S', Set in 'S': sensitivity function, 'T': complementary sensitivity function, 'SP': response from input disturbance to output
 
-## 3.2. tf
+### 3.2. tf
 
 pylib_sakata.ctrl.**tf**(*num, den, dt=0*)
 
 This function calls **tf** function in control library.
 
 - Parameters:
   - num: polynomial coefficients of the numerator of the LTI model
@@ -317,15 +315,15 @@
 >>> print(ctrl.tf([1., 2.], [3., 4., 5.]))
 
      s + 2
 ---------------
 3 s^2 + 4 s + 5
 ```
 
-## 3.3. ss
+### 3.3. ss
 
 pylib_sakata.ctrl.**ss**(*A, B, C, D, dt=0*)
 
 This function calls **ss** function in control library.
 
 - Parameters:
   - A, B, C, D: state space matrices
@@ -343,15 +341,15 @@
      [7.]]
 
 C = [[6. 8.]]
 
 D = [[9.]]
 ```
 
-## 3.4. zpk
+### 3.4. zpk
 
 pylib_sakata.ctrl.**zpk**(*z, p, k, dt=0*)
 
 - Parameters:
   - A, B, C, D: state space matrices
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
 - Returns:
@@ -362,21 +360,21 @@
 >>> ctrl.zpk([-1., -2.], [-3., -4., -5.], 2.)
 
       (s+1)(s+2)
 2 * ---------------
     (s+3)(s+4)(s+5)
 ```
 
-## 3.5. tf2ss
+### 3.5. tf2ss
 
-pylib_sakata.ctrl.**tf2ss**(*tf, form='reachable'*)
+pylib_sakata.ctrl.**tf2ss**(*tf, form=None*)
 
 - Parameters:
   - tf: instance of TransferFunction class
-  - form: canonical form (Optional), Default: reachable. You can select the canonical form in reachable, observable, and modal.
+  - form: canonical form (Optional), you can select the canonical form in 'reachable', 'observable', and 'modal'.
 - Returns:
   - out: instance of StateSpace class
 
 **Examples**
 ```python
 >>> Sys_tf = ctrl.tf([1., 2.], [3., 4., 5.])
 >>> print(ctrl.tf2ss(Sys_tf))
@@ -387,15 +385,15 @@
      [0.]]
 
 C = [[0.33333333 0.66666667]]
 
 D = [[0.]]
 ```
 
-## 3.6. tf2zpk
+### 3.6. tf2zpk
 
 pylib_sakata.ctrl.**tf2zpk**(*tf*)
 
 - Parameters:
   - tf: instance of TransferFunction class
 - Returns:
   - out: instance of ZpkModel class
@@ -407,15 +405,15 @@
 
                        (s+2)
 0.3333 * ----------------------------------
          (s+0.6667+1.106j)(s+0.6667-1.106j)
 ```
 
 
-## 3.7. ss2tf
+### 3.7. ss2tf
 
 pylib_sakata.ctrl.**ss2tf**(*ss*)
 
 - Parameters:
   - ss: instance of StateSpace class
 - Returns:
   - out: instance of TransferFunction class
@@ -426,15 +424,15 @@
 >>> print(ctrl.ss2tf(Sys_ss))
 
 9 s^2 + 113 s + 118
 -------------------
    s^2 + 3 s + 2
 ```
 
-## 3.8. ss2zpk
+### 3.8. ss2zpk
 
 pylib_sakata.ctrl.**ss2zpk**(*ss*)
 
 - Parameters:
   - ss: instance of StateSpace class
 - Returns:
   - out: instance of ZpkModel class
@@ -445,15 +443,15 @@
 >>> ctrl.ss2zpk(Sys_ss)
 
     (s+11.41)(s+1.149)
 9 * ------------------
         (s+2)(s+1)
 ```
 
-## 3.9. zpk2tf
+### 3.9. zpk2tf
 
 pylib_sakata.ctrl.**zpk2tf**(*zpk*)
 
 - Parameters:
   - zpk: instance of ZpkModel class
 - Returns:
   - out: instance of TransferFunction class
@@ -464,15 +462,15 @@
 >>> print(ctrl.zpk2tf(Sys_zpk))
 
     2 s^2 + 6 s + 4
 ------------------------
 s^3 + 12 s^2 + 47 s + 60
 ```
 
-## 3.10. zpk2ss
+### 3.10. zpk2ss
 
 pylib_sakata.ctrl.**zpk2ss**(*zpk, form='reachable'*)
 
 - Parameters:
   - zpk: instance of ZpkModel class
   - form: canonical form (Optional), Default: reachable. You can select the canonical form in reachable, observable, and modal.
 - Returns:
@@ -491,15 +489,15 @@
      [0.]]
 
 C = [[2. 6. 4.]]
 
 D = [[0.]]
 ```
 
-## 3.11. sys2frd
+### 3.11. sys2frd
 
 pylib_sakata.ctrl.**sys2frd**(*sys, freq*)
 
 - Parameters:
   - sys: LTI model (StateSpace or TransferFunction or ZpkModel)
   - freq: 1-D array frequency data [Hz]
 - Returns:
@@ -525,15 +523,15 @@
 freq = array([   1.            1.00069108    1.00138264 ...  998.61926487  999.30939397
  1000.        ])
 resp = array([1.89109027e-01-0.06951671j 1.89033162e-01-0.06962001j
  1.88957165e-01-0.0697232j  ... 4.57206511e-07-0.00031875j
  4.56575231e-07-0.00031853j 4.55944822e-07-0.00031831j])
 ```
 
-## 3.12. feedback
+### 3.12. feedback
 
 pylib_sakata.ctrl.**feedback**(*sysP, sysC, sys='S'*)
 
 This function is for calculating the feedback system that consist of two LTI model (P: plant and C: controller).
 
 - Parameters:
   - sysP: LTI model (StateSpace or TransferFunction or ZpkModel) of the plant
@@ -558,15 +556,15 @@
 >>> ctrl.feedback(P_zpk, C_zpk)
 
                      s(s+2)(s+2)s
 1 * -----------------------------------------------
     (s+1)(s+1-0.0001508j)(s+1+0.0001508j)(s+0.9998)
 ```
 
-## 3.13. frdfeedback
+### 3.13. frdfeedback
 
 pylib_sakata.ctrl.**frdfeedback**(*frdP, frdC, sys='S'*)
 
 This function is for calculating the feedback system that consist of two freqresp (P: plant and C: controller).
 
 - Parameters:
   - frdP: 1-D array complex data of the frequency response of the plant
@@ -586,15 +584,15 @@
 >>> C_frd = ctrl.tf2frd(C_tf, freq)
 >>> ctrl.frdfeedback(P_frd, C_frd)
 array([1.04746047+1.56990662e-02j, 1.04739933+1.56671729e-02j,
        1.04733826+1.56353434e-02j, ..., 1.00000005+1.61927479e-11j,
        1.00000005+1.61592227e-11j, 1.00000005+1.61257668e-11j])
 ```
 
-## 3.14. c2d
+### 3.14. c2d
 
 pylib_sakata.ctrl.**c2d**(*sysC, dt, method='tustin'*)
 
 The matched method of **c2d** in control library does not supported for pure integrals and pure derivatives because of dc gain inf error. This function solved this problem.
 
 - Parameters:
   - sysC: continuous time LTI model (StateSpace or TransferFunction or ZpkModel) of the plant
@@ -602,44 +600,40 @@
   - method: discretized method (Optional), Default: 'tustin', set a method in 'tustin', 'matched', 'zoh', and etc.
 - Returns:
   - out: discrete time LTI model (StateSpace or TransferFunction or ZpkModel) of the feedback system
 
 **Examples**
 ```python
 >>> C_tf = ctrl.tf([1., 3., 2.], [1., 3., 0.])
->>> print(ctrl.c2d_matched(C_tf, 0.001))
+>>> print(ctrl.c2d(C_tf, 0.001, 'matched'))
 
 z^2 - 1.997 z + 0.997
 ---------------------
 z^2 - 1.997 z + 0.997
 
 dt = 0.001
 ```
 ```python
 >>> C_zpk = ctrl.zpk([-1., -2.,], [0., -3.,], 1.)
->>> ctrl.c2d_matched(C_zpk, 0.001)
+>>> ctrl.c2d(C_zpk, 0.001, 'matched')
 
     (z-0.999)(z-0.998)
 1 * ------------------
       (z-1)(z-0.997)
 
 dt = 0.001
 ```
 
-## 3.15. pi
+### 3.15. pi
 
 pylib_sakata.ctrl.**pi**(*freq, zeta, L, R, dt=None, method='tustin'*)
 
 This function is for design of a PI controller.
-$$
-C_{PI}(s) = K_P + \frac{K_I}{s} = \frac{b_1s+b_0}{s}
-$$
-$$
-P(s) = \frac{1}{Ls+R}
-$$
+$$C_{PI}(s) = K_P + \frac{K_I}{s} = \frac{b_1s+b_0}{s}$$
+$$P(s) = \frac{1}{Ls+R}$$
 
 - Parameters:
   - freq: frequency[Hz] of the pole pair of the feedback system with the PI controller
   - zeta: damping of the pole pair of the feedback system with the PI controller
   - L: inductance[H] of the plant
   - R: resistance[$\Omega$] of the plant
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
@@ -661,25 +655,21 @@
 2844 z + 1104
 -------------
     z - 1
 
 dt = 0.001
 ```
 
-## 3.16. pd
+### 3.16. pd
 
 pylib_sakata.ctrl.**pd**(*freq1, freq2, zeta2, M, C, K, dt=None, method='tustin'*)
 
 This function is for design of a PD controller.
-$$
-C_{PID}(s) = K_P + \frac{K_D s}{\tau_D s+1} = \frac{b_1s+b_0}{s+a_1}
-$$
-$$
-P(s) = \frac{1}{Ms^2+Cs+K}
-$$
+$$C_{PD}(s) = K_P + \frac{K_D s}{\tau_D s+1} = \frac{b_1s+b_0}{s+a_0}$$
+$$P(s) = \frac{1}{Ms^2+Cs+K}$$
 
 - Parameters:
   - freq1: frequency[Hz] of the first pole of the feedback system with the PD controller
   - freq2: frequency[Hz] of the second pole pair of the feedback system with the PD controller
   - zeta2: damping of the second pole pair of the feedback system with the PD controller
   - M: mass[kg] of the plant
   - C: viscosity[N/(m/s)] of the plant
@@ -703,25 +693,21 @@
 1.653e+04 z - 1.607e+04
 -----------------------
       z - 0.8641
 
 dt = 0.001
 ```
 
-## 3.17. pid
+### 3.17. pid
 
 pylib_sakata.ctrl.**pid**(*freq1, zeta1, freq2, zeta2, M, C, K, dt=None, method='tustin'*)
 
 This function is for design of a PID controller.
-$$
-C_{PID}(s) = K_P + \frac{K_I}{s} + \frac{K_D s}{\tau_D s+1} = \frac{b_2s^2+b_1s+b_0}{s^2+a_1s}
-$$
-$$
-P(s) = \frac{1}{Ms^2+Cs+K}
-$$
+$$C_{PID}(s) = K_P + \frac{K_I}{s} + \frac{K_D s}{\tau_D s+1} = \frac{b_2s^2+b_1s+b_0}{s^2+a_1s}$$
+$$P(s) = \frac{1}{Ms^2+Cs+K}$$
 
 - Parameters:
   - freq1: frequency[Hz] of the first pole pair of the feedback system with the PID controller
   - zeta1: damping of the first pole pair of the feedback system with the PID controller
   - freq2: frequency[Hz] of the second pole pair of the feedback system with the PID controller
   - zeta2: damping of the second pole pair of the feedback system with the PID controller
   - M: mass[kg] of the plant
@@ -746,22 +732,20 @@
 3.32e+04 z^2 - 6.485e+04 z + 3.167e+04
 --------------------------------------
         z^2 - 1.811 z + 0.8111
 
 dt = 0.001
 ```
 
-## 3.18. pl1st
+### 3.18. pl1st
 
 pylib_sakata.ctrl.**pl1st**(*freq1, freq2, dt=None, method='tustin'*)
 
 This function is for design of a first order phase lead filter.
-$$
-F_{PL}(s) = \frac{f_2}{f_1} * \frac{s+2\pi f_1}{s+2\pi f_2}
-$$
+$$F_{PL}(s) = \frac{f_2}{f_1} * \frac{s+2\pi f_1}{s+2\pi f_2}$$
 
 - Parameters:
   - freq1: frequency[Hz] of numerator of the phase lead filter
   - freq2: frequency[Hz] of denominator of the phase lead filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
@@ -781,22 +765,20 @@
         (z-0.7285)
 1.761 * ----------
         (z-0.5219)
 
 dt = 0.001
 ```
 
-## 3.19. pl2nd
+### 3.19. pl2nd
 
 pylib_sakata.ctrl.**pl2nd**(*freq1, zeta1, freq2, zeta2, dt=None, method='tustin'*)
 
 This function is for design of a second order phase lead filter.
-$$
-F_{PL^2}(s) = \left( \frac{f_2}{f_1} \right)^2 * \frac{s^2+2\zeta_1 (2\pi f_1)s+(2\pi f_1)^2}{s^2+2\zeta_2 (2\pi f_2)s+(2\pi f_2)^2}
-$$
+$$F_{PL^2}(s) = \left( \frac{f_2}{f_1} \right)^2 * \frac{s^2+2\zeta_1 (2\pi f_1)s+(2\pi f_1)^2}{s^2+2\zeta_2 (2\pi f_2)s+(2\pi f_2)^2}$$
 
 - Parameters:
   - freq1: frequency[Hz] of numerator of the phase lead filter
   - zeta1: damping of numerator of the phase lead filter
   - freq2: frequency[Hz] of denominator of the phase lead filter
   - zeta2: damping of denominator of the phase lead filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
@@ -818,22 +800,20 @@
 1.618 z^2 - 2.536 z + 1.046
 ---------------------------
   z^2 - 1.172 z + 0.4283
 
 dt = 0.001
 ```
 
-## 3.20. lpf1st
+### 3.20. lpf1st
 
 pylib_sakata.ctrl.**lpf1st**(*freq, dt=None, method='tustin'*)
 
 This function is for design of a first order low pass filter.
-$$
-F_{LP}(s) = \frac{2\pi f}{s+2\pi f}
-$$
+$$F_{LP}(s) = \frac{2\pi f}{s+2\pi f}$$
 
 - Parameters:
   - freq: frequency[Hz] of the low pass filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
   - out: instance of TransferFunction class of the low pass filter
@@ -852,22 +832,20 @@
 0.2391 z + 0.2391
 -----------------
    z - 0.5219
 
 dt = 0.001
 ```
 
-## 3.21. lpf2nd
+### 3.21. lpf2nd
 
 pylib_sakata.ctrl.**lpf2nd**(*freq, zeta, dt=None, method='tustin'*)
 
 This function is for design of a second order low pass filter.
-$$
-F_{LP^2}(s) = \frac{(2\pi f)^2}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}
-$$
+$$F_{LP^2}(s) = \frac{(2\pi f)^2}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}$$
 
 - Parameters:
   - freq: frequency[Hz] of the low pass filter
   - zeta1: damping of the low pass filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
@@ -887,22 +865,20 @@
 0.06415 z^2 + 0.1283 z + 0.06415
 --------------------------------
      z^2 - 1.172 z + 0.4283
 
 dt = 0.001
 ```
 
-## 3.22. hpf1st
+### 3.22. hpf1st
 
 pylib_sakata.ctrl.**hpf1st**(*freq, dt=None, method='tustin'*)
 
 This function is for design of a first order high pass filter.
-$$
-F_{HP}(s) = 1 - F_{LP}(s) = \frac{s}{s+2\pi f}
-$$
+$$F_{HP}(s) = 1 - F_{LP}(s) = \frac{s}{s+2\pi f}$$
 
 - Parameters:
   - freq: frequency[Hz] of the high pass filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
   - out: instance of TransferFunction class of the high pass filter
@@ -921,22 +897,20 @@
 0.7609 z - 0.7609
 -----------------
    z - 0.5219
 
 dt = 0.001
 ```
 
-## 3.23. hpf2nd
+### 3.23. hpf2nd
 
 pylib_sakata.ctrl.**hpf2nd**(*freq, zeta, dt=None, method='tustin'*)
 
 This function is for design of a second order high pass filter.
-$$
-F_{HP^2}(s) = 1 - F_{LP^2}(s) = \frac{s^2+2\zeta (2\pi f)s}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}
-$$
+$$F_{HP^2}(s) = 1 - F_{LP^2}(s) = \frac{s^2+2\zeta (2\pi f)s}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}$$
 
 - Parameters:
   - freq: frequency[Hz] of the high pass filter
   - zeta1: damping of the high pass filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'tustin', set a method if dt > 0
 - Returns:
@@ -956,22 +930,20 @@
 0.9358 z^2 - 1.3 z + 0.3641
 ---------------------------
   z^2 - 1.172 z + 0.4283
 
 dt = 0.001
 ```
 
-## 3.24. nf
+### 3.24. nf
 
 pylib_sakata.ctrl.**nf**(*freq, zeta, depth, dt=None, method='matched'*)
 
 This function is for design of notch filters.
-$$
-F_{notch}(s) = \frac{s^2+2d\zeta (2\pi f)s+(2\pi f)^2}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}
-$$
+$$F_{notch}(s) = \frac{s^2+2d\zeta (2\pi f)s+(2\pi f)^2}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}$$
 
 - Parameters:
   - freq: array of frequency[Hz] of the notch filters
   - zeta: array of damping of the notch filters
   - depth: array of depth of the notch filters (0 < depth < 1)
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
   - method: discretized method (Optional), Default: 'matched', set a method if dt > 0
@@ -990,22 +962,20 @@
 >>> ctrl.nf([100., 200., 300.], [0.02, 0.02, 0.02], [0.01, 0.01, 0.01], 0.001)
 array([TransferFunction(array([ 0.9876627 , -1.59787102,  0.9874145 ]), array([ 1.        , -1.59797428,  0.97518046]), 0.001),
        TransferFunction(array([ 0.97553399, -0.6027617 ,  0.97504375]), array([ 1.        , -0.60316088,  0.95097692]), 0.001),
        TransferFunction(array([0.96362486, 0.59532837, 0.96289858]), array([1.        , 0.59447771, 0.92737411]), 0.001)],
       dtype=object)
 ```
 
-## 3.25. pf
+### 3.25. pf
 
 pylib_sakata.ctrl.**pf**(*freq, zeta, k, phi, dt=None, method='tustin'*)
 
 This function is for design of peak filters ([resonant filters](https://ieeexplore.ieee.org/document/4291569)).
-$$
-F_{peak}(s) = \frac{k(s^2-\phi s)}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}
-$$
+$$F_{peak}(s) = \frac{k(s^2-\phi s)}{s^2+2\zeta (2\pi f)s+(2\pi f)^2}$$
 
 - Parameters:
   - freq: array of frequency[Hz] of the peak filters
   - zeta: array of damping of the peak filters
   - k: array of peak width of the peak filters
   - phi: array of phase lead of the peak filter
   - dt: sampling time of the LTI model (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
@@ -1026,15 +996,15 @@
 >>> ctrl.pf([2., 3., 5.], [0.001, 0.001, 0.001], [-0.00025695, -0.00049616, 0.0003898], [860.21053991, 633.22924516, -1090.49879949], 0.001)
 array([TransferFunction(array([-0.00014643,  0.00051387, -0.00036745]), array([ 1.        , -1.99981696,  0.99997487]), 0.001),
        TransferFunction(array([-0.00033903,  0.00099221, -0.00065318]), array([ 1.        , -1.99960704,  0.9999623 ]), 0.001),
        TransferFunction(array([ 0.00060217, -0.00077938,  0.00017721]), array([ 1.        , -1.9989505 ,  0.99993719]), 0.001)],
       dtype=object)
 ```
 
-## 3.26. pfoptparam
+### 3.26. pfoptparam
 pylib_sakata.ctrl.**pfoptparam**(freq, zeta, depth, sysT)
 
 This function is for getting parameters of optimized peak filters ([resonant filters](https://ieeexplore.ieee.org/document/4291569)).
 
 - Parameters:
   - freq: array of frequency[Hz] of the peak filters
   - zeta: array of damping of the peak filters
@@ -1051,15 +1021,15 @@
 >>> Ps = ctrl.tf([1.], [2., 10., 0.])
 >>> Cs = ctrl.pid(10., 1., 10., 0.7, 2., 10., 0.)
 >>> ctrl.pfoptparam([2., 3., 5.], [0.001, 0.001, 0.001], [0.1, 0.1, 0.1], ctrl.feedback(Ps, Cs, sys='T'))
 The common pole-zeros of the zpk model have been deleted.
 ([2.0, 3.0, 5.0], [0.001, 0.001, 0.001], array([-0.00025695, -0.00049616,  0.0003898 ]), array([  860.21053991,   633.22924516, -1090.49879949]))
 ```
 
-## 3.27. pfopt
+### 3.27. pfopt
 
 pylib_sakata.ctrl.**pfopt**(*freq, zeta, depth, sysT, dt=None, method='tustin'*)
 
 This function is for design of optimized peak filters ([resonant filters](https://ieeexplore.ieee.org/document/4291569)).
 
 - Parameters:
   - freq: array of frequency[Hz] of the peak filters
@@ -1087,33 +1057,32 @@
 The common pole-zeros of the zpk model have been deleted.
 array([TransferFunction(array([ 0.0049857 , -0.00972818,  0.00474248]), array([ 1.        , -1.99981696,  0.99997487]), 0.001),
        TransferFunction(array([ 0.00740923, -0.01446026,  0.00705103]), array([ 1.        , -1.99960704,  0.9999623 ]), 0.001),
        TransferFunction(array([ 0.01227286, -0.02398427,  0.01171141]), array([ 1.        , -1.9989505 ,  0.99993719]), 0.001)],
       dtype=object)
 ```
 
-## 3.28. dob
+### 3.28. dob
 pylib_sakata.ctrl.**dob**(*freq, zeta, M, C, K, dt, nd = 0*)
 
 This function is for design of a discrete-time disturbance observer (DOB).
-$$
-\hat{d} = -z^{n_d} Q[z] u + Q[z] P^{-1}[z] y
-$$
+$$\hat{d} = -z^{-n_d} Q[z] u + Q[z] P^{-1}[z] y$$
+
 Here, it is defined that disturbance $d$ is injected in the system as plus sign.
 
 - Parameters:
   - freq: frequency[Hz] of the pole pair of the DOB
   - zeta: damping of the pole pair of the DOB
   - M: mass[kg] of the plant
   - C: viscosity[N/(m/s)] of the plant
   - K: stiffness[N/m] of the plant
   - dt: sampling time of the system
   - nd: sampling number of the dead-time of the system
 - Returns:
-  - DOBu: $z^{n_d} Q[z]$
+  - DOBu: $z^{-n_d} Q[z]$
   - DOBy: $Q[z] P^{-1}[z]$
 
 **Examples**
 ```python
 >>> DOBu, DOBy = ctrl.dob(5., 0.7, 1., 10., 0., 0.001, 1)
 >>> print(DOBu)
 
@@ -1128,15 +1097,15 @@
 970.3 z^2 - 1931 z + 960.7
 --------------------------
   z^2 - 1.956 z + 0.957
 
 dt = 0.001
 ```
 
-## 3.29. zpetc
+### 3.29. zpetc
 pylib_sakata.ctrl.**zpetc**(*Pz, dt, zerothr=0.99*)
 
 This function is for design of a zero phase error tracking controller ([ZPETC](https://engineering.purdue.edu/ME576/ZPETC_Tomizuka.pdf)).
 
 - Parameters:
   - Pz: instance of TransferFunction class of discrete-time LTI system
   - dt: sampling time of the system
@@ -1166,47 +1135,47 @@
 
 dt = 0.001
 
 >>> Nzpetc
 2
 ```
 
-## 3.30. filt
+### 3.30. filt
 pylib_sakata.ctrl.**filt**(*num, den, dt*)
 
 This function is to create transfer functions as rational expressions in $z^{-1}$ and to order the numerator and denominator terms in ascending powers of $z^{-1}$.
 
 - Parameters:
   - num: polynomial coefficients of the numerator of the discrete-time LTI model
   - den: polynomial coefficients of the denominator of the discrete-time LTI model
   - dt: sampling time of the discrete-time LTI model
 - Returns:
   - out: instance of TransferFunction class of ZPETC
 
-## 3.31. minreal
+### 3.31. minreal
 pylib_sakata.ctrl.**minreal**(*sys*)
 
 This function is to delete the common pole-zeros of the system.
 
 - Parameters:
   - sys: LTI model (StateSpace or TransferFunction or ZpkModel)
 - Returns:
   - out: LTI model whose the common pole-zeros were deleted
 
-## 3.32. makeprmset
+### 3.32. makeprmset
 pylib_sakata.ctrl.**makeprmset**(*path='.'*)
 
 This function is to create Cpp and header files of controller parameter sets
 
 - Parameters:
   - path: path to create Cpp and header files of controller parameter sets
 - Returns:
   - None
   
-## 3.33. defprmset
+### 3.33. defprmset
 pylib_sakata.ctrl.**defprmset**(*tfz, prmSetName, path='.', mode='a'*)
 
 - Parameters:
   - tfz: discrete time TransferFunction model
   - prmSetName: parameter set name of the following struct in Cpp
   - path: path to create Cpp and header files of controller parameter sets
   - mode: mode to open Cpp and header files
@@ -1232,17 +1201,17 @@
 	double	dA[4];
 	double	dB[4];
 	double	dInPre[3];
 	double	dOutPre[3];
 } TF3_INF;						// 3rd order TF information
 ```
 
-# 4. pylib_sakata.fft
+## 4. pylib_sakata.fft
 
-## 4.1. FreqResp
+### 4.1. FreqResp
 
 class pylib_sakata.fft.**FreqResp**(*freq, resp, dt=0*)
 
 - Parameters:
   - freq: 1-D array frequency data [Hz]
   - resp: 1-D array frequency response data [complex data]
   - dt: sampling time (Optional), Default: 0, set the value >= 0. If dt = 0, the system is continuous time system.
@@ -1277,15 +1246,15 @@
 
 - \__**rtruediv**__(*other*)
 	Right divide two FRDs.
 
 - \__**pow**__(*other*)
 	A FRD to the power of x.
 
-## 4.2. fft
+### 4.2. fft
 
 pylib_sakata.fft.**fft**(*data, dt*)
 
 This function is for calculating FFT from 1-D array data.
 
 - Parameters:
   - data: 1-D array time response data
@@ -1302,25 +1271,25 @@
 >>> x = np.sin(2*np.pi*10.0*t) + np.sin(2*np.pi*50.0*t)
 >>> fft.fft(x, dt)
 (array([0.00000000e+00, 1.00010001e-01, 2.00020002e-01, ...,
        9.99799980e+02, 9.99899990e+02, 1.00000000e+03]), array([3.93463040e-17, 2.39600781e-06, 4.79322523e-06, ...,
        7.19286425e-06, 4.79322523e-06, 2.39600781e-06]))
 ```
 
-## 4.3. fft_ave
+### 4.3. fft_ave
 
 pylib_sakata.fft.**fft_ave**(*data, dt, windivnum=4, overlap=0.5*)
 
 This function is for calculating averaged FFT from 1-D array data.
 
 - Parameters:
   - data: 1-D array time response data
   - dt: sampling time of the time response data
   - windivnum: number of windows to divide the time response data
-  - overlap: overlap retio divided time response data (0 <= overlap < 1)
+  - overlap: overlap ratio divided time response data (0 <= overlap < 1)
 - Returns:
   - freq_data: 1-D array frequency data [Hz]
   - fft_data: 1-D array FFT data
 
 **Examples**
 ```python
 import numpy as np
@@ -1329,27 +1298,27 @@
 >>> x = np.sin(2*np.pi*10.0*t) + np.sin(2*np.pi*50.0*t)
 >>> fft.fft_ave(x, dt, 4, 0.5)
 (array([0.00000000e+00, 4.88519785e-01, 9.77039570e-01, ...,
        9.99022960e+02, 9.99511480e+02, 1.00000000e+03]), array([5.33388114e-05, 5.46444944e-05, 5.85999322e-05, ...,
        6.53498409e-05, 5.85999322e-05, 5.46444944e-05]))
 ```
 
-## 4.4. tfestimate
+### 4.4. tfestimate
 
 pylib_sakata.fft.**tfestimate**(*x, y, freq, dt, windivnum=4, overlap=0.5*)
 
 This function is for system identification from input and output time response data.
 
 - Parameters:
   - x: 1-D array time response data of input
   - y: 1-D array time response data of output
   - freq: 1-D array frequency data [Hz]
   - dt: sampling time of the time response data
   - windivnum: number of windows to divide the time response data
-  - overlap: overlap retio divided time response data (0 <= overlap < 1)
+  - overlap: overlap ratio divided time response data (0 <= overlap < 1)
 - Returns:
   - freqresp: instance of FreqResp class
   - coh: 1-D array coherence data
 
 **Examples**
 ```python
 >>> import numpy as np
@@ -1367,15 +1336,15 @@
 >>> fft.tfestimate(u, y, freq, dt)
 (array([-0.11586071-1.49076948e-01j, -0.11590257-1.49078279e-01j,
        -0.11594446-1.49079611e-01j, ..., -0.13155661-1.45847229e-01j,
        -0.14201211-1.03211830e-01j, -0.15745492-1.88460358e-14j]), array([0.77271576, 0.77244166, 0.7721674 , ..., 0.23080322, 0.32843388,
        0.43848208]))
 ```
 
-## 4.5. frdresize
+### 4.5. frdresize
 
 pylib_sakata.fft.**frdresize**(*freqresp, freq*)
 
 This function is for resizing a frequency response data.
 
 - Parameters:
   - freqresp: instance of FreqResp class
@@ -1395,57 +1364,57 @@
 freq = array([   1.            1.00069108    1.00138264 ...  998.61926487  999.30939397
  1000.        ])
 resp = array([-5.10821217e-03-5.65218353e-02j -5.10244172e-03-5.64813436e-02j
  -5.09666728e-03-5.64408239e-02j ... -5.64622394e-09-5.31301950e-05j
  -5.63759203e-09-5.30909366e-05j -5.62895416e-09-5.30516511e-05j])
 ```
 
-## 4.6. frdsim
+### 4.6. frdsim
 
 pylib_sakata.fft.**frdsim**(*freqresp, x, dt*)
 
 This function is for simulation steady time response data when a time-domain data is input to a system written by frequency response data.
-$$
-y(t) = \text{ifft}(\text{FreqResp}(\omega)\times\text{fft}(u(t)))
-$$
+$$y(t) = \text{ifft}(\text{FreqResp}(\omega)\times\text{fft}(u(t)))$$
 
 - Parameters:
   - freqresp: instance of FreqResp class
   - x: 1-D array time response data of input
   - dt: sampling time of the time response data
 - Returns:
+  - t: 1-D array time data [s]
   - y: 1-D array time response data of output
 
 **Examples**
 ```python
 >>> import numpy as np
 >>> freq = np.logspace(np.log10(1.), np.log10(1000.), 100, base=10)
 >>> Sys_tf = ctrl.tf([1., 2.], [3., 4., 5.])
 >>> freqresp = ctrl.sys2frd(Sys_tf, freq)
 >>> dt = 0.001
 >>> t = np.linspace(0.0, 10., int(10./dt))
 >>> x = np.sin(2*np.pi*10.0*t) + np.sin(2*np.pi*50.0*t)
 >>> fft.frdsim(freqresp, x, dt)
-array([-0.00635301, -0.00630568, -0.00612106, ..., -0.00610225,
-       -0.0062943 , -0.00634922])
+(array([0.000e+00, 1.000e-03, 2.000e-03, ..., 9.996e+00, 9.997e+00,
+       9.998e+00]), array([-0.00635301, -0.00630568, -0.00612106, ..., -0.00610225,
+       -0.0062943 , -0.00634922]))
 ```
 
-# 5. pylib_sakta.meas
+## 5. pylib_sakata.meas
 
-## 5.1. MeasData
+### 5.1. MeasData
 
-class pylib_sakata.meas.**MeasData**(*time, list, value, time, dt*)
+class pylib_sakata.meas.**MeasData**(*list, value, time, dt*)
 
 - Parameters:
-  - dataList: array of data list (*str*)
-  - dataValue: array of data value
+  - list: array of data list (*str*)
+  - value: array of data value
   - time: 1-D array time data [s]
   - dt: sampling time of the time response data
 
-## 5.2. getcsvdata
+### 5.2. getcsvdata
 
 pylib_sakata.meas.**getcsvdata**(*filePath*)
 
 This function is for getting measurement data from a csv file.
 
 - Parameters:
   - filePath: csv file path of measurement file
@@ -1453,15 +1422,15 @@
   - instance of MeasData class
 
 **Examples**
 ```python
 measdata = meas.getcsvdata('data\001-inject.csv')
 ```
 
-## 5.3. gettxtdata
+### 5.3. gettxtdata
 
 pylib_sakata.meas.**gettxtdata**(*filePath*)
 
 This function is for getting measurement data from a txt file.
 
 - Parameters:
   - filePath: txt file path of measurement file
@@ -1469,15 +1438,15 @@
   - instance of MeasData class
 
 **Examples**
 ```python
 measdata = meas.gettxtdata('data\001-inject.txt')
 ```
 
-## 5.4. getmatdata
+### 5.4. getmatdata
 
 pylib_sakata.meas.**getmatdata**(*filePath*)
 
 This function is for getting measurement data from a mat file.
 
 - Parameters:
   - filePath: mat file path of measurement file
@@ -1485,52 +1454,52 @@
   - instance of MeasData class
 
 **Examples**
 ```python
 measdata = meas.getmatdata('data\001-inject.mat')
 ```
 
-## 5.5. getdata
+### 5.5. getdata
 
 pylib_sakata.meas.**getdata**(*filePath*)
 
 This function is for getting measurement data from a file.
 
 - Parameters:
   - filePath: file path of measurement file (.csv, .txt, and .mat are supported.)
 - Returns:
   - instance of MeasData class
 
 **Examples**
 ```python
-measdata = meas.getmatdata('data\001-inject.csv')
+measdata = meas.getdata('data\001-inject.csv')
 ```
 ```python
-measdata = meas.getmatdata('data\001-inject.txt')
+measdata = meas.getdata('data\001-inject.txt')
 ```
 ```python
-measdata = meas.getmatdata('data\001-inject.mat')
+measdata = meas.getdata('data\001-inject.mat')
 ```
 
-## 5.6. getdataindex
+### 5.6. getdataindex
 
 pylib_sakata.meas.**getdataindex**(*measdata, dataName*)
 
 - Parameters:
   - measdata: instance of MeasData class
   - dataName: data name
 - Returns:
   - index: index of dataName
 
 **Examples**
 ```python
 index = meas.getdataindex(measdata, 'ServoOut')
 ```
 
-## 5.7. measdata2frd
+### 5.7. measdata2frd
 
 pylib_sakata.meas.**measdata2frd**(*filePath, inputName, outputName, flagName, freq, inputGain=1.0, outputGain=1.0, windivnum=4, overlap=0.5*)
 
 This function is for system identification from input and output time response data of measurement file.
 
 - Parameters:
   - filePath: file path of measurement file (.csv, .txt, and .mat are supported.)
@@ -1538,74 +1507,136 @@
   - outputName: output data name in the measurement file
   - flagName: flag data name in the measurement file
   - freq: 1-D array frequency data [Hz]
   - inputGain: inputdata gain (Optional), Default: 1.0, unit of input can be fixed by this parameter.
   - outputGain: outputdata gain (Optional), Default: 1.0, unit of output can be fixed by this parameter.
   - dt: sampling time of the time response data
   - windivnum: number of windows to divide the time response data
-  - overlap: overlap retio divided time response data (0 <= overlap < 1)
+  - overlap: overlap ratio divided time response data (0 <= overlap < 1)
 - Returns:
   - freqresp: instance of FreqResp class
   - coh: 1-D array coherence data
 
 **Examples**
 ```python
 import numpy as np
 freq = np.logspace(np.log10(1.), np.log10(1000.), 10000, base=10)
 freqresp, coh = measdata2frd('data\001-inject.csv', 'ServoOut', 'PosErrUm', 'FlagNoise', freq, 1., 1.e-6)
 ```
 
-# 6. pylib_sakata.traj
+## 6. pylib_sakata.traj
 
-## 6.1. TrajInf
+### 6.1. TrajInf
 
 class pylib_sakata.traj.**TrajInf**(*time, pos, vel, acc, T, dt*)
 
 - Parameters:
   - time: 1-D array time data [s]
   - pos: 1-D array position trajectory data [m]
   - vel: 1-D array velocity trajectory data [m/s]
   - acc: 1-D array acceleration trajectory data [m/s^2]
   - T: moving time [s]
   - dt: sampling time of the trajectory data
 
-## 6.2. traj4th
+### 6.2. traj3rd
 
-pylib_sakata.traj.**traj4th**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
+pylib_sakata.traj.**traj3rd**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)  
+
+This function is for generation of a 3rd order polynomial trajectory.
+
+- Parameters:
+  - posStart: start position of the trajectory
+  - posStep: step position of the trajectory
+  - velMax: maximum of velocity of the trajectory
+  - accAve: average of accelation (= decelation) of the trajectory
+  - dt: sampling time of the trajectory data.
+  - Tstay: time after the step moving
+- Returns:
+  - out: instance of TrajInf class of the 3rd order polynomial trajectory
+
+**Examples**
+```python
+traj = traj.traj3rd(0, 100, 100, 200, 0.001, 0.5)
+```
+
+### 6.3. traj3rd2
+
+pylib_sakata.traj.**traj3rd2**(*posStart, posStep, velMax, accAve, jerkRatio, dt, Tstay=0*)  
+
+This function is for generation of a 3rd order polynomial trajectory as trapezoidal accelaration trajectory.
+
+- Parameters:
+  - posStart: start position of the trajectory
+  - posStep: step position of the trajectory
+  - velMax: maximum of velocity of the trajectory
+  - accAve: average of accelation (= decelation) of the trajectory
+  - jerkRatio: ratio of jerk time per accelaration time (0 < jerkRatio <= 0.5)
+  - dt: sampling time of the trajectory data.
+  - Tstay: time after the step moving
+- Returns:
+  - out: instance of TrajInf class of the 3rd order polynomial trajectory
+
+**Examples**
+```python
+traj = traj.traj3rd2(0, 100, 100, 200, 0.001, 0.2, 0.5)
+```
+
+### 6.4. traj4th
+
+pylib_sakata.traj.**traj4th**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)  
+pylib_sakata.traj.**traj4th2**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
 
 This function is for generation of a 4th order polynomial trajectory.
 
 - Parameters:
   - posStart: start position of the trajectory
   - posStep: step position of the trajectory
   - velMax: maximum of velocity of the trajectory
   - accAve: average of accelation (= decelation) of the trajectory
   - dt: sampling time of the trajectory data.
+  - Tstay: time after the step moving
 - Returns:
   - out: instance of TrajInf class of the 4th order polynomial trajectory
 
 **Examples**
 ```python
 traj = traj.traj4th(0, 100, 100, 200, 0.001, 0.5)
+```
 
-fig = plot.makefig()
-ax1 = fig.add_subplot(311)
-ax2 = fig.add_subplot(312)
-ax3 = fig.add_subplot(313)
-plot.plot_xy(ax1, traj.time, traj.pos, ylabel='[m]', legend=['Pos'], title='TrajInf')
-plot.plot_xy(ax2, traj.time, traj.vel, ylabel='[m/s]', legend=['Vel'])
-plot.plot_xy(ax3, traj.time, traj.acc, xlabel='Time [s]', ylabel='[m/s^2]', legend=['Acc'])
-plot.savefig('time_traj.png')
+### 6.5. trajSinStep
+
+pylib_sakata.traj.**trajSinStep**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
+pylib_sakata.traj.**trajSinStep2**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
+pylib_sakata.traj.**trajSinStep3**(*posStart, posStep, velMax, accAve, dt, Tstay=0*)
+
+This function is for generation of a trajectory based on sine waves.
+
+- Parameters:
+  - posStart: start position of the trajectory
+  - posStep: step position of the trajectory
+  - velMax: maximum of velocity of the trajectory
+  - accAve: average of accelation (= decelation) of the trajectory
+  - dt: sampling time of the trajectory data.
+  - Tstay: time after the step moving
+- Returns:
+  - out: instance of TrajInf class of the trajectory based on sine waves
+
+**Examples**
+```python
+traj = traj.SinStep(0, 100, 100, 200, 0.001, 0.5)
 ```
 
-<img src="figure\time_traj.png" alt="vscode_disp" style="zoom: 80%;" />
+The comparison of these trajectories under the specification: posStep = 1, velMax = 1, accAve = 2 is shown as follows.
+
+<img src="figure\time_traj.png" alt="vscode_disp" style="zoom: 15%;" />
+<img src="figure\time_fft.png" alt="vscode_disp" style="zoom: 40%;" />
 
-# 7. pylib_sakata.plot
+## 7. pylib_sakata.plot
 
-## 7.1. plot_xy
+### 7.1. plot_xy
 
 pylib_sakata.plot.**plot_xy**(*ax, x, y, styl='-', col='b', width=1.5, alpha=1.0, xrange=None, yrange=None, xlabel=None, ylabel=None, legend=None, loc='best', title=None, xscale='linear', yscale='linear', labelouter=True*)
 
 This function is for drawing a 2-D figure from x and y data. You can select xy scale in linear type, log type and so on.
 
 - Parameters:
   - ax: handle of axis
@@ -1642,15 +1673,15 @@
 ax2 = fig2.add_subplot(312)
 ax3 = fig2.add_subplot(313)
 plot.plot_xy(ax1, fft_axis, chirp_fft, '-', 'm', 1.5, 1.0, freqrange, [0, 1.0], ylabel='Input [N]', legend=['Chirp'], title='Power spectrum density', xscale='log')
 plot.plot_xy(ax2, fft_axis, u_fft, '-', 'b', 1.5, 1.0, freqrange, [0, 0.1], ylabel='Input [N]', legend=['Servo Out'], xscale='log')
 plot.plot_xy(ax3, fft_axis, y_fft*1.0e6, '-', 'b', 1.5, 1.0, freqrange, [0, 20], xlabel='Frequency [Hz]', ylabel='Output [um]', legend=['Position'], xscale='log')
 ```
 
-## 7.2. plot_tf
+### 7.2. plot_tf
 
 pylib_sakata.plot.**plot_tf**(*ax_mag, ax_phase, sys, freq, styl='-', col='b', width=1.5, alpha=1.0, freqrange=None, magrange=None, legend=None, loc='best', title=None, labelouter=True*)
 
 This function is for drawing a Bode diagram from a LTI model.
 
 - Parameters:
   - ax_mag: handle of magnitude axis
@@ -1683,25 +1714,24 @@
 fig2 = plot.makefig()
 ax_mag = fig2.add_subplot(211)
 ax_phase = fig2.add_subplot(212)
 plot.plot_tf(ax_mag, ax_phase, T, freq, '-', 'm', 1.5, 1.0, title='Frequency response of complementary sensitivity function')
 plot.plot_tf(ax_mag, ax_phase, Tn, freq, '--', 'b', 1.5, 1.0, [1, 1000], [-60, 10], legend=['Measurement','Model'])
 ```
 
-## 7.3. plot_tffrd
+### 7.3. plot_tffrd
 
 pylib_sakata.plot.**plot_tffrd**(*ax_mag, ax_phase, freqresp, styl='-', col='b', width=1.5, alpha=1.0, freqrange=None, magrange=None, legend=None, loc='best', title=None, labelouter=True, ax_coh=None, coh=None*)
 
 This function is for drawing a Bode diagram from a frequency response data.
 
 - Parameters:
   - ax_mag: handle of magnitude axis
   - ax_phase: handle of phase axis, if you set as None, phase axis is skipped.
   - freqresp: instance of FreqResp class
-  - freq: 1-D array frequency data [Hz]
   - styl: line style (Optional), Default: '-', Select in '-' (solid), '--' (dashed), '.' (dotted), '-.' (dashdot)
   - col: line color (Optional), Default: 'b' (blue)
   - width: line width (Optional), Default: 1.5
   - alpha: transmittance of line, Default: 1.0, set from 0 to 1.0
   - freqrange: plot range of frequency-axis (Optional), Default: None, set as [freqmin, freqmax]
   - magrange: plot range of magnitude-axis (Optional), Default: None, set as [magmin, magmax]
   - legend: legend of data, Default: None, set a list of strings data
@@ -1734,15 +1764,15 @@
 fig3 = plot.makefig()
 ax_mag = fig2.add_subplot(211)
 ax_phase = fig2.add_subplot(212)
 plot.plot_tffrd(ax_mag, ax_phase, T_frd, '-', 'm', 1.5, 1.0, title='Frequency response of complementary sensitivity function')
 plot.plot_tffrd(ax_mag, ax_phase, Tn_frd, '--', 'b', 1.5, 1.0, [1, 1000], [-60, 10], legend=['Measurement','Model'])
 ```
 
-## 7.4. plot_nyquist
+### 7.4. plot_nyquist
 
 pylib_sakata.plot.**plot_nyquist**(*ax, freqresp, styl='-', col='b', width=1.5, alpha=1.0, xrange=None, yrange=None, legend=None, loc='best', title=None, labelouter=True*)
 
 This function is for drawing a Nyquist diagram from a frequency response data of a open loop system
 
 - Parameters:
   - ax: handle of axis
@@ -1764,15 +1794,15 @@
 ```python
 fig = plot.makefig()
 ax = fig.add_subplot(111)
 plot.plot_nyquist(ax, G_frd, '-', 'm', 1.5, 1.0, title='Nyquist Diagram')
 plot.plot_nyquist(ax, Gn_frd, '--', 'b', 1.5, 1.0, legend=['Measurement','Model'])
 ```
 
-## 7.5. plot_nyquist_assistline
+### 7.5. plot_nyquist_assistline
 
 pylib_sakata.plot.**plot_nyquist_assistline**(*ax*)
 
 This function is for drawing assist line of a Nyquist diagram.
 
 - Parameters:
   - ax: handle of axis
@@ -1780,32 +1810,33 @@
   - None
 
 **Examples**
 ```python
 plot.plot_nyquist_assistline(ax)
 ```
 
-## 7.6. makefig
+### 7.6. makefig
 
-pylib_sakata.plot.**makefig**(dpi=100, popwin=False)
+pylib_sakata.plot.**makefig**(dpi=100, figsize=(6, 4), popwin=False)
 
 This function will make a new figure handle.
 
 - Parameters:
   - dpi: dot per inch of figure (Optional), Default: 100
+  - figsize: set figure size (Optional), Default: (6, 4) which means 600x400 pixels
   - popwin: switch to fix the popup window of the figure (Optional), Default: False
 - Returns:
   - fig: figure handle
 
 **Examples**
 ```python
 fig = plot.makefig()
 ```
 
-## 7.7. savefig
+### 7.7. savefig
 
 pylib_sakata.plot.**savefig**(*figName*)
 
 This function will save a current figure.
 
 - Parameters:
   - figName: figure name for saving a current figure, set strings data
@@ -1813,43 +1844,41 @@
   - None
 
 **Examples**
 ```python
 plot.savefig('freq_P.png')
 ```
 
-## 7.8. showfig
+### 7.8. showfig
 
 pylib_sakata.plot.**showfig**()
 
 This function will call matplotlib.pyplot.show()
 
 **Examples**
 ```python
 showfig()
 ```
 
-# 8. pylib_sakata.init
+## 8. pylib_sakata.init
 
-## 8.1. close_all
+### 8.1. close_all
 
 pylib_sakata.init.**close_all**()
 
 This function is for closing current opened figures.
 
 **Examples**
 ```python
 close_all()
 ```
 
-## 8.2. clear_all
+### 8.2. clear_all
 
 pylib_sakata.init.**clear_all**()
 
 This function is for deleting all defined variables.
 
 **Examples**
 ```python
 clear_all()
 ```
-
-
```

