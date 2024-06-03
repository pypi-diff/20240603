# Comparing `tmp/timeit_compare-1.2.2.tar.gz` & `tmp/timeit_compare-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeit_compare-1.2.2.tar", last modified: Thu May  9 16:03:17 2024, max compression
+gzip compressed data, was "timeit_compare-1.3.0.tar", last modified: Mon Jun  3 14:14:42 2024, max compression
```

## Comparing `timeit_compare-1.2.2.tar` & `timeit_compare-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 16:03:17.446076 timeit_compare-1.2.2/
--rw-rw-rw-   0        0        0     1089 2024-04-13 14:44:22.000000 timeit_compare-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     3916 2024-05-09 16:03:17.445572 timeit_compare-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2945 2024-05-02 10:48:47.000000 timeit_compare-1.2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-09 16:03:17.446076 timeit_compare-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1248 2024-05-09 10:37:12.000000 timeit_compare-1.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 16:03:17.442880 timeit_compare-1.2.2/timeit_compare.egg-info/
--rw-rw-rw-   0        0        0     3916 2024-05-09 16:03:17.000000 timeit_compare-1.2.2/timeit_compare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-05-09 16:03:17.000000 timeit_compare-1.2.2/timeit_compare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 16:03:17.000000 timeit_compare-1.2.2/timeit_compare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-09 16:03:17.000000 timeit_compare-1.2.2/timeit_compare.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    26093 2024-05-09 14:39:51.000000 timeit_compare-1.2.2/timeit_compare.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:14:42.670591 timeit_compare-1.3.0/
+-rw-rw-rw-   0        0        0     1089 2024-04-13 14:44:22.000000 timeit_compare-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4094 2024-06-03 14:14:42.669591 timeit_compare-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2966 2024-06-02 18:40:49.000000 timeit_compare-1.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-03 14:14:42.670591 timeit_compare-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1434 2024-06-02 10:29:32.000000 timeit_compare-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-03 14:14:42.659750 timeit_compare-1.3.0/timeit_compare/
+-rw-rw-rw-   0        0        0    23318 2024-06-03 13:00:56.000000 timeit_compare-1.3.0/timeit_compare/__init__.py
+-rw-rw-rw-   0        0        0     2469 2024-06-02 13:24:29.000000 timeit_compare-1.3.0/timeit_compare/__init__.pyi
+-rw-rw-rw-   0        0        0     3657 2024-06-02 20:49:53.000000 timeit_compare-1.3.0/timeit_compare/__main__.py
+-rw-rw-rw-   0        0        0       77 2024-06-02 13:24:29.000000 timeit_compare-1.3.0/timeit_compare/__main__.pyi
+drwxrwxrwx   0        0        0        0 2024-06-03 14:14:42.668453 timeit_compare-1.3.0/timeit_compare.egg-info/
+-rw-rw-rw-   0        0        0     4094 2024-06-03 14:14:42.000000 timeit_compare-1.3.0/timeit_compare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2024-06-03 14:14:42.000000 timeit_compare-1.3.0/timeit_compare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-03 14:14:42.000000 timeit_compare-1.3.0/timeit_compare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-06-03 14:14:42.000000 timeit_compare-1.3.0/timeit_compare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-06-03 14:14:42.000000 timeit_compare-1.3.0/timeit_compare.egg-info/top_level.txt
```

### Comparing `timeit_compare-1.2.2/LICENSE` & `timeit_compare-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeit_compare-1.2.2/setup.py` & `timeit_compare-1.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='timeit_compare',
-    version='1.2.2',
-    py_modules=['timeit_compare'],
-    license='MIT',
+    version='1.3.0',
+    packages=['timeit_compare'],
+    install_requires=['typing_extensions'],
     python_requires='>=3.6.0',
-    description='Based on the timeit library, timeit_compare can time multiple '
-                'statements and provide comparison results.',
+    license='MIT',
+    description='Based on the timeit library, timeit_compare can conveniently '
+                'measure execution times of multiple statements and provide '
+                'some basic descriptive statistics to compare the results.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['timeit_compare', 'timeit', 'performance'],
     author='Liu Wei',
     author_email='23S112099@stu.hit.edu.cn',
     maintainer='Liu Wei',
     maintainer_email='23S112099@stu.hit.edu.cn',
@@ -25,9 +27,10 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
+        'Programming Language :: Python :: 3.13'
     ]
 )
```

### Comparing `timeit_compare-1.2.2/timeit_compare.py` & `timeit_compare-1.3.0/timeit_compare/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,587 +1,595 @@
 """
-Based on the timeit library, timeit_compare can time multiple statements and
-provide comparison results.
+Based on the timeit library, timeit_compare can conveniently measure execution
+times of multiple statements and provide some basic descriptive statistics to
+compare the results.
 
 Python quick usage:
     from timeit_compare import compare
 
-    compare(*timer_args[, setup][, globals][, repeat][, number][, time]
-        [, show_progress][, sort_by][, reverse][, decimal])
+    compare(*add_timers[, setup][, globals][, add_stats][, repeat][, number]
+        [, time][, show_progress][, sort_by][, reverse][, stats][, percentage]
+        [, precision])
 
 See the function compare.
 
 Command line usage:
-    python -m timeit_compare [-s] [-r] [-n] [-t] [--hide-progress] [--sort-by]
-        [--reverse] [-d] [-h] [--] [timer_args ...]
+    python -m timeit_compare [-h] [-v] [-a ADD_TIMERS [ADD_TIMERS ...]]
+        [-s SETUP [SETUP ...]] [-r REPEAT] [-n NUMBER] [-t TIME] [--no-progress]
+        [--sort-by {mean,median,min,max,std}] [--no-sort] [--reverse]
+        [--stats [{mean,median,min,max,std} ...]]
+        [--percentage [{mean,median,min,max,std} ...]] [-p PRECISION]
 
-See the function main.
+Run 'python -m timeit_compare -h' for command line help.
+"""
 
