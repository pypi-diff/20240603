# Comparing `tmp/mat3ra_made-2024.5.9.post0.tar.gz` & `tmp/mat3ra_made-2024.6.3.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mat3ra_made-2024.5.9.post0.tar", last modified: Thu May  9 17:49:17 2024, max compression
+gzip compressed data, was "mat3ra_made-2024.6.3.post0.tar", last modified: Mon Jun  3 04:40:58 2024, max compression
```

## Comparing `mat3ra_made-2024.5.9.post0.tar` & `mat3ra_made-2024.6.3.post0.tar`

### file list

```diff
@@ -1,168 +1,182 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.824788 mat3ra_made-2024.5.9.post0/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.babelrc
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.eslintrc.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.796788 mat3ra_made-2024.5.9.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.800788 mat3ra_made-2024.5.9.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.800788 mat3ra_made-2024.5.9.post0/.husky/
--rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.husky/post-checkout
--rwxr-xr-x   0 runner    (1001) docker     (127)      347 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.husky/post-commit
--rwxr-xr-x   0 runner    (1001) docker     (127)      345 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.husky/post-merge
--rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.husky/pre-commit
--rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.husky/pre-push
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.mocharc.json
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-05-09 17:49:17.824788 mat3ra_made-2024.5.9.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   373142 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 17:49:17.824788 mat3ra_made-2024.5.9.post0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.796788 mat3ra_made-2024.5.9.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/abstract/array_with_ids.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/abstract/scalar_with_id.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/basis/
--rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/basis/basis.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/basis/constrained_basis.ts
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/basis/types.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/cell/
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/cell/cell.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/cell/conventional_cell.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/cell/primitive_cell.ts
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/constants.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/constraints/constraints.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/lattice.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/lattice_bravais.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/lattice_vectors.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.804788 mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/lattice_reciprocal.js
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/paths.js
--rw-r--r--   0 runner    (1001) docker     (127)    24706 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/symmetry_points.ts
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/types.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/lattice/unit_cell.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/made.js
--rw-r--r--   0 runner    (1001) docker     (127)    13731 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/material.ts
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/math.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/js/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/cif.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/errors.js
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/espresso.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/native_format_parsers.js
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/parsers.js
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/poscar.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/xyz.ts
--rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/parsers/xyz_combinatorial_basis.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/js/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/tools/basis.js
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/tools/cell.js
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/tools/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/tools/material.js
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/tools/supercell.ts
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/tools/surface.js
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/js/types.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/py/mat3ra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/material.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.808788 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/build/
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/build/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/calculate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/modify.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.820788 mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-05-09 17:49:17.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-09 17:49:17.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:49:17.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-09 17:49:17.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 17:49:17.000000 mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.812788 mat3ra_made-2024.5.9.post0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.816788 mat3ra_made-2024.5.9.post0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/AsGe-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/C2H4-translated.json
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/C2H4.json
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/FeLiSi-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/FeO.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Ge2-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Graphene.json
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Graphene.poscar
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/H2+H-final.json
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/H2+H-image.json
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/H2+H-initial.json
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/H2O.poscar
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/LiFeSi-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Na.json
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Na4Cl4-cartesian.json
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Na4Cl4.json
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Na4Cl4.poscar
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Ni-hex.json
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Ni-hex.poscar
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/OSi-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si-hex.json
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si-hex.poscar
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si-pwscf.in
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si-slab.json
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si-supercell.json
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si.json
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si2-basis-repeated.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Si2-basis.json
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Zr1H23Zr1H1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/Zr1H23Zr1H1.poscar
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/fixtures/atomic-constraints.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.816788 mat3ra_made-2024.5.9.post0/tests/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.816788 mat3ra_made-2024.5.9.post0/tests/js/basis/
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/basis/basis.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.816788 mat3ra_made-2024.5.9.post0/tests/js/cell/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/cell/cell.js
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/cell/primitive_cell.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.816788 mat3ra_made-2024.5.9.post0/tests/js/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/constraints/constraints.js
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/enums.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.820788 mat3ra_made-2024.5.9.post0/tests/js/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice.js
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice_bravais.js
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice_reciprocal.js
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice_vectors.js
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/material.test.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.820788 mat3ra_made-2024.5.9.post0/tests/js/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/parsers/espresso.js
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/parsers/native_formats.js
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/parsers/poscar.js
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/parsers/xyz.js
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/parsers/xyz_combinatorial_basis.js
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/setup.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.820788 mat3ra_made-2024.5.9.post0/tests/js/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/tools/basis.js
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/tools/supercell.js
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/tools/surface.js
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/js/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.800788 mat3ra_made-2024.5.9.post0/tests/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:17.820788 mat3ra_made-2024.5.9.post0/tests/py/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_material.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_analyze.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_build_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_calculate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_modify.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tests/py/unit/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tsconfig-transpile.json
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-09 17:49:02.000000 mat3ra_made-2024.5.9.post0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.272470 mat3ra_made-2024.6.3.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/.eslintrc.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.244470 mat3ra_made-2024.6.3.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.252470 mat3ra_made-2024.6.3.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.252470 mat3ra_made-2024.6.3.post0/.husky/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      351 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/.husky/post-checkout
+-rwxr-xr-x   0 runner    (1001) docker     (127)      347 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/.husky/post-commit
+-rwxr-xr-x   0 runner    (1001) docker     (127)      345 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/.husky/post-merge
+-rwxr-xr-x   0 runner    (1001) docker     (127)       89 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/.husky/pre-commit
+-rwxr-xr-x   0 runner    (1001) docker     (127)      341 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/.husky/pre-push
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/.mocharc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-06-03 04:40:58.272470 mat3ra_made-2024.6.3.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   373142 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-03 04:40:58.272470 mat3ra_made-2024.6.3.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.244470 mat3ra_made-2024.6.3.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.252470 mat3ra_made-2024.6.3.post0/src/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.252470 mat3ra_made-2024.6.3.post0/src/js/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/abstract/array_with_ids.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/abstract/scalar_with_id.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.252470 mat3ra_made-2024.6.3.post0/src/js/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/basis/basis.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/basis/constrained_basis.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/basis/types.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.252470 mat3ra_made-2024.6.3.post0/src/js/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/cell/cell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/cell/conventional_cell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/cell/primitive_cell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/constants.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.252470 mat3ra_made-2024.6.3.post0/src/js/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/constraints/constraints.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.252470 mat3ra_made-2024.6.3.post0/src/js/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/lattice/lattice.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/lattice/lattice_bravais.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/lattice/lattice_vectors.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.256470 mat3ra_made-2024.6.3.post0/src/js/lattice/reciprocal/
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/lattice/reciprocal/lattice_reciprocal.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/lattice/reciprocal/paths.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24706 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/lattice/reciprocal/symmetry_points.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/lattice/types.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/lattice/unit_cell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/made.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14337 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/material.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/math.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.256470 mat3ra_made-2024.6.3.post0/src/js/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/parsers/cif.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/parsers/errors.js
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/parsers/espresso.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/parsers/native_format_parsers.js
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/parsers/parsers.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/parsers/poscar.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/parsers/xyz.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/parsers/xyz_combinatorial_basis.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.256470 mat3ra_made-2024.6.3.post0/src/js/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/tools/basis.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/tools/cell.js
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/tools/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/tools/material.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/tools/supercell.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/tools/surface.js
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/js/types.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.256470 mat3ra_made-2024.6.3.post0/src/py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.256470 mat3ra_made-2024.6.3.post0/src/py/mat3ra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.256470 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/material.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.256470 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.256470 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.260470 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8596 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/interface/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/interface/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/interface/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/interface/termination_pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/interface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.260470 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/slab/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/slab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/slab/builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/slab/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/slab/termination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/build/supercell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.268470 mat3ra_made-2024.6.3.post0/src/py/mat3ra_made.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-06-03 04:40:58.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra_made.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-06-03 04:40:58.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra_made.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-03 04:40:58.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra_made.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-06-03 04:40:58.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra_made.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-03 04:40:58.000000 mat3ra_made-2024.6.3.post0/src/py/mat3ra_made.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.260470 mat3ra_made-2024.6.3.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.264470 mat3ra_made-2024.6.3.post0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/AsGe-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/C2H4-translated.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/C2H4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/FeLiSi-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/FeO.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Ge2-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Graphene.json
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Graphene.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/H2+H-final.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/H2+H-image.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/H2+H-initial.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/H2O.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/LiFeSi-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Na.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Na4Cl4-cartesian.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Na4Cl4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Na4Cl4.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Ni-hex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Ni-hex.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/OSi-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Si-hex.json
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Si-hex.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Si-pwscf.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Si-slab.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Si-supercell.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Si.json
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Si2-basis-repeated.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Si2-basis.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Zr1H23Zr1H1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/Zr1H23Zr1H1.poscar
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/fixtures/atomic-constraints.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.264470 mat3ra_made-2024.6.3.post0/tests/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.264470 mat3ra_made-2024.6.3.post0/tests/js/basis/
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/basis/basis.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.264470 mat3ra_made-2024.6.3.post0/tests/js/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/cell/cell.js
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/cell/primitive_cell.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.264470 mat3ra_made-2024.6.3.post0/tests/js/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/constraints/constraints.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/enums.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.264470 mat3ra_made-2024.6.3.post0/tests/js/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/lattice/lattice.js
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/lattice/lattice_bravais.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/lattice/lattice_reciprocal.js
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/lattice/lattice_vectors.js
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/material.test.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.264470 mat3ra_made-2024.6.3.post0/tests/js/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/parsers/espresso.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/parsers/native_formats.js
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/parsers/poscar.js
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/parsers/xyz.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/parsers/xyz_combinatorial_basis.js
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/setup.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.268470 mat3ra_made-2024.6.3.post0/tests/js/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/tools/basis.js
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/tools/supercell.js
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/tools/surface.js
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/js/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.248470 mat3ra_made-2024.6.3.post0/tests/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:58.268470 mat3ra_made-2024.6.3.post0/tests/py/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/py/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/py/unit/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/py/unit/test_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/py/unit/test_tools_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/py/unit/test_tools_build_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/py/unit/test_tools_build_slab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/py/unit/test_tools_build_supercell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/py/unit/test_tools_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/py/unit/test_tools_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/py/unit/test_tools_modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tests/py/unit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tsconfig-transpile.json
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-03 04:40:40.000000 mat3ra_made-2024.6.3.post0/tsconfig.json
```

### Comparing `mat3ra_made-2024.5.9.post0/.github/workflows/cicd.yml` & `mat3ra_made-2024.6.3.post0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/.gitignore` & `mat3ra_made-2024.6.3.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/.pre-commit-config.yaml` & `mat3ra_made-2024.6.3.post0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/LICENSE.md` & `mat3ra_made-2024.6.3.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/PKG-INFO` & `mat3ra_made-2024.6.3.post0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-made
-Version: 2024.5.9.post0
+Version: 2024.6.3.post0
 Summary: MAterials DEfinitions and/or MAterials DEsign library.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2019 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `mat3ra_made-2024.5.9.post0/README.md` & `mat3ra_made-2024.6.3.post0/README.md`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/package-lock.json` & `mat3ra_made-2024.6.3.post0/package-lock.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/package.json` & `mat3ra_made-2024.6.3.post0/package.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/pyproject.toml` & `mat3ra_made-2024.6.3.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/abstract/array_with_ids.ts` & `mat3ra_made-2024.6.3.post0/src/js/abstract/array_with_ids.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/abstract/scalar_with_id.ts` & `mat3ra_made-2024.6.3.post0/src/js/abstract/scalar_with_id.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/basis/basis.ts` & `mat3ra_made-2024.6.3.post0/src/js/basis/basis.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/basis/constrained_basis.ts` & `mat3ra_made-2024.6.3.post0/src/js/basis/constrained_basis.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/cell/cell.ts` & `mat3ra_made-2024.6.3.post0/src/js/cell/cell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/cell/conventional_cell.ts` & `mat3ra_made-2024.6.3.post0/src/js/cell/conventional_cell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/cell/primitive_cell.ts` & `mat3ra_made-2024.6.3.post0/src/js/cell/primitive_cell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/constraints/constraints.ts` & `mat3ra_made-2024.6.3.post0/src/js/constraints/constraints.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/lattice/lattice.ts` & `mat3ra_made-2024.6.3.post0/src/js/lattice/lattice.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/lattice/lattice_bravais.ts` & `mat3ra_made-2024.6.3.post0/src/js/lattice/lattice_bravais.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/lattice/lattice_vectors.ts` & `mat3ra_made-2024.6.3.post0/src/js/lattice/lattice_vectors.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/lattice_reciprocal.js` & `mat3ra_made-2024.6.3.post0/src/js/lattice/reciprocal/lattice_reciprocal.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/paths.js` & `mat3ra_made-2024.6.3.post0/src/js/lattice/reciprocal/paths.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/lattice/reciprocal/symmetry_points.ts` & `mat3ra_made-2024.6.3.post0/src/js/lattice/reciprocal/symmetry_points.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/lattice/types.ts` & `mat3ra_made-2024.6.3.post0/src/js/lattice/types.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/lattice/unit_cell.ts` & `mat3ra_made-2024.6.3.post0/src/js/lattice/unit_cell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/made.js` & `mat3ra_made-2024.6.3.post0/src/js/made.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/material.ts` & `mat3ra_made-2024.6.3.post0/src/js/material.ts`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import { HasConsistencyChecksHasMetadataNamedDefaultableInMemoryEntity } from "@mat3ra/code/dist/js/entity";
 import { AnyObject } from "@mat3ra/code/dist/js/entity/in_memory";
-// import MaterialJSONSchemaObject from "@mat3ra/esse/dist/js/schema/material.json";
 import {
     ConsistencyCheck,
     DerivedPropertiesSchema,
     FileSourceSchema,
     InChIRepresentationSchema,
     MaterialSchema,
 } from "@mat3ra/esse/dist/js/types";
@@ -106,18 +105,18 @@
         }
 
         static get defaultConfig() {
             return defaultMaterialConfig;
         }
 
         get src() {
-            return this.prop<FileSourceSchema>("src") as FileSourceSchema;
+            return this.prop("src");
         }
 
-        set src(src: FileSourceSchema) {
+        set src(src: FileSourceSchema | undefined) {
             this.setProp("src", src);
         }
 
         updateFormula() {
             this.setProp("formula", this.Basis.formula);
             this.setProp("unitCellFormula", this.Basis.unitCellFormula);
         }
@@ -158,14 +157,21 @@
             return this.prop("formula") || this.Basis.formula;
         }
 
         get unitCellFormula(): string {
             return this.prop("unitCellFormula") || this.Basis.unitCellFormula;
         }
 
+        // should be private, but TS throws error "Property 'unsetFileProps' of exported class expression may not be private or protected"
+        unsetFileProps() {
+            this.unsetProp("src");
+            this.unsetProp("icsdId");
+            this.unsetProp("external");
+        }
+
         /**
          * @param textOrObject Basis text or JSON object.
          * @param format Format (xyz, etc.)
          * @param unitz crystal/cartesian
          */
         setBasis(textOrObject: string | BasisConfig, format?: string, unitz?: string) {
             let basis: BasisConfig | undefined;
@@ -173,14 +179,15 @@
                 case "xyz":
                     basis = parsers.xyz.toBasisConfig(textOrObject as string, unitz);
                     break;
                 default:
                     basis = textOrObject as BasisConfig;
             }
             this.setProp("basis", basis);
+            this.unsetFileProps();
             this.updateFormula();
         }
 
         setBasisConstraints(constraints: Constraint[]) {
             this.setBasis({ ...this.basis, constraints });
         }
 
@@ -205,14 +212,15 @@
 
         get lattice(): BravaisConfigProps | undefined {
             return this.prop("lattice", undefined);
         }
 
         set lattice(config: BravaisConfigProps | undefined) {
             this.setProp("lattice", config);
+            this.unsetFileProps();
         }
 
         get Lattice(): Lattice {
             return new Lattice(this.lattice);
         }
 
         /**
@@ -307,17 +315,16 @@
             return parsers.espresso.toEspressoFormat(this.toJSON());
         }
 
         /**
          * Returns material in POSCAR format. Pass `true` to ignore original poscar source and re-serialize.
          */
         getAsPOSCAR(ignoreOriginal = false, omitConstraints = false): string {
-            const { src } = this;
             // By default return original source if exists
-            if (src && src.extension === "poscar" && !ignoreOriginal) {
+            if (this.src?.extension === "poscar" && !ignoreOriginal) {
                 return this.src.text;
             }
             return parsers.poscar.toPoscar(this.toJSON(), omitConstraints);
         }
 
         /**
          * Returns a copy of the material with conventional cell constructed instead of primitive.
@@ -384,14 +391,27 @@
                         },
                     );
                 });
             }
 
             return checks;
         }
+
+        static constructMaterialFileSource(
+            fileName: string,
+            fileContent: string,
+            fileExtension: string,
+        ): FileSourceSchema {
+            return {
+                extension: fileExtension,
+                filename: fileName,
+                text: fileContent,
+                hash: CryptoJS.MD5(fileContent).toString(),
+            };
+        }
     }
 
     return MadeMaterial;
 }
 
 export const Material = MaterialMixin(
     HasConsistencyChecksHasMetadataNamedDefaultableInMemoryEntity,
```

