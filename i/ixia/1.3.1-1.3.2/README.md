# Comparing `tmp/ixia-1.3.1.tar.gz` & `tmp/ixia-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixia-1.3.1.tar", max compression
+gzip compressed data, was "ixia-1.3.2.tar", max compression
```

## Comparing `ixia-1.3.1.tar` & `ixia-1.3.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1056 2023-01-19 17:08:28.542416 ixia-1.3.1/LICENSE
--rw-r--r--   0        0        0     1515 2023-04-04 21:41:05.065273 ixia-1.3.1/README.md
--rw-r--r--   0        0        0     1049 2023-10-02 07:49:32.774550 ixia-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1142 2023-10-02 07:48:55.430637 ixia-1.3.1/src/ixia/__init__.py
--rw-r--r--   0        0        0     1941 2023-07-13 19:40:26.601614 ixia-1.3.1/src/ixia/date_time.py
--rw-r--r--   0        0        0     9016 2023-08-13 20:06:59.206328 ixia-1.3.1/src/ixia/distributions.py
--rw-r--r--   0        0        0     2581 2023-07-14 17:23:43.182836 ixia-1.3.1/src/ixia/integers.py
--rw-r--r--   0        0        0     5454 2023-07-14 17:19:42.230984 ixia-1.3.1/src/ixia/sequences.py
--rw-r--r--   0        0        0     1785 2023-08-13 14:54:04.883838 ixia-1.3.1/src/ixia/strings.py
--rw-r--r--   0        0        0     2227 1970-01-01 00:00:00.000000 ixia-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-06-03 12:08:50.855591 ixia-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1515 2024-05-28 16:15:16.153977 ixia-1.3.2/README.md
+-rw-r--r--   0        0        0     1188 2024-05-28 15:58:54.104411 ixia-1.3.2/ixia/__init__.py
+-rw-r--r--   0        0        0     2200 2024-05-28 15:58:54.104553 ixia-1.3.2/ixia/date_time.py
+-rw-r--r--   0        0        0     9159 2024-05-28 16:15:16.154489 ixia-1.3.2/ixia/distributions.py
+-rw-r--r--   0        0        0     2693 2024-05-28 15:58:54.104871 ixia-1.3.2/ixia/integers.py
+-rw-r--r--   0        0        0        0 2024-05-28 16:22:15.383661 ixia-1.3.2/ixia/py.typed
+-rw-r--r--   0        0        0     5626 2024-05-28 16:15:16.154825 ixia-1.3.2/ixia/sequences.py
+-rw-r--r--   0        0        0     1786 2024-05-28 15:58:54.105347 ixia-1.3.2/ixia/strings.py
+-rw-r--r--   0        0        0     1247 2024-06-03 12:09:03.244853 ixia-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2268 1970-01-01 00:00:00.000000 ixia-1.3.2/PKG-INFO
```

### Comparing `ixia-1.3.1/LICENSE` & `ixia-1.3.2/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022–2023 trag1c
+Copyright (c) 2022–2024 trag1c
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ixia-1.3.1/README.md` & `ixia-1.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ## Documentation
 Ixia documentation is available at https://trag1c.github.io/ixia/.
 
 ## License
 Ixia is licensed under the MIT License.
 
 ## ⚠️ Important Notes
-While supporting Python 3.8+, Ixia is based on the Python 3.11 implementation
+While supporting Python 3.8+, Ixia is based on the Python 3.12 implementation
 of the `random` module. The following changes have been made to the module
 since Python 3.8:
 - `getrandbits` accepts 0 for `k`
 - `choices` raises a `ValueError` if all weights are zero
 - `sample` has a new `counts` parameter
 - `gauss` and `normal_variate` have default parameter values
