# Comparing `tmp/xarpes-0.1.0.tar.gz` & `tmp/xarpes-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarpes-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "xarpes-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xarpes-0.1.0.tar` & `xarpes-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0    18092 2024-05-30 12:58:26.966923 xarpes-0.1.0/LICENSE
--rw-r--r--   0        0        0     3151 2024-05-30 13:37:41.004445 xarpes-0.1.0/README.md
--rw-r--r--   0        0        0      612 2024-05-30 13:25:14.508616 xarpes-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      149 2024-05-30 13:04:29.271118 xarpes-0.1.0/xarpes/__init__.py
--rw-r--r--   0        0        0     5954 2024-05-30 13:05:52.023798 xarpes-0.1.0/xarpes/band_map.py
--rw-r--r--   0        0        0     3480 2024-05-30 12:58:26.954922 xarpes-0.1.0/xarpes/distributions.py
--rw-r--r--   0        0        0     1177 2024-05-30 13:05:10.773510 xarpes-0.1.0/xarpes/functions.py
--rw-r--r--   0        0        0     5206 2024-05-30 13:04:53.188508 xarpes-0.1.0/xarpes/plotting.py
--rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 xarpes-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0    35149 2024-06-02 15:16:58.370851 xarpes-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0     3324 2024-06-02 15:16:29.101945 xarpes-0.2.0/README.md
+-rwxr-xr-x   0        0        0      625 2024-06-02 11:12:10.476982 xarpes-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0      291 2024-05-29 10:56:48.000000 xarpes-0.2.0/xarpes/.ipynb_checkpoints/__init__-checkpoint.py
+-rwxr-xr-x   0        0        0     7423 2024-06-02 15:33:12.000000 xarpes-0.2.0/xarpes/.ipynb_checkpoints/band_map-checkpoint.py
+-rwxr-xr-x   0        0        0    13410 2024-06-02 15:32:56.000000 xarpes-0.2.0/xarpes/.ipynb_checkpoints/distributions-checkpoint.py
+-rwxr-xr-x   0        0        0     4600 2024-06-02 15:33:22.000000 xarpes-0.2.0/xarpes/.ipynb_checkpoints/functions-checkpoint.py
+-rwxr-xr-x   0        0        0     5343 2024-06-02 15:33:09.000000 xarpes-0.2.0/xarpes/.ipynb_checkpoints/plotting-checkpoint.py
+-rwxr-xr-x   0        0        0      149 2024-06-03 09:02:42.838874 xarpes-0.2.0/xarpes/__init__.py
+-rwxr-xr-x   0        0        0     7423 2024-06-02 15:33:12.136538 xarpes-0.2.0/xarpes/band_map.py
+-rwxr-xr-x   0        0        0    13410 2024-06-02 15:32:56.826971 xarpes-0.2.0/xarpes/distributions.py
+-rwxr-xr-x   0        0        0     4600 2024-06-02 15:33:22.242443 xarpes-0.2.0/xarpes/functions.py
+-rwxr-xr-x   0        0        0     5343 2024-06-02 15:33:09.246452 xarpes-0.2.0/xarpes/plotting.py
+-rw-r--r--   0        0        0     3865 1970-01-01 00:00:00.000000 xarpes-0.2.0/PKG-INFO
```

### Comparing `xarpes-0.1.0/README.md` & `xarpes-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -76,14 +76,20 @@
 	cd xARPES
 	conda create -n <my_env> -c defaults -c conda-forge --file requirements.txt
 	conda activate <my_env>
 	conda develop .
 
 Answer `y` to questions.
 
+# Examples
+
+Afer installation of xARPES, the `examples/` folder can be downloaded to the current directory with
+
+    python3 -c "import xarpes; xarpes.download_examples()"
+
 # Execution
 
 It is recommended to use JupyterLab to analyse data. JupyterLab is launched using:
 
 	jupyter lab
 
 # License