### Comparing `mat3ra_made-2024.5.9.post0/src/js/parsers/espresso.ts` & `mat3ra_made-2024.6.3.post0/src/js/parsers/espresso.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/parsers/native_format_parsers.js` & `mat3ra_made-2024.6.3.post0/src/js/parsers/native_format_parsers.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/parsers/poscar.ts` & `mat3ra_made-2024.6.3.post0/src/js/parsers/poscar.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/parsers/xyz.ts` & `mat3ra_made-2024.6.3.post0/src/js/parsers/xyz.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/parsers/xyz_combinatorial_basis.js` & `mat3ra_made-2024.6.3.post0/src/js/parsers/xyz_combinatorial_basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/tools/basis.js` & `mat3ra_made-2024.6.3.post0/src/js/tools/basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/tools/cell.js` & `mat3ra_made-2024.6.3.post0/src/js/tools/cell.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/tools/material.js` & `mat3ra_made-2024.6.3.post0/src/js/tools/material.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/tools/supercell.ts` & `mat3ra_made-2024.6.3.post0/src/js/tools/supercell.ts`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/js/tools/surface.js` & `mat3ra_made-2024.6.3.post0/src/js/tools/surface.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/material.py` & `mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/material.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/analyze.py` & `mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/analyze.py`

 * *Files 16% similar despite different names*