```

### Comparing `ixia-1.3.1/src/ixia/__init__.py` & `ixia-1.3.2/ixia/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .date_time import rand_date, rand_time
 from .distributions import (
     beta_variate,
+    binomial_variate,
     expo_variate,
     gamma_variate,
     gauss,
     log_norm_variate,
     normal_variate,
     pareto_variate,
     random,
@@ -23,14 +24,15 @@
     universe_rand,
 )
 from .sequences import choice, choices, sample, shuffle, shuffled
 from .strings import passphrase, rand_bytes, rand_hex, rand_line, rand_urlsafe
 
 __all__ = (
     "beta_variate",
+    "binomial_variate",
     "choice",
     "choices",
     "expo_variate",
     "gamma_variate",
     "gauss",
     "log_norm_variate",
     "normal_variate",
```

### Comparing `ixia-1.3.1/src/ixia/date_time.py` & `ixia-1.3.2/ixia/date_time.py`

 * *Files 24% similar despite different names*

```diff
@@ -47,25 +47,33 @@
         + time.second * 10**6
         + time.minute * 6 * 10**7
         + time.hour * 36 * 10**8
     )
 
 
 def rand_date(start: Datelike, end: Datelike | None = None) -> dt.date:
+    """
+    Returns a random date between start and end. If end is None, defaults to Dec 31.
+    """
     start = _convert_date(start)
     if end is None:
         end = dt.date(start.year, 12, 31)
     elif isinstance(end, int):
         end = dt.date(end, 12, 31)
     else:
         end = _convert_date(end)
     return start + dt.timedelta(days=rand_below((end - start).days + 1))
 
 
 def rand_time(start: Timelike | None = None, end: Timelike | None = None) -> dt.time:
+    """
+    Returns a random time between start and end.
+    If start is None, defaults to 00:00:00.
+    If end is None, defaults to 23:59:59.999999.
+    """
     start = dt.time.min if start is None else _convert_time(start)
     end = dt.time.max if end is None else _convert_time(end)
     out = rand_int(_microseconds(start), _microseconds(end))
     out, us = divmod(out, 1_000_000)
     out, s = divmod(out, 60)
     h, m = divmod(out, 60)
     return dt.time(h, m, s, us)
```

### Comparing `ixia-1.3.1/src/ixia/distributions.py` & `ixia-1.3.2/ixia/distributions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
 
 from math import acos, cos, e, exp, fabs, floor, lgamma, log, log2, pi, sin, sqrt, tau
 from operator import index
 from os import urandom
+from pathlib import Path
 from typing import ClassVar, Union
 
 Number = Union[int, float]
+PASSPHRASE_DEFAULT_PATH = Path("/usr/share/dict/words")
 
 
-class Cache:
+class _Cache:
     gauss_next: float | None = None
     words: ClassVar[list[str]] = []
-    words_path: str = "/usr/share/dict/words"
+    words_path: Path = Path("/usr/share/dict/words")
 
 
 def beta_variate(alpha: Number, beta: Number) -> float:
     """
     Beta distribution.
 
     Conditions on the parameters are alpha > 0 and beta > 0.
@@ -37,21 +39,23 @@
 
         sum(random() < p for _ in range(n))
 
     Returns an integer in the range [0, n]
     """
     # Error checking and edge cases
     if n < 0:
-        raise ValueError("n must be non-negative")
+        msg = "n must be non-negative"
+        raise ValueError(msg)
     if p == 0.0:
         return 0
     if p == 1.0:
         return n
     if not (0.0 < p < 1.0):
-        raise ValueError("p must be in range [0, 1]")
+        msg = "p must be in range [0, 1]"
+        raise ValueError(msg)
 
     # Fast path for a common case
     if n == 1:
         return index(random() < p)
 
     # Exploit symmetry to establish:  p <= 0.5
     if p > 0.5:
@@ -67,39 +71,37 @@
             y += floor(log2(random()) / c) + 1
             if y > n:
                 return x
             x += 1
 
     # BTRS: Transformed rejection with squeeze method by Wolfgang Hörmann
     # https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.47.8407
-    assert n*p >= 10.0 and p <= 0.5
     setup_complete = False
     alpha = m = h = lpq = 0.0
 
     spq = sqrt(n * p * (1.0 - p))  # Standard deviation of the distribution
     b = 1.15 + 2.53 * spq
     a = -0.0873 + 0.0248 * b + 0.01 * p
     c = n * p + 0.5
     vr = 0.92 - 4.2 / b
 
     while True:
-        u = random() - 0.5
         us = 0.5 - fabs(u := random() - 0.5)
         k = floor((2.0 * a / us + b) * u + c)
         if k < 0 or k > n:
             continue
 
         # The early-out "squeeze" test substantially reduces
         # the number of acceptance condition evaluations.
         v = random()
         if us >= 0.07 and v <= vr:
             return k
 
         # Acceptance-rejection test.