```

### Comparing `xarpes-0.1.0/pyproject.toml` & `xarpes-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 dependencies = [
     "igor2",
     "jupyterlab",
     "jupytext",
     "matplotlib",
     "numpy",
     "scipy",
+    "lmfit",
 ]
```

### Comparing `xarpes-0.1.0/xarpes/band_map.py` & `xarpes-0.2.0/xarpes/.ipynb_checkpoints/band_map-checkpoint.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (C) 2024 xARPES Developers
-# This program is free software under the terms of the GNU GPLv2 license.
+# This program is free software under the terms of the GNU GPLv3 license.
 
 # get_ax_fig_plt and add_fig_kwargs originate from pymatgen/util/plotting.py.
 # Copyright (C) 2011-2024 Shyue Ping Ong and the pymatgen Development Team
 # Pymatgen is released under the MIT License.
 
 # See also abipy/tools/plotting.py.
 # Copyright (C) 2021 Matteo Giantomassi and the AbiPy Group
@@ -24,51 +24,80 @@
         2D array of counts for given (E,k) or (E,angle) pairs [counts]
     angles : ndarray
         1D array of angular values for the abscissa [degrees]
     ekin : ndarray
         1D array of kinetic energy values for the ordinate [eV]
     energy_resolution : float
         Energy resolution of the detector [eV]
-    temperature : float
+    temperature : float, None
         Temperature of the sample [K]
-    hnuminphi : float
+    hnuminphi : float, None
         Kinetic energy minus the work function [eV]
+    hnuminphi_std : float, None
+        Standard deviation of kinetic energy minus work function [eV]
     """
     def __init__(self, intensities, angles, ekin, energy_resolution=None,
-                 temperature=None, hnuminphi=None):
-
+                 temperature=None, hnuminphi=None, hnuminphi_std=None):
         self.intensities = intensities
         self.angles = angles
         self.ekin = ekin
         self.energy_resolution = energy_resolution
         self.temperature = temperature
         self.hnuminphi = hnuminphi
+        self.hnuminphi_std = hnuminphi_std
 
     @property
     def hnuminphi(self):
-        r"""Returns the photon energy minus the work function in eV.
+        r"""Returns the photon energy minus the work function in eV if it has
+        been set, either during instantiation, with the setter, or by fitting
+        the Fermi-Dirac distribution to the integrated weight.
 
         Returns
         -------
-        hnuminphi : float
+        hnuminphi : float, None
             Kinetic energy minus the work function [eV]
         """
         return self._hnuminphi
 
     @hnuminphi.setter
     def hnuminphi(self, hnuminphi):
-        r"""Manually sets the photon energy minus the work function in eV.
+        r"""Manually sets the photon energy minus the work function in eV if it
+        has been set; otherwise returns None.
 
         Parameters
         ----------
-        hnuminphi : float
+        hnuminphi : float, None
             Kinetic energy minus the work function [eV]
         """
         self._hnuminphi = hnuminphi
 
+    @property
+    def hnuminphi_std(self):
+        r"""Returns standard deviation of the photon energy minus the work
+        function in eV.
+
+        Returns
+        -------
+        hnuminphi_std : float
+            Standard deviation of energy minus the work function [eV]
+        """
+        return self._hnuminphi_std
+
+    @hnuminphi_std.setter
+    def hnuminphi_std(self, hnuminphi_std):
+        r"""Manually sets the standard deviation of photon energy minus the
+        work function in eV.
+
+        Parameters
+        ----------
+        hnuminphi_std : float
+            Standard deviation of energy minus the work function [eV]
+        """
+        self._hnuminphi_std = hnuminphi_std
+
     def shift_angles(self, shift):
         r"""
         Shifts the angles by the specified amount in degrees. Used to shift
         from the detector angle to the material angle.
 
         Parameters
         ----------
