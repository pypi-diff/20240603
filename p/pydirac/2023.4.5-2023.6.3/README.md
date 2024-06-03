# Comparing `tmp/pydirac-2023.4.5.tar.gz` & `tmp/pydirac-2023.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydirac-2023.4.5.tar", last modified: Mon Jun  3 07:31:41 2024, max compression
+gzip compressed data, was "pydirac-2023.6.3.tar", last modified: Mon Jun  3 07:16:49 2024, max compression
```

## Comparing `pydirac-2023.4.5.tar` & `pydirac-2023.6.3.tar`

### file list

```diff
@@ -1,282 +1,282 @@
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.084421 pydirac-2023.4.5/
--rw-r--r--   0 yingxing   (501) staff       (20)    35149 2024-06-01 22:13:43.000000 pydirac-2023.4.5/LICENSE
--rw-r--r--   0 yingxing   (501) staff       (20)       19 2024-06-01 22:13:43.000000 pydirac-2023.4.5/MANIFEST.in
--rw-r--r--   0 yingxing   (501) staff       (20)    44500 2024-06-03 07:31:41.084220 pydirac-2023.4.5/PKG-INFO
--rw-r--r--   0 yingxing   (501) staff       (20)     2446 2024-06-01 22:13:43.000000 pydirac-2023.4.5/README.md
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.021770 pydirac-2023.4.5/examples/
--rw-r--r--   0 yingxing   (501) staff       (20)      975 2024-06-01 22:13:43.000000 pydirac-2023.4.5/examples/run_cc.py
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.022114 pydirac-2023.4.5/pydirac/
--rw-r--r--   0 yingxing   (501) staff       (20)      907 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/__init__.py
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.023723 pydirac-2023.4.5/pydirac/analysis/
--rw-r--r--   0 yingxing   (501) staff       (20)       85 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/analysis/__init__.py
--rw-r--r--   0 yingxing   (501) staff       (20)    13544 2024-06-03 07:30:54.000000 pydirac-2023.4.5/pydirac/analysis/polarizability.py
--rw-r--r--   0 yingxing   (501) staff       (20)     3836 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/analysis/utility.py
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.024104 pydirac-2023.4.5/pydirac/cli/
--rw-r--r--   0 yingxing   (501) staff       (20)       40 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/cli/__init__.py
--rw-r--r--   0 yingxing   (501) staff       (20)     3226 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/cli/pypam.py
--rw-r--r--   0 yingxing   (501) staff       (20)      398 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/cli/pypam_atom_db.py
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.025364 pydirac-2023.4.5/pydirac/core/
--rw-r--r--   0 yingxing   (501) staff       (20)      177 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/core/__init__.py
--rw-r--r--   0 yingxing   (501) staff       (20)     7154 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/core/basis.py
--rw-r--r--   0 yingxing   (501) staff       (20)     2544 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/core/molecule.py
--rw-r--r--   0 yingxing   (501) staff       (20)    16908 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/core/orbitals.py
--rw-r--r--   0 yingxing   (501) staff       (20)    14275 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/core/periodic.py
--rw-r--r--   0 yingxing   (501) staff       (20)    17664 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/core/settings.py
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.025742 pydirac-2023.4.5/pydirac/data/
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/data/__init__.py
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.026039 pydirac-2023.4.5/pydirac/data/__pycache__/
--rw-r--r--   0 yingxing   (501) staff       (20)      150 2024-06-03 07:03:23.000000 pydirac-2023.4.5/pydirac/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 yingxing   (501) staff       (20)      166 2024-06-02 08:45:01.000000 pydirac-2023.4.5/pydirac/data/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.028040 pydirac-2023.4.5/pydirac/data/basisset/
--rw-r--r--   0 yingxing   (501) staff       (20)    50979 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/data/basisset/dyall.acv3z
--rw-r--r--   0 yingxing   (501) staff       (20)    64766 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/data/basisset/dyall.acv4z
--rw-r--r--   0 yingxing   (501) staff       (20)   184658 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/data/basisset/dyall.cv3z
--rw-r--r--   0 yingxing   (501) staff       (20)   232373 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/data/basisset/dyall.cv4z
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.028515 pydirac-2023.4.5/pydirac/data/template/
--rw-r--r--   0 yingxing   (501) staff       (20)      412 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/data/template/AtomicDHFSet.yaml
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.029510 pydirac-2023.4.5/pydirac/io/
--rw-r--r--   0 yingxing   (501) staff       (20)       95 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/io/__init__.py
--rw-r--r--   0 yingxing   (501) staff       (20)    36240 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/io/inputs.py
--rw-r--r--   0 yingxing   (501) staff       (20)    20429 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/io/outputs.py
--rw-r--r--   0 yingxing   (501) staff       (20)    43301 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/io/sets.py
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.029991 pydirac-2023.4.5/pydirac/tests/
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/__init__.py
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.030294 pydirac-2023.4.5/pydirac/tests/analysis/
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/analysis/__init__.py
--rw-r--r--   0 yingxing   (501) staff       (20)      843 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/analysis/test_polarizability.py
--rw-r--r--   0 yingxing   (501) staff       (20)     3237 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/analysis/test_utility.py
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.030669 pydirac-2023.4.5/pydirac/tests/core/
--rw-r--r--   0 yingxing   (501) staff       (20)      953 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/core/__init__.py
--rw-r--r--   0 yingxing   (501) staff       (20)      307 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/core/test_basis.py
--rw-r--r--   0 yingxing   (501) staff       (20)      159 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/core/test_settings.py
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.030796 pydirac-2023.4.5/pydirac/tests/data/
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.031656 pydirac-2023.4.5/pydirac/tests/data/He_mrci/
--rw-r--r--   0 yingxing   (501) staff       (20)      454 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/He_dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/He_dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/He_dyall.acv4z_0.0000_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)    82307 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out
--rw-r--r--   0 yingxing   (501) staff       (20)      453 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/PYDIRAC.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      515 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/PYDIRAC_KRCI_VISUAL.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.032662 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/
--rw-r--r--   0 yingxing   (501) staff       (20)      453 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/He_dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/He_dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   125192 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.0005.out
--rw-r--r--   0 yingxing   (501) staff       (20)      515 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/PYDIRAC_KRCI_VISUAL.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.033334 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/
--rw-r--r--   0 yingxing   (501) staff       (20)      453 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/He_dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/He_dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   124831 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/He_dyall.acv4z_He_dyall.acv4z_zff=+0.001.out
--rw-r--r--   0 yingxing   (501) staff       (20)      515 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/PYDIRAC_KRCI_VISUAL.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.033968 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/
--rw-r--r--   0 yingxing   (501) staff       (20)      453 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/He_dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/He_dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   124617 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/He_dyall.acv4z_He_dyall.acv4z_zff=+0.002.out
--rw-r--r--   0 yingxing   (501) staff       (20)      515 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/PYDIRAC_KRCI_VISUAL.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.034772 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/
--rw-r--r--   0 yingxing   (501) staff       (20)      453 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/He_dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/He_dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   125615 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.005.out
--rw-r--r--   0 yingxing   (501) staff       (20)      515 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/PYDIRAC_KRCI_VISUAL.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.036228 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/
--rw-r--r--   0 yingxing   (501) staff       (20)      453 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/He_dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/He_dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   128056 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out
--rw-r--r--   0 yingxing   (501) staff       (20)      515 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/PYDIRAC_KRCI_VISUAL.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.036529 pydirac-2023.4.5/pydirac/tests/data/He_nr/
--rw-r--r--   0 yingxing   (501) staff       (20)      352 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/He_Ml0.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/He_dyall.acv4z.mol
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.042176 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/
--rw-r--r--   0 yingxing   (501) staff       (20)      352 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_+0.0005_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_+0.001_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_+0.002_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_+0.005_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_0.0000_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)    87652 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.0005.out
--rw-r--r--   0 yingxing   (501) staff       (20)    87794 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.001.out
--rw-r--r--   0 yingxing   (501) staff       (20)    87795 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.002.out
--rw-r--r--   0 yingxing   (501) staff       (20)    89085 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.005.out
--rw-r--r--   0 yingxing   (501) staff       (20)    88008 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/dyall.acv4z_JOB_DONE
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.044742 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/
--rw-r--r--   0 yingxing   (501) staff       (20)      477 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv3z_0.0000_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)    71124 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=0.0000.out
--rw-r--r--   0 yingxing   (501) staff       (20)      443 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv4z_0.0000_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)   103751 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out
--rw-r--r--   0 yingxing   (501) staff       (20)      477 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/PYDIRAC.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      539 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/PYDIRAC_KRCI_VISUAL.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.045386 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/
--rw-r--r--   0 yingxing   (501) staff       (20)      474 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   114677 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00001.out
--rw-r--r--   0 yingxing   (501) staff       (20)      539 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/PYDIRAC_KRCI_VISUAL.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.046111 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/
--rw-r--r--   0 yingxing   (501) staff       (20)      474 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   114616 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00002.out
--rw-r--r--   0 yingxing   (501) staff       (20)      539 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/PYDIRAC_KRCI_VISUAL.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.047189 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/
--rw-r--r--   0 yingxing   (501) staff       (20)      474 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   114650 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00001.out
--rw-r--r--   0 yingxing   (501) staff       (20)      539 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/PYDIRAC_KRCI_VISUAL.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.047813 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/
--rw-r--r--   0 yingxing   (501) staff       (20)      474 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   114616 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00002.out
--rw-r--r--   0 yingxing   (501) staff       (20)      539 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/PYDIRAC_KRCI_VISUAL.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.048897 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/
--rw-r--r--   0 yingxing   (501) staff       (20)      474 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   117085 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=0.0000.out
--rw-r--r--   0 yingxing   (501) staff       (20)      539 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/PYDIRAC_KRCI_VISUAL.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.049529 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00001/
--rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   148255 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00001.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.050930 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00002/
--rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   149186 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00002.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.051825 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00001/
--rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   147900 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00001.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.052665 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00002/
--rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   149186 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00002.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.053205 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_0.0000/
--rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   151756 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.019711 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.055109 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00001/
--rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   143179 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00001.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.055741 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00002/
--rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   143478 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00002.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.056823 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00001/
--rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   142627 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00001.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.058572 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00002/
--rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   143381 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00002.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.059306 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_0.0000/
--rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   146620 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.059851 pydirac-2023.4.5/pydirac/tests/data/He_q_so/
--rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/He_d-aug-dyall.acv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/He_d-aug-dyall.acv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/PYDIRAC.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.060243 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00001/
--rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)    80860 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00001.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.061510 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00002/
--rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)    80798 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00002.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.062035 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00001/
--rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)    80857 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00001.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.062776 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00002/
--rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)    80798 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00002.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.065237 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_0.0000/
--rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)    83666 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=0.0000.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.066376 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/
--rw-r--r--   0 yingxing   (501) staff       (20)      340 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/He_Ml0.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/He_d-aug-dyall.acv4z.mol
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.069877 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/
--rw-r--r--   0 yingxing   (501) staff       (20)      340 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_+0.00001_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_+0.00002_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_-0.00001_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_-0.00002_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_0.0000_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)    75980 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00001.out
--rw-r--r--   0 yingxing   (501) staff       (20)    76074 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00002.out
--rw-r--r--   0 yingxing   (501) staff       (20)    76074 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00001.out
--rw-r--r--   0 yingxing   (501) staff       (20)    76076 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00002.out
--rw-r--r--   0 yingxing   (501) staff       (20)    75429 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/d-aug-dyall.acv4z_JOB_DONE
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.070119 pydirac-2023.4.5/pydirac/tests/data/He_so/
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/He_dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)      303 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/PYDIRAC.inp
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.070542 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.0005/
--rw-r--r--   0 yingxing   (501) staff       (20)      303 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.0005/He_dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.0005/He_dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)    65529 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.0005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.0005.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.071739 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.001/
--rw-r--r--   0 yingxing   (501) staff       (20)      303 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.001/He_dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.001/He_dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)    65528 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.001/He_dyall.acv4z_He_dyall.acv4z_zff=+0.001.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.073103 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.002/
--rw-r--r--   0 yingxing   (501) staff       (20)      303 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.002/He_dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.002/He_dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)    65552 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.002/He_dyall.acv4z_He_dyall.acv4z_zff=+0.002.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.073871 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.005/
--rw-r--r--   0 yingxing   (501) staff       (20)      303 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.005/He_dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.005/He_dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)    65819 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.005.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.074633 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_0.0000/
--rw-r--r--   0 yingxing   (501) staff       (20)      303 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_0.0000/He_dyall.acv4z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_0.0000/He_dyall.acv4z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)    65447 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_0.0000/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.075035 pydirac-2023.4.5/pydirac/tests/data/K_mrci/
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.075571 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0005/
--rw-r--r--   0 yingxing   (501) staff       (20)      560 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0005/K_d-aug-dyall.cv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      155 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0005/K_d-aug-dyall.cv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   360077 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0005/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.0005.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.077339 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.001/
--rw-r--r--   0 yingxing   (501) staff       (20)      560 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.001/K_d-aug-dyall.cv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      155 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.001/K_d-aug-dyall.cv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   347769 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.001/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.001.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.079038 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0015/
--rw-r--r--   0 yingxing   (501) staff       (20)      560 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0015/K_d-aug-dyall.cv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      155 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0015/K_d-aug-dyall.cv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   370304 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0015/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.0015.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.080233 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.002/
--rw-r--r--   0 yingxing   (501) staff       (20)      560 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.002/K_d-aug-dyall.cv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      155 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.002/K_d-aug-dyall.cv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   372781 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.002/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.002.out
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.082497 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/
--rw-r--r--   0 yingxing   (501) staff       (20)      560 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z.inp
--rw-r--r--   0 yingxing   (501) staff       (20)      155 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z.mol
--rw-r--r--   0 yingxing   (501) staff       (20)   299392 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=0.0000.out
--rw-r--r--   0 yingxing   (501) staff       (20)    41689 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=0.0000.out.0
--rwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_SCF_JOB_DONE
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/data/__init__.py
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.083025 pydirac-2023.4.5/pydirac/tests/data/__pycache__/
--rw-r--r--   0 yingxing   (501) staff       (20)      156 2024-06-03 07:03:23.000000 pydirac-2023.4.5/pydirac/tests/data/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.083694 pydirac-2023.4.5/pydirac/tests/io/
--rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/io/__init__.py
--rw-r--r--   0 yingxing   (501) staff       (20)     3579 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/io/test_inputs.py
--rw-r--r--   0 yingxing   (501) staff       (20)     1944 2024-06-03 07:30:54.000000 pydirac-2023.4.5/pydirac/tests/io/test_outputs.py
--rw-r--r--   0 yingxing   (501) staff       (20)     2093 2024-06-01 22:13:43.000000 pydirac-2023.4.5/pydirac/tests/io/test_sets.py
-drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:31:41.083877 pydirac-2023.4.5/pydirac.egg-info/
--rw-r--r--   0 yingxing   (501) staff       (20)    44500 2024-06-03 07:31:40.000000 pydirac-2023.4.5/pydirac.egg-info/PKG-INFO
--rw-r--r--   0 yingxing   (501) staff       (20)    14538 2024-06-03 07:31:41.000000 pydirac-2023.4.5/pydirac.egg-info/SOURCES.txt
--rw-r--r--   0 yingxing   (501) staff       (20)        1 2024-06-03 07:31:40.000000 pydirac-2023.4.5/pydirac.egg-info/dependency_links.txt
--rw-r--r--   0 yingxing   (501) staff       (20)       49 2024-06-03 07:31:40.000000 pydirac-2023.4.5/pydirac.egg-info/entry_points.txt
--rw-r--r--   0 yingxing   (501) staff       (20)       44 2024-06-03 07:31:40.000000 pydirac-2023.4.5/pydirac.egg-info/requires.txt
--rw-r--r--   0 yingxing   (501) staff       (20)        8 2024-06-03 07:31:40.000000 pydirac-2023.4.5/pydirac.egg-info/top_level.txt
--rw-r--r--   0 yingxing   (501) staff       (20)     1719 2024-06-03 07:30:54.000000 pydirac-2023.4.5/pyproject.toml
--rw-r--r--   0 yingxing   (501) staff       (20)       38 2024-06-03 07:31:41.084457 pydirac-2023.4.5/setup.cfg
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.897321 pydirac-2023.6.3/
+-rw-r--r--   0 yingxing   (501) staff       (20)    35149 2024-06-01 22:13:43.000000 pydirac-2023.6.3/LICENSE
+-rw-r--r--   0 yingxing   (501) staff       (20)       19 2024-06-01 22:13:43.000000 pydirac-2023.6.3/MANIFEST.in
+-rw-r--r--   0 yingxing   (501) staff       (20)    44500 2024-06-03 07:16:49.897118 pydirac-2023.6.3/PKG-INFO
+-rw-r--r--   0 yingxing   (501) staff       (20)     2446 2024-06-01 22:13:43.000000 pydirac-2023.6.3/README.md
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.829016 pydirac-2023.6.3/examples/
+-rw-r--r--   0 yingxing   (501) staff       (20)      975 2024-06-01 22:13:43.000000 pydirac-2023.6.3/examples/run_cc.py
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.829356 pydirac-2023.6.3/pydirac/
+-rw-r--r--   0 yingxing   (501) staff       (20)      907 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/__init__.py
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.831090 pydirac-2023.6.3/pydirac/analysis/
+-rw-r--r--   0 yingxing   (501) staff       (20)       85 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/analysis/__init__.py
+-rw-r--r--   0 yingxing   (501) staff       (20)    14988 2024-06-03 07:08:02.000000 pydirac-2023.6.3/pydirac/analysis/polarizability.py
+-rw-r--r--   0 yingxing   (501) staff       (20)     3836 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/analysis/utility.py
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.831503 pydirac-2023.6.3/pydirac/cli/
+-rw-r--r--   0 yingxing   (501) staff       (20)       40 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/cli/__init__.py
+-rw-r--r--   0 yingxing   (501) staff       (20)     3226 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/cli/pypam.py
+-rw-r--r--   0 yingxing   (501) staff       (20)      398 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/cli/pypam_atom_db.py
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.832927 pydirac-2023.6.3/pydirac/core/
+-rw-r--r--   0 yingxing   (501) staff       (20)      177 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/core/__init__.py
+-rw-r--r--   0 yingxing   (501) staff       (20)     7154 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/core/basis.py
+-rw-r--r--   0 yingxing   (501) staff       (20)     2544 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/core/molecule.py
+-rw-r--r--   0 yingxing   (501) staff       (20)    16908 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/core/orbitals.py
+-rw-r--r--   0 yingxing   (501) staff       (20)    14275 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/core/periodic.py
+-rw-r--r--   0 yingxing   (501) staff       (20)    17664 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/core/settings.py
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.833285 pydirac-2023.6.3/pydirac/data/
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/data/__init__.py
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.833637 pydirac-2023.6.3/pydirac/data/__pycache__/
+-rw-r--r--   0 yingxing   (501) staff       (20)      150 2024-06-03 07:03:23.000000 pydirac-2023.6.3/pydirac/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 yingxing   (501) staff       (20)      166 2024-06-02 08:45:01.000000 pydirac-2023.6.3/pydirac/data/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.835779 pydirac-2023.6.3/pydirac/data/basisset/
+-rw-r--r--   0 yingxing   (501) staff       (20)    50979 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/data/basisset/dyall.acv3z
+-rw-r--r--   0 yingxing   (501) staff       (20)    64766 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/data/basisset/dyall.acv4z
+-rw-r--r--   0 yingxing   (501) staff       (20)   184658 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/data/basisset/dyall.cv3z
+-rw-r--r--   0 yingxing   (501) staff       (20)   232373 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/data/basisset/dyall.cv4z
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.836127 pydirac-2023.6.3/pydirac/data/template/
+-rw-r--r--   0 yingxing   (501) staff       (20)      412 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/data/template/AtomicDHFSet.yaml
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.837110 pydirac-2023.6.3/pydirac/io/
+-rw-r--r--   0 yingxing   (501) staff       (20)       95 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/io/__init__.py
+-rw-r--r--   0 yingxing   (501) staff       (20)    36240 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/io/inputs.py
+-rw-r--r--   0 yingxing   (501) staff       (20)    20429 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/io/outputs.py
+-rw-r--r--   0 yingxing   (501) staff       (20)    43301 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/io/sets.py
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.837605 pydirac-2023.6.3/pydirac/tests/
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/__init__.py
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.837925 pydirac-2023.6.3/pydirac/tests/analysis/
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/analysis/__init__.py
+-rw-r--r--   0 yingxing   (501) staff       (20)      843 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/analysis/test_polarizability.py
+-rw-r--r--   0 yingxing   (501) staff       (20)     3237 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/analysis/test_utility.py
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.838310 pydirac-2023.6.3/pydirac/tests/core/
+-rw-r--r--   0 yingxing   (501) staff       (20)      953 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/core/__init__.py
+-rw-r--r--   0 yingxing   (501) staff       (20)      307 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/core/test_basis.py
+-rw-r--r--   0 yingxing   (501) staff       (20)      159 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/core/test_settings.py
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.838444 pydirac-2023.6.3/pydirac/tests/data/
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.839245 pydirac-2023.6.3/pydirac/tests/data/He_mrci/
+-rw-r--r--   0 yingxing   (501) staff       (20)      454 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/He_dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/He_dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/He_dyall.acv4z_0.0000_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)    82307 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out
+-rw-r--r--   0 yingxing   (501) staff       (20)      453 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/PYDIRAC.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      515 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/PYDIRAC_KRCI_VISUAL.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.840316 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/
+-rw-r--r--   0 yingxing   (501) staff       (20)      453 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/He_dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/He_dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   125192 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.0005.out
+-rw-r--r--   0 yingxing   (501) staff       (20)      515 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/PYDIRAC_KRCI_VISUAL.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.840999 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/
+-rw-r--r--   0 yingxing   (501) staff       (20)      453 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/He_dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/He_dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   124831 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/He_dyall.acv4z_He_dyall.acv4z_zff=+0.001.out
+-rw-r--r--   0 yingxing   (501) staff       (20)      515 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/PYDIRAC_KRCI_VISUAL.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.841780 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/
+-rw-r--r--   0 yingxing   (501) staff       (20)      453 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/He_dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/He_dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   124617 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/He_dyall.acv4z_He_dyall.acv4z_zff=+0.002.out
+-rw-r--r--   0 yingxing   (501) staff       (20)      515 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/PYDIRAC_KRCI_VISUAL.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.843898 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/
+-rw-r--r--   0 yingxing   (501) staff       (20)      453 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/He_dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/He_dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   125615 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.005.out
+-rw-r--r--   0 yingxing   (501) staff       (20)      515 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/PYDIRAC_KRCI_VISUAL.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.847016 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/
+-rw-r--r--   0 yingxing   (501) staff       (20)      453 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/He_dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/He_dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   128056 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out
+-rw-r--r--   0 yingxing   (501) staff       (20)      515 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/PYDIRAC_KRCI_VISUAL.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.847264 pydirac-2023.6.3/pydirac/tests/data/He_nr/
+-rw-r--r--   0 yingxing   (501) staff       (20)      352 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/He_Ml0.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/He_dyall.acv4z.mol
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.850934 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/
+-rw-r--r--   0 yingxing   (501) staff       (20)      352 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_+0.0005_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_+0.001_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_+0.002_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_+0.005_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_0.0000_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)    87652 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.0005.out
+-rw-r--r--   0 yingxing   (501) staff       (20)    87794 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.001.out
+-rw-r--r--   0 yingxing   (501) staff       (20)    87795 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.002.out
+-rw-r--r--   0 yingxing   (501) staff       (20)    89085 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.005.out
+-rw-r--r--   0 yingxing   (501) staff       (20)    88008 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/dyall.acv4z_JOB_DONE
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.853304 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/
+-rw-r--r--   0 yingxing   (501) staff       (20)      477 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv3z_0.0000_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)    71124 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=0.0000.out
+-rw-r--r--   0 yingxing   (501) staff       (20)      443 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv4z_0.0000_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)   103751 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out
+-rw-r--r--   0 yingxing   (501) staff       (20)      477 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/PYDIRAC.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      539 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/PYDIRAC_KRCI_VISUAL.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.854051 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/
+-rw-r--r--   0 yingxing   (501) staff       (20)      474 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   114677 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00001.out
+-rw-r--r--   0 yingxing   (501) staff       (20)      539 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/PYDIRAC_KRCI_VISUAL.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.855266 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/
+-rw-r--r--   0 yingxing   (501) staff       (20)      474 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   114616 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00002.out
+-rw-r--r--   0 yingxing   (501) staff       (20)      539 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/PYDIRAC_KRCI_VISUAL.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.856374 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/
+-rw-r--r--   0 yingxing   (501) staff       (20)      474 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   114650 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00001.out
+-rw-r--r--   0 yingxing   (501) staff       (20)      539 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/PYDIRAC_KRCI_VISUAL.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.857017 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/
+-rw-r--r--   0 yingxing   (501) staff       (20)      474 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   114616 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00002.out
+-rw-r--r--   0 yingxing   (501) staff       (20)      539 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/PYDIRAC_KRCI_VISUAL.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.858080 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/
+-rw-r--r--   0 yingxing   (501) staff       (20)      474 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   117085 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=0.0000.out
+-rw-r--r--   0 yingxing   (501) staff       (20)      539 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/PYDIRAC_KRCI_VISUAL.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.859210 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00001/
+-rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   148255 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00001.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.860416 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00002/
+-rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   149186 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00002.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.861774 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00001/
+-rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   147900 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00001.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.862791 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00002/
+-rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   149186 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00002.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.863399 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_0.0000/
+-rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   151756 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.826623 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.864334 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00001/
+-rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   143179 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00001.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.865059 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00002/
+-rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   143478 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00002.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.866242 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00001/
+-rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   142627 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00001.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.867664 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00002/
+-rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   143381 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00002.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.869169 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_0.0000/
+-rw-r--r--   0 yingxing   (501) staff       (20)      440 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   146620 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.869759 pydirac-2023.6.3/pydirac/tests/data/He_q_so/
+-rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/He_d-aug-dyall.acv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/He_d-aug-dyall.acv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/PYDIRAC.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.870314 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00001/
+-rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)    80860 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00001.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.871179 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00002/
+-rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)    80798 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00002.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.871661 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00001/
+-rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)    80857 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00001.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.872249 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00002/
+-rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)    80798 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00002.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.872888 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_0.0000/
+-rw-r--r--   0 yingxing   (501) staff       (20)      402 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)    83666 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=0.0000.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.873232 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/
+-rw-r--r--   0 yingxing   (501) staff       (20)      340 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/He_Ml0.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/He_d-aug-dyall.acv4z.mol
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.876672 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/
+-rw-r--r--   0 yingxing   (501) staff       (20)      340 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      158 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_+0.00001_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_+0.00002_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_-0.00001_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_-0.00002_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_0.0000_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)    75980 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00001.out
+-rw-r--r--   0 yingxing   (501) staff       (20)    76074 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00002.out
+-rw-r--r--   0 yingxing   (501) staff       (20)    76074 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00001.out
+-rw-r--r--   0 yingxing   (501) staff       (20)    76076 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00002.out
+-rw-r--r--   0 yingxing   (501) staff       (20)    75429 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/d-aug-dyall.acv4z_JOB_DONE
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.876897 pydirac-2023.6.3/pydirac/tests/data/He_so/
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/He_dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)      303 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/PYDIRAC.inp
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.877282 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.0005/
+-rw-r--r--   0 yingxing   (501) staff       (20)      303 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.0005/He_dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.0005/He_dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)    65529 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.0005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.0005.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.878354 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.001/
+-rw-r--r--   0 yingxing   (501) staff       (20)      303 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.001/He_dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.001/He_dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)    65528 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.001/He_dyall.acv4z_He_dyall.acv4z_zff=+0.001.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.879464 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.002/
+-rw-r--r--   0 yingxing   (501) staff       (20)      303 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.002/He_dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.002/He_dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)    65552 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.002/He_dyall.acv4z_He_dyall.acv4z_zff=+0.002.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.880619 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.005/
+-rw-r--r--   0 yingxing   (501) staff       (20)      303 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.005/He_dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.005/He_dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)    65819 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.005.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.883972 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_0.0000/
+-rw-r--r--   0 yingxing   (501) staff       (20)      303 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_0.0000/He_dyall.acv4z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      146 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_0.0000/He_dyall.acv4z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)    65447 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_0.0000/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.884377 pydirac-2023.6.3/pydirac/tests/data/K_mrci/
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.884733 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0005/
+-rw-r--r--   0 yingxing   (501) staff       (20)      560 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0005/K_d-aug-dyall.cv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      155 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0005/K_d-aug-dyall.cv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   360077 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0005/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.0005.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.887968 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.001/
+-rw-r--r--   0 yingxing   (501) staff       (20)      560 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.001/K_d-aug-dyall.cv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      155 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.001/K_d-aug-dyall.cv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   347769 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.001/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.001.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.890236 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0015/
+-rw-r--r--   0 yingxing   (501) staff       (20)      560 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0015/K_d-aug-dyall.cv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      155 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0015/K_d-aug-dyall.cv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   370304 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0015/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.0015.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.891761 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.002/
+-rw-r--r--   0 yingxing   (501) staff       (20)      560 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.002/K_d-aug-dyall.cv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      155 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.002/K_d-aug-dyall.cv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   372781 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.002/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.002.out
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.894778 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/
+-rw-r--r--   0 yingxing   (501) staff       (20)      560 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z.inp
+-rw-r--r--   0 yingxing   (501) staff       (20)      155 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z.mol
+-rw-r--r--   0 yingxing   (501) staff       (20)   299392 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=0.0000.out
+-rw-r--r--   0 yingxing   (501) staff       (20)    41689 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=0.0000.out.0
+-rwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_SCF_JOB_DONE
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/data/__init__.py
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.895309 pydirac-2023.6.3/pydirac/tests/data/__pycache__/
+-rw-r--r--   0 yingxing   (501) staff       (20)      156 2024-06-03 07:03:23.000000 pydirac-2023.6.3/pydirac/tests/data/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.896220 pydirac-2023.6.3/pydirac/tests/io/
+-rw-r--r--   0 yingxing   (501) staff       (20)        0 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/io/__init__.py
+-rw-r--r--   0 yingxing   (501) staff       (20)     3579 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/io/test_inputs.py
+-rw-r--r--   0 yingxing   (501) staff       (20)     1956 2024-06-03 07:07:05.000000 pydirac-2023.6.3/pydirac/tests/io/test_outputs.py
+-rw-r--r--   0 yingxing   (501) staff       (20)     2093 2024-06-01 22:13:43.000000 pydirac-2023.6.3/pydirac/tests/io/test_sets.py
+drwxr-xr-x   0 yingxing   (501) staff       (20)        0 2024-06-03 07:16:49.896691 pydirac-2023.6.3/pydirac.egg-info/
+-rw-r--r--   0 yingxing   (501) staff       (20)    44500 2024-06-03 07:16:49.000000 pydirac-2023.6.3/pydirac.egg-info/PKG-INFO
+-rw-r--r--   0 yingxing   (501) staff       (20)    14538 2024-06-03 07:16:49.000000 pydirac-2023.6.3/pydirac.egg-info/SOURCES.txt
+-rw-r--r--   0 yingxing   (501) staff       (20)        1 2024-06-03 07:16:49.000000 pydirac-2023.6.3/pydirac.egg-info/dependency_links.txt
+-rw-r--r--   0 yingxing   (501) staff       (20)       49 2024-06-03 07:16:49.000000 pydirac-2023.6.3/pydirac.egg-info/entry_points.txt
+-rw-r--r--   0 yingxing   (501) staff       (20)       44 2024-06-03 07:16:49.000000 pydirac-2023.6.3/pydirac.egg-info/requires.txt
+-rw-r--r--   0 yingxing   (501) staff       (20)        8 2024-06-03 07:16:49.000000 pydirac-2023.6.3/pydirac.egg-info/top_level.txt
+-rw-r--r--   0 yingxing   (501) staff       (20)     1719 2024-06-03 07:15:19.000000 pydirac-2023.6.3/pyproject.toml
+-rw-r--r--   0 yingxing   (501) staff       (20)       38 2024-06-03 07:16:49.897472 pydirac-2023.6.3/setup.cfg
```

### Comparing `pydirac-2023.4.5/LICENSE` & `pydirac-2023.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/PKG-INFO` & `pydirac-2023.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydirac
-Version: 2023.4.5
+Version: 2023.6.3
 Summary: This tool provides a convenient solution for managing input and output files when using the DIRAC program for computational chemistry. With this tool, users can easily generate properly formatted input files and parse the output files to extract relevant information. It is designed to streamline the process of preparing input files and handling the output generated by DIRAC, saving users time and reducing the potential for errors.
 Author-email: YingXing Cheng <yingxing.cheng@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pydirac-2023.4.5/README.md` & `pydirac-2023.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/examples/run_cc.py` & `pydirac-2023.6.3/examples/run_cc.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/__init__.py` & `pydirac-2023.6.3/pydirac/__init__.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/analysis/polarizability.py` & `pydirac-2023.6.3/pydirac/analysis/polarizability.py`

 * *Files 8% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             The matrix A for the given electric field strengths.
         """
         A = np.zeros((len(field), self.nb_coeffs))
         for i, v in enumerate(field):
             A[i, :] = self.get_coeff(v)
         return A
 
-    def get_svd_from_array(self, energy, field):
+    def get_svd_from_array(self, energy, field, rcond=None):
         """
         Calculate the SVD-based solution for the least-squares problem.
 
         Parameters
         ----------
         energy : array_like of float
             The energy values.
@@ -157,46 +157,70 @@
             if np.isclose(f, 0.0):
                 e_ref = e
 
         # define a matrix
         A = self.get_A(np.asarray(field))
         b = np.asarray(energy) - e_ref
 
-        x_svd = np.linalg.lstsq(A, b, rcond=1e-8)[0]
-        return x_svd
-
-    def get_res_svd(self, filename):
-        """
-        Calculate the SVD-based solution for the least-squares problem using the data from a file.
-
-        Parameters
-        ----------
-        filename : str
-            The name of the file containing the electric field strengths and energy values.
-
-        Returns
-        -------
-        array_like of float
-            The coefficients.
-        """
-        with open(filename) as f:
-            context = f.readlines()
-
-        if len(context) < 3:
-            raise ValueError(f"Data points in {filename} is less than 3")
-
-        filed_energy = [tuple(c.split()) for c in context]
-        energy, field = [], []
-        for f, e in filed_energy:
-            f = float(f)
-            energy.append(float(e))
-            field.append(f)
+        # x_svd = np.linalg.lstsq(A, b, rcond=1e-8)[0]
+        # x_svd = np.linalg.lstsq(A, b, rcond=None)[0]
+        # print(x_svd)
+
+        # Solve the least squares problem using SVD
+        x_svd, residuals, rank, s = np.linalg.lstsq(A, b, rcond=rcond)
+
+        # Manually calculate residuals if not provided by np.linalg.lstsq
+        if residuals.size == 0:
+            residuals = b - np.dot(A, x_svd)
+            residual_sum_of_squares = np.sum(residuals**2)
+        else:
+            residual_sum_of_squares = residuals[0]
+            # residuals2 = b - np.dot(A, x_svd)
+            # residual_sum_of_squares2 = np.sum(residuals2**2)
+            # assert np.allclose(residual_sum_of_squares, residual_sum_of_squares2)
+            # print("assert True")
+
+        # Calculate the covariance matrix of the coefficients
+        # Assuming homoscedasticity (constant variance of residuals)
+        MSE = residual_sum_of_squares / (len(energy) - len(x_svd))  # Mean Squared Error
+        cov_matrix = np.linalg.inv(np.dot(A.T, A)) * MSE
+
+        # Standard errors are the square roots of the diagonal elements of the covariance matrix
+        standard_errors = np.sqrt(np.diag(cov_matrix))
+        return x_svd, standard_errors
+
+    # def get_res_svd(self, filename):
+    #     """
+    #     Calculate the SVD-based solution for the least-squares problem using the data from a file.
+
+    #     Parameters
+    #     ----------
+    #     filename : str
+    #         The name of the file containing the electric field strengths and energy values.
+
+    #     Returns
+    #     -------
+    #     array_like of float
+    #         The coefficients.
+    #     """
+    #     with open(filename) as f:
+    #         context = f.readlines()
+
+    #     if len(context) < 3:
+    #         raise ValueError(f"Data points in {filename} is less than 3")
+
+    #     filed_energy = [tuple(c.split()) for c in context]
+    #     energy, field = [], []
+    #     for f, e in filed_energy:
+    #         f = float(f)
+    #         energy.append(float(e))
+    #         field.append(f)
 
-        x_svd = self.get_svd_from_array(energy, field)
-        return x_svd
+    #     x_svd = self.get_svd_from_array(energy, field)
+    #     return x_svd
 
 
 def get_polarizability(
     dirname: str = "./", calc_dir_patters=None, deepth: int = 0, verbos=False
 ) -> dict:
     """Get polarizability from a directory
 
@@ -279,15 +303,17 @@
             )
             all_res["calc_dir"] = e_dict
 
         # Step 3. deal with all sub_dir
         # ------------------------------
         all_res["sub_dir"] = {}
         if do_sub_dir:
-            sub_dirs = [d for d in glob.glob("*") if os.path.isdir(d) and d not in clc_dirs]
+            sub_dirs = [
+                d for d in glob.glob("*") if os.path.isdir(d) and d not in clc_dirs
+            ]
 
             for sd in sub_dirs:
                 res = get_polarizability(
                     os.path.join(dirname, sd),
                     calc_dir_patters,
                     deepth - 1,
                     verbos=verbos,
@@ -327,15 +353,15 @@
                 if k not in energies.keys():
                     energies[k] = []
                 energies[k].append(v)
 
         elif o.inp.calc_method == "CI":
             # check all roots converged
             for i in o.energy_settings["ci_converged"]:
-                if not np.alltrue(np.asarray(i)):
+                if not np.all(np.asarray(i)):
                     raise RuntimeError("Not all roots are converged!")
 
             for k, v in o.energy_settings["ci_e"].items():
                 if k not in energies.keys():
                     energies[k] = []
                 energies[k].append(v)
 
@@ -356,26 +382,35 @@
             )
             del_k_lis.append(k)
     for k in del_k_lis:
         energies.pop(k)
 
     # {'scf': alpha_scf, 'mp2':alpha_scf, 'ccsd':alpha_ccsd}
     res = {}
+    res_error = {}
     for k, energy in energies.items():
         polar_key = k.strip("_e")
-        res[polar_key] = pc.get_svd_from_array(energy, fields)
-    res_all = {"energy": {"energies": energies, "fields": fields}, "polar": res}
+        _polar, _error = pc.get_svd_from_array(energy, fields)
+        res[polar_key] = _polar
+        res_error[polar_key] = _error
+    res_all = {
+        "energy": {"energies": energies, "fields": fields},
+        "polar": res,
+        "polar_error": res_error,
+    }
     return res_all
 
 
 def get_polarizability_from_output_list(dirname, output_lis, tag=None, verbos=True):
     all_basis_res = {}
     for o in output_lis:
         task_type, orbit = o.task_type, o.calc_orbit
-        obt_info = get_orbital_info(orbit["occ"], orbit["vir"]) if len(orbit) else "null"
+        obt_info = (
+            get_orbital_info(orbit["occ"], orbit["vir"]) if len(orbit) else "null"
+        )
         k = get_keyword(o.mol.molecule.atomic_info.symbol, task_type, obt_info)
         if k not in all_basis_res:
             all_basis_res[k] = []
         all_basis_res[k].append(o)
 
     e_res = {}
     for k, v in all_basis_res.items():
@@ -410,9 +445,11 @@
                 task_record[o.task_type] += 1
     for v in task_record.values():
         if v >= 3:
             return True
     else:
         if verbos:
             print(task_record)
-            warnings.warn("the maximum of output objects with the same type is less than 3")
+            warnings.warn(
+                "the maximum of output objects with the same type is less than 3"
+            )
         return False
```