-        # Note, the original paper errorneously omits the call to log(v)
+        # Note, the original paper erroneously omits the call to log(v)
         # when comparing to the log of the rescaled binomial distribution.
         if not setup_complete:
             alpha = (2.83 + 5.1 / b) * spq
             lpq = log(p / (1.0 - p))
             m = floor((n + 1) * p)
             h = lgamma(m + 1) + lgamma(n - m + 1)
             setup_complete = True
@@ -124,18 +126,18 @@
 def gamma_variate(alpha: Number, beta: Number) -> float:
     """
     Gamma distribution.
 
     Conditions on the parameters are alpha > 0 and beta > 0.
     """
     if alpha <= 0.0 or beta <= 0.0:
-        raise ValueError("gamma_variate: alpha and beta must be > 0.0")
+        msg = "gamma_variate: alpha and beta must be > 0.0"
+        raise ValueError(msg)
 
     if alpha > 1.0:
-
         # Uses R.C.H. Cheng, "The generation of Gamma
         # variables with non-integral shape parameters",
         # Applied Statistics, (1977), 26, No. 1, p71-74
 
         ainv = sqrt(2.0 * alpha - 1.0)
         b = alpha - log(4)
         c = alpha + ainv
@@ -177,21 +179,21 @@
     Gaussian distribution.
 
     mu is the mean, and sigma is the standard deviation.
     This is slightly faster than the normal_variate() function.
 
     Not thread-safe without a lock around calls.
     """
-    z = Cache.gauss_next
-    Cache.gauss_next = None
+    z = _Cache.gauss_next
+    _Cache.gauss_next = None
     if z is None:
         xtau = random() * tau
         g2rad = sqrt(-2.0 * log(1.0 - random()))
         z = cos(xtau) * g2rad
-        Cache.gauss_next = sin(xtau) * g2rad
+        _Cache.gauss_next = sin(xtau) * g2rad
     return mu + z * sigma
 
 
 def log_norm_variate(mu: Number, sigma: Number) -> float:
     """
     Log normal distribution.
 
@@ -225,15 +227,15 @@
 def pareto_variate(alpha: Number) -> float:
     """
     Pareto distribution.
 
     alpha is the shape parameter.
     """
     # Jain, pg. 495
-    return (1.0 - random()) ** (-1.0 / alpha)
+    return (1.0 - random()) ** (-1.0 / alpha)  # type: ignore[no-any-return]
 
 
 def random() -> float:
     """Generates a random number in range [0.0, 1.0)."""
     return (int.from_bytes(urandom(7), "big") >> 3) * 2**-53
 
 
@@ -299,8 +301,8 @@
 def weibull_variate(alpha: Number, beta: Number) -> float:
     """
     Weibull distribution.
 
     alpha is the scale parameter, beta is the shape parameter.
     """
     # Jain, pg. 499; bug fix courtesy Bill Arms
-    return alpha * (-log(1.0 - random())) ** (1.0 / beta)
+    return alpha * (-log(1.0 - random())) ** (1.0 / beta)  # type: ignore[no-any-return]
```

### Comparing `ixia-1.3.1/src/ixia/integers.py` & `ixia-1.3.2/ixia/integers.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     """Returns a random int in the range [0, n)."""
     return secrets.randbelow(n)
 
 
 def rand_bits(k: int) -> int:
     """Generates an int with k random bits."""
     if k < 0:
-        raise ValueError("number of bits must be non-negative")
+        msg = "number of bits must be non-negative"
+        raise ValueError(msg)
     numbytes = (k + 7) // 8
     x = int.from_bytes(urandom(numbytes), "big")
     return x >> (numbytes * 8 - k)
 
 
 def rand_bool() -> bool:
     """Returns a random bool."""
@@ -36,33 +37,38 @@
     return [rand_int(a, b) for _ in range(k)]
 
 
 def rand_range(start: int, stop: int | None = None, step: int = 1) -> int:
     """Chooses a random item from range([start,] stop[, step])."""
     if stop is None:
         if step != 1:
-            raise TypeError("Missing a non-None stop argument")
+            msg = "Missing a non-None stop argument"
+            raise TypeError(msg)
         if start > 0:
             return secrets.randbelow(start)
-        raise ValueError("empty range for rand_range")
+        msg = "empty range for rand_range"
+        raise ValueError(msg)
 
     width = stop - start
     if step == 1:
         if width > 0:
             return start + secrets.randbelow(width)