@@ -80,14 +109,17 @@
     @add_fig_kwargs
     def fit_fermi_edge(self, hnuminphi_guess, background_guess=0.0,
                        integrated_weight_guess=1.0, angle_min=-np.infty,
                        angle_max=np.infty, ekin_min=-np.infty,
                        ekin_max=np.infty, ax=None, **kwargs):
         r"""
         Fits the Fermi edge of the band map and plots the result.
+        Also sets hnuminphi, the kinetic energy minus the work function in eV.
+        The fitting includes an energy convolution with an abscissa range
+        expanded by 5 times the energy resolution standard deviation.
 
         Parameters
         ----------
         hnuminphi_guess : float
             Initial guess for kinetic energy minus the work function [eV]
         background_guess : float
             Initial guess for background intensity [counts]
@@ -100,21 +132,25 @@
         ekin_min : float
             Minimum kinetic energy of integration interval [eV]
         ekin_max : float
             Maximum kinetic energy of integration interval [eV]
         ax : Matplotlib-Axes / NoneType
             Axis for plotting the Fermi edge on. Created if not provided by
             the user.
+
+        Other parameters
+        ----------------
         **kwargs : dict, optional
             Additional arguments passed on to add_fig_kwargs. See the keyword
             table below.
 
         Returns
         -------
-        Matplotlib-Figure
+        fig : Matplotlib-Figure
+            Figure containing the Fermi edge fit
         """
         from xarpes.functions import fit_leastsq
 
         ax, fig, plt = get_ax_fig_plt(ax=ax)
 
         min_angle_index = np.argmin(np.abs(self.angles - angle_min))
         max_angle_index = np.argmin(np.abs(self.angles - angle_max))
@@ -144,14 +180,15 @@
 
         fdir_final = fermi_dirac(temperature=self.temperature,
                                  hnuminphi=popt[0], background=popt[1],
                                  integrated_weight=popt[2],
                                  name='Fitted result')
 
         self.hnuminphi = popt[0]
+        self.hnuminphi_std = np.sqrt(np.diag(pcov))[0][0]
 
         ax.set_xlabel(r'$E_{\mathrm{kin}}$ (-)')
         ax.set_ylabel('Counts (-)')
         ax.set_xlim([ekin_min, ekin_max])
 
         ax.plot(energy_range, integrated_intensity, label='Data')
 
@@ -161,8 +198,8 @@
 
         ax.plot(energy_range, fdir_final.convolve(energy_range,
                 energy_resolution=self.energy_resolution),
                 label=fdir_final.name)
 
         ax.legend()
 
-        return fig
+        return fig
```

### Comparing `xarpes-0.1.0/xarpes/plotting.py` & `xarpes-0.2.0/xarpes/.ipynb_checkpoints/plotting-checkpoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (C) 2024 xARPES Developers
-# This program is free software under the terms of the GNU GPLv2 license.
+# This program is free software under the terms of the GNU GPLv3 license.
 
 # get_ax_fig_plt and add_fig_kwargs originate from pymatgen/util/plotting.py.
 # Copyright (C) 2011-2024 Shyue Ping Ong and the pymatgen Development Team
 # pymatgen is released under the MIT License.
 
 # See also abipy/tools/plotting.py.
 # Copyright (C) 2021 Matteo Giantomassi and the AbiPy Group
@@ -11,49 +11,56 @@
 
 """Functions related to plotting."""
 
 from functools import wraps
 import matplotlib.pyplot as plt
 import matplotlib as mpl
 
-def my_plot_settings(name='default'):
+def plot_settings(name='default'):
     mpl.rc('xtick', labelsize=10, direction='in')
     mpl.rc('ytick', labelsize=10, direction='in')
     lw = dict(default=2.0, large=4.0)[name]
     mpl.rcParams['lines.linewidth'] = lw
     mpl.rcParams['lines.markersize'] = 3
     mpl.rcParams['xtick.major.size'] = 4
     mpl.rcParams['xtick.minor.size'] = 2
     mpl.rcParams['xtick.major.width'] = 0.8
     mpl.rcParams.update({'font.size': 16})
 
-
 def get_ax_fig_plt(ax=None, **kwargs):