```diff
@@ -51,7 +51,21 @@
 
     Returns:
         float: The surface area of the atoms.
     """
     matrix = atoms.cell
     cross_product = np.cross(matrix[0], matrix[1])
     return np.linalg.norm(cross_product)
+
+
+@decorator_convert_material_args_kwargs_to_atoms
+def get_chemical_formula(atoms: Atoms):
+    """
+    Calculate the formula of the atoms structure.
+
+    Args:
+        atoms (ase.Atoms): The Atoms object to calculate the formula of.
+
+    Returns:
+        str: The formula of the atoms.
+    """
+    return atoms.get_chemical_formula()
```

### Comparing `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/calculate.py` & `mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/calculate.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/convert.py` & `mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/convert.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 import inspect
+import json
 from functools import wraps
 from typing import Any, Callable, Dict, Union
 
 from ase import Atoms
-from mat3ra.made.material import Material
 from mat3ra.utils.mixins import RoundNumericValuesMixin
+from mat3ra.utils.object import NumpyNDArrayRoundEncoder
+from pymatgen.core.interface import Interface, label_termination
 from pymatgen.core.structure import Lattice, Structure
+from pymatgen.core.surface import Slab
 from pymatgen.io.ase import AseAtomsAdaptor
 from pymatgen.io.vasp.inputs import Poscar
 
