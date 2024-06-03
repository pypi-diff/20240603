# Comparing `tmp/OptiCommPy-0.7.0.tar.gz` & `tmp/OptiCommPy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OptiCommPy-0.7.0.tar", last modified: Fri Dec  8 16:07:37 2023, max compression
+gzip compressed data, was "OptiCommPy-0.9.0.tar", last modified: Mon Jun  3 14:26:45 2024, max compression
```

## Comparing `OptiCommPy-0.7.0.tar` & `OptiCommPy-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-12-08 16:07:37.862980 OptiCommPy-0.7.0/
--rw-rw-rw-   0        0        0    35823 2022-08-27 14:09:58.000000 OptiCommPy-0.7.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-12-08 16:07:37.859994 OptiCommPy-0.7.0/OptiCommPy.egg-info/
--rw-rw-rw-   0        0        0     4682 2023-12-08 16:07:37.000000 OptiCommPy-0.7.0/OptiCommPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-12-08 16:07:37.000000 OptiCommPy-0.7.0/OptiCommPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-08 16:07:37.000000 OptiCommPy-0.7.0/OptiCommPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      182 2023-12-08 16:07:37.000000 OptiCommPy-0.7.0/OptiCommPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-12-08 16:07:37.000000 OptiCommPy-0.7.0/OptiCommPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4682 2023-12-08 16:07:37.860981 OptiCommPy-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     3637 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-12-08 16:07:37.830981 OptiCommPy-0.7.0/optic/
--rw-rw-rw-   0        0        0       14 2022-08-27 14:09:58.000000 OptiCommPy-0.7.0/optic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-08 16:07:37.843980 OptiCommPy-0.7.0/optic/comm/
--rw-rw-rw-   0        0        0     1644 2023-07-02 19:21:41.000000 OptiCommPy-0.7.0/optic/comm/fec.py
--rw-rw-rw-   0        0        0    21837 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/comm/metrics.py
--rw-rw-rw-   0        0        0     6408 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/comm/modulation.py
--rw-rw-rw-   0        0        0     6164 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/comm/ofdm.py
-drwxrwxrwx   0        0        0        0 2023-12-08 16:07:37.849982 OptiCommPy-0.7.0/optic/dsp/
--rw-rw-rw-   0        0        0     9790 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/dsp/carrierRecovery.py
--rw-rw-rw-   0        0        0     4650 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/dsp/clockRecovery.py
--rw-rw-rw-   0        0        0    18084 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/dsp/core.py
--rw-rw-rw-   0        0        0     1151 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/dsp/coreGPU.py
--rw-rw-rw-   0        0        0    24423 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/dsp/equalization.py
-drwxrwxrwx   0        0        0        0 2023-12-08 16:07:37.857993 OptiCommPy-0.7.0/optic/models/
--rw-rw-rw-   0        0        0    25641 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/models/amplification.py
--rw-rw-rw-   0        0        0    17298 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/models/channels.py
--rw-rw-rw-   0        0        0    18688 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/models/devices.py
--rw-rw-rw-   0        0        0    25911 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/models/modelsGPU.py
--rw-rw-rw-   0        0        0     6299 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/models/tx.py
--rw-rw-rw-   0        0        0     9450 2023-07-02 19:21:41.000000 OptiCommPy-0.7.0/optic/plot.py
--rw-rw-rw-   0        0        0     4094 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/optic/utils.py
--rw-rw-rw-   0        0        0      307 2022-08-27 14:09:58.000000 OptiCommPy-0.7.0/runner
--rw-rw-rw-   0        0        0       42 2023-12-08 16:07:37.862980 OptiCommPy-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     2323 2023-12-08 16:03:18.000000 OptiCommPy-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:26:45.853091 OptiCommPy-0.9.0/
+-rw-rw-rw-   0        0        0    35823 2022-09-22 14:11:31.000000 OptiCommPy-0.9.0/LICENSE
+drwxrwxrwx   0        0        0        0 2024-06-03 14:26:45.798915 OptiCommPy-0.9.0/OptiCommPy.egg-info/
+-rw-rw-rw-   0        0        0     4471 2024-06-03 14:26:45.000000 OptiCommPy-0.9.0/OptiCommPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      626 2024-06-03 14:26:45.000000 OptiCommPy-0.9.0/OptiCommPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 14:26:45.000000 OptiCommPy-0.9.0/OptiCommPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2024-06-03 14:26:45.000000 OptiCommPy-0.9.0/OptiCommPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-03 14:26:45.000000 OptiCommPy-0.9.0/OptiCommPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4471 2024-06-03 14:26:45.853091 OptiCommPy-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3781 2024-05-09 19:03:37.000000 OptiCommPy-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-06-03 14:26:45.801906 OptiCommPy-0.9.0/optic/
+-rw-rw-rw-   0        0        0       14 2022-09-22 14:11:31.000000 OptiCommPy-0.9.0/optic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:26:45.805896 OptiCommPy-0.9.0/optic/comm/
+-rw-rw-rw-   0        0        0    29586 2024-05-09 17:55:52.000000 OptiCommPy-0.9.0/optic/comm/metrics.py
+-rw-rw-rw-   0        0        0    13323 2024-04-25 19:51:19.000000 OptiCommPy-0.9.0/optic/comm/modulation.py
+-rw-rw-rw-   0        0        0     9044 2024-04-25 19:51:19.000000 OptiCommPy-0.9.0/optic/comm/ofdm.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:26:45.819610 OptiCommPy-0.9.0/optic/dsp/
+-rw-rw-rw-   0        0        0    11539 2024-05-09 17:55:52.000000 OptiCommPy-0.9.0/optic/dsp/carrierRecovery.py
+-rw-rw-rw-   0        0        0     6702 2024-04-25 19:51:19.000000 OptiCommPy-0.9.0/optic/dsp/clockRecovery.py
+-rw-rw-rw-   0        0        0    20766 2024-04-25 19:51:19.000000 OptiCommPy-0.9.0/optic/dsp/core.py
+-rw-rw-rw-   0        0        0     1333 2024-04-25 19:51:19.000000 OptiCommPy-0.9.0/optic/dsp/coreGPU.py
+-rw-rw-rw-   0        0        0    28073 2024-04-25 19:51:19.000000 OptiCommPy-0.9.0/optic/dsp/equalization.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:26:45.839421 OptiCommPy-0.9.0/optic/models/
+-rw-rw-rw-   0        0        0    25643 2024-05-09 17:55:52.000000 OptiCommPy-0.9.0/optic/models/amplification.py
+-rw-rw-rw-   0        0        0    19003 2024-04-25 19:51:19.000000 OptiCommPy-0.9.0/optic/models/channels.py
+-rw-rw-rw-   0        0        0    21265 2024-04-25 19:51:19.000000 OptiCommPy-0.9.0/optic/models/devices.py
+-rw-rw-rw-   0        0        0    27784 2024-04-25 19:51:19.000000 OptiCommPy-0.9.0/optic/models/modelsGPU.py
+-rw-rw-rw-   0        0        0     6299 2024-04-22 20:20:43.000000 OptiCommPy-0.9.0/optic/models/tx.py
+-rw-rw-rw-   0        0        0    18980 2024-04-25 19:51:19.000000 OptiCommPy-0.9.0/optic/plot.py
+-rw-rw-rw-   0        0        0     4094 2024-02-01 14:50:36.000000 OptiCommPy-0.9.0/optic/utils.py
+-rw-rw-rw-   0        0        0      307 2022-09-22 14:11:32.000000 OptiCommPy-0.9.0/runner
+-rw-rw-rw-   0        0        0       42 2024-06-03 14:26:45.853091 OptiCommPy-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2344 2024-06-03 14:25:06.000000 OptiCommPy-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:26:45.848928 OptiCommPy-0.9.0/tests/
+-rw-rw-rw-   0        0        0      557 2024-04-25 19:51:19.000000 OptiCommPy-0.9.0/tests/test_dsp.py
+-rw-rw-rw-   0        0        0     3052 2024-04-25 19:51:19.000000 OptiCommPy-0.9.0/tests/test_metrics.py
+-rw-rw-rw-   0        0        0     2243 2024-04-25 19:51:19.000000 OptiCommPy-0.9.0/tests/test_modulation.py
```

### Comparing `OptiCommPy-0.7.0/LICENSE` & `OptiCommPy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OptiCommPy-0.7.0/OptiCommPy.egg-info/SOURCES.txt` & `OptiCommPy-0.9.0/OptiCommPy.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 LICENSE
-README.md
+README.rst
 runner
 setup.py
 OptiCommPy.egg-info/PKG-INFO
 OptiCommPy.egg-info/SOURCES.txt
 OptiCommPy.egg-info/dependency_links.txt
 OptiCommPy.egg-info/requires.txt
 OptiCommPy.egg-info/top_level.txt
 optic/__init__.py
 optic/plot.py
 optic/utils.py
-optic/comm/fec.py
 optic/comm/metrics.py
 optic/comm/modulation.py
 optic/comm/ofdm.py
 optic/dsp/carrierRecovery.py
 optic/dsp/clockRecovery.py
 optic/dsp/core.py
 optic/dsp/coreGPU.py
 optic/dsp/equalization.py
 optic/models/amplification.py
 optic/models/channels.py
 optic/models/devices.py
 optic/models/modelsGPU.py
-optic/models/tx.py
+optic/models/tx.py
+tests/test_dsp.py
+tests/test_metrics.py
+tests/test_modulation.py
```

### Comparing `OptiCommPy-0.7.0/optic/comm/metrics.py` & `OptiCommPy-0.9.0/optic/comm/metrics.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,47 +2,51 @@
 ================================================================================
 Metrics for signal and performance characterization (:mod:`optic.comm.metrics`)
 ================================================================================
 
 .. autosummary::
    :toctree: generated/
 
+   bert                     -- Calculate BER and Q-factor for optical communication using On-Off Keying (OOK).
    fastBERcalc              -- Monte Carlo BER/SER/SNR calculation
    calcLLR                  -- LLR calculation (circular AGWN channel)
    monteCarloGMI            -- Monte Carlo based generalized mutual information (GMI) estimation
-   monteCarloMI            --  Monte Carlo based mutual information (MI) estimation
+   monteCarloMI             -- Monte Carlo based mutual information (MI) estimation
    Qfunc                    -- Calculate function Q(x)
    calcEVM                  -- Calculate error vector magnitude (EVM) metrics
    theoryBER                -- Theoretical (approx.) bit error probability for PAM/QAM/PSK in AWGN channel
+   theoryMI                 -- Calculate mutual information for the DCMC AWGN channel
    calcLinOSNR              -- Calculate the OSNR evolution in a multi-span fiber transmission system
 """
 
 
 """Metrics for signal and performance characterization."""
 import logging as logg
 
 import numpy as np
 from numba import njit, prange
 from scipy.special import erf
+from scipy.integrate import dblquad
 import scipy.constants as const
 
+from optic.utils import dB2lin
 from optic.dsp.core import pnorm, signal_power
-from optic.comm.modulation import GrayMapping, demodulateGray, minEuclid
+from optic.comm.modulation import grayMapping, demodulateGray, minEuclid
 
 
 def bert(Irx, bitsTx=None, seed=123):
     """
     Calculate Bit Error Rate (BER) and Q-factor for optical communication using On-Off Keying (OOK).
 
     Parameters
     ----------
-    Irx : numpy.ndarray
+    Irx : numpy.np.array
         Received signal intensity values.
 
-    bitsTx : numpy.ndarray, optional
+    bitsTx : numpy.np.array, optional
         Transmitted bit sequence. If not provided, a random bit sequence is generated.
 
     seed : int, optional
         Random seed for bit sequence generation when bitsTx is not provided.
 
     Returns
     -------
@@ -65,54 +69,48 @@
     - `std0`: The standard deviation of the signal when the transmitted bit is 0.
 
     The optimal decision threshold `Id` and the Q-factor are calculated based on the signal statistics.
 
     The function then applies the optimal decision rule to estimate the received bit sequence `bitsRx`. The Bit Error Rate (BER) is calculated
     by comparing `bitsRx` to `bitsTx`.
 
-    Example
-    -------
-    >>> Irx = np.array([0.1, 0.8, 0.2, 0.7, 0.3])
-    >>> bitsTx = np.array([0, 1, 0, 1, 0])
-    >>> BER, Q = ook_BERT(Irx, bitsTx)
-    >>> print(f"BER: {BER}, Q-factor: {Q}")
-
     References
     ----------
-    Agrawal, Govind P. Fiber-optic communication systems. John Wiley & Sons, 2012.
+    [1] Agrawal, Govind P. Fiber-optic communication systems. John Wiley & Sons, 2012.
 
     """
     if bitsTx is None:
-        np.random.seed(seed=seed) # fixing the seed 
+        np.random.seed(seed=seed)  # fixing the seed
 
         # generate reference pseudo-random bit sequence
         bitsTx = np.random.randint(2, size=Irx.size)
 
     # get received signal statistics
-    I1 = np.mean(Irx[bitsTx==1]) # average value of I1
-    I0 = np.mean(Irx[bitsTx==0]) # average value of I0
+    I1 = np.mean(Irx[bitsTx == 1])  # average value of I1
+    I0 = np.mean(Irx[bitsTx == 0])  # average value of I0
 
-    std1 = np.std(Irx[bitsTx==1]) # standard deviation std1 of I1
-    std0 = np.std(Irx[bitsTx==0]) # standard deviation std0 of I0
+    std1 = np.std(Irx[bitsTx == 1])  # standard deviation std1 of I1
+    std0 = np.std(Irx[bitsTx == 0])  # standard deviation std0 of I0
 
-    Id = (std1*I0 + std0*I1)/(std1 + std0) # optimal decision threshold
-    Q = (I1-I0)/(std1 + std0) # Qfactor 
+    Id = (std1 * I0 + std0 * I1) / (std1 + std0)  # optimal decision threshold
+    Q = (I1 - I0) / (std1 + std0)  # Qfactor
 
     # apply the optimal decision rule
     bitsRx = np.empty(bitsTx.size)
-    bitsRx[Irx> Id] = 1
-    bitsRx[Irx<= Id] = 0
+    bitsRx[Irx > Id] = 1
+    bitsRx[Irx <= Id] = 0
 
     # calculate the BER
     err = np.logical_xor(bitsRx, bitsTx)
 
     BER = np.mean(err)
 
     return BER, Q
 
+
 def fastBERcalc(rx, tx, M, constType):
     """
     Monte Carlo BER/SER/SNR calculation.
 
     Parameters
     ----------
     rx : np.array
@@ -129,20 +127,24 @@
     BER : np.array
         Bit-error-rate.
     SER : np.array
         Symbol-error-rate.
     SNR : np.array
         Estimated SNR from the received constellation.
 