-    r"""Helper function used in plot functions supporting an optional Axes
-    argument. If ax is None, we build the `matplotlib` figure and create the
-    Axes else. We return the current active figure.
-
-    Args:
-        ax (Axes, optional): Axes object. Defaults to None.
-        kwargs: keyword arguments are passed to plt.figure if ax is not None.
-
-      Returns:
-        ax: :class:`Axes` object
-        figure: matplotlib figure
-        plt: matplotlib pyplot module.
+    r"""Helper function used in plot functions supporting an optional `Axes`
+    argument.
+
+    If `ax` is `None`, we build the `matplotlib` figure and create the `Axes`.
+    Else we return the current active figure.
+
+    Parameters
+    ----------
+    ax : object
+        `Axes` object. Defaults to `None`.
+    **kwargs
+        Keyword arguments are passed to `plt.figure` if `ax` is not `None`.
+
+    Returns
+    -------
+    ax : object
+        `Axes` object.
+    figure : object
+        `matplotlib` figure.
+    plt : object
+        `matplotlib.pyplot` module.
     """
     if ax is None:
         fig = plt.figure(**kwargs)
         ax = fig.gca()
     else:
         fig = plt.gcf()
 
     return ax, fig, plt
 
-
 def add_fig_kwargs(func):
     """Decorator that adds keyword arguments for functions returning matplotlib
     figures.
 
     The function should return either a matplotlib figure or None to signal
     some sort of error/unexpected event.
     """
@@ -111,26 +118,31 @@
         if fig_close:
             plt.close(fig=fig)
 
         return fig
 
     # Add docstring to the decorated method.
     doc_str = """\n\n
+
+        notes
+        -----
+
         Keyword arguments controlling the display of the figure:
 
         ================  ====================================================
         kwargs            Meaning
         ================  ====================================================
         title             Title of the plot (Default: None).
         show              True to show the figure (default: True).
         savefig           "abc.png" or "abc.eps" to save the figure to a file.
         size_kwargs       Dictionary with options passed to fig.set_size_inches
                           e.g. size_kwargs=dict(w=3, h=4)
         tight_layout      True to call fig.tight_layout (default: False)
-        ax_grid           True (False) to add (remove) grid from all axes in fig.
+        ax_grid           True (False) to add (remove) grid from all axes in
+                          fig.
                           Default: None i.e. fig is left unchanged.
         ax_annotate       Add labels to  subplots e.g. (a), (b).
                           Default: False
         fig_close         Close figure. Default: False.
         ================  ====================================================
 
 """
@@ -138,8 +150,8 @@
     if wrapper.__doc__ is not None:
         # Add s at the end of the docstring.
         wrapper.__doc__ += f'\n{doc_str}'
     else:
         # Use s
         wrapper.__doc__ = doc_str
 
-    return wrapper
+    return wrapper
```

### Comparing `xarpes-0.1.0/PKG-INFO` & `xarpes-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: xarpes
-Version: 0.1.0
+Version: 0.2.0
 Summary: Extraction from angle resolved photoemission spectra
 Author: xARPES Developers
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: igor2
 Requires-Dist: jupyterlab
 Requires-Dist: jupytext
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy
+Requires-Dist: lmfit
 Project-URL: Documentation, https://xarpes.github.io
 
 ![xARPES](https://xarpes.github.io/_images/xarpes.svg)
 
 Repository for the code xARPES &ndash; extraction from angle resolved photoemission spectra.
 
 This preliminary release can only be used to fit a Fermi edge. The complete functionality will be made available soon.
@@ -93,14 +94,20 @@
 	cd xARPES
 	conda create -n <my_env> -c defaults -c conda-forge --file requirements.txt
 	conda activate <my_env>
 	conda develop .
 
 Answer `y` to questions.
 
+# Examples
+
+Afer installation of xARPES, the `examples/` folder can be downloaded to the current directory with
+
+    python3 -c "import xarpes; xarpes.download_examples()"
+
 # Execution
 
 It is recommended to use JupyterLab to analyse data. JupyterLab is launched using:
 
 	jupyter lab
 
 # License
```