+from ..material import Material
+
+PymatgenStructure = Structure
+PymatgenSlab = Slab
+PymatgenInterface = Interface
+ASEAtoms = Atoms
+label_pymatgen_slab_termination = label_termination
+
 
 def to_pymatgen(material_or_material_data: Union[Material, Dict[str, Any]]) -> Structure:
     """
     Converts material object in ESSE format to a pymatgen Structure object.
 
     Args:
         material_or_material_data (dict|class): A dictionary containing the material information in ESSE format.
@@ -48,15 +59,15 @@
         # Passing labels does not work for pymatgen `2023.6.23` supporting py3.8
         print(f"labels: {labels}. Not passing labels to pymatgen.")
         structure = Structure(lattice, elements, coordinates, coords_are_cartesian=coords_are_cartesian)
 
     return structure
 
 
-def from_pymatgen(structure: Structure):
+def from_pymatgen(structure: Union[Structure, Interface]) -> Dict[str, Any]:
     """
     Converts a pymatgen Structure object to a material object in ESSE format.
 
     Args:
         structure (Structure): A pymatgen Structure object.
 
     Returns:
@@ -87,21 +98,34 @@
             "b": __round__(structure.lattice.matrix[1].tolist()),
             "c": __round__(structure.lattice.matrix[2].tolist()),
             "alat": 1,
             "units": "angstrom",
         },
     }
 