### Comparing `pydirac-2023.4.5/pydirac/analysis/utility.py` & `pydirac-2023.6.3/pydirac/analysis/utility.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/cli/pypam.py` & `pydirac-2023.6.3/pydirac/cli/pypam.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/core/basis.py` & `pydirac-2023.6.3/pydirac/core/basis.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/core/molecule.py` & `pydirac-2023.6.3/pydirac/core/molecule.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/core/orbitals.py` & `pydirac-2023.6.3/pydirac/core/orbitals.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/core/periodic.py` & `pydirac-2023.6.3/pydirac/core/periodic.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/core/settings.py` & `pydirac-2023.6.3/pydirac/core/settings.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/data/basisset/dyall.acv3z` & `pydirac-2023.6.3/pydirac/data/basisset/dyall.acv3z`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/data/basisset/dyall.acv4z` & `pydirac-2023.6.3/pydirac/data/basisset/dyall.acv4z`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/data/basisset/dyall.cv3z` & `pydirac-2023.6.3/pydirac/data/basisset/dyall.cv3z`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/data/basisset/dyall.cv4z` & `pydirac-2023.6.3/pydirac/data/basisset/dyall.cv4z`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/io/inputs.py` & `pydirac-2023.6.3/pydirac/io/inputs.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/io/outputs.py` & `pydirac-2023.6.3/pydirac/io/outputs.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/io/sets.py` & `pydirac-2023.6.3/pydirac/io/sets.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/analysis/test_polarizability.py` & `pydirac-2023.6.3/pydirac/tests/analysis/test_polarizability.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/analysis/test_utility.py` & `pydirac-2023.6.3/pydirac/tests/analysis/test_utility.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/core/__init__.py` & `pydirac-2023.6.3/pydirac/tests/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_mrci/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out` & `pydirac-2023.6.3/pydirac/tests/data/He_mrci/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_mrci/PYDIRAC_KRCI_VISUAL.inp` & `pydirac-2023.6.3/pydirac/tests/data/He_mrci/PYDIRAC_KRCI_VISUAL.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.0005.out` & `pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.0005.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/PYDIRAC_KRCI_VISUAL.inp` & `pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.0005/PYDIRAC_KRCI_VISUAL.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/He_dyall.acv4z_He_dyall.acv4z_zff=+0.001.out` & `pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/He_dyall.acv4z_He_dyall.acv4z_zff=+0.001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/PYDIRAC_KRCI_VISUAL.inp` & `pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.001/PYDIRAC_KRCI_VISUAL.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/He_dyall.acv4z_He_dyall.acv4z_zff=+0.002.out` & `pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/He_dyall.acv4z_He_dyall.acv4z_zff=+0.002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/PYDIRAC_KRCI_VISUAL.inp` & `pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.002/PYDIRAC_KRCI_VISUAL.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.005.out` & `pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.005.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/PYDIRAC_KRCI_VISUAL.inp` & `pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_+0.005/PYDIRAC_KRCI_VISUAL.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out` & `pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/PYDIRAC_KRCI_VISUAL.inp` & `pydirac-2023.6.3/pydirac/tests/data/He_mrci/dyall.acv4z_0.0000/PYDIRAC_KRCI_VISUAL.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.0005.out` & `pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.0005.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.001.out` & `pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.002.out` & `pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.005.out` & `pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=+0.005.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out` & `pydirac-2023.6.3/pydirac/tests/data/He_nr/Ml0/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=0.0000.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=0.0000.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/PYDIRAC_KRCI_VISUAL.inp` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/PYDIRAC_KRCI_VISUAL.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00001.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/PYDIRAC_KRCI_VISUAL.inp` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00001/PYDIRAC_KRCI_VISUAL.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00002.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/PYDIRAC_KRCI_VISUAL.inp` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_+0.00002/PYDIRAC_KRCI_VISUAL.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00001.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/PYDIRAC_KRCI_VISUAL.inp` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00001/PYDIRAC_KRCI_VISUAL.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00002.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/PYDIRAC_KRCI_VISUAL.inp` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_-0.00002/PYDIRAC_KRCI_VISUAL.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=0.0000.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=0.0000.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/PYDIRAC_KRCI_VISUAL.inp` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv3z_0.0000/PYDIRAC_KRCI_VISUAL.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00001.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00002.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00001.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00002.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00001.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00002.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_+0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00001.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00001/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00002.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_-0.00002/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_mrci/old_code/d-aug-dyall.acv4z_0.0000/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00001.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00002.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_+0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00001.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00001/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00002.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_-0.00002/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=-0.00002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=0.0000.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_so/d-aug-dyall.acv3z_0.0000/He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=0.0000.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00001.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00002.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=+0.00002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00001.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00002.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=-0.00002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out` & `pydirac-2023.6.3/pydirac/tests/data/He_q_theta/Ml0/He_d-aug-dyall.acv4z_He_d-aug-dyall.acv4z_zff=0.0000.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.0005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.0005.out` & `pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.0005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.0005.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.001/He_dyall.acv4z_He_dyall.acv4z_zff=+0.001.out` & `pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.001/He_dyall.acv4z_He_dyall.acv4z_zff=+0.001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.002/He_dyall.acv4z_He_dyall.acv4z_zff=+0.002.out` & `pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.002/He_dyall.acv4z_He_dyall.acv4z_zff=+0.002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_+0.005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.005.out` & `pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_+0.005/He_dyall.acv4z_He_dyall.acv4z_zff=+0.005.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/He_so/dyall.acv4z_0.0000/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out` & `pydirac-2023.6.3/pydirac/tests/data/He_so/dyall.acv4z_0.0000/He_dyall.acv4z_He_dyall.acv4z_zff=0.0000.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0005/K_d-aug-dyall.cv3z.inp` & `pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0005/K_d-aug-dyall.cv3z.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0005/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.0005.out` & `pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0005/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.0005.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.001/K_d-aug-dyall.cv3z.inp` & `pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.001/K_d-aug-dyall.cv3z.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.001/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.001.out` & `pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.001/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.001.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0015/K_d-aug-dyall.cv3z.inp` & `pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0015/K_d-aug-dyall.cv3z.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0015/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.0015.out` & `pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.0015/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.0015.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.002/K_d-aug-dyall.cv3z.inp` & `pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.002/K_d-aug-dyall.cv3z.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.002/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.002.out` & `pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_+0.002/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=+0.002.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z.inp` & `pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z.inp`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=0.0000.out` & `pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=0.0000.out`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=0.0000.out.0` & `pydirac-2023.6.3/pydirac/tests/data/K_mrci/d-aug-dyall.cv3z_0.0000/K_d-aug-dyall.cv3z_K_d-aug-dyall.cv3z_zff=0.0000.out.0`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/io/test_inputs.py` & `pydirac-2023.6.3/pydirac/tests/io/test_inputs.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac/tests/io/test_outputs.py` & `pydirac-2023.6.3/pydirac/tests/io/test_outputs.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,23 +29,23 @@
         data_root
         / "He_q_so"
         / "d-aug-dyall.acv3z_+0.00001"
         / "He_d-aug-dyall.acv3z_He_d-aug-dyall.acv3z_zff=+0.00001.out"
     )
     o = Output(out_fn)
     res = o.as_dict()