-        raise ValueError(f"empty range for rand_range ({start}, {stop}, {step})")
+        msg = f"empty range for rand_range ({start}, {stop}, {step})"
+        raise ValueError(msg)
 
     if step > 0:
         n = (width + step - 1) // step
     elif step < 0:
         n = (width + step + 1) // step
     else:
-        raise ValueError("zero step for rand_range")
+        msg = "zero step for rand_range"
+        raise ValueError(msg)
     if n <= 0:
-        raise ValueError("empty range for rand_range")
+        msg = "empty range for rand_range"
+        raise ValueError(msg)
     return start + step * secrets.randbelow(n)
 
 
 def universe_rand() -> int:
     """Generates a random number based on the universe."""
     bm = 0xFF  # bound max, 1 byte
     s = 0
```

### Comparing `ixia-1.3.1/src/ixia/sequences.py` & `ixia-1.3.2/ixia/sequences.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,16 @@
     """
     Chooses a random element from a non-empty sequence.
 
     If the relative weights or cumulative weights are not specified,
     the selections are made with equal probability.
     """
     if not seq:
-        raise IndexError("Cannot choose from an empty sequence")
+        msg = "Cannot choose from an empty sequence"
+        raise IndexError(msg)
     if weights is None and cumulative_weights is None:
         return secrets.choice(seq)
     return choices(seq, weights, cumulative_weights=cumulative_weights)[0]
 
 
 def choices(
     seq: Sequence[T],
@@ -44,36 +45,39 @@
     If the relative weights or cumulative weights are not specified,
     the selections are made with equal probability.
     """
     n = len(seq)
 
     if cumulative_weights is None:
         if weights is None:
-            n += 0.0  # convert to float for a small speed improvement
-            return [seq[floor(random() * n)] for _ in range(k)]
+            n_ = n + 0.0  # convert to float for a small speed improvement
+            return [seq[floor(random() * n_)] for _ in range(k)]
         try:
             cumulative_weights = list(accumulate(weights))
         except TypeError:
             if not isinstance(weights, int):
                 raise
-            raise TypeError(
-                f"The number of choices must be a keyword argument: k={weights}"
-            ) from None
+            msg = f"The number of choices must be a keyword argument: k={weights}"
+            raise TypeError(msg) from None
     elif weights is not None:
-        raise TypeError("Cannot specify both weights and cumulative weights")
+        msg = "Cannot specify both weights and cumulative weights"
+        raise TypeError(msg)
 
     if len(cumulative_weights) != n:
-        raise ValueError("The number of weights does not match the sequence")
+        msg = "The number of weights does not match the sequence"
+        raise ValueError(msg)
 
     total = cumulative_weights[-1] + 0.0  # convert to float
     if total <= 0.0:
-        raise ValueError("Total of weights must be greater than zero")
+        msg = "Total of weights must be greater than zero"
+        raise ValueError(msg)
 
     if not isfinite(total):
-        raise ValueError("Total of weights must be finite")
+        msg = "Total of weights must be finite"
+        raise ValueError(msg)
 
     hi = n - 1
     return [seq[bisect(cumulative_weights, random() * total, 0, hi)] for _ in range(k)]
 
 
 def sample(seq: Sequence[T], k: int, *, counts: Iterable[int] | None = None) -> list[T]:
     """
@@ -81,15 +85,15 @@
 
     Returns a new list containing elements from the sequence while leaving the original
     sequence unchanged. The resulting list is in selection order so that all sub-slices
     will also be valid random samples. This allows raffle winners (the sample) to be
     partitioned into grand prize and second place winners (the subslices).
 
     Members of the sequence don't need to be hashable nor unique. If the sequence
-    contains repeats, then each occurence is a possible selection in the sample.
+    contains repeats, then each occurrence is a possible selection in the sample.
 
     Repeated elements can be specified one at a time or with
     the optional counts parameter. For example:
 
         sample(["red", "blue"], counts=[4, 2], k=5)
 
     is equivalent to:
@@ -103,24 +107,28 @@
         sample(range(10_000_000), 60)
     """
     n = len(seq)
 
     if counts is not None:
         cum_counts = list(accumulate(counts))
         if len(cum_counts) != n:
-            raise ValueError("The number of counts does not match the sequence")
+            msg = "The number of counts does not match the sequence"
+            raise ValueError(msg)
         total = cum_counts.pop()
         if not isinstance(total, int):
-            raise TypeError("Counts must be integers")
+            msg = "Counts must be integers"
+            raise TypeError(msg)
         if total <= 0:
-            raise ValueError("Total of counts must be greater than zero")
+            msg = "Total of counts must be greater than zero"
+            raise ValueError(msg)
         selections = sample(range(total), k=k)
         return [seq[bisect(cum_counts, s)] for s in selections]
     if not 0 <= k <= n:
-        raise ValueError("Sample larger than sequence or is negative")
+        msg = "Sample larger than sequence or is negative"
+        raise ValueError(msg)
 
     result: list[T] = []
     setsize = 21  # size of a small set minus size of an empty list
     if k > 5:
         setsize += 4 ** ceil(log(k * 3, 4))
 
     if n <= setsize:
```

### Comparing `ixia-1.3.1/src/ixia/strings.py` & `ixia-1.3.2/ixia/strings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from __future__ import annotations
 
 import secrets
 from base64 import urlsafe_b64encode
 from io import TextIOBase
-from os import urandom
+from os import PathLike, urandom
 from pathlib import Path
-from sys import platform
 
-from .distributions import Cache
+from .distributions import PASSPHRASE_DEFAULT_PATH, _Cache
 from .sequences import choice, choices
 
-PASSPHRASE_DEFAULT_PATH = "/usr/share/dict/words"
-PASSPHRASE_PLATFORMS = {"linux", "darwin", "aix"}
-
 
 def passphrase(
-    n: int, *, sep: str = "-", words_path: str = PASSPHRASE_DEFAULT_PATH
+    n: int, *, sep: str = "-", words_path: PathLike[str] | str = PASSPHRASE_DEFAULT_PATH
 ) -> str:
     """Generates an XKCD-style passphrase."""
-    if words_path == PASSPHRASE_DEFAULT_PATH and platform not in PASSPHRASE_PLATFORMS:
-        raise NotImplementedError(f"word list unavailable on {platform}")
-    if not Cache.words or Cache.words_path != words_path:
-        Cache.words = Path(words_path).read_text().splitlines()
-        Cache.words_path = words_path
-    return sep.join(choices(Cache.words, k=n)).lower()
+    words_path = Path(words_path)
+    if words_path == PASSPHRASE_DEFAULT_PATH and not words_path.exists():
+        msg = "word list unavailable at the default path; please provide a valid path"
+        raise NotImplementedError(msg)
+    if not (_Cache.words and _Cache.words_path == words_path):
+        _Cache.words = words_path.read_text().splitlines()
+        _Cache.words_path = words_path
+    return sep.join(choices(_Cache.words, k=n)).lower()
 
 
 def rand_bytes(n: int = 32) -> bytes:
     """Generates n random bytes. Defaults to 32."""
     return urandom(n)
```

### Comparing `ixia-1.3.1/PKG-INFO` & `ixia-1.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ixia
-Version: 1.3.1
-Summary: A library connecting secrets' security with random's versatility
+Version: 1.3.2
+Summary: Connecting secrets' security with random's versatility
 Home-page: https://github.com/trag1c/ixia
 License: MIT
 Author: trag1c
 Author-email: trag1cdev@yahoo.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Documentation, https://trag1c.github.io/ixia/
 Project-URL: Repository, https://github.com/trag1c/ixia
 Description-Content-Type: text/markdown
 
 # Ixia
 Ixia is a cryptographically secure RNG library. It mainly merges `secrets`'
 security with `random`'s versatility, but also adds some of its own
@@ -35,15 +36,15 @@
 ## Documentation
 Ixia documentation is available at https://trag1c.github.io/ixia/.
 
 ## License
 Ixia is licensed under the MIT License.
 
 ## ⚠️ Important Notes
-While supporting Python 3.8+, Ixia is based on the Python 3.11 implementation
+While supporting Python 3.8+, Ixia is based on the Python 3.12 implementation
 of the `random` module. The following changes have been made to the module
 since Python 3.8:
 - `getrandbits` accepts 0 for `k`
 - `choices` raises a `ValueError` if all weights are zero
 - `sample` has a new `counts` parameter
 - `gauss` and `normal_variate` have default parameter values
```