-Note that if an error occurs during the operation of a statement, the program
-will stop timing this statement, display the error type in the error cell of
-the final results, and then continue to time other statements without errors.
+# python >= 3.6
 
-If you actively terminate the program, all statements immediately stop timing
-and then output the comparison results of the data already obtained.
+import itertools
+import statistics
+import sys
+import time
+from collections import namedtuple, OrderedDict
+from keyword import iskeyword
+from timeit import Timer
+from typing import Sequence
 
-To ensure a good user experience, the output terminal should use a font that
-has a fixed width and supports unicode characters. Additionally, it is best not
-to automatically wrap lines of text.
-"""
+if sys.version_info >= (3, 7):
+    OrderedDict = dict
 
-from collections import namedtuple
-from itertools import count, chain
-from time import perf_counter
-from timeit import Timer
-from typing import Union, Sequence, Callable, Iterable
+__version__ = '1.3.0'
 
 __all__ = ['TimerResult', 'Compare', 'compare']
 
+# store the result of a timer
+TimerResult = namedtuple('TimerResult', (
+    'id', 'repeat', 'stats', 'time', 'number'))
 
-def _percent(a, b):
-    """Internal function."""
-    return a / b if b else 1.0
+_DEFAULT_STATS = OrderedDict(
+    mean=statistics.fmean if sys.version_info >= (3, 8) else statistics.mean,
+    median=statistics.median,
+    min=min,
+    max=max,
+    std=statistics.stdev
+)
 
 
-# store the result of a timer
-TimerResult = namedtuple(
-    'TimerResult',
-    (
-        'index', 'error', 'time', 'repeat', 'number',
-        'mean', 'median', 'min', 'max', 'std'
-    )
-)
+def _stat_call(func, time):
+    """Internal function."""
+    try:
+        value = func(time)
+        if isinstance(value, (float, int)):
+            return value
+    except:
+        pass
 
 
-class _Timer:
+class _Timer(Timer):
     """Internal class."""
 
-    def __init__(self, index, stmt, setup, globals):
-        self.index = index
+    def __init__(self, stmt, setup, globals):
+        super().__init__(stmt, setup, time.perf_counter, globals)
+        self.id = -1
         self.stmt = stmt
-        self.timer = Timer(stmt, setup, perf_counter, globals)
-        self.error = None
-        self.time = []
+        self.time = ()
         self.total_time = 0.0
-        self.mean = self.median = self.min = self.max = self.std = None
+        self.stats = {}
         self._result = None
 
-    def reset(self):
-        self.error = None
-        self.time.clear()
-        self.total_time = 0.0
-        self.mean = self.median = self.min = self.max = self.std = None
-        self._result = None
+    repeat = property(lambda self: len(self.time))
 
-    def pre_timeit(self, number):
-        if self.error is None:
-            try:
-                time = self.timer.timeit(number)
-            except Exception as e:
-                self.error = type(e)
-                return None, True
-            else:
-                return time, False
-        return None, False
+    def add_stat(self, stat, func):
+        self.stats[stat] = _stat_call(func, self.time)
+        self._result = None
 
-    def pre_interrupt(self, e):
-        if self.error is None:
-            self.error = type(e)
-            return True
-        return False
+    def del_stat(self, stat):
+        del self.stats[stat]
+        self._result = None
 
-    def timeit(self, number):
-        if self.error is None:
+    if sys.version_info >= (3, 11):
+        def timeit(self, number):
             try:
-                time = self.timer.timeit(number)
+                return super().timeit(number)
             except Exception as e:
-                self.error = type(e)
-                return True
-            else:
-                self.time.append(time / number)
-                self.total_time += time
-        return False
-
-    def interrupt(self, e, repeat):
-        if self.error is None:
-            if len(self.time) < repeat:
-                self.error = type(e)
-                return True
-        return False
-
-    def statistic(self):
-        if self.time:
-            n = len(self.time)
-            mean = sum(self.time) / n
-            sorted_time = sorted(self.time)
-            k = n // 2
-            if n & 1:
-                median = sorted_time[k]
-            else:
-                median = (sorted_time[k] + sorted_time[k - 1]) / 2
-            min_ = sorted_time[0]
-            max_ = sorted_time[-1]
-            if n >= 2:
-                std = ((sum(i * i for i in self.time) - n * mean * mean) /
-                       (n - 1)) ** 0.5
-            else:
-                std = None
-        else:
-            mean = median = min_ = max_ = std = None
+                e.add_note(f'(timer id: {self.id})')
+                raise
 
-        self.mean = mean
-        self.median = median
-        self.min = min_
-        self.max = max_
-        self.std = std
-
-    def get_result(self, number):
+    def get_result(self, number, stats_namedtuple):
         if self._result is None:
             self._result = TimerResult(
-                self.index, self.error, self.time.copy(), len(self.time),
-                number, self.mean, self.median, self.min, self.max, self.std)
+                id=self.id,
+                repeat=self.repeat,
+                stats=stats_namedtuple(**self.stats),
+                time=self.time,
+                number=number)
         return self._result
 
-    _null = '-'
+    def get_line(self, stats, max_value, precision):
+        line = []
 
-    def get_line(self, decimal, max_mean, max_median, repeat):
-        index = f'{self.index}'
+        id = f'{self.id}'
+        line.append(id)
 
         if isinstance(self.stmt, str):
             stmt = repr(self.stmt)[1:-1]
         elif callable(self.stmt):
             if hasattr(self.stmt, '__name__'):
                 stmt = f'{self.stmt.__name__}()'
             else:
                 stmt = self._null
         else:
             stmt = self._null
         if len(stmt) > 25:
             stmt = f'{stmt[:24]}…'
+        line.append(stmt)
 
-        if self.time:
-            scale = float(f"1e{f'{self.min:.0e}'.split('e', 1)[1]}")
-            unit = f'{scale:.0e}s'
-
-            d_time = decimal
-
-            def format_time(second):
-                return f'{second / scale:.{d_time}f}'
-
-            d_percent = max(decimal - 2, 0)
-
-            def format_percent(percent):
-                d = d_percent + (
-                    0 if percent >= 1.0 else
-                    1 if percent >= 0.1 else
-                    2
-                )
-                return f'{percent:#.{d}%}'
-
-            d_progress = 5 + decimal
-
-            def format_progress(percent):
-                return _progress_bar(percent, d_progress)
-
-            mean = format_time(self.mean)
-            percent = _percent(self.mean, max_mean)
-            mean_percent = format_percent(percent)
-            mean_progress = format_progress(percent)
-
-            median = format_time(self.median)
-            percent = _percent(self.median, max_median)
-            median_percent = format_percent(percent)
-            median_progress = format_progress(percent)
-
-            min_ = format_time(self.min)
-            max_ = format_time(self.max)
-            if len(self.time) >= 2:
-                std = format_time(self.std)
+        repeat = f'{self.repeat}'
+        line.append(repeat)
+
+        p_time = precision
+        p_percentage = max(precision - 2, 0)
+        p_progress = 5 + precision
+
+        for stat in stats:
+            value = self.stats[stat]
+
+            if value is not None:
+                key_time = self.format_time(value, p_time)
             else:
-                std = self._null
+                key_time = self._null
+            line.append(key_time)
 
-        else:
-            unit = mean = mean_percent = mean_progress = \
-                median = median_percent = median_progress = \
-                min_ = max_ = std = self._null
-
-        if self.error is not None:
-            error = self.error.__name__
-            if len(self.time) < repeat:
-                error = f'{error}(r={len(self.time)})'
-        else:
-            error = self._null
+            if stat in max_value:
+                if value is not None:
+                    percent = value / max_value[stat] \
+                        if max_value[stat] else 1.0
+                    key_percent = [
+                        self.format_percentage(percent, p_percentage),
+                        self.format_progress(percent, p_progress)]
+                else:
+                    key_percent = [self._null, self._null]
+                line.extend(key_percent)
 
-        return (index, stmt, unit, mean, mean_percent, mean_progress, median,
-                median_percent, median_progress, min_, max_, std, error)
+        return line
+
+    _null = '-'
+
+    @staticmethod
+    def format_time(second, p):
+        s = f'{second:#.{p}g}'
+        if 'e' in s:
+            # 1e+05 -> 1e+5
+            a, b = s.split('e', 1)
+            s = f'{a}e{int(b):+}'
+        return s
+
+    @staticmethod
+    def format_percentage(percent, p):
+        k = 1.0 - 5 * 0.1 ** (p + 4)
+        d = p + (
+            0 if percent >= k else
+            1 if percent >= 0.1 * k else
+            2
+        )
+        return f'{percent:#.{d}%}'
+
+    @staticmethod
+    def format_progress(percent, p):
+        return _progress_bar(percent, p)
 
 
 class Compare:
-    """Main class, used to create timers, run timers, view or print timer
-    results."""
+    """Main class, used to create timers, create statistics, run timers, and get
+    or print results."""
 
-    def __init__(self) -> None:
+    def __init__(self):
         """Constructor."""
-        self._index = count()
-        self._timer = {}
-        self._repeat = 0
+        self._timer_id = itertools.count()
+        self._timer = OrderedDict()
+        self._stats = _DEFAULT_STATS.copy()
         self._number = 0
+        self._stats_namedtuple = None
 
-    def reset(self) -> None:
-        """Reset all timers for a rerun. All results will be deleted."""
-        for timer in self._timer.values():
-            timer.reset()
-        self._repeat = 0
-        self._number = 0
-
-    def add_timer(
-            self,
-            stmt: Union[Callable, str],
-            setup: Union[Callable, str] = 'pass',
-            globals: dict = None
-    ) -> int:
+    def add_timer(self, stmt, setup='pass', globals=None):
         """