+    metadata = {"boundaryConditions": {"type": "pbc", "offset": 0}}
+
+    # TODO: consider using Interface JSONSchema from ESSE when such created and adapt interface_properties accordingly.
+    # Add interface properties to metadata according to pymatgen Interface as a JSON object
+    if hasattr(structure, "interface_properties"):
+        interface_props = structure.interface_properties
+        # TODO: figure out how to round the values and stringify terminations tuple
+        #  in the interface properties with Encoder
+        for key, value in interface_props.items():
+            if isinstance(value, tuple):
+                interface_props[key] = str(value)
+        metadata["interface_properties"] = json.loads(json.dumps(interface_props, cls=NumpyNDArrayRoundEncoder))
+
     material_data = {
         "name": structure.formula,
         "basis": basis,
         "lattice": lattice,
         "isNonPeriodic": not structure.is_ordered,
         "_id": "",
-        "metadata": {"boundaryConditions": {"type": "pbc", "offset": 0}},
+        "metadata": metadata,
         "isUpdated": True,
     }
 
     return material_data
 
 
 def to_poscar(material_or_material_data: Union[Material, Dict[str, Any]]) -> str:
```

### Comparing `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/modify.py` & `mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/modify.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/src/py/mat3ra/made/tools/utils.py` & `mat3ra_made-2024.6.3.post0/src/py/mat3ra/made/tools/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from functools import wraps
+from typing import Callable
+
+from mat3ra.utils.matrix import convert_2x2_to_3x3
 from pymatgen.core.structure import Structure
 
 
 # TODO: convert to accept ASE Atoms object
 def translate_to_bottom_pymatgen_structure(structure: Structure):
     """
     Translate the structure to the bottom of the cell.
@@ -13,7 +17,20 @@
     """
     min_c = min(site.c for site in structure)
     translation_vector = [0, 0, -min_c]
     translated_structure = structure.copy()
     for site in translated_structure:
         site.coords += translation_vector
     return translated_structure
