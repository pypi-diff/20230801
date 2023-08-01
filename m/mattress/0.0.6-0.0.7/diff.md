# Comparing `tmp/mattress-0.0.6.tar.gz` & `tmp/mattress-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mattress-0.0.6.tar", last modified: Tue Aug  1 15:45:35 2023, max compression
+gzip compressed data, was "mattress-0.0.7.tar", last modified: Tue Aug  1 20:40:38 2023, max compression
```

## Comparing `mattress-0.0.6.tar` & `mattress-0.0.7.tar`

### file list

```diff
@@ -1,239 +1,239 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.493059 mattress-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-01 15:45:21.000000 mattress-0.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.465059 mattress-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.469059 mattress-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-01 15:45:21.000000 mattress-0.0.6/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-01 15:45:21.000000 mattress-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-01 15:45:21.000000 mattress-0.0.6/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-01 15:45:21.000000 mattress-0.0.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 15:45:21.000000 mattress-0.0.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-01 15:45:21.000000 mattress-0.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-08-01 15:45:21.000000 mattress-0.0.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-01 15:45:21.000000 mattress-0.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-01 15:45:21.000000 mattress-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-01 15:45:35.493059 mattress-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-01 15:45:21.000000 mattress-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.469059 mattress-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-01 15:45:21.000000 mattress-0.0.6/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.469059 mattress-0.0.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 15:45:21.000000 mattress-0.0.6/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 15:45:21.000000 mattress-0.0.6/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-01 15:45:21.000000 mattress-0.0.6/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-08-01 15:45:21.000000 mattress-0.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-01 15:45:21.000000 mattress-0.0.6/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-01 15:45:21.000000 mattress-0.0.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 15:45:21.000000 mattress-0.0.6/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 15:45:21.000000 mattress-0.0.6/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-01 15:45:21.000000 mattress-0.0.6/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-01 15:45:21.000000 mattress-0.0.6/docs/tutorial
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-01 15:45:21.000000 mattress-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-01 15:45:35.493059 mattress-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-01 15:45:21.000000 mattress-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.465059 mattress-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.473059 mattress-0.0.6/src/mattress/
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-08-01 15:45:21.000000 mattress-0.0.6/src/mattress/TatamiNumericPointer.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-01 15:45:21.000000 mattress-0.0.6/src/mattress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-08-01 15:45:21.000000 mattress-0.0.6/src/mattress/cpphelpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.469059 mattress-0.0.6/src/mattress/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.473059 mattress-0.0.6/src/mattress/extern/tatami/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 15:45:22.000000 mattress-0.0.6/src/mattress/extern/tatami/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.465059 mattress-0.0.6/src/mattress/extern/tatami/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.473059 mattress-0.0.6/src/mattress/extern/tatami/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.473059 mattress-0.0.6/src/mattress/extern/tatami/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   108951 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.473059 mattress-0.0.6/src/mattress/extern/tatami/gallery/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/gallery/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/gallery/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.473059 mattress-0.0.6/src/mattress/extern/tatami/gallery/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/gallery/src/char2double.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/gallery/src/colsums.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/gallery/src/parallel.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/gallery/src/print_vector.h
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/gallery/src/read_h5.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/gallery/src/read_mm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.465059 mattress-0.0.6/src/mattress/extern/tatami/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.473059 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.477059 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/base/
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/base/Options.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/base/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.477059 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/dense/
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/dense/convert_to_dense.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.477059 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.477059 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/binary/
--rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.477059 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/unary/
--rw-r--r--   0 runner    (1001) docker     (123)    31440 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.477059 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/other/
--rw-r--r--   0 runner    (1001) docker     (123)    29155 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.477059 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/
--rw-r--r--   0 runner    (1001) docker     (123)    27711 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    27710 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/convert_to_compressed_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/convert_to_fragmented_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.477059 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/stats/medians.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/stats/sums.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/stats/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/stats/variances.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.481059 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/
--rw-r--r--   0 runner    (1001) docker     (123)    26535 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22752 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23308 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/tatami.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.481059 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/ElementType.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/convert_to_dense.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/convert_to_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.481059 mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/tatami_test.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/utils.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.481059 mattress-0.0.6/src/mattress/extern/tatami/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.465059 mattress-0.0.6/src/mattress/extern/tatami/tests/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.481059 mattress-0.0.6/src/mattress/extern/tatami/tests/src/dense/
--rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/dense/convert_to_dense.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.481059 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.481059 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/binary/
--rw-r--r--   0 runner    (1001) docker     (123)    42584 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.485059 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    62084 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30151 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.485059 mattress-0.0.6/src/mattress/extern/tatami/tests/src/other/
--rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.485059 mattress-0.0.6/src/mattress/extern/tatami/tests/src/sparse/
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21117 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/sparse/convert_to_compressed_sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/sparse/convert_to_fragmented_sparse.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.485059 mattress-0.0.6/src/mattress/extern/tatami/tests/src/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/stats/medians.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/stats/parallelize.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/stats/ranges.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/stats/sums.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/stats/variances.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.489059 mattress-0.0.6/src/mattress/extern/tatami/tests/src/subset/
--rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.489059 mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.489059 mattress-0.0.6/src/mattress/extern/tatami_hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 15:45:22.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/.git
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.469059 mattress-0.0.6/src/mattress/extern/tatami_hdf5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.489059 mattress-0.0.6/src/mattress/extern/tatami_hdf5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.489059 mattress-0.0.6/src/mattress/extern/tatami_hdf5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   108708 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/docs/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.489059 mattress-0.0.6/src/mattress/extern/tatami_hdf5/extern/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/extern/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.469059 mattress-0.0.6/src/mattress/extern/tatami_hdf5/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.489059 mattress-0.0.6/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)    48131 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/tatami_hdf5.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.489059 mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.493059 mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-08-01 15:45:23.000000 mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.493059 mattress-0.0.6/src/mattress/include/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-01 15:45:21.000000 mattress-0.0.6/src/mattress/include/Mattress.h
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-08-01 15:45:21.000000 mattress-0.0.6/src/mattress/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.493059 mattress-0.0.6/src/mattress/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-08-01 15:45:21.000000 mattress-0.0.6/src/mattress/lib/bindings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-01 15:45:21.000000 mattress-0.0.6/src/mattress/lib/common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-08-01 15:45:21.000000 mattress-0.0.6/src/mattress/lib/compressed_sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-01 15:45:21.000000 mattress-0.0.6/src/mattress/lib/dense.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-01 15:45:21.000000 mattress-0.0.6/src/mattress/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-01 15:45:21.000000 mattress-0.0.6/src/mattress/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.473059 mattress-0.0.6/src/mattress.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-01 15:45:35.000000 mattress-0.0.6/src/mattress.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-08-01 15:45:35.000000 mattress-0.0.6/src/mattress.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:45:35.000000 mattress-0.0.6/src/mattress.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 15:45:35.000000 mattress-0.0.6/src/mattress.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 15:45:35.000000 mattress-0.0.6/src/mattress.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 15:45:35.000000 mattress-0.0.6/src/mattress.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 15:45:35.493059 mattress-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-01 15:45:21.000000 mattress-0.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-01 15:45:21.000000 mattress-0.0.6/tests/test_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-01 15:45:21.000000 mattress-0.0.6/tests/test_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-01 15:45:21.000000 mattress-0.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.501857 mattress-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-08-01 20:40:23.000000 mattress-0.0.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.457856 mattress-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.469856 mattress-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-01 20:40:23.000000 mattress-0.0.7/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-01 20:40:23.000000 mattress-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-01 20:40:23.000000 mattress-0.0.7/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-01 20:40:23.000000 mattress-0.0.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-01 20:40:23.000000 mattress-0.0.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-01 20:40:23.000000 mattress-0.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-08-01 20:40:23.000000 mattress-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-01 20:40:23.000000 mattress-0.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-01 20:40:23.000000 mattress-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-08-01 20:40:38.501857 mattress-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-08-01 20:40:23.000000 mattress-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.469856 mattress-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-01 20:40:23.000000 mattress-0.0.7/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.469856 mattress-0.0.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 20:40:23.000000 mattress-0.0.7/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 20:40:23.000000 mattress-0.0.7/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-01 20:40:23.000000 mattress-0.0.7/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-08-01 20:40:23.000000 mattress-0.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-01 20:40:23.000000 mattress-0.0.7/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-01 20:40:23.000000 mattress-0.0.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 20:40:23.000000 mattress-0.0.7/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 20:40:23.000000 mattress-0.0.7/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-01 20:40:23.000000 mattress-0.0.7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-08-01 20:40:23.000000 mattress-0.0.7/docs/tutorial
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-01 20:40:23.000000 mattress-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-01 20:40:38.501857 mattress-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-08-01 20:40:23.000000 mattress-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.457856 mattress-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.473857 mattress-0.0.7/src/mattress/
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-08-01 20:40:23.000000 mattress-0.0.7/src/mattress/TatamiNumericPointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-08-01 20:40:23.000000 mattress-0.0.7/src/mattress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-08-01 20:40:23.000000 mattress-0.0.7/src/mattress/cpphelpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.465856 mattress-0.0.7/src/mattress/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.473857 mattress-0.0.7/src/mattress/extern/tatami/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.457856 mattress-0.0.7/src/mattress/extern/tatami/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.473857 mattress-0.0.7/src/mattress/extern/tatami/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.473857 mattress-0.0.7/src/mattress/extern/tatami/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108951 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.473857 mattress-0.0.7/src/mattress/extern/tatami/gallery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/gallery/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/gallery/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.477856 mattress-0.0.7/src/mattress/extern/tatami/gallery/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/gallery/src/char2double.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/gallery/src/colsums.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/gallery/src/parallel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/gallery/src/print_vector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/gallery/src/read_h5.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/gallery/src/read_mm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.461856 mattress-0.0.7/src/mattress/extern/tatami/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.477856 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.477856 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/base/
+-rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/base/Options.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/base/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.477856 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/dense/
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/dense/convert_to_dense.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.477856 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.481856 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.481856 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/unary/
+-rw-r--r--   0 runner    (1001) docker     (123)    31440 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17594 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10874 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.481856 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/other/
+-rw-r--r--   0 runner    (1001) docker     (123)    29155 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14885 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.481856 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/
+-rw-r--r--   0 runner    (1001) docker     (123)    27711 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27710 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16795 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14977 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/convert_to_compressed_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/convert_to_fragmented_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.485857 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/stats/medians.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10646 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/stats/sums.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/stats/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/stats/variances.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.485857 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/
+-rw-r--r--   0 runner    (1001) docker     (123)    26535 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22752 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11177 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23308 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/tatami.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.485857 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/ElementType.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/convert_to_dense.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/convert_to_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.489857 mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/tatami_test.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/utils.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.489857 mattress-0.0.7/src/mattress/extern/tatami/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.465856 mattress-0.0.7/src/mattress/extern/tatami/tests/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.489857 mattress-0.0.7/src/mattress/extern/tatami/tests/src/dense/
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/dense/convert_to_dense.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.489857 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.489857 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/binary/
+-rw-r--r--   0 runner    (1001) docker     (123)    42584 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.489857 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    62084 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30151 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.493857 mattress-0.0.7/src/mattress/extern/tatami/tests/src/other/
+-rw-r--r--   0 runner    (1001) docker     (123)    14777 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.493857 mattress-0.0.7/src/mattress/extern/tatami/tests/src/sparse/
+-rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9890 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21117 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7623 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/sparse/convert_to_compressed_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/sparse/convert_to_fragmented_sparse.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.493857 mattress-0.0.7/src/mattress/extern/tatami/tests/src/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/stats/medians.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/stats/parallelize.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11128 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/stats/ranges.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/stats/sums.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/stats/variances.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.493857 mattress-0.0.7/src/mattress/extern/tatami/tests/src/subset/
+-rw-r--r--   0 runner    (1001) docker     (123)    21245 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.497857 mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.497857 mattress-0.0.7/src/mattress/extern/tatami_hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/.git
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.465856 mattress-0.0.7/src/mattress/extern/tatami_hdf5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.497857 mattress-0.0.7/src/mattress/extern/tatami_hdf5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.497857 mattress-0.0.7/src/mattress/extern/tatami_hdf5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   108708 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/docs/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.497857 mattress-0.0.7/src/mattress/extern/tatami_hdf5/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/extern/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.465856 mattress-0.0.7/src/mattress/extern/tatami_hdf5/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.497857 mattress-0.0.7/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)    48131 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/tatami_hdf5.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.497857 mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.501857 mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    22267 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17105 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-08-01 20:40:24.000000 mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.501857 mattress-0.0.7/src/mattress/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-01 20:40:23.000000 mattress-0.0.7/src/mattress/include/Mattress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-08-01 20:40:23.000000 mattress-0.0.7/src/mattress/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.501857 mattress-0.0.7/src/mattress/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-08-01 20:40:23.000000 mattress-0.0.7/src/mattress/lib/bindings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-01 20:40:23.000000 mattress-0.0.7/src/mattress/lib/common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-08-01 20:40:23.000000 mattress-0.0.7/src/mattress/lib/compressed_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-01 20:40:23.000000 mattress-0.0.7/src/mattress/lib/dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-01 20:40:23.000000 mattress-0.0.7/src/mattress/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-01 20:40:23.000000 mattress-0.0.7/src/mattress/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.473857 mattress-0.0.7/src/mattress.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-08-01 20:40:38.000000 mattress-0.0.7/src/mattress.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-08-01 20:40:38.000000 mattress-0.0.7/src/mattress.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:40:38.000000 mattress-0.0.7/src/mattress.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:40:38.000000 mattress-0.0.7/src/mattress.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 20:40:38.000000 mattress-0.0.7/src/mattress.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 20:40:38.000000 mattress-0.0.7/src/mattress.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:40:38.501857 mattress-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-01 20:40:23.000000 mattress-0.0.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-01 20:40:23.000000 mattress-0.0.7/tests/test_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-01 20:40:23.000000 mattress-0.0.7/tests/test_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-01 20:40:23.000000 mattress-0.0.7/tox.ini
```

### Comparing `mattress-0.0.6/.coveragerc` & `mattress-0.0.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/.github/workflows/pypi-test.yml` & `mattress-0.0.7/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/.gitignore` & `mattress-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/.readthedocs.yml` & `mattress-0.0.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/CONTRIBUTING.md` & `mattress-0.0.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/LICENSE.txt` & `mattress-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/docs/Makefile` & `mattress-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/docs/conf.py` & `mattress-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/docs/index.md` & `mattress-0.0.7/docs/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # mattress
 