-        Add a timer.
+        Add a new timer.
         :param stmt: statement to be timed.
-        :param setup: statement to be executed once initially (default 'pass').
+        :param setup: statement to be executed once initially (default: 'pass').
             Execution time of this setup statement is NOT timed.
         :param globals: if specified, the code will be executed within that
-            namespace (default None, inside timeit's namespace).
-        :return: index of the new timer.
+            namespace (default: {}).
+        :return: an identifier for the new timer.
         """
-        index = next(self._index)
-        timer = _Timer(index, stmt, setup, globals)
-        self._timer[index] = timer
-        return index
+        if globals is None:
+            globals = {}
+        timer = _Timer(stmt, setup, globals)
+        for stat, func in self._stats.items():
+            timer.add_stat(stat, func)
+        id = next(self._timer_id)
+        timer.id = id
+        self._timer[id] = timer
+        return id
 
-    def del_timer(self, index: int) -> None:
+    def del_timer(self, id):
         """
         Delete a timer.
-        :param index: index of the timer.
+        :param id: timer id.
         """
-        del self._timer[index]
-
-    def run(
-            self,
-            repeat: int = 5,
-            number: int = 0,
-            time: Union[float, int] = 1.0,
-            include: Iterable[int] = None,
-            exclude: Iterable[int] = None,
-            show_progress: bool = False
-    ) -> None:
-        """
-        Run timers.
-        :param repeat: how many times to repeat the timer (default 5).
-        :param number: how many times to execute statement (default 0,
-            estimated by time).
-        :param time: approximate total running time of all statements in
-            seconds (default 1.0). Ignored when number is greater than 0.
-        :param include: indexes of the included timers (default None, including
-            all timers).
-        :param exclude: indexes of the excluded timers (default None, no timers
-            are excluded).
-        :param show_progress: whether to show a progress bar (default False).
-        """
-        args = Compare._run_args(repeat, number, time, show_progress)
-        timers = self._select(include, exclude)
-        self.reset()
-        self._run(timers, *args)
+        del self._timer[id]
 
-    def get_result(self, index: int) -> TimerResult:
+    def add_stat(self, stat, func):
         """
-        Get the result of a timer.
-        :param index: index of the timer.
-        :return: the result of the specified timer.
+        Add a new statistic.
+        :param stat: name of the new statistic.
+        :param func: a function to calculate the new statistic. This function
+            should allow receiving a tuple composed of floating point time and
+            return a real number or None.
         """
-        return self._timer[index].get_result(self._number)
+        stat = self._check_stat(stat)
+
+        if not callable(func):
+            raise TypeError(f'func must be a callable, not '
+                            f'{type(func).__name__!r}')
+
+        self._stats[stat] = func
+        self._stats_namedtuple = None
+        for timer in self._timer.values():
+            timer.add_stat(stat, func)
 
-    def get_fastest(self, sort_by: str = 'mean') -> Union[TimerResult, None]:
+    def _check_stat(self, stat, message='stat'):
+        """Internal function."""
+        if type(stat) is not str:
+            raise TypeError(f'{message} must be a string, not '
+                            f'{type(stat).__name__!r}')
+        if not stat.isidentifier():
+            raise ValueError(f'{message} must be a valid identifier, not '
+                             f'{stat!r}')
+        if iskeyword(stat):
+            raise ValueError(f'{message} cannot be a keyword: {stat!r}')
+        if stat.startswith('_'):
+            raise ValueError(f'{message} cannot start with an underscore: '
+                             f'{stat!r}')
+        return stat.lower()
+
+    def del_stat(self, stat):
         """
-        Get the result of the fastest timer.
-        :param sort_by: the basis for sorting the results, which can be 'index',
-            'mean', 'median', 'min', 'max' or 'std' (default 'mean').
-        :return: the result of the specified timer.
+        Delete a statistic.
+        :param stat: name of the statistic.
         """
-        sort_by = Compare._sort_by_args(sort_by)
-
-        min_timer = None
-        min_time = float('inf')
+        stat = self._check_stat_select(stat)
 
+        del self._stats[stat]
+        self._stats_namedtuple = None
         for timer in self._timer.values():
-            time = getattr(timer, sort_by)
-            if time is not None:
-                if time < min_time:
-                    min_timer, min_time = timer, time
-
-        if min_timer is not None:
-            return min_timer.get_result(self._number)
-
-    def print_results(
-            self,
-            sort_by: str = 'mean',
-            reverse: bool = False,
-            decimal: int = 2,
-            include: Iterable[int] = None,
-            exclude: Iterable[int] = None
-    ) -> None:
-        """
-        Print the results of the timers in tabular form.
-        :param sort_by: the basis for sorting the results, which can be 'index',
-            'mean', 'median', 'min', 'max' or 'std' (default 'mean').
-        :param reverse: whether to sort the results in descending order
-            (default False).
-        :param decimal: number of decimal places to be retained (default 2).
-        :param include: indexes of the included timers (default None, including
-            all timers).
-        :param exclude: indexes of the excluded timers (default None, no timers
-            are excluded).
-        """
-        args = Compare._print_results_args(sort_by, reverse, decimal)
-        timers = self._select(include, exclude)
-        return self._print_results(timers, *args)
+            timer.del_stat(stat)
 
-    def _select(self, include=None, exclude=None):
+    def _check_stat_select(self, stat, message='stat'):
         """Internal function."""
-        if include is not None and exclude is not None:
+        stat = self._check_stat(stat, message)
+        if stat not in self._stats:
             raise ValueError(
-                'the include and exclude parameters cannot be '
-                'set simultaneously')
-        if include is not None:
-            include = set(include)
-            timers = [self._timer[index] for index in include]
-        elif exclude is not None:
-            exclude = set(exclude)
-            include = self._timer.keys() - exclude
-            timers = [self._timer[index] for index in include]
-        else:
-            timers = list(self._timer.values())
-        return timers
+                f"stat {stat!r} is not in the optional statistics: "
+                f"{{{', '.join(map(repr, self._stats))}}}.")
+        return stat
 
-    def _run(self, timers, repeat, number, time, show_progress):
-        """Internal function."""
-        timer_num = len(timers)
-        error = 0
-        total_repeat = timer_num * repeat
-        complete = 0
-
-        def update_progress():
-            if not show_progress:
-                return
-            percent = _percent(complete, total_repeat)
-            string = (f'\r|{_progress_bar(percent, 12)}| '
-                      f'{complete}/{total_repeat} completed, '
-                      f'{error}/{timer_num} error')
-            print(string, end='', flush=True)
+    def run(self, repeat=5, number=0, time=1.0, show_progress=False):
+        """
+        Run timers.
+        :param repeat: how many times to repeat the timer (default: 5).
+        :param number: how many times to execute statement (default: estimated
+            by time).
+        :param time: if specified and no number greater than 0 is specified, it
+            will be used to estimate a number so that the total execution time
+            (in seconds) of all statements is approximately equal to this value
+            (default: 1.0).
+        :param show_progress: whether to show a progress bar (default: False).
+        """
+        if not isinstance(repeat, int):
+            raise TypeError(f'repeat must be a integer, not '
+                            f'{type(repeat).__name__!r}')
+        if repeat < 1:
+            repeat = 1
+
+        if not isinstance(number, int):
+            raise TypeError(f'number must be a integer, not '
+                            f'{type(number).__name__!r}')
+
+        if not isinstance(time, (float, int)):
+            raise TypeError(f'time must be a real number, not '
+                            f'{type(time).__name__!r}')
+        if time < 0.0:
+            time = 0.0
+
+        show_progress = bool(show_progress)
+
+        if not self._timer:
+            return
 
         if show_progress:
             print('timing now...')
 
-        if number == 0:
-            def estimate():
-                nonlocal error
+        # Temporarily store the results and update them to the instance
+        # properties after all processing is completed and no errors occur
+        new = {
+            timer: {
+                'time': [],
+                'total_time': 0.0,
+                'stats': {},
+                '_results': None
+            }
+            for timer in self._timer.values()
+        }
+
+        catch_interrupt = hasattr(self, '_catch_interrupt')
+
+        try:
+            if number <= 0:
                 n = 1
                 while True:
-                    total_time = 0.0
-                    for timer in timers:
-                        pre_time, turn_error = timer.pre_timeit(n)
-                        if pre_time is not None:
-                            total_time += pre_time
-                        if turn_error:
-                            error += 1
-                    if error == timer_num:
-                        return 0
-                    if total_time > 0.2:
-                        return max(round(n * time / total_time / repeat), 1)
-                    n = int(n * 0.25 / total_time) + 1 if total_time else n * 2
+                    t = 0.0
+                    for timer in new:
+                        t += timer.timeit(n)
+                    if t > 0.2:
+                        number = max(round(n * time / t / repeat), 1)
+                        break
+                    n = int(n * 0.25 / t) + 1 if t else n * 2
 
-            try:
-                number = estimate()
-            except (KeyboardInterrupt, SystemExit) as e:
-                for timer in timers:
-                    turn_error = timer.pre_interrupt(e)
-                    if turn_error:
-                        error += 1
-
-        update_progress()
+            if show_progress:
+                progress = self._run_progress(len(new) * repeat)
+            else:
+                progress = itertools.repeat(None)
 
-        try:
+            next(progress)
             for _ in range(repeat):
-                for timer in timers:
-                    turn_error = timer.timeit(number)
-                    if turn_error:
-                        error += 1
-                    complete += 1
-                    update_progress()
-
-        except (KeyboardInterrupt, SystemExit) as e:
-            for timer in timers:
-                turn_error = timer.interrupt(e, repeat)
-                if turn_error:
-                    error += 1
-            complete = total_repeat
-            update_progress()
+                for timer, result in new.items():
+                    t = timer.timeit(number)
+                    result['time'].append(t / number)
+                    result['total_time'] += t
+                    next(progress)
+
+        except KeyboardInterrupt as e:
+            if not catch_interrupt:
+                raise
+            self._catch_interrupt = e
 
         if show_progress:
             print()
 
-        for timer in timers:
-            timer.statistic()
-
-        self._repeat = repeat
+        for result in new.values():
+            result['time'] = tuple(result['time'])
+            for stat, func in self._stats.items():
+                result['stats'][stat] = _stat_call(func, result['time'])
+
+        # update new results
+        for timer, result in new.items():
+            timer.__dict__.update(result)
         self._number = number
 
-    def _print_results(self, timers, sort_by, reverse, decimal):
-        """Internal function."""
-        title = 'Comparison Results'
+    @staticmethod
+    def _run_progress(task_num):
+        for i in range(task_num + 1):
+            progress = (f'\r|{_progress_bar(i / task_num, 12)}| '
+                        f'{i}/{task_num} completed')
+            print(progress, end='', flush=True)
+            yield
+
+    def get_result(self, id):
+        """
+        Get the result of a timer.
+        :param id: timer id.
+        :return: the result of the specified timer.
+        """
+        if self._stats_namedtuple is None:
+            self._stats_namedtuple = namedtuple('Stats', self._stats)
+        return self._timer[id].get_result(
+            self._number, self._stats_namedtuple)
 
-        header = ['Idx', 'Stmt', 'Unit', 'Mean', 'Median', 'Min', 'Max',
-                  'Std', 'Err']
-        if sort_by == 'index':
-            i = 0
-        elif sort_by == 'mean':
-            i = 3
-        elif sort_by == 'median':
-            i = 4
-        elif sort_by == 'min':
-            i = 5
-        elif sort_by == 'max':
-            i = 6
-        else:  # sort_by == 'std'
-            i = 7
-        header[i] = f"{header[i]} {'↓' if not reverse else '↑'}"
-        header[5] = f'{header[5]} - {header.pop(6)}'
-
-        header_cols = (1, 1, 1, 3, 3, 2, 1, 1)
-
-        max_mean = 0.0
-        max_median = 0.0
-        total_time = 0.0
+    def get_min(self, stat='mean'):
+        """
+        Get the result of the timer with the minimum statistic.
+        :param stat: search by this statistic (default: 'mean').
+        :return: the result of the specified timer.
+        """
+        stat = self._check_stat_select(stat)
 
-        for timer in timers:
-            if timer.mean is not None:
-                if timer.mean > max_mean:
-                    max_mean = timer.mean
-            if timer.median is not None:
-                if timer.median > max_median:
-                    max_median = timer.median
-            total_time += timer.total_time
+        min_id = None
+        min_value = float('inf')
 
-        result, result1 = [], []
-        for timer in timers:
-            (result if getattr(timer, sort_by) is not None else
-             result1).append(timer)
+        for id, timer in self._timer.items():
+            value = timer.stats[stat]
+            if value is not None:
+                if value < min_value:
+                    min_id, min_value = id, value
 
-        result.sort(key=lambda item: getattr(item, sort_by), reverse=reverse)
-        result.extend(result1)
+        if min_id is not None:
+            return self.get_result(min_id)
 
-        body = [timer.get_line(decimal, max_mean, max_median, self._repeat)
-                for timer in result]
+    def get_max(self, stat='mean'):
+        """
+        Get the result of the timer with the maximum statistic.
+        :param stat: search by this statistic (default: 'mean').
+        :return: the result of the specified timer.
+        """
+        stat = self._check_stat_select(stat)
 
-        note = (f"{self._repeat} repetition{'s' if self._repeat != 1 else ''}, "
-                f"{self._number} loop{'s' if self._number != 1 else ''} each, "
-                f"total runtime {total_time:.4f}s")
+        max_id = None
+        max_value = float('-inf')
 
-        print(_table(title, header, header_cols, body, note))
+        for id, timer in self._timer.items():
+            value = timer.stats[stat]
+            if value is not None:
+                if value > max_value:
+                    max_id, max_value = id, value
 
-    @staticmethod
-    def _sort_by_args(sort_by):
-        """Internal function."""
-        if not isinstance(sort_by, str):
-            raise TypeError(f'sort_by must be a string, not {type(sort_by)}')
-        sort_by = sort_by.lower()
-        if sort_by not in {'index', 'mean', 'median', 'min', 'max', 'std'}:
-            raise ValueError(
-                f'sort_by must be index, mean, median, min, max or std, '
-                f'not {sort_by}')
+        if max_id is not None:
+            return self.get_result(max_id)
 
-        return sort_by
+    def print_results(self, include=None, exclude=None, sort_by='mean',
+                      reverse=False, stats=None, percentage=None, precision=2):
+        """
+        Print the results of the timers in tabular form.
+        :param include: ids of the included timers (default: including all
+            timers).
+        :param exclude: ids of the excluded timers (default: no timers
+            excluded).
+        :param sort_by: statistic for sorting the results (default: 'mean'). If
+            None is specified, no sorting will be performed.
+        :param reverse: whether to sort the results in descending order
+            (default: False).
+        :param stats: statistics in the column headers of the table (default:
+            all statistics in default order).
+        :param percentage: statistics showing percentage (default: same as
+            sort_by).
+        :param precision: digits precision of the results (default: 2).
+        """
+        args = self._print_results_args(
+            include, exclude, sort_by, reverse, stats, percentage, precision)
+        return self._print_results(*args)
 
-    @staticmethod
-    def _run_args(repeat, number, time, show_progress):
+    def _print_results_args(self, include, exclude, sort_by, reverse, stats,
+                            percentage, precision):
         """Internal function."""
-        if not isinstance(repeat, int):
-            raise TypeError(f'repeat must be a integer, not {type(repeat)}')
-        if repeat < 1:
-            repeat = 1
+        if include is not None and exclude is not None:
+            raise ValueError('include and exclude cannot be set simultaneously')
+        if include is not None:
+            include = set(include)
+            timers = [self._timer[i] for i in include]
+        elif exclude is not None:
+            exclude = set(exclude)
+            timers = [timer for i, timer in self._timer.items()
+                      if i not in exclude]
+        else:
+            timers = list(self._timer.values())
 
-        if not isinstance(number, int):
-            raise TypeError(f'number must be a integer, not {type(number)}')
-        if number < 0:
-            number = 0
+        if sort_by is not None:
+            sort_by = self._check_stat_select(sort_by, 'sort_by')
 
-        if not isinstance(time, (float, int)):
-            raise TypeError(f'time must be a real number, not {type(time)}')
-        if time < 0.0:
-            time = 0.0
+        reverse = bool(reverse)
 
-        show_progress = bool(show_progress)
+        if stats is None:
+            stats = list(self._stats)
+        else:
+            if isinstance(stats, str):
+                stats = stats.replace(',', ' ').split()
+            stats = [self._check_stat_select(stat) for stat in stats]
+
+        if percentage is None:
+            percentage = sort_by
+        if percentage is None:
+            percentage = []
+        elif isinstance(percentage, str):
+            percentage = percentage.replace(',', ' ').split()
+        percentage = {self._check_stat_select(stat, 'item in percentage')
+                      for stat in percentage}
+        percentage &= set(stats)
+
+        if not isinstance(precision, int):
+            raise TypeError(f'precision must be a integer, not '
+                            f'{type(precision).__name__!r}')
+        if precision < 1:
+            precision = 1
+        elif precision > 8:
+            precision = 8
 
-        return repeat, number, time, show_progress
+        return timers, sort_by, reverse, stats, percentage, precision
 
-    @staticmethod
-    def _print_results_args(sort_by, reverse, decimal):
+    def _print_results(self, timers, sort_by, reverse, stats, percentage,
+                       precision):
         """Internal function."""
-        sort_by = Compare._sort_by_args(sort_by)
+        title = 'Comparison Results (unit: s)'
 
-        reverse = bool(reverse)
+        header = ['Id', 'Stmt', 'Rpt', *(stat.title() for stat in stats)]
+        if sort_by is not None:
+            for i, stat in enumerate(stats, 3):
+                if stat == sort_by:
+                    header[i] = f"{header[i]} {'↓' if not reverse else '↑'}"
+
+            timers_sort, timers_none = [], []
+            for timer in timers:
+                (timers_sort if timer.stats[sort_by] is not None else
+                 timers_none).append(timer)
+            timers_sort.sort(key=lambda item: item.stats[sort_by],
+                             reverse=reverse)
+            timers = timers_sort + timers_none
+
+        header_cols = [1] * len(header)
+        for i, stat in enumerate(stats, 3):
+            if stat in percentage:
+                header_cols[i] = 3
 
-        if not isinstance(decimal, int):
-            raise TypeError(f'decimal must be a integer, not {type(decimal)}')
-        if decimal < 0:
-            decimal = 0
-        elif decimal > 8:
-            decimal = 8
-
-        return sort_by, reverse, decimal
-
-
-def compare(
-        *timer_args: Union[Sequence, Callable, str],
-        setup: Union[Callable, str] = 'pass',
-        globals: dict = None,
-        repeat: int = 5,
-        number: int = 0,
-        time: Union[float, int] = 1.0,
-        show_progress: bool = True,
-        sort_by: str = 'mean',
-        reverse: bool = False,
-        decimal: int = 2
-) -> None:
+        max_value = dict.fromkeys(percentage, 0.0)
+        for timer in timers:
+            for stat in percentage:
+                value = timer.stats[stat]
+                if value is not None:
+                    if value > max_value[stat]:
+                        max_value[stat] = value
+
+        body = [timer.get_line(stats, max_value, precision) for timer in timers]
+
+        total_time = sum(timer.total_time for timer in timers)
+        notes = [
+            f"{self._number} execution{'s' if self._number != 1 else ''} for "
+            f"each statement per repetition",
+            f"total execution time {total_time:.4f}s"
+        ]
+
+        print(_table(title, header, header_cols, body, notes))
+
+
+def compare(*add_timers, setup='pass', globals=None, add_stats=(), repeat=5,
+            number=0, time=1.0, show_progress=True, sort_by='mean',
+            reverse=False, stats=None, percentage=None, precision=2):
     """
-    Convenience function to create Compare object, call add_timer, run and
-    print_results methods.
+    Convenience function to create Compare object, call add_timer, add_stat, run
+    and print_results methods.
 
-    :param timer_args: a sequence (statement, setup, globals) or a single
-        statement for Compare.add_timer method.
-    :param setup: default setup for positional parameters with no or None setup
-        given (default: same as Compare.add_timer).
-    :param globals: default globals for positional parameters with no or None
-        globals given (default: same as Compare.add_timer).
+    :param add_timers: (statement, setup, globals) or a single statement for
+        Compare.add_timer method.
+    :param setup: the global default value for setup in add_timers (default:
+        same as Compare.add_timer).
+    :param globals: the global default value for globals in add_timers (default:
+        same as Compare.add_timer).
+    See add_timer, add_stat, run, and print_results methods of the class Compare
+    for other parameters.
 
-    See add_timer, run, and print_results methods of the class Compare.
+    If the program is interrupted by Ctrl+C, the results will still be printed.
     """
-    run_args = Compare._run_args(repeat, number, time, show_progress)
-    print_results_args = Compare._print_results_args(sort_by, reverse, decimal)
     cmp = Compare()
-    for args in timer_args:
+
+    for args in add_timers:
         if isinstance(args, Sequence) and not isinstance(args, str):
             args = list(args)
             if len(args) < 3:
                 args.extend([None] * (3 - len(args)))
             if args[1] is None:
                 args[1] = setup
             if args[2] is None:
                 args[2] = globals
         else:
             args = args, setup, globals
         cmp.add_timer(*args)
-    timers = cmp._select()
-    cmp._run(timers, *run_args)
-    cmp._print_results(timers, *print_results_args)
+
+    for stat, func in add_stats:
+        cmp.add_stat(stat, func)
+
+    # Validate the arguments of print_results method beforehand to avoid wasting
+    # time in case an error caused by the arguments occurs after the timers have
+    # finished running
+    print_results_args = cmp._print_results_args(
+        None, None, sort_by, reverse, stats, percentage, precision)
+
+    cmp._catch_interrupt = None
+    cmp.run(repeat, number, time, show_progress)
+    interrupt = cmp._catch_interrupt
+
+    cmp._print_results(*print_results_args)
+
+    if interrupt is not None:
+        raise interrupt
 
 
 _BLOCK = ' ▏▎▍▌▋▊▉█'
 
 
 def _progress_bar(progress, length):
     """Internal function."""
@@ -589,33 +597,29 @@
         string = ' ' * length
 
     elif progress >= 1.0:
         string = _BLOCK[-1] * length
 
     else:
         d = 1.0 / length
-        q = progress // d
-        block1 = _BLOCK[-1] * int(q)
-
-        r = progress % d
+        q, r = divmod(progress, d)
+        full = _BLOCK[-1] * int(q)
         d2 = d / 8
         i = (r + d2 / 2) // d2
-        block2 = _BLOCK[int(i)]
-
-        block3 = ' ' * (length - len(block1) - len(block2))
-
-        string = f'{block1}{block2}{block3}'
+        half_full = _BLOCK[int(i)]
+        empty = ' ' * (length - len(full) - len(half_full))
+        string = f'{full}{half_full}{empty}'
 
     return string
 
 
-_TABLE_NUMBER = count(1)
+_TABLE_NUMBER = itertools.count(1)
 
 
-def _table(title, header, header_cols, body, note):
+def _table(title, header, header_cols, body, notes):
     """Internal function."""
     title = f'Table {next(_TABLE_NUMBER)}. {title}'
 
     body_width = [2] * sum(header_cols)
     for i, item in enumerate(zip(*body)):
         body_width[i] += max(map(len, item))
 
@@ -627,26 +631,26 @@
             bw = body_width[i]
             if hw > bw:
                 body_width[i] = hw
         else:
             bw = sum(body_width[i: i + col]) + col - 1
             if hw > bw:
                 bw = hw - bw
-                q, r = bw // col, bw % col
+                q, r = divmod(bw, col)
                 for j in range(i, i + col):
                     body_width[j] += q
                 for j in range(i, i + r):
                     body_width[j] += 1
         if hw < bw:
             hw = bw
         header_width.append(hw)
         i += col
 
     total_width = sum(header_width) + len(header_width) + 1
-    other_width = max(len(title), len(note))
+    other_width = max(len(title), *map(len, notes))
     if other_width > total_width:
         bw = other_width - total_width
         dl = ' ' * (bw // 2)
         dr = ' ' * (bw - bw // 2)
         total_width = other_width
     else:
         dl = dr = ''
@@ -664,115 +668,25 @@
         if col == 1:
             border = '─' * next(bw)
         else:
             border = '┬'.join('─' * next(bw) for _ in range(col))
         split_border.append(border)
     split_border = f"{dl}├{'┼'.join(split_border)}┤{dr}"
 
-    lines = [title_line, top_border, header_line, split_border]
-    lines.extend([body_line] * len(body))
-    lines.append(bottom_border)
-    lines.append(note_line)
-    template = '\n'.join(lines)
+    template = '\n'.join(
+        (
+            title_line,
+            top_border,
+            header_line,
+            split_border,
+            *[body_line] * len(body),
+            bottom_border,
+            *[note_line] * len(notes)
+        )
+    )
 
     return template.format(
         title,
         *header,
-        *chain.from_iterable(body),
-        note
+        *itertools.chain.from_iterable(body),
+        *notes
     )
-
-
-def main() -> None:
-    """Usage:
-  python -m timeit_compare [-s] [-r] [-n] [-t] [--hide-progress] [--sort-by]
-    [--reverse] [-d] [-h] [--] [timer_args ...]
-
-Options:
-  -s, --setup       default setup for positional parameters with no setup given
-                    (default 'pass').
-  -r, --repeat      how many times to repeat the timer (default 5).
-  -n, --number      how many times to execute statement (default 0, estimated
-                    by time).
-  -t, --time        approximate total running time of all statements in seconds
-                    (default 1.0). Ignored when number is greater than 0.
-  --hide-progress   hide the progress bar.
-  --sort-by         the basis for sorting the results, which can be 'index',
-                    'mean', 'median', 'min', 'max' or 'std' (default 'mean').
-  --reverse         sort the results in descending order.
-  -d, --decimal     number of decimal places to be retained (default 2).
-  -h, --help        print this usage message and exit.
-  --                separate options from statement, use when statement starts
-                    with '-'.
-  timer_args        statement to be timed (statement) and statement to be
-                    executed once initially (setup, default -s). Statement and
-                    setup are given in a single argument, separated by ';;',
-                    multi-line statement and setup can be given by separating
-                    lines with ';'. Execution time of the setup statement is NOT
-                    timed."""
-    import sys
-    args = sys.argv[1:]
-
-    import getopt
-    try:
-        opts, args = getopt.getopt(
-            args, 's:r:n:t:d:h',
-            ['setup=', 'repeat=', 'number=', 'time=', 'hide-progress',
-             'sort-by=', 'reverse', 'decimal=', 'help'])
-    except getopt.error as e:
-        e.msg = f'{e.msg}\nuse -h/--help for command line help'
-        raise
-
-    timer_args = [
-        [j.replace(';', '\n') for j in i.split(';;', 1)]
-        for i in args
-    ]
-    setup = []
-    globals = None
-    repeat = 5
-    number = 0
-    time = 1.0
-    show_progress = True
-    sort_by = 'mean'
-    reverse = False
-    decimal = 2
-    for k, v in opts:
-        if k in ('-s', '--setup'):
-            setup.append(v.replace(';', '\n'))
-        elif k in ('-r', '--repeat'):
-            repeat = int(v)
-        elif k in ('-n', '--number'):
-            number = int(v)
-        elif k in ('-t', '--time'):
-            time = float(v)
-        elif k == '--hide-progress':
-            show_progress = False
-        elif k == '--sort-by':
-            sort_by = v
-        elif k == '--reverse':
-            reverse = True
-        elif k in ('-d', '--decimal'):
-            decimal = int(v)
-        elif k in ('-h', '--help'):
-            print(main.__doc__)
-            return
-    setup = '\n'.join(setup) if setup else 'pass'
-
-    import os
-    sys.path.insert(0, os.curdir)
-
-    compare(
-        *timer_args,
-        setup=setup,
-        globals=globals,
-        repeat=repeat,
-        number=number,
-        time=time,
-        show_progress=show_progress,
-        sort_by=sort_by,
-        reverse=reverse,
-        decimal=decimal
-    )
-
-
-if __name__ == '__main__':
-    main()
```