-    assert pytest.approx(res["energy_settings"]["scf_e"], -2.861794767985585)
-    assert pytest.approx(res["energy_settings"]["mp2_e"], -2.895006044817857)
-    assert pytest.approx(res["energy_settings"]["ccsd_e"], -2.900862077849925)
-    assert pytest.approx(res["energy_settings"]["ccsd(t)_e"], -2.900862077849925)
+    assert res["energy_settings"]["scf_e"] == pytest.approx(-2.861794767985585)
+    assert res["energy_settings"]["mp2_e"] == pytest.approx(-2.895006044817857)
+    assert res["energy_settings"]["ccsd_e"] == pytest.approx(-2.900862077849925)
+    assert res["energy_settings"]["ccsd(t)_e"] == pytest.approx(-2.900862077849925)
     assert res["task_type"] == "Q-4C-DC-CC@d-aug-dyall.acv3z"
 
 
 def test_mrci():
     out_fn = str(
         data_root / "He_mrci" / "dyall.acv4z_+0.001/He_dyall.acv4z_He_dyall.acv4z_zff=+0.001.out"
     )
     o = Output(out_fn)
     res = o.as_dict()
-    assert pytest.approx(res["energy_settings"]["scf_e"], -2.8618113380597565)
-    assert pytest.approx(res["energy_settings"]["ci_e"]["sym_1_root_1"], -2.8975548136776)
+    assert res["energy_settings"]["scf_e"] == pytest.approx(-2.8618113380597565)
+    assert res["energy_settings"]["ci_e"]["sym_1_root_1"] == pytest.approx(-2.8975548136776)
     assert res["task_type"] == "D-4C-DC-CI@dyall.acv4z"