+    References
+    ----------
+    [1] Proakis, J. G., & Salehi, M. Digital Communications (5th Edition). McGraw-Hill Education, 2008.
+
     """
     if M != 2 and constType == "ook":
         logg.warn("OOK has only 2 symbols, but M != 2. Changing M to 2.")
         M = 2
     # constellation parameters
-    constSymb = GrayMapping(M, constType)
+    constSymb = grayMapping(M, constType)
     Es = np.mean(np.abs(constSymb) ** 2)
 
     # We want all the signal sequences to be disposed in columns:
     try:
         if rx.shape[1] > rx.shape[0]:
             rx = rx.T
     except IndexError:
@@ -200,14 +202,18 @@
         Bit-to-symbol mapping.
 
     Returns
     -------
     LLRs : np.array
         sequence of calculated LLRs.
 
+    References
+    ----------
+    [1] A. Alvarado, T. Fehenberger, B. Chen, e F. M. J. Willems, “Achievable Information Rates for Fiber Optics: Applications and Computations”, Journal of Lightwave Technology, vol. 36, nº 2, p. 424–439, jan. 2018, doi: 10.1109/JLT.2017.2786351.
+
     """
     M = len(constSymb)
     b = int(np.log2(M))
 
     LLRs = np.zeros(len(rxSymb) * b)
 
     for i in prange(len(rxSymb)):
@@ -240,20 +246,24 @@
 
     Returns
     -------
     GMI : np.array
         Generalized mutual information values.
     NGMI : np.array
         Normalized mutual information.
+    
+    References
+    ----------
+    [1] A. Alvarado, T. Fehenberger, B. Chen, e F. M. J. Willems, “Achievable Information Rates for Fiber Optics: Applications and Computations”, Journal of Lightwave Technology, vol. 36, nº 2, p. 424–439, jan. 2018, doi: 10.1109/JLT.2017.2786351.
 
     """
     if px is None:
         px = []
     # constellation parameters
-    constSymb = GrayMapping(M, constType)
+    constSymb = grayMapping(M, constType)
 
     # get bit mapping
     b = int(np.log2(M))
     bitMap = demodulateGray(constSymb, M, constType)
     bitMap = bitMap.reshape(-1, b)
 
     # We want all the signal sequences to be disposed in columns:
@@ -335,21 +345,25 @@
         p.m.f. of the constellation symbols. The default is [].
 
     Returns
     -------
     MI : np.array
         Estimated MI values.
 
+    References
+    ----------
+    [1] A. Alvarado, T. Fehenberger, B. Chen, e F. M. J. Willems, “Achievable Information Rates for Fiber Optics: Applications and Computations”, Journal of Lightwave Technology, vol. 36, nº 2, p. 424–439, jan. 2018, doi: 10.1109/JLT.2017.2786351.
+
     """
     if px is None:
         px = []
     if len(px) == 0:  # if px is not defined
         px = 1 / M * np.ones(M)  # assume uniform distribution
     # constellation parameters
-    constSymb = GrayMapping(M, constType)
+    constSymb = grayMapping(M, constType)
     Es = np.sum(np.abs(constSymb) ** 2 * px)
     constSymb = constSymb / np.sqrt(Es)
 
     # We want all the signal sequences to be disposed in columns:
     try:
         if rx.shape[1] > rx.shape[0]:
             rx = rx.T
@@ -372,15 +386,15 @@
         rx[:, k] = pnorm(rx[:, k])
         tx[:, k] = pnorm(tx[:, k])
     # Estimate noise variance from the data
     noiseVar = np.var(rx - tx, axis=0)
 
     for k in range(nModes):
         σ2 = noiseVar[k]
-        MI[k] = calcMI(rx[:, k], tx[:, k], σ2, constSymb, px)
+        MI[k] = calcMI(rx[:, k], tx[:, k], σ2, constSymb, px)[0]
     return MI
 
 
 @njit
 def calcMI(rx, tx, σ2, constSymb, pX):
     """
     Mutual information (MI) calculation (circular AGWN channel).
@@ -399,14 +413,18 @@
         prob. mass function (p.m.f.) of the constellation symbols.
 
     Returns
     -------
     scalar
         Estimated mutual information.
 
+    References
+    ----------
+    [1] A. Alvarado, T. Fehenberger, B. Chen, e F. M. J. Willems, “Achievable Information Rates for Fiber Optics: Applications and Computations”, Journal of Lightwave Technology, vol. 36, nº 2, p. 424–439, jan. 2018, doi: 10.1109/JLT.2017.2786351.
+
     """
     N = len(rx)
     H_XgY = np.zeros(1, dtype=np.float64)
     H_X = np.sum(-pX * np.log2(pX))
 
     for k in range(N):
         indSymb = np.argmin(np.abs(tx[k] - constSymb))
@@ -439,14 +457,18 @@
     x : scalar
         function input.
 
     Returns
     -------
     scalar
         value of Q(x).
+    
+    References
+    ----------
+    [1] Proakis, J. G., & Salehi, M. Digital Communications (5th Edition). McGraw-Hill Education, 2008.
 
     """
     return 0.5 - 0.5 * erf(x / np.sqrt(2))
 
 
 def calcEVM(symb, M, constType, symbTx=None):
     """
@@ -464,14 +486,20 @@
         Sequence of transmitted symbols (noiseless). The default is [].
 
     Returns
     -------
     EVM : np.array
         Error vector magnitude (EVM) per signal dimension.
 
+    References
+    ----------
+    [1] R. A. Shafik, et al, “On the error vector magnitude as a performance metric and comparative analysis”, em 2006 International Conference on Emerging Technologies, 2006, p. 27–31. doi: 10.1109/ICET.2006.335992.
+
+    [2] H. A. Mahmoud e H. Arslan, “Error vector magnitude to SNR conversion for nondata-aided receivers”, IEEE Transactions on Wireless Communications, vol. 8, nº 5, p. 2694–2704, 2009, doi: 10.1109/TWC.2009.080862.
+
     """
     if symbTx is None:
         symbTx = []
     symb = pnorm(symb)
 
     # We want all the signal sequences to be disposed in columns:
     try:
@@ -483,15 +511,15 @@
         try:
             if symbTx.shape[1] > symbTx.shape[0]:
                 symbTx = symbTx.T
         except IndexError:
             symbTx = symbTx.reshape(len(symbTx), 1)
         symbTx = pnorm(symbTx)
     # constellation parameters
-    constSymb = GrayMapping(M, constType)
+    constSymb = grayMapping(M, constType)
     constSymb = pnorm(constSymb)
 
     EVM = np.zeros(symb.shape[1])
 
     for ii in range(symb.shape[1]):
         if not len(symbTx):
             decided = np.zeros(symb.shape[0], dtype="complex")
@@ -524,14 +552,24 @@
         Modulation type: 'pam', 'qam' or 'psk'
 
     Returns
     -------
     Pb : scalar
         Theoretical probability of bit error.
 
+    Notes
+    -----
+    The values of error probability obtained with this function are good approximations for moderate to high SNR regime (see [1]).
+    All cases assume Gray mapped constellations. For low SNR values and high constellation cardinalities (Pb>1e-1), the results 
+    should underestimate the real error probability.
+
+    References
+    ----------
+    [1] Proakis, J. G., & Salehi, M. Digital Communications (5th Edition). McGraw-Hill Education, 2008.
+   
     """
     EbN0lin = 10 ** (EbN0 / 10)
     k = np.log2(M)
 
     if constType == "qam":
         L = np.sqrt(M)
         Pb = (
@@ -540,21 +578,181 @@
             / np.log2(L)
             * Qfunc(np.sqrt(3 * np.log2(L) / (L**2 - 1) * (2 * EbN0lin)))
         )
     elif constType == "psk":
         Ps = 2 * Qfunc(np.sqrt(2 * k * EbN0lin) * np.sin(np.pi / M))
         Pb = Ps / k
     elif constType == "pam":
-        Ps = (2 * (M - 1) / M) * Qfunc(
-            np.sqrt(6 * np.log2(M) / (M**2 - 1) * EbN0lin)
-        )
+        Ps = (2 * (M - 1) / M) * Qfunc(np.sqrt(6 * np.log2(M) / (M**2 - 1) * EbN0lin))
         Pb = Ps / k
     return Pb
 
 
+@njit
+def condEntropy(yI, yQ, const, pX, ind, σ):
+    """
+    Calculate conditional entropy H(X|Y=y)
+
+    Parameters
+    ----------
+    yI, yQ : float
+        Real and imaginary parts of the received signal Y.
+    const : array_like
+        Constellation of complex-valued transmitted symbols.
+    pX : array_like
+        Probability of each transmitted symbol.
+    ind : int
+        Index of the transmitted symbol.
+    σ : float
+        Standard deviation of the Gaussian noise.
+
+    Returns
+    -------
+    float
+        conditional entropy H(X|Y=y).
+
+    References
+    ----------
+    [1] A. Alvarado, T. Fehenberger, B. Chen, e F. M. J. Willems, “Achievable Information Rates for Fiber Optics: Applications and Computations”, Journal of Lightwave Technology, vol. 36, nº 2, p. 424–439, jan. 2018, doi: 10.1109/JLT.2017.2786351.
+    """
+    π = np.pi
+    prob = 0
+    M = len(const)
+
+    for ii in prange(len(const)):
+        xI = const[ii].real
+        xQ = const[ii].imag
+        prob += (
+            1
+            / (2 * π * σ**2)
+            * np.exp(-((yI - xI) ** 2 + (yQ - xQ) ** 2) / (2 * σ**2))
+            * pX[ii]
+        )
+
+    log2pY = np.log2(max([prob, 1e-50]))
+
+    xI = const[ind].real
+    xQ = const[ind].imag
+
+    expTerm = (
+        1 / (2 * π * σ**2) * np.exp(-((yI - xI) ** 2 + (yQ - xQ) ** 2) / (2 * σ**2))
+    )
+
+    int1 = expTerm * np.log2(max([expTerm, 1e-50]))  # p(Y|X)*log2(p(Y|X))
+
+    int2 = expTerm * np.log2(pX[ind])  # p(Y|X)*log2(p(X))
+
+    int3 = expTerm * log2pY  # p(Y|X)*log2(p(Y))
+
+    return (
+        -(int1 + int2 - int3) * pX[ind]
+    )  # integral of p(Y,X)*log2(p(Y|X)p(X)/p(Y)) = H(X|Y)
+
+
+@njit
+def minR(R, x):
+    """
+    Find the index of the minimum absolute difference between an array R and a value x.
+
+    Parameters
+    ----------
+    R : array_like
+        Array of values.
+    x : float
+        Value for comparison.
+
+    Returns
+    -------
+    int
+        Index of the minimum absolute difference.
+    """
+    return np.argmin(np.abs(R - np.abs(x)))
+
+
+def theoryMI(M, constType, SNR, pX=None, symetry=True, lim=np.inf, tol=1e-3):
+    """
+    Calculate mutual information for discrete input continuous output the memoryless AWGN channel (DCMC).
+
+    Parameters
+    ----------
+    M : int
+        Number of symbols in the constellation.
+    constType : str
+        Type of constellation ('qam', 'psk').
+    SNR : float
+        Signal-to-noise ratio in dB.
+    pX : array_like, optional
+        Probability of each transmitted symbol (default is None).
+    symetry : bool, optional
+        Flag to exploit rotational symmetry of the constellation (default is True).
+    lim : int, optional
+        Limit for numerical integration (default is np.inf).
+    tol : float, optional
+        Tolerance for numerical integration error (default is 1e-3).
+
+    Returns
+    -------
+    float
+        Mutual information for the given parameters.
+    
+    References
+    ----------
+    [1] A. Alvarado, T. Fehenberger, B. Chen, e F. M. J. Willems, “Achievable Information Rates for Fiber Optics: Applications and Computations”, Journal of Lightwave Technology, vol. 36, nº 2, p. 424–439, jan. 2018, doi: 10.1109/JLT.2017.2786351.
+    """
+    constSymb = grayMapping(M, constType)  # get constellation
+    Es = signal_power(constSymb)  # calculate average symbol energy
+    constSymb = constSymb / np.sqrt(Es)  # normalize average symbol energy
+
+    σ = np.sqrt((1 / 2) * 1 / dB2lin(SNR))  # noise variance per dimension
+
+    if pX is None:
+        pX = 1 / M * np.ones(M)
+
+    MI = -np.sum(pX * np.log2(pX))
+
+    if symetry:
+        # Exploit rotational symmetry of the constellation to speed up calculations
+        constR = np.abs(constSymb)
+        R = np.unique(constR)
+        MI_R = np.zeros(R.shape)
+        symbCount = np.zeros(R.shape)
+
+        for ind in range(len(R)):
+            symbCount[ind] = np.sum(constR == R[ind])
+
+        for ind in range(len(constSymb)):
+            indR = minR(R, constSymb[ind])
+
+            if MI_R[indR] == 0:
+                MI_R[indR] = dblquad(
+                    condEntropy,
+                    -lim,
+                    lim,
+                    -lim,
+                    lim,
+                    args=(constSymb, pX, ind, σ),
+                    epsabs=tol,
+                )[0]
+        MI -= np.sum(MI_R * symbCount)
+
+    else:
+        for ind in range(len(constSymb)):
+            MI -= dblquad(
+                condEntropy,
+                -lim,
+                lim,
+                -lim,
+                lim,
+                args=(constSymb, pX, ind, σ),
+                epsabs=tol,
+            )[0]
+
+    return MI
+
+
 def GN_Model_NyquistWDM(Rs, Nch, Δf, α, γ, Ls, Ns, Ptx_dBm, D, Bref, Fc):
     # Reference: [1] P. Poggiolini, "The GN Model of Non-Linear Propagation in
     # Uncompensated Coherent Optical Systems," in Journal of Lightwave
     # Technology, vol. 30, no. 24, pp. 3857-3879, Dec.15, 2012,
     # doi: 10.1109/JLT.2012.2217729.
 
     # Channel parameters:
@@ -572,20 +770,15 @@
     var_NLI = (
         (8 / 27)
         * (γ**2)
         * Leff**2
         * (Ptx / Rs) ** 3
         * (
             np.arcsinh(
-                (np.pi**2)
-                / 2
-                * np.abs(β2)
-                * Leffa
-                * Nch ** (2 * Rs / Δf)
-                * Rs**2
+                (np.pi**2) / 2 * np.abs(β2) * Leffa * Nch ** (2 * Rs / Δf) * Rs**2
             )
         )
         / (np.pi * np.abs(β2) * Leffa)
         * Bref
     )
 
     epsilon = (3 / 10) * np.log(
@@ -607,15 +800,14 @@
     # multiplication by two here? without the multiplication by two, var_NLI
     # does not match the split-step simulation.
 
     return var_NLI
 
 
 def ASE_NyquistWDM(α, Ls, Ns, NF, Bref, Fc):
-
     # ASE noise power calculation:
     G = α * Ls  # amplifier gain (dB)
 
     NF_lin = 10 ** (NF / 10)  # amplifier noise figure (linear)
     G_lin = 10 ** (G / 10)  # amplifier gain (linear)
     nsp = (G_lin * NF_lin - 1) / (2 * (G_lin - 1))
 
@@ -642,17 +834,15 @@
     Ns = Ltotal // Ls
 
     OSNR = np.zeros(len(Ptx))
     P_nli = np.zeros(len(Ptx))
     P_ase = np.zeros(len(Ptx))
 
     for k, Ptx_dBm in enumerate(Ptx):
-        P_nli[k] = GN_Model_NyquistWDM(
-            Rs, Nch, Δf, α, γ, Ls, Ns, Ptx_dBm, D, Bref, Fc
-        )
+        P_nli[k] = GN_Model_NyquistWDM(Rs, Nch, Δf, α, γ, Ls, Ns, Ptx_dBm, D, Bref, Fc)
         P_ase[k] = ASE_NyquistWDM(α, Ls, Ns, NF, Bref, Fc)
         OSNR[k] = 10 ** (Ptx_dBm / 10) * 1e-3 / (P_nli[k] + P_ase[k])
     return OSNR, P_nli, P_ase
 
 
 def calcLinOSNR(Ns, Pin, α, Ls, OSNRin, NF=4.5, Fc=193.1e12, Bref=12.5e9):
     """
@@ -678,14 +868,22 @@
         Reference bandwidth for OSNR measurement. The default is 12.5e9.
 
     Returns
     -------
     OSNR : np.array
         OSNR values in dB at the output of each fiber span.
 
+    References
+    ----------
+    [1] J. G. Proakis; M. Salehi, Communication Systems Engineering, 2nd Edition. Pearson, 2002.
+
+    [2] R. -J. Essiambre, et al, "Capacity Limits of Optical Fiber Networks,"  Journal of Lightwave Technology, vol. 28, no. 4, p. 662-701, 2010, doi: 10.1109/JLT.2009.2039464.
+
+    [3] R. Schober, P. Bayvel, e F. D. Pasquale, “Analytical model for the calculation of the optical signal-to-noise ratio (SNR) of WDM EDFA chains”, Optical and Quantum Electronics, vol. 31, no 3, p. 237–241. 1999, doi: 10.1023/A:1006948826091.
+
     """
     G = α * Ls
     NF_lin = 10 ** (NF / 10)  # amplifier noise figure (linear)
     G_lin = 10 ** (G / 10)  # amplifier gain (linear)
     nsp = (G_lin * NF_lin - 1) / (2 * (G_lin - 1))
 
     # ASE noise power calculation:
```

### Comparing `OptiCommPy-0.7.0/optic/dsp/carrierRecovery.py` & `OptiCommPy-0.9.0/optic/comm/ofdm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,335 +1,268 @@
 """
-==========================================================================================
-DSP algorithms for carrier phase and frequency recovery (:mod:`optic.dsp.carrierRecovery`)
-==========================================================================================
+==================================================
+OFDM utilities (:mod:`optic.comm.ofdm`)
+==================================================
 
 .. autosummary::
    :toctree: generated/
-   :nosignatures:
 
-   bps            -- Blind phase search (BPS) carrier phase recovery algorithm
-   ddpll          -- Decision-directed phase-locked loop (DD-PLL) carrier phase recovery algorithm
-   viterbi        -- Viterbi & Viterbi carrier phase recovery algorithm
-   fourthPowerFOE -- Frequency offset (FO) estimation and compensation with the 4th-power method
-   cpr            -- General function to call and configure any of the CPR algorithms in this module   
+   hermit                   -- Hermitian simmetry block
+   zeroPad                  -- Pad an input array with zeros on both sides
+   calcSymbolRate           -- Calculate the symbol rate of a given OFDM configuration
+   modulateOFDM             -- OFDM symbols modulator
+   demodulateOFDM           -- OFDM symbols demodulator   
 """
-
-import matplotlib.pyplot as plt
 import numpy as np
-from numba import njit
-from numpy.fft import fft, fftfreq, fftshift
-
-from optic.dsp.core import pnorm, movingAverage
-from optic.comm.modulation import GrayMapping
+from numpy.fft  import fft, ifft, fftshift
+from scipy.interpolate import interp1d
 
-
-def cpr(Ei, param=None, symbTx=None):
+def hermit(V):
     """
-    Carrier phase recovery function (CPR)
+    Hermitian simmetry block.
 
     Parameters
     ----------
-    Ei : complex-valued ndarray
-        received constellation symbols.
-    param : core.param object, optional
-        configuration parameters. The default is [].
-
-        - param.alg: CPR algorithm to be used ['bps', 'ddpll', or 'viterbi']
-
-        BPS params:
-
-        - param.M: constellation order. The default is 4.
-
-        - param.N: length of BPS the moving average window. The default is 35.
-
-        - param.B: number of BPS test phases. The default is 64.
-
-        DDPLL params:
-
-        - param.tau1: DDPLL loop filter param. 1. The default is 1/2*pi*10e6.
-
-        - param.tau2: DDPLL loop filter param. 2. The default is 1/2*pi*10e6.
-
-        - param.Kv: DDPLL loop filter gain. The default is 0.1.
-
-        - param.Ts: symbol period. The default is 1/32e9.
-
-        - param.pilotInd: indexes of pilot-symbol locations.
-
-        Viterbi params:
-
-        - param.N: length of the moving average window. The default is 35.
-
-    symbTx :complex-valued ndarray, optional
-        Transmitted symbol sequence. The default is [].
-
-    Raises
-    ------
-    ValueError
-        Error is generated if the CPR algorithm is not correctly
-        passed.
-
+    V : complex-valued np.array
+        input array
+        
     Returns
     -------
-    Eo : complex-valued ndarray
-        Phase-compensated signal.
-    θ : real-valued ndarray
-        Time-varying estimated phase-shifts.
-
+    Vh : complex-valued np.array
+        vector with hermitian simmetry
     """
-    if symbTx is None:
-        symbTx = np.zeros(Ei.shape)
-    if param is None:
-        param = []
-
-    # check input parameters
-    alg = getattr(param, "alg", "bps")
-    M = getattr(param, "M", 4)
-    constType = getattr(param, "constType", "qam")
-    B = getattr(param, "B", 64)
-    N = getattr(param, "N", 35)
-    Kv = getattr(param, "Kv", 0.1)
-    tau1 = getattr(param, "tau1", 1 / (2 * np.pi * 10e6))
-    tau2 = getattr(param, "tau2", 1 / (2 * np.pi * 10e6))
-    Ts = getattr(param, "Ts", 1 / 32e9)
-    pilotInd = getattr(param, "pilotInd", np.array([len(Ei) + 1]))
-    returnPhases = getattr(param, "returnPhases", False)
-
-    try:
-        Ei.shape[1]
-    except IndexError:
-        Ei = Ei.reshape(len(Ei), 1)
-
-    # constellation parameters
-    constSymb = GrayMapping(M, constType)
-    constSymb = pnorm(constSymb)
-
-    # 4th power frequency offset estimation/compensation
-    Ei, _ = fourthPowerFOE(Ei, 1 / Ts)
-    Ei = pnorm(Ei)
-
-    if alg == "ddpll":
-        θ = ddpll(Ei, Ts, Kv, tau1, tau2, constSymb, symbTx, pilotInd)
-    elif alg == "bps":
-        θ = bps(Ei, N // 2, constSymb, B)
-    elif alg == "viterbi":
-        θ = viterbi(Ei, N)
-    else:
-        raise ValueError("CPR algorithm incorrectly specified.")
-    θ = np.unwrap(4 * θ, axis=0) / 4
-
-    Eo = pnorm(Ei * np.exp(1j * θ))
-
-    if Eo.shape[1] == 1:
-        Eo = Eo[:]
-        θ = θ[:]
-
-    if returnPhases:
-        return Eo, θ
-    else:
-        return Eo
-
+    
+    Vh = np.zeros(2*len(V) + 2, complex)
+    
+    Vh[1:len(V)+1] = V 
+    
+    for j in range(len(V)):
+        Vh[len(Vh) - j - 1] = np.conjugate(V[j])
+    
+    return Vh
 
-@njit
-def bps(Ei, N, constSymb, B):
+def zeroPad(x, L):
     """
-    Blind phase search (BPS) algorithm
+    Pad an input array with zeros on both sides.
 
     Parameters
     ----------
-    Ei : complex-valued ndarray
-        Received constellation symbols.
-    N : int
-        Half of the 2*N+1 average window.
-    constSymb : complex-valued ndarray
-        Complex-valued constellation.
-    B : int
-        number of test phases.
+    x : array_like
+        Input array to be padded.
+    L : int
+        Number of zeros to pad on each side of the array.
 
     Returns
     -------
-    θ : real-valued ndarray
-        Time-varying estimated phase-shifts.
+    padded_array : np.array
+        Padded array with zeros added at the beginning and end.
 
-    """
-    nModes = Ei.shape[1]
-
-    ϕ_test = np.arange(0, B) * (np.pi / 2) / B  # test phases
+    Notes
+    -----
+    This function pads the input array `x` with `L` zeros on both sides, effectively increasing
+    its length by `2*L`.
 
-    θ = np.zeros(Ei.shape, dtype="float")
+    """
+    return np.pad(x, (L, L), 'constant', constant_values=0)
 
-    zeroPad = np.zeros((N, nModes), dtype="complex")
-    x = np.concatenate(
-        (zeroPad, Ei, zeroPad)
-    )  # pad start and end of the signal with zeros
 
-    L = x.shape[0]
+def calcSymbolRate(M, Rb, Nfft, Np, G, hermitSym):
+    """    
+    Calculate the symbol rate of a given OFDM configuration.
 
-    for n in range(nModes):
-        dist = np.zeros((B, constSymb.shape[0]), dtype="float")
-        dmin = np.zeros((B, 2 * N + 1), dtype="float")
+    Parameters
+    ----------
+    M         : scalar
+                constellation order
+    Rb        : scalar
+                bit rate
+    Nfft      : scalar
+                size of FFT
+    Np        : scalar
+                number of pilot subcarriers
+    G         : scalar
+                cyclic prefix length
+    hermitSym : boolean
+                True: Real OFDM symbols / False: Complex OFDM symbols
 
-        for k in range(L):
-            for indPhase, ϕ in enumerate(ϕ_test):
-                dist[indPhase, :] = np.abs(x[k, n] * np.exp(1j * ϕ) - constSymb) ** 2
-                dmin[indPhase, -1] = np.min(dist[indPhase, :])
-            if k >= 2 * N:
-                sumDmin = np.sum(dmin, axis=1)
-                indRot = np.argmin(sumDmin)
-                θ[k - 2 * N, n] = ϕ_test[indRot]
-            dmin = np.roll(dmin, -1)
-    return θ
+    Returns
+    -------
+    Rs        : scalar
+                OFDM symbol rate
+    """    
+    nDataSymbols = (Nfft//2 - 1 - Np) if hermitSym else (Nfft - Np)
+    return Rb / (nDataSymbols/(Nfft + G) * np.log2(M))
 
 
-@njit
-def ddpll(Ei, Ts, Kv, tau1, tau2, constSymb, symbTx, pilotInd):
+def modulateOFDM(symb, param):
     """
-    Decision-directed Phase-locked Loop (DDPLL) algorithm
+    Modulate OFDM signal.
 
     Parameters
     ----------
-    Ei : complex-valued ndarray
-        Received constellation symbols.
-    Ts : float scalar
-        Symbol period.
-    Kv : float scalar
-        Loop filter gain.
-    tau1 : float scalar
-        Loop filter parameter 1.
-    tau2 : float scalar
-        Loop filter parameter 2.
-    constSymb : complex-valued ndarray
-        Complex-valued ideal constellation symbols.
-    symbTx : complex-valued ndarray
-        Transmitted symbol sequence.
-    pilotInd : int ndarray
-        Indexes of pilot-symbol locations.
+    symb : np.np.array
+        Complex-valued array of modulation symbols representing the symbols sequence to be transmitted.
+    param : optic.utils.parameters object
+        An object containing the parameters for OFDM modulation.
+        - Nfft : scalar, optional. Size of the FFT. Default is 512.
+
+        - G : scalar, optional. Cyclic prefix length. Default is 4.
+
+        - hermitSymmetry : bool, optional. If True, indicates real OFDM symbols; if False, indicates complex OFDM symbols. Default is False.
+
+        - pilot : complex-valued scalar, optional. Pilot symbol. Default is 1 + 1j.
+
+        - pilotCarriers : np.array, optional. Indexes of pilot subcarriers. Default is an empty array.
+        - SpS : int, optional. Oversampling factor. Default is 2.
 
     Returns
     -------
-    θ : real-valued ndarray
-        Time-varying estimated phase-shifts.
+    np.array
+        Complex-valued array representing the OFDM symbols sequence transmitted.  
 
     References
     ----------
-    [1] H. Meyer, Digital Communication Receivers: Synchronization, Channel
-    estimation, and Signal Processing, Wiley 1998. Section 5.8 and 5.9.
-
+    [1] Proakis, J. G., & Salehi, M. Digital Communications (5th Edition). McGraw-Hill Education, 2008.
     """
-    nSymbols, nModes = Ei.shape
-
-    θ = np.zeros((nSymbols, nModes), dtype=np.float64)
+    # Check and set default values for input parameters
+    Nfft = getattr(param, "Nfft", 512)
+    G = getattr(param, "G", 4)
+    hermitSymmetry = getattr(param, "hermitSymmetry", False)
+    pilot = getattr(param, "pilot", 1+1j)
+    pilotCarriers = getattr(param, "pilotCarriers", np.array([], dtype = int))
+    SpS = getattr(param, "SpS", 2)
+        
+    # Number of pilot subcarriers
+    Np = len(pilotCarriers)
+
+    # Number of subcarriers
+    Ns = Nfft//2 - 1 if hermitSymmetry else Nfft
+    numSymb  = len(symb)
+    numOFDMframes = numSymb//(Ns - Np)
+
+    Carriers = np.arange(0, Ns)
+    dataCarriers  = np.array(list(set(Carriers) - set(pilotCarriers)))
+
+    # Serial to parallel
+    symb_par = np.reshape(symb, (numOFDMframes, Ns - Np))   
+    sigOFDM_par = np.zeros( (numOFDMframes, SpS*(Nfft + G)), dtype=np.complex64)
+    
+    for indFrame in range(numOFDMframes):
+        # Start OFDM frame with zeros
+        frameOFDM = np.zeros(Ns, dtype=np.complex64) 
+
+        # Insert data and pilot subcarriers                    
+        frameOFDM[dataCarriers]  = symb_par[indFrame, :]
+        frameOFDM[pilotCarriers] = pilot
+
+        # Hermitian symmetry
+        if hermitSymmetry:
+            frameOFDM = hermit(frameOFDM)
+       
+        # IFFT operation       
+        sigOFDM_par[indFrame, SpS*G : SpS*(G + Nfft)] = ifft(fftshift(zeroPad(frameOFDM, (Nfft*(SpS-1))//2))) * np.sqrt(SpS*Nfft)
+        
+        # Cyclic prefix addition
+        if G > 0:
+            sigOFDM_par[indFrame, 0 : SpS*G] = sigOFDM_par[indFrame, Nfft*SpS : SpS*(Nfft + G)].copy()
 
-    # Loop filter coefficients
-    a1b = np.array(
-        [
-            1,
-            Ts / (2 * tau1) * (1 - 1 / np.tan(Ts / (2 * tau2))),
-            Ts / (2 * tau1) * (1 + 1 / np.tan(Ts / (2 * tau2))),
-        ]
-    )
-
-    u = np.zeros(3, dtype=np.float64)  # [u_f, u_d1, u_d]
-
-    for n in range(nModes):
-        u[2] = 0  # Output of phase detector (residual phase error)
-        u[0] = 0  # Output of loop filter
-
-        for k in range(Ei.shape[0]):
-            u[1] = u[2]
-
-            # Remove estimate of phase error from input symbol
-            Eo = Ei[k, n] * np.exp(1j * θ[k, n])
-
-            # Slicer (perform hard decision on symbol)
-            if k in pilotInd:
-                # phase estimation with pilot symbol
-                # Generate phase error signal (also called x_n (Meyer))
-                u[2] = np.imag(Eo * np.conj(symbTx[k, n]))
-            else:
-                # find closest constellation symbol
-                decided = np.argmin(np.abs(Eo - constSymb))
-                # Generate phase error signal (also called x_n (Meyer))
-                u[2] = np.imag(Eo * np.conj(constSymb[decided]))
-            # Pass phase error signal in Loop Filter (also called e_n (Meyer))
-            u[0] = np.sum(a1b * u)
-
-            # Estimate the phase error for the next symbol
-            if k < Ei.shape[0] - 1:
-                θ[k + 1, n] = θ[k, n] - Kv * u[0]
-    return θ
+    return sigOFDM_par.ravel()
 
 
-def viterbi(Ei, N=35, M=4):
+def demodulateOFDM(sig, param):
     """
-    Viterbi & Viterbi carrier phase recovery algorithm.
+    Demodulate OFDM signal.
 
     Parameters
     ----------
-    Ei : ndarray
-        Input signal.
-    N : int, optional
-        Size of the moving average window.
-    M : int, optional
-        M-th power order.
+    sig : np.np.array
+        Complex-valued array representing the OFDM signal sequence received at one sample per symbol.
+    param : optic.utils.parameters object
+        An object containing the parameters for OFDM demodulation.
 
-    Returns
-    -------
-    ndarray, float
-        Estimated phase error.
-    """
-    return (
-        -np.unwrap(
-            np.angle(movingAverage(Ei**M, N)) / M, period=2 * np.pi / M, axis=0
-        )
-        - np.pi / 4
-    )
+        - Nfft : scalar, optional. Size of the FFT. Default is 512.
 
+        - N : scalar, optional. Number of transmitted subcarriers. Default is calculated based on `Nfft`.
 
-def fourthPowerFOE(Ei, Fs, plotSpec=False):  # sourcery skip: extract-method
-    """
-    Estimate the frequency offset (FO) with the 4th-power method.
+        - G : scalar, optional. Cyclic prefix length. Default is 4.
 
-    Parameters
-    ----------
-    Ei : ndarray
-        Input signal.
-    Fs : float
-        Sampling frequency.
-    plotSpec : bool, optional
-        Whether to plot the spectrum. Default is False.
+        - hermitSymmetry : bool, optional.If True, indicates real OFDM symbols; if False, indicates complex OFDM symbols. Default is False.
+
+        - pilot : complex-valued scalar, optional. Pilot symbol. Default is 1 + 1j.
+
+        - pilotCarriers : np.array, optional.Indexes of pilot subcarriers. Default is an empty array.
+
+        - returnChannel : bool, optional. If True, return the estimated channel. Default is False.
 
     Returns
     -------
-    ndarray, float
-        - The output signal after applying frequency offset correction.
-        - The estimated frequency offset.
+    np.array or tuple
+        If `returnChannel` is False, returns a complex-valued array representing the demodulated symbols sequence received.
+        If `returnChannel` is True, returns a tuple containing the demodulated symbols sequence received and the estimated channel.
+
+    Notes
+    -----
+    - The input signal must be sampled at one sample per symbol.
+    - This function performs demodulation of the OFDM signal according to the provided parameters, including channel estimation and single tap equalization.
 
+    References
+    ----------
+    [1] Proakis, J. G., & Salehi, M. Digital Communications (5th Edition). McGraw-Hill Education, 2008.
     """
-    Nfft = Ei.shape[0]
+    # Check and set default values for input parameters
+    Nfft = getattr(param, "Nfft", 512)
+    G = getattr(param, "G", 4)
+    hermitSymmetry = getattr(param, "hermitSymmetry", False)
+    pilot = getattr(param, "pilot", 1+1j)
+    pilotCarriers = getattr(param, "pilotCarriers", np.array([], dtype = int))
+    returnChannel = getattr(param,'returnChannel', False)
+    
+    # Number of pilot subcarriers
+    Np = len(pilotCarriers)
+
+    # Number of subcarriers
+    N = Nfft//2 - 1 if hermitSymmetry else Nfft
+    Carriers      = np.arange(0, N)
+    dataCarriers  = np.array(list(set(Carriers) - set(pilotCarriers)))
+
+    H_abs = 0
+    H_pha = 0
+
+    numSymb       = len(sig)
+    numOFDMframes = numSymb//(Nfft + G)
+
+    sig_par = np.reshape(sig, (numOFDMframes, Nfft + G))
+
+    # Cyclic prefix removal
+    sig_par = sig_par[:, G : G + Nfft]
+
+    # FFT operation
+    for indFrame in range(numOFDMframes):
+        sig_par[indFrame, :] = fftshift(fft(sig_par[indFrame,:])) / np.sqrt(Nfft)
+
+    if hermitSymmetry:
+        # Removal of hermitian symmetry
+        sig_par = sig_par[:, 1 : 1 + N]
+
+    # Channel estimation and single tap equalization    
+    if Np != 0:
+        # Channel estimation
+        for indFrame in range(numOFDMframes):
+            H_est = sig_par[indFrame, :][pilotCarriers] / pilot
+
+            H_abs += interp1d(pilotCarriers, np.abs(H_est), kind = 'linear', fill_value = "extrapolate")(Carriers)
+            H_pha += interp1d(pilotCarriers, np.angle(H_est), kind = 'linear', fill_value = "extrapolate")(Carriers)
+
+            if(indFrame == numOFDMframes - 1):
+                H_abs = H_abs/numOFDMframes
+                H_pha = H_pha/numOFDMframes
+
+        for indFrame in range(numOFDMframes):
+            sig_par[indFrame, :] = sig_par[indFrame, :] / (H_abs*np.exp(1j*H_pha))
 
-    f = Fs * fftfreq(Nfft)
-    f = fftshift(f)
+        # Pilot extraction
+        sig_par = sig_par[:, dataCarriers]
 
-    nModes = Ei.shape[1]
-    Eo = Ei.copy()
-    t = np.arange(0, Eo.shape[0]) * 1 / Fs
-
-    for n in range(nModes):
-        f4 = 10 * np.log10(np.abs(fftshift(fft(Ei[:, n] ** 4))))
-        indFO = np.argmax(f4)
-        fo = f[indFO] / 4
-        Eo[:, n] = Ei[:, n] * np.exp(-1j * 2 * np.pi * fo * t)
-
-    if plotSpec:
-        plotSpectrum(f, f4, indFO)
-    return Eo, f[indFO] / 4
-
-
-def plotSpectrum(f, f4, indFO):
-    plt.figure()
-    plt.plot(f, f4, label="$|FFT(s[k]^4)|[dB]$")
-    plt.plot(f[indFO], f4[indFO], "x", label="$4f_o$")
-    plt.legend()
-    plt.xlim(min(f), max(f))
-    plt.grid()
+    if returnChannel:
+        return sig_par.ravel(), H_abs*np.exp(1j*H_pha)
+    else:
+        return sig_par.ravel()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `OptiCommPy-0.7.0/optic/dsp/core.py` & `OptiCommPy-0.9.0/optic/dsp/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,14 +27,15 @@
    movingAverage          -- Calculate the sliding window moving average
 """
 
 """Digital signal processing utilities."""
 import numpy as np
 from numba import njit, prange
 from scipy import signal
+from numpy.fft import fft, ifft, fftfreq, fftshift
 
 
 @njit
 def sigPow(x):
     """
     Calculate the average power of x per mode.
 
@@ -83,14 +84,18 @@
     prec: cp.dtype
         Size of the complex representation.
 
     Returns
     -------
     y : np.array
         Output (filtered) signal.
+
+    References
+    ----------
+    [1] P. S. R. Diniz, E. A. B. da Silva, e S. L. Netto, Digital Signal Processing: System Analysis and Design. Cambridge University Press, 2010.
     """
     try:
         x.shape[1]
     except IndexError:
         x = x.reshape(len(x), 1)
     y = x.copy()
     nModes = x.shape[1]
@@ -98,34 +103,31 @@
     for n in range(nModes):
         y[:, n] = np.convolve(x[:, n], h, mode="same")
     if y.shape[1] == 1:
         y = y[:, 0]
     return y
 
 
-import numpy as np
-
-
 @njit
 def rrcFilterTaps(t, alpha, Ts):
     """
     Generate Root-Raised Cosine (RRC) filter coefficients.
 
     Parameters
     ----------
-    t : array-like
+    t : np.array
         Time values.
     alpha : float
         RRC roll-off factor.
     Ts : float
         Symbol period.
 
     Returns
     -------
-    coeffs : ndarray
+    coeffs : np.array
         RRC filter coefficients.
 
     References
     ----------
     [1] Proakis, J. G., & Salehi, M. (2008). Digital Communications (5th Edition). McGraw-Hill Education.
     """
     coeffs = np.zeros(len(t), dtype=np.float64)
@@ -156,24 +158,24 @@
 @njit
 def rcFilterTaps(t, alpha, Ts):
     """
     Generate Raised Cosine (RC) filter coefficients.
 
     Parameters
     ----------
-    t : array-like
+    t : np.array
         Time values.
     alpha : float
         RC roll-off factor.
     Ts : float
         Symbol period.
 
     Returns
     -------
-    coeffs : ndarray
+    coeffs : np.array
         RC filter coefficients.
 
     References
     ----------
     [1] Proakis, J. G., & Salehi, M. (2008). Digital Communications (5th Edition). McGraw-Hill Education.
     """
     coeffs = np.zeros(len(t), dtype=np.float64)
@@ -247,27 +249,27 @@
 @njit(parallel=True)
 def clockSamplingInterp(x, Fs_in=1, Fs_out=1, jitter_rms=1e-9):
     """
     Interpolate signal to a given sampling rate.
 
     Parameters
     ----------
-    x : ndarray
+    x : np.array
         Input signal.
     param : core.parameter
         Resampling parameters:
             - param.Fs_in  : sampling frequency of the input signal.
 
             - param.Fs_out : sampling frequency of the output signal.
 
             - param.jitter_rms: standard deviation of the time jitter.
 
     Returns
     -------
-    y : ndarray
+    y : np.array
         Resampled signal.
 
     """
     nModes = x.shape[1]
 
     inTs = 1 / Fs_in
     outTs = 1 / Fs_out
@@ -337,14 +339,18 @@
         Type of response ('rect', 'gauss'). The default is "rect".
 
     Returns
     -------
     h : np.array
         Filter coefficients.
 
+    References
+    ----------
+    [1] P. S. R. Diniz, E. A. B. da Silva, e S. L. Netto, Digital Signal Processing: System Analysis and Design. Cambridge University Press, 2010.
+
     """
     fu = fc / fa
     d = (N - 1) / 2
     n = np.arange(0, N)
 
     # calculate filter coefficients
     if typeF == "rect":
@@ -360,33 +366,37 @@
 
 def upsample(x, factor):
     """
     Upsample a signal by inserting zeros between samples.
 
     Parameters
     ----------
-    x : array-like
+    x : np.array
         Input signal to upsample.
     factor : int
         Upsampling factor. The signal will be upsampled by inserting
         `factor - 1` zeros between each original sample.
 
     Returns
     -------
-    xUp : array-like
+    xUp : np.array
         The upsampled signal with zeros inserted between samples.
 
     Notes
     -----
     This function inserts zeros between the samples of the input signal to
     increase its sampling rate. The upsampling factor determines how many
     zeros are inserted between each original sample.
 
     If the input signal is a 2D array, the upsampling is performed
     column-wise.
+
+    References
+    ----------
+    [1] P. S. R. Diniz, E. A. B. da Silva, e S. L. Netto, Digital Signal Processing: System Analysis and Design. Cambridge University Press, 2010.
     """
     try:
         xUp = np.zeros((factor * x.shape[0], x.shape[1]), dtype=x.dtype)
         xUp[0::factor, :] = x
     except IndexError:
         xUp = np.zeros(factor * x.shape[0], dtype=x.dtype)
         xUp[0::factor] = x
@@ -410,14 +420,18 @@
         - param.SpS_out : samples per symbol of the output signal.
 
     Returns
     -------
     Eo : np.array
         Decimated signal.
 
+    References
+    ----------
+    [1] P. S. R. Diniz, E. A. B. da Silva, e S. L. Netto, Digital Signal Processing: System Analysis and Design. Cambridge University Press, 2010.
+
     """
     try:
         Ei.shape[1]
     except IndexError:
         Ei = Ei.reshape(len(Ei), 1)
 
     decFactor = int(param.SpS_in / param.SpS_out)
@@ -442,29 +456,33 @@
 
 def resample(Ei, param):
     """
     Resample signal to a given sampling rate.
 
     Parameters
     ----------
-    Ei : ndarray
+    Ei : np.array
         Input signal.
     param : core.parameter
         Resampling parameters:
             - param.Rs      : symbol rate of the signal.
 
             - param.SpS_in  : samples per symbol of the input signal.
-            
+
             - param.SpS_out : samples per symbol of the output signal.
 
     Returns
     -------
-    Eo : ndarray
+    Eo : np.array
         Resampled signal.
 
+    References
+    ----------
+    [1] P. S. R. Diniz, E. A. B. da Silva, e S. L. Netto, Digital Signal Processing: System Analysis and Design. Cambridge University Press, 2010.
+
     """
     try:
         Ei.shape[1]
     except IndexError:
         Ei = Ei.reshape(len(Ei), 1)
     nModes = Ei.shape[1]
     inFs = param.SpS_in * param.Rs
@@ -501,26 +519,27 @@
     tx : np.array
         Transmitted symbol sequence.
     SpS : int
         Samples per symbol of input signals.
 
     Returns
     -------
-    tx : ndarray
+    tx : np.array
         Transmitted sequence synchronized to rx.
 
     """
     nModes = rx.shape[1]
 
     rx = rx[0::SpS, :]
 
     # calculate time delay
     delay = np.zeros(nModes)
 
     corrMatrix = np.zeros((nModes, nModes))
+    rot = np.ones((nModes, nModes), dtype=np.complex64)
 
     if mode == "amp":
         for n in range(nModes):
             for m in range(nModes):
                 corrMatrix[m, n] = np.max(
                     np.abs(signal.correlate(np.abs(tx[:, m]), np.abs(rx[:, n])))
                 )
@@ -529,23 +548,30 @@
         tx = tx[:, swap]
 
         for k in range(nModes):
             delay[k] = finddelay(np.abs(tx[:, k]), np.abs(rx[:, k]))
     elif mode == "real":
         for n in range(nModes):
             for m in range(nModes):
-                corrMatrix[m, n] = np.max(
+                c1 = np.max(
                     np.abs(signal.correlate(np.real(tx[:, m]), np.real(rx[:, n])))
                 )
-        swap = np.argmax(corrMatrix, axis=0)
+                c2 = np.max(
+                    np.abs(signal.correlate(np.real(tx[:, m]), np.imag(rx[:, n])))
+                )
+                corrMatrix[m, n] = np.max([c1, c2])
+
+                if c2 > c1:
+                    rot[m, n] = np.exp(-1j * np.pi / 4)
 
+        swap = np.argmax(corrMatrix, axis=0)
         tx = tx[:, swap]
 
         for k in range(nModes):
-            delay[k] = finddelay(np.real(tx[:, k]), np.real(rx[:, k]))
+            delay[k] = finddelay(np.real(rot[k, swap[k]] * tx[:, k]), np.real(rx[:, k]))
 
     # compensate time delay
     for k in range(nModes):
         tx[:, k] = np.roll(tx[:, k], -int(delay[k]))
     return tx
 
 
@@ -562,15 +588,15 @@
 
     Returns
     -------
     d : int
         Delay between x and y, in samples.
 
     """
-    return np.argmax(signal.correlate(x, y)) - x.shape[0] + 1
+    return np.argmax(np.abs(signal.correlate(x, y))) - x.shape[0] + 1
 
 
 @njit
 def pnorm(x):
     """
     Normalize the average power of each componennt of x.
 
@@ -592,21 +618,21 @@
 def gaussianComplexNoise(shapeOut, σ2=1.0):
     """
     Generate complex circular Gaussian noise.
 
     Parameters
     ----------
     shapeOut : tuple of int
-        Shape of ndarray to be generated.
+        Shape of np.array to be generated.
     σ2 : float, optional
         Variance of the noise (default is 1).
 
     Returns
     -------
-    noise : ndarray
+    noise : np.array
         Generated complex circular Gaussian noise.
     """
     return np.random.normal(0, np.sqrt(σ2 / 2), shapeOut) + 1j * np.random.normal(
         0, np.sqrt(σ2 / 2), shapeOut
     )
 
 
@@ -614,21 +640,21 @@
 def gaussianNoise(shapeOut, σ2=1.0):
     """
     Generate Gaussian noise.
 
     Parameters
     ----------
     shapeOut : tuple of int
-        Shape of ndarray to be generated.
+        Shape of np.array to be generated.
     σ2 : float, optional
         Variance of the noise (default is 1).
 
     Returns
     -------
-    noise : ndarray
+    noise : np.array
         Generated Gaussian noise.
     """
     return np.random.normal(0, np.sqrt(σ2), shapeOut)
 
 
 @njit
 def phaseNoise(lw, Nsamples, Ts):
@@ -645,14 +671,18 @@
         sampling period.
 
     Returns
     -------
     phi : np.array
         realization of the phase noise process.
 
+    References
+    ----------
+    [1] M. Seimetz, High-Order Modulation for Optical Fiber Transmission. em Springer Series in Optical Sciences. Springer Berlin Heidelberg, 2009.
+
     """
     σ2 = 2 * np.pi * lw * Ts
     phi = np.zeros(Nsamples)
 
     for ind in range(Nsamples - 1):
         phi[ind + 1] = phi[ind] + np.random.normal(0, np.sqrt(σ2))
 
@@ -661,44 +691,82 @@
 
 def movingAverage(x, N):
     """
     Calculate the sliding window moving average of a 2D NumPy array along each column.
 
     Parameters
     ----------
-    x : numpy.ndarray
+    x : numpy.np.array
         Input 2D array with shape (M, N), where M is the number of samples and N is the number of columns.
     N : int
         Size of the sliding window.
 
     Returns
     -------
-    numpy.ndarray
+    numpy.np.array
         2D array containing the sliding window moving averages along each column.
 
     Notes
     -----
     The function pads the signal with zeros at both ends to compensate for the lag between the output
     of the moving average and the original signal.
 
     """
     nCol = x.shape[1]
     y = np.zeros(x.shape, dtype=x.dtype)
 
-    startInd = N//2
-
-    if N%2:
-        endInd = -N//2+1
-    else:
-        endInd = -N//2
+    startInd = N // 2
 
+    endInd = -N // 2 + 1 if N % 2 else -N // 2
     for indCol in range(nCol):
         # Pad the signal with zeros at both ends
-        padded_x = np.pad(x[:, indCol], (N//2, N//2), mode='constant')
+        padded_x = np.pad(x[:, indCol], (N // 2, N // 2), mode="constant")
 
         # Calculate moving average using convolution
         h = np.ones(N) / N
-        ma = np.convolve(padded_x, h, 'same')
+        ma = np.convolve(padded_x, h, "same")
         y[:, indCol] = ma[startInd:endInd]
 
     return y
 
+
+def delaySignal(sig, delay, fs):
+    """
+    Apply a time delay to a signal sampled at fs samples per second using FFT/IFFT algorithms.
+    
+    Parameters
+    ----------
+    sig : array_like
+        The input signal.
+    delay : float
+        The time delay to apply to the signal (in seconds).
+    fs : float
+        Sampling frequency of the signal (in samples per second).
+    
+    Returns
+    -------
+    array_like
+        The delayed signal.
+    """
+    # Calculate the length of the signal
+    N = len(sig)    
+
+    # Calculate the length of zero padding needed
+    pad_length = int(np.ceil(delay * fs))
+    
+    # Zero-pad the signal to avoid circular shift
+    sig_padded = np.pad(sig, (0, pad_length), mode='constant')
+       
+    # Compute the frequency vector
+    freq = fftshift(fftfreq(len(sig_padded), d=1/fs))
+    
+    # Compute the FFT of the signal
+    sig_fft = fftshift(fft(sig_padded))
+    
+    # Apply the phase shift corresponding to the time delay
+    phase_shift = np.exp(-1j * 2 * np.pi * freq * delay)
+    delayed_sig_fft = fftshift(sig_fft * phase_shift)
+    
+    # Compute the IFFT of the delayed signal
+    delayed_sig = ifft(delayed_sig_fft)[:N]
+    
+    return delayed_sig
```

### Comparing `OptiCommPy-0.7.0/optic/dsp/coreGPU.py` & `OptiCommPy-0.9.0/optic/dsp/coreGPU.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,14 +15,18 @@
     prec: cp.dtype
         Size of the complex representation.
 
     Returns
     -------
     y : np.array
         Output (filtered) signal.
+
+    References
+    ----------
+    [1] P. S. R. Diniz, E. A. B. da Silva, e S. L. Netto, Digital Signal Processing: System Analysis and Design. Cambridge University Press, 2010.
     """
     try:
         x.shape[1]
     except IndexError:
         x = x.reshape(len(x), 1)
     nModes = x.shape[1]
```

### Comparing `OptiCommPy-0.7.0/optic/dsp/equalization.py` & `OptiCommPy-0.9.0/optic/dsp/equalization.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import numpy as np
 import scipy.constants as const
 from numba import njit
 from numpy.fft import fft, fftfreq, ifft
 from tqdm.notebook import tqdm
 from optic.dsp.core import pnorm
 from optic.models.channels import linearFiberChannel
-from optic.comm.modulation import GrayMapping
+from optic.comm.modulation import grayMapping
 
 
 def edc(Ei, param):
     """
     Electronic chromatic dispersion compensation (EDC).
 
     Parameters
@@ -44,102 +44,122 @@
         - param.Fs: sampling frequency [Hz] [default: []]
 
     Returns
     -------
     np.array
         CD compensated signal.
 
+    References
+    ----------
+
+    [1] S. J. Savory, “Digital coherent optical receivers: Algorithms and subsystems”, IEEE Journal on Selected Topics in Quantum Electronics, vol. 16, nº 5, p. 1164–1179, set. 2010, doi: 10.1109/JSTQE.2010.2044751.
+
+    [2] K. Kikuchi, “Fundamentals of Coherent Optical Fiber Communications”, J. Lightwave Technol., JLT, vol. 34, nº 1, p. 157–179, jan. 2016.
+
     """
     try:
         Fs = param.Fs
     except AttributeError:
         logg.error("Simulation sampling frequency (Fs) not provided.")
 
     # check input parameters
     param.L = getattr(param, "L", 50)
     param.D = getattr(param, "D", 16)
     param.Fc = getattr(param, "Fc", 193.1e12)
 
     param.alpha = 0
     param.D = -param.D
+    logg.info(f"Running CD compensation...")
 
     return linearFiberChannel(Ei, param)
 
 
 def mimoAdaptEqualizer(x, param=None, dx=None):
     """
     N-by-N MIMO adaptive equalizer.
-
-    Algorithms available: 'cma', 'rde', 'nlms', 'dd-lms', 'da-rde', 'rls', 'dd-rls', 'static'.
-
+    
     Parameters
     ----------
-    x : array-like
+    x : np.array
         Input array.
+    dx : np.array, optional
+        Syncronized exact symbol sequence corresponding to the received input array x.
     param : object, optional
         Parameter object containing the following attributes:
 
         - numIter : int, number of pre-convergence iterations (default: 1)
 
         - nTaps : int, number of filter taps (default: 15)
 
         - mu : float or list of floats, step size parameter(s) (default: [1e-3])
 
         - lambdaRLS : float, RLS forgetting factor (default: 0.99)
 
         - SpS : int, samples per symbol (default: 2)
 
-        - H : array-like, coefficient matrix (default: [])
+        - H : np.array, coefficient matrix (default: [])
 
         - L : int or list of ints, length of the output of the training section (default: [])
 
         - Hiter : list, history of coefficient matrices (default: [])
 
         - storeCoeff : bool, flag indicating whether to store coefficient matrices (default: False)
 
+        - runWL: bool, flag indicating whether to run the equalizer in the widely-linear mode. (default: False)
+
         - alg : str or list of strs, specifying the equalizer algorithm(s) (default: ['nlms'])
 
         - constType : str, constellation type (default: 'qam')
 
         - M : int, modulation order (default: 4)
 
         - prgsBar : bool, flag indicating whether to display progress bar (default: True)
 
-        - returnResults : bool, return filters, MSE and filters per iteration
-
-    dx : array-like, optional
-        Syncronized exact symbol sequence corresponding to the received input array x.
-
     Returns
     -------
-    yEq : array-like
+    yEq : np.array
         Equalized output array.
-    H : array-like
+    H : np.array
         Coefficient matrix.
-    errSq : array-like
+    errSq : np.array
         Squared absolute error array.
     Hiter : list
         History of coefficient matrices.
 
+    Notes
+    -----
+    Algorithms available: 'cma', 'rde', 'nlms', 'dd-lms', 'da-rde', 'rls', 'dd-rls', 'static'.
+
+    References
+    ----------
+    [1] P. S. R. Diniz, Adaptive Filtering: Algorithms and Practical Implementation. Springer US, 2012.
+
+    [2] S. J. Savory, “Digital coherent optical receivers: Algorithms and subsystems”, IEEE Journal on Selected Topics in Quantum Electronics, vol. 16, nº 5, p. 1164–1179, set. 2010, doi: 10.1109/JSTQE.2010.2044751.
+
+    [3] K. Kikuchi, “Fundamentals of Coherent Optical Fiber Communications”, J. Lightwave Technol., JLT, vol. 34, nº 1, p. 157–179, jan. 2016.
+
+    [4] E. P. Da Silva e D. Zibar, “Widely Linear Equalization for IQ Imbalance and Skew Compensation in Optical Coherent Receivers”, Journal of Lightwave Technology, vol. 34, nº 15, p. 3577–3586, ago. 2016, doi: 10.1109/JLT.2016.2577716.
     """
     if dx is None:
         dx = []
     if param is None:
         param = []
 
     # check input parameters
     numIter = getattr(param, "numIter", 1)
     nTaps = getattr(param, "nTaps", 15)
     mu = getattr(param, "mu", [1e-3])
     lambdaRLS = getattr(param, "lambdaRLS", 0.99)
     SpS = getattr(param, "SpS", 2)
     H = getattr(param, "H", [])
+    H_ = getattr(param, "H_", [])
     L = getattr(param, "L", [])
     Hiter = getattr(param, "Hiter", [])
     storeCoeff = getattr(param, "storeCoeff", False)
+    runWL = getattr(param, "runWL", False)
     alg = getattr(param, "alg", ["nlms"])
     constType = getattr(param, "constType", "qam")
     M = getattr(param, "M", 4)
     prgsBar = getattr(param, "prgsBar", True)
     returnResults = getattr(param, "returnResults", False)
 
     # We want all the signal sequences to be disposed in columns:
@@ -160,15 +180,15 @@
     Lpad = int(np.floor(nTaps / 2))
     zeroPad = np.zeros((Lpad, nModes), dtype="complex")
     x = np.concatenate(
         (zeroPad, x, zeroPad)
     )  # pad start and end of the signal with zeros
 
     # Defining training parameters:
-    constSymb = GrayMapping(M, constType)  # constellation
+    constSymb = grayMapping(M, constType)  # constellation
     constSymb = pnorm(constSymb)  # normalized constellation symbols
 
     totalNumSymb = int(np.fix((len(x) - nTaps) / SpS + 1))
 
     if not L:  # if L is not defined
         L = [
             totalNumSymb
@@ -176,14 +196,19 @@
     if not H:  # if H is not defined
         H = np.zeros((nModes**2, nTaps), dtype="complex")
 
         for initH in range(nModes):  # initialize filters' taps
             H[
                 initH + initH * nModes, int(np.floor(H.shape[1] / 2))
             ] = 1  # Central spike initialization
+    if not H_:  # if H_ is not defined      
+        H_ = np.zeros((nModes**2, nTaps), dtype="complex")
+
+
+    logg.info(f"Running adaptive equalizer...")
     # Equalizer training:
     if type(alg) == list:
         yEq = np.zeros((totalNumSymb, x.shape[1]), dtype="complex")
         errSq = np.zeros((totalNumSymb, x.shape[1])).T
 
         nStart = 0
         for indstage, runAlg in enumerate(alg):
@@ -192,102 +217,112 @@
             nEnd = nStart + L[indstage]
 
             if indstage == 0:
                 for indIter in tqdm(range(numIter), disable=not (prgsBar)):
                     logg.info(
                         f"{runAlg} pre-convergence training iteration #%d", indIter
                     )
-                    yEq[nStart:nEnd, :], H, errSq[:, nStart:nEnd], Hiter = coreAdaptEq(
+                    yEq[nStart:nEnd, :], H, H_, errSq[:, nStart:nEnd], Hiter = coreAdaptEq(
                         x[nStart * SpS : (nEnd + 2 * Lpad) * SpS, :],
                         dx[nStart:nEnd, :],
                         SpS,
                         H,
+                        H_,
                         L[indstage],
                         mu[indstage],
                         lambdaRLS,
                         nTaps,
                         storeCoeff,
+                        runWL,
                         runAlg,
                         constSymb,
                     )
                     logg.info(
                         f"{runAlg} MSE = %.6f.", np.nanmean(errSq[:, nStart:nEnd])
                     )
             else:
-                yEq[nStart:nEnd, :], H, errSq[:, nStart:nEnd], Hiter = coreAdaptEq(
+                yEq[nStart:nEnd, :], H, H_, errSq[:, nStart:nEnd], Hiter = coreAdaptEq(
                     x[nStart * SpS : (nEnd + 2 * Lpad) * SpS, :],
                     dx[nStart:nEnd, :],
                     SpS,
                     H,
+                    H_,
                     L[indstage],
                     mu[indstage],
                     lambdaRLS,
                     nTaps,
                     storeCoeff,
+                    runWL,
                     runAlg,
                     constSymb,
                 )
                 logg.info(f"{runAlg} MSE = %.6f.", np.nanmean(errSq[:, nStart:nEnd]))
             nStart = nEnd
     else:
         for indIter in tqdm(range(numIter), disable=not (prgsBar)):
             logg.info(f"{alg}training iteration #%d", indIter)
             yEq, H, errSq, Hiter = coreAdaptEq(
                 x, dx, SpS, H, L, mu, nTaps, storeCoeff, alg, constSymb
             )
             logg.info(f"{alg}MSE = %.6f.", np.nanmean(errSq))
 
     if returnResults:
-        if storeCoeff:
+        if runWL:
+            return yEq, H, H_, errSq, Hiter
+        else: 
             return yEq, H, errSq, Hiter
-        else:
-            return yEq, H, errSq
     else:
         return yEq
 
 
 @njit
-def coreAdaptEq(x, dx, SpS, H, L, mu, lambdaRLS, nTaps, storeCoeff, alg, constSymb):
+def coreAdaptEq(x, dx, SpS, H, H_, L, mu, lambdaRLS, nTaps, storeCoeff, runWL, alg, constSymb):
     """
     Adaptive equalizer core processing function
 
     Parameters
     ----------
-    x : array-like
+    x : np.array
         Input array.
-    dx : array-like
+    dx : np.array
         Exact constellation radius array.
     SpS : int
         Samples per symbol.
-    H : array-like
+    H : np.array
         Coefficient matrix.
+    H_ : np.array
+        Augmented coefficient matrix.
     L : int
         Length of the output.
     mu : float
         Step size parameter.
     lambdaRLS : float
         RLS forgetting factor.
     nTaps : int
         Number of taps.
     storeCoeff : bool
         Flag indicating whether to store coefficient matrices.
+    runWL : bool
+        Run widely-linear mode
     alg : str
         Equalizer algorithm.
-    constSymb : array-like
+    constSymb : np.array
         Constellation symbols.
 
     Returns
     -------
-    yEq : array-like
+    yEq : np.array
         Equalized output array.
-    H : array-like
+    H : np.array
         Coefficient matrix.
-    errSq : array-like
+    H_ : np.array
+        Augmented coefficient matrix.
+    errSq : np.array
         Squared absolute error array.
-    Hiter : array-like
+    Hiter : np.array
         History of coefficient matrices.
 
     """
     # allocate variables
     nModes = int(x.shape[1])
     indTaps = np.arange(0, nTaps)
     indMode = np.arange(0, nModes)
@@ -327,28 +362,33 @@
 
         # pass signal sequence through the equalizer:
         for N in range(nModes):
             inEq = x[indIn, N : N + 1]  # slice input coming from the Nth mode
             outEq += (
                 H[indMode + N * nModes, :] @ inEq
             )  # add contribution from the Nth mode to the equalizer's output
+            if runWL:
+                outEq += (
+                    H_[indMode + N * nModes, :] @ np.conj(inEq)
+                )  # add augmented contribution from the Nth mode to the equalizer's output
+
         yEq[ind, :] = outEq.T
 
         # update equalizer taps acording to the specified
         # algorithm and save squared error:
         if alg == "nlms":
-            H, errSq[:, ind] = nlmsUp(x[indIn, :], dx[ind, :], outEq, mu, H, nModes)
+            H, H_, errSq[:, ind] = nlmsUp(x[indIn, :], dx[ind, :], outEq, mu, H, H_, nModes, runWL)
         elif alg == "cma":
-            H, errSq[:, ind] = cmaUp(x[indIn, :], Rcma, outEq, mu, H, nModes)
+            H, H_, errSq[:, ind] = cmaUp(x[indIn, :], Rcma, outEq, mu, H, H_, nModes, runWL)
         elif alg == "dd-lms":
-            H, errSq[:, ind] = ddlmsUp(x[indIn, :], constSymb, outEq, mu, H, nModes)
+            H, H_, errSq[:, ind] = ddlmsUp(x[indIn, :], constSymb, outEq, mu, H, H_, nModes, runWL)
         elif alg == "rde":
-            H, errSq[:, ind] = rdeUp(x[indIn, :], Rrde, outEq, mu, H, nModes)
+            H, H_, errSq[:, ind] = rdeUp(x[indIn, :], Rrde, outEq, mu, H, H_, nModes, runWL)
         elif alg == "da-rde":
-            H, errSq[:, ind] = dardeUp(x[indIn, :], dx[ind, :], outEq, mu, H, nModes)
+            H, H_, errSq[:, ind] = dardeUp(x[indIn, :], dx[ind, :], outEq, mu, H, H_, nModes, runWL)
         elif alg == "rls":
             H, Sd, errSq[:, ind] = rlsUp(
                 x[indIn, :], dx[ind, :], outEq, lambdaRLS, H, Sd, nModes
             )
         elif alg == "dd-rls":
             H, Sd, errSq[:, ind] = ddrlsUp(
                 x[indIn, :], constSymb, outEq, lambdaRLS, H, Sd, nModes
@@ -359,42 +399,49 @@
             raise ValueError(
                 "Equalization algorithm not specified (or incorrectly specified)."
             )
         if storeCoeff:
             Hiter[:, :, ind] = H
         else:
             Hiter[:, :, 0] = H
-    return yEq, H, errSq, Hiter
+
+    return yEq, H, H_, errSq, Hiter
 
 
 @njit
-def nlmsUp(x, dx, outEq, mu, H, nModes):
+def nlmsUp(x, dx, outEq, mu, H, H_, nModes, runWL):
     """
     Coefficient update with the NLMS algorithm.
 
     Parameters
     ----------
-    x : array-like
+    x : np.array
         Input array.
-    dx : array-like
+    dx : np.array
         Desired output array.
-    outEq : array-like
+    outEq : np.array
         Equalized output array.
     mu : float
         Step size for the update.
-    H : array-like
+    H : np.array
         Coefficient matrix.
+    H_ : np.array
+        Augmented coefficient matrix.
     nModes : int
         Number of modes.
+    runWL: bool
+        Run widely-linear mode.
 
     Returns
     -------
-    H : array-like
+    H : np.array
         Updated coefficient matrix.
-    err_sq : array-like
+    H : np.array
+        Updated augmented coefficient matrix.
+    err_sq : np.array
         Squared absolute error.
 
     """
     indMode = np.arange(0, nModes)
     err = dx - outEq.T  # calculate output error for the NLMS algorithm
 
     errDiag = np.diag(err[0])  # define diagonal matrix from error array
@@ -405,46 +452,49 @@
         inAdapt = x[:, N].T / np.linalg.norm(x[:, N]) ** 2  # NLMS normalization
         inAdaptPar = (
             inAdapt.repeat(nModes).reshape(len(x), -1).T
         )  # expand input to parallelize tap adaptation
         H[indUpdTaps, :] += (
             mu * errDiag @ np.conj(inAdaptPar)
         )  # gradient descent update
-    return H, np.abs(err) ** 2
-
+        if runWL:
+            H_[indUpdTaps, :] += (
+                mu * errDiag @ inAdaptPar
+            )  # gradient descent update
+    return H, H_, np.abs(err) ** 2
 
 @njit
 def rlsUp(x, dx, outEq, λ, H, Sd, nModes):
     """
     Coefficient update with the RLS algorithm.
 
     Parameters
     ----------
-    x : array-like
+    x : np.array
         Input array.
-    dx : array-like
+    dx : np.array
         Desired output array.
-    outEq : array-like
+    outEq : np.array
         Equalized output array.
     λ : float
         Forgetting factor.
-    H : array-like
+    H : np.array
         Coefficient matrix.
-    Sd : array-like
+    Sd : np.array
         Inverse correlation matrix.
     nModes : int
         Number of modes.
 
     Returns
     -------
-    H : array-like
+    H : np.array
         Updated coefficient matrix.
-    Sd : array-like
+    Sd : np.array
         Updated inverse correlation matrix.
-    err_sq : array-like
+    err_sq : np.array
         Squared absolute error.
 
     """
     nTaps = H.shape[1]
     indMode = np.arange(0, nModes)
     indTaps = np.arange(0, nTaps)
 
@@ -473,38 +523,44 @@
         H[indUpdModes, :] += errDiag @ (Sd_ @ inAdaptPar.T).T
 
         Sd[indUpdTaps, :] = Sd_
     return H, Sd, np.abs(err) ** 2
 
 
 @njit
-def ddlmsUp(x, constSymb, outEq, mu, H, nModes):
+def ddlmsUp(x, constSymb, outEq, mu, H, H_, nModes, runWL):
     """
     Coefficient update with the DD-LMS algorithm.
 
     Parameters
     ----------
-    x : array-like
+    x : np.array
         Input array.
-    constSymb : array-like
+    constSymb : np.array
         Array of constellation symbols.
-    outEq : array-like
+    outEq : np.array
         Equalized output array.
     mu : float
         Step size for the update.
-    H : array-like
+    H : np.array
         Coefficient matrix.
+    H_ : np.array
+        Augmented coefficient matrix.
     nModes : int
         Number of modes.
+    runWL: bool
+        Run widely-linear mode.
 
     Returns
     -------
-    H : array-like
+    H : np.array
         Updated coefficient matrix.
-    err_sq : array-like
+    H_ : np.array
+        Updated augmented coefficient matrix.
+    err_sq : np.array
         Squared absolute error.
 
     """
     indMode = np.arange(0, nModes)
     outEq = outEq.T
     decided = np.zeros(outEq.shape, dtype=np.complex128)
 
@@ -520,47 +576,51 @@
         indUpdTaps = indMode + N * nModes  # simplify indexing
         inAdapt = x[:, N].T
         inAdaptPar = (
             inAdapt.repeat(nModes).reshape(len(x), -1).T
         )  # expand input to parallelize tap adaptation
         H[indUpdTaps, :] += (
             mu * errDiag @ np.conj(inAdaptPar)
-        )  # gradient descent update
-    return H, np.abs(err) ** 2
+        )  # gradient descent update        
+        if runWL:
+            H_[indUpdTaps, :] += (
+                mu * errDiag @ inAdaptPar
+            )  # gradient descent update   
+    return H, H_, np.abs(err) ** 2
 
 
 @njit
 def ddrlsUp(x, constSymb, outEq, λ, H, Sd, nModes):
     """
     Coefficient update with the DD-RLS algorithm.
 
     Parameters
     ----------
-    x : array-like
+    x : np.array
         Input array.
-    constSymb : array-like
+    constSymb : np.array
         Array of constellation symbols.
-    outEq : array-like
+    outEq : np.array
         Equalized output array.
     λ : float
         Forgetting factor.
-    H : array-like
+    H : np.array
         Coefficient matrix.
-    Sd : array-like
+    Sd : np.array
         Inverse correlation matrix.
     nModes : int
         Number of modes.
 
     Returns
     -------
-    H : array-like
+    H : np.array
         Updated coefficient matrix.
-    Sd : array-like
+    Sd : np.array
         Updated inverse correlation matrix.
-    err_sq : array-like
+    err_sq : np.array
         Squared absolute error.
 
     """
     nTaps = H.shape[1]
     indMode = np.arange(0, nModes)
     indTaps = np.arange(0, nTaps)
 
@@ -595,38 +655,44 @@
         H[indUpdModes, :] += errDiag @ (Sd_ @ inAdaptPar.T).T
 
         Sd[indUpdTaps, :] = Sd_
     return H, Sd, np.abs(err) ** 2
 
 
 @njit
-def cmaUp(x, R, outEq, mu, H, nModes):
+def cmaUp(x, R, outEq, mu, H, H_, nModes, runWL):
     """
     Coefficient update with the CMA algorithm.
 
     Parameters
     ----------
-    x : array-like
+    x : np.array
         Input array.
-    R : array-like
+    R : np.array
         Correlation array.
-    outEq : array-like
+    outEq : np.array
         Equalized output array.
     mu : float
         Step size parameter.
-    H : array-like
+    H : np.array
         Coefficient matrix.
+    H_ : np.array
+        Augmented coefficient matrix.
     nModes : int
         Number of modes.
+    runWL: bool
+        Run widely-linear mode.
 
     Returns
     -------
-    H : array-like
+    H : np.array
         Updated coefficient matrix.
-    err_sq : array-like
+    H_ : np.array
+        Updated augmented coefficient matrix.
+    err_sq : np.array
         Squared absolute error.
 
     """
     indMode = np.arange(0, nModes)
     outEq = outEq.T
     err = R - np.abs(outEq) ** 2  # calculate output error for the CMA algorithm
 
@@ -638,42 +704,52 @@
         inAdapt = x[:, N].T
         inAdaptPar = (
             inAdapt.repeat(nModes).reshape(len(x), -1).T
         )  # expand input to parallelize tap adaptation
         H[indUpdTaps, :] += (
             mu * prodErrOut @ np.conj(inAdaptPar)
         )  # gradient descent update
-    return H, np.abs(err) ** 2
+        if runWL:
+            H_[indUpdTaps, :] += (
+            mu * prodErrOut @ inAdaptPar
+            )  # gradient descent update
+    return H, H_, np.abs(err) ** 2
 
 
 @njit
-def rdeUp(x, R, outEq, mu, H, nModes):
+def rdeUp(x, R, outEq, mu, H, H_, nModes, runWL):
     """
     Coefficient update with the RDE algorithm.
 
     Parameters
     ----------
-    x : array-like
+    x : np.array
         Input array.
-    R : array-like
+    R : np.array
         Constellation radius array.
-    outEq : array-like
+    outEq : np.array
         Equalized output array.
     mu : float
         Step size parameter.
-    H : array-like
+    H : np.array
         Coefficient matrix.
+    H_ : np.array
+        Augmented coefficient matrix.
     nModes : int
         Number of modes.
+    runWL: bool
+        Run widely-linear mode.
 
     Returns
     -------
-    H : array-like
+    H : np.array
         Updated coefficient matrix.
-    err_sq : array-like
+    H_ : np.array
+        Updated augmented coefficient matrix.
+    err_sq : np.array
         Squared absolute error.
 
     """
     indMode = np.arange(0, nModes)
     outEq = outEq.T
     decidedR = np.zeros(outEq.shape, dtype=np.complex128)
 
@@ -693,42 +769,53 @@
         inAdapt = x[:, N].T
         inAdaptPar = (
             inAdapt.repeat(nModes).reshape(len(x), -1).T
         )  # expand input to parallelize tap adaptation
         H[indUpdTaps, :] += (
             mu * prodErrOut @ np.conj(inAdaptPar)
         )  # gradient descent update
-    return H, np.abs(err) ** 2
+        if runWL:
+            H_[indUpdTaps, :] += (
+            mu * prodErrOut @ inAdaptPar
+            )  # gradient descent update
+
+    return H, H_, np.abs(err) ** 2
 
 
 @njit
-def dardeUp(x, dx, outEq, mu, H, nModes):
+def dardeUp(x, dx, outEq, mu, H, H_, nModes, runWL):
     """
     Coefficient update with the data-aided RDE algorithm.
 
     Parameters
     ----------
-    x : array-like
+    x : np.array
         Input array.
-    dx : array-like
+    dx : np.array
         Exact constellation radius array.
-    outEq : array-like
+    outEq : np.array
         Equalized output array.
     mu : float
         Step size parameter.
-    H : array-like
+    H : np.array
         Coefficient matrix.
+    H_ : np.array
+        Augmented coefficient matrix.
     nModes : int
         Number of modes.
+    runWL: bool
+        Run widely-linear mode.
 
     Returns
     -------
-    H : array-like
+    H : np.array
         Updated coefficient matrix.
-    err_sq : array-like
+    H_ : np.array
+        Updated augmented coefficient matrix.
+    err_sq : np.array
         Squared absolute error.
 
     """
     indMode = np.arange(0, nModes)
     outEq = outEq.T
     decidedR = np.zeros(outEq.shape, dtype=np.complex128)
 
@@ -747,15 +834,19 @@
         inAdapt = x[:, N].T
         inAdaptPar = (
             inAdapt.repeat(nModes).reshape(len(x), -1).T
         )  # expand input to parallelize tap adaptation
         H[indUpdTaps, :] += (
             mu * prodErrOut @ np.conj(inAdaptPar)
         )  # gradient descent update
-    return H, np.abs(err) ** 2
+        if runWL:
+            H_[indUpdTaps, :] += (
+            mu * prodErrOut @ inAdaptPar
+            )  # gradient descent update
+    return H, H_, np.abs(err) ** 2
 
 
 def dbp(Ei, Fs, Ltotal, Lspan, hz=0.5, alpha=0.2, gamma=1.3, D=16, Fc=193.1e12):
     """
     Digital backpropagation (symmetric, single-pol.)
 
     :param Ei: input signal
```

### Comparing `OptiCommPy-0.7.0/optic/models/amplification.py` & `OptiCommPy-0.9.0/optic/models/amplification.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import matplotlib.pyplot as plt
 import matplotlib.mlab as mlab
 
 from scipy import interpolate
 from numpy.fft import fft, ifft, fftfreq
 from scipy.integrate import solve_ivp
 
-import pandas as pd
+# import pandas as pd
 from scipy.signal import find_peaks
 from scipy.constants import lambda2nu
 from scipy import signal
 from scipy.constants import c, Planck
 
 from scipy.constants import c, Planck
 from scipy.special import jv, kv
```

### Comparing `OptiCommPy-0.7.0/optic/models/channels.py` & `OptiCommPy-0.9.0/optic/models/channels.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,14 +50,20 @@
         - param.returnParameters: bool, return channel parameters [default: False]
 
     Returns
     -------
     Eo : np.array
         Optical field at the output of the fiber.
 
+    References
+    ----------
+    [1] G. P. Agrawal, Fiber-Optic Communication Systems. Wiley, 2021.
+
+    [2] S. J. Savory, “Digital coherent optical receivers: Algorithms and subsystems”, IEEE Journal on Selected Topics in Quantum Electronics, vol. 16, nº 5, p. 1164–1179, set. 2010, doi: 10.1109/JSTQE.2010.2044751.
+
     """
     try:
         Fs = param.Fs
     except AttributeError:
         logg.error("Simulation sampling frequency (Fs) not provided.")
 
     # check input parameters
@@ -96,18 +102,15 @@
     )
 
     if Nmodes == 1:
         Eo = Eo.reshape(
             Eo.size,
         )
 
-    if returnParameters:
-        return Eo, param
-    else:
-        return Eo
+    return (Eo, param) if returnParameters else Eo
 
 
 def ssfm(Ei, param=None):
     """
     Split-step Fourier method (symmetric, single-pol.).
 
     Parameters
@@ -147,14 +150,20 @@
 
     Returns
     -------
     Ech : np.array
         Optical signal after nonlinear propagation.
     param : parameter object  (struct)
         Object with physical/simulation parameters used in the split-step alg.
+  
+    References
+    ----------
+    [1] G. P. Agrawal, Nonlinear Fiber Optics, Elsevier Science, 2013. 
+
+    [2] O. V. Sinkin, R. Holzlöhner, J. Zweck, e C. R. Menyuk, “Optimization of the split-step Fourier method in modeling optical-fiber communications systems”, Journal of Lightwave Technology, vol. 21, nº 1, p. 61–68, jan. 2003, doi: 10.1109/JLT.2003.808628.
 
     """
     try:
         Fs = param.Fs
     except AttributeError:
         logg.error("Simulation sampling frequency (Fs) not provided.")
 
@@ -234,23 +243,24 @@
         if amp == "edfa":
             Ech = edfa(Ech, paramAmp)
         elif amp == "ideal":
             Ech = Ech * np.exp(α / 2 * Nsteps * hz)
         elif amp is None:
             Ech = Ech * np.exp(0)
 
-    if returnParameters:
-        return (
+    return (
+        (
             Ech.reshape(
                 len(Ech),
             ),
             param,
         )
-    else:
-        return Ech
+        if returnParameters
+        else Ech
+    )
 
 
 def manakovSSF(Ei, param):
     """
     Run the Manakov split-step Fourier model (symmetric, dual-pol.).
 
     Parameters
@@ -301,14 +311,22 @@
     Returns
     -------
     Ech : np.array
         Optical signal after nonlinear propagation.
     param : parameter object  (struct)
         Object with physical/simulation parameters used in the split-step alg.
 
+    References
+    ----------
+    [1] D. Marcuse, C. R. Menyuk, e P. K. A. Wai, “Application of the Manakov-PMD equation to studies of signal propagation in optical fibers with randomly varying birefringence”, Journal of Lightwave Technology, vol. 15, nº 9, p. 1735–1745, 1997, doi: 10.1109/50.622902.
+
+    [2] P. Serena, C. Lasagni, S. Musetti, e A. Bononi, “On Numerical Simulations of Ultra-Wideband Long-Haul Optical Communication Systems”, Journal of Lightwave Technology, vol. 38, nº 5, p. 1019–1031, 2020, doi: 10.1109/JLT.2019.2938580.
+
+    [3] O. V. Sinkin, R. Holzlöhner, J. Zweck, e C. R. Menyuk, “Optimization of the split-step Fourier method in modeling optical-fiber communications systems”, Journal of Lightwave Technology, vol. 21, nº 1, p. 61–68, jan. 2003, doi: 10.1109/JLT.2003.808628.
+
     """
     try:
         Fs = param.Fs
     except AttributeError:
         logg.error("Simulation sampling frequency (Fs) not provided.")
 
     # check input parameters
@@ -379,14 +397,15 @@
     else:
         argLimOp = argLimOp.reshape(1, -1)
 
     if saveSpanN:
         Ech_spans = np.zeros((Ei.shape[0], Ei.shape[1] * len(saveSpanN))).astype(prec)
         indRecSpan = 0
 
+    logg.info(f"Running Manakov SSF model on CPU...")
     for spanN in tqdm(range(1, Nspans + 1), disable=not (prgsBar)):
         Ex_conv = Ech_x.copy()
         Ey_conv = Ech_y.copy()
 
         z_current = 0
 
         # fiber propagation steps
@@ -542,14 +561,18 @@
         Generate complex-valued noise. The default is True.
 
     Returns
     -------
     np.array
         Input signal plus noise.
 
+    References
+    ----------
+    [1] P. Massoud Salehi e J. Proakis, Digital Communications. McGraw-Hill Education, 2007.
+
     """
     snr_lin = 10 ** (snr / 10)
     noiseVar = sigPow(sig) / snr_lin
     σ2 = (Fs / B) * noiseVar
 
     if complexNoise:
         noise = gaussianComplexNoise(sig.shape, σ2)
```

### Comparing `OptiCommPy-0.7.0/optic/models/devices.py` & `OptiCommPy-0.9.0/optic/models/devices.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,14 +54,18 @@
     Vπ : scalar
         PM's Vπ voltage.
     Returns
     -------
     Ao : np.array
         Modulated optical field at the output of the PM.
 
+    References
+    ----------
+    [1] G. P. Agrawal, Fiber-Optic Communication Systems. Wiley, 2021.
+
     """
     try:
         u.shape
     except AttributeError:
         u = np.array([u])
 
     try:
@@ -94,14 +98,20 @@
         - param.Vb: MZM's bias voltage [V][default: -1 V]
 
     Returns
     -------
     Ao : np.array
         Modulated optical field at the output of the MZM.
 
+    References
+    ----------
+    [1] G. P. Agrawal, Fiber-Optic Communication Systems. Wiley, 2021.
+    
+    [2] M. Seimetz, High-Order Modulation for Optical Fiber Transmission. em Springer Series in Optical Sciences. Springer Berlin Heidelberg, 2009.
+
     """
     if param is None:
         param = []
 
     # check input parameters
     Vpi = getattr(param, "Vpi", 2)
     Vb = getattr(param, "Vb", -1)
@@ -145,14 +155,18 @@
         - param.Vphi: PM bias voltage [V][default: 1 V]
 
     Returns
     -------
     Ao : complex-valued np.array
         Modulated optical field at the output of the IQM.
 
+    References
+    ----------
+    [1] M. Seimetz, High-Order Modulation for Optical Fiber Transmission. em Springer Series in Optical Sciences. Springer Berlin Heidelberg, 2009.
+
     """
     if param is None:
         param = []
 
     # check input parameters
     Vpi = getattr(param, "Vpi", 2)
     VbI = getattr(param, "VbI", -2)
@@ -201,14 +215,18 @@
     Returns
     -------
     Ex : (N,) np.array
         Ex output single pol. field.
     Ey : (N,) np.array
         Ey output single pol. field.
 
+    References
+    ----------
+    [1] M. Seimetz, High-Order Modulation for Optical Fiber Transmission. em Springer Series in Optical Sciences. Springer Berlin Heidelberg, 2009.
+
     """
     try:
         assert E.shape[1] == 2, "E need to be a (N,2) or a (N,) np.array"
     except IndexError:
         E = np.repeat(E, 2).reshape(-1, 2)
         E[:, 1] = 0
 
@@ -254,14 +272,18 @@
         - param.ideal: ideal PD?(i.e. no noise, no frequency resp.) [default: True]
 
     Returns
     -------
     ipd : np.array
           photocurrent.
 
+    References
+    ----------
+    [1] G. P. Agrawal, Fiber-Optic Communication Systems. Wiley, 2021.
+
     """
     if param is None:
         param = []
     kB = const.value("Boltzmann constant")
     q = const.value("elementary charge")
 
     # check input parameters
@@ -335,14 +357,19 @@
         - param.ideal: ideal PD?(i.e. no noise, no frequency resp.) [default: True]
 
     Returns
     -------
     ibpd : np.array
            Balanced photocurrent.
 
+    References
+    ----------
+    [1] M. Seimetz, High-Order Modulation for Optical Fiber Transmission. em Springer Series in Optical Sciences. Springer Berlin Heidelberg, 2009.
+    
+    [2] K. Kikuchi, “Fundamentals of Coherent Optical Fiber Communications”, J. Lightwave Technol., JLT, vol. 34, nº 1, p. 157–179, jan. 2016.
     """
     assert E1.shape == E2.shape, "E1 and E2 need to have the same shape"
 
     i1 = photodiode(E1, param)
     i2 = photodiode(E2, param)
     return i1 - i2
 
@@ -359,14 +386,19 @@
         Input LO optical field.
 
     Returns
     -------
     Eo : np.array
         Optical hybrid outputs.
 
+    References
+    ----------
+    [1] M. Seimetz, High-Order Modulation for Optical Fiber Transmission. em Springer Series in Optical Sciences. Springer Berlin Heidelberg, 2009.
+
+    [2] K. Kikuchi, “Fundamentals of Coherent Optical Fiber Communications”, J. Lightwave Technol., JLT, vol. 34, nº 1, p. 157–179, jan. 2016.
     """
     assert Es.shape == (len(Es),), "Es need to have a (N,) shape"
     assert Elo.shape == (len(Elo),), "Elo need to have a (N,) shape"
     assert Es.shape == Elo.shape, "Es and Elo need to have the same (N,) shape"
 
     # optical hybrid transfer matrix
     T = np.array(
@@ -397,14 +429,19 @@
         Parameters of the photodiodes.
 
     Returns
     -------
     s : np.array
         Downconverted signal after balanced detection.
 
+    References
+    ----------
+    [1] M. Seimetz, High-Order Modulation for Optical Fiber Transmission. em Springer Series in Optical Sciences. Springer Berlin Heidelberg, 2009.
+
+    [2] K. Kikuchi, “Fundamentals of Coherent Optical Fiber Communications”, J. Lightwave Technol., JLT, vol. 34, nº 1, p. 157–179, jan. 2016.
     """
     assert Es.shape == (len(Es),), "Es need to have a (N,) shape"
     assert Elo.shape == (len(Elo),), "Elo need to have a (N,) shape"
     assert Es.shape == Elo.shape, "Es and Elo need to have the same (N,) shape"
 
     # optical 2 x 4 90° hybrid
     Eo = hybrid_2x4_90deg(Es, Elo)
@@ -432,14 +469,19 @@
         Parameters of the photodiodes.
 
     Returns
     -------
     S : np.array
         Downconverted signal after balanced detection.
 
+    References
+    ----------
+    [1] M. Seimetz, High-Order Modulation for Optical Fiber Transmission. em Springer Series in Optical Sciences. Springer Berlin Heidelberg, 2009.
+
+    [2] K. Kikuchi, “Fundamentals of Coherent Optical Fiber Communications”, J. Lightwave Technol., JLT, vol. 34, nº 1, p. 157–179, jan. 2016.
     """
     assert len(Es) == len(Elo), "Es and Elo need to have the same length"
 
     Elox, Eloy = pbs(Elo, θ=np.pi / 4)  # split LO into two orth. polarizations
     Esx, Esy = pbs(Es, θ=θsig)  # split signal into two orth. polarizations
 
     Sx = coherentReceiver(Esx, Elox, param)  # coherent detection of pol.X
@@ -465,14 +507,18 @@
         - param.Fs : sampling frequency in samples/second.
 
     Returns
     -------
     Eo : np.array
         Amplified noisy optical signal.
 
+    References
+    ----------
+    [1] R. -J. Essiambre,et al, "Capacity Limits of Optical Fiber Networks," in Journal of Lightwave Technology, vol. 28, no. 4, pp. 662-701, 2010, doi: 10.1109/JLT.2009.2039464.
+
     """
     try:
         Fs = param.Fs
     except AttributeError:
         logg.error("Simulation sampling frequency (Fs) not provided.")
 
     # check input parameters
@@ -516,14 +562,18 @@
         - param.Ns: number of signal samples [default: 1e3]
 
     Returns
     -------
     optical_signal : np.array
           Optical signal with phase noise and RIN.
 
+    References
+    ----------
+    [1] M. Seimetz, High-Order Modulation for Optical Fiber Transmission. em Springer Series in Optical Sciences. Springer Berlin Heidelberg, 2009.
+
     """
     try:
         Fs = param.Fs
     except AttributeError:
         logg.error("Simulation sampling frequency (Fs) not provided.")
 
     P = getattr(param, "P", 10)  # Laser power in dBm
@@ -536,15 +586,15 @@
     # Simulate Maxwellian random walk phase noise
     pn = phaseNoise(lw, Ns, 1 / Fs)
 
     # Simulate relative intensity noise  (RIN)[todo:check correct model]
     deltaP = gaussianComplexNoise(pn.shape, RIN_var)
 
     # Return optical signal
-    return np.sqrt(dBm2W(P)) * np.exp(1j * pn) + deltaP
+    return np.sqrt(dBm2W(P) + deltaP) * np.exp(1j * pn) 
 
 
 def adc(Ei, param):
     """
     Analog-to-digital converter (ADC) model.
 
     Parameters
```

### Comparing `OptiCommPy-0.7.0/optic/models/modelsGPU.py` & `OptiCommPy-0.9.0/optic/models/modelsGPU.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,21 +29,21 @@
 def gaussianComplexNoise(shapeOut, σ2=1.0):
     """
     Generate complex circular Gaussian noise.
 
     Parameters
     ----------
     shapeOut : tuple of int
-        Shape of ndarray to be generated.
+        Shape of np.array to be generated.
     σ2 : float, optional
         Variance of the noise (default is 1).
 
     Returns
     -------
-    noise : ndarray
+    noise : np.array
         Generated complex circular Gaussian noise.
     """
     return normal(0, np.sqrt(σ2 / 2), shapeOut) + 1j * normal(
         0, np.sqrt(σ2 / 2), shapeOut
     )
 
 
@@ -64,14 +64,18 @@
         - param.Fs : sampling frequency in samples/second.
 
     Returns
     -------
     Eo : np.array
         Amplified noisy optical signal.
 
+    References
+    ----------
+    [1] R. -J. Essiambre,et al, "Capacity Limits of Optical Fiber Networks," in Journal of Lightwave Technology, vol. 28, no. 4, pp. 662-701, 2010, doi: 10.1109/JLT.2009.2039464.
+
     """
     try:
         Fs = param.Fs
     except AttributeError:
         logg.error("Simulation sampling frequency (Fs) not provided.")
 
     # check input parameters
@@ -141,14 +145,21 @@
     Returns
     -------
     Ech : np.array
         Optical signal after nonlinear propagation.
     param : parameter object  (struct)
         Object with physical/simulation parameters used in the split-step alg.
 
+    References
+    ----------
+    [1] G. P. Agrawal, Nonlinear Fiber Optics, Elsevier Science, 2013. 
+
+    [2] O. V. Sinkin, R. Holzlöhner, J. Zweck, e C. R. Menyuk, “Optimization of the split-step Fourier method in modeling optical-fiber communications systems”, Journal of Lightwave Technology, vol. 21, nº 1, p. 61–68, jan. 2003, doi: 10.1109/JLT.2003.808628.
+
+
     """
     try:
         Fs = param.Fs
     except AttributeError:
         logg.error("Simulation sampling frequency (Fs) not provided.")
 
     # check input parameters
@@ -256,18 +267,15 @@
     Ech = cp.asnumpy(Ech_spans)
 
     if Ech.shape[1] == 1:
         Ech = Ech.reshape(
             len(Ech),
         )
 
-    if returnParameters:
-        return Ech, param
-    else:
-        return Ech
+    return (Ech, param) if returnParameters else Ech
 
 
 def manakovSSF(Ei, param):
     """
     Run the Manakov split-step Fourier model (symmetric, dual-pol.).
 
     Parameters
@@ -317,14 +325,22 @@
     Returns
     -------
     Ech : np.array
         Optical signal after nonlinear propagation.
     param : parameter object  (struct)
         Object with physical/simulation parameters used in the split-step alg.
 
+    References
+    ----------
+    [1] D. Marcuse, C. R. Menyuk, e P. K. A. Wai, “Application of the Manakov-PMD equation to studies of signal propagation in optical fibers with randomly varying birefringence”, Journal of Lightwave Technology, vol. 15, nº 9, p. 1735–1745, 1997, doi: 10.1109/50.622902.
+
+    [2] P. Serena, C. Lasagni, S. Musetti, e A. Bononi, “On Numerical Simulations of Ultra-Wideband Long-Haul Optical Communication Systems”, Journal of Lightwave Technology, vol. 38, nº 5, p. 1019–1031, 2020, doi: 10.1109/JLT.2019.2938580.
+
+    [3] O. V. Sinkin, R. Holzlöhner, J. Zweck, e C. R. Menyuk, “Optimization of the split-step Fourier method in modeling optical-fiber communications systems”, Journal of Lightwave Technology, vol. 21, nº 1, p. 61–68, jan. 2003, doi: 10.1109/JLT.2003.808628.
+
     """
     try:
         Fs = param.Fs
     except AttributeError:
         logg.error("Simulation sampling frequency (Fs) not provided.")
 
     # check input parameters
@@ -407,14 +423,15 @@
     else:
         argLimOp = argLimOp.reshape(1, -1)
 
     if saveSpanN:
         Ech_spans = cp.zeros((Ei_.shape[0], Ei_.shape[1] * len(saveSpanN))).astype(prec)
         indRecSpan = 0
 
+    logg.info(f"Running Manakov SSF model on GPU...")
     for spanN in tqdm(range(1, Nspans + 1), disable=not (prgsBar)):
         Ex_conv = Ech_x.copy()
         Ey_conv = Ech_y.copy()
         z_current = 0
 
         # fiber propagation steps
         while z_current < Lspan:
@@ -494,18 +511,15 @@
         Ech_x = cp.asnumpy(Ech_x)
         Ech_y = cp.asnumpy(Ech_y)
 
         Ech = Ei.copy()
         Ech[:, 0::2] = Ech_x.T
         Ech[:, 1::2] = Ech_y.T
 
-    if returnParameters:
-        return Ech, param
-    else:
-        return Ech
+    return (Ech, param) if returnParameters else Ech
 
 
 def nlinPhaseRot(Ex, Ey, Pch, γ):
     """
     Calculate nonlinear phase-shift per step for the Manakov SSFM.
 
     Parameters
@@ -602,14 +616,20 @@
 
     Returns
     -------
     Ech : np.array
         Optical signal after nonlinear backward propagation.
     param : parameter object  (struct)
         Object with physical/simulation parameters used in the split-step alg.
+    
+    References
+    ----------
+    [1] E. Ip e J. M. Kahn, “Compensation of dispersion and nonlinear impairments using digital backpropagation”, Journal of Lightwave Technology, vol. 26, nº 20, p. 3416–3425, 2008, doi: 10.1109/JLT.2008.927791.
+
+    [2] E. Ip, “Nonlinear compensation using backpropagation for polarization-multiplexed transmission”, Journal of Lightwave Technology, vol. 28, nº 6, p. 939–951, mar. 2010, doi: 10.1109/JLT.2010.2040135.
 
     """
     try:
         Fs = param.Fs
     except AttributeError:
         logg.error("Simulation sampling frequency (Fs) not provided.")
 
@@ -768,18 +788,15 @@
         Ech_x = cp.asnumpy(Ech_x)
         Ech_y = cp.asnumpy(Ech_y)
 
         Ech = Ei.copy()
         Ech[:, 0::2] = Ech_x.T
         Ech[:, 1::2] = Ech_y.T
 
-    if returnParameters:
-        return Ech, param
-    else:
-        return Ech
+    return (Ech, param) if returnParameters else Ech
 
 
 def setPowerforParSSFM(sig, powers):
     powers_lin = 10 ** (powers / 10) * 1e-3
     powers_lin = powers_lin.repeat(2) / 2
 
     for i in np.arange(0, sig.shape[1], 2):
```

### Comparing `OptiCommPy-0.7.0/optic/models/tx.py` & `OptiCommPy-0.9.0/optic/models/tx.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """
 
 import numpy as np
 from tqdm.notebook import tqdm
 
 from optic.dsp.core import pnorm, pulseShape, signal_power, upsample, phaseNoise
 from optic.models.devices import iqm
-from optic.comm.modulation import GrayMapping, modulateGray
+from optic.comm.modulation import grayMapping, modulateGray
 
 try:
     from optic.dsp.coreGPU import firFilter
 except ImportError:
     from optic.dsp.core import firFilter
 
 import logging as logg
@@ -124,15 +124,15 @@
     symbTxWDM = np.zeros(
         (len(t) // param.SpS, param.Nmodes, param.Nch), dtype="complex"
     )
 
     Psig = 0
 
     # constellation symbols info
-    const = GrayMapping(param.M, param.constType)
+    const = grayMapping(param.M, param.constType)
     Es = np.mean(np.abs(const) ** 2)
 
     # pulse shaping filter
     if param.pulse == "nrz":
         pulse = pulseShape("nrz", param.SpS)
     elif param.pulse == "rrc":
         pulse = pulseShape("rrc", param.SpS, N=param.Ntaps, alpha=param.alphaRRC, Ts=Ts)
```

### Comparing `OptiCommPy-0.7.0/optic/utils.py` & `OptiCommPy-0.9.0/optic/utils.py`

 * *Files identical despite different names*

### Comparing `OptiCommPy-0.7.0/setup.py` & `OptiCommPy-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Authors: OpticCommPy contributors
-# License: BSD 3-Clause
+# License: GPL-3.0 license
 
 from setuptools import setup
 
 # Taken from scikit-commpy setup.py
 DISTNAME = "OptiCommPy"
 DESCRIPTION = "Optical Communications Algorithms with Python"
-LONG_DESCRIPTION = open("README.md", encoding="utf8").read()
+LONG_DESCRIPTION = open("README.rst", encoding="utf8").read()
 MAINTAINER = "Edson Porto da Silva"
 MAINTAINER_EMAIL = "edsonporto88@gmail.com"
 URL = "https://github.com/edsonportosilva/OptiCommPy"
-LICENSE = "BSD 3-Clause"
-VERSION = "0.7.0"
+LICENSE = "GPL-3.0 license"
+VERSION = "0.9.0"
 
 # This is a list of files to install, and where
 # (relative to the 'root' dir, where setup.py is)
 # You could be more specific.
 files = ["optic/*", "optic/comm/*", "optic/dsp/*", "optic/models/*"]
 
 setup(
@@ -29,34 +29,34 @@
     # Name the folder where your packages live:
     # (If you have other packages (dirs) or modules (py files) then
     # put them into the package directory - they will be found
     # recursively.)
     packages=["optic", "optic.comm", "optic.models", "optic.dsp"],
     # py_modules = ['plot', 'core', 'comm', 'dsp', 'models'],
     install_requires=[
-        "numpy>=1.9.2",
-        "scipy>=0.15.0",
+        "numpy>=1.24.4",
+        "scipy>=1.13.0",
         "matplotlib>=3.7.0",
         "sympy",
         "tqdm>=4.64.1",
-        "numba>=0.54.1",
-        "scikit-commpy>=0.7.0",
+        "numba>=0.54.0,<=0.57",
         "simple-pid>=1.0.1",
         "mpl-scatter-density>=0.7.0",
-        "pandas>=2.0.0",
         "sphinx-rtd-theme>=1.2.2",
+        "nbsphinx>=0.9.3",
+        "nbsphinx-link>=1.3.0"
     ],
     #'package' package must contain files (see list above)
     # This dict maps the package name =to=> directories
     # It says, package *needs* these files.
     package_data={"optic": files},
     #'runner' is in the root.
     scripts=["runner"],
-    test_suite="nose.collector",
-    tests_require=["nose"],
+    test_suite="tests",
+    tests_require=["pytest", "unittest"],
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Telecommunications Industry",
         "Operating System :: Unix",
```