+
+
+def decorator_convert_2x2_to_3x3(func: Callable) -> Callable:
+    """
+    Decorator to convert a 2x2 matrix to a 3x3 matrix.
+    """
+
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+        new_args = [convert_2x2_to_3x3(arg) if isinstance(arg, list) and len(arg) == 2 else arg for arg in args]
+        return func(*new_args, **kwargs)
+
+    return wrapper
```

### Comparing `mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/PKG-INFO` & `mat3ra_made-2024.6.3.post0/src/py/mat3ra_made.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mat3ra-made
-Version: 2024.5.9.post0
+Version: 2024.6.3.post0
 Summary: MAterials DEfinitions and/or MAterials DEsign library.
 Author-email: "Exabyte Inc." <info@mat3ra.com>
 License: # LICENSE
         
         Copyright 2019 Exabyte Inc.
         
         Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `mat3ra_made-2024.5.9.post0/src/py/mat3ra_made.egg-info/SOURCES.txt` & `mat3ra_made-2024.6.3.post0/src/py/mat3ra_made.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -36,19 +36,19 @@
 src/js/lattice/lattice_bravais.ts
 src/js/lattice/lattice_vectors.ts
 src/js/lattice/types.ts
 src/js/lattice/unit_cell.ts
 src/js/lattice/reciprocal/lattice_reciprocal.js
 src/js/lattice/reciprocal/paths.js
 src/js/lattice/reciprocal/symmetry_points.ts
-src/js/parsers/cif.js
+src/js/parsers/cif.ts
 src/js/parsers/errors.js
 src/js/parsers/espresso.ts
 src/js/parsers/native_format_parsers.js
-src/js/parsers/parsers.js
+src/js/parsers/parsers.ts
 src/js/parsers/poscar.ts
 src/js/parsers/xyz.ts
 src/js/parsers/xyz_combinatorial_basis.js
 src/js/tools/basis.js
 src/js/tools/cell.js
 src/js/tools/index.js
 src/js/tools/material.js
@@ -61,15 +61,26 @@
 src/py/mat3ra/made/tools/__init__.py
 src/py/mat3ra/made/tools/analyze.py
 src/py/mat3ra/made/tools/calculate.py
 src/py/mat3ra/made/tools/convert.py
 src/py/mat3ra/made/tools/modify.py
 src/py/mat3ra/made/tools/utils.py
 src/py/mat3ra/made/tools/build/__init__.py
-src/py/mat3ra/made/tools/build/interface.py
+src/py/mat3ra/made/tools/build/mixins.py
+src/py/mat3ra/made/tools/build/supercell.py
+src/py/mat3ra/made/tools/build/interface/__init__.py
+src/py/mat3ra/made/tools/build/interface/builders.py
+src/py/mat3ra/made/tools/build/interface/configuration.py
+src/py/mat3ra/made/tools/build/interface/enums.py
+src/py/mat3ra/made/tools/build/interface/termination_pair.py
+src/py/mat3ra/made/tools/build/interface/utils.py
+src/py/mat3ra/made/tools/build/slab/__init__.py
+src/py/mat3ra/made/tools/build/slab/builders.py
+src/py/mat3ra/made/tools/build/slab/configuration.py
+src/py/mat3ra/made/tools/build/slab/termination.py
 src/py/mat3ra_made.egg-info/PKG-INFO
 src/py/mat3ra_made.egg-info/SOURCES.txt
 src/py/mat3ra_made.egg-info/dependency_links.txt
 src/py/mat3ra_made.egg-info/requires.txt
 src/py/mat3ra_made.egg-info/top_level.txt
 tests/.gitattributes
 tests/fixtures/AsGe-basis.json
@@ -123,13 +134,14 @@
 tests/js/tools/basis.js
 tests/js/tools/supercell.js
 tests/js/tools/surface.js
 tests/py/unit/__init__.py
 tests/py/unit/fixtures.py
 tests/py/unit/test_material.py
 tests/py/unit/test_tools_analyze.py
-tests/py/unit/test_tools_build.py
 tests/py/unit/test_tools_build_interface.py
+tests/py/unit/test_tools_build_slab.py
+tests/py/unit/test_tools_build_supercell.py
 tests/py/unit/test_tools_calculate.py
 tests/py/unit/test_tools_convert.py
 tests/py/unit/test_tools_modify.py
 tests/py/unit/utils.py
```

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/C2H4-translated.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/C2H4-translated.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/C2H4.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/C2H4.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/FeO.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/FeO.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/Graphene.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/Graphene.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/H2+H-final.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/H2+H-final.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/H2+H-image.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/H2+H-image.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/H2+H-initial.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/H2+H-initial.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/Na.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/Na.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/Na4Cl4-cartesian.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/Na4Cl4-cartesian.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/Na4Cl4.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/Na4Cl4.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/Na4Cl4.poscar` & `mat3ra_made-2024.6.3.post0/tests/fixtures/Na4Cl4.poscar`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/Ni-hex.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/Ni-hex.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/Si-hex.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/Si-hex.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/Si-slab.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/Si-slab.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/Si-supercell.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/Si-supercell.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/Si.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/Si.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/Si2-basis-repeated.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/Si2-basis-repeated.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/Zr1H23Zr1H1.json` & `mat3ra_made-2024.6.3.post0/tests/fixtures/Zr1H23Zr1H1.json`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/fixtures/Zr1H23Zr1H1.poscar` & `mat3ra_made-2024.6.3.post0/tests/fixtures/Zr1H23Zr1H1.poscar`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/basis/basis.js` & `mat3ra_made-2024.6.3.post0/tests/js/basis/basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/cell/cell.js` & `mat3ra_made-2024.6.3.post0/tests/js/cell/cell.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/cell/primitive_cell.js` & `mat3ra_made-2024.6.3.post0/tests/js/cell/primitive_cell.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/constraints/constraints.js` & `mat3ra_made-2024.6.3.post0/tests/js/constraints/constraints.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/enums.js` & `mat3ra_made-2024.6.3.post0/tests/js/enums.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice.js` & `mat3ra_made-2024.6.3.post0/tests/js/lattice/lattice.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice_bravais.js` & `mat3ra_made-2024.6.3.post0/tests/js/lattice/lattice_bravais.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/lattice/lattice_reciprocal.js` & `mat3ra_made-2024.6.3.post0/tests/js/lattice/lattice_reciprocal.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/parsers/native_formats.js` & `mat3ra_made-2024.6.3.post0/tests/js/parsers/native_formats.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/parsers/poscar.js` & `mat3ra_made-2024.6.3.post0/tests/js/parsers/poscar.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/parsers/xyz.js` & `mat3ra_made-2024.6.3.post0/tests/js/parsers/xyz.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/parsers/xyz_combinatorial_basis.js` & `mat3ra_made-2024.6.3.post0/tests/js/parsers/xyz_combinatorial_basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/tools/basis.js` & `mat3ra_made-2024.6.3.post0/tests/js/tools/basis.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/js/tools/supercell.js` & `mat3ra_made-2024.6.3.post0/tests/js/tools/supercell.js`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_calculate.py` & `mat3ra_made-2024.6.3.post0/tests/py/unit/test_tools_calculate.py`

 * *Files identical despite different names*

### Comparing `mat3ra_made-2024.5.9.post0/tests/py/unit/test_tools_convert.py` & `mat3ra_made-2024.6.3.post0/tests/py/unit/test_tools_convert.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import numpy as np
 from ase import Atoms
 from ase.build import bulk
 from mat3ra.made.material import Material
 from mat3ra.made.tools.convert import from_ase, from_poscar, from_pymatgen, to_ase, to_poscar, to_pymatgen