```

### Comparing `pydirac-2023.4.5/pydirac/tests/io/test_sets.py` & `pydirac-2023.6.3/pydirac/tests/io/test_sets.py`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pydirac.egg-info/PKG-INFO` & `pydirac-2023.6.3/pydirac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydirac
-Version: 2023.4.5
+Version: 2023.6.3
 Summary: This tool provides a convenient solution for managing input and output files when using the DIRAC program for computational chemistry. With this tool, users can easily generate properly formatted input files and parse the output files to extract relevant information. It is designed to streamline the process of preparing input files and handling the output generated by DIRAC, saving users time and reducing the potential for errors.
 Author-email: YingXing Cheng <yingxing.cheng@ugent.be>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pydirac-2023.4.5/pydirac.egg-info/SOURCES.txt` & `pydirac-2023.6.3/pydirac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydirac-2023.4.5/pyproject.toml` & `pydirac-2023.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pydirac"
-version = "2023.4.5"
+version = "2023.6.3"
 authors = [
   { name="YingXing Cheng", email="yingxing.cheng@ugent.be" },
 ]
 description = "This tool provides a convenient solution for managing input and output files when using the DIRAC program for computational chemistry. With this tool, users can easily generate properly formatted input files and parse the output files to extract relevant information. It is designed to streamline the process of preparing input files and handling the output generated by DIRAC, saving users time and reducing the potential for errors."
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.6"
```