-Mattress provides tatami representations for python matrices (numpy, scipy etc)
-
+The **mattress** package implements Python bindings to the [**tatami**](https://github.com/tatami-inc) C++ library for matrix representations.
+Downstream packages can use **mattress** to develop C++ extensions that are interoperable with many different matrix classes, e.g., dense, sparse, delayed or file-backed.
+It is based on the [**beachmat**](https://bioconductor/packages/beachmat) Bioconductor package, which does the same thing for R packages.
 
 ## Install
 
 Package is published to [PyPI](https://pypi.org/project/mattress/)
 
 ```shell
 pip install mattress
```

### Comparing `mattress-0.0.6/setup.cfg` & `mattress-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/setup.py` & `mattress-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/TatamiNumericPointer.py` & `mattress-0.0.7/src/mattress/TatamiNumericPointer.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/__init__.py` & `mattress-0.0.7/src/mattress/__init__.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml` & `mattress-0.0.7/src/mattress/extern/tatami/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml` & `mattress-0.0.7/src/mattress/extern/tatami/.github/workflows/run-gallery.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/.github/workflows/run-tests.yaml` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -16,35 +16,30 @@
             omp: true
           }
         - {
             name: "Ubuntu Latest GCC, coverage enabled", 
             os: ubuntu-latest,
             cov: true
           }
-        - {
-            name: "macOS Latest Clang", 
-            os: macos-latest
-          }
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Get latest CMake
       uses: lukka/get-cmake@latest
 
-    - name: Configure the build for Mac
-      if: ${{ matrix.config.os == 'macos-latest' }}
-      run: cmake -S . -B build
+    - name: Install HDF5
+      run: sudo apt-get install libhdf5-dev
 
     - name: Configure the build with coverage
-      if: ${{ matrix.config.os == 'ubuntu-latest' && matrix.config.cov }}
+      if: ${{ matrix.config.cov }}
       run: cmake -S . -B build -DCODE_COVERAGE=ON 
 
     - name: Configure the build with OpenMP
-      if: ${{ matrix.config.os == 'ubuntu-latest' && matrix.config.omp }}
+      if: ${{ matrix.config.omp }}
       run: cmake -S . -B build -DUSE_OPENMP=ON
 
     - name: Run the build
       run: cmake --build build
 
     - name: Run the tests
       run: |
```

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/CMakeLists.txt` & `mattress-0.0.7/src/mattress/extern/tatami/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/LICENSE` & `mattress-0.0.7/src/mattress/extern/tatami/LICENSE`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/README.md` & `mattress-0.0.7/src/mattress/extern/tatami/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/docs/Doxyfile` & `mattress-0.0.7/src/mattress/extern/tatami/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/gallery/CMakeLists.txt` & `mattress-0.0.7/src/mattress/extern/tatami/gallery/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/gallery/README.md` & `mattress-0.0.7/src/mattress/extern/tatami/gallery/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/gallery/src/char2double.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/gallery/src/char2double.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/gallery/src/colsums.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/gallery/src/colsums.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/gallery/src/parallel.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/gallery/src/parallel.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/gallery/src/print_vector.h` & `mattress-0.0.7/src/mattress/extern/tatami/gallery/src/print_vector.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/gallery/src/read_h5.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/gallery/src/read_h5.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/gallery/src/read_mm.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/gallery/src/read_mm.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/gallery/src/sparse_extractor.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/base/Extractor.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/base/Matrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/base/Options.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/base/Options.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/base/SparseRange.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/base/utils.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/base/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/dense/DenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/dense/VirtualDenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/dense/convert_to_dense.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/dense/convert_to_dense.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/arith_utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/binary/DelayedBinaryIsometricOp.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/binary/arith_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/binary/boolean_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/binary/compare_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/binary/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/boolean_utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/compare_utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/unary/DelayedUnaryIsometricOp.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/unary/arith_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/unary/boolean_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/unary/compare_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/isometric/unary/math_helpers.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/other/DelayedBind.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/other/DelayedCast.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/other/DelayedTranspose.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/CompressedSparseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/FragmentedSparseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/SemiCompressedSparseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/SparseSecondaryExtractorCore.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/convert_to_compressed_sparse.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/convert_to_compressed_sparse.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/convert_to_fragmented_sparse.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/convert_to_fragmented_sparse.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/primary_extraction.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/sparse/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/stats/medians.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/stats/medians.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/stats/ranges.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/stats/sums.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/stats/sums.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/stats/utils.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/stats/utils.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -3,26 +3,39 @@
 
 #include "../base/Matrix.hpp"
 #include "../base/utils.hpp"
 #include "../utils/Oracles.hpp"
 
 #include <cmath>
 
+#ifndef TATAMI_CUSTOM_PARALLEL
+#ifndef _OPENMP
+#include <thread>
+#endif
+#include <string>
+#include <stdexcept>
+#include <vector>
+#endif
+
 /**
  * @file utils.hpp
  *
  * @brief Utilities for computing matrix statistics.
  */
 
 namespace tatami {
 
 /**
- * Apply a function to a set of tasks, distributing them to threads via OpenMP if enabled.
- * Callers can specify a custom parallelization scheme by defining a `TATAMI_CUSTOM_PARALLEL` function-like macro, 
- * which should accept the `fun`, `tasks` and `threads` arguments as below.
+ * Apply a function to a set of tasks in parallel.
+ * This can be done using:
+ *
+ * - OpenMP, if available and enabled by the compiler.
+ * - Using a custom parallelization scheme, by defining a `TATAMI_CUSTOM_PARALLEL` function-like macro. 
+ *   This should accept the `fun`, `tasks` and `threads` arguments as below.
+ * - `<thread>`, otherwise.
  *
  * @tparam parallel_ Whether the tasks should be run in parallel.
  * If `false`, no parallelization is performed and all tasks are run on the current thread.
  * @tparam Function_ Function to be applied for a contiguous range of tasks.
  * This should accept three arguments:
  * - `thread`, the thread number executing this task range.
  *   This will be passed as a `size_t`.
@@ -33,41 +46,74 @@
  * @tparam Index_ Integer type for the number of tasks.
  *
  * @param fun Function that executes a contiguous range of tasks.
  * @param tasks Number of tasks.
  * @param threads Number of threads.
  */
 template<bool parallel_ = true, class Function_, typename Index_>
-void parallelize(Function_ fun, Index_ tasks, size_t
-#if defined(_OPENMP) || defined(TATAMI_CUSTOM_PARALLEL)
-    threads // wrap here to avoid used variable warnings (which are in turn converted to errors).
-#endif
-) {
-#if defined(_OPENMP) || defined(TATAMI_CUSTOM_PARALLEL)
-
+void parallelize(Function_ fun, Index_ tasks, size_t threads) {
     if constexpr(parallel_) {
-
         if (threads > 1) {
 #ifndef TATAMI_CUSTOM_PARALLEL
             Index_ worker_size = (tasks / threads) + (tasks % threads > 0); // Ceiling of an integer division.
             threads = (tasks / worker_size) + (tasks % worker_size > 0); // Set the actual number of required threads.
+            std::vector<std::string> errors(threads);
 
+#if defined(_OPENMP)
             #pragma omp parallel for num_threads(threads)
             for (size_t t = 0; t < threads; ++t) {
                 Index_ start = worker_size * t; // Will not overflow due to the above recomputation of 'threads'.
                 Index_ remaining = tasks - start; // Must be positive, as otherwise 'tasks % worker_size = 0' and the iteration wouldn't even get here.
-                fun(t, start, std::min(remaining, worker_size)); // Use 'remaining' to avoid potential overflow from computing 'end = start + worker_size'.
+
+                try {
+                    fun(t, start, std::min(remaining, worker_size)); // Use 'remaining' to avoid potential overflow from computing 'end = start + worker_size'.
+                } catch (std::exception& e) {
+                    errors[t] = e.what();
+                } catch (...) {
+                    errors[t] = "unknown error in thread " + std::to_string(t);
+                }
             }
+
+#else
+            Index_ first = 0;
+            std::vector<std::thread> workers;
+            workers.reserve(threads);
+
+            for (size_t t = 0; t < threads && first < tasks; ++t) {
+                Index_ remaining = tasks - first;
+                Index_ len = std::min(remaining, worker_size);
+                workers.emplace_back([&fun,&errors](int t, Index_ first, Index_ len) -> void {
+                    try {
+                        fun(t, first, len);
+                    } catch (std::exception& e) {
+                        errors[t] = e.what();
+                    } catch (...) {
+                        errors[t] = "unknown error in thread " + std::to_string(t);
+                    }
+                }, t, first, len);
+                first += len;
+            }
+
+            for (auto& wrk : workers) {
+                wrk.join();
+            }
+#endif
+
+            for (const auto& e : errors) {
+                if (!e.empty()) {
+                    throw std::runtime_error(e);
+                }
+            }
+
 #else
             TATAMI_CUSTOM_PARALLEL(std::move(fun), tasks, threads);
 #endif
             return;
         }
     }
-#endif
 
     fun(0, 0, tasks);
     return;
 }
 
 /**
  * @tparam row_ Whether to perform extraction on rows.
```

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/stats/variances.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/stats/variances.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/DelayedSubset.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetBlock.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSorted.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetSortedUnique.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/DelayedSubsetUnique.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/make_DelayedSubset.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/subset/utils.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/subset/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/tatami.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/tatami.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/ArrayView.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/Oracles.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/SomeNumericArray.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/bind_intersection.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/compress_sparse_triplets.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/convert_to_sparse.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/convert_to_sparse.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/process_consecutive_indices.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami/utils/wrap_shared_ptr.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/simulate_vector.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/temp_file_path.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/test_access_base.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/test_column_access.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/test_oracle_access.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/test_row_access.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/include/tatami_test/utils.hpp` & `mattress-0.0.7/src/mattress/extern/tatami/include/tatami_test/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/README.md` & `mattress-0.0.7/src/mattress/extern/tatami/tests/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/dense/DenseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/dense/convert_to_dense.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/dense/convert_to_dense.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/binary/arith_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/binary/boolean_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/binary/compare_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/arith_scalar_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/arith_vector_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_scalar_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/boolean_vector_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/compare_scalar_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/compare_vector_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/unary/math_helpers.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/isometric/utils.h` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/isometric/utils.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/other/DelayedBind.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/other/DelayedCast.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/other/DelayedTranspose.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/sparse/CompressedSparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/sparse/FragmentedSparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/sparse/SemiCompressedSparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/sparse/SparseSecondaryExtractorCore.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/sparse/convert_to_compressed_sparse.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/sparse/convert_to_compressed_sparse.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/sparse/convert_to_fragmented_sparse.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/sparse/convert_to_fragmented_sparse.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/stats/custom_parallel.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/stats/medians.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/stats/medians.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/stats/ranges.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/stats/ranges.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/stats/sums.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/stats/sums.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/stats/variances.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/stats/variances.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/subset/DelayedSubset.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/subset/DelayedSubsetBlock.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/ArrayView.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/Oracles.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/SomeNumericArray.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/bind_intersection.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/compress_sparse_triplets.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/process_consecutive_indices.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp` & `mattress-0.0.7/src/mattress/extern/tatami/tests/src/utils/wrap_shared_ptr.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/.github/workflows/doxygenate.yaml`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/.github/workflows/run-tests.yaml` & `mattress-0.0.7/src/mattress/extern/tatami/.github/workflows/run-tests.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -7,41 +7,37 @@
     name: ${{ matrix.config.name }}
     runs-on: ${{ matrix.config.os }}
     strategy:
       fail-fast: false
       matrix:
         config:
         - {
-            name: "Ubuntu Latest GCC, OpenMP enabled", 
-            os: ubuntu-latest,
-            omp: true
-          }
-        - {
             name: "Ubuntu Latest GCC, coverage enabled", 
             os: ubuntu-latest,
             cov: true
           }
+        - {
+            name: "macOS Latest Clang", 
+            os: macos-latest
+          }
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Get latest CMake
       uses: lukka/get-cmake@latest
 
-    - name: Install HDF5
-      run: sudo apt-get install libhdf5-dev
+    - name: Configure the build for Mac
+      if: ${{ matrix.config.os == 'macos-latest' }}
+      run: cmake -S . -B build
 
     - name: Configure the build with coverage
-      if: ${{ matrix.config.cov }}
+      if: ${{ matrix.config.os == 'ubuntu-latest' && matrix.config.cov }}
       run: cmake -S . -B build -DCODE_COVERAGE=ON 
 
-    - name: Configure the build with OpenMP
-      if: ${{ matrix.config.omp }}
-      run: cmake -S . -B build -DUSE_OPENMP=ON
-
     - name: Run the build
       run: cmake --build build
 
     - name: Run the tests
       run: |
         cd build
         ctest
```

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/CMakeLists.txt` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/LICENSE` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/LICENSE`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/README.md` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/README.md`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/docs/Doxyfile` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/docs/Doxyfile`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5CompressedSparseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/Hdf5DenseMatrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/load_hdf5_matrix.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/utils.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/include/tatami_hdf5/write_sparse_matrix_to_hdf5.hpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/src/Hdf5CompressedSparseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/src/Hdf5DenseMatrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/src/custom_parallel.h`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/src/load_hdf5_matrix.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp` & `mattress-0.0.7/src/mattress/extern/tatami_hdf5/tests/src/write_sparse_matrix_to_hdf5.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/interface.py` & `mattress-0.0.7/src/mattress/interface.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/lib/bindings.cpp` & `mattress-0.0.7/src/mattress/lib/bindings.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* DO NOT MODIFY: this is automatically generated by the ctypes-compiler */
+/* DO NOT MODIFY: this is automatically generated by the ctypes-wrapper */
 
 #include <cstring>
 #include <stdexcept>
 
 #ifdef _WIN32
 #define PYAPI __declspec(dllexport)
 #else
```

### Comparing `mattress-0.0.6/src/mattress/lib/common.cpp` & `mattress-0.0.7/src/mattress/lib/common.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/lib/compressed_sparse.cpp` & `mattress-0.0.7/src/mattress/lib/compressed_sparse.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/lib/dense.cpp` & `mattress-0.0.7/src/mattress/lib/dense.cpp`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress/utils.py` & `mattress-0.0.7/src/mattress/utils.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/src/mattress.egg-info/SOURCES.txt` & `mattress-0.0.7/src/mattress.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/tests/test_dense.py` & `mattress-0.0.7/tests/test_dense.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/tests/test_sparse.py` & `mattress-0.0.7/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `mattress-0.0.6/tox.ini` & `mattress-0.0.7/tox.ini`

 * *Files identical despite different names*