+from mat3ra.utils import assertion as assertion_utils
 from pymatgen.core.structure import Element, Lattice, Structure
 
+from .fixtures import INTERFACE_PROPERTIES_JSON, INTERFACE_STRUCTURE
+
 PYMATGEN_LATTICE = Lattice.from_parameters(a=3.84, b=3.84, c=3.84, alpha=120, beta=90, gamma=60)
 PYMATGEN_STRUCTURE = Structure(PYMATGEN_LATTICE, ["Si", "Si"], [[0, 0, 0], [0.75, 0.5, 0.75]])
 
 POSCAR_CONTENT = """Si2
 1.0
    3.3489202364344242    0.0000000000000000    1.9335000000000004
    1.1163067454781415    3.1573922784475164    1.9335000000000004
@@ -30,14 +33,17 @@
     assert (structure.frac_coords == [[0.0, 0.0, 0.0], [0.25, 0.25, 0.25]]).all()
 
 
 def test_from_pymatgen():
     material_data = from_pymatgen(PYMATGEN_STRUCTURE)
     assert material_data["lattice"]["a"] == 3.84
     assert material_data["lattice"]["alpha"] == 120
+    interface_data = from_pymatgen(INTERFACE_STRUCTURE)
+    actual_properties = interface_data["metadata"]["interface_properties"]
+    assertion_utils.assert_deep_almost_equal(INTERFACE_PROPERTIES_JSON, actual_properties)
 
 
 def test_to_poscar():
     material = Material.create(Material.default_config)
     poscar = to_poscar(material)
     assert poscar == POSCAR_CONTENT
```

### Comparing `mat3ra_made-2024.5.9.post0/tests/py/unit/utils.py` & `mat3ra_made-2024.6.3.post0/tests/py/unit/utils.py`

 * *Files identical despite different names*

