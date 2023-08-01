# Comparing `tmp/artistools-2023.5.16.3.tar.gz` & `tmp/artistools-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artistools-2023.5.16.3.tar", last modified: Tue May 16 20:40:06 2023, max compression
+gzip compressed data, was "artistools-2023.8.1.tar", last modified: Tue Aug  1 11:58:18 2023, max compression
```

## Comparing `artistools-2023.5.16.3.tar` & `artistools-2023.8.1.tar`

### file list

```diff
@@ -1,387 +1,388 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.678305 artistools-2023.5.16.3/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.642305 artistools-2023.5.16.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.642305 artistools-2023.5.16.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.github/workflows/deploypypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.github/workflows/deploytestpypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.landscape.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/.python-version
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-16 20:40:06.678305 artistools-2023.5.16.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.622304 artistools-2023.5.16.3/artistools/
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.622304 artistools-2023.5.16.3/artistools/atomic/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/atomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/atomic/_atomic_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/codecomparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.622304 artistools-2023.5.16.3/artistools/data/
--rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/ElBiEn_2007.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/atomic_properties.txt
--rw-r--r--   0 runner    (1001) docker     (123)    30868 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/betaminusdecays.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/binding_energies.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/collion-AR1985.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/collion-reference.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/collion.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/elements.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.626304 artistools-2023.5.16.3/artistools/data/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/400.txt
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/520.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.626304 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/ASIAGO/zs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    48059 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/FUV.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/H.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/H_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)    55262 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/J.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/J_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/K.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/K_ab.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.626304 artistools-2023.5.16.3/artistools/data/filters/LCOGT/
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11032 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/R.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LCOGT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/LSQ/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LSQ/rs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/LT/
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LT/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LT/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/LT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/NOT/
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/R.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NOT/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/NTT/
--rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/B.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/R.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22775 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NTT/zs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26456 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/NUV.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/OGLE/
--rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/OGLE/I.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20398 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/OGLE/V.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/PS1/
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/PS1/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/PS1/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/PS1/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/PS1/ws.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/PS1/zs.txt
--rw-r--r--   0 runner    (1001) docker     (123)    84060 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/R.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.630304 artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/zs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/U.txt
--rw-r--r--   0 runner    (1001) docker     (123)    55259 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/V.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/gs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/is.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/rs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/us.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/uvm2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/uvm2_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/uvw1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/uvw1_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/uvw2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/uvw2_ab.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/filters/zs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.650305 artistools-2023.5.16.3/artistools/data/lightcurves/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_Bband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_Rband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_Vband_photometric_point.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_unfiltered_lc_data.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_unfiltered_lc_data_I.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_unfiltered_lc_data_R.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_unfiltered_lc_data_V.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2004cs_unfiltered_lc_data_rs.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2007qd_lc_rs_microJy.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2008ha_lc_B.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2008ha_lc_I.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2008ha_lc_R.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/2008ha_lc_V.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN1991T.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN1999by.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN1999dq.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2005cf.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2011fe.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2012cg.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2012dn.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2012fr.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2014J.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2015F.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2015H_r_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2016jhr_BV.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2016jhr_gri.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/SN2018byg.dat.meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.650305 artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/iPTF13ebh.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Hdef_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Hdef_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Hdef_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Hdef_2014_V_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Ldef_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Ldef_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Ldef_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100Ldef_2014_V_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100def_2014_B_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100def_2014_I_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100def_2014_R_band.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/lightcurves/n100def_2014_V_band.txt.meta.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.670305 artistools-2023.5.16.3/artistools/data/refspectra/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    75182 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    73950 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2010lp_20110928_fors2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2010lp_20110928_fors2.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2015H_19_days_since_explosion.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2016jhr_18days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2016jhr_29.33d_num1.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    80396 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   423964 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    80401 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    60829 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None_filtered.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)    96381 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None_filtered.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   423466 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   787320 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   713500 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   713176 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   664004 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   708656 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   712196 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   709200 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   552728 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   707384 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)   705880 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/CMFGEN_12.1days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/CMFGEN_18days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   257680 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/N3_def_1.71_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/N3_def_4.50_days_after_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/N3_def_5.54_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/N3_def_6.72_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   104189 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+10_num45.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+11_2_num47.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+11_num46.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+18_2_num51.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+1_num28.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+21_num53.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+28.2_num59.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_+31_num60.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-0_8_num27.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-1.8_num26.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-10_num5.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-3_num24.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-5_num20.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-6_num17.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-7_7_num12.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-7_num13.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-9_8_num6.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2011fe_-9_num9.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2012fr_+0_num46.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2012fr_-10_num8.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   210900 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2019yvq-2020-01-04-7days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/SN2019yvq-2020-01-12-15days.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/dop_dered_SN2013aa_20140208_fc_final.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/iPTF13ebh_20131114-12_8d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/iPTF13ebh_20131116-10_7d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/iPTF13ebh_20131116-11.1d-optical.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/iPTF13ebh_20131120-6_8d.dat.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   122618 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/n5_def_1.56_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/n5_def_4.42_days_after_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/n5_def_5.68_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/n5_def_6.65_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/n5_def_8.77_days_before_r_peak.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/nero-nebspec.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)   103168 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt.meta.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/solar_r_abundance_pattern.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/data/splitmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5325 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/deposition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.638305 artistools-2023.5.16.3/artistools/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19625 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/estimators_classic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2290 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/exportmassfractions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/plot3destimators_classic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    42569 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/estimators/plotestimators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25084 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/gsinetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/hesma_scripts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14318 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/initial_composition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.638305 artistools-2023.5.16.3/artistools/inputmodel/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6390 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/1dslicefrom3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3834 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/botyanski2017.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5478 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/describeinputmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/downscale3dgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10107 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/energyinputfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.638305 artistools-2023.5.16.3/artistools/inputmodel/fromcmfgen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/fromcmfgen/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10742 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py
--rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/fromcmfgen/rd_cmfgen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2920 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/fullymixed.py
--rw-r--r--   0 runner    (1001) docker     (123)    44529 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/inputmodel_misc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3723 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/lapuente.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3034 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/makeartismodel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3969 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/maketardismodelfromartis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/map_1d_to_3d_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14501 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/maptogrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16453 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/modelfromhydro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/opacityinputfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2824 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/plotdensity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8280 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/recombinationenergy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24896 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/rprocess_from_trajectory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5534 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/rprocess_solar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2613 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/scalevelocity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3486 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/shen2018.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8370 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/slice1Dfromconein3dmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/inputmodel/test_inputmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.638305 artistools-2023.5.16.3/artistools/lightcurve/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22507 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)    64689 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/plotlightcurve.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2575 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/test_lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)    31958 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/viewingangleanalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/lightcurve/writebollightcurvedata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36660 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/linefluxes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4936 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/logfiles.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5822 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/macroatom.py
--rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (123)    48179 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.642305 artistools-2023.5.16.3/artistools/nltepops/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nltepops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nltepops/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nltepops/nltepops.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33086 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nltepops/plotnltepops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.642305 artistools-2023.5.16.3/artistools/nonthermal/
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nonthermal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nonthermal/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58909 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nonthermal/_nonthermal_core.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5021 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nonthermal/leptontransport.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11706 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nonthermal/plotnonthermal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14234 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/nonthermal/solvespencerfanocmd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.642305 artistools-2023.5.16.3/artistools/packets/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32364 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/packets/packets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/packets/packetsplots.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13422 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/plotspherical.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/plottools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    42385 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/radfield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.642305 artistools-2023.5.16.3/artistools/spectra/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51706 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/plotspectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/sampleblackbodyfrompacketTR.py
--rw-r--r--   0 runner    (1001) docker     (123)    54235 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4995 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/test_spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/spectra/test_vspectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4325 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/test_artistools.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20279 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/transitions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6887 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/viewing_angles_visualization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10909 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistools/writecomparisondata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.646304 artistools-2023.5.16.3/artistools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-16 20:40:06.000000 artistools-2023.5.16.3/artistools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23480 2023-05-16 20:40:06.000000 artistools-2023.5.16.3/artistools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:40:06.000000 artistools-2023.5.16.3/artistools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-16 20:40:06.000000 artistools-2023.5.16.3/artistools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 20:40:06.000000 artistools-2023.5.16.3/artistools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 20:40:06.000000 artistools-2023.5.16.3/artistools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/artistoolscompletions.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.674305 artistools-2023.5.16.3/images/
--rw-r--r--   0 runner    (1001) docker     (123)   154047 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/images/fig-emission.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    93995 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/images/fig-emission.png
--rw-r--r--   0 runner    (1001) docker     (123)    31156 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/images/fig-estimators.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   184801 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/images/fig-estimators.png
--rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/images/fig-nlte-Ni.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    82001 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/images/fig-nlte-Ni.png
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 20:40:06.678305 artistools-2023.5.16.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1433 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.674305 artistools-2023.5.16.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.674305 artistools-2023.5.16.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/data/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      455 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/data/setuptestdata.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.678305 artistools-2023.5.16.3/tests/data/testmodel_3d_10^3/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/data/testmodel_3d_10^3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    76456 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/data/testmodel_3d_10^3/abundances.txt.xz
--rw-r--r--   0 runner    (1001) docker     (123)    27560 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/data/testmodel_3d_10^3/model.txt.xz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:40:06.678305 artistools-2023.5.16.3/tests/output/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/output/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      497 2023-05-16 20:38:57.000000 artistools-2023.5.16.3/tests/plottransitions_example.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.702211 artistools-2023.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-01 11:56:42.000000 artistools-2023.8.1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-01 11:56:42.000000 artistools-2023.8.1/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-08-01 11:56:42.000000 artistools-2023.8.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.658211 artistools-2023.8.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-01 11:56:42.000000 artistools-2023.8.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.658211 artistools-2023.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-01 11:56:42.000000 artistools-2023.8.1/.github/workflows/deploypypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-01 11:56:42.000000 artistools-2023.8.1/.github/workflows/deploytestpypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-08-01 11:56:42.000000 artistools-2023.8.1/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-08-01 11:56:42.000000 artistools-2023.8.1/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-01 11:56:42.000000 artistools-2023.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-01 11:56:42.000000 artistools-2023.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 11:56:42.000000 artistools-2023.8.1/.python-version
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-08-01 11:56:42.000000 artistools-2023.8.1/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-01 11:56:42.000000 artistools-2023.8.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-01 11:56:42.000000 artistools-2023.8.1/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-08-01 11:56:42.000000 artistools-2023.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-01 11:56:42.000000 artistools-2023.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-08-01 11:58:18.702211 artistools-2023.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-08-01 11:56:42.000000 artistools-2023.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.658211 artistools-2023.8.1/artistools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.658211 artistools-2023.8.1/artistools/atomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/atomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/atomic/_atomic_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/codecomparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.662211 artistools-2023.8.1/artistools/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    70935 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/ElBiEn_2007.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/atomic_properties.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30868 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/betaminusdecays.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/binding_energies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/collion-AR1985.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/collion-reference.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/collion.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/elements.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.662211 artistools-2023.8.1/artistools/data/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/400.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/520.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.666211 artistools-2023.8.1/artistools/data/filters/ASIAGO/
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/ASIAGO/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/ASIAGO/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17947 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/ASIAGO/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/ASIAGO/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/ASIAGO/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/ASIAGO/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/ASIAGO/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    48059 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/FUV.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/H.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/H_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    55262 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/J.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/J_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/K.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/K_ab.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.666211 artistools-2023.8.1/artistools/data/filters/LCOGT/
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LCOGT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LCOGT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11032 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LCOGT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LCOGT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LCOGT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LCOGT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LCOGT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LCOGT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LCOGT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LCOGT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.666211 artistools-2023.8.1/artistools/data/filters/LSQ/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LSQ/rs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.666211 artistools-2023.8.1/artistools/data/filters/LT/
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/LT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.666211 artistools-2023.8.1/artistools/data/filters/NOT/
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NOT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NOT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NOT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NOT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NOT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NOT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NOT/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NOT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NOT/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NOT/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.670211 artistools-2023.8.1/artistools/data/filters/NTT/
+-rw-r--r--   0 runner    (1001) docker     (123)     7873 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NTT/B.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NTT/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13701 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NTT/R.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NTT/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NTT/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NTT/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NTT/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22775 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NTT/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26456 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/NUV.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.670211 artistools-2023.8.1/artistools/data/filters/OGLE/
+-rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/OGLE/I.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20398 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/OGLE/V.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.670211 artistools-2023.8.1/artistools/data/filters/PS1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/PS1/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/PS1/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/PS1/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/PS1/ws.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/PS1/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    84060 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/R.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.670211 artistools-2023.8.1/artistools/data/filters/SKYMAPPER/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/SKYMAPPER/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/SKYMAPPER/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/SKYMAPPER/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/SKYMAPPER/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/SKYMAPPER/zs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/U.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    55259 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/V.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/gs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/is.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/rs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/us.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/uvm2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/uvm2_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/uvw1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/uvw1_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/uvw2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/uvw2_ab.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/filters/zs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.674211 artistools-2023.8.1/artistools/data/lightcurves/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/2004cs_Bband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/2004cs_Rband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/2004cs_Vband_photometric_point.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/2004cs_unfiltered_lc_data.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/2004cs_unfiltered_lc_data_I.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/2004cs_unfiltered_lc_data_R.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/2004cs_unfiltered_lc_data_V.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/2004cs_unfiltered_lc_data_rs.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/2007qd_lc_rs_microJy.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/2008ha_lc_B.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/2008ha_lc_I.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/2008ha_lc_R.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/2008ha_lc_V.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN1991T.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN1999by.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN1999dq.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN2005cf.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN2011fe.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN2012cg.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN2012dn.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN2012fr.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN2014J.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN2015F.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN2015H_r_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN2016jhr_BV.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN2016jhr_gri.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/SN2018byg.dat.meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.674211 artistools-2023.8.1/artistools/data/lightcurves/bollightcurves/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/bollightcurves/AT2017gfo.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/iPTF13ebh.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/n100Hdef_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/n100Hdef_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/n100Hdef_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/n100Hdef_2014_V_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/n100Ldef_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/n100Ldef_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/n100Ldef_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/n100Ldef_2014_V_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/n100def_2014_B_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/n100def_2014_I_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/n100def_2014_R_band.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/lightcurves/n100def_2014_V_band.txt.meta.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.694211 artistools-2023.8.1/artistools/data/refspectra/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    75182 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    73950 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2010lp_20110928_fors2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2010lp_20110928_fors2.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2015H_19_days_since_explosion.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2016jhr_18days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2016jhr_29.33d_num1.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    80396 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   423964 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    80401 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    60829 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None_filtered.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    96381 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None_filtered.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   423466 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   787320 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   713500 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   713176 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   664004 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   708656 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   712196 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   709200 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   552728 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   707384 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)   705880 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/CMFGEN_12.1days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/CMFGEN_18days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   257680 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/N3_def_1.71_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/N3_def_4.50_days_after_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/N3_def_5.54_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/N3_def_6.72_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   104189 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_+10_num45.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_+11_2_num47.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_+11_num46.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_+18_2_num51.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_+1_num28.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_+21_num53.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_+28.2_num59.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_+31_num60.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_-0_8_num27.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_-1.8_num26.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_-10_num5.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_-3_num24.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_-5_num20.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_-6_num17.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_-7_7_num12.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_-7_num13.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_-9_8_num6.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2011fe_-9_num9.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2012fr_+0_num46.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2012fr_-10_num8.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   210930 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   210900 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2019yvq-2020-01-04-7days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/SN2019yvq-2020-01-12-15days.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/dop_dered_SN2013aa_20140208_fc_final.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/iPTF13ebh_20131114-12_8d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/iPTF13ebh_20131116-10_7d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/iPTF13ebh_20131116-11.1d-optical.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/iPTF13ebh_20131120-6_8d.dat.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   122618 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/n5_def_1.56_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/n5_def_4.42_days_after_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/n5_def_5.68_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/n5_def_6.65_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/n5_def_8.77_days_before_r_peak.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/nero-nebspec.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   103168 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt.meta.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/solar_r_abundance_pattern.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/data/splitmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5354 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/deposition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.694211 artistools-2023.8.1/artistools/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/estimators/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19204 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/estimators/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/estimators/estimators_classic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2245 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/estimators/exportmassfractions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/estimators/plot3destimators_classic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42214 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/estimators/plotestimators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26251 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/gsinetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/hesma_scripts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14200 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/initial_composition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.698211 artistools-2023.8.1/artistools/inputmodel/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6348 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/1dslicefrom3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3828 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/botyanski2017.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5504 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/describeinputmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/downscale3dgrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/energyinputfiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.698211 artistools-2023.8.1/artistools/inputmodel/fromcmfgen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/fromcmfgen/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10706 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/fromcmfgen/rd_cmfgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2892 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/fullymixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44378 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/inputmodel_misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3723 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/lapuente.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3030 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/makeartismodel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3968 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/maketardismodelfromartis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/map_1d_to_3d_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14478 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/maptogrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16349 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/modelfromhydro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/opacityinputfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2789 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/plotdensity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8192 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/recombinationenergy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24623 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/rprocess_from_trajectory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5406 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/rprocess_solar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2553 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/scalevelocity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3485 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/shen2018.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8371 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/slice1Dfromconein3dmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/inputmodel/test_inputmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.698211 artistools-2023.8.1/artistools/lightcurve/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/lightcurve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/lightcurve/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22365 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/lightcurve/lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64812 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/lightcurve/plotlightcurve.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2575 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/lightcurve/test_lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31760 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/lightcurve/viewingangleanalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/lightcurve/writebollightcurvedata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38266 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/linefluxes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4770 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/logfiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5615 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/macroatom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (123)    50160 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.698211 artistools-2023.8.1/artistools/nltepops/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/nltepops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/nltepops/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/nltepops/nltepops.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32900 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/nltepops/plotnltepops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.702211 artistools-2023.8.1/artistools/nonthermal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/nonthermal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/nonthermal/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58463 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/nonthermal/_nonthermal_core.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5014 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/nonthermal/leptontransport.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11674 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/nonthermal/plotnonthermal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14240 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/nonthermal/solvespencerfanocmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.702211 artistools-2023.8.1/artistools/packets/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32308 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/packets/packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/packets/packetsplots.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13414 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/plotspherical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/plottools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/py.typed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42215 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/radfield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.702211 artistools-2023.8.1/artistools/spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/spectra/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      100 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/spectra/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54025 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/spectra/plotspectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/spectra/sampleblackbodyfrompacketTR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52958 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/spectra/spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4957 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/spectra/test_spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1351 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/spectra/test_vspectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2240 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4287 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/test_artistools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20424 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/transitions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6885 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/viewing_angles_visualization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11330 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistools/writecomparisondata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.658211 artistools-2023.8.1/artistools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-08-01 11:58:18.000000 artistools-2023.8.1/artistools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-08-01 11:58:18.000000 artistools-2023.8.1/artistools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:58:18.000000 artistools-2023.8.1/artistools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-08-01 11:58:18.000000 artistools-2023.8.1/artistools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-01 11:58:18.000000 artistools-2023.8.1/artistools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 11:58:18.000000 artistools-2023.8.1/artistools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-08-01 11:56:42.000000 artistools-2023.8.1/artistoolscompletions.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.702211 artistools-2023.8.1/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   154047 2023-08-01 11:56:42.000000 artistools-2023.8.1/images/fig-emission.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    93995 2023-08-01 11:56:42.000000 artistools-2023.8.1/images/fig-emission.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31156 2023-08-01 11:56:42.000000 artistools-2023.8.1/images/fig-estimators.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   184801 2023-08-01 11:56:42.000000 artistools-2023.8.1/images/fig-estimators.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21031 2023-08-01 11:56:42.000000 artistools-2023.8.1/images/fig-nlte-Ni.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    82001 2023-08-01 11:56:42.000000 artistools-2023.8.1/images/fig-nlte-Ni.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-08-01 11:56:42.000000 artistools-2023.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-01 11:56:42.000000 artistools-2023.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:58:18.702211 artistools-2023.8.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      902 2023-08-01 11:56:42.000000 artistools-2023.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.702211 artistools-2023.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:56:42.000000 artistools-2023.8.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.702211 artistools-2023.8.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 11:56:42.000000 artistools-2023.8.1/tests/data/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      455 2023-08-01 11:56:42.000000 artistools-2023.8.1/tests/data/setuptestdata.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.702211 artistools-2023.8.1/tests/data/testmodel_3d_10^3/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 11:56:42.000000 artistools-2023.8.1/tests/data/testmodel_3d_10^3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    76456 2023-08-01 11:56:42.000000 artistools-2023.8.1/tests/data/testmodel_3d_10^3/abundances.txt.xz
+-rw-r--r--   0 runner    (1001) docker     (123)    27560 2023-08-01 11:56:42.000000 artistools-2023.8.1/tests/data/testmodel_3d_10^3/model.txt.xz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:58:18.702211 artistools-2023.8.1/tests/output/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-01 11:56:42.000000 artistools-2023.8.1/tests/output/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      497 2023-08-01 11:56:42.000000 artistools-2023.8.1/tests/plottransitions_example.sh
```

### Comparing `artistools-2023.5.16.3/.codecov.yml` & `artistools-2023.8.1/.codecov.yml`

 * *Files 20% similar despite different names*

```diff
@@ -15,7 +15,8 @@
     # patch:
     #   default:
     #     target: auto
     #     threshold: 0%
     #     if_ci_failed: ignore #success, failure, error, ignore
     #     informational: true
     #     only_pulls: false
+comment: false
```

### Comparing `artistools-2023.5.16.3/.github/workflows/deploypypi.yml` & `artistools-2023.8.1/.github/workflows/deploypypi.yml`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/.github/workflows/deploytestpypi.yml` & `artistools-2023.8.1/.github/workflows/deploytestpypi.yml`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/.github/workflows/linter.yml` & `artistools-2023.8.1/.github/workflows/linter.yml`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
             - name: Install dependencies
               run: |
                   python3 -m pip install --upgrade pip wheel mypy
                   python3 -m pip install -r requirements.txt
             - name: Lint with mypy
               run: |
-                  mkdir -p .mypy_cache
                   mypy --install-types --non-interactive
 
     pylint:
         runs-on: ubuntu-latest
         steps:
             - name: Checkout Code
               uses: actions/checkout@v3
@@ -73,15 +72,15 @@
                   # Full git history is needed to get a proper list of changed files within `super-linter`
                   fetch-depth: 0
 
             - name: Lint Code Base
               uses: github/super-linter/slim@v5.0.0
               env:
                   LINTER_RULES_PATH: ./
-                  #   LOG_LEVEL: WARNING
+                  LOG_LEVEL: WARN
                   VALIDATE_GITLEAKS: false
                   VALIDATE_JSCPD: false
                   VALIDATE_PYTHON_BLACK: false
                   VALIDATE_PYTHON_FLAKE8: false
                   VALIDATE_PYTHON_ISORT: false
                   VALIDATE_PYTHON_PYLINT: false
                   VALIDATE_PYTHON_MYPY: false
```

### Comparing `artistools-2023.5.16.3/.github/workflows/pytest.yml` & `artistools-2023.8.1/.github/workflows/pytest.yml`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,19 @@
     merge_group:
 
 jobs:
     pytest:
         timeout-minutes: 10
         runs-on: ${{ matrix.os }}
         strategy:
+            fail-fast: false
             matrix:
                 # os: [ubuntu-latest, macos-latest]
                 os: [ubuntu-latest]
-                python-version: ['3.9', '3.10', '3.11']
+                python-version: ['3.10', '3.11']
         env:
             OS: ${{ matrix.os }}
             PYTHON: ${{ matrix.python-version }}
 
         steps:
             - name: Checkout Code
               uses: actions/checkout@v3
```

### Comparing `artistools-2023.5.16.3/.gitignore` & `artistools-2023.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/.pre-commit-config.yaml` & `artistools-2023.8.1/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -25,22 +25,32 @@
           - id: requirements-txt-fixer
           - id: trailing-whitespace
     - repo: https://github.com/jumanjihouse/pre-commit-hook-yamlfmt
       rev: 0.2.3
       hooks:
           - id: yamlfmt
     - repo: https://github.com/charliermarsh/ruff-pre-commit
-      rev: v0.0.267
+      rev: v0.0.281
       hooks:
           - id: ruff
             args: [--fix, --exit-non-zero-on-fix]
     - repo: https://github.com/psf/black
-      rev: 23.3.0
+      rev: 23.7.0
       hooks:
           - id: black
-    - repo: https://github.com/pre-commit/mirrors-mypy
-      rev: v1.3.0
+    # - repo: https://github.com/pre-commit/mirrors-mypy
+    #   rev: v1.4.1
+    #   hooks:
+    #       - id: mypy
+    #         additional_dependencies: [numpy, types-PyYAML, pandas>=2.0.3, polars>=0.18.10]
+    #         types: [python]
+    #         require_serial: true
+    - repo: local
       hooks:
           - id: mypy
-            additional_dependencies: [numpy, types-PyYAML, types-psutil]
+            name: mypy
+            entry: dmypy
             types: [python]
+            # files: \.py$
+            language: python
             require_serial: true
+            args: [run, --, --cache-fine-grained]
```

### Comparing `artistools-2023.5.16.3/CODEOWNERS` & `artistools-2023.8.1/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/LICENSE.txt` & `artistools-2023.8.1/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2017-2022 ARTIS Collaboration
+Copyright (c) 2017-2023 ARTIS Collaboration
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `artistools-2023.5.16.3/README.md` & `artistools-2023.8.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # Artistools
 
 > Artistools is collection of plotting, analysis, and file format conversion tools for the [ARTIS](https://github.com/artis-mcrt/artis) radiative transfer code.
 
+[![DOI](https://zenodo.org/badge/53433932.svg)](https://zenodo.org/badge/latestdoi/53433932)
 ![GitHub Build and test status](https://github.com/artis-mcrt/artistools/workflows/Build%20and%20test/badge.svg)
 [![codecov](https://codecov.io/gh/artis-mcrt/artistools/branch/main/graph/badge.svg?token=XFlarJqeZd)](https://codecov.io/gh/artis-mcrt/artistools)
-[![CodeFactor](https://www.codefactor.io/repository/github/artis-mcrt/artistools/badge)](https://www.codefactor.io/repository/github/artis-mcrt/artistools)
 
 ## Installation
 Requires Python >= 3.9
 
-First clone the repository, for example:
+artistools can be installed from PyPI using `pip install artistools'. For development, clone the repository and make an editable install:
 ```sh
 git clone https://github.com/artis-mcrt/artistools.git
-```
-Then from within the repository directory run:
-```sh
+cd artistools
 python3 -m pip install -e .
 pre-commit install
 ```
 
 ## Usage
 Type "artistools" at the command-line to get a full list of commands. The most frequently used commands are:
 - plotartisestimators
@@ -36,7 +34,12 @@
 ![NLTE plot](https://github.com/artis-mcrt/artistools/raw/main/images/fig-nlte-Ni.png)
 ![Estimator plot](https://github.com/artis-mcrt/artistools/raw/main/images/fig-estimators.png)
 
 ## License
 Distributed under the MIT license. See [LICENSE](https://github.com/artis-mcrt/artistools/blob/main/LICENSE) for more information.
 
 [https://github.com/artis-mcrt/artistools](https://github.com/artis-mcrt/artistools)
+
+
+## Citing Artistools
+
+If you make use of artistools please cite it. For details, see [https://zenodo.org/badge/latestdoi/53433932](https://zenodo.org/badge/latestdoi/53433932).
```

### Comparing `artistools-2023.5.16.3/artistools/__init__.py` & `artistools-2023.8.1/artistools/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """artistools.
 
 A collection of plotting, analysis, and file format conversion tools
 for the ARTIS radiative transfer code.
 """
-import artistools.atomic
-import artistools.codecomparison
-import artistools.commands
-import artistools.deposition
-import artistools.estimators
-import artistools.inputmodel
-import artistools.lightcurve
-import artistools.macroatom
-import artistools.nltepops
-import artistools.nonthermal
-import artistools.packets
-import artistools.plotspherical
-import artistools.radfield
-import artistools.spectra
-import artistools.transitions
-import artistools.writecomparisondata
 
+import typing as t
+
+from . import atomic
+from . import codecomparison
+from . import commands
+from . import deposition
+from . import estimators
+from . import initial_composition
+from . import inputmodel
+from . import lightcurve
+from . import macroatom
+from . import nltepops
+from . import nonthermal
+from . import packets
+from . import plotspherical
+from . import radfield
+from . import spectra
+from . import transitions
+from . import writecomparisondata
 from .__main__ import addargs
 from .__main__ import main
 from .configuration import get_config
 from .configuration import set_config
 from .inputmodel import add_derived_cols_to_modeldata
 from .inputmodel import get_2d_modeldata
 from .inputmodel import get_cell_angle
@@ -68,15 +71,15 @@
 from .misc import get_nu_grid
 from .misc import get_phi_bins
 from .misc import get_runfolders
 from .misc import get_syn_dir
 from .misc import get_time_range
 from .misc import get_timestep_of_timedays
 from .misc import get_timestep_time
-from .misc import get_timestep_times_float
+from .misc import get_timestep_times
 from .misc import get_viewingdirection_costhetabincount
 from .misc import get_viewingdirection_phibincount
 from .misc import get_viewingdirectionbincount
 from .misc import get_vpkt_config
 from .misc import get_vspec_dir_labels
 from .misc import get_wid_init_at_tmin
 from .misc import get_wid_init_at_tmodel
@@ -95,8 +98,13 @@
 from .misc import split_dataframe_dirbins
 from .misc import stripallsuffixes
 from .misc import trim_or_pad
 from .misc import vec_len
 from .misc import zopen
 from .plottools import set_mpl_style
 
+
+def get_path(**kwargs: t.Any) -> None:
+    print(get_config("path_artistools_dir"))
+
+
 set_mpl_style()
```

### Comparing `artistools-2023.5.16.3/artistools/__main__.py` & `artistools-2023.8.1/artistools/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # PYTHON_ARGCOMPLETE_OK
+from __future__ import annotations
+
 import argparse
 import importlib
-from typing import Optional
 
 import argcomplete
 
 from .commands import dictcommands as atdictcommands
 from .misc import CustomArgHelpFormatter
 
 
@@ -17,15 +18,15 @@
     def func(args) -> None:
         parser.print_help()
 
     parser.set_defaults(func=func)
     subparsers = parser.add_subparsers(dest=f"{parentcommand} command", required=False)
 
     for subcommand, subcommands in dictcommands.items():
-        strhelp: Optional[str]
+        strhelp: str | None
         if isinstance(subcommands, dict):
             strhelp = "command group"
             submodule = None
         else:
             submodulename, funcname = subcommands
             namestr = f"artistools.{submodulename.removeprefix('artistools.')}" if submodulename else "artistools"
             submodule = importlib.import_module(namestr, package="artistools")
```

### Comparing `artistools-2023.5.16.3/artistools/atomic/_atomic_core.py` & `artistools-2023.8.1/artistools/atomic/_atomic_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,17 +104,15 @@
             targetlist = []
             ntargets = int(fphixs.readline())
             for _ in range(ntargets):
                 level, fraction = fphixs.readline().split()
                 targetlist.append((int(level) - firstlevelnumber, float(fraction)))
 
         if not ionlist or (Z, lowerionstage) in ionlist:
-            phixslist = []
-            for _ in range(nphixspoints):
-                phixslist.append(float(fphixs.readline()) * 1e-18)
+            phixslist = [float(fphixs.readline()) * 1e-18 for _ in range(nphixspoints)]
             phixstable = np.array(list(zip(xgrid, phixslist)))
 
             yield Z, upperionstage, upperionlevel, lowerionstage, lowerionlevel, targetlist, phixstable
 
         else:
             for _ in range(nphixspoints):
                 fphixs.readline()
@@ -161,16 +159,15 @@
         if not quiet:
             print(f"Reading {adatafilename.relative_to(Path(modelpath).parent)}")
 
         for Z, ionstage, level_count, ionisation_energy_ev, dflevels in parse_adata(fadata, phixsdict, ionlist):
             translist = transitionsdict.get((Z, ionstage), pd.DataFrame())
             level_lists.append(iontuple(Z, ionstage, level_count, ionisation_energy_ev, dflevels, translist))
 
-    dfadata = pd.DataFrame(level_lists)
-    return dfadata
+    return pd.DataFrame(level_lists)
 
 
 def parse_recombratefile(frecomb):
     for line in frecomb:
         Z, upper_ionstage, t_count = (int(x) for x in line.split())
         arr_log10t = []
         arr_rrc_low_n = []
```

### Comparing `artistools-2023.5.16.3/artistools/codecomparison.py` & `artistools-2023.8.1/artistools/codecomparison.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """File readers for Blondin et al. code comparison file formats
 The model paths are not real file system paths, but take a form like this:
 codecomparison/[modelname]/[codename].
 
 e.g., codecomparison/DDC10/artisnebular
 """
+from __future__ import annotations
+
 import math
-from collections.abc import Sequence
+import typing as t
 from pathlib import Path
-from typing import Any
-from typing import Literal
-from typing import Union
 
-import matplotlib.axes
 import numpy as np
 import pandas as pd
 
 import artistools as at
 
+if t.TYPE_CHECKING:
+    import matplotlib.axes
+
 
-def get_timestep_times_float(
-    modelpath: Union[Path, str], loc: Literal["start", "mid", "end", "delta"] = "mid"
-) -> np.ndarray[Any, np.dtype[np.float64]]:
+def get_timestep_times(
+    modelpath: Path | str, loc: t.Literal["start", "mid", "end", "delta"] = "mid"
+) -> np.ndarray[t.Any, np.dtype[np.float64]]:
     modelpath = Path(modelpath)
     _, modelname, codename = modelpath.parts
 
     filepath = Path(at.get_config()["codecomparisondata1path"], modelname, f"phys_{modelname}_{codename}.txt")
 
-    with open(filepath, encoding="utf-8") as fphys:
+    with filepath.open(encoding="utf-8") as fphys:
         _ = int(fphys.readline().replace("#NTIMES:", ""))
         tmids = np.array([float(x) for x in fphys.readline().replace("#TIMES[d]:", "").split()])
 
     tstarts = np.zeros_like(tmids)
     tstarts[1:] = (tmids[1:] + tmids[:-1]) / 2.0
     tstarts[0] = tmids[0] - (tstarts[1] - tmids[0])
 
@@ -41,38 +42,36 @@
     if loc == "mid":
         return tmids
     if loc == "start":
         return tstarts
     if loc == "end":
         return tends
     if loc == "delta":
-        tdeltas = tends - tstarts
-        return tdeltas
-
+        return tends - tstarts
     msg = "loc must be one of 'mid', 'start', 'end', or 'delta'"
     raise ValueError(msg)
 
 
 def read_reference_estimators(
-    modelpath: Union[str, Path],
-    modelgridindex: Union[None, int, Sequence[int]] = None,
-    timestep: Union[None, int, Sequence[int]] = None,
-) -> dict[tuple[int, int], Any]:
+    modelpath: str | Path,
+    modelgridindex: None | int | t.Sequence[int] = None,
+    timestep: None | int | t.Sequence[int] = None,
+) -> dict[tuple[int, int], t.Any]:
     """Read estimators from code comparison workshop file."""
     virtualfolder, inputmodel, codename = Path(modelpath).parts
     assert virtualfolder == "codecomparison"
 
     inputmodelfolder = Path(at.get_config()["codecomparisondata1path"], inputmodel)
 
     physfilepath = Path(inputmodelfolder, f"phys_{inputmodel}_{codename}.txt")
 
-    estimators: dict[tuple[int, int], Any] = {}
+    estimators: dict[tuple[int, int], t.Any] = {}
     cur_timestep = -1
     cur_modelgridindex = -1
-    with open(physfilepath) as fphys:
+    with physfilepath.open() as fphys:
         ntimes = int(fphys.readline().replace("#NTIMES:", ""))
         arr_timedays = np.array([float(x) for x in fphys.readline().replace("#TIMES[d]:", "").split()])
         assert len(arr_timedays) == ntimes
 
         for line in fphys:
             row = line.split()
 
@@ -101,15 +100,15 @@
 
                 estimators[key]["velocity_outer"] = estimators[key]["vel_mid"]
 
     ionfracfilepaths = inputmodelfolder.glob(f"ionfrac_*_{inputmodel}_{codename}.txt")
     for ionfracfilepath in ionfracfilepaths:
         _, element, _, _ = ionfracfilepath.stem.split("_")
 
-        with open(ionfracfilepath) as fions:
+        with Path(ionfracfilepath).open() as fions:
             print(ionfracfilepath)
             ntimes_2 = int(fions.readline().replace("#NTIMES:", ""))
             assert ntimes_2 == ntimes
 
             nstages = int(fions.readline().replace("#NSTAGES:", ""))
 
             arr_timedays_2 = np.array([float(x) for x in fions.readline().replace("#TIMES[d]:", "").split()])
@@ -171,39 +170,37 @@
 
                     assert np.isclose(float(row[0]), estimators[tsmgi]["vel_mid"], rtol=0.01)
                     assert estimators[key]["vel_mid"]
 
     return estimators
 
 
-def get_spectra(modelpath: Union[str, Path]) -> tuple[pd.DataFrame, np.ndarray]:
+def get_spectra(modelpath: str | Path) -> tuple[pd.DataFrame, np.ndarray]:
     modelpath = Path(modelpath)
     virtualfolder, inputmodel, codename = modelpath.parts
     assert virtualfolder == "codecomparison"
 
     inputmodelfolder = Path(at.get_config()["codecomparisondata1path"], inputmodel)
 
     specfilepath = Path(inputmodelfolder, f"spectra_{inputmodel}_{codename}.txt")
 
-    with open(specfilepath) as fspec:
+    with specfilepath.open() as fspec:
         ntimes = int(fspec.readline().replace("#NTIMES:", ""))
         _ = int(fspec.readline().replace("#NWAVE:", ""))
         arr_timedays = np.array([float(x) for x in fspec.readline().split()[1:]])
         assert len(arr_timedays) == ntimes
 
         dfspectra = pd.read_csv(
             fspec, delim_whitespace=True, header=None, names=["lambda", *list(arr_timedays)], comment="#"
         )
 
     return dfspectra, arr_timedays
 
 
-def plot_spectrum(
-    modelpath: Union[str, Path], timedays: Union[str, float], axis: matplotlib.axes.Axes, **plotkwargs
-) -> None:
+def plot_spectrum(modelpath: str | Path, timedays: str | float, axis: matplotlib.axes.Axes, **plotkwargs) -> None:
     dfspectra, arr_timedays = get_spectra(modelpath)
     timeindex = (np.abs(arr_timedays - float(timedays))).argmin()
     timedays_found = dfspectra.columns[timeindex + 1]
 
     print(f"{modelpath}: requested spectrum at {timedays} days. Closest matching spectrum is at {timedays_found} days")
     assert np.isclose(arr_timedays[timeindex], float(timedays_found), rtol=0.01)  # check columns match
     assert np.isclose(float(timedays), float(timedays_found), rtol=0.1)  # found a detect match to requested time
```

### Comparing `artistools-2023.5.16.3/artistools/commands.py` & `artistools-2023.8.1/artistools/commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,23 @@
+from __future__ import annotations
+
 import argparse
 import subprocess
+import typing as t
 from pathlib import Path
-from typing import Any
-from typing import Union
-
-try:
-    from typing_extensions import TypeAlias
-except ImportError:
-    from typing import TypeAlias
 
-cmdtype: TypeAlias = dict[str, Union[tuple[str, str], "cmdtype"]]
+cmdtype: t.TypeAlias = dict[str, t.Union[tuple[str, str], "cmdtype"]]
 
+# new subparser based list
 dictcommands: cmdtype = {
     "comparetogsinetwork": ("gsinetwork", "main"),
     "deposition": ("deposition", "main_analytical"),
     "describeinputmodel": ("inputmodel.describeinputmodel", "main"),
     "exportmassfractions": ("estimators.exportmassfractions", "main"),
+    "getpath": ("", "get_path"),
     "listtimesteps": ("", "showtimesteptimes"),
     "makeartismodelfromparticlegridmap": ("inputmodel.modelfromhydro", "main"),
     "maketardismodelfromartis": ("inputmodel.maketardismodelfromartis", "main"),
     "maptogrid": ("inputmodel.maptogrid", "main"),
     "plotestimators": ("estimators.plotestimators", "main"),
     "plotinitialcomposition": ("initial_composition", "main"),
     "plotlightcurves": ("lightcurve.plotlightcurve", "main"),
@@ -52,45 +50,104 @@
         "makeartismodelsolar_rprocess": ("inputmodel.rprocess_solar", "main"),
         "makeartismodelfromsingletrajectory": ("inputmodel.rprocess_from_trajectory", "main"),
     },
 }
 
 
 def get_commandlist() -> dict[str, tuple[str, str]]:
-    commandlist = {
+    # direct commands (one file installed per command)
+    # we generally should phase this out except for a couple of main ones like at and artistools
+    return {
         "at": ("artistools", "main"),
         "artistools": ("artistools", "main"),
         "artistools-comparetogsinetwork": ("artistools.gsinetwork", "main"),
-        "artistools-modeldeposition": ("artistools.deposition", "main_analytical"),
-        "getartisspencerfano": ("artistools.nonthermal.solvespencerfanocmd", "main"),
-        "artistools-spencerfano": ("artistools.nonthermal.solvespencerfanocmd", "main"),
+        "artistools-modeldeposition": (
+            "artistools.deposition",
+            "main_analytical",
+        ),
+        "getartisspencerfano": (
+            "artistools.nonthermal.solvespencerfanocmd",
+            "main",
+        ),
+        "artistools-spencerfano": (
+            "artistools.nonthermal.solvespencerfanocmd",
+            "main",
+        ),
         "listartistimesteps": ("artistools", "showtimesteptimes"),
         "artistools-timesteptimes": ("artistools", "showtimesteptimes"),
-        "artistools-make1dslicefrom3dmodel": ("artistools.inputmodel.1dslicefrom3d", "main"),
-        "makeartismodel1dslicefromcone": ("artistools.inputmodel.slice1Dfromconein3dmodel", "main"),
-        "makeartismodelbotyanski2017": ("artistools.inputmodel.botyanski2017", "main"),
-        "makeartismodelfromshen2018": ("artistools.inputmodel.shen2018", "main"),
-        "makeartismodelfromlapuente": ("artistools.inputmodel.lapuente", "main"),
-        "makeartismodelscalevelocity": ("artistools.inputmodel.scalevelocity", "main"),
-        "makeartismodelfullymixed": ("artistools.inputmodel.fullymixed", "main"),
-        "makeartismodelsolar_rprocess": ("artistools.inputmodel.rprocess_solar", "main"),
-        "makeartismodelfromsingletrajectory": ("artistools.inputmodel.rprocess_from_trajectory", "main"),
-        "makeartismodelfromparticlegridmap": ("artistools.inputmodel.modelfromhydro", "main"),
+        "artistools-make1dslicefrom3dmodel": (
+            "artistools.inputmodel.1dslicefrom3d",
+            "main",
+        ),
+        "makeartismodel1dslicefromcone": (
+            "artistools.inputmodel.slice1Dfromconein3dmodel",
+            "main",
+        ),
+        "makeartismodelbotyanski2017": (
+            "artistools.inputmodel.botyanski2017",
+            "main",
+        ),
+        "makeartismodelfromshen2018": (
+            "artistools.inputmodel.shen2018",
+            "main",
+        ),
+        "makeartismodelfromlapuente": (
+            "artistools.inputmodel.lapuente",
+            "main",
+        ),
+        "makeartismodelscalevelocity": (
+            "artistools.inputmodel.scalevelocity",
+            "main",
+        ),
+        "makeartismodelfullymixed": (
+            "artistools.inputmodel.fullymixed",
+            "main",
+        ),
+        "makeartismodelsolar_rprocess": (
+            "artistools.inputmodel.rprocess_solar",
+            "main",
+        ),
+        "makeartismodelfromsingletrajectory": (
+            "artistools.inputmodel.rprocess_from_trajectory",
+            "main",
+        ),
+        "makeartismodelfromparticlegridmap": (
+            "artistools.inputmodel.modelfromhydro",
+            "main",
+        ),
         "makeartismodel": ("artistools.inputmodel.makeartismodel", "main"),
-        "artistools-maketardismodelfromartis": ("artistools.inputmodel.maketardismodelfromartis", "main"),
+        "artistools-maketardismodelfromartis": (
+            "artistools.inputmodel.maketardismodelfromartis",
+            "main",
+        ),
         "artistools-maptogrid": ("artistools.inputmodel.maptogrid", "main"),
         "plotartismodeldensity": ("artistools.inputmodel.plotdensity", "main"),
-        "artistools-plotdensity": ("artistools.inputmodel.plotdensity", "main"),
+        "artistools-plotdensity": (
+            "artistools.inputmodel.plotdensity",
+            "main",
+        ),
         "plotartismodeldeposition": ("artistools.deposition", "main"),
         "artistools-deposition": ("artistools.deposition", "main"),
-        "artistools-describeinputmodel": ("artistools.inputmodel.describeinputmodel", "main"),
-        "plotartisestimators": ("artistools.estimators.plotestimators", "main"),
+        "artistools-describeinputmodel": (
+            "artistools.inputmodel.describeinputmodel",
+            "main",
+        ),
+        "plotartisestimators": (
+            "artistools.estimators.plotestimators",
+            "main",
+        ),
         "artistools-estimators": ("artistools.estimators", "main"),
-        "artistools-exportmassfractions": ("artistools.estimators.exportmassfractions", "main"),
-        "plotartislightcurve": ("artistools.lightcurve.plotlightcurve", "main"),
+        "artistools-exportmassfractions": (
+            "artistools.estimators.exportmassfractions",
+            "main",
+        ),
+        "plotartislightcurve": (
+            "artistools.lightcurve.plotlightcurve",
+            "main",
+        ),
         "artistools-lightcurve": ("artistools.lightcurve", "main"),
         "plotartislinefluxes": ("artistools.linefluxes", "main"),
         "artistools-linefluxes": ("artistools.linefluxes", "main"),
         "plotartismacroatom": ("artistools.macroatom", "main"),
         "artistools-macroatom": ("artistools.macroatom", "main"),
         "plotartisnltepops": ("artistools.nltepops.plotnltepops", "main"),
         "artistools-nltepops": ("artistools.nltepops", "main"),
@@ -98,39 +155,54 @@
         "artistools-nonthermal": ("artistools.nonthermal", "main"),
         "plotartisradfield": ("artistools.radfield", "main"),
         "artistools-radfield": ("artistools.radfield", "main"),
         "plotartisspectrum": ("artistools.spectra.plotspectra", "main"),
         "artistools-spectrum": ("artistools.spectra", "main"),
         "plotartistransitions": ("artistools.transitions", "main"),
         "artistools-transitions": ("artistools.transitions", "main"),
-        "plotartisinitialcomposition": ("artistools.initial_composition", "main"),
-        "artistools-initialcomposition": ("artistools.initial_composition", "main"),
-        "artistools-writecodecomparisondata": ("artistools.writecomparisondata", "main"),
-        "artistools-setup_completions": ("artistools.commands", "setup_completions"),
-        "artistools-viewingangles": ("artistools.viewing_angles_visualization", "main"),
-        "plotartisviewingangles": ("artistools.viewing_angles_visualization", "main"),
+        "plotartisinitialcomposition": (
+            "artistools.initial_composition",
+            "main",
+        ),
+        "artistools-initialcomposition": (
+            "artistools.initial_composition",
+            "main",
+        ),
+        "artistools-writecodecomparisondata": (
+            "artistools.writecomparisondata",
+            "main",
+        ),
+        "artistools-setup_completions": (
+            "artistools.commands",
+            "setup_completions",
+        ),
+        "artistools-viewingangles": (
+            "artistools.viewing_angles_visualization",
+            "main",
+        ),
+        "plotartisviewingangles": (
+            "artistools.viewing_angles_visualization",
+            "main",
+        ),
     }
 
-    return commandlist
-
 
 def get_console_scripts() -> list[str]:
-    console_scripts = [
+    return [
         f"{command} = {submodulename}:{funcname}" for command, (submodulename, funcname) in get_commandlist().items()
     ]
-    return console_scripts
 
 
-def setup_completions(*args: Any, **kwargs: Any) -> None:
+def setup_completions(*args: t.Any, **kwargs: t.Any) -> None:
     # Add the following lines to your .zshrc file to get command completion:
     # autoload -U bashcompinit
     # bashcompinit
     # source artistoolscompletions.sh
     path_repo = Path(__file__).absolute().parent.parent
-    with open(path_repo / "artistoolscompletions.sh", "w", encoding="utf-8") as f:
+    with (path_repo / "artistoolscompletions.sh").open("w", encoding="utf-8") as f:
         f.write("#!/usr/bin/env zsh\n")
 
         proc = subprocess.run(
             ["register-python-argcomplete", "__MY_COMMAND__"], capture_output=True, text=True, check=True
         )
 
         if proc.stderr:
```

### Comparing `artistools-2023.5.16.3/artistools/data/ElBiEn_2007.txt` & `artistools-2023.8.1/artistools/data/ElBiEn_2007.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/atomic_properties.txt` & `artistools-2023.8.1/artistools/data/atomic_properties.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/betaminusdecays.txt` & `artistools-2023.8.1/artistools/data/betaminusdecays.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/binding_energies.txt` & `artistools-2023.8.1/artistools/data/binding_energies.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/collion-AR1985.txt` & `artistools-2023.8.1/artistools/data/collion-AR1985.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/collion-reference.txt` & `artistools-2023.8.1/artistools/data/collion-reference.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/collion.txt` & `artistools-2023.8.1/artistools/data/collion.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/elements.csv` & `artistools-2023.8.1/artistools/data/elements.csv`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/400.txt` & `artistools-2023.8.1/artistools/data/filters/400.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/520.txt` & `artistools-2023.8.1/artistools/data/filters/520.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/B.txt` & `artistools-2023.8.1/artistools/data/filters/ASIAGO/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/U.txt` & `artistools-2023.8.1/artistools/data/filters/ASIAGO/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/V.txt` & `artistools-2023.8.1/artistools/data/filters/ASIAGO/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/gs.txt` & `artistools-2023.8.1/artistools/data/filters/ASIAGO/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/is.txt` & `artistools-2023.8.1/artistools/data/filters/ASIAGO/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/rs.txt` & `artistools-2023.8.1/artistools/data/filters/ASIAGO/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/ASIAGO/zs.txt` & `artistools-2023.8.1/artistools/data/filters/ASIAGO/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/B.txt` & `artistools-2023.8.1/artistools/data/filters/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/FUV.txt` & `artistools-2023.8.1/artistools/data/filters/FUV.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/H.txt` & `artistools-2023.8.1/artistools/data/filters/H.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/H_ab.txt` & `artistools-2023.8.1/artistools/data/filters/H_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/I.txt` & `artistools-2023.8.1/artistools/data/filters/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/J.txt` & `artistools-2023.8.1/artistools/data/filters/J.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/J_ab.txt` & `artistools-2023.8.1/artistools/data/filters/J_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/K.txt` & `artistools-2023.8.1/artistools/data/filters/K.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/K_ab.txt` & `artistools-2023.8.1/artistools/data/filters/K_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LCOGT/B.txt` & `artistools-2023.8.1/artistools/data/filters/LCOGT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LCOGT/I.txt` & `artistools-2023.8.1/artistools/data/filters/LCOGT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LCOGT/R.txt` & `artistools-2023.8.1/artistools/data/filters/LCOGT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LCOGT/U.txt` & `artistools-2023.8.1/artistools/data/filters/LCOGT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LCOGT/V.txt` & `artistools-2023.8.1/artistools/data/filters/LCOGT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LCOGT/gs.txt` & `artistools-2023.8.1/artistools/data/filters/LCOGT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LCOGT/is.txt` & `artistools-2023.8.1/artistools/data/filters/LCOGT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LCOGT/rs.txt` & `artistools-2023.8.1/artistools/data/filters/LCOGT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LCOGT/us.txt` & `artistools-2023.8.1/artistools/data/filters/LCOGT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LCOGT/zs.txt` & `artistools-2023.8.1/artistools/data/filters/LCOGT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LSQ/rs.txt` & `artistools-2023.8.1/artistools/data/filters/LSQ/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LT/gs.txt` & `artistools-2023.8.1/artistools/data/filters/LT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LT/is.txt` & `artistools-2023.8.1/artistools/data/filters/LT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LT/rs.txt` & `artistools-2023.8.1/artistools/data/filters/LT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LT/us.txt` & `artistools-2023.8.1/artistools/data/filters/LT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/LT/zs.txt` & `artistools-2023.8.1/artistools/data/filters/LT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NOT/B.txt` & `artistools-2023.8.1/artistools/data/filters/NOT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NOT/I.txt` & `artistools-2023.8.1/artistools/data/filters/NOT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NOT/R.txt` & `artistools-2023.8.1/artistools/data/filters/NOT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NOT/U.txt` & `artistools-2023.8.1/artistools/data/filters/NOT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NOT/V.txt` & `artistools-2023.8.1/artistools/data/filters/NOT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NOT/gs.txt` & `artistools-2023.8.1/artistools/data/filters/NOT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NOT/is.txt` & `artistools-2023.8.1/artistools/data/filters/NOT/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NOT/rs.txt` & `artistools-2023.8.1/artistools/data/filters/NOT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NOT/us.txt` & `artistools-2023.8.1/artistools/data/filters/NOT/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NOT/zs.txt` & `artistools-2023.8.1/artistools/data/filters/NOT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NTT/B.txt` & `artistools-2023.8.1/artistools/data/filters/NTT/B.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NTT/I.txt` & `artistools-2023.8.1/artistools/data/filters/NTT/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NTT/R.txt` & `artistools-2023.8.1/artistools/data/filters/NTT/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NTT/U.txt` & `artistools-2023.8.1/artistools/data/filters/NTT/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NTT/V.txt` & `artistools-2023.8.1/artistools/data/filters/NTT/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NTT/gs.txt` & `artistools-2023.8.1/artistools/data/filters/NTT/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NTT/rs.txt` & `artistools-2023.8.1/artistools/data/filters/NTT/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NTT/zs.txt` & `artistools-2023.8.1/artistools/data/filters/NTT/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/NUV.txt` & `artistools-2023.8.1/artistools/data/filters/NUV.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/OGLE/I.txt` & `artistools-2023.8.1/artistools/data/filters/OGLE/I.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/OGLE/V.txt` & `artistools-2023.8.1/artistools/data/filters/OGLE/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/PS1/gs.txt` & `artistools-2023.8.1/artistools/data/filters/PS1/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/PS1/is.txt` & `artistools-2023.8.1/artistools/data/filters/PS1/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/PS1/rs.txt` & `artistools-2023.8.1/artistools/data/filters/PS1/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/PS1/ws.txt` & `artistools-2023.8.1/artistools/data/filters/PS1/ws.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/PS1/zs.txt` & `artistools-2023.8.1/artistools/data/filters/PS1/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/R.txt` & `artistools-2023.8.1/artistools/data/filters/R.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/gs.txt` & `artistools-2023.8.1/artistools/data/filters/SKYMAPPER/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/is.txt` & `artistools-2023.8.1/artistools/data/filters/SKYMAPPER/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/rs.txt` & `artistools-2023.8.1/artistools/data/filters/SKYMAPPER/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/us.txt` & `artistools-2023.8.1/artistools/data/filters/SKYMAPPER/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/SKYMAPPER/zs.txt` & `artistools-2023.8.1/artistools/data/filters/SKYMAPPER/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/U.txt` & `artistools-2023.8.1/artistools/data/filters/U.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/V.txt` & `artistools-2023.8.1/artistools/data/filters/V.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/gs.txt` & `artistools-2023.8.1/artistools/data/filters/gs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/is.txt` & `artistools-2023.8.1/artistools/data/filters/is.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/rs.txt` & `artistools-2023.8.1/artistools/data/filters/rs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/us.txt` & `artistools-2023.8.1/artistools/data/filters/us.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/uvm2.txt` & `artistools-2023.8.1/artistools/data/filters/uvm2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/uvm2_ab.txt` & `artistools-2023.8.1/artistools/data/filters/uvm2_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/uvw1.txt` & `artistools-2023.8.1/artistools/data/filters/uvw1.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/uvw1_ab.txt` & `artistools-2023.8.1/artistools/data/filters/uvw1_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/uvw2.txt` & `artistools-2023.8.1/artistools/data/filters/uvw2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/uvw2_ab.txt` & `artistools-2023.8.1/artistools/data/filters/uvw2_ab.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/filters/zs.txt` & `artistools-2023.8.1/artistools/data/filters/zs.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt` & `artistools-2023.8.1/artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt` & `artistools-2023.8.1/artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt` & `artistools-2023.8.1/artistools/data/refspectra/2003du_20031213_3219_8822_00.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/2010lp_20110928_fors2.txt` & `artistools-2023.8.1/artistools/data/refspectra/2010lp_20110928_fors2.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii` & `artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-05-08_P200_DBSP_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii` & `artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-05-14_Keck1_LRIS_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii` & `artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-05-17_P200_DBSP_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii` & `artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-06-03_Keck1_MOSFIRE_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii` & `artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-06-08_P200_DBSP_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii` & `artistools-2023.8.1/artistools/data/refspectra/2018byg_2018-06-17_Keck1_LRIS_None.ascii`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz` & `artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57983.969_Phase+1.43d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz` & `artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57984.969_Phase+2.42d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz` & `artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57985.974_Phase+3.41d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz` & `artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57986.974_Phase+4.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz` & `artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57987.980_Phase+5.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz` & `artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57988.990_Phase+6.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz` & `artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57990.000_Phase+7.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz` & `artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57991.000_Phase+8.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz` & `artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57992.000_Phase+9.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz` & `artistools-2023.8.1/artistools/data/refspectra/AT2017gfo_ENGRAVE_v1.0_XSHOOTER_MJD-57993.000_Phase+10.40d.dat.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt` & `artistools-2023.8.1/artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt` & `artistools-2023.8.1/artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt` & `artistools-2023.8.1/artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt` & `artistools-2023.8.1/artistools/data/refspectra/SN2013aa_20140216_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt` & `artistools-2023.8.1/artistools/data/refspectra/SN2013aa_20140421_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt` & `artistools-2023.8.1/artistools/data/refspectra/SN2013cs_20140325_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt` & `artistools-2023.8.1/artistools/data/refspectra/SN2013ct_20131119_3Ang.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt` & `artistools-2023.8.1/artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt` & `artistools-2023.8.1/artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/data/solar_r_abundance_pattern.txt` & `artistools-2023.8.1/artistools/data/solar_r_abundance_pattern.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/deposition.py` & `artistools-2023.8.1/artistools/deposition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #!/usr/bin/env python3
+from __future__ import annotations
+
 import argparse
 import math
+import typing as t
 from math import exp
-from typing import Optional
 
 from astropy import units as u
 
 import artistools as at
 
 
 def forward_doubledecay(
@@ -41,15 +43,15 @@
 
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("-modelpath", default=".", help="Path to ARTIS folder")
 
     parser.add_argument("-timedays", "-t", default=330, type=float, help="Time in days")
 
 
-def main_analytical(args: Optional[argparse.Namespace] = None, argsraw: Optional[list[str]] = None, **kwargs) -> None:
+def main_analytical(args: argparse.Namespace | None = None, argsraw: list[str] | None = None, **kwargs: t.Any) -> None:
     """Use the model initial conditions to calculate the deposition rates."""
     if args is None:
         parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
     dfmodel, t_model_init, _ = at.inputmodel.get_modeldata_tuple(args.modelpath)
@@ -110,15 +112,15 @@
         #     nnlevel = dfnltepops_cell.query('level == 0', inplace=False).iloc[0]['n_NLTE']
         #     width = ((v_outer - v_inner) * t_now).to('cm').value
         #     tau = width * phixs * nnlevel
         #     print(f'width: {width:.3e} cm, phixs: {phixs:.3e} cm^2, nnlevel: {nnlevel:.3e} cm^-3, tau: {tau:.3e}')
     print(f'Global posdep: {global_posdep.to("solLum"):.3e}')
 
 
-def main(args: Optional[argparse.Namespace] = None, argsraw: Optional[list[str]] = None, **kwargs) -> None:
+def main(args: argparse.Namespace | None = None, argsraw: list[str] | None = None, **kwargs: t.Any) -> None:
     """Plot deposition rate of a model at time t (days)."""
     main_analytical(args=args, argsraw=argsraw, **kwargs)
     if args is None:
         parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
```

### Comparing `artistools-2023.5.16.3/artistools/estimators/__init__.py` & `artistools-2023.8.1/artistools/estimators/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""Artistools - estimators related functions."""
-
+"""Artistools - functions for handling data in estimators_????.out files (e.g., temperatures, densities, abundances)."""
+from . import estimators_classic
 from .estimators import apply_filters
 from .estimators import get_averaged_estimators
 from .estimators import get_averageexcitation
 from .estimators import get_averageionisation
 from .estimators import get_dictlabelreplacements
 from .estimators import get_ionrecombrates_fromfile
 from .estimators import get_partiallycompletetimesteps
```

### Comparing `artistools-2023.5.16.3/artistools/estimators/estimators.py` & `artistools-2023.8.1/artistools/estimators/estimators.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 #!/usr/bin/env python3
 """Functions for reading and processing estimator files.
 
 Examples are temperatures, populations, and heating/cooling rates.
 """
+
+from __future__ import annotations
+
 import argparse
+import contextlib
 import math
 import multiprocessing
 import sys
+import typing as t
 from collections import namedtuple
-from collections.abc import Collection
-from collections.abc import Iterator
-from collections.abc import Sequence
 from functools import partial
 from functools import reduce
 from pathlib import Path
-from typing import Any
-from typing import Optional
-from typing import Union
 
 import numpy as np
 import pandas as pd
+from typeguard import typechecked
 
 import artistools as at
-import artistools.nltepops
 
 
-def get_variableunits(key: Optional[str] = None) -> Union[str, dict[str, str]]:
+def get_variableunits(key: str | None = None) -> str | dict[str, str]:
     variableunits = {
         "time": "days",
         "gamma_NT": "/s",
         "gamma_R_bfest": "/s",
         "TR": "K",
         "Te": "K",
         "TJ": "K",
@@ -39,53 +38,53 @@
         "cooling": "erg/s/cm3",
         "velocity": "km/s",
         "velocity_outer": "km/s",
     }
     return variableunits[key] if key else variableunits
 
 
-def get_variablelongunits(key: Optional[str] = None) -> Union[str, dict[str, str]]:
+def get_variablelongunits(key: str | None = None) -> str | dict[str, str]:
     variablelongunits = {
         "heating_dep/total_dep": "",
         "TR": "Temperature [K]",
         "Te": "Temperature [K]",
         "TJ": "Temperature [K]",
     }
     return variablelongunits[key] if key else variablelongunits
 
 
-def get_dictlabelreplacements(key: Optional[str] = None) -> Union[str, dict[str, str]]:
+def get_dictlabelreplacements(key: str | None = None) -> str | dict[str, str]:
     dictlabelreplacements = {
         "lognne": "Log nne",
         "Te": "T$_e$",
         "TR": "T$_R$",
         "gamma_NT": r"$\Gamma_{\rm non-thermal}$ [s$^{-1}$]",
         "gamma_R_bfest": r"$\Gamma_{\rm phot}$ [s$^{-1}$]",
         "heating_dep/total_dep": "Heating fraction",
     }
     return dictlabelreplacements[key] if key else dictlabelreplacements
 
 
 def apply_filters(
-    xlist: Union[list, np.ndarray], ylist: Union[list, np.ndarray], args: argparse.Namespace
-) -> tuple[Union[list, np.ndarray], Union[list, np.ndarray]]:
+    xlist: list[float] | np.ndarray, ylist: list[float] | np.ndarray, args: argparse.Namespace
+) -> tuple[list[float] | np.ndarray, list[float] | np.ndarray]:
     filterfunc = at.get_filterfunc(args)
 
     if filterfunc is not None:
         ylist = filterfunc(ylist)
 
     return xlist, ylist
 
 
-def get_ionrecombrates_fromfile(filename: Union[Path, str]) -> pd.DataFrame:
+def get_ionrecombrates_fromfile(filename: Path | str) -> pd.DataFrame:
     """WARNING: copy pasted from artis-atomic! replace with a package import soon ionstage is the lower ion stage."""
     print(f"Reading {filename}")
 
     header_row = []
-    with open(filename) as filein:
+    with Path(filename).open() as filein:
         while True:
             line = filein.readline()
             if line.strip().startswith("TOTAL RECOMBINATION RATE"):
                 line = filein.readline()
                 line = filein.readline()
                 header_row = filein.readline().strip().replace(" n)", "-n)").split()
                 break
@@ -97,25 +96,23 @@
         index_logt = header_row.index("log(T)")
         index_low_n = header_row.index("RRC(low-n)")
         index_tot = header_row.index("RRC(total)")
 
         recomb_tuple = namedtuple("recomb_tuple", ["logT", "RRC_low_n", "RRC_total"])
         records = []
         for line in filein:
-            row = line.split()
-            if row:
+            if row := line.split():
                 if len(row) != len(header_row):
                     print("Row contains wrong number of items for header:")
                     print(header_row)
                     print(row)
                     sys.exit()
                 records.append(recomb_tuple(*[float(row[index]) for index in [index_logt, index_low_n, index_tot]]))
 
-    dfrecombrates = pd.DataFrame.from_records(records, columns=recomb_tuple._fields)
-    return dfrecombrates
+    return pd.DataFrame.from_records(records, columns=recomb_tuple._fields)
 
 
 def get_units_string(variable: str) -> str:
     if variable in get_variableunits():
         return f" [{get_variableunits(variable)}]"
     if variable.split("_")[0] in get_variableunits():
         return f' [{get_variableunits(variable.split("_")[0])}]'
@@ -124,47 +121,44 @@
 
 def parse_estimfile(
     estfilepath: Path,
     modelpath: Path,
     get_ion_values: bool = True,
     get_heatingcooling: bool = True,
     skip_emptycells: bool = False,
-) -> Iterator[tuple[int, int, dict]]:  # pylint: disable=unused-argument
+) -> t.Iterator[tuple[int, int, dict]]:  # pylint: disable=unused-argument
     """Generate timestep, modelgridindex, dict from estimator file."""
     with at.zopen(estfilepath) as estimfile:
         timestep: int = -1
         modelgridindex: int = -1
-        estimblock: dict[Any, Any] = {}
+        estimblock: dict[t.Any, t.Any] = {}
         for line in estimfile:
             row: list[str] = line.split()
             if not row:
                 continue
 
             if row[0] == "timestep":
                 # yield the previous block before starting a new one
                 if (
                     timestep >= 0
                     and modelgridindex >= 0
-                    and not (skip_emptycells and estimblock.get("emptycell", True))
+                    and (not skip_emptycells or not estimblock.get("emptycell", True))
                 ):
                     yield timestep, modelgridindex, estimblock
 
                 timestep = int(row[1])
                 # if timestep > itstep:
                 #     print(f"Dropping estimator data from timestep {timestep} and later (> itstep {itstep})")
                 #     # itstep in input.txt is updated by ARTIS at every timestep, so the data beyond here
                 #     # could be half-written to disk and cause parsing errors
                 #     return
 
                 modelgridindex = int(row[3])
-                # print(f'Timestep {timestep} cell {modelgridindex}')
-
-                estimblock = {}
                 emptycell = row[4] == "EMPTYCELL"
-                estimblock["emptycell"] = emptycell
+                estimblock = {"emptycell": emptycell}
                 if not emptycell:
                     # will be TR, Te, W, TJ, nne
                     for variablename, value in zip(row[4::2], row[5::2]):
                         estimblock[variablename] = float(value)
                     estimblock["lognne"] = math.log10(estimblock["nne"]) if estimblock["nne"] > 0 else float("-inf")
 
             elif row[1].startswith("Z=") and get_ion_values:
@@ -216,41 +210,41 @@
                     estimblock["populations"].setdefault("total", 0.0)
                     estimblock["populations"]["total"] += estimblock["populations"][atomic_number]
                     estimblock.setdefault("nntot", 0.0)
                     estimblock["nntot"] += estimblock["populations"][atomic_number]
 
             elif row[0] == "heating:" and get_heatingcooling:
                 for heatingtype, value in zip(row[1::2], row[2::2]):
-                    key = "heating_" + heatingtype if not heatingtype.startswith("heating_") else heatingtype
+                    key = heatingtype if heatingtype.startswith("heating_") else "heating_" + heatingtype
                     estimblock[key] = float(value)
 
                 if "heating_gamma/gamma_dep" in estimblock and estimblock["heating_gamma/gamma_dep"] > 0:
                     estimblock["gamma_dep"] = estimblock["heating_gamma"] / estimblock["heating_gamma/gamma_dep"]
                 elif "heating_dep/total_dep" in estimblock and estimblock["heating_dep/total_dep"] > 0:
                     estimblock["total_dep"] = estimblock["heating_dep"] / estimblock["heating_dep/total_dep"]
 
             elif row[0] == "cooling:" and get_heatingcooling:
                 for coolingtype, value in zip(row[1::2], row[2::2]):
                     estimblock["cooling_" + coolingtype] = float(value)
 
     # reached the end of file
-    if timestep >= 0 and modelgridindex >= 0 and not (skip_emptycells and estimblock.get("emptycell", True)):
+    if timestep >= 0 and modelgridindex >= 0 and (not skip_emptycells or not estimblock.get("emptycell", True)):
         yield timestep, modelgridindex, estimblock
 
 
 def read_estimators_from_file(
-    folderpath: Union[Path, str],
+    folderpath: Path | str,
     modelpath: Path,
-    arr_velocity_outer: Optional[Sequence[float]],
+    arr_velocity_outer: t.Sequence[float] | None,
     mpirank: int,
     printfilename: bool = False,
     get_ion_values: bool = True,
     get_heatingcooling: bool = True,
     skip_emptycells: bool = False,
-) -> dict[tuple[int, int], Any]:
+) -> dict[tuple[int, int], t.Any]:
     estimators_thisfile = {}
     estimfilename = f"estimators_{mpirank:04d}.out"
     try:
         estfilepath = at.firstexisting(estimfilename, folder=folderpath, tryzipped=True)
     except FileNotFoundError:
         # not worth printing an error, because ranks with no cells to update do not produce an estimator file
         # print(f'Warning: Could not find {estfilepath.relative_to(modelpath.parent)}')
@@ -272,74 +266,73 @@
             file_estimblock["velocity"] = file_estimblock["velocity_outer"]
 
         estimators_thisfile[(fileblock_timestep, fileblock_modelgridindex)] = file_estimblock
 
     return estimators_thisfile
 
 
+@typechecked
 def read_estimators(
-    modelpath: Union[Path, str] = Path(),
-    modelgridindex: Union[None, int, Sequence[int]] = None,
-    timestep: Union[None, int, Sequence[int]] = None,
-    mpirank: Optional[int] = None,
-    runfolder: Union[None, str, Path] = None,
+    modelpath: Path | str = Path(),
+    modelgridindex: None | int | t.Sequence[int] = None,
+    timestep: None | int | t.Sequence[int] = None,
+    mpirank: int | None = None,
+    runfolder: None | str | Path = None,
     get_ion_values: bool = True,
     get_heatingcooling: bool = True,
     skip_emptycells: bool = False,
     add_velocity: bool = True,
 ) -> dict[tuple[int, int], dict]:
     """Read estimator files into a nested dictionary structure.
 
     Speed it up by only retrieving estimators for a particular timestep(s) or modelgrid cells.
     """
     modelpath = Path(modelpath)
-    match_modelgridindex: Collection[int]
+    match_modelgridindex: t.Collection[int]
     if modelgridindex is None:
         match_modelgridindex = []
     elif isinstance(modelgridindex, int):
         match_modelgridindex = (modelgridindex,)
     else:
         match_modelgridindex = tuple(modelgridindex)
 
     if -1 in match_modelgridindex:
         match_modelgridindex = []
 
-    match_timestep: Collection[int]
+    match_timestep: t.Collection[int]
     if timestep is None:
         match_timestep = []
     elif isinstance(timestep, int):
         match_timestep = (timestep,)
     else:
         match_timestep = tuple(timestep)
 
     if not Path(modelpath).exists() and Path(modelpath).parts[0] == "codecomparison":
-        return artistools.codecomparison.read_reference_estimators(
-            modelpath, timestep=timestep, modelgridindex=modelgridindex
-        )
+        return at.codecomparison.read_reference_estimators(modelpath, timestep=timestep, modelgridindex=modelgridindex)
 
     # print(f" matching cells {match_modelgridindex} and timesteps {match_timestep}")
 
     arr_velocity_outer = None
     if add_velocity:
         modeldata, _ = at.inputmodel.get_modeldata(modelpath, getheadersonly=True)
         if "velocity_outer" in modeldata.columns:
             modeldata, _ = at.inputmodel.get_modeldata(modelpath)
-            arr_velocity_outer = tuple([float(v) for v in modeldata["velocity_outer"].to_numpy()])
+            arr_velocity_outer = tuple(float(v) for v in modeldata["velocity_outer"].to_numpy())
 
     mpiranklist = (
         at.get_mpiranklist(modelpath, modelgridindex=match_modelgridindex, only_ranks_withgridcells=True)
         if mpirank is None
         else [mpirank]
     )
 
     runfolders = at.get_runfolders(modelpath, timesteps=match_timestep) if runfolder is None else [Path(runfolder)]
 
     printfilename = len(mpiranklist) < 10
 
-    estimators = {}
+    estimators: dict[tuple[int, int], dict] = {}
     for folderpath in runfolders:
         if not printfilename:
             print(
                 f"Reading {len(list(mpiranklist))} estimator files in {folderpath.relative_to(Path(modelpath).parent)}"
             )
 
         processfile = partial(
@@ -371,69 +364,65 @@
                     print(
                         f"WARNING: Duplicate estimator block for (timestep, mgi) key {k}. "
                         f"Dropping block from {filepath}"
                     )
 
                 del estimators_thisfile[k]
 
-            estimators.update(estimators_thisfile)
+            estimators |= estimators_thisfile
 
     return estimators
 
 
 def get_averaged_estimators(
-    modelpath: Union[Path, str],
+    modelpath: Path | str,
     estimators: dict[tuple[int, int], dict],
-    timesteps: Union[int, Sequence[int]],
+    timesteps: int | t.Sequence[int],
     modelgridindex: int,
-    keys: Union[str, list],
+    keys: str | list,
     avgadjcells: int = 0,
-) -> Union[Any, float]:
+) -> t.Any | float:
     """Get the average of estimators[(timestep, modelgridindex)][keys[0]]...[keys[-1]] across timesteps."""
     if isinstance(keys, str):
         keys = [keys]
 
     # reduce(lambda d, k: d[k], keys, dictionary) returns dictionary[keys[0]][keys[1]]...[keys[-1]]
     # applying all keys in the keys list
 
     # if single timestep, no averaging needed
     if isinstance(timesteps, int):
         return reduce(lambda d, k: d[k], [(timesteps, modelgridindex), *keys], estimators)
 
     firsttimestepvalue = reduce(lambda d, k: d[k], [(timesteps[0], modelgridindex), *keys], estimators)
     if isinstance(firsttimestepvalue, dict):
-        dictout = {
+        return {
             k: get_averaged_estimators(modelpath, estimators, timesteps, modelgridindex, [*keys, k])
             for k in firsttimestepvalue
         }
 
-        return dictout
-
-    tdeltas = at.get_timestep_times_float(modelpath, loc="delta")
+    tdeltas = at.get_timestep_times(modelpath, loc="delta")
     valuesum = 0
     tdeltasum = 0
     for timestep, tdelta in zip(timesteps, tdeltas):
         for mgi in range(modelgridindex - avgadjcells, modelgridindex + avgadjcells + 1):
-            try:
+            with contextlib.suppress(KeyError):
                 valuesum += reduce(lambda d, k: d[k], [(timestep, mgi), *keys], estimators) * tdelta
                 tdeltasum += tdelta
-            except KeyError:
-                pass
     return valuesum / tdeltasum
 
     # except KeyError:
     #     if (timestep, modelgridindex) in estimators:
     #         print(f'Unknown x variable: {xvariable} for timestep {timestep} in cell {modelgridindex}')
     #     else:
     #         print(f'No data for cell {modelgridindex} at timestep {timestep}')
     #     print(estimators[(timestep, modelgridindex)])
     #     sys.exit()
 
 
-def get_averageionisation(populations: dict[Any, float], atomic_number: int) -> float:
+def get_averageionisation(populations: dict[t.Any, float], atomic_number: int) -> float:
     free_electron_weighted_pop_sum = 0.0
     found = False
     popsum = 0.0
     for key in populations:
         if isinstance(key, tuple) and key[0] == atomic_number:
             found = True
             ion_stage = key[1]
@@ -465,43 +454,34 @@
     k_b = 8.617333262145179e-05  # eV / K
 
     ionpopsum = dfnltepops_ion.n_NLTE.sum()
     energypopsum = (
         dfnltepops_ion[dfnltepops_ion.level >= 0].eval("@ionlevels.iloc[level].energy_ev.values * n_NLTE").sum()
     )
 
-    try:
+    with contextlib.suppress(IndexError):  # no superlevel with cause IndexError
         superlevelrow = dfnltepops_ion[dfnltepops_ion.level < 0].iloc[0]
         levelnumber_sl = dfnltepops_ion.level.max() + 1
 
         energy_boltzfac_sum = (
             ionlevels.iloc[levelnumber_sl:].eval("energy_ev * g * exp(- energy_ev / @k_b / @T_exc)").sum()
         )
 
         boltzfac_sum = ionlevels.iloc[levelnumber_sl:].eval("g * exp(- energy_ev / @k_b / @T_exc)").sum()
         # adjust to the actual superlevel population from ARTIS
         energypopsum += energy_boltzfac_sum * superlevelrow.n_NLTE / boltzfac_sum
-    except IndexError:
-        # no superlevel
-        pass
-
     return energypopsum / ionpopsum
 
 
-def get_partiallycompletetimesteps(estimators: dict[Any, Any]) -> list[int]:
+def get_partiallycompletetimesteps(estimators: dict[tuple[int, int], dict]) -> list[int]:
     """During a simulation, some estimator files can contain information for some cells but not others
     for the current timestep.
     """
     timestepcells: dict[int, list[int]] = {}
     all_mgis = set()
     for nts, mgi in estimators:
         if nts not in timestepcells:
             timestepcells[nts] = []
         timestepcells[nts].append(mgi)
         all_mgis.add(mgi)
 
-    nts_incomplete = []
-    for nts, mgilist in timestepcells.items():
-        if len(mgilist) < len(all_mgis):
-            nts_incomplete.append(nts)
-
-    return nts_incomplete
+    return [nts for nts, mgilist in timestepcells.items() if len(mgilist) < len(all_mgis)]
```

### Comparing `artistools-2023.5.16.3/artistools/estimators/estimators_classic.py` & `artistools-2023.8.1/artistools/estimators/estimators_classic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-import glob
+from __future__ import annotations
+
 import gzip
-import os
+import typing as t
 from pathlib import Path
 
 import artistools as at
 
+if t.TYPE_CHECKING:
+    import pandas as pd
+
 
-def get_atomic_composition(modelpath):
+def get_atomic_composition(modelpath: Path) -> dict[int, int]:
     """Read ion list from output file."""
     atomic_composition = {}
 
-    with open(modelpath / "output_0-0.txt") as foutput:
+    with (modelpath / "output_0-0.txt").open() as foutput:
         ioncount = 0
         for row in foutput:
             if row.split()[0] == "[input.c]":
                 split_row = row.split()
                 if split_row[1] == "element":
                     Z = int(split_row[4])
                     ioncount = 0
                 elif split_row[1] == "ion":
                     ioncount += 1
                     atomic_composition[Z] = ioncount
     return atomic_composition
 
 
-def parse_ion_row_classic(row, outdict, atomic_composition):
+def parse_ion_row_classic(row: list[str], outdict: dict[str, t.Any], atomic_composition: dict[int, int]) -> None:
     outdict["populations"] = {}
 
     elements = atomic_composition.keys()
 
     i = 6  # skip first 6 numbers in est file. These are n, TR, Te, W, TJ, grey_depth.
     # Numbers after these 6 are populations
     for atomic_number in elements:
@@ -40,76 +44,70 @@
             elpop = outdict["populations"].get(atomic_number, 0)
             outdict["populations"][atomic_number] = elpop + value_thision
 
             totalpop = outdict["populations"].get("total", 0)
             outdict["populations"]["total"] = totalpop + value_thision
 
 
-def get_estimator_files(modelpath):
-    estimfiles = (
-        glob.glob(os.path.join(modelpath, "estimators_????.out"), recursive=True)
-        + glob.glob(os.path.join(modelpath, "estimators_????.out.gz"), recursive=True)
-        + glob.glob(os.path.join(modelpath, "*/estimators_????.out"), recursive=True)
-        + glob.glob(os.path.join(modelpath, "*/estimators_????.out.gz"), recursive=True)
-    )
-
-    return estimfiles
-
-
-def get_first_ts_in_run_directory(modelpath):
+def get_first_ts_in_run_directory(modelpath) -> dict[str, int]:
     folderlist_all = (*sorted([child for child in Path(modelpath).iterdir() if child.is_dir()]), Path(modelpath))
 
     first_timesteps_in_dir = {}
 
     for folder in folderlist_all:
-        if os.path.isfile(folder / "output_0-0.txt"):
-            with open(folder / "output_0-0.txt") as output_0:
+        if (folder / "output_0-0.txt").is_file():
+            with (folder / "output_0-0.txt").open() as output_0:
                 timesteps_in_dir = [
                     line.strip("...\n").split(" ")[-1]
                     for line in output_0
                     if "[debug] update_packets: updating packet 0 for timestep" in line
                 ]
             first_ts = timesteps_in_dir[0]
             first_timesteps_in_dir[str(folder)] = int(first_ts)
 
     return first_timesteps_in_dir
 
 
-def read_classic_estimators(modelpath, modeldata, readonly_mgi=False, readonly_timestep=False):
-    estimfiles = get_estimator_files(modelpath)
+def read_classic_estimators(
+    modelpath: Path,
+    modeldata: pd.DataFrame,
+    readonly_mgi: list[int] | None = None,
+    readonly_timestep: list[int] | None = None,
+) -> dict[tuple[int, int], t.Any] | None:
+    estimfiles = list(Path(modelpath).glob("**/estimators_????.out"))
     if not estimfiles:
         print("No estimator files found")
-        return False
+        return None
     print(f"Reading {len(estimfiles)} estimator files...")
 
     first_timesteps_in_dir = get_first_ts_in_run_directory(modelpath)
     atomic_composition = get_atomic_composition(modelpath)
 
     inputparams = at.get_inputparams(modelpath)
     ndimensions = inputparams["n_dimensions"]
 
-    estimators = {}
-    for estfile in estimfiles:
-        opener = gzip.open if estfile.endswith(".gz") else open
+    estimators: dict[tuple[int, int], t.Any] = {}
+    for estfilepath in estimfiles:
+        opener: t.Any = gzip.open if str(estfilepath).endswith(".gz") else open
 
         # If classic plots break it's probably getting first timestep here
         # Try either of the next two lines
-        timestep = first_timesteps_in_dir[str(estfile).split("/")[0]]  # get the starting timestep for the estfile
+        timestep = first_timesteps_in_dir[str(estfilepath).split("/")[0]]  # get the starting timestep for the estfile
         # timestep = first_timesteps_in_dir[str(estfile[:-20])]
         # timestep = 0  # if the first timestep in the file is 0 then this is fine
-        with opener(estfile) as estfile:
+        with opener(estfilepath) as estfile:
             modelgridindex = -1
             for line in estfile:
                 row = line.split()
                 if int(row[0]) <= int(modelgridindex):
                     timestep += 1
                 modelgridindex = int(row[0])
 
-                if (readonly_mgi is False or modelgridindex in readonly_mgi) and (
-                    readonly_timestep is False or timestep in readonly_timestep
+                if (not readonly_mgi or modelgridindex in readonly_mgi) and (
+                    not readonly_timestep or timestep in readonly_timestep
                 ):
                     estimators[(timestep, modelgridindex)] = {}
 
                     if ndimensions == 1:
                         estimators[(timestep, modelgridindex)]["velocity_outer"] = modeldata["velocity_outer"][
                             modelgridindex
                         ]
```

### Comparing `artistools-2023.5.16.3/artistools/estimators/exportmassfractions.py` & `artistools-2023.8.1/artistools/estimators/exportmassfractions.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,37 +17,34 @@
             formatter_class=at.CustomArgHelpFormatter, description="Create solar r-process pattern in ARTIS format."
         )
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
-    modelpath: Path = Path(".")
+    modelpath: Path = Path()
     timestep = 14
     elmass = {el.Z: el.mass for _, el in at.get_composition_data(modelpath).iterrows()}
     outfilename = args.outputpath
-    with open(outfilename, "w") as fout:
+    with Path(outfilename).open("w") as fout:
         modelgridindexlist = range(10)
         estimators = at.estimators.read_estimators(modelpath, timestep=timestep, modelgridindex=modelgridindexlist)
         for modelgridindex in modelgridindexlist:
             tdays = estimators[(timestep, modelgridindex)]["tdays"]
             popdict = estimators[(timestep, modelgridindex)]["populations"]
 
             numberdens = {}
             totaldens = 0.0  # number density times atomic mass summed over all elements
             for key in popdict:
                 try:
                     atomic_number = int(key)
                     numberdens[atomic_number] = popdict[atomic_number]
                     totaldens += numberdens[atomic_number] * elmass[atomic_number]
-                except ValueError:
+                except (ValueError, TypeError):
                     pass
-                except TypeError:
-                    pass
-
             massfracs = {
                 atomic_number: numberdens[atomic_number] * elmass[atomic_number] / totaldens
                 for atomic_number in numberdens
             }
 
             fout.write(f"{tdays}d shell {modelgridindex}\n")
             massfracsum = 0.0
```

### Comparing `artistools-2023.5.16.3/artistools/estimators/plot3destimators_classic.py` & `artistools-2023.8.1/artistools/estimators/plot3destimators_classic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,54 @@
+from __future__ import annotations
+
+import typing as t
 from collections import namedtuple
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pyvista as pv
 
 import artistools as at
 
 CLIGHT = 2.99792458e10
 
 
-def read_selected_mgi(modelpath, readonly_mgi, readonly_timestep=False):
+def read_selected_mgi(
+    modelpath: Path, readonly_mgi: None | list[int] = None, readonly_timestep: None | list[int] = None
+) -> dict[tuple[int, int], t.Any] | None:
     modeldata, _ = at.inputmodel.get_modeldata(modelpath)
-    estimators = at.estimators.estimators_classic.read_classic_estimators(
+    return at.estimators.estimators_classic.read_classic_estimators(
         modelpath, modeldata, readonly_mgi=readonly_mgi, readonly_timestep=readonly_timestep
     )
-    return estimators
 
 
 def get_modelgridcells_along_axis(modelpath):
-    ArgsTuple = namedtuple("args", "modelpath sliceaxis other_axis1 other_axis2 positive_axis")
+    ArgsTuple = namedtuple("ArgsTuple", "modelpath sliceaxis other_axis1 other_axis2 positive_axis")
     args = ArgsTuple(modelpath=modelpath, sliceaxis="x", other_axis1="z", other_axis2="y", positive_axis=True)
 
     profile1d = at.inputmodel.slice1Dfromconein3dmodel.get_profile_along_axis(args=args)
-    readonly_mgi = get_mgi_of_modeldata(profile1d, modelpath)
-
-    return readonly_mgi
+    return get_mgi_of_modeldata(profile1d, modelpath)
 
 
-def get_modelgridcells_2D_slice(modeldata, modelpath):
-    sliceaxis = "z"
+def get_modelgridcells_2D_slice(modeldata, modelpath) -> list[int]:
+    sliceaxis: t.Literal["x", "y", "z"] = "z"
 
     slicedata = at.initial_composition.get_2D_slice_through_3d_model(modeldata, sliceaxis)
-    readonly_mgi = get_mgi_of_modeldata(slicedata, modelpath)
-
-    return readonly_mgi
+    return get_mgi_of_modeldata(slicedata, modelpath)
 
 
-def get_mgi_of_modeldata(modeldata, modelpath):
+def get_mgi_of_modeldata(modeldata, modelpath) -> list[int]:
     assoc_cells, mgi_of_propcells = at.get_grid_mapping(modelpath=modelpath)
-    readonly_mgi = []
-    for _index, row in modeldata.iterrows():
-        if row["rho"] > 0:
-            mgi = mgi_of_propcells[int(row["inputcellid"]) - 1]
-            readonly_mgi.append(mgi)
-    return readonly_mgi
+    return [mgi_of_propcells[int(row["inputcellid"]) - 1] for _index, row in modeldata.iterrows() if row["rho"] > 0]
 
 
 def plot_Te_vs_time_lineofsight_3d_model(modelpath, modeldata, estimators, readonly_mgi):
     assoc_cells, mgi_of_propcells = at.get_grid_mapping(modelpath=modelpath)
-    times = at.get_timestep_times_float(modelpath)
+    times = at.get_timestep_times(modelpath)
 
     for mgi in readonly_mgi:
         associated_modeldata_row_for_mgi = modeldata.loc[modeldata["inputcellid"] == assoc_cells[mgi][0]]
 
         Te = [estimators[(timestep, mgi)]["Te"] for timestep, _ in enumerate(times)]
         plt.scatter(times, Te, label=f'vel={associated_modeldata_row_for_mgi["vel_y_mid"].to_numpy()[0] / CLIGHT}')
 
@@ -63,15 +58,15 @@
     plt.xscale("log")
     plt.legend()
     plt.show()
 
 
 def plot_Te_vs_velocity(modelpath, modeldata, estimators, readonly_mgi):
     assoc_cells, mgi_of_propcells = at.get_grid_mapping(modelpath=modelpath)
-    times = at.get_timestep_times_float(modelpath)
+    times = at.get_timestep_times(modelpath)
     timesteps = [50, 55, 60, 65, 70, 75, 80, 90]
 
     for timestep in timesteps:
         Te = [estimators[(timestep, mgi)]["Te"] for mgi in readonly_mgi]
 
         associated_modeldata_rows = [
             modeldata.loc[modeldata["inputcellid"] == assoc_cells[mgi][0]] for mgi in readonly_mgi
@@ -85,16 +80,16 @@
     plt.yscale("log")
     plt.legend()
     plt.show()
 
 
 def get_Te_vs_velocity_2D(modelpath, modeldata, vmax, estimators, readonly_mgi, timestep):
     assoc_cells, mgi_of_propcells = at.get_grid_mapping(modelpath=modelpath)
-    times = at.get_timestep_times_float(modelpath)
-    print([(ts, time) for ts, time in enumerate(times)])
+    times = at.get_timestep_times(modelpath)
+    print(list(enumerate(times)))
     time = times[timestep]
     print(f"time {time} days")
 
     ngridcells = len(modeldata["inputcellid"])
     Te = np.zeros(ngridcells)
 
     for mgi in readonly_mgi:
@@ -102,17 +97,17 @@
 
     grid = round(len(modeldata["inputcellid"]) ** (1.0 / 3.0))
     grid_Te = np.zeros((grid, grid, grid))  # needs 3D array
     xgrid = np.zeros(grid)
 
     vmax = vmax / CLIGHT
     i = 0
-    for z in range(0, grid):
-        for y in range(0, grid):
-            for x in range(0, grid):
+    for z in range(grid):
+        for y in range(grid):
+            for x in range(grid):
                 grid_Te[x, y, z] = Te[i]
                 if modeldata["rho"][i] == 0.0:
                     grid_Te[x, y, z] = None
                 xgrid[x] = -vmax + 2 * x * vmax / grid
                 i += 1
 
     return grid_Te, xgrid
@@ -151,24 +146,24 @@
     )
 
     p.camera_position = "xy"
     p.add_title(f"{time:.1f} days")
     p.show(screenshot=modelpath / f"3Dplot_Te{time:.1f}days_disk.png")
 
 
-def main():
-    modelpath = Path(".")
+def main() -> None:
+    modelpath = Path()
     modeldata, _, vmax = at.inputmodel.get_modeldata_tuple(modelpath)
 
     # # Get mgi of grid cells along axis for 1D plot
     # # readonly_mgi = get_modelgridcells_along_axis(modelpath)
     readonly_mgi = get_modelgridcells_2D_slice(modeldata, modelpath)
     #
     timestep = 82
-    times = at.get_timestep_times_float(modelpath)
+    times = at.get_timestep_times(modelpath)
     time = times[timestep]
     estimators = read_selected_mgi(modelpath, readonly_mgi=readonly_mgi, readonly_timestep=[timestep])
     grid_Te, xgrid = get_Te_vs_velocity_2D(modelpath, modeldata, vmax, estimators, readonly_mgi, timestep)
     grid = round(len(modeldata["inputcellid"]) ** (1.0 / 3.0))
     make_2d_plot(grid, grid_Te, vmax, modelpath, xgrid, time)
```

### Comparing `artistools-2023.5.16.3/artistools/estimators/plotestimators.py` & `artistools-2023.8.1/artistools/estimators/plotestimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
 """Functions for plotting artis estimators and internal structure.
 
 Examples are temperatures, populations, heating/cooling rates.
 """
+
 import argparse
+import contextlib
 import math
 import sys
 from pathlib import Path
 
 import argcomplete
 import matplotlib.pyplot as plt
 import numpy as np
@@ -123,15 +125,15 @@
     if seriestype == "averageionisation":
         ax.set_ylabel("Average ion charge")
     elif seriestype == "averageexcitation":
         ax.set_ylabel("Average excitation [eV]")
     else:
         raise ValueError
 
-    arr_tdelta = at.get_timestep_times_float(modelpath, loc="delta")
+    arr_tdelta = at.get_timestep_times(modelpath, loc="delta")
     for paramvalue in params:
         if seriestype == "averageionisation":
             atomic_number = at.get_atomic_number(paramvalue)
         else:
             atomic_number = at.get_atomic_number(paramvalue.split(" ")[0])
             ion_stage = at.decode_roman_numeral(paramvalue.split(" ")[1])
         ylist = []
@@ -193,15 +195,15 @@
         raise ValueError
 
     modeldata, _ = at.inputmodel.get_modeldata(modelpath)
     modeldata = modeldata.eval("modelcellvolume = cellmass_grams / (10 ** logrho)")
 
     adata = at.atomic.get_levels(modelpath)
 
-    arr_tdelta = at.get_timestep_times_float(modelpath, loc="delta")
+    arr_tdelta = at.get_timestep_times(modelpath, loc="delta")
     for paramvalue in params:
         paramsplit = paramvalue.split(" ")
         atomic_number = at.get_atomic_number(paramsplit[0])
         ion_stage = at.decode_roman_numeral(paramsplit[1])
         levelindex = int(paramsplit[2])
 
         ionlevels = adata.query("Z == @atomic_number and ion_stage == @ion_stage").iloc[0].levels
@@ -531,15 +533,15 @@
     if dfalldata is not None:
         dfalldata[variablename] = ylist
 
     ylist.insert(0, ylist[0])
 
     xlist, ylist = at.estimators.apply_filters(xlist, ylist, args)
 
-    ax.plot(xlist, ylist, linewidth=1.5, label=linelabel, color=dictcolors.get(variablename, None), **plotkwargs)
+    ax.plot(xlist, ylist, linewidth=1.5, label=linelabel, color=dictcolors.get(variablename), **plotkwargs)
 
 
 def get_xlist(
     xvariable, allnonemptymgilist, estimators, timestepslist, modelpath, args
 ) -> tuple[list[float], list[float], list[float]]:
     if xvariable in ["cellid", "modelgridindex"]:
         mgilist_out = [mgi for mgi in allnonemptymgilist if mgi <= args.xmax] if args.xmax >= 0 else allnonemptymgilist
@@ -547,15 +549,15 @@
         timestepslist_out = timestepslist
     elif xvariable == "timestep":
         mgilist_out = allnonemptymgilist
         xlist = timestepslist
         timestepslist_out = timestepslist
     elif xvariable == "time":
         mgilist_out = allnonemptymgilist
-        timearray = at.get_timestep_times_float(modelpath)
+        timearray = at.get_timestep_times(modelpath)
         xlist = [np.mean([timearray[ts] for ts in tslist]) for tslist in timestepslist]
         timestepslist_out = timestepslist
     else:
         xlist = []
         mgilist_out = []
         timestepslist_out = []
         for modelgridindex, timesteps in zip(allnonemptymgilist, timestepslist):
@@ -744,15 +746,15 @@
         outfilename = str(args.outputfile).format(modelgridindex=mgilist[0])
 
     else:
         timeavg = (args.timemin + args.timemax) / 2.0
         if args.multiplot and not args.classicartis:
             tdays = estimators[(timestepslist[0][0], mgilist[0])]["tdays"]
             figure_title = f"{modelname}\nTimestep {timestepslist[0]} ({tdays:.2f}d)"
-        elif args.multiplot and args.classicartis:
+        elif args.multiplot:
             timedays = float(at.get_timestep_time(modelpath, timestepslist[0]))
             figure_title = f"{modelname}\nTimestep {timestepslist[0]} ({timedays:.2f}d)"
         else:
             figure_title = f"{modelname}\nTimestep {timestepslist[0]} ({timeavg:.2f}d)"
 
         defaultoutputfile = Path("plotestimators_ts{timestep:02d}_{timeavg:.0f}d.pdf")
         if Path(args.outputfile).is_dir():
@@ -798,15 +800,15 @@
         ionstr = (
             f"{at.get_elsymbol(atomic_number)} {at.roman_numerals[ion_stage]} to {at.roman_numerals[ion_stage - 1]}"
         )
 
         listT_e = []
         list_rrc = []
         list_rrc2 = []
-        for _, dicttimestepmodelgrid in estimators.items():
+        for dicttimestepmodelgrid in estimators.values():
             if (
                 not dicttimestepmodelgrid["emptycell"]
                 and (atomic_number, ion_stage) in dicttimestepmodelgrid["RRC_LTE_Nahar"]
             ):
                 listT_e.append(dicttimestepmodelgrid["Te"])
                 list_rrc.append(dicttimestepmodelgrid["RRC_LTE_Nahar"][(atomic_number, ion_stage)])
                 list_rrc2.append(dicttimestepmodelgrid["Alpha_R"][(atomic_number, ion_stage)])
@@ -816,31 +818,28 @@
 
         # sort the pairs by temperature ascending
         listT_e, list_rrc, list_rrc2 = zip(*sorted(zip(listT_e, list_rrc, list_rrc2), key=lambda x: x[0]))
 
         ax.plot(listT_e, list_rrc, linewidth=2, label=f"{ionstr} ARTIS RRC_LTE_Nahar", **plotkwargs)
         ax.plot(listT_e, list_rrc2, linewidth=2, label=f"{ionstr} ARTIS Alpha_R", **plotkwargs)
 
-        try:
+        with contextlib.suppress(KeyError):
             dfrates = recombcalibrationdata[(atomic_number, ion_stage)].query(
                 "T_e > @T_e_min & T_e < @T_e_max", local_dict={"T_e_min": min(listT_e), "T_e_max": max(listT_e)}
             )
 
             ax.plot(
                 dfrates.T_e,
                 dfrates.rrc_total,
                 linewidth=2,
                 label=ionstr + " (calibration)",
                 markersize=6,
                 marker="s",
                 **plotkwargs,
             )
-        except KeyError:
-            pass
-
         # rrcfiles = glob.glob(
         #     f'/Users/lshingles/Library/Mobile Documents/com~apple~CloudDocs/GitHub/'
         #     f'artis-atomic/atomic-data-nahar/{at.get_elsymbol(atomic_number).lower()}{ion_stage - 1}.rrc*.txt')
         # if rrcfiles:
         #     dfrecombrates = get_ionrecombrates_fromfile(rrcfiles[0])
         #
         #     dfrecombrates.query("logT > @logT_e_min & logT < @logT_e_max",
@@ -939,29 +938,29 @@
     )
 
     parser.add_argument(
         "--classicartis", action="store_true", help="Flag to show using output from classic ARTIS branch"
     )
 
 
-def main(args=None, argsraw=None, **kwargs):
+def main(args=None, argsraw=None, **kwargs) -> None:
     """Plot ARTIS estimators."""
     if args is None:
         parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
 
     modelpath = Path(args.modelpath)
 
     modelname = at.get_model_name(modelpath)
 
     if not args.timedays and not args.timestep and args.modelgridindex > -1:
-        args.timestep = f"0-{len(at.get_timestep_times_float(modelpath)) - 1}"
+        args.timestep = f"0-{len(at.get_timestep_times(modelpath)) - 1}"
 
     (timestepmin, timestepmax, args.timemin, args.timemax) = at.get_time_range(
         modelpath, args.timestep, args.timemin, args.timemax, args.timedays
     )
 
     print(
         f"Plotting estimators for '{modelname}' timesteps {timestepmin} to {timestepmax} "
@@ -975,118 +974,116 @@
 
         modeldata, _ = at.inputmodel.get_modeldata(modelpath)
         estimators = artistools.estimators.estimators_classic.read_classic_estimators(modelpath, modeldata)
     else:
         estimators = at.estimators.read_estimators(
             modelpath=modelpath, modelgridindex=args.modelgridindex, timestep=tuple(timesteps_included)
         )
+    assert estimators is not None
 
     for ts in reversed(timesteps_included):
         tswithdata = [ts for (ts, mgi) in estimators]
         for ts in timesteps_included:
             if ts not in tswithdata:
                 timesteps_included.remove(ts)
                 print(f"ts {ts} requested but no data found. Removing.")
 
     if not timesteps_included:
         print("No timesteps with data are included")
         return
 
-    plotlist = (
-        args.plotlist
-        if args.plotlist
-        else [
-            # [['initabundances', ['Fe', 'Ni_stable', 'Ni_56']]],
-            # ['heating_dep', 'heating_coll', 'heating_bf', 'heating_ff',
-            #  ['_yscale', 'linear']],
-            # ['cooling_adiabatic', 'cooling_coll', 'cooling_fb', 'cooling_ff',
-            #  ['_yscale', 'linear']],
-            # [['initmasses', ['Ni_56', 'He', 'C', 'Mg']]],
-            # ['heating_gamma/gamma_dep'],
-            # ['nne'],
-            ["TR", "Te", "TJ", ["_yscale", "linear"]],
-            # ['Te'],
-            # [['averageionisation', ['Fe', 'Ni']]],
-            # [['averageexcitation', ['Fe II', 'Fe III']]],
-            # [['populations', ['Sr89', 'Sr90', 'Sr91', 'Sr92', 'Sr93', 'Sr94', 'Sr95']],
-            #  ['_ymin', 1e-3], ['_ymax', 5]],
-            [["populations", ["Fe", "Co", "Ni", "Sr", "Nd", "U"]]],
-            # [['populations', ['He I', 'He II', 'He III']]],
-            # [['populations', ['C I', 'C II', 'C III', 'C IV', 'C V']]],
-            # [['populations', ['O I', 'O II', 'O III', 'O IV']]],
-            # [['populations', ['Ne I', 'Ne II', 'Ne III', 'Ne IV', 'Ne V']]],
-            # [['populations', ['Si I', 'Si II', 'Si III', 'Si IV', 'Si V']]],
-            # [['populations', ['Cr I', 'Cr II', 'Cr III', 'Cr IV', 'Cr V']]],
-            # [['populations', ['Fe I', 'Fe II', 'Fe III', 'Fe IV', 'Fe V', 'Fe VI', 'Fe VII', 'Fe VIII']]],
-            # [['populations', ['Co I', 'Co II', 'Co III', 'Co IV', 'Co V', 'Co VI', 'Co VII']]],
-            # [['populations', ['Ni I', 'Ni II', 'Ni III', 'Ni IV', 'Ni V', 'Ni VI', 'Ni VII']]],
-            # [['populations', ['Fe II', 'Fe III', 'Co II', 'Co III', 'Ni II', 'Ni III']]],
-            # [['populations', ['Fe I', 'Fe II', 'Fe III', 'Fe IV', 'Fe V', 'Ni II']]],
-            # [['RRC_LTE_Nahar', ['Fe II', 'Fe III', 'Fe IV', 'Fe V']]],
-            # [['RRC_LTE_Nahar', ['Co II', 'Co III', 'Co IV', 'Co V']]],
-            # [['RRC_LTE_Nahar', ['Ni I', 'Ni II', 'Ni III', 'Ni IV', 'Ni V', 'Ni VI', 'Ni VII']]],
-            # [['Alpha_R / RRC_LTE_Nahar', ['Fe II', 'Fe III', 'Fe IV', 'Fe V', 'Ni III']]],
-            # [['gamma_NT', ['Fe I', 'Fe II', 'Fe III', 'Fe IV', 'Fe V', 'Ni II']]],
-        ]
-    )
+    plotlist = args.plotlist or [
+        # [['initabundances', ['Fe', 'Ni_stable', 'Ni_56']]],
+        # ['heating_dep', 'heating_coll', 'heating_bf', 'heating_ff',
+        #  ['_yscale', 'linear']],
+        # ['cooling_adiabatic', 'cooling_coll', 'cooling_fb', 'cooling_ff',
+        #  ['_yscale', 'linear']],
+        # [['initmasses', ['Ni_56', 'He', 'C', 'Mg']]],
+        # ['heating_gamma/gamma_dep'],
+        # ['nne'],
+        ["TR", "Te", "TJ", ["_yscale", "linear"]],
+        # ['Te'],
+        # [['averageionisation', ['Fe', 'Ni']]],
+        # [['averageexcitation', ['Fe II', 'Fe III']]],
+        # [['populations', ['Sr89', 'Sr90', 'Sr91', 'Sr92', 'Sr93', 'Sr94', 'Sr95']],
+        #  ['_ymin', 1e-3], ['_ymax', 5]],
+        [["populations", ["Fe", "Co", "Ni", "Sr", "Nd", "U"]]],
+        # [['populations', ['He I', 'He II', 'He III']]],
+        # [['populations', ['C I', 'C II', 'C III', 'C IV', 'C V']]],
+        # [['populations', ['O I', 'O II', 'O III', 'O IV']]],
+        # [['populations', ['Ne I', 'Ne II', 'Ne III', 'Ne IV', 'Ne V']]],
+        # [['populations', ['Si I', 'Si II', 'Si III', 'Si IV', 'Si V']]],
+        # [['populations', ['Cr I', 'Cr II', 'Cr III', 'Cr IV', 'Cr V']]],
+        # [['populations', ['Fe I', 'Fe II', 'Fe III', 'Fe IV', 'Fe V', 'Fe VI', 'Fe VII', 'Fe VIII']]],
+        # [['populations', ['Co I', 'Co II', 'Co III', 'Co IV', 'Co V', 'Co VI', 'Co VII']]],
+        # [['populations', ['Ni I', 'Ni II', 'Ni III', 'Ni IV', 'Ni V', 'Ni VI', 'Ni VII']]],
+        # [['populations', ['Fe II', 'Fe III', 'Co II', 'Co III', 'Ni II', 'Ni III']]],
+        # [['populations', ['Fe I', 'Fe II', 'Fe III', 'Fe IV', 'Fe V', 'Ni II']]],
+        # [['RRC_LTE_Nahar', ['Fe II', 'Fe III', 'Fe IV', 'Fe V']]],
+        # [['RRC_LTE_Nahar', ['Co II', 'Co III', 'Co IV', 'Co V']]],
+        # [['RRC_LTE_Nahar', ['Ni I', 'Ni II', 'Ni III', 'Ni IV', 'Ni V', 'Ni VI', 'Ni VII']]],
+        # [['Alpha_R / RRC_LTE_Nahar', ['Fe II', 'Fe III', 'Fe IV', 'Fe V', 'Ni III']]],
+        # [['gamma_NT', ['Fe I', 'Fe II', 'Fe III', 'Fe IV', 'Fe V', 'Ni II']]],
+    ]
 
     if args.recombrates:
         plot_recombrates(modelpath, estimators, 26, [2, 3, 4, 5])
         plot_recombrates(modelpath, estimators, 27, [3, 4])
         plot_recombrates(modelpath, estimators, 28, [3, 4, 5])
-    else:
-        modeldata, _ = at.inputmodel.get_modeldata(modelpath)
 
-        if args.modelgridindex > -1 or args.x in ["time", "timestep"]:
-            # plot time evolution in specific cell
-            if not args.x:
-                args.x = "time"
-            mgilist = [args.modelgridindex] * len(timesteps_included)
-            timesteplist_unfiltered = [(ts,) for ts in timesteps_included]
-            if estimators[(args.modelgridindex, timesteps_included[0])]["emptycell"]:
-                msg = f"cell {args.modelgridindex} is empty. no estimators available"
-                raise ValueError(msg)
-            make_plot(modelpath, timesteplist_unfiltered, mgilist, estimators, args.x, plotlist, args)
-        else:
-            # plot a range of cells in a time snapshot showing internal structure
+        return
+    modeldata, _ = at.inputmodel.get_modeldata(modelpath)
 
-            if not args.x:
-                args.x = "velocity_outer"
+    if args.modelgridindex > -1 or args.x in ["time", "timestep"]:
+        # plot time evolution in specific cell
+        if not args.x:
+            args.x = "time"
+        mgilist = [args.modelgridindex] * len(timesteps_included)
+        timesteplist_unfiltered = [[ts] for ts in timesteps_included]
+        if estimators[(args.modelgridindex, timesteps_included[0])]["emptycell"]:
+            msg = f"cell {args.modelgridindex} is empty. no estimators available"
+            raise ValueError(msg)
+        make_plot(modelpath, timesteplist_unfiltered, mgilist, estimators, args.x, plotlist, args)
+    else:
+        # plot a range of cells in a time snapshot showing internal structure
 
-            if args.classicartis:
-                allnonemptymgilist = [
-                    modelgridindex
-                    for modelgridindex in modeldata.index
-                    if (timesteps_included[0], modelgridindex) in estimators
-                ]
-            else:
-                allnonemptymgilist = [
-                    modelgridindex
-                    for modelgridindex in modeldata.index
-                    if not estimators[(timesteps_included[0], modelgridindex)]["emptycell"]
-                ]
-
-            if args.multiplot:
-                pdf_list = []
-                modelpath_list = []
-                for timestep in range(timestepmin, timestepmax + 1):
-                    timesteplist_unfiltered = [[timestep]] * len(allnonemptymgilist)
-                    outfilename = make_plot(
-                        modelpath, timesteplist_unfiltered, allnonemptymgilist, estimators, args.x, plotlist, args
-                    )
+        if not args.x:
+            args.x = "velocity_outer"
+
+        if args.classicartis:
+            allnonemptymgilist = [
+                modelgridindex
+                for modelgridindex in modeldata.index
+                if (timesteps_included[0], modelgridindex) in estimators
+            ]
+        else:
+            allnonemptymgilist = [
+                modelgridindex
+                for modelgridindex in modeldata.index
+                if not estimators[(timesteps_included[0], modelgridindex)]["emptycell"]
+            ]
+
+        if args.multiplot:
+            pdf_list = []
+            modelpath_list = []
+            for timestep in range(timestepmin, timestepmax + 1):
+                timesteplist_unfiltered = [[timestep]] * len(allnonemptymgilist)
+                outfilename = make_plot(
+                    modelpath, timesteplist_unfiltered, allnonemptymgilist, estimators, args.x, plotlist, args
+                )
 
-                    if "/" in outfilename:
-                        outfilename = outfilename.split("/")[1]
+                if "/" in outfilename:
+                    outfilename = outfilename.split("/")[1]
 
-                    pdf_list.append(outfilename)
-                    modelpath_list.append(modelpath)
+                pdf_list.append(outfilename)
+                modelpath_list.append(modelpath)
 
-                if len(pdf_list) > 1:
-                    at.join_pdf_files(pdf_list, modelpath_list)
+            if len(pdf_list) > 1:
+                at.join_pdf_files(pdf_list, modelpath_list)
 
-            else:
-                timesteplist_unfiltered = [timesteps_included] * len(allnonemptymgilist)
-                make_plot(modelpath, timesteplist_unfiltered, allnonemptymgilist, estimators, args.x, plotlist, args)
+        else:
+            timesteplist_unfiltered = [timesteps_included] * len(allnonemptymgilist)
+            make_plot(modelpath, timesteplist_unfiltered, allnonemptymgilist, estimators, args.x, plotlist, args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `artistools-2023.5.16.3/artistools/gsinetwork.py` & `artistools-2023.8.1/artistools/gsinetwork.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
+from __future__ import annotations
+
 import argparse
 import math
 import multiprocessing
-from collections.abc import Collection
-from collections.abc import Sequence
+import typing as t
 from functools import partial
 from pathlib import Path
-from typing import Any
-from typing import Union
 
 import argcomplete
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 import artistools as at
 
 
+def strnuc_to_latex(strnuc: str):
+    """Convert a string like sr89 to $^{89}$Sr."""
+    elsym = strnuc.rstrip("0123456789")
+    massnum = strnuc.removeprefix(elsym)
+
+    return rf"$^{{{massnum}}}${elsym.title()}"
+
+
 def plot_qdot(
     modelpath: Path,
     dfpartcontrib: pd.DataFrame,
     dfmodel: pd.DataFrame,
     allparticledata: dict[int, dict[str, np.ndarray]],
-    arr_time_artis_days: Collection[float],
-    arr_artis_ye: Collection[float],
-    arr_time_gsi_days: Collection[float],
-    pdfoutpath: Union[Path, str],
+    arr_time_artis_days: t.Sequence[float],
+    arr_artis_ye: t.Sequence[float],
+    arr_time_gsi_days: t.Sequence[float],
+    pdfoutpath: Path | str,
+    xmax: None | float = None,
 ) -> None:
     try:
         depdata = at.get_deposition(modelpath=modelpath)
 
     except FileNotFoundError:
         print("Can't do qdot plot because no deposition.out file")
         return
@@ -43,16 +51,16 @@
     heatcols = ["hbeta", "halpha", "hbfis", "hspof", "Ye", "Qdot"]
 
     arr_heat = {col: np.zeros_like(arr_time_gsi_days) for col in heatcols}
 
     model_mass_grams = dfmodel.cellmass_grams.sum()
     print(f"model mass: {model_mass_grams / 1.989e33:.3f} Msun")
 
-    # calculate global heating rates from the individual particle heating rates
-    dfpartcontrib_nomissing = dfpartcontrib.query("particleid in @allparticledata.keys()")
+    print("Calculating global heating rates from the individual particle heating rates...")
+    dfpartcontrib_nomissing = dfpartcontrib[dfpartcontrib["particleid"].isin(allparticledata.keys())]
     for cellindex, dfpartcontribthiscell in dfpartcontrib_nomissing.groupby("cellindex"):
         if cellindex >= len(dfmodel):
             continue
 
         cell_mass_frac = dfmodel.iloc[cellindex - 1].cellmass_grams / model_mass_grams
 
         if cell_mass_frac == 0.0:
@@ -63,14 +71,16 @@
         contribtuples = dfpartcontribthiscell[["particleid", "frac_of_cellmass"]].itertuples(index=False)
 
         for particleid, frac_of_cellmass in contribtuples:
             thisparticledata = allparticledata[particleid]
             for col in heatcols:
                 arr_heat[col] += thisparticledata[col] * cell_mass_frac * frac_of_cellmass / frac_of_cellmass_sum
 
+    print("  done.")
+
     show_ye = False
     nrows = 2 if show_ye else 1
     fig, axes = plt.subplots(
         nrows=nrows,
         ncols=1,
         sharex=True,
         sharey=False,
@@ -81,15 +91,15 @@
         axes = [axes]
 
     axis = axes[0]
 
     # axis.set_ylim(bottom=1e7, top=2e10)
     # axis.set_xlim(left=tstart, right=tend)
     xmin = min(arr_time_gsi_days) * 0.9
-    xmax = max(arr_time_gsi_days) * 1.03
+    xmax = xmax or max(arr_time_gsi_days) * 1.03
     axis.set_xlim(left=xmin, right=xmax)
 
     # axis.set_xscale('log')
 
     # axis.set_xlim(left=1., right=arr_time_artis[-1])
     axes[-1].set_xlabel("Time [days]")
     axis.set_yscale("log")
@@ -154,25 +164,25 @@
     axis.plot(
         arr_time_gsi_days,
         arr_heat["hbfis"],
         linewidth=2,
         linestyle="dotted",
         # marker='x', markersize=8,
         # color='black',
-        label=r"$\dot{Q}_{hbfis}$ GSI Network",
+        label=r"$\dot{Q}_{\beta fis}$ GSI Network",
     )
 
     axis.plot(
         arr_time_gsi_days,
         arr_heat["hspof"],
         linewidth=2,
         linestyle="dotted",
         # marker='x', markersize=8,
         # color='black',
-        label=r"$\dot{Q}_{spof}$ GSI Network",
+        label=r"$\dot{Q}_{sponfis}$ GSI Network",
     )
 
     axis.legend(loc="best", frameon=False, handlelength=1, ncol=3, numpoints=1)
 
     if show_ye:
         axes[1].plot(
             arr_time_gsi_days,
@@ -203,39 +213,44 @@
     print(f"Saved {pdfoutpath}")
 
 
 def plot_cell_abund_evolution(
     modelpath: Path,
     dfpartcontrib: pd.DataFrame,
     allparticledata,
-    arr_time_artis_days: Sequence[float],
-    arr_time_gsi_days: Sequence[float],
-    arr_strnuc: Sequence[str],
+    arr_time_artis_days: t.Sequence[float],
+    arr_time_gsi_days: t.Sequence[float],
+    arr_strnuc: t.Sequence[str],
     arr_abund_artis: dict[str, list[float]],
     t_model_init_days: float,
     dfcell: pd.DataFrame,
     pdfoutpath: Path,
     mgi: int,
+    hideinputmodelpoints: bool = True,
+    xmax: None | float = None,
 ) -> None:
-    dfpartcontrib_thiscell = dfpartcontrib.query("cellindex == (@mgi + 1) and particleid in @allparticledata.keys()")
+    dfpartcontrib_thiscell = dfpartcontrib[
+        (dfpartcontrib["cellindex"] == (mgi + 1)) & (dfpartcontrib["particleid"].isin(allparticledata.keys()))
+    ]
     frac_of_cellmass_sum = dfpartcontrib_thiscell.frac_of_cellmass.sum()
     print(f"frac_of_cellmass_sum: {frac_of_cellmass_sum} (can be < 1.0 because of missing particles)")
     # if arr_strnuc[0] != 'Ye':
     #     arr_strnuc.insert(0, 'Ye')
 
-    arr_abund_gsi: dict[str, np.ndarray[Any, np.dtype[np.float64]]] = {}
-
-    for strnuc in arr_strnuc:
-        arr_abund_gsi[strnuc] = np.zeros_like(arr_time_gsi_days)
+    arr_abund_gsi: dict[str, np.ndarray[t.Any, np.dtype[np.float64]]] = {
+        strnuc: np.zeros_like(arr_time_gsi_days) for strnuc in arr_strnuc
+    }
 
     # calculate the GSI values from the particles contributing to this cell
     for particleid, frac_of_cellmass in dfpartcontrib_thiscell[["particleid", "frac_of_cellmass"]].itertuples(
         index=False
     ):
-        frac_of_cellmass = dfpartcontrib_thiscell.query("particleid == @particleid").frac_of_cellmass.sum()
+        frac_of_cellmass = dfpartcontrib_thiscell[dfpartcontrib_thiscell["particleid"] == particleid][
+            "frac_of_cellmass"
+        ].sum()
 
         for strnuc in arr_strnuc:
             arr_abund_gsi[strnuc] += allparticledata[particleid][strnuc] * frac_of_cellmass / frac_of_cellmass_sum
 
     fig, axes = plt.subplots(
         nrows=len(arr_strnuc),
         ncols=1,
@@ -251,73 +266,77 @@
 
     axes[-1].set_xlabel("Time [days]")
     axis = axes[0]
     print("nuc", "gsi_abund", "inputmodel_abund", "artis_abund")
     for axis, strnuc in zip(axes, arr_strnuc):
         # print(arr_time_artis_days)
         xmin = min(arr_time_gsi_days) * 0.9
-        xmax = max(arr_time_gsi_days) * 1.03
-        # xmax = 5  # TODO: remove
+        xmax = xmax or max(arr_time_gsi_days) * 1.03
         axis.set_xlim(left=xmin, right=xmax)
         # axis.set_yscale('log')
         # axis.set_ylabel(f'X({strnuc})')
         if strnuc == "Ye":
             axis.set_ylabel("Electron fraction")
         else:
             axis.set_ylabel("Mass fraction")
 
+        strnuc_latex = strnuc_to_latex(strnuc)
+
         axis.plot(
             arr_time_gsi_days,
             arr_abund_gsi[strnuc],
             # linestyle='None',
             linewidth=2,
             marker="x",
             markersize=8,
-            label=f"{strnuc} GSI Network",
+            label=f"{strnuc_latex} Network",
             color="black",
         )
 
         if strnuc in arr_abund_artis:
             axis.plot(
                 arr_time_artis_days,
                 arr_abund_artis[strnuc],
                 linewidth=2,
                 # linestyle='None',
                 # marker='+', markersize=15,
-                label=f"{strnuc} ARTIS",
+                label=f"{strnuc_latex} ARTIS",
                 color="red",
             )
 
-        if f"X_{strnuc}" in dfcell:
+        if f"X_{strnuc}" in dfcell and not hideinputmodelpoints:
             axis.plot(
                 t_model_init_days,
                 dfcell[f"X_{strnuc}"],
                 marker="+",
                 markersize=15,
                 markeredgewidth=2,
-                label=f"{strnuc} ARTIS inputmodel",
+                label=f"{strnuc_latex} ARTIS inputmodel",
                 color="blue",
             )
             print(
                 f'{strnuc} {arr_abund_gsi[strnuc][0]:.2e} {dfcell[f"X_{strnuc}"]:.2e}, {arr_abund_artis[strnuc][0]:.2e}'
             )
 
         axis.legend(loc="best", frameon=False, handlelength=1, ncol=1, numpoints=1)
 
-    fig.suptitle(f"{modelname} cell {mgi}", y=0.995, fontsize=10)
+        at.plottools.autoscale(ax=axis)
+
+    # fig.suptitle(f"{modelname} cell {mgi}", y=0.995, fontsize=10)
     at.plottools.autoscale(axis, margin=0.05)
     fig.savefig(pdfoutpath, format="pdf")
     print(f"Saved {pdfoutpath}")
 
 
 def get_particledata(
-    arr_time_s: Sequence[float],
+    arr_time_s: t.Sequence[float],
     arr_strnuc: list[str],
     traj_root: Path,
     particleid: int,
+    verbose: bool = False,
 ) -> tuple[int, dict[str, np.ndarray]]:
     """For an array of times (NSM time including time before merger), interpolate the heating rates of various decay channels
     and (if arr_strnuc is not empty) the nuclear mass fractions.
     """
     try:
         nts_min = at.inputmodel.rprocess_from_trajectory.get_closest_network_timestep(
             traj_root, particleid, timesec=min(arr_time_s), cond="lessthan"
@@ -330,18 +349,19 @@
         print(f"No network calculation for particle {particleid}")
         # make sure we weren't requesting abundance data for this particle that has no network data
         if arr_strnuc:
             print("ERROR:", particleid, arr_strnuc)
         assert not arr_strnuc
         return -1, {}
 
-    print(
-        "Reading network calculation heating.dat,"
-        f" energy_thermo.dat{', and nz-plane abundances' if arr_strnuc else ''} for particle {particleid}..."
-    )
+    if verbose:
+        print(
+            "Reading network calculation heating.dat,"
+            f" energy_thermo.dat{', and nz-plane abundances' if arr_strnuc else ''} for particle {particleid}..."
+        )
 
     particledata = {}
     nstep_timesec = {}
     with at.inputmodel.rprocess_from_trajectory.open_tar_file_or_extracted(
         traj_root, particleid, "./Run_rprocess/heating.dat"
     ) as f:
         dfheating = pd.read_csv(
@@ -400,33 +420,34 @@
         for strnuc in arr_strnuc:
             massfracs_interp = np.interp(arr_time_s, arr_traj_time_s, arr_massfracs[strnuc])
             particledata[strnuc] = np.array(massfracs_interp)
 
     return particleid, particledata
 
 
-def plot_qdot_abund_modelcells(modelpath: Path, mgiplotlist: Sequence[int], arr_el_a: list[tuple[str, int]]):
+def plot_qdot_abund_modelcells(
+    modelpath: Path, mgiplotlist: t.Sequence[int], arr_el_a: list[tuple[str, int]], xmax: None | float = None
+):
     # default values, because early model.txt didn't specify this
     griddatafolder: Path = Path("SFHo_snapshot")
     mergermodelfolder: Path = Path("SFHo_short")
     trajfolder: Path = Path("SFHo")
     with at.zopen(modelpath / "model.txt") as fmodel:
         while True:
             line = fmodel.readline()
-            if line.startswith("#"):
-                if line.startswith("# gridfolder:"):
-                    griddatafolder = Path(line.strip().removeprefix("# gridfolder: "))
-                    mergermodelfolder = Path(line.strip().removeprefix("# gridfolder: ").removesuffix("_snapshot"))
-                elif line.startswith("# trajfolder:"):
-                    trajfolder = Path(line.strip().removeprefix("# trajfolder: ").replace("SFHO", "SFHo"))
-            else:
+            if not line.startswith("#"):
                 break
+            if line.startswith("# gridfolder:"):
+                griddatafolder = Path(line.strip().removeprefix("# gridfolder: "))
+                mergermodelfolder = Path(line.strip().removeprefix("# gridfolder: ").removesuffix("_snapshot"))
+            elif line.startswith("# trajfolder:"):
+                trajfolder = Path(line.strip().removeprefix("# trajfolder: ").replace("SFHO", "SFHo"))
 
-    # merger_root = Path(Path.home() / "Google Drive/Shared Drives/GSI NSM/Mergers")
-    merger_root = Path("/Users/luke/Downloads/Mergers")
+    merger_root = Path(Path.home() / "Google Drive/Shared Drives/GSI NSM/Mergers")
+    # merger_root = Path("/Users/luke/Downloads/Mergers")
     griddata_root = Path(merger_root, mergermodelfolder, griddatafolder)
     traj_root = Path(merger_root, mergermodelfolder, trajfolder)
     print(f"model.txt traj_root: {traj_root}")
     print(f"model.txt griddata_root: {griddata_root}")
     assert traj_root.is_dir()
 
     arr_el, arr_a = zip(*arr_el_a)
@@ -455,15 +476,15 @@
         corr = (
             dfmodel.eval(f"X_{strnuc} * cellmass_grams_mapped").sum()
             / dfmodel.eval(f"X_{strnuc} * cellmass_grams").sum()
         )
         # print(strnuc, corr)
         correction_factors[strnuc] = corr
 
-    tmids = at.get_timestep_times_float(modelpath, loc="mid")
+    tmids = at.get_timestep_times(modelpath, loc="mid")
     MH = 1.67352e-24  # g
 
     arr_time_artis_days: list[float] = []
     arr_abund_artis: dict[int, dict[str, list[float]]] = {}
     get_global_Ye = False
     artis_ye_sum: dict[int, float] = {}
     artis_ye_norm: dict[int, float] = {}
@@ -519,15 +540,15 @@
                 cell_protoncount = 0.0
                 cell_nucleoncount = 0.0
                 cellvolume = dfmodel.iloc[mgi].cellmass_grams / rho_cgs
                 for popkey, abund in estimators[(nts, mgi)]["populations"].items():
                     if isinstance(popkey, str) and abund > 0.0:
                         if popkey.endswith("_otherstable"):
                             # TODO: use mean molecular weight, but this is not needed for kilonova input files anyway
-                            pass
+                            print(f"WARNING {popkey}={abund} not contributed")
                         else:
                             try:
                                 z, a = at.get_z_a_nucname(popkey)
                                 cell_protoncount += z * abund * cellvolume
                                 cell_nucleoncount += a * abund * cellvolume
 
                             except AssertionError:
@@ -539,50 +560,51 @@
                 artis_ye_norm[nts] = artis_ye_norm.get(nts, 0.0) + cell_nucleoncount
 
         arr_artis_ye = [artis_ye_sum[nts] / artis_ye_norm[nts] for nts in sorted(artis_ye_sum.keys())]
 
     except FileNotFoundError:
         pass
 
-    arr_time_artis_days_alltimesteps = at.get_timestep_times_float(modelpath)
+    arr_time_artis_days_alltimesteps = at.get_timestep_times(modelpath)
     arr_time_artis_s_alltimesteps = np.array([t * 8.640000e04 for t in arr_time_artis_days_alltimesteps])
     # no completed timesteps yet, so display full set of timesteps that artis will compute
-    if len(arr_time_artis_days) == 0:
+    if not arr_time_artis_days:
         arr_time_artis_days = list(arr_time_artis_days_alltimesteps)
 
     arr_time_gsi_s = np.array([t_model_init_days * 86400, *arr_time_artis_s_alltimesteps])
 
     # times in artis are relative to merger, but NSM simulation time started earlier
     mergertime_geomunits = at.inputmodel.modelfromhydro.get_merger_time_geomunits(griddata_root)
     t_mergertime_s = mergertime_geomunits * 4.926e-6
     arr_time_gsi_s_incpremerger = np.array([t_model_init_days * 86400 + t_mergertime_s, *arr_time_artis_s_alltimesteps])
     arr_time_gsi_days = list(arr_time_gsi_s / 86400)
 
     dfpartcontrib = at.inputmodel.rprocess_from_trajectory.get_gridparticlecontributions(modelpath)
-    dfpartcontrib = dfpartcontrib.query("cellindex <= @npts_model and frac_of_cellmass > 0")
+    dfpartcontrib = dfpartcontrib[(dfpartcontrib["cellindex"] <= npts_model) & (dfpartcontrib["frac_of_cellmass"] > 0)]
 
-    list_particleids_getabund = dfpartcontrib.query("(cellindex - 1) in @mgiplotlist").particleid.unique()
-    fworkerwithabund = partial(get_particledata, arr_time_gsi_s_incpremerger, arr_strnuc, traj_root)
+    mgiplotlistplus1 = (mgi + 1 for mgi in mgiplotlist)
+    list_particleids_getabund = dfpartcontrib[dfpartcontrib["cellindex"].isin(mgiplotlistplus1)].particleid.unique()
+    fworkerwithabund = partial(get_particledata, arr_time_gsi_s_incpremerger, arr_strnuc, traj_root, verbose=True)
 
     print(f"Reading trajectories from {traj_root}")
-    print(f"  Reading Qdot/thermo and abundance data for {len(list_particleids_getabund)} particles")
+    print(f"Reading Qdot/thermo and abundance data for {len(list_particleids_getabund)} particles")
 
     if at.get_config()["num_processes"] > 1:
         with multiprocessing.get_context("fork").Pool(processes=at.get_config()["num_processes"]) as pool:
             list_particledata_withabund = pool.map(fworkerwithabund, list_particleids_getabund)
             pool.close()
             pool.join()
     else:
         list_particledata_withabund = [fworkerwithabund(particleid) for particleid in list_particleids_getabund]
 
     list_particleids_noabund = [
         pid for pid in dfpartcontrib.particleid.unique() if pid not in list_particleids_getabund
     ]
     fworkernoabund = partial(get_particledata, arr_time_gsi_s_incpremerger, [], traj_root)
-    print(f"  Reading for Qdot/thermo data (no abundances needed) for {len(list_particleids_noabund)} particles")
+    print(f"Reading for Qdot/thermo data (no abundances needed) for {len(list_particleids_noabund)} particles")
 
     if at.get_config()["num_processes"] > 1:
         with multiprocessing.get_context("fork").Pool(processes=at.get_config()["num_processes"]) as pool:
             list_particledata_noabund = pool.map(fworkernoabund, list_particleids_noabund)
             pool.close()
             pool.join()
     else:
@@ -595,14 +617,15 @@
         dfpartcontrib,
         dfmodel,
         allparticledata,
         arr_time_artis_days,
         arr_artis_ye,
         arr_time_gsi_days,
         pdfoutpath=Path(modelpath, "gsinetwork_global-qdot.pdf"),
+        xmax=xmax,
     )
 
     for mgi in mgiplotlist:
         plot_cell_abund_evolution(
             modelpath,
             dfpartcontrib,
             allparticledata,
@@ -610,22 +633,25 @@
             arr_time_gsi_days,
             arr_strnuc,
             arr_abund_artis.get(mgi, {}),
             t_model_init_days,
             dfmodel.iloc[mgi],
             mgi=mgi,
             pdfoutpath=Path(modelpath, f"gsinetwork_cell{mgi}-abundance.pdf"),
+            xmax=xmax,
         )
 
 
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("-modelpath", default=".", help="Path for ARTIS files")
 
     parser.add_argument("-outputpath", "-o", default=".", help="Path for output files")
 
+    parser.add_argument("-xmax", default=None, type=int, help="Maximum time in days to plot")
+
     parser.add_argument(
         "-modelgridindex",
         "-cell",
         "-mgi",
         default=None,
         help="Modelgridindex (zero-indexed) to plot or list such as 4,5,6",
     )
@@ -638,37 +664,57 @@
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
 
     arr_el_a = [
-        # ("He", 4),
-        ("Ga", 72),
+        ("He", 4),
+        # ("Ga", 72),
         ("Sr", 89),
+        ("Sr", 91),
+        ("Sr", 92),
+        ("Y", 92),
+        ("Y", 93),
+        ("Zr", 93),
         ("Ba", 140),
         ("Ce", 141),
         ("Nd", 147),
         # ('Rn', 222),
-        ("Ra", 223),
-        ("Ra", 224),
-        ("Ra", 225),
+        # ("Ra", 223),
+        # ("Ra", 224),
+        # ("Ra", 225),
         # ("Ac", 225),
         # ('Th', 234),
         # ('Pa', 233),
         # ('U', 235),
     ]
-    arr_el_a.sort(key=lambda x: (at.get_atomic_number(x[0]), -x[1]))
+
+    # arr_el_a = [
+    #     ("He", 4),
+    #     ("Ga", 72),
+    #     ("Sr", 91),
+    #     ("Sr", 92),
+    # ]
+
+    # arr_el_a = [
+    #     ("Y", 92),
+    #     ("Zr", 93),
+    #     ("Ce", 141),
+    #     ("Nd", 147),
+    # ]
+
+    arr_el_a.sort(key=lambda x: (at.get_atomic_number(x[0]), x[1]))
 
     modelpath = Path(args.modelpath)
     if args.modelgridindex is None:
         mgiplotlist = []
     elif hasattr(args.modelgridindex, "split"):
         mgiplotlist = [int(mgi) for mgi in args.modelgridindex.split(",")]
     else:
         mgiplotlist = [int(args.modelgridindex)]
 
-    plot_qdot_abund_modelcells(modelpath, mgiplotlist, arr_el_a)
+    plot_qdot_abund_modelcells(modelpath, mgiplotlist, arr_el_a, xmax=args.xmax)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `artistools-2023.5.16.3/artistools/hesma_scripts.py` & `artistools-2023.8.1/artistools/hesma_scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def plot_hesma_spectrum(timeavg, axes):
     hesma_file = Path("/Users/ccollins/Downloads/hesma_files/M2a/hesma_specseq.dat")
     hesma_spec = pd.read_csv(hesma_file, comment="#", delim_whitespace=True, dtype=float)
     # print(hesma_spec)
 
     def match_closest_time(reftime):
-        return str(f"{min([float(x) for x in hesma_spec.keys()[1:]], key=lambda x: abs(x - reftime))}")
+        return str(f"{min((float(x) for x in hesma_spec.keys()[1:]), key=lambda x: abs(x - reftime))}")
 
     closest_time = match_closest_time(timeavg)
     closest_time = f"{closest_time:.2f}"
     print(closest_time)
 
     # Scale distance to 1 Mpc
     dist_mpc = 1e-5  # HESMA specta at 10 pc
@@ -92,15 +92,15 @@
         outfilename = f"{modelname}_vspec_res.dat"
         if angle == 0:
             vspecdata.to_csv(outpath / outfilename, sep=" ", index=False)  # create file
         else:
             # append to file
             vspecdata.to_csv(outpath / outfilename, mode="a", sep=" ", index=False)
 
-    with open(outpath / outfilename, "r+") as f:  # add comment to start of file
+    with (outpath / outfilename).open("r+") as f:  # add comment to start of file
         content = f.read()
         f.seek(0, 0)
         f.write(
             f"# File contains spectra at observer angles {angle_names} for Model {modelname}.\n# A header line"
             " containing spectra time is repeated at the beginning of each observer angle. Column 0 gives wavelength."
             " \n# Spectra are at a distance of 10 pc."
             "\n"
@@ -139,17 +139,18 @@
             names=["peakmag", "risetime", "dm40"],
             skiprows=1,
         )
 
     angles = np.arange(0, 100)
     angle_definition = at.get_dirbin_labels(angles, modelpath=None)
 
-    outdata = {}
-    outdata["peakmag"] = dm15data["peakmag"]  # dm15 peak mag probably more accurate - shorter time window
-    outdata["dm15"] = dm15data["dm15"]
+    outdata = {
+        "peakmag": dm15data["peakmag"],  # dm15 peak mag probably more accurate - shorter time window
+        "dm15": dm15data["dm15"],
+    }
     if dm40:
         outdata["dm40"] = dm40data["dm40"]
     outdata["angle_bin"] = angle_definition.values()
 
     outdataframe = pd.DataFrame(outdata)
     outdataframe = outdataframe.round(decimals=4)
     outdataframe.to_csv(outpath / f"{modelname}_width-luminosity.dat", sep=" ", index=False, header=True)
```

### Comparing `artistools-2023.5.16.3/artistools/initial_composition.py` & `artistools-2023.8.1/artistools/initial_composition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
+from __future__ import annotations
+
 import argparse
 import math
-import os
+import typing as t
 from pathlib import Path
-from typing import Any
-from typing import Literal
-from typing import Optional
 
 import argcomplete
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
-import pandas as pd
 from astropy import units as u
 
 import artistools as at
 
+if t.TYPE_CHECKING:
+    import pandas as pd
+
 
-def plot_2d_initial_abundances(modelpath, args):
+def plot_2d_initial_abundances(modelpath: Path, args: argparse.Namespace) -> None:
     model = at.inputmodel.get_2d_modeldata(modelpath)
     abundances = at.inputmodel.get_initelemabundances(modelpath)
 
     abundances["inputcellid"] = abundances["inputcellid"].apply(float)
 
     merge_dfs = model.merge(abundances, how="inner", on="inputcellid")
 
-    with open(os.path.join(modelpath, "model.txt")) as fmodelin:
+    with Path(modelpath, "model.txt").open() as fmodelin:
         fmodelin.readline()  # npts r, npts z
         t_model = float(fmodelin.readline())  # days
         vmax = float(fmodelin.readline())  # v_max in [cm/s]
 
     r = merge_dfs["cellpos_mid[r]"] / t_model * (u.cm / u.day).to("km/s") / 10**3
     z = merge_dfs["cellpos_mid[z]"] / t_model * (u.cm / u.day).to("km/s") / 10**3
 
@@ -52,19 +53,19 @@
     outfilename = f"plotcomposition{args.plotvars}.pdf"
     plt.savefig(Path(modelpath) / outfilename, format="pdf")
     print(f"Saved {outfilename}")
 
 
 def get_2D_slice_through_3d_model(
     dfmodel: pd.DataFrame,
-    sliceaxis: Literal["x", "y", "z"],
-    modelmeta: Optional[dict[str, Any]] = None,
-    plotaxis1: Optional[Literal["x", "y", "z"]] = None,
-    plotaxis2: Optional[Literal["x", "y", "z"]] = None,
-    sliceindex: Optional[int] = None,
+    sliceaxis: t.Literal["x", "y", "z"],
+    modelmeta: dict[str, t.Any] | None = None,
+    plotaxis1: t.Literal["x", "y", "z"] | None = None,
+    plotaxis2: t.Literal["x", "y", "z"] | None = None,
+    sliceindex: int | None = None,
 ) -> pd.DataFrame:
     if not sliceindex:
         # get midpoint
         sliceposition: float = dfmodel.iloc[(dfmodel["pos_x_min"]).abs().argsort()][:1]["pos_x_min"].item()
         # Choose position to slice. This gets minimum absolute value as the closest to 0
     else:
         cell_boundaries = []
@@ -167,28 +168,25 @@
             f"Scaling modeldata to {targetmodeltime_days} days. \nWARNING: abundances not scaled for radioactive decays"
         )
 
         dfmodel, modelmeta = at.inputmodel.scale_model_to_time(
             targetmodeltime_days=targetmodeltime_days, modelmeta=modelmeta, dfmodel=dfmodel
         )
 
-    sliceaxis: Literal["x", "y", "z"] = "z"
+    sliceaxis: t.Literal["x", "y", "z"] = "z"
 
-    axes: list[Literal["x", "y", "z"]] = ["x", "y", "z"]
-    plotaxis1: Literal["x", "y", "z"] = [ax for ax in axes if ax != sliceaxis][0]
-    plotaxis2: Literal["x", "y", "z"] = [ax for ax in axes if ax not in [sliceaxis, plotaxis1]][0]
+    axes: list[t.Literal["x", "y", "z"]] = ["x", "y", "z"]
+    plotaxis1: t.Literal["x", "y", "z"] = next(ax for ax in axes if ax != sliceaxis)
+    plotaxis2: t.Literal["x", "y", "z"] = next(ax for ax in axes if ax not in [sliceaxis, plotaxis1])
 
     df2dslice = get_2D_slice_through_3d_model(
         dfmodel=dfmodel, modelmeta=modelmeta, sliceaxis=sliceaxis, plotaxis1=plotaxis1, plotaxis2=plotaxis2
     )
 
-    subplots = False
-    if len(args.plotvars) > 1:
-        subplots = True
-
+    subplots = bool(len(args.plotvars) > 1)
     if not subplots:
         fig, ax = plt.subplots(1, 1, figsize=(8, 7), tight_layout={"pad": 0.4, "w_pad": 0.0, "h_pad": 0.0})
     else:
         rows = 1
         cols = len(args.plotvars)
 
         fig, axes = plt.subplots(
@@ -219,33 +217,32 @@
         plt.xlabel(xlabel, fontsize="x-large")  # , fontweight='bold')
         plt.ylabel(ylabel, fontsize="x-large")  # , fontweight='bold')
     else:
         cbar = fig.colorbar(scaledmap, ax=axes, shrink=cols * 0.08, location="top", pad=0.8, anchor=(0.5, 3.0))
         fig.text(0.5, 0.15, xlabel, ha="center", va="center")
         fig.text(0.05, 0.5, ylabel, ha="center", va="center", rotation="vertical")
 
-    # cbar.set_label(label="test", size="x-large")  # , fontweight='bold')
     if "cellYe" not in args.plotvars and "tracercount" not in args.plotvars:
         if args.logcolorscale:
             cbar.ax.set_title(r"log10($\rho$) [g/cm3]", size="small")
         else:
             cbar.ax.set_title(r"$\rho$ [g/cm3]", size="small")
     # cbar.ax.tick_params(labelsize='x-large')
 
     # plt.tight_layout()
     # ax.labelsize: 'large'
     # plt.title(f'At {sliceaxis} = {sliceposition}')
 
-    outfilename = args.outputfile if args.outputfile else f"plotcomposition_{','.join(args.plotvars)}.pdf"
+    outfilename = args.outputfile or f"plotcomposition_{','.join(args.plotvars)}.pdf"
     plt.savefig(Path(modelpath) / outfilename, format="pdf")
 
     print(f"Saved {outfilename}")
 
 
-def get_model_abundances_Msun_1D(modelpath):
+def get_model_abundances_Msun_1D(modelpath: Path) -> pd.DataFrame:
     filename = modelpath / "model.txt"
     modeldata, t_model_init_days, _ = at.inputmodel.get_modeldata_tuple(filename)
     abundancedata = at.inputmodel.get_initelemabundances(modelpath)
 
     t_model_init_seconds = t_model_init_days * 24 * 60 * 60
 
     modeldata["volume_shell"] = (
@@ -278,17 +275,15 @@
 
     merge_dfs = model.merge(abundances, how="inner", on="inputcellid")
     elements = [x for x in merge_dfs if "X_" in x]
 
     merge_dfs["max"] = merge_dfs[elements].idxmax(axis=1)
 
     merge_dfs["max"] = merge_dfs["max"].apply(lambda x: at.get_atomic_number(x[2:]))
-    merge_dfs = merge_dfs[merge_dfs["max"] != 1]
-
-    return merge_dfs
+    return merge_dfs[merge_dfs["max"] != 1]
 
 
 def make_3d_plot(modelpath, args):
     import pyvista as pv
 
     pv.set_plot_theme("document")  # set white background
 
@@ -314,17 +309,17 @@
     grid = round(len(model["rho"]) ** (1.0 / 3.0))
     surfacecolorscale = np.zeros((grid, grid, grid))  # needs 3D array
     xgrid = np.zeros(grid)
 
     surfacearr = np.array(model[coloursurfaceby])
 
     i = 0
-    for z in range(0, grid):
-        for y in range(0, grid):
-            for x in range(0, grid):
+    for z in range(grid):
+        for y in range(grid):
+            for x in range(grid):
                 surfacecolorscale[x, y, z] = surfacearr[i]
                 xgrid[x] = -vmax + 2 * x * vmax / grid
                 i += 1
 
     x, y, z = np.meshgrid(xgrid, xgrid, xgrid)
 
     mesh = pv.StructuredGrid(x, y, z)
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/1dslicefrom3d.py` & `artistools-2023.8.1/artistools/inputmodel/1dslicefrom3d.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 import argparse
 import math
-import os
 import sys
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 
 from artistools import CustomArgHelpFormatter
 
@@ -53,15 +52,15 @@
 
 def slice_3dmodel(inputfolder, outputfolder, chosenaxis):
     xlist = []
     ylists = [[], [], []]
     listout = []
     dict3dcellidto1dcellid = {}
     outcellid = 0
-    with open(os.path.join(inputfolder, "model.txt")) as fmodelin:
+    with Path(inputfolder, "model.txt").open() as fmodelin:
         fmodelin.readline()  # npts_model3d
         t_model = fmodelin.readline()  # days
         fmodelin.readline()  # v_max in [cm/s]
 
         while True:
             # two lines making up a model grid cell
             block = fmodelin.readline(), fmodelin.readline()
@@ -93,27 +92,27 @@
                 outcellid += 1
                 dict3dcellidto1dcellid[int(cell["cellid"])] = outcellid
                 append_cell_to_output(cell, outcellid, t_model, listout, xlist, ylists)
                 print(f"Cell {outcellid:4d} input1: {block[0].rstrip()}")
                 print(f"Cell {outcellid:4d} input2: {block[1].rstrip()}")
                 print(f"Cell {outcellid:4d} output: {listout[-1]}")
 
-    with open(os.path.join(outputfolder, "model.txt"), "w") as fmodelout:
+    with Path(outputfolder, "model.txt").open("w") as fmodelout:
         fmodelout.write(f"{outcellid:7d}\n")
         fmodelout.write(t_model)
         for line in listout:
             fmodelout.write(line + "\n")
 
     return dict3dcellidto1dcellid, xlist, ylists
 
 
 def slice_abundance_file(inputfolder, outputfolder, dict3dcellidto1dcellid):
     with (
-        open(os.path.join(inputfolder, "abundances.txt")) as fabundancesin,
-        open(os.path.join(outputfolder, "abundances.txt"), "w") as fabundancesout,
+        Path(inputfolder, "abundances.txt").open() as fabundancesin,
+        Path(outputfolder, "abundances.txt").open("w") as fabundancesout,
     ):
         currentblock = []
         keepcurrentblock = False
         for line in fabundancesin:
             linesplit = line.split()
 
             if len(currentblock) + len(linesplit) >= 30:
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/__init__.py` & `artistools-2023.8.1/artistools/inputmodel/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import artistools.inputmodel.botyanski2017
-import artistools.inputmodel.describeinputmodel
-import artistools.inputmodel.downscale3dgrid
-import artistools.inputmodel.energyinputfiles
-import artistools.inputmodel.makeartismodel
-import artistools.inputmodel.maketardismodelfromartis
-import artistools.inputmodel.modelfromhydro
-import artistools.inputmodel.opacityinputfile
-import artistools.inputmodel.rprocess_from_trajectory
-
+from . import botyanski2017
+from . import describeinputmodel
+from . import downscale3dgrid
+from . import energyinputfiles
+from . import makeartismodel
+from . import maketardismodelfromartis
+from . import modelfromhydro
+from . import opacityinputfile
+from . import rprocess_from_trajectory
 from .inputmodel_misc import add_derived_cols_to_modeldata
 from .inputmodel_misc import get_2d_modeldata
 from .inputmodel_misc import get_3d_model_data_merged_model_and_abundances_minimal
 from .inputmodel_misc import get_3d_modeldata_minimal
 from .inputmodel_misc import get_cell_angle
 from .inputmodel_misc import get_dfmodel_dimensions
 from .inputmodel_misc import get_initelemabundances
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/botyanski2017.py` & `artistools-2023.8.1/artistools/inputmodel/botyanski2017.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 import argparse
 import math
-import os.path
+from pathlib import Path
 
 import numpy as np
 import pandas as pd
 from astropy import units as u
 
 import artistools as at
 
@@ -95,13 +95,13 @@
         vol_shell = 4 * math.pi / 3 * (r_outer**3 - r_inner**3)
         m_shell = rho * vol_shell / u.solMass.to("g")
         m_tot += m_shell
 
         v_inner = v_outer
     print(f"M_tot = {m_tot:.3f} solMass")
 
-    at.inputmodel.save_modeldata(dfmodel, t_model_init_days, os.path.join(args.outputpath, "model.txt"))
-    at.inputmodel.save_initelemabundances(dfelabundances, os.path.join(args.outputpath, "abundances.txt"))
+    at.inputmodel.save_modeldata(dfmodel, t_model_init_days, Path(args.outputpath, "model.txt"))
+    at.inputmodel.save_initelemabundances(dfelabundances, Path(args.outputpath, "abundances.txt"))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/describeinputmodel.py` & `artistools-2023.8.1/artistools/inputmodel/describeinputmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         action="store_true",
         help="Give element abundances only, no isotope abundances (implies --getelemabundances)",
     )
 
     parser.add_argument("--getelemabundances", action="store_true", help="Get elemental abundance masses")
 
 
-def main(args=None, argsraw=None, **kwargs):
+def main(args=None, argsraw=None, **kwargs) -> None:
     """Describe an ARTIS input model, such as the mass, velocity structure, and abundances."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
             description=__doc__,
         )
 
@@ -73,15 +73,15 @@
             dfmodel = dfmodel.query("inputcellid == (@mgi + 1)")
             print(dfmodel.iloc[0])
 
     mass_msun_rho = dfmodel["cellmass_grams"].sum() / 1.989e33
 
     mass_msun_isotopes = 0.0
     mass_msun_elem = 0.0
-    speciesmasses = {}
+    speciesmasses: dict[str, float] = {}
     for column in dfmodel.columns:
         if column.startswith("X_"):
             species = column.replace("X_", "")
             speciesabund_g = np.dot(dfmodel[column], dfmodel["cellmass_grams"])
 
             species_mass_msun = speciesabund_g / 1.989e33
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/downscale3dgrid.py` & `artistools-2023.8.1/artistools/inputmodel/downscale3dgrid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from __future__ import annotations
+
 from pathlib import Path
-from typing import Union
 
 import numpy as np
 
 import artistools as at
 
 
-def make_downscaled_3d_grid(modelpath: Union[str, Path], outputgridsize: int = 50, plot: bool = False) -> Path:
-    """Should be same as downscale_3d_grid.pro
-    Expects a 3D model with grid^3 cells and outputs 3D model with smallgrid^3 cells.
+def make_downscaled_3d_grid(modelpath: str | Path, outputgridsize: int = 50, plot: bool = False) -> Path:
+    """Get a 3D model with smallgrid^3 cells from a 3D model with grid^3 cells.
+    Should be same as downscale_3d_grid.pro.
     """
     modelpath = Path(modelpath)
 
     dfmodel, modelmeta = at.get_modeldata(modelpath, dtype_backend="pyarrow")
     dfelemabund = at.inputmodel.get_initelemabundances(modelpath, dtype_backend="pyarrow")
 
     inputgridsize = modelmeta["ncoordgrid"]
@@ -39,89 +40,89 @@
     max_atomic_number = len(dfelemabund.columns) - 1
     assert max_atomic_number == 30
     abund = np.zeros((grid, grid, grid, max_atomic_number + 1))
 
     print("reading abundance file")
 
     cellindex = 0
-    for z in range(0, grid):
-        for y in range(0, grid):
-            for x in range(0, grid):
+    for z in range(grid):
+        for y in range(grid):
+            for x in range(grid):
                 abund[x, y, z] = dfelemabund.iloc[cellindex].to_numpy()
                 cellindex += 1
 
     print("reading model file")
     t_model_days = modelmeta["t_model_init_days"]
     vmax = modelmeta["vmax_cmps"]
 
     cellindex = 0
-    for z in range(0, grid):
-        for y in range(0, grid):
-            for x in range(0, grid):
+    for z in range(grid):
+        for y in range(grid):
+            for x in range(grid):
                 rho[x, y, z] = dfmodel.iloc[cellindex]["rho"]
                 radioabunds[x, y, z, :] = dfmodel.iloc[cellindex][abundcols]
 
                 cellindex += 1
 
     rho_small = np.zeros((smallgrid, smallgrid, smallgrid))
     radioabunds_small = np.zeros((smallgrid, smallgrid, smallgrid, nabundcols))
     abund_small = np.zeros((smallgrid, smallgrid, smallgrid, max_atomic_number + 1))
 
-    for z in range(0, smallgrid):
-        for y in range(0, smallgrid):
-            for x in range(0, smallgrid):
-                for zz in range(0, merge):
-                    for yy in range(0, merge):
-                        for xx in range(0, merge):
+    for z in range(smallgrid):
+        for y in range(smallgrid):
+            for x in range(smallgrid):
+                for zz in range(merge):
+                    for yy in range(merge):
+                        for xx in range(merge):
                             rho_small[x, y, z] += rho[x * merge + xx, y * merge + yy, z * merge + zz]
                             for i in range(nabundcols):
                                 radioabunds_small[x, y, z, i] += (
                                     radioabunds[x * merge + xx, y * merge + yy, z * merge + zz, i]
                                     * rho[x * merge + xx, y * merge + yy, z * merge + zz]
                                 )
 
                             abund_small[x, y, z, :] += (
                                 abund[x * merge + xx, y * merge + yy, z * merge + zz]
                                 * rho[x * merge + xx, y * merge + yy, z * merge + zz]
                             )
 
-    for z in range(0, smallgrid):
-        for y in range(0, smallgrid):
-            for x in range(0, smallgrid):
+    for z in range(smallgrid):
+        for y in range(smallgrid):
+            for x in range(smallgrid):
                 if rho_small[x, y, z] > 0:
                     radioabunds_small[x, y, z, :] /= rho_small[x, y, z]
 
                     for i in range(1, max_atomic_number + 1):  # check this
                         abund_small[x, y, z, i] /= rho_small[x, y, z]
                     rho_small[x, y, z] /= merge**3
 
     print("writing abundance file")
     i = 0
-    with open(modelpath / smallabundancefile, "w") as newabundancefile:
-        for z in range(0, smallgrid):
-            for y in range(0, smallgrid):
-                for x in range(0, smallgrid):
+    with (modelpath / smallabundancefile).open("w") as newabundancefile:
+        for z in range(smallgrid):
+            for y in range(smallgrid):
+                for x in range(smallgrid):
                     line = abund_small[x, y, z, :].tolist()  # index 1:30 are abundances
                     line[0] = int(i + 1)  # replace index 0 with index id
                     i += 1
                     newabundancefile.writelines("%g " % item for item in line)
                     newabundancefile.writelines("\n")
 
     print("writing model file")
     xmax = vmax * t_model_days * 3600 * 24
     cellindex = 0
-    with open(modelpath / smallmodelfile, "w") as newmodelfile:
+    with (modelpath / smallmodelfile).open("w") as newmodelfile:
         gridsize = int(smallgrid**3)
         newmodelfile.write(f"{gridsize}\n")
         newmodelfile.write(f"{t_model_days}\n")
         newmodelfile.write(f"{vmax}\n")
 
-        for z in range(0, smallgrid):
-            for y in range(0, smallgrid):
-                for x in range(0, smallgrid):
+        for z in range(smallgrid):
+            for y in range(smallgrid):
+                for x in range(smallgrid):
                     line1 = [
                         int(cellindex + 1),
                         -xmax + 2 * x * xmax / smallgrid,
                         -xmax + 2 * y * xmax / smallgrid,
                         -xmax + 2 * z * xmax / smallgrid,
                         rho_small[x, y, z],
                     ]
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/energyinputfiles.py` & `artistools-2023.8.1/artistools/inputmodel/energyinputfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 DAY = 86400  # day in seconds
 MSUN = 1.989e33  # solar mass in grams
 
 
 def write_energydistribution_file(energydistdata, outputfilepath="."):
     print("Writing energydistribution.txt")
-    with open(Path(outputfilepath) / "energydistribution.txt", "w") as fmodel:
+    with Path(outputfilepath, "energydistribution.txt").open("w") as fmodel:
         fmodel.write(f'{len(energydistdata["cell_energy"])}\n')  # write number of points
         energydistdata.to_csv(fmodel, header=False, sep="\t", index=False, float_format="%g")
 
 
 def write_energyrate_file(energy_rate_data, outputfilepath="."):
     print("Writing energyrate.txt")
-    with open(Path(outputfilepath) / "energyrate.txt", "w") as fmodel:
+    with Path(outputfilepath, "energyrate.txt").open("w") as fmodel:
         fmodel.write(f'{len(energy_rate_data["times"])}\n')  # write number of points
         energy_rate_data.to_csv(fmodel, sep="\t", index=False, header=False, float_format="%.10f")
 
 
 def rprocess_const_and_powerlaw():
     """Following eqn 4 Korobkin 2012."""
 
@@ -198,17 +198,15 @@
 
     cellenergy = np.array([Etot] * numberofcells)
     cellenergy = cellenergy * (rho / sum(rho))
 
     energydistdata = {"cellid": np.arange(1, len(rho) + 1), "cell_energy": cellenergy}
 
     print(f"sum energy cells {sum(energydistdata['cell_energy'])} should equal Etot")
-    energydistdata = pd.DataFrame(data=energydistdata)
-
-    return energydistdata
+    return pd.DataFrame(data=energydistdata)
 
 
 def make_energy_files(rho, Mtot_grams, outputpath=None, modelpath=None, model=None):
     powerlaw = True
     if powerlaw:
         print("Using power law for energy rate")
         # times_and_rate, E_tot_per_gram = rprocess_const_and_powerlaw()
@@ -252,11 +250,10 @@
         names=["cellid", "cell_energy"],
     )
     etot = energydistribution_data["cell_energy"].sum()
     return etot, energydistribution_data
 
 
 def get_energy_rate_fromfile(modelpath):
-    energyrate_data = pd.read_csv(
+    return pd.read_csv(
         Path(modelpath) / "energyrate.txt", skiprows=1, delim_whitespace=True, header=None, names=["times", "rate"]
     )
-    return energyrate_data
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py` & `artistools-2023.8.1/artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 """Convert a CMFGEN model file to ARTIS format. Original script possibly by Markus Kromer?."""
 # from rd_cmfgen import rd_nuc_decay_data
 from math import exp
+from pathlib import Path
 
 import numpy as np
 
 from .rd_cmfgen import rd_sn_hydro_data
 
 msun = 1.989e33
 
@@ -75,17 +76,15 @@
                     s,
                     f" goes fully to top isotope Z={zparent} A={numnucleons} of the chain at time zero",
                 )
             else:
                 print(
                     "shell",
                     s,
-                    " has none of the last isotope Z={} A={} of the chain at time zero".format(
-                        zparent - 2, numnucleons
-                    ),
+                    f" has none of the last isotope Z={zparent - 2} A={numnucleons} of the chain at time zero",
                 )
         else:
             iso3fromdecay[s] = (
                 (iso1fract0[s] + iso2fract0[s]) * (lamb1 - lamb2)
                 - iso2fract0[s] * lamb1 * exp(-lamb2 * tlate)
                 + iso2fract0[s] * lamb2 * exp(-lamb2 * tlate)
                 - iso1fract0[s] * lamb1 * exp(-lamb2 * tlate)
@@ -154,16 +153,16 @@
     a["specfrac"][:, indexofatomicnumber[zparent - 2]] += iso3fraclate - iso3fract0
 
 
 def timeshift_double_decay(
     a, indexofatomicnumber, indexofisotope, zparent, numnucleons, timeold, timenew, meanlife1_days, meanlife2_days
 ):
     # take abundances back to time zero and then forward to the selected model time
-    elfracsum_before = sum([a["specfrac"][:, indexofatomicnumber[zparent - i]] for i in range(3)])
-    isofracsum_before = sum([a["isofrac"][:, indexofisotope[(zparent - i, numnucleons)]] for i in range(3)])
+    elfracsum_before = sum(a["specfrac"][:, indexofatomicnumber[zparent - i]] for i in range(3))
+    isofracsum_before = sum(a["isofrac"][:, indexofisotope[(zparent - i, numnucleons)]] for i in range(3))
 
     reverse_doubledecay(
         a,
         indexofatomicnumber,
         indexofisotope,
         zparent=zparent,
         numnucleons=numnucleons,
@@ -179,16 +178,16 @@
         zparent=zparent,
         numnucleons=numnucleons,
         tlate=timenew,
         meanlife1_days=meanlife1_days,
         meanlife2_days=meanlife2_days,
     )
 
-    elfracsum_after = sum([a["specfrac"][:, indexofatomicnumber[zparent - i]] for i in range(3)])
-    isofracsum_after = sum([a["isofrac"][:, indexofisotope[(zparent - i, numnucleons)]] for i in range(3)])
+    elfracsum_after = sum(a["specfrac"][:, indexofatomicnumber[zparent - i]] for i in range(3))
+    isofracsum_after = sum(a["isofrac"][:, indexofisotope[(zparent - i, numnucleons)]] for i in range(3))
     assert np.all(abs(elfracsum_before - elfracsum_after) < 1e-10)
 
 
 def main():
     a = rd_sn_hydro_data(snapshot, reverse="true")
 
     # Mapping of the CMFGEN species to atomic numbers, and masking IGEs
@@ -205,15 +204,15 @@
     rout = np.append(rout, r[-1])  # cmfgen uses the radius of the outermost zone as the outer boundary
     rin = rmax
     rin = np.insert(rin, 0, 0)  # for artis we use 0 as inner radius for the innermost shell, cmfgen uses
     # the innermost radius r[0], this gives a slight discrepancy (<1%) in the total mass
     dm = 4 / 3 * np.pi * (rout**3 - rin**3) * a["dens"] / msun
     print(dm.sum(), dm.sum() / (a["dmass"].sum() / msun))  # Check total mass
 
-    with open(model + "/model.txt", "w") as f:
+    with Path(model, "model.txt").open("w") as f:
         f.write(str(a["nd"]) + "\n")
         f.write(str(a["time"]) + "\n")
 
         for i in range(a["nd"]):
             vel = rout[i] / a["time"] / 3600 / 24 / 1e5  # a['vel'][i]
             rho = np.log10(a["dens"][i])
             igefrac = a["specfrac"][i, ige_index].sum()
@@ -234,15 +233,15 @@
         abund[:, spectoz[i]] = a["specfrac"][:, i]
 
     for i in range(a["nd"]):
         abund[i, 0] = i + 1
 
     # Write to file abundances.txt
     fmtstring = "%d " + "%1.7e " * 30
-    np.savetxt(model + "/abundances.txt", abund[:, :], fmt=fmtstring)
+    np.savetxt(f"{model}/abundances.txt", abund[:, :], fmt=fmtstring)
 
     # M = 0
     # for i in range(a['nd']):
     #     M += dm[i]
     #     print(i + 1, a['vel'][i], dm[i], M)
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/fromcmfgen/rd_cmfgen.py` & `artistools-2023.8.1/artistools/inputmodel/fromcmfgen/rd_cmfgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
         sumisofrac = np.zeros(nd)
         for iiso in range(len(idx)):
             sumisofrac += isofrac[:, idx[iiso]]
         # compare to corresponding species mass fraction
         absdiff = np.abs(specfrac[:, spec.index(s)] - sumisofrac)
         relabsdiff = absdiff / sumisofrac
         if np.max(relabsdiff) > MAX_POP_DIFF:
-            sys.exit("ERROR - Maximum absolute difference > MAX_POP_DIFF for species {:s}".format(s))
+            sys.exit(f"ERROR - Maximum absolute difference > MAX_POP_DIFF for species {s:s}")
 
     # reversed vectors if reverse=True
     if reverse:
         rad = rad[::-1]
         vel = vel[::-1]
         sigma = sigma[::-1]
         temp = temp[::-1]
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/fullymixed.py` & `artistools-2023.8.1/artistools/inputmodel/fullymixed.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,16 @@
     parser.add_argument("-scalefactor", "-s", default=0.5, help="Kinetic energy scale factor")
     parser.add_argument("-inputpath", "-i", default=".", help="Path of input files")
     parser.add_argument("-outputpath", "-o", default=".", help="Path of output files")
 
 
 def eval_mshell(dfmodel, t_model_init_seconds):
     dfmodel = dfmodel.eval(
-        (
-            "cellmass_grams = 10 ** logrho * 4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
-            "* (1e5 * @t_model_init_seconds) ** 3"
-        ),
+        "cellmass_grams = 10 ** logrho * 4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
+        "* (1e5 * @t_model_init_seconds) ** 3",
     )
 
 
 def main(args=None, argsraw=None, **kwargs) -> None:
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/inputmodel_misc.py` & `artistools-2023.8.1/artistools/inputmodel/inputmodel_misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
+from __future__ import annotations
+
+import argparse
 import errno
 import gc
 import math
 import os.path
 import pickle
 import time
+import typing as t
 from collections import defaultdict
-from collections.abc import Sequence
 from functools import lru_cache
 from pathlib import Path
-from typing import Any
-from typing import Callable
-from typing import Literal
-from typing import Optional
-from typing import Union
 
 import numpy as np
 import pandas as pd
 import polars as pl
 import pyarrow as pa
 import pyarrow.parquet as pq
+from typeguard import typechecked
 
 import artistools as at
 
 
+@typechecked
 def read_modelfile_text(
-    filename: Union[Path, str],
+    filename: Path | str,
     printwarningsonly: bool = False,
     getheadersonly: bool = False,
     skipnuclidemassfraccolumns: bool = False,
-    dtype_backend: Literal["pyarrow", "numpy_nullable"] = "numpy_nullable",
-) -> tuple[pd.DataFrame, dict[str, Any]]:
+    dtype_backend: t.Literal["pyarrow", "numpy_nullable"] = "numpy_nullable",
+) -> tuple[pd.DataFrame, dict[t.Any, t.Any]]:
     """Read an artis model.txt file containing cell velocities, density, and abundances of radioactive nuclides."""
     onelinepercellformat = None
 
-    modelmeta: dict[str, Any] = {"headercommentlines": []}
+    modelmeta: dict[str, t.Any] = {"headercommentlines": []}
 
     modelpath = Path(filename).parent
     if not printwarningsonly:
         print(f"Reading {filename}")
 
     numheaderrows = 0
     with at.zopen(filename) as fmodel:
@@ -152,15 +152,15 @@
                     "X_Ni56",
                     "X_Co56",
                     "X_Fe52",
                     "X_Cr48",
                     "X_Ni57",
                     "X_Co57",
                 ]
-            # last two abundances are optional
+            # last two abundances are Optional
             assert columns is not None
             if ncols_line_even == ncols_line_odd and (ncols_line_even + ncols_line_odd) > len(columns):
                 # one line per cell format
                 ncols_line_odd = 0
 
             assert len(columns) in [
                 ncols_line_even + ncols_line_odd,
@@ -190,27 +190,27 @@
             ncols_line_even = 4
         elif modelmeta["dimensions"] == 3:
             ncols_line_even = 5
         ncols_line_odd = 0
 
     nrows_read = 1 if getheadersonly else modelcellcount
 
-    skiprows: Union[list, int, None]
+    skiprows: list[int] | int | None
 
     skiprows = (
         numheaderrows
         if onelinepercellformat
         else [
             x
             for x in range(numheaderrows + modelcellcount * 2)
             if x < numheaderrows or (x - numheaderrows - 1) % 2 == 0
         ]
     )
 
-    dtypes: defaultdict[str, Union[Callable, str]]
+    dtypes: defaultdict[str, str]
     if dtype_backend == "pyarrow":
         dtypes = defaultdict(lambda: "float32[pyarrow]")
         dtypes["inputcellid"] = "int32[pyarrow]"
         dtypes["tracercount"] = "int32[pyarrow]"
     else:
         dtypes = defaultdict(lambda: "float32")
         dtypes["inputcellid"] = "int32"
@@ -277,15 +277,15 @@
         dfmodel["cellmass_grams"] = dfmodel["rho"] * wid_init**3
 
         dfmodel = dfmodel.rename(columns={"pos_x": "pos_x_min", "pos_y": "pos_y_min", "pos_z": "pos_z_min"})
         if "pos_x_min" in dfmodel.columns and not printwarningsonly:
             print("  model cell positions are defined in the header")
         elif not getheadersonly:
 
-            def vectormatch(vec1, vec2):
+            def vectormatch(vec1: list[float], vec2: list[float]) -> bool:
                 xclose = np.isclose(vec1[0], vec2[0], atol=xmax_tmodel / ncoordgridx)
                 yclose = np.isclose(vec1[1], vec2[1], atol=xmax_tmodel / ncoordgridy)
                 zclose = np.isclose(vec1[2], vec2[2], atol=xmax_tmodel / ncoordgridz)
 
                 return all([xclose, yclose, zclose])
 
             posmatch_xyz = True
@@ -330,24 +330,25 @@
                 )
 
     modelmeta["modelcellcount"] = modelcellcount
 
     return dfmodel, modelmeta
 
 
+@typechecked
 def get_modeldata(
-    modelpath: Union[Path, str] = Path(),
+    modelpath: Path | str = Path(),
     get_elemabundances: bool = False,
-    derived_cols: Optional[Sequence[str]] = None,
+    derived_cols: t.Sequence[str] | None = None,
     printwarningsonly: bool = False,
     getheadersonly: bool = False,
     skipnuclidemassfraccolumns: bool = False,
-    dtype_backend: Literal["pyarrow", "numpy_nullable"] = "numpy_nullable",
+    dtype_backend: t.Literal["pyarrow", "numpy_nullable"] = "numpy_nullable",
     use_polars: bool = False,
-) -> tuple[pd.DataFrame, dict[str, Any]]:
+) -> tuple[pd.DataFrame, dict[t.Any, t.Any]]:
     """Read an artis model.txt file containing cell velocities, densities, and mass fraction abundances of radioactive nuclides.
 
     Parameters
     ----------
         - inputpath: either a path to model.txt file, or a folder containing model.txt
         - get_elemabundances: also read elemental abundances (abundances.txt) and
             merge with the output DataFrame
@@ -455,30 +456,32 @@
         dfmodel = dfmodel.collect().to_pandas(use_pyarrow_extension_array=(dtype_backend == "pyarrow"))
         if modelmeta["npts_model"] > 100000 and not getheadersonly:
             dfmodel.info(verbose=False, memory_usage="deep")
 
     return dfmodel, modelmeta
 
 
-def get_modeldata_tuple(*args, **kwargs) -> tuple[pd.DataFrame, float, float]:
-    """Deprecated but included for compatibility with fixed length tuple return type
-    Use get_modeldata() instead!.
+@typechecked
+def get_modeldata_tuple(*args: t.Any, **kwargs: t.Any) -> tuple[pd.DataFrame, float, float]:
+    """Get model from model.txt file
+    DEPRECATED: Use get_modeldata() instead.
     """
     dfmodel, modelmeta = get_modeldata(*args, **kwargs)
 
     return dfmodel, modelmeta["t_model_init_days"], modelmeta["vmax_cmps"]
 
 
+@typechecked
 def add_derived_cols_to_modeldata(
-    dfmodel: Union[pl.DataFrame, pl.LazyFrame],
-    derived_cols: Sequence[str],
-    dimensions: Optional[int] = None,
-    t_model_init_seconds: Optional[float] = None,
-    wid_init: Optional[float] = None,
-    modelpath: Optional[Path] = None,
+    dfmodel: pl.DataFrame | pl.LazyFrame,
+    derived_cols: t.Sequence[str],
+    dimensions: int | None = None,
+    t_model_init_seconds: float | None = None,
+    wid_init: float | None = None,
+    modelpath: Path | None = None,
 ) -> pl.LazyFrame:
     """Add columns to modeldata using e.g. derived_cols = ('velocity', 'Ye')."""
     if dimensions is None:
         dimensions = get_dfmodel_dimensions(dfmodel)
 
     dfmodel = dfmodel.lazy()
     newcols = []
@@ -540,56 +543,54 @@
 
 
 def get_cell_angle(dfmodel: pd.DataFrame, modelpath: Path) -> pd.DataFrame:
     """Get angle between origin to cell midpoint and the syn_dir axis."""
     syn_dir = at.get_syn_dir(modelpath)
 
     cos_theta = np.zeros(len(dfmodel))
-    i = 0
-    for _, cell in dfmodel.iterrows():
+    for i, (_, cell) in enumerate(dfmodel.iterrows()):
         mid_point = [cell["pos_x_mid"], cell["pos_y_mid"], cell["pos_z_mid"]]
         cos_theta[i] = (np.dot(mid_point, syn_dir)) / (at.vec_len(mid_point) * at.vec_len(syn_dir))
-        i += 1
     dfmodel["cos_theta"] = cos_theta
     cos_bins = [-1, -0.8, -0.6, -0.4, -0.2, 0, 0.2, 0.4, 0.6, 0.8, 1]  # including end bin
     labels = [0, 10, 20, 30, 40, 50, 60, 70, 80, 90]  # to agree with escaping packet bin numbers
     assert at.get_viewingdirection_costhetabincount() == 10
     assert at.get_viewingdirection_phibincount() == 10
     dfmodel["cos_bin"] = pd.cut(dfmodel["cos_theta"], cos_bins, labels=labels)
     # dfmodel['cos_bin'] = np.searchsorted(cos_bins, dfmodel['cos_theta'].values) -1
 
     return dfmodel
 
 
 def get_mean_cell_properties_of_angle_bin(
-    dfmodeldata: pd.DataFrame, vmax_cmps: float, modelpath=None
+    dfmodeldata: pd.DataFrame, vmax_cmps: float, modelpath: Path
 ) -> dict[int, pd.DataFrame]:
     if "cos_bin" not in dfmodeldata:
         get_cell_angle(dfmodeldata, modelpath)
 
     dfmodeldata["rho"][dfmodeldata["rho"] == 0] = None
 
     cell_velocities = np.unique(dfmodeldata["vel_x_min"].values)
     cell_velocities = cell_velocities[cell_velocities >= 0]
     velocity_bins = np.append(cell_velocities, vmax_cmps)
 
     mid_velocities = np.unique(dfmodeldata["vel_x_mid"].values)
     mid_velocities = mid_velocities[mid_velocities >= 0]
 
-    mean_bin_properties = {}
-    for bin_number in range(10):
-        mean_bin_properties[bin_number] = pd.DataFrame(
+    mean_bin_properties = {
+        bin_number: pd.DataFrame(
             {
                 "velocity": mid_velocities,
                 "mean_rho": np.zeros_like(mid_velocities, dtype=float),
                 "mean_Ye": np.zeros_like(mid_velocities, dtype=float),
                 "mean_Q": np.zeros_like(mid_velocities, dtype=float),
             }
         )
-
+        for bin_number in range(10)
+    }
     # cos_bin_number = 90
     for bin_number in range(10):
         cos_bin_number = bin_number * 10
         # get cells with bin number
         dfanglebin = dfmodeldata.query("cos_bin == @cos_bin_number", inplace=False)
 
         binned = pd.cut(dfanglebin["vel_r_mid"], velocity_bins, labels=False, include_lowest=True)
@@ -606,17 +607,17 @@
             for binindex, mean_Q in dfanglebin.groupby(binned)["Q"].mean().iteritems():
                 i += 1
                 mean_bin_properties[bin_number]["mean_Q"][binindex] += mean_Q
 
     return mean_bin_properties
 
 
-def get_2d_modeldata(modelpath):
-    filepath = os.path.join(modelpath, "model.txt")
-    with open(filepath) as f:
+def get_2d_modeldata(modelpath: str | Path) -> pd.DataFrame:
+    filepath = Path(modelpath, "model.txt")
+    with filepath.open() as f:
         num_lines = sum(1 for _ in f)
     skiprowlist = [0, 1, 2]
     skiprowlistodds = skiprowlist + [i for i in range(3, num_lines) if i % 2 == 1]
     skiprowlistevens = skiprowlist + [i for i in range(3, num_lines) if i % 2 == 0]
 
     model1stlines = pd.read_csv(filepath, delim_whitespace=True, header=None, skiprows=skiprowlistevens)
     model2ndlines = pd.read_csv(filepath, delim_whitespace=True, header=None, skiprows=skiprowlistodds)
@@ -633,22 +634,22 @@
         "X_Fe52",
         "X_Cr48",
     ]
     model.columns = column_names
     return model
 
 
-def get_3d_model_data_merged_model_and_abundances_minimal(args):
+def get_3d_model_data_merged_model_and_abundances_minimal(args: argparse.Namespace) -> pd.DataFrame:
     """Get 3D data without generating all the extra columns in standard routine.
     Needed for large (eg. 200^3) models.
     """
     model = get_3d_modeldata_minimal(args.modelpath)
     abundances = get_initelemabundances(args.modelpath[0])
 
-    with open(os.path.join(args.modelpath[0], "model.txt")) as fmodelin:
+    with Path(args.modelpath[0], "model.txt").open() as fmodelin:
         fmodelin.readline()  # npts_model3d
         args.t_model = float(fmodelin.readline())  # days
         args.vmax = float(fmodelin.readline())  # v_max in [cm/s]
 
     print(model.keys())
 
     merge_dfs = model.merge(abundances, how="inner", on="inputcellid")
@@ -658,21 +659,19 @@
     gc.collect()
 
     merge_dfs.info(verbose=False, memory_usage="deep")
 
     return merge_dfs
 
 
-def get_3d_modeldata_minimal(modelpath) -> pd.DataFrame:
+def get_3d_modeldata_minimal(modelpath: str | Path) -> pd.DataFrame:
     """Read 3D model without generating all the extra columns in standard routine.
     Needed for large (eg. 200^3) models.
     """
-    model = pd.read_csv(
-        os.path.join(modelpath[0], "model.txt"), delim_whitespace=True, header=None, skiprows=3, dtype=np.float64
-    )
+    model = pd.read_csv(Path(modelpath, "model.txt"), delim_whitespace=True, header=None, skiprows=3, dtype=np.float64)
     columns = [
         "inputcellid",
         "cellpos_in[z]",
         "cellpos_in[y]",
         "cellpos_in[x]",
         "rho_model",
         "X_Fegroup",
@@ -685,23 +684,24 @@
     model.columns = columns
 
     print("model.txt memory usage:")
     model.info(verbose=False, memory_usage="deep")
     return model
 
 
+@typechecked
 def save_modeldata(
     dfmodel: pd.DataFrame,
-    t_model_init_days: Optional[float] = None,
-    filename: Union[Path, str, None] = None,
-    modelpath: Union[Path, str, None] = None,
-    vmax: Optional[float] = None,
-    dimensions: Optional[int] = None,
-    headercommentlines: Optional[list[str]] = None,
-    modelmeta: Optional[dict[str, Any]] = None,
+    t_model_init_days: float | None = None,
+    filename: Path | str | None = None,
+    modelpath: Path | str | None = None,
+    vmax: float | None = None,
+    dimensions: int | None = None,
+    headercommentlines: list[str] | None = None,
+    modelmeta: dict[str, t.Any] | None = None,
     twolinespercell: bool = False,
     float_format: str = ".4e",
 ) -> None:
     """Save a pandas DataFrame and snapshot time into ARTIS model.txt."""
     if modelmeta:
         if "headercommentlines" in modelmeta:
             assert headercommentlines is None
@@ -744,15 +744,15 @@
             "X_Fegroup",
             "X_Ni56",
             "X_Co56",
             "X_Fe52",
             "X_Cr48",
         ]
 
-    # these two columns are optional, but position is important and they must appear before any other custom cols
+    # these two columns are Optional, but position is important and they must appear before t.Any other custom cols
     if "X_Ni57" in dfmodel.columns:
         standardcols.append("X_Ni57")
 
     if "X_Co57" in dfmodel.columns:
         standardcols.append("X_Co57")
 
     # set missing radioabundance columns to zero
@@ -767,15 +767,15 @@
     )  # sort columns by atomic number, mass number
 
     assert modelpath is not None or filename is not None
     if filename is None:
         filename = "model.txt"
     modelfilepath = Path(modelpath, filename) if modelpath is not None else Path(filename)
 
-    with open(modelfilepath, "w", encoding="utf-8") as fmodel:
+    with modelfilepath.open("w", encoding="utf-8") as fmodel:
         if headercommentlines is not None:
             fmodel.write("\n".join([f"# {line}" for line in headercommentlines]) + "\n")
         fmodel.write(f"{len(dfmodel)}\n")
         fmodel.write(f"{t_model_init_days}\n")
         if dimensions == 3:
             fmodel.write(f"{vmax}\n")
 
@@ -813,29 +813,29 @@
                     else zeroabund
                 )
                 fmodel.write("\n")
 
     print(f"Saved {modelfilepath} (took {time.perf_counter() - timestart:.1f} seconds)")
 
 
-def get_mgi_of_velocity_kms(modelpath: Path, velocity: float, mgilist=None) -> Union[int, float]:
+def get_mgi_of_velocity_kms(modelpath: Path, velocity: float, mgilist: t.Sequence[int] | None = None) -> int | float:
     """Return the modelgridindex of the cell whose outer velocity is closest to velocity.
     If mgilist is given, then chose from these cells only.
     """
     modeldata, _, _ = get_modeldata_tuple(modelpath)
 
     velocity = float(velocity)
 
     if not mgilist:
         mgilist = list(modeldata.index)
         arr_vouter = modeldata["velocity_outer"].to_numpy()
     else:
         arr_vouter = np.array([modeldata["velocity_outer"][mgi] for mgi in mgilist])
 
-    index_closestvouter = np.abs(arr_vouter - velocity).argmin()
+    index_closestvouter = int(np.abs(arr_vouter - velocity).argmin())
 
     if velocity < arr_vouter[index_closestvouter] or index_closestvouter + 1 >= len(mgilist):
         return mgilist[index_closestvouter]
     if velocity < arr_vouter[index_closestvouter + 1]:
         return mgilist[index_closestvouter + 1]
     if np.isnan(velocity):
         return float("nan")
@@ -844,15 +844,15 @@
     raise AssertionError
 
 
 @lru_cache(maxsize=8)
 def get_initelemabundances(
     modelpath: Path = Path(),
     printwarningsonly: bool = False,
-    dtype_backend: Literal["pyarrow", "numpy_nullable"] = "numpy_nullable",
+    dtype_backend: t.Literal["pyarrow", "numpy_nullable"] = "numpy_nullable",
 ) -> pd.DataFrame:
     """Return a table of elemental mass fractions by cell from abundances."""
     abundancefilepath = at.firstexisting("abundances.txt", folder=modelpath, tryzipped=True)
 
     filenameparquet = at.stripallsuffixes(Path(abundancefilepath)).with_suffix(".txt.parquet")
     if filenameparquet.exists() and Path(abundancefilepath).stat().st_mtime > filenameparquet.stat().st_mtime:
         print(f"{abundancefilepath} has been modified after {filenameparquet}. Deleting out of date parquet file.")
@@ -894,18 +894,19 @@
     abundancedata.index.name = "modelgridindex"
     if dtype_backend == "pyarrow":
         abundancedata.index = abundancedata.index.astype("int32[pyarrow]")
 
     return abundancedata
 
 
+@typechecked
 def save_initelemabundances(
     dfelabundances: pd.DataFrame,
-    abundancefilename: Union[Path, str],
-    headercommentlines: Optional[Sequence[str]] = None,
+    abundancefilename: Path | str,
+    headercommentlines: t.Sequence[str] | None = None,
 ) -> None:
     """Save a DataFrame (same format as get_initelemabundances) to abundances.txt.
     columns must be:
         - inputcellid: integer index to match model.txt (starting from 1)
         - X_El: mass fraction of element with two-letter code 'El' (e.g., X_H, X_He, H_Li, ...).
     """
     timestart = time.perf_counter()
@@ -918,59 +919,56 @@
     elcolnames = [f"X_{at.get_elsymbol(Z)}" for Z in range(1, 1 + max(atomic_numbers))]
 
     # set missing elemental abundance columns to zero
     for col in elcolnames:
         if col not in dfelabundances.columns:
             dfelabundances[col] = 0.0
 
-    with open(abundancefilename, "w", encoding="utf-8") as fabund:
+    with Path(abundancefilename).open("w", encoding="utf-8") as fabund:
         if headercommentlines is not None:
             fabund.write("\n".join([f"# {line}" for line in headercommentlines]) + "\n")
         for row in dfelabundances.itertuples(index=False):
             fabund.write(f" {row.inputcellid:6d} ")
             fabund.write(" ".join([f"{getattr(row, colname, 0.):.6e}" for colname in elcolnames]))
             fabund.write("\n")
 
     print(f"Saved {abundancefilename} (took {time.perf_counter() - timestart:.1f} seconds)")
 
 
-def save_empty_abundance_file(ngrid: int, outputfilepath=Path()) -> None:
-    """Dummy abundance file with only zeros."""
+def save_empty_abundance_file(ngrid: int, outputfilepath: str | Path = Path()) -> None:
+    """Save dummy abundance file with only zeros."""
     if Path(outputfilepath).is_dir():
         outputfilepath = Path(outputfilepath) / "abundances.txt"
 
     Z_atomic = np.arange(1, 31)
 
-    abundancedata: dict[str, Any] = {"cellid": range(1, ngrid + 1)}
+    abundancedata: dict[str, t.Any] = {"cellid": range(1, ngrid + 1)}
     for atomic_number in Z_atomic:
         abundancedata[f"Z={atomic_number}"] = np.zeros(ngrid)
 
     # abundancedata['Z=28'] = np.ones(ngrid)
 
     dfabundances = pd.DataFrame(data=abundancedata).round(decimals=5)
     dfabundances.to_csv(outputfilepath, header=False, sep=" ", index=False)
 
 
-def get_dfmodel_dimensions(dfmodel: Union[pd.DataFrame, pl.DataFrame, pl.LazyFrame]) -> int:
+def get_dfmodel_dimensions(dfmodel: pd.DataFrame | pl.DataFrame | pl.LazyFrame) -> int:
     if "pos_x_min" in dfmodel.columns:
         return 3
 
-    if "pos_z_mid" in dfmodel.columns:
-        return 2
-
-    return 1
+    return 2 if "pos_z_mid" in dfmodel.columns else 1
 
 
 def sphericalaverage(
     dfmodel: pd.DataFrame,
     t_model_init_days: float,
     vmax: float,
-    dfelabundances: Optional[pd.DataFrame] = None,
-    dfgridcontributions: Optional[pd.DataFrame] = None,
-    nradialbins: Optional[int] = None,
+    dfelabundances: pd.DataFrame | None = None,
+    dfgridcontributions: pd.DataFrame | None = None,
+    nradialbins: int | None = None,
 ) -> tuple[pd.DataFrame, pd.DataFrame, pd.DataFrame]:
     """Convert 3D Cartesian grid model to 1D spherical."""
     t_model_init_seconds = t_model_init_days * 24 * 60 * 60
     xmax = vmax * t_model_init_seconds
     ngridpoints = len(dfmodel)
     ncoordgridx = round(ngridpoints ** (1.0 / 3.0))
     wid_init = 2 * xmax / ncoordgridx
@@ -1019,35 +1017,31 @@
 
             if rhomean > 0.0 and dfgridcontributions is not None:
                 dfcellcont = dfgridcontributions.query("cellindex in @matchedcells.inputcellid.to_numpy()")
 
                 for particleid, dfparticlecontribs in dfcellcont.groupby("particleid"):
                     frac_of_cellmass_avg = (
                         sum(
-                            [
-                                (row.frac_of_cellmass * celldensity[row.cellindex])
-                                for row in dfparticlecontribs.itertuples(index=False)
-                            ]
+                            row.frac_of_cellmass * celldensity[row.cellindex]
+                            for row in dfparticlecontribs.itertuples(index=False)
                         )
                         / matchedcellrhosum
                     )
 
                     contriboutrow = {
                         "particleid": particleid,
                         "cellindex": radialcellid,
                         "frac_of_cellmass": frac_of_cellmass_avg,
                     }
 
                     if includemissingcolexists:
                         frac_of_cellmass_includemissing_avg = (
                             sum(
-                                [
-                                    (row.frac_of_cellmass_includemissing * celldensity[row.cellindex])
-                                    for row in dfparticlecontribs.itertuples(index=False)
-                                ]
+                                row.frac_of_cellmass_includemissing * celldensity[row.cellindex]
+                                for row in dfparticlecontribs.itertuples(index=False)
                             )
                             / matchedcellrhosum
                         )
                         contriboutrow["frac_of_cellmass_includemissing"] = frac_of_cellmass_includemissing_avg
 
                     outgridcontributions.append(contriboutrow)
 
@@ -1091,17 +1085,17 @@
 
     return dfmodel1d, dfabundances1d, dfgridcontributions1d
 
 
 def scale_model_to_time(
     dfmodel: pd.DataFrame,
     targetmodeltime_days: float,
-    t_model_days: Optional[float] = None,
-    modelmeta: Optional[dict[str, Any]] = None,
-) -> tuple[pd.DataFrame, Optional[dict[str, Any]]]:
+    t_model_days: float | None = None,
+    modelmeta: dict[str, t.Any] | None = None,
+) -> tuple[pd.DataFrame, dict[str, t.Any] | None]:
     """Homologously expand model to targetmodeltime_days, reducing density and adjusting position columns to match."""
     if t_model_days is None:
         assert modelmeta is not None
         t_model_days = modelmeta["t_model_days"]
 
     timefactor = targetmodeltime_days / t_model_days
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/lapuente.py` & `artistools-2023.8.1/artistools/inputmodel/lapuente.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/makeartismodel.py` & `artistools-2023.8.1/artistools/inputmodel/makeartismodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
 
     if not args.modelpath:
-        args.modelpath = [Path(".")]
-    elif isinstance(args.modelpath, (str, Path)):
+        args.modelpath = [Path()]
+    elif isinstance(args.modelpath, str | Path):
         args.modelpath = [args.modelpath]
 
     args.modelpath = at.flatten_list(args.modelpath)
 
     if args.downscale3dgrid:
         at.inputmodel.downscale3dgrid.make_downscaled_3d_grid(
             modelpath=Path(args.modelpath[0]), outputgridsize=args.outputgridsize
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/maketardismodelfromartis.py` & `artistools-2023.8.1/artistools/inputmodel/maketardismodelfromartis.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,25 +81,25 @@
                 {"name": "density", "unit": "g/cm^3", "desc": "density of shell"},
                 {"name": "t_rad", "unit": "K", "desc": "radiative temperature"},
                 {"name": "dilution_factor", "desc": "dilution factor of shell"},
                 *[{"name": strnuc, "desc": f"fractional {strnuc} abundance"} for strnuc in listspecies],
             ]
         },
     }
-    with open(outputfilepath, "w") as fileout:
+    with outputfilepath.open("w") as fileout:
         fileout.write("---\n")
         yamldump(dictmeta, fileout, sort_keys=False)
         fileout.write("---\n")
         fileout.write(",".join(["velocity", "density", "t_rad", "dilution_factor", *listspecies]))
         fileout.write("\n")
 
         # fileout.write(f'{0.},{0.:.4e},{0.},{0.},{",".join([f"{0.:.4e}" for _ in listspecies])}\n')
 
         for cell in dfmodel.itertuples(index=False):
-            abundlist = [f'{getattr(cell, "X_" + strnuc):.4e}' for strnuc in listspecies]
+            abundlist = [f'{getattr(cell, f"X_{strnuc}"):.4e}' for strnuc in listspecies]
             fileout.write(
                 f'{cell.velocity_outer},{cell.rho:.4e},{temperature},{dilution_factor},{",".join(abundlist)}\n'
             )
 
     print(f"Saved {outputfilepath}")
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/map_1d_to_3d_grid.py` & `artistools-2023.8.1/artistools/inputmodel/map_1d_to_3d_grid.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/maptogrid.py` & `artistools-2023.8.1/artistools/inputmodel/maptogrid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
 # adapted from Fortran maptogrid.f90 and kernelmodule.f90
 # original Fortran code by Andreas Bauswein
+from __future__ import annotations
+
 import argparse
 import math
 from pathlib import Path
-from typing import Union
 
 import argcomplete
 import numpy as np
 import pandas as pd
 
 import artistools as at
 
@@ -69,39 +70,38 @@
             vsum = 0.25 * dif2 * dif2 * dif2
             wij[i] = cnormk * vsum
 
     return wij
 
 
 def kernelvals2(rij2: float, hmean: float, wij: np.ndarray) -> float:  # ist schnell berechnet aber keine Gradienten
-    hmean21 = 1.0 / (hmean * hmean)
+    hmean21 = 1.0 / hmean**2
     hmean31 = hmean21 / hmean
     v2 = rij2 * hmean21
     index = math.floor(v2 / dvtable)
     dxx = v2 - index * dvtable
     index1 = index + 1
     dwdx = (wij[index1] - wij[index]) / dvtable
-    wtij = (wij[index] + dwdx * dxx) * hmean31
-    return wtij
+    return (wij[index] + dwdx * dxx) * hmean31
 
 
 def maptogrid(
-    ejectasnapshotpath: Path, outputfolderpath: Union[Path, str], ncoordgrid: int = 50, downsamplefactor: int = 1
+    ejectasnapshotpath: Path, outputfolderpath: Path | str, ncoordgrid: int = 50, downsamplefactor: int = 1
 ) -> None:
     if not ejectasnapshotpath.is_file():
         print(f"{ejectasnapshotpath} not found")
         return
 
     # save the printed output to a log file
     logfilepath = Path("maptogridlog.txt")
     logfilepath.unlink(missing_ok=True)
 
     def logprint(*args, **kwargs):
         print(*args, **kwargs)
-        with open(logfilepath, "at", encoding="utf-8") as logfile:
+        with logfilepath.open("a", encoding="utf-8") as logfile:
             logfile.write(" ".join([str(x) for x in args]) + "\n")
 
     wij = get_wij()
 
     assert ncoordgrid % 2 == 0
 
     snapshot_columns = [
@@ -178,15 +178,15 @@
     vy = dfsnapshot["vy"].to_numpy()
     vz = dfsnapshot["vz"].to_numpy()
     pmass = dfsnapshot["pmass"].to_numpy()
     rho_rst = dfsnapshot["rho_rst"].to_numpy()
     rho = dfsnapshot["rho"].to_numpy()
     Ye = dfsnapshot["ye"].to_numpy()
 
-    with open(Path(outputfolderpath, "ejectapartanalysis.dat"), mode="w", encoding="utf-8") as fpartanalysis:
+    with Path(outputfolderpath, "ejectapartanalysis.dat").open(mode="w", encoding="utf-8") as fpartanalysis:
         for n in range(npart):
             totmass = totmass + pmass[n]
 
             dis = math.sqrt(x[n] ** 2 + y[n] ** 2 + z[n] ** 2)  # original dis
 
             x[n] += vx[n] * dtextra
             y[n] += vy[n] * dtextra
@@ -346,15 +346,15 @@
         if min(loc_i, loc_j, loc_k) < 0 or max(loc_i, loc_j, loc_k) > ncoordgrid - 1:
             continue
         logprint(f"particle {n} is totally unused but located in cell {loc_i} {loc_j} {loc_k}")
 
     with np.errstate(divide="ignore", invalid="ignore"):
         gye = np.divide(gye, grho)
 
-        with open(Path(outputfolderpath, "gridcontributions.txt"), "w", encoding="utf-8") as fcontribs:
+        with Path(outputfolderpath, "gridcontributions.txt").open("w", encoding="utf-8") as fcontribs:
             fcontribs.write("particleid cellindex frac_of_cellmass\n")
             for (n, i, j, k), rho_contrib in particle_rho_contribs.items():
                 gridindex = (k * ncoordgrid + j) * ncoordgrid + i + 1
                 fcontribs.write(f"{particleid[n]} {gridindex} {rho_contrib / grho[i, j, k]}\n")
         logprint("saved gridcontributions.txt")
 
     # check some stuff on the grid
@@ -395,15 +395,15 @@
         f" {(nzerocentral) / (4.0 * 3.14 / 3.0 * rmean**3 / (dx * dy * dz))}"
     )
 
     logprint("probably we want to choose grid size, i.e. x0, as compromise between mapped mass and rho=0 cells")
 
     # output grid - adapt as you need output
 
-    with open(Path(outputfolderpath, "grid.dat"), "w", encoding="utf-8") as fgrid:
+    with Path(outputfolderpath, "grid.dat").open("w", encoding="utf-8") as fgrid:
         fgrid.write(f"{ncoordgrid**3} # ncoordgrid\n")
         fgrid.write(f"{dtextra} # extra time after explosion simulation ended (in geom units)\n")
         fgrid.write(f"{x0} # xmax\n")
         fgrid.write(" gridindex    pos_x_min    pos_y_min    pos_z_min    rho    cellYe    tracercount\n")
         gridindex = 1
         for k in range(ncoordgrid):
             gz = z0 + dz * k
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/modelfromhydro.py` & `artistools-2023.8.1/artistools/inputmodel/modelfromhydro.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
+from __future__ import annotations
+
 import argparse
 import datetime
 import math
 import sys
 from pathlib import Path
 
 import argcomplete
@@ -49,28 +51,24 @@
         "enuxtrap(i)",
         "iwasequil(i, 1)",
         "iwasequil(i, 2)",
         "iwasequil(i, 3)",
     ]
 
     types_dict = {"id": int}
-    types_dict.update({col: float for col in column_names if col not in types_dict})
+    types_dict |= {col: float for col in column_names if col not in types_dict}
 
-    ejectasnapshot = pd.read_csv(
+    return pd.read_csv(
         Path(pathtosnapshot) / "ejectasnapshot.dat",
         delim_whitespace=True,
         header=None,
         names=column_names,
         dtype=types_dict,
     )
 
-    # Everything is in geometric units here
-
-    return ejectasnapshot
-
 
 def get_merger_time_geomunits(pathtogriddata: Path) -> float:
     mergertimefile = pathtogriddata / "tmerger.txt"
     if mergertimefile.exists():
         with mergertimefile.open("rt") as fmergertimefile:
             comments = fmergertimefile.readline()
             assert comments.startswith("#")
@@ -78,18 +76,17 @@
             print(f"Found simulation merger time to be {mergertime_geomunits} ({mergertime_geomunits * 4.926e-6} s) ")
         return mergertime_geomunits
 
     print('Make file "tmerger.txt" with time of merger in geom units')
     sys.exit(1)
 
 
-def get_snapshot_time_geomunits(pathtogriddata: Path) -> tuple[float, float]:
-    import glob
-
-    snapshotinfofiles = glob.glob(str(Path(pathtogriddata) / "*_info.dat*"))
+def get_snapshot_time_geomunits(pathtogriddata: Path | str) -> tuple[float, float]:
+    pathtogriddata = Path(pathtogriddata)
+    snapshotinfofiles = list(pathtogriddata.glob("*_info.dat*"))
     if not snapshotinfofiles:
         print("No info file found for dumpstep")
         sys.exit(1)
 
     if len(snapshotinfofiles) > 1:
         print("Too many sfho_info.dat files found")
         sys.exit(1)
@@ -100,15 +97,15 @@
             line1 = fsnapshotinfo.readline()
             simulation_end_time_geomunits = float(line1.split()[2])
             print(
                 f"Found simulation snapshot time to be {simulation_end_time_geomunits} "
                 f"({simulation_end_time_geomunits * 4.926e-6} s)"
             )
 
-        mergertime_geomunits = get_merger_time_geomunits(Path(pathtogriddata))
+        mergertime_geomunits = get_merger_time_geomunits(pathtogriddata)
         print(f"  time since merger {(simulation_end_time_geomunits - mergertime_geomunits) * 4.926e-6} s")
 
     else:
         print("Could not find snapshot info file to get simulation time")
         sys.exit(1)
 
     return simulation_end_time_geomunits, mergertime_geomunits
@@ -141,15 +138,15 @@
     km_to_cm = 1e5
     griddata["pos_x_min"] = griddata["pos_x_min"] * factor_position * km_to_cm
     griddata["pos_y_min"] = griddata["pos_y_min"] * factor_position * km_to_cm
     griddata["pos_z_min"] = griddata["pos_z_min"] * factor_position * km_to_cm
 
     griddata["rho"] = griddata["rho"] * 6.176e17  # convert to g/cm3
 
-    with open(griddatfilepath, encoding="utf-8") as gridfile:
+    with griddatfilepath.open(encoding="utf-8") as gridfile:
         ngrid = int(gridfile.readline().split()[0])
         if ngrid != len(griddata["inputcellid"]):
             print("length of file and ngrid don't match")
             sys.exit(1)
         extratime_geomunits = float(gridfile.readline().split()[0])
         xmax = abs(float(gridfile.readline().split()[0]))
         xmax = (xmax * factor_position) * (u.km).to(u.cm)
@@ -196,20 +193,20 @@
 
 
 def read_mattia_grid_data_file(pathtogriddata):
     # griddatfilepath = Path(pathtogriddata) / "q90_m0.01_v0.1.txt"
     griddatfilepath = Path(pathtogriddata) / "1D_m0.01_v0.1.txt"
 
     griddata = pd.read_csv(griddatfilepath, delim_whitespace=True, comment="#", skiprows=1)
-    with open(griddatfilepath) as gridfile:
+    with griddatfilepath.open() as gridfile:
         t_model = float(gridfile.readline())
         print(f"t_model {t_model} seconds")
     xmax = max(griddata["posx"])
     vmax = xmax / t_model  # cm/s
-    t_model = t_model / (24.0 * 3600)  # days
+    t_model /= 24.0 * 3600
     ngrid = len(griddata["posx"])
 
     griddata["rho"][griddata["rho"] <= 1e-50] = 0.0
     inputcellid = np.arange(1, ngrid + 1)
     griddata["inputcellid"] = inputcellid
 
     return griddata, t_model, vmax
@@ -220,27 +217,27 @@
 
     rho = np.zeros((grid, grid, grid))
     cellYe = np.zeros((grid, grid, grid))
     tracercount = np.zeros((grid, grid, grid))
     Q = np.zeros((grid, grid, grid))
 
     i = 0
-    for z in range(0, grid):
-        for y in range(0, grid):
-            for x in range(0, grid):
+    for z in range(grid):
+        for y in range(grid):
+            for x in range(grid):
                 rho[x, y, z] = griddata["rho"][i]
                 cellYe[x, y, z] = griddata["cellYe"][i]
                 tracercount[x, y, z] = griddata["tracercount"][i]
                 Q[x, y, z] = griddata["Q"][i]
                 i += 1
 
-    for z in range(0, grid):
+    for z in range(grid):
         z_mirror = grid - 1 - z
-        for y in range(0, grid):
-            for x in range(0, grid):
+        for y in range(grid):
+            for x in range(grid):
                 if z < 50:
                     rho[x, y, z] = rho[x, y, z]
                     cellYe[x, y, z] = cellYe[x, y, z]
                     tracercount[x, y, z] = tracercount[x, y, z]
                     Q[x, y, z] = Q[x, y, z]
                 if z >= 50:
                     rho[x, y, z] = rho[x, y, z_mirror]
@@ -249,17 +246,17 @@
                     Q[x, y, z] = Q[x, y, z_mirror]
 
     rho_1d_array = np.zeros(len(griddata))
     cellYe_1d_array = np.zeros(len(griddata))
     tracercount_1d_array = np.zeros(len(griddata))
     Q_1d_array = np.zeros(len(griddata))
     i = 0
-    for z in range(0, grid):
-        for y in range(0, grid):
-            for x in range(0, grid):
+    for z in range(grid):
+        for y in range(grid):
+            for x in range(grid):
                 rho_1d_array[i] = rho[x, y, z]
                 cellYe_1d_array[i] = cellYe[x, y, z]
                 tracercount_1d_array[i] = tracercount[x, y, z]
                 Q_1d_array[i] = Q[x, y, z]
                 i += 1
 
     griddata["rho"] = rho_1d_array
@@ -298,16 +295,15 @@
         ) < 0.1:
             # if griddata['rho'][i] == 0:
             print("Inner empty cells")
             print(
                 cellid, griddata["pos_x_min"][i], griddata["pos_y_min"][i], griddata["pos_z_min"][i], griddata["rho"][i]
             )
             griddata["rho"][i] += density_hole
-            if griddata["cellYe"][i] < 0.4:
-                griddata["cellYe"][i] = 0.4
+            griddata["cellYe"][i] = max(griddata["cellYe"][i], 0.4)
             # print("Inner empty cells filled")
             print(
                 cellid, griddata["pos_x_min"][i], griddata["pos_y_min"][i], griddata["pos_z_min"][i], griddata["rho"][i]
             )
 
     return griddata
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/opacityinputfile.py` & `artistools-2023.8.1/artistools/inputmodel/opacityinputfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import pandas as pd
 
 
 def all_cells_same_opacity(modelpath, ngrid):
     cell_opacities = np.array([0.1] * ngrid)
 
-    with open(Path(modelpath) / "opacity.txt", "w") as fopacity:
+    with Path(modelpath, "opacity.txt").open("w") as fopacity:
         fopacity.write(f"{ngrid}\n")
 
         for cellid, opacity in enumerate(cell_opacities):
             fopacity.write(f"{cellid+1}    {opacity}\n")
 
 
 def opacity_by_Ye(outputfilepath, griddata):
@@ -37,25 +37,23 @@
         elif Ye <= 0.35:
             cell_opacities[index] = 3.3
         else:
             cell_opacities[index] = 0.96
 
     griddata["opacity"] = cell_opacities
 
-    with open(Path(outputfilepath) / "opacity.txt", "w") as fopacity:
+    with Path(outputfilepath, "opacity.txt").open("w") as fopacity:
         fopacity.write(f'{len(griddata["inputcellid"])}\n')
         griddata[["inputcellid", "opacity"]].to_csv(fopacity, sep="\t", index=False, header=False, float_format="%.10f")
 
 
 def get_opacity_from_file(modelpath):
     opacity_file_contents = np.loadtxt(Path(modelpath) / "opacity.txt", unpack=True, skiprows=1)
-    opacity = opacity_file_contents[1]
-
-    return opacity
+    return opacity_file_contents[1]
 
 
 def write_Ye_file(outputfilepath, griddata):
-    with open(Path(outputfilepath) / "Ye.txt", "w") as fYe:
+    with Path(outputfilepath, "Ye.txt").open("w") as fYe:
         fYe.write(f'{len(griddata["inputcellid"])}\n')
         griddata[["inputcellid", "cellYe"]].to_csv(fYe, sep="\t", index=False, header=False, float_format="%.10f")
 
     print("Saved Ye.txt")
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/plotdensity.py` & `artistools-2023.8.1/artistools/inputmodel/plotdensity.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,30 +46,27 @@
         args.modelpath = ["."]
 
     for modelpath in args.modelpath:
         dfmodel, _, _ = at.get_modeldata_tuple(modelpath)
         label = at.get_model_name(modelpath)
         enclosed_xvals = []
         enclosed_yvals = []
-        binned_xvals = []
-        binned_yvals = []
+        binned_xvals: list[float] = []
+        binned_yvals: list[float] = []
         mass_cumulative = 0.0
         enclosed_xvals = [0.0]
         enclosed_yvals = [0.0]
 
         # total_mass = dfmodel.cellmass_grams.sum() / 1.989e33
         for cell in dfmodel.itertuples(index=False):
-            binned_xvals.append(cell.velocity_inner / 299792.458)
-            binned_xvals.append(cell.velocity_outer / 299792.458)
+            binned_xvals.extend((cell.velocity_inner / 299792.458, cell.velocity_outer / 299792.458))
             delta_beta = (cell.velocity_outer - cell.velocity_inner) / 299792.458
 
             yval = cell.cellmass_grams / 1.989e33 / delta_beta
-            binned_yvals.append(yval)
-            binned_yvals.append(yval)
-
+            binned_yvals.extend((yval, yval))
             enclosed_xvals.append(cell.velocity_outer / 299792.458)
             mass_cumulative += cell.cellmass_grams / 1.989e33
             enclosed_yvals.append(mass_cumulative)
 
         axes[0].plot(binned_xvals, binned_yvals, label=label)
         axes[1].plot(enclosed_xvals, enclosed_yvals, label=label)
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/recombinationenergy.py` & `artistools-2023.8.1/artistools/inputmodel/recombinationenergy.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,17 +52,14 @@
                 model_el_binding_en_ev[elsymb] = model_el_binding_en_ev.get(elsymb, 0.0) + contrib_binding_en_ev
                 mass_msun_accounted += species_mass_msun
                 model_tot_binding_en_ev += contrib_binding_en_ev
 
             elif species.lower() != "fegroup":  # ignore special group abundance
                 pass
 
-            else:
-                pass
-
     def sortkey(item):
         return at.get_atomic_number(item[0])
 
     for elsymb, binding_en_ev in sorted(model_el_binding_en_ev.items(), key=sortkey):
         zstr = f"Z={atomic_number}"
         print(f"{zstr:>5} {binding_en_ev * ev_erg} erg")
 
@@ -105,17 +102,16 @@
     with at.inputmodel.rprocess_from_trajectory.open_tar_file_or_extracted(
         traj_root=traj_root, particleid=particleid, memberfilename=memberfilename
     ) as fthermo:
         dfthermo = pd.read_csv(fthermo, delim_whitespace=True, usecols=["#count", "time/s", "Qdot", "Ye"])
         dfthermo = dfthermo.rename(columns={"time/s": "time_s"})
         dfthermo = dfthermo.query("time_s >= @tmin_s")
         dfthermo = dfthermo.query("time_s <= @time_s_end")
-        en_released_ev_per_gram = np.trapz(y=dfthermo["Qdot"], x=dfthermo["time_s"]) * erg_to_ev
+        return np.trapz(y=dfthermo["Qdot"], x=dfthermo["time_s"]) * erg_to_ev
         # print(dfthermo)
-    return en_released_ev_per_gram
 
 
 def get_particles_recomb_nuc_energy(traj_root, dfbinding):
     dfsnapshot = at.inputmodel.modelfromhydro.read_ejectasnapshot(
         "/Users/luke/Library/Mobile Documents/com~apple~CloudDocs/Archive/Astronomy/Mergers/SFHo_snapshot"
     )
     dfsnapshot = dfsnapshot.sort_values("ye")
@@ -202,15 +198,15 @@
         )
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
 
-    with open(at.get_config()["path_datadir"] / "ElBiEn_2007.txt") as fbinding:
+    with Path(at.get_config()["path_datadir"], "ElBiEn_2007.txt").open() as fbinding:
         for _ in range(11):
             header = fbinding.readline().lstrip(" #").split()
         # print(header)
         dfbinding = pd.read_csv(fbinding, delim_whitespace=True, names=header)
         # print(dfbinding)
 
     traj_root = Path(
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/rprocess_from_trajectory.py` & `artistools-2023.8.1/artistools/inputmodel/rprocess_from_trajectory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
+from __future__ import annotations
+
 import argparse
 import io
 import math
 import multiprocessing
 import tarfile
 import time
+import typing as t
 from functools import lru_cache
 from functools import partial
 from pathlib import Path
-from typing import Literal
-from typing import Optional
-from typing import Union
 
 import argcomplete
 import numpy as np
 import pandas as pd
 
 import artistools as at
 
 
 def get_elemabund_from_nucabund(dfnucabund: pd.DataFrame) -> dict[str, float]:
     """Return a dictionary of elemental abundances from nuclear abundance DataFrame."""
-    dictelemabund: dict[str, float] = {}
-    for atomic_number in range(1, dfnucabund.Z.max() + 1):
-        dictelemabund[f"X_{at.get_elsymbol(atomic_number)}"] = dfnucabund.query(
-            "Z == @atomic_number", inplace=False
-        ).massfrac.sum()
+    dictelemabund: dict[str, float] = {
+        f"X_{at.get_elsymbol(atomic_number)}": dfnucabund.query("Z == @atomic_number", inplace=False).massfrac.sum()
+        for atomic_number in range(1, dfnucabund.Z.max() + 1)
+    }
     return dictelemabund
 
 
 def open_tar_file_or_extracted(traj_root: Path, particleid: int, memberfilename: str):
     """Trajectory files are generally stored as {particleid}.tar.xz, but this is slow
     to access, so first check for extracted files, or decompressed .tar files,
     which are much faster to access.
@@ -42,15 +41,15 @@
     if not tarfilepath.is_file():
         tarfilepath = Path(traj_root, f"{particleid}.tar.xz")
 
     if memberfilename.endswith(".dat") and not path_extracted_file.is_file():
         tarfile.open(tarfilepath, "r:*").extract(path=Path(traj_root, str(particleid)), member=memberfilename)
 
     if path_extracted_file.is_file():
-        return open(path_extracted_file, encoding="utf-8")  # noqa: SIM115
+        return path_extracted_file.open(encoding="utf-8")
 
     if not tarfilepath.is_file():
         print(f"No network data found for particle {particleid} (so can't access {memberfilename})")
         raise FileNotFoundError
 
     # print(f"using {tarfilepath} for {memberfilename}")
     # return tarfile.open(tarfilepath, "r:*").extractfile(member=memberfilename)
@@ -64,52 +63,46 @@
     print(f"Member {memberfilename} not found in {tarfilepath}")
     raise AssertionError
 
 
 @lru_cache(maxsize=16)
 def get_dfevol(traj_root: Path, particleid: int) -> pd.DataFrame:
     with open_tar_file_or_extracted(traj_root, particleid, "./Run_rprocess/evol.dat") as evolfile:
-        dfevol = pd.read_csv(
+        return pd.read_csv(
             evolfile,
             sep=r"\s+",
             comment="#",
             usecols=[0, 1],
             names=["nstep", "timesec"],
             engine="c",
             dtype={0: "int32[pyarrow]", 1: "float32[pyarrow]"},
             dtype_backend="pyarrow",
         )
 
-    return dfevol
-
 
 def get_closest_network_timestep(
-    traj_root: Path, particleid: int, timesec: float, cond: Literal["lessthan", "greaterthan", "nearest"] = "nearest"
+    traj_root: Path, particleid: int, timesec: float, cond: t.Literal["lessthan", "greaterthan", "nearest"] = "nearest"
 ) -> int:
     """cond:
     'lessthan': find highest timestep less than time_sec
     'greaterthan': find lowest timestep greater than time_sec.
     """
     dfevol = get_dfevol(traj_root, particleid)
 
     if cond == "nearest":
         idx = np.abs(dfevol.timesec.to_numpy() - timesec).argmin()
+        return dfevol["nstep"].to_numpy()[idx]
 
-    elif cond == "greaterthan":
-        return dfevol.query("timesec > @timesec")["nstep"].min()
-
-    elif cond == "lessthan":
-        return dfevol.query("timesec < @timesec")["nstep"].max()
+    if cond == "greaterthan":
+        return dfevol[dfevol["timesec"] > timesec]["nstep"].min()
 
-    else:
-        raise AssertionError
-
-    nts: int = dfevol["nstep"].to_numpy()[idx]
+    if cond == "lessthan":
+        return dfevol[dfevol["timesec"] < timesec]["nstep"].max()
 
-    return nts
+    raise AssertionError
 
 
 def get_trajectory_timestepfile_nuc_abund(
     traj_root: Path, particleid: int, memberfilename: str
 ) -> tuple[pd.DataFrame, float]:
     """Get the nuclear abundances for a particular trajectory id number and time
     memberfilename should be something like "./Run_rprocess/tday_nz-plane".
@@ -158,15 +151,15 @@
     # print(f'abund sum: {normfactor}')
     # dfnucabund.eval('numberfrac = abund / @normfactor', inplace=True)
 
     return dfnucabund, t_model_init_seconds
 
 
 def get_trajectory_qdotintegral(particleid: int, traj_root: Path, nts_max: int, t_model_s: float) -> float:
-    """Initial cell energy [erg/g]."""
+    """Calculate initial cell energy [erg/g] from reactions t < t_model_s (reduced by work done)."""
     with open_tar_file_or_extracted(traj_root, particleid, "./Run_rprocess/energy_thermo.dat") as enthermofile:
         try:
             dfthermo: pd.DataFrame = pd.read_csv(
                 enthermofile,
                 sep=r"\s+",
                 usecols=["time/s", "Qdot"],
                 engine="c",
@@ -191,16 +184,16 @@
 
     return qdotintegral
 
 
 def get_trajectory_abund_q(
     particleid: int,
     traj_root: Path,
-    t_model_s: Optional[float] = None,
-    nts: Optional[int] = None,
+    t_model_s: float | None = None,
+    nts: int | None = None,
     getqdotintegral: bool = False,
 ) -> dict[str, float]:
     """Get the nuclear mass fractions (and Qdotintegral) for a particle particle number as a given time
     nts: GSI network timestep number.
     """
     assert t_model_s is not None or nts is not None
     try:
@@ -248,15 +241,15 @@
         )
 
     return dict_traj_nuc_abund
 
 
 def get_modelcellabundance(
     dict_traj_nuc_abund: dict[int, pd.DataFrame], minparticlespercell: int, cellgroup: tuple[int, pd.DataFrame]
-) -> Optional[dict[str, float]]:
+) -> dict[str, float] | None:
     cellindex: int
     dfthiscellcontribs: pd.DataFrame
     cellindex, dfthiscellcontribs = cellgroup
 
     if len(dfthiscellcontribs) < minparticlespercell:
         return None
 
@@ -265,26 +258,24 @@
         for particleid, frac_of_cellmass in dfthiscellcontribs[["particleid", "frac_of_cellmass"]].itertuples(
             index=False
         )
         if particleid in dict_traj_nuc_abund
     ]
 
     # adjust frac_of_cellmass for missing particles
-    cell_frac_sum = sum([frac_of_cellmass for _, frac_of_cellmass in contribparticles])
+    cell_frac_sum = sum(frac_of_cellmass for _, frac_of_cellmass in contribparticles)
 
     nucabundcolnames = {
         col for particleid in dfthiscellcontribs.particleid for col in dict_traj_nuc_abund.get(particleid, {})
     }
 
     row = {
         nucabundcolname: sum(
-            [
-                frac_of_cellmass * traj_nuc_abund.get(nucabundcolname, 0.0) / cell_frac_sum
-                for traj_nuc_abund, frac_of_cellmass in contribparticles
-            ]
+            frac_of_cellmass * traj_nuc_abund.get(nucabundcolname, 0.0) / cell_frac_sum
+            for traj_nuc_abund, frac_of_cellmass in contribparticles
         )
         for nucabundcolname in nucabundcolnames
     }
 
     row["inputcellid"] = cellindex
 
     # if n % 100 == 0:
@@ -293,46 +284,45 @@
     #           f'{n:4d} of {active_inputcellcount:4d}, {n / active_inputcellcount * 100:4.1f}%) '
     #           f' contributing {len(dfthiscellcontribs):4d} particles.'
     #           f' total func time {functime:.1f} s, {n / functime:.1f} cell/s,'
     #           f' expected time: {functime / n * active_inputcellcount:.1f}')
     return row
 
 
-def get_gridparticlecontributions(gridcontribpath: Union[Path, str]) -> pd.DataFrame:
-    dfcontribs = pd.read_csv(
-        Path(gridcontribpath, "gridcontributions.txt"),
+def get_gridparticlecontributions(gridcontribpath: Path | str) -> pd.DataFrame:
+    return pd.read_csv(
+        at.zopen(Path(gridcontribpath, "gridcontributions.txt")),
         delim_whitespace=True,
         dtype={
             0: "int32[pyarrow]",
             1: "int32[pyarrow]",
             2: "float32[pyarrow]",
             3: "float32[pyarrow]",
         },
         dtype_backend="pyarrow",
     )
 
-    return dfcontribs
 
+def particlenetworkdatafound(traj_root: Path, particleid: int) -> bool:
+    return (
+        (traj_root / f"{particleid}.tar.xz").is_file()
+        or (traj_root / f"{particleid}.tar").is_file()
+        or (traj_root / str(particleid)).is_dir()
+    )
 
-def filtermissinggridparticlecontributions(traj_root: Path, dfcontribs: pd.DataFrame) -> pd.DataFrame:
-    missing_particleids = []
-    for particleid in sorted(dfcontribs.particleid.unique()):
-        if (
-            not Path(traj_root, f"{particleid}.tar.xz").is_file()
-            and not Path(traj_root, f"{particleid}.tar").is_file()
-            and not Path(traj_root, str(particleid)).is_dir()
-        ):
-            missing_particleids.append(particleid)
-            # print(f' WARNING particle {particleid} not found!')
 
+def filtermissinggridparticlecontributions(traj_root: Path, dfcontribs: pd.DataFrame) -> pd.DataFrame:
+    missing_particleids = [
+        particleid
+        for particleid in sorted(dfcontribs.particleid.unique())
+        if not particlenetworkdatafound(traj_root, particleid)
+    ]
     print(
-        (
-            f"Adding gridcontributions column that excludes {len(missing_particleids)} "
-            "particles without abundance data and renormalising..."
-        ),
+        f"Adding gridcontributions column that excludes {len(missing_particleids)} "
+        "particles without abundance data and renormalising...",
         end="",
     )
     # after filtering, frac_of_cellmass_includemissing will still include particles with rho but no abundance data
     # frac_of_cellmass will exclude particles with no abundances
     dfcontribs["frac_of_cellmass_includemissing"] = dfcontribs["frac_of_cellmass"]
     # dfcontribs.query('particleid not in @missing_particleids', inplace=True)
     dfcontribs.loc[dfcontribs.eval("particleid in @missing_particleids"), "frac_of_cellmass"] = 0.0
@@ -543,44 +533,20 @@
         traj_root, particleid, "./Run_rprocess/tday_nz-plane"
     )
     dfnucabund = dfnucabund.iloc[dfnucabund["Z"] >= 1]
     dfnucabund["radioactive"] = True
 
     t_model_init_days = t_model_init_seconds / (24 * 60 * 60)
 
-    wollager_profilename = "wollager_ejectaprofile_10bins.txt"
-    if Path(wollager_profilename).exists():
-        print(f"{wollager_profilename} found")
-        t_model_init_days_in = float(Path(wollager_profilename).open("rt").readline().strip().removesuffix(" day"))
-        dfdensities = pd.read_csv(
-            wollager_profilename, delim_whitespace=True, skiprows=1, names=["cellid", "velocity_outer", "rho"]
-        )
-        dfdensities["cellid"] = dfdensities["cellid"].astype(int)
-        dfdensities["velocity_inner"] = np.concatenate(([0.0], dfdensities["velocity_outer"].to_numpy()[:-1]))
-
-        t_model_init_seconds_in = t_model_init_days_in * 24 * 60 * 60
-        dfdensities = dfdensities.eval(
-            (
-                "cellmass_grams = rho * 4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
-                "* (1e5 * @t_model_init_seconds_in) ** 3"
-            ),
-        )
-
-        # now replace the density at the input time with the density at required time
-
-        dfdensities = dfdensities.eval(
-            (
-                "rho = cellmass_grams / ("
-                "4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
-                " * (1e5 * @t_model_init_seconds) ** 3)"
-            ),
-        )
+    wollaeger_profilename = "wollaeger_ejectaprofile_10bins.txt"
+    if Path(wollaeger_profilename).exists():
+        dfdensities = get_wollaeger_density_profile(wollaeger_profilename)
     else:
         rho = 1e-11
-        print(f"{wollager_profilename} not found. Using rho {rho} g/cm3")
+        print(f"{wollaeger_profilename} not found. Using rho {rho} g/cm3")
         dfdensities = pd.DataFrame({"rho": rho, "velocity_outer": 6.0e4}, index=[0])
 
     # print(dfdensities)
 
     # write abundances.txt
     dictelemabund = get_elemabund_from_nucabund(dfnucabund)
 
@@ -603,31 +569,56 @@
         "X_Co57": 0.0,
     }
 
     for _, row in dfnucabund.query("radioactive == True").iterrows():
         A = row.N + row.Z
         rowdict[f"X_{at.get_elsymbol(row.Z)}{A}"] = row.massfrac
 
-    modeldata = []
-    for mgi, densityrow in dfdensities.iterrows():
-        # print(mgi, densityrow)
-        modeldata.append(
-            dict(
-                inputcellid=mgi + 1,
-                velocity_outer=densityrow["velocity_outer"],
-                logrho=math.log10(densityrow["rho"]),
-                **rowdict,
-            )
+    modeldata = [
+        dict(
+            inputcellid=mgi + 1,
+            velocity_outer=densityrow["velocity_outer"],
+            logrho=math.log10(densityrow["rho"]),
+            **rowdict,
         )
+        for mgi, densityrow in dfdensities.iterrows()
+    ]
     # print(modeldata)
 
     dfmodel = pd.DataFrame(modeldata)
     # print(dfmodel)
     at.inputmodel.save_modeldata(dfmodel=dfmodel, t_model_init_days=t_model_init_days, modelpath=Path(args.outputpath))
-    with open(Path(args.outputpath, "gridcontributions.txt"), "w") as fcontribs:
+    with Path(args.outputpath, "gridcontributions.txt").open("w") as fcontribs:
         fcontribs.write("particleid cellindex frac_of_cellmass\n")
         for cell in dfmodel.itertuples(index=False):
-            fcontribs.write(f"{particleid} {cell.inputcellid} {1.}\n")
+            fcontribs.write(f"{particleid} {cell.inputcellid} 1.0\n")
+
+
+def get_wollaeger_density_profile(wollaeger_profilename):
+    print(f"{wollaeger_profilename} found")
+    t_model_init_days_in = float(Path(wollaeger_profilename).open("rt").readline().strip().removesuffix(" day"))
+    result = pd.read_csv(
+        wollaeger_profilename,
+        delim_whitespace=True,
+        skiprows=1,
+        names=["cellid", "velocity_outer", "rho"],
+    )
+    result["cellid"] = result["cellid"].astype(int)
+    result["velocity_inner"] = np.concatenate(([0.0], result["velocity_outer"].to_numpy()[:-1]))
+
+    t_model_init_seconds_in = t_model_init_days_in * 24 * 60 * 60
+    result = result.eval(
+        "cellmass_grams = rho * 4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
+        "* (1e5 * @t_model_init_seconds_in) ** 3"
+    )
+
+    # now replace the density at the input time with the density at required time
+
+    return result.eval(
+        "rho = cellmass_grams / ("
+        "4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
+        " * (1e5 * @t_model_init_seconds) ** 3)"
+    )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/rprocess_solar.py` & `artistools-2023.8.1/artistools/inputmodel/rprocess_solar.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,15 @@
         delim_whitespace=True,
         comment="#",
         names=["A", "Z", "Q[MeV]", "Egamma[MeV]", "Eelec[MeV]", "Eneutrino[MeV]", "tau[s]"],
     )
 
     def undecayed_z(row):
         dfmasschain = dfbetaminus.query("A == @row.A", inplace=False)
-        if not dfmasschain.empty:
-            return int(dfmasschain.Z.min())  # decay to top of chain
-        return int(row.Z)
+        return int(row.Z) if dfmasschain.empty else int(dfmasschain.Z.min())
 
     dfsolarabund_undecayed = dfsolarabund.copy()
     dfsolarabund_undecayed["Z"] = dfsolarabund_undecayed.apply(undecayed_z, axis=1)
 
     # Andreas uses 90% Fe and the rest solar
     dfsolarabund_undecayed = dfsolarabund_undecayed.append(
         {"Z": 26, "A": 56, "numberfrac": 0.005, "radioactive": False}, ignore_index=True
@@ -76,28 +74,24 @@
             wollager_profilename, delim_whitespace=True, skiprows=1, names=["cellid", "velocity_outer", "rho"]
         )
         dfdensities["cellid"] = dfdensities["cellid"].astype(int)
         dfdensities["velocity_inner"] = np.concatenate(([0.0], dfdensities["velocity_outer"].to_numpy()[:-1]))
 
         t_model_init_seconds_in = t_model_init_days_in * 24 * 60 * 60
         dfdensities = dfdensities.eval(
-            (
-                "cellmass_grams = rho * 4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
-                "* (1e5 * @t_model_init_seconds_in) ** 3"
-            ),
+            "cellmass_grams = rho * 4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
+            "* (1e5 * @t_model_init_seconds_in) ** 3",
         )
 
         # now replace the density at the input time with the density at required time
 
         dfdensities = dfdensities.eval(
-            (
-                "rho = cellmass_grams / ("
-                "4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
-                " * (1e5 * @t_model_init_seconds) ** 3)"
-            ),
+            "rho = cellmass_grams / ("
+            "4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
+            " * (1e5 * @t_model_init_seconds) ** 3)",
         )
     else:
         dfdensities = pd.DataFrame({"rho": 10**-3, "velocity_outer": 6.0e4}, index=[0])
 
     # print(dfdensities)
     cellcount = len(dfdensities)
     # write abundances.txt
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/scalevelocity.py` & `artistools-2023.8.1/artistools/inputmodel/scalevelocity.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,16 @@
     parser.add_argument(
         "-outputfile", "-o", default="model_velscale{velscale:.2f}.txt", help="Path of output model file"
     )
 
 
 def eval_mshell(dfmodel: pd.DataFrame, t_model_init_seconds: float) -> None:
     dfmodel = dfmodel.eval(
-        (
-            "cellmass_grams = 10 ** logrho * 4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
-            "* (1e5 * @t_model_init_seconds) ** 3"
-        ),
+        "cellmass_grams = 10 ** logrho * 4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
+        "* (1e5 * @t_model_init_seconds) ** 3",
     )
 
 
 def main(args=None, argsraw=None, **kwargs) -> None:
     """Scale the velocity of an ARTIS model, keeping mass constant and saving back to ARTIS format."""
     if args is None:
         parser = argparse.ArgumentParser(
@@ -60,19 +58,17 @@
 
     print(f"Applying velocity factor of {velscale} (kinetic energy factor {kescale}) and conserving shell masses")
 
     dfmodel.velocity_inner *= velscale
     dfmodel.velocity_outer *= velscale
 
     dfmodel = dfmodel.eval(
-        (
-            "logrho = log10(cellmass_grams / ("
-            "4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
-            " * (1e5 * @t_model_init_seconds) ** 3))"
-        ),
+        "logrho = log10(cellmass_grams / ("
+        "4. / 3. * @math.pi * (velocity_outer ** 3 - velocity_inner ** 3)"
+        " * (1e5 * @t_model_init_seconds) ** 3))",
     )
 
     eval_mshell(dfmodel, t_model_init_seconds)
 
     print(dfmodel)
 
     outputfile = args.outputfile.format(velscale=velscale, kescale=kescale)
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/shen2018.py` & `artistools-2023.8.1/artistools/inputmodel/shen2018.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 import argparse
 import math
-import os.path
+from pathlib import Path
 
 import pandas as pd
 from astropy import units as u
 
 import artistools as at
 
 
@@ -19,15 +19,15 @@
     if args is None:
         parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
-    with open(args.inputpath) as infile:
+    with Path(args.inputpath).open() as infile:
         columns = infile.readline().split()
 
     atomicnumberofspecies = {}
     isotopesofelem: dict[int, list[str]] = {}
     for species in columns[5:]:
         atomic_number = at.get_atomic_number(species.rstrip("0123456789"))
         atomicnumberofspecies[species] = atomic_number
@@ -71,28 +71,28 @@
 
         tot_ni56mass += m_shell_grams * shell.ni56
 
         abundances = [0.0 for _ in range(31)]
 
         X_Fegroup = 0.0
         for atomic_number in range(1, 31):
-            abundances[atomic_number] = sum([float(shell[species]) for species in isotopesofelem[atomic_number]])
+            abundances[atomic_number] = sum(float(shell[species]) for species in isotopesofelem[atomic_number])
             if atomic_number >= 26:
                 X_Fegroup += abundances[atomic_number]
 
         radioabundances = [X_Fegroup, shell.ni56, shell.co56, shell.fe52, shell.cr48, shell.ni57, shell.co57]
 
         dfmodel.loc[cellid] = [cellid, v_outer, math.log10(rho), *radioabundances]
         dfelabundances.loc[cellid] = [cellid, *abundances[1:31]]
 
         v_inner = v_outer
         m_enc_inner = m_enc_outer
 
     print(f'M_tot  = {m_enc_outer /  u.solMass.to("g"):.3f} solMass')
     print(f'M_Ni56 = {tot_ni56mass /  u.solMass.to("g"):.3f} solMass')
 
-    at.save_modeldata(dfmodel, t_model_init_days, os.path.join(args.outputpath, "model.txt"))
-    at.inputmodel.save_initelemabundances(dfelabundances, os.path.join(args.outputpath, "abundances.txt"))
+    at.save_modeldata(dfmodel, t_model_init_days, Path(args.outputpath, "model.txt"))
+    at.inputmodel.save_initelemabundances(dfelabundances, Path(args.outputpath, "abundances.txt"))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/slice1Dfromconein3dmodel.py` & `artistools-2023.8.1/artistools/inputmodel/slice1Dfromconein3dmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
     # print(modelpath)
     model_df = model_df.round(decimals=5)  # model files seem to be to 5 sf
     model_df.to_csv(args.modelpath[0] / "model_1D.txt", sep=" ", header=False)  # write model.txt
 
     abundances_df.to_csv(args.modelpath[0] / "abundances_1D.txt", sep=" ", header=False)  # write abundances.txt
 
-    with open(args.modelpath[0] / "model_1D.txt", "r+") as f:  # add number of cells and tmodel to start of file
+    with Path(args.modelpath[0], "model_1D.txt").open("r+") as f:  # add number of cells and tmodel to start of file
         content = f.read()
         f.seek(0, 0)
         f.write(f"{model_df.shape[0]}\n{args.t_model}".rstrip("\r\n") + "\n" + content)
 
     print("Saved abundances_1D.txt and model_1D.txt")
 
 
@@ -212,15 +212,15 @@
             description=__doc__,
         )
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     if not args.modelpath:
-        args.modelpath = [Path(".")]
+        args.modelpath = [Path()]
 
     args.other_axis1 = None
     args.other_axis2 = None
     axes = ["x", "y", "z"]
     for ax in axes:
         if args.other_axis1 is None and ax != args.sliceaxis:
             args.other_axis1 = ax
```

### Comparing `artistools-2023.5.16.3/artistools/inputmodel/test_inputmodel.py` & `artistools-2023.8.1/artistools/inputmodel/test_inputmodel.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/lightcurve/__init__.py` & `artistools-2023.8.1/artistools/lightcurve/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/lightcurve/lightcurve.py` & `artistools-2023.8.1/artistools/lightcurve/lightcurve.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
+from __future__ import annotations
+
 import argparse
 import math
-import os
-from collections.abc import Collection
+import typing as t
 from pathlib import Path
-from typing import Any
-from typing import Literal
-from typing import Optional
-from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import polars as pl
 from astropy import constants as const
 from astropy import units as u
+from typeguard import typechecked
 
 import artistools as at
 
 
+@typechecked
 def readfile(
-    filepath: Union[str, Path],
-) -> dict[int, pd.DataFrame]:
+    filepath: str | Path,
+) -> dict[int, pl.DataFrame]:
     """Read an ARTIS light curve file."""
     print(f"Reading {filepath}")
-    lcdata: dict[int, pd.DataFrame] = {}
+    lcdata: dict[int, pl.DataFrame] = {}
     if "_res" in str(filepath):
         # get a dict of dfs with light curves at each viewing direction bin
         lcdata_res = pl.read_csv(
             at.zopen(filepath, "rb").read(), separator=" ", has_header=False, new_columns=["time", "lum", "lum_cmf"]
         )
         lcdata = at.split_dataframe_dirbins(lcdata_res, index_of_repeated_value=0, output_polarsdf=True)
     else:
@@ -40,15 +39,15 @@
             dfsphericalaverage = dfsphericalaverage[: dfsphericalaverage.height // 2]
         lcdata[-1] = dfsphericalaverage
 
     return lcdata
 
 
 def read_3d_gammalightcurve(
-    filepath: Union[str, Path],
+    filepath: str | Path,
 ) -> dict[int, pd.DataFrame]:
     columns = ["time"]
     columns.extend(np.arange(0, 100))
     lcdata = pd.read_csv(filepath, delim_whitespace=True, header=None)
     lcdata.columns = columns
     # lcdata = lcdata.rename(columns={0: 'time', 1: 'lum', 2: 'lum_cmf'})
 
@@ -56,29 +55,30 @@
     for angle in np.arange(0, 100):
         res_data[angle] = lcdata[["time", angle]]
         res_data[angle] = res_data[angle].rename(columns={angle: "lum"})
 
     return res_data
 
 
+@typechecked
 def get_from_packets(
-    modelpath: Union[str, Path],
-    escape_type: Literal["TYPE_RPKT", "TYPE_GAMMA"] = "TYPE_RPKT",
-    maxpacketfiles: Optional[int] = None,
-    directionbins: Optional[Collection[int]] = None,
+    modelpath: str | Path,
+    escape_type: t.Literal["TYPE_RPKT", "TYPE_GAMMA"] = "TYPE_RPKT",
+    maxpacketfiles: int | None = None,
+    directionbins: t.Collection[int] | None = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
     get_cmf_column: bool = True,
 ) -> dict[int, pl.DataFrame]:
     """Get ARTIS luminosity vs time from packets files."""
     if directionbins is None:
         directionbins = [-1]
-    tmidarray = at.get_timestep_times_float(modelpath=modelpath, loc="mid")
-    timearray = at.get_timestep_times_float(modelpath=modelpath, loc="start")
-    arr_timedelta = at.get_timestep_times_float(modelpath=modelpath, loc="delta")
+    tmidarray = at.get_timestep_times(modelpath=modelpath, loc="mid")
+    timearray = at.get_timestep_times(modelpath=modelpath, loc="start")
+    arr_timedelta = at.get_timestep_times(modelpath=modelpath, loc="delta")
     # timearray = np.arange(250, 350, 0.1)
     if get_cmf_column:
         _, modelmeta = at.inputmodel.get_modeldata(modelpath, getheadersonly=True, printwarningsonly=True)
         escapesurfacegamma = math.sqrt(1 - (modelmeta["vmax_cmps"] / 29979245800) ** 2)
     else:
         escapesurfacegamma = None
 
@@ -168,17 +168,17 @@
     return lcdata
 
 
 def generate_band_lightcurve_data(
     modelpath: Path,
     args: argparse.Namespace,
     angle: int = -1,
-    modelnumber: Optional[int] = None,
+    modelnumber: int | None = None,
 ) -> dict:
-    """Method adapted from https://github.com/cinserra/S3/blob/master/src/s3/SMS.py."""
+    """Integrate spectra to get band magnitude vs time. Method adapted from https://github.com/cinserra/S3/blob/master/src/s3/SMS.py."""
     from scipy.interpolate import interp1d
 
     if args.plotvspecpol and (modelpath / "vpkt.txt").is_file():
         print("Found vpkt.txt, using virtual packets")
         stokes_params = (
             at.spectra.get_vspecpol_data(vspecangle=angle, modelpath=modelpath)
             if angle >= 0
@@ -228,15 +228,15 @@
                 (time, bol_magnitude)
                 for time, bol_magnitude in zip(times, bol_magnitudes)
                 if math.isfinite(bol_magnitude)
             ]
         elif filter_name not in filters_dict:
             filters_dict[filter_name] = []
 
-    filterdir = os.path.join(at.get_config()["path_artistools_dir"], "data/filters/")
+    filterdir = Path(at.get_config()["path_artistools_dir"], "data/filters/")
 
     for filter_name in filters_list:
         if filter_name == "bol":
             continue
         zeropointenergyflux, wavefilter, transmission, wavefilter_min, wavefilter_max = get_filter_data(
             filterdir, filter_name
         )
@@ -275,59 +275,57 @@
                 filters_dict[filter_name].append((time, phot_filtobs_sn))
 
     return filters_dict
 
 
 def bolometric_magnitude(
     modelpath: Path,
-    timearray: Collection[float],
+    timearray: t.Collection[float],
     args: argparse.Namespace,
     angle: int = -1,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
 ) -> tuple[list[float], list[float]]:
     magnitudes = []
     times = []
 
     for timestep, time in enumerate(timearray):
         time = float(time)
 
         if (args.timemin is None or args.timemin <= time) and (args.timemax is None or args.timemax >= time):
-            if angle != -1:
-                if args.plotvspecpol:
-                    spectrum = at.spectra.get_vspecpol_spectrum(modelpath, time, angle, args)
-                else:
-                    spectrum = at.spectra.get_spectrum(
-                        modelpath=modelpath,
-                        directionbins=[angle],
-                        timestepmin=timestep,
-                        timestepmax=timestep,
-                        average_over_phi=average_over_phi,
-                        average_over_theta=average_over_theta,
-                    )[angle]
-            else:
+            if angle == -1:
                 spectrum = at.spectra.get_spectrum(modelpath=modelpath, timestepmin=timestep, timestepmax=timestep)[-1]
 
+            elif args.plotvspecpol:
+                spectrum = at.spectra.get_vspecpol_spectrum(modelpath, time, angle, args)
+            else:
+                spectrum = at.spectra.get_spectrum(
+                    modelpath=modelpath,
+                    directionbins=[angle],
+                    timestepmin=timestep,
+                    timestepmax=timestep,
+                    average_over_phi=average_over_phi,
+                    average_over_theta=average_over_theta,
+                )[angle]
             integrated_flux = np.trapz(spectrum["f_lambda"], spectrum["lambda_angstroms"])
             integrated_luminosity = integrated_flux * 4 * np.pi * np.power(u.Mpc.to("cm"), 2)
             Mbol_sun = 4.74
-            magnitude = Mbol_sun - (2.5 * np.log10(integrated_luminosity / const.L_sun.to("erg/s").value))
+            with np.errstate(divide="ignore"):
+                magnitude = Mbol_sun - (2.5 * np.log10(integrated_luminosity / const.L_sun.to("erg/s").value))
             magnitudes.append(magnitude)
             times.append(time)
             # print(const.L_sun.to('erg/s').value)
             # sys.exit(1)
 
     return times, magnitudes
 
 
-def get_filter_data(
-    filterdir: Union[Path, str], filter_name: str
-) -> tuple[float, np.ndarray, np.ndarray, float, float]:
+def get_filter_data(filterdir: Path | str, filter_name: str) -> tuple[float, np.ndarray, np.ndarray, float, float]:
     """Filter data in 'data/filters' taken from https://github.com/cinserra/S3/tree/master/src/s3/metadata."""
-    with Path(filterdir, filter_name + ".txt").open("r") as filter_metadata:  # defintion of the file
+    with Path(filterdir, f"{filter_name}.txt").open("r") as filter_metadata:  # defintion of the file
         line_in_filter_metadata = filter_metadata.readlines()  # list of lines
 
     zeropointenergyflux = float(line_in_filter_metadata[0])
     # zero point in energy flux (erg/cm^2/s)
 
     wavefilter, transmission = [], []
     for row in line_in_filter_metadata[4:]:
@@ -338,22 +336,22 @@
     wavefilter_min = min(wavefilter)
     wavefilter_max = int(max(wavefilter))
 
     return zeropointenergyflux, np.array(wavefilter), np.array(transmission), wavefilter_min, wavefilter_max
 
 
 def get_spectrum_in_filter_range(
-    modelpath: Union[Path, str],
+    modelpath: Path | str,
     timestep: int,
     time: float,
     wavefilter_min: float,
     wavefilter_max: float,
     angle: int = -1,
-    spectrum: Optional[pd.DataFrame] = None,
-    args: Optional[argparse.Namespace] = None,
+    spectrum: pd.DataFrame | None = None,
+    args: argparse.Namespace | None = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
 ) -> tuple[np.ndarray, np.ndarray]:
     spectrum = at.spectra.get_spectrum_at_time(
         Path(modelpath),
         timestep=timestep,
         time=time,
@@ -371,17 +369,15 @@
 
     return np.array(wavelength_from_spectrum), np.array(flux)
 
 
 def evaluate_magnitudes(flux, transmission, wavelength_from_spectrum, zeropointenergyflux: float) -> float:
     cf = flux * transmission
     flux_obs = abs(np.trapz(cf, wavelength_from_spectrum))  # using trapezoidal rule to integrate
-    phot_filtobs_sn = 0.0 if flux_obs == 0.0 else -2.5 * np.log10(flux_obs / zeropointenergyflux)
-
-    return phot_filtobs_sn
+    return 0.0 if flux_obs == 0.0 else -2.5 * np.log10(flux_obs / zeropointenergyflux)
 
 
 def get_band_lightcurve(band_lightcurve_data, band_name, args: argparse.Namespace) -> tuple[list[float], np.ndarray]:
     time, brightness_in_mag = zip(
         *[
             (time, brightness)
             for time, brightness in band_lightcurve_data[band_name]
@@ -409,40 +405,37 @@
             plot_times.append(time)
             colour_delta_mag.append(time_dict_1[time] - time_dict_2[time])
 
     return plot_times, colour_delta_mag
 
 
 def read_hesma_lightcurve(args: argparse.Namespace) -> pd.DataFrame:
-    hesma_directory = os.path.join(at.get_config()["path_artistools_dir"], "data/hesma")
+    hesma_directory = Path(at.get_config()["path_artistools_dir"], "data/hesma")
     filename = args.plot_hesma_model
     hesma_modelname = hesma_directory / filename
 
-    column_names = []
-    with open(hesma_modelname) as f:
+    column_names: list[str] = []
+    with hesma_modelname.open() as f:
         first_line = f.readline()
         if "#" in first_line:
-            for i in first_line:
-                if i != "#" and i != " " and i != "\n":
-                    column_names.append(i)
-
+            column_names.extend(i for i in first_line if i not in ["#", " ", "\n"])
             hesma_model = pd.read_csv(
                 hesma_modelname, delim_whitespace=True, header=None, comment="#", names=column_names
             )
 
         else:
             hesma_model = pd.read_csv(hesma_modelname, delim_whitespace=True)
     return hesma_model
 
 
-def read_reflightcurve_band_data(lightcurvefilename: Union[Path, str]) -> tuple[pd.DataFrame, dict[str, Any]]:
+def read_reflightcurve_band_data(lightcurvefilename: Path | str) -> tuple[pd.DataFrame, dict[str, t.Any]]:
     filepath = Path(at.get_config()["path_artistools_dir"], "data", "lightcurves", lightcurvefilename)
     metadata = at.get_file_metadata(filepath)
 
-    data_path = os.path.join(at.get_config()["path_artistools_dir"], f"data/lightcurves/{lightcurvefilename}")
+    data_path = Path(at.get_config()["path_artistools_dir"], f"data/lightcurves/{lightcurvefilename}")
     lightcurve_data = pd.read_csv(data_path, comment="#")
     if len(lightcurve_data.keys()) == 1:
         lightcurve_data = pd.read_csv(data_path, comment="#", delim_whitespace=True)
 
     lightcurve_data["magnitude"] = pd.to_numeric(lightcurve_data["magnitude"])  # force column to be float
 
     lightcurve_data["time"] = lightcurve_data["time"].apply(lambda x: x - (metadata["timecorrection"]))
@@ -470,31 +463,33 @@
         if Path(lightcurvefilename).is_file()
         else Path(at.get_config()["path_artistools_dir"], "data/lightcurves/bollightcurves", lightcurvefilename)
     )
 
     metadata = at.get_file_metadata(data_path)
 
     # check for possible header line and read table
-    with open(data_path) as flc:
+    with data_path.open() as flc:
         filepos = flc.tell()
         line = flc.readline()
         if line.startswith("#"):
             columns = line.lstrip("#").split()
         else:
             flc.seek(filepos)  # undo the readline() and go back
             columns = None
 
         dflightcurve = pd.read_csv(flc, delim_whitespace=True, header=None, names=columns)
 
-    colrenames = {
+    if colrenames := {
         k: v
-        for k, v in {dflightcurve.columns[0]: "time_days", dflightcurve.columns[1]: "luminosity_erg/s"}.items()
+        for k, v in {
+            dflightcurve.columns[0]: "time_days",
+            dflightcurve.columns[1]: "luminosity_erg/s",
+        }.items()
         if k != v
-    }
-    if colrenames:
+    }:
         print(f"{data_path}: renaming columns {colrenames}")
         dflightcurve = dflightcurve.rename(columns=colrenames)
 
     return dflightcurve, metadata
 
 
 def get_sn_sample_bol():
```

### Comparing `artistools-2023.5.16.3/artistools/lightcurve/plotlightcurve.py` & `artistools-2023.8.1/artistools/lightcurve/plotlightcurve.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 # PYTHON_ARGCOMPLETE_OK
+from __future__ import annotations
+
 import argparse
 import math
-import os
 import sys
+import typing as t
 from collections.abc import Iterable
-from collections.abc import Sequence
 from pathlib import Path
-from typing import Any
-from typing import Literal
-from typing import Optional
-from typing import Union
 
 import argcomplete
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import polars as pl
@@ -23,16 +20,16 @@
 
 import artistools as at
 
 color_list = list(plt.get_cmap("tab20")(np.linspace(0, 1.0, 20)))
 
 
 def plot_deposition_thermalisation(axis, axistherm, modelpath, modelname, plotkwargs, args) -> None:
-    if args.logscalex:
-        axistherm.set_xscale("log")
+    # if args.logscalex:
+    #     axistherm.set_xscale("log")
 
     # if args.logscaley:
     #     axistherm.set_yscale("log")
     #     axistherm.set_ylim(bottom=0.1, top=1.0)
 
     if args.plotthermalisation:
         dfmodel, modelmeta = at.inputmodel.get_modeldata(
@@ -116,59 +113,73 @@
                 **plotkwargs,
                 "label": plotkwargs["label"] + r" $\dot{E}_{dep,\beta^-}$",
                 "linestyle": "dashed",
                 "color": color_beta,
             },
         )
 
-    c23modelpath = Path(
-        "/Users/luke/Library/CloudStorage/GoogleDrive-luke@lukeshingles.com/Shared"
-        " drives/ARTIS/artis_runs_published/Collinsetal2023/sfho_long_1-35-135Msun"
-    )
-
-    c23energyrate = at.inputmodel.energyinputfiles.get_energy_rate_fromfile(c23modelpath)
-    c23etot, c23energydistribution_data = at.inputmodel.energyinputfiles.get_etot_fromfile(c23modelpath)
-
-    dE = np.diff(c23energyrate["rate"] * c23etot)
-    dt = np.diff(c23energyrate["times"] * 24 * 60 * 60)
-
-    axis.plot(
-        c23energyrate["times"][1:],
-        dE / dt * 0.308,
-        color="grey",
-        linestyle="--",
-        zorder=20,
-        label=r"Collins+23 $\dot{E}_{rad,\beta^-}$",
-    )
+    # c23modelpath = Path(
+    #     Path.home(), "Google Drive/Shared drives/ARTIS/artis_runs_published/Collinsetal2023/sfho_long_1-35-135Msun"
+    # )
+
+    # c23energyrate = at.inputmodel.energyinputfiles.get_energy_rate_fromfile(c23modelpath)
+    # c23etot, c23energydistribution_data = at.inputmodel.energyinputfiles.get_etot_fromfile(c23modelpath)
+
+    # dE = np.diff(c23energyrate["rate"] * c23etot)
+    # dt = np.diff(c23energyrate["times"] * 24 * 60 * 60)
+
+    # axis.plot(
+    #     c23energyrate["times"][1:],
+    #     dE / dt * 0.308,
+    #     color="grey",
+    #     linestyle="--",
+    #     zorder=20,
+    #     label=r"Collins+23 $\dot{E}_{rad,\beta^-}$",
+    # )
 
     # color_alpha = next(axis._get_lines.prop_cycler)['color']
     color_alpha = "C1"
 
-    # if 'eps_alpha_ana_Lsun' in depdata:
-    #     axis.plot(depdata['tmid_days'], depdata['eps_alpha_ana_Lsun'] * 3.826e33, **dict(
-    #         plotkwargs, **{
-    #             'label': plotkwargs['label'] + r' $\dot{E}_{rad,\alpha}$ analytical',
-    #             'linestyle': 'solid',
-    #             'color': color_alpha,
-    #         }))
+    plotalphadep = False
+    if plotalphadep:
+        if "eps_alpha_ana_Lsun" in depdata:
+            axis.plot(
+                depdata["tmid_days"],
+                depdata["eps_alpha_ana_Lsun"] * 3.826e33,
+                **{
+                    **plotkwargs,
+                    "label": plotkwargs["label"] + r" $\dot{E}_{rad,\alpha}$ analytical",
+                    "linestyle": "solid",
+                    "color": color_alpha,
+                },
+            )
 
-    # if 'eps_alpha_Lsun' in depdata:
-    #     axis.plot(depdata['tmid_days'], depdata['eps_alpha_Lsun'] * 3.826e33, **dict(
-    #         plotkwargs, **{
-    #             'label': plotkwargs['label'] + r' $\dot{E}_{rad,\alpha}$',
-    #             'linestyle': 'dashed',
-    #             'color': color_alpha,
-    #         }))
+        if "eps_alpha_Lsun" in depdata:
+            axis.plot(
+                depdata["tmid_days"],
+                depdata["eps_alpha_Lsun"] * 3.826e33,
+                **{
+                    **plotkwargs,
+                    "label": plotkwargs["label"] + r" $\dot{E}_{rad,\alpha}$",
+                    "linestyle": "dashed",
+                    "color": color_alpha,
+                },
+            )
+
+        axis.plot(
+            depdata["tmid_days"],
+            depdata["alphadep_Lsun"] * 3.826e33,
+            **{
+                **plotkwargs,
+                "label": plotkwargs["label"] + r" $\dot{E}_{dep,\alpha}$",
+                "linestyle": "dotted",
+                "color": color_alpha,
+            },
+        )
 
-    # axis.plot(depdata['tmid_days'], depdata['alphadep_Lsun'] * 3.826e33, **dict(
-    #     plotkwargs, **{
-    #         'label': plotkwargs['label'] + r' $\dot{E}_{dep,\alpha}$',
-    #         'linestyle': 'dotted',
-    #         'color': color_alpha,
-    #     }))
     if args.plotthermalisation:
         axistherm.plot(
             depdata["tmid_days"],
             depdata["gammadep_Lsun"] / depdata["eps_gamma_Lsun"],
             **{**plotkwargs, "label": modelname + r" $f_\gamma$", "linestyle": "solid", "color": color_gamma},
         )
 
@@ -246,27 +257,28 @@
             depdata["tmid_days"],
             barnes_f_alpha,
             **{**plotkwargs, "label": r"Barnes+16 $f_\alpha$", "linestyle": "dashed", "color": color_alpha},
         )
 
 
 def plot_artis_lightcurve(
-    modelpath: Union[str, Path],
+    modelpath: str | Path,
     axis,
     lcindex: int = 0,
-    label: Optional[str] = None,
-    escape_type: Literal["TYPE_RPKT", "TYPE_GAMMA"] = "TYPE_RPKT",
+    label: str | None = None,
+    escape_type: t.Literal["TYPE_RPKT", "TYPE_GAMMA"] = "TYPE_RPKT",
     frompackets: bool = False,
-    maxpacketfiles: Optional[int] = None,
+    maxpacketfiles: int | None = None,
     axistherm=None,
-    directionbins: Optional[Sequence[int]] = None,
+    directionbins: t.Sequence[int] | None = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
+    usedegrees: bool = False,
     args=None,
-) -> Optional[pd.DataFrame]:
+) -> pd.DataFrame | None:
     lcfilename = None
     modelpath = Path(modelpath)
     if Path(modelpath).is_file():  # handle e.g. modelpath = 'modelpath/light_curve.out'
         lcfilename = Path(modelpath).parts[-1]
         modelpath = Path(modelpath).parent
 
     if not modelpath.is_dir():
@@ -316,28 +328,29 @@
 
         if average_over_phi:
             lcdataframes = at.average_direction_bins(lcdataframes, overangle="phi")
 
         if average_over_theta:
             lcdataframes = at.average_direction_bins(lcdataframes, overangle="theta")
 
-    plotkwargs: dict[str, Any] = {}
-    plotkwargs["label"] = modelname
-    plotkwargs["linestyle"] = args.linestyle[lcindex]
-    plotkwargs["color"] = args.color[lcindex]
+    plotkwargs: dict[str, t.Any] = {
+        "label": modelname,
+        "linestyle": args.linestyle[lcindex],
+        "color": args.color[lcindex],
+    }
     if args.dashes[lcindex]:
         plotkwargs["dashes"] = args.dashes[lcindex]
     if args.linewidth[lcindex]:
         plotkwargs["linewidth"] = args.linewidth[lcindex]
 
     # check if doing viewing angle stuff, and if so define which data to use
     dirbins, angle_definition = at.lightcurve.parse_directionbin_args(modelpath, args)
 
     if args.colorbarcostheta or args.colorbarphi:
-        costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels()
+        costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels(usedegrees=usedegrees)
         scaledmap = make_colorbar_viewingangles_colormap()
 
     lctimemin, lctimemax = float(lcdataframes[dirbins[0]]["time"].to_numpy().min()), float(
         lcdataframes[dirbins[0]]["time"].to_numpy().max()
     )
 
     print(f" range of light curve: {lctimemin:.2f} to {lctimemax:.2f} days")
@@ -445,36 +458,37 @@
     if args.plotdeposition or args.plotthermalisation:
         plot_deposition_thermalisation(axis, axistherm, modelpath, modelname, plotkwargs, args)
 
     return lcdataframes
 
 
 def make_lightcurve_plot(
-    modelpaths: Sequence[Union[str, Path]],
+    modelpaths: t.Sequence[str | Path],
     filenameout: str,
     frompackets: bool = False,
-    escape_type: Literal["TYPE_RPKT", "TYPE_GAMMA"] = "TYPE_RPKT",
-    maxpacketfiles: Optional[int] = None,
+    escape_type: t.Literal["TYPE_RPKT", "TYPE_GAMMA"] = "TYPE_RPKT",
+    maxpacketfiles: int | None = None,
     args=None,
 ):
     """Use light_curve.out or light_curve_res.out files to plot light curve."""
+    conffigwidth = float(at.get_config()["figwidth"])
     fig, axis = plt.subplots(
         nrows=1,
         ncols=1,
         sharex=True,
-        figsize=(args.figscale * at.get_config()["figwidth"] * 1.6, args.figscale * at.get_config()["figwidth"]),
+        figsize=(args.figscale * conffigwidth, args.figscale * conffigwidth / 1.6),
         tight_layout={"pad": 0.2, "w_pad": 0.0, "h_pad": 0.0},
     )
 
     if args.plotthermalisation:
         figtherm, axistherm = plt.subplots(
             nrows=1,
             ncols=1,
             sharex=True,
-            figsize=(args.figscale * at.get_config()["figwidth"] * 1.6, args.figscale * at.get_config()["figwidth"]),
+            figsize=(args.figscale * conffigwidth, args.figscale * conffigwidth / 1.6),
             tight_layout={"pad": 0.2, "w_pad": 0.0, "h_pad": 0.0},
         )
     else:
         axistherm = None
 
     # take any assigned colours our of the cycle
     colors = [
@@ -485,15 +499,15 @@
 
     plottedsomething = False
     for lcindex, modelpath in enumerate(modelpaths):
         if not Path(modelpath).is_dir() and not Path(modelpath).exists() and "." in str(modelpath):
             bolreflightcurve = Path(modelpath)
 
             dflightcurve, metadata = at.lightcurve.read_bol_reflightcurve_data(bolreflightcurve)
-            lightcurvelabel = metadata.get("label", bolreflightcurve)
+            lightcurvelabel = args.label[lcindex] or metadata.get("label", bolreflightcurve)
             color = ["0.0", "0.5", "0.7"][reflightcurveindex]
             plotkwargs = {"label": lightcurvelabel, "color": color, "zorder": 0}
             if (
                 "luminosity_errminus_erg/s" in dflightcurve.columns
                 and "luminosity_errplus_erg/s" in dflightcurve.columns
             ):
                 axis.errorbar(
@@ -518,14 +532,15 @@
                 escape_type=escape_type,
                 frompackets=frompackets,
                 maxpacketfiles=maxpacketfiles,
                 axistherm=axistherm,
                 directionbins=args.plotviewingangle if args.plotviewingangle is not None else [-1],
                 average_over_phi=args.average_over_phi_angle,
                 average_over_theta=args.average_over_theta_angle,
+                usedegrees=args.usedegrees,
                 args=args,
             )
             plottedsomething = plottedsomething or (lcdataframes is not None)
 
     if args.reflightcurves:
         for bolreflightcurve in args.reflightcurves:
             if args.Lsun:
@@ -561,27 +576,29 @@
             axistherm.legend(loc="best", handlelength=2, frameon=args.legendframeon, numpoints=1, prop={"size": 9})
 
     axis.set_xlabel(r"Time [days]")
 
     if args.magnitude:
         axis.set_ylabel("Absolute Bolometric Magnitude")
     else:
-        str_units = " [erg/s]" if not args.Lsun else "$/ \\mathrm{L}_\\odot$"
+        str_units = "$/ \\mathrm{L}_\\odot$" if args.Lsun else " [erg/s]"
         if args.plotdeposition:
-            yvarname = ""
+            yvarname = r"$L$ or $\dot{E}$"
         elif escape_type == "TYPE_GAMMA":
             yvarname = r"$\mathrm{L}_\gamma$"
         elif escape_type == "TYPE_RPKT":
             yvarname = r"$\mathrm{L}_{\mathrm{UVOIR}}$"
         else:
             yvarname = r"$\mathrm{L}_{\mathrm{" + escape_type.replace("_", r"\_") + r"}}$"
         axis.set_ylabel(yvarname + str_units)
 
     if args.colorbarcostheta or args.colorbarphi:
-        costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels()
+        costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels(
+            usedegrees=args.usedegrees
+        )
         scaledmap = make_colorbar_viewingangles_colormap()
         make_colorbar_viewingangles(phi_viewing_angle_bins, scaledmap, args)
 
     if args.logscalex:
         axis.set_xscale("log")
 
     if args.logscaley:
@@ -614,21 +631,21 @@
 
 
 def create_axes(args):
     if "labelfontsize" in args:
         font = {"size": args.labelfontsize}
         mpl.rc("font", **font)
 
-    args.subplots = False  # todo: set as command line arg
+    args.subplots = False  # TODO: set as command line arg
 
-    if (args.filter and len(args.filter) > 1) or args.subplots is True:
+    if (args.filter and len(args.filter) > 1) or args.subplots:
         args.subplots = True
         rows = 2
         cols = 3
-    elif (args.colour_evolution and len(args.colour_evolution) > 1) or args.subplots is True:
+    elif args.colour_evolution and len(args.colour_evolution) > 1:
         args.subplots = True
         rows = 1
         cols = 3
     else:
         args.subplots = False
         rows = 1
         cols = 1
@@ -652,16 +669,16 @@
     return fig, ax
 
 
 def get_linelabel(
     modelpath: Path,
     modelname: str,
     modelnumber: int,
-    angle: Optional[int],
-    angle_definition: Optional[dict[int, str]],
+    angle: int | None,
+    angle_definition: dict[int, str] | None,
     args,
 ) -> str:
     if angle is not None and angle != -1:
         assert angle_definition is not None
         linelabel = f"{angle_definition[angle]}" if args.nomodelname else f"{modelname} {angle_definition[angle]}"
         # linelabel = None
         # linelabel = fr"{modelname} $\theta$ = {angle_names[index]}$^\circ$"
@@ -789,21 +806,23 @@
         cbar.update_ticks()
 
 
 def make_band_lightcurves_plot(modelpaths, filternames_conversion_dict, outputfolder, args: argparse.Namespace) -> None:
     # angle_names = [0, 45, 90, 180]
     # plt.style.use('dark_background')
 
-    args.labelfontsize = 22  # todo: make command line arg
+    args.labelfontsize = 22  # TODO: make command line arg
     fig, ax = create_axes(args)
 
-    plotkwargs: dict[str, Any] = {}
+    plotkwargs: dict[str, t.Any] = {}
 
     if args.colorbarcostheta or args.colorbarphi:
-        costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels()
+        costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels(
+            usedegrees=args.usedegrees
+        )
         scaledmap = make_colorbar_viewingangles_colormap()
 
     first_band_name = None
     for modelnumber, modelpath in enumerate(modelpaths):
         modelpath = Path(modelpath)  # Make sure modelpath is defined as path. May not be necessary
 
         # check if doing viewing angle stuff, and if so define which data to use
@@ -812,56 +831,54 @@
         for index, angle in enumerate(angles):
             modelname = at.get_model_name(modelpath)
             print(f"Reading spectra: {modelname} (angle {angle})")
             band_lightcurve_data = at.lightcurve.generate_band_lightcurve_data(
                 modelpath, args, angle, modelnumber=modelnumber
             )
 
-            if modelnumber == 0 and args.plot_hesma_model:  # Todo: does this work?
+            if modelnumber == 0 and args.plot_hesma_model:  # TODO: does this work?
                 hesma_model = at.lightcurve.read_hesma_lightcurve(args)
                 plotkwargs["label"] = str(args.plot_hesma_model).split("_")[:3]
 
             for plotnumber, band_name in enumerate(band_lightcurve_data):
                 if first_band_name is None:
                     first_band_name = band_name
                 time, brightness_in_mag = at.lightcurve.get_band_lightcurve(band_lightcurve_data, band_name, args)
 
                 if args.print_data or args.write_data:
-                    txtlinesout = []
-                    txtlinesout.append(f"# band: {band_name}")
-                    txtlinesout.append(f"# model: {modelname}")
-                    txtlinesout.append("# time_days magnitude")
-                    for t, m in zip(time, brightness_in_mag):
-                        txtlinesout.append(f"{t} {m}")
+                    txtlinesout = [
+                        f"# band: {band_name}",
+                        f"# model: {modelname}",
+                        "# time_days magnitude",
+                    ]
+                    txtlinesout.extend(f"{t_d} {m}" for t_d, m in zip(time, brightness_in_mag))
                     txtout = "\n".join(txtlinesout)
-                    if args.write_data:
-                        bandoutfile = (
-                            Path(f"band_{band_name}_angle_{angle}.txt")
-                            if angle != -1
-                            else Path(f"band_{band_name}.txt")
-                        )
-                        with bandoutfile.open("w") as f:
-                            f.write(txtout)
-                        print(f"Saved {bandoutfile}")
-                    if args.print_data:
-                        print(txtout)
+                if args.write_data:
+                    bandoutfile = (
+                        Path(f"band_{band_name}_angle_{angle}.txt") if angle != -1 else Path(f"band_{band_name}.txt")
+                    )
+                    with bandoutfile.open("w") as f:
+                        f.write(txtout)
+                    print(f"Saved {bandoutfile}")
+                if args.print_data:
+                    print(txtout)
 
                 plotkwargs["label"] = get_linelabel(modelpath, modelname, modelnumber, angle, angle_definition, args)
-                # plotkwargs['label'] = '\n'.join(wrap(linelabel, 40))  # todo: could be arg? wraps text in label
+                # plotkwargs['label'] = '\n'.join(wrap(linelabel, 40))  # TODO: could be arg? wraps text in label
 
                 filterfunc = at.get_filterfunc(args)
                 if filterfunc is not None:
                     brightness_in_mag = filterfunc(brightness_in_mag)
 
                 # This does the same thing as below -- leaving code in case I'm wrong (CC)
                 # if args.plotviewingangle and args.plotviewingangles_lightcurves:
                 #     global define_colours_list
                 #     plt.plot(time, brightness_in_mag, label=modelname, color=define_colours_list[angle], linewidth=3)
 
-                if modelnumber == 0 and args.plot_hesma_model and band_name in hesma_model:  # todo: see if this works
+                if modelnumber == 0 and args.plot_hesma_model and band_name in hesma_model:  # TODO: see if this works
                     ax.plot(hesma_model.t, hesma_model[band_name], color="black")
 
                 # axarr[plotnumber].axis([0, 60, -16, -19.5])
                 text_key = (
                     filternames_conversion_dict[band_name] if band_name in filternames_conversion_dict else band_name
                 )
 
@@ -917,15 +934,15 @@
 
                 if args.linestyle:
                     plotkwargs["linestyle"] = args.linestyle[modelnumber]
 
                 # if not (args.test_viewing_angle_fit or args.calculate_peak_time_mag_deltam15_bool):
                 curax = ax[plotnumber] if args.subplots else ax
                 if args.subplots:
-                    if len(angles) > 1 or (args.plotviewingangle and os.path.isfile(modelpath / "specpol_res.out")):
+                    if len(angles) > 1 or (args.plotviewingangle and (modelpath / "specpol_res.out").is_file()):
                         ax[plotnumber].plot(time, brightness_in_mag, linewidth=4, **plotkwargs)
                     # I think this was just to have a different line style for viewing angles....
                     else:
                         ax[plotnumber].plot(time, brightness_in_mag, linewidth=4, **plotkwargs)
                         # if key is not 'bol':
                         #     ax[plotnumber].plot(
                         #         cmfgen_mags['time[d]'], cmfgen_mags[key], label='CMFGEN', color='k', linewidth=3)
@@ -940,15 +957,15 @@
     fig, ax = set_lightcurve_plot_labels(fig, ax, filternames_conversion_dict, args, band_name=first_band_name)
     set_lightcurveplot_legend(ax, args)
 
     if args.colorbarcostheta or args.colorbarphi:
         make_colorbar_viewingangles(phi_viewing_angle_bins, scaledmap, args, fig=fig, ax=ax)
 
     if args.filter and len(band_lightcurve_data) == 1:
-        args.outputfile = os.path.join(outputfolder, f"plot{first_band_name}lightcurves.pdf")
+        args.outputfile = Path(outputfolder, f"plot{first_band_name}lightcurves.pdf")
     if args.show:
         plt.show()
 
     (ax[0] if args.subplots else ax).invert_yaxis()
 
     plt.savefig(args.outputfile, format="pdf")
     print(f"Saved figure: {args.outputfile}")
@@ -980,15 +997,15 @@
 #         markers = args.refspecmarkers
 #         for i, reflightcurve in enumerate(args.reflightcurves):
 #             plot_lightcurve_from_refdata(filters_dict.keys(), reflightcurve, colours[i], markers[i],
 #                                       filternames_conversion_dict)
 
 
 def colour_evolution_plot(modelpaths, filternames_conversion_dict, outputfolder, args):
-    args.labelfontsize = 24  # todo: make command line arg
+    args.labelfontsize = 24  # TODO: make command line arg
     angle_counter = 0
 
     fig, ax = create_axes(args)
 
     plotkwargs = {}
 
     for modelnumber, modelpath in enumerate(modelpaths):
@@ -1017,15 +1034,15 @@
                 if args.color and args.plotviewingangle:
                     print(
                         "WARNING: -color argument will not work with viewing angles for colour evolution plots,"
                         "colours are taken from color_list array instead"
                     )
                     # plotkwargs["color"] = color_list[angle_counter]  # index instaed of angle_counter??
                     angle_counter += 1
-                elif args.plotviewingangle and not args.color:
+                elif args.plotviewingangle:
                     plotkwargs["color"] = color_list[angle_counter]
                     angle_counter += 1
                 elif args.color:
                     plotkwargs["color"] = args.color[modelnumber]
                 if args.linestyle:
                     plotkwargs["linestyle"] = args.linestyle[modelnumber]
 
@@ -1059,28 +1076,28 @@
                     textcoords="offset points",
                     xytext=(-30, -30),
                     horizontalalignment="right",
                     verticalalignment="top",
                     fontsize="x-large",
                 )
 
-        # UNCOMMENT TO ESTIMATE COLOUR AT TIME B MAX
-        # def match_closest_time(reftime):
-        #     return ("{}".format(min([float(x) for x in plot_times], key=lambda x: abs(x - reftime))))
-        #
-        # tmax_B = 17.0  # CHANGE TO TIME OF B MAX
-        # tmax_B = float(match_closest_time(tmax_B))
-        # print(f'{filter_names[0]} - {filter_names[1]} at t_Bmax ({tmax_B}) = '
-        #       f'{diff[plot_times.index(tmax_B)]}')
+            # UNCOMMENT TO ESTIMATE COLOUR AT TIME B MAX
+            # def match_closest_time(reftime):
+            #     return ("{}".format(min([float(x) for x in plot_times], key=lambda x: abs(x - reftime))))
+            #
+            # tmax_B = 17.0  # CHANGE TO TIME OF B MAX
+            # tmax_B = float(match_closest_time(tmax_B))
+            # print(f'{filter_names[0]} - {filter_names[1]} at t_Bmax ({tmax_B}) = '
+            #       f'{diff[plot_times.index(tmax_B)]}')
 
     fig, ax = set_lightcurve_plot_labels(fig, ax, filternames_conversion_dict, args)
     ax = at.plottools.set_axis_properties(ax, args)
     set_lightcurveplot_legend(ax, args)
 
-    args.outputfile = os.path.join(outputfolder, f"plotcolorevolution{filter_names[0]}-{filter_names[1]}.pdf")
+    args.outputfile = Path(outputfolder, f"plotcolorevolution{filter_names[0]}-{filter_names[1]}.pdf")
     for i in range(2):
         if filter_names[i] in filternames_conversion_dict:
             filter_names[i] = filternames_conversion_dict[filter_names[i]]
     # plt.text(10, args.ymax - 0.5, f'{filter_names[0]}-{filter_names[1]}', fontsize='x-large')
 
     if args.show:
         plt.show()
@@ -1102,21 +1119,21 @@
 
 
 def plot_lightcurve_from_refdata(
     filter_names, lightcurvefilename, color, marker, filternames_conversion_dict, ax, plotnumber
 ):
     lightcurve_data, metadata = at.lightcurve.read_reflightcurve_band_data(lightcurvefilename)
     linename = metadata["label"] if plotnumber == 0 else None
-    filterdir = os.path.join(at.get_config()["path_artistools_dir"], "data/filters/")
+    filterdir = Path(at.get_config()["path_artistools_dir"], "data/filters/")
 
     filter_data = {}
     for plotnumber, filter_name in enumerate(filter_names):
         if filter_name == "bol":
             continue
-        f = filterdir / Path(f"{filter_name}.txt").open()
+        f = Path(filterdir / f"{filter_name}.txt").open()
         lines = f.readlines()
         lambda0 = float(lines[2])
 
         if filter_name == "bol":
             continue
         if filter_name in filternames_conversion_dict:
             filter_name = filternames_conversion_dict[filter_name]
@@ -1182,15 +1199,15 @@
     return linename
 
 
 def plot_color_evolution_from_data(
     filter_names, lightcurvefilename, color, marker, filternames_conversion_dict, ax, plotnumber, args
 ):
     lightcurve_from_data, metadata = at.lightcurve.read_reflightcurve_band_data(lightcurvefilename)
-    filterdir = os.path.join(at.get_config()["path_artistools_dir"], "data/filters/")
+    filterdir = Path(at.get_config()["path_artistools_dir"], "data/filters/")
 
     filter_data = []
     for i, filter_name in enumerate(filter_names):
         f = filterdir / Path(f"{filter_name}.txt").open()
         lines = f.readlines()
         lambda0 = float(lines[2])
 
@@ -1267,15 +1284,15 @@
     parser.add_argument("-linestyle", default=[], nargs="*", help="List of line styles")
 
     parser.add_argument("-linewidth", default=[], nargs="*", help="List of line widths")
 
     parser.add_argument("-dashes", default=[], nargs="*", help="Dashes property of lines")
 
     parser.add_argument(
-        "-figscale", type=float, default=1.0, help="Scale factor for plot area. 1.0 is for single-column"
+        "-figscale", type=float, default=1.6, help="Scale factor for plot area. 1.0 is for single-column"
     )
 
     parser.add_argument("--frompackets", action="store_true", help="Read packets files instead of light_curve.out")
 
     parser.add_argument("-maxpacketfiles", type=int, default=None, help="Limit the number of packet files read")
 
     parser.add_argument("--gamma", action="store_true", help="Make light curve from gamma rays instead of R-packets")
@@ -1344,14 +1361,19 @@
         type=int,
         nargs="+",
         help=(
             "Plot viewing angles. Expects int for angle number in specpol_res.out"
             "use args = -1 to select all the viewing angles"
         ),
     )
+    parser.add_argument(
+        "--usedegrees",
+        action="store_true",
+        help="Use degrees instead of radians for viewing angles. Only works with -plotviewingangle",
+    )
 
     parser.add_argument("-ymax", type=float, default=None, help="Plot range: y-axis")
 
     parser.add_argument("-ymin", type=float, default=None, help="Plot range: y-axis")
 
     parser.add_argument("-xmax", type=float, default=None, help="Plot range: x-axis")
 
@@ -1464,20 +1486,14 @@
     )
 
     parser.add_argument(
         "--noangleaveraged", action="store_true", help="Don't plot angle averaged values on viewing angle scatter plots"
     )
 
     parser.add_argument(
-        "--plotviewingangles_lightcurves",
-        action="store_true",
-        help="Make lightcurve plots for the viewing angles and models specified",
-    )
-
-    parser.add_argument(
         "--average_over_phi_angle",
         action="store_true",
         help="Average over phi (azimuthal) viewing angles to make direction bins into polar angle bins",
     )
 
     # for backwards compatibility with above option
     parser.add_argument(
```

### Comparing `artistools-2023.5.16.3/artistools/lightcurve/test_lightcurve.py` & `artistools-2023.8.1/artistools/lightcurve/test_lightcurve.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/lightcurve/viewingangleanalysis.py` & `artistools-2023.8.1/artistools/lightcurve/viewingangleanalysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
+from __future__ import annotations
+
 import argparse
-import glob
-import os
 import sys
-from collections.abc import Sequence
+import typing as t
 from pathlib import Path
-from typing import Any
-from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from astropy import constants as const
 from matplotlib.legend_handler import HandlerTuple
+from typeguard import typechecked
 
 import artistools as at
 
 define_colours_list = [
     "k",
     "tab:blue",
     "tab:red",
@@ -143,25 +142,23 @@
     "r",
     "deeppink",
     "sandybrown",
     "teal",
 ]
 
 
-def parse_directionbin_args(modelpath: Union[Path, str], args) -> tuple[Sequence[int], dict[int, str]]:
+@typechecked
+def parse_directionbin_args(modelpath: Path | str, args: argparse.Namespace) -> tuple[t.Sequence[int], dict[int, str]]:
     modelpath = Path(modelpath)
-    viewing_angle_data = False
-    if len(glob.glob(str(modelpath / "*_res.out*"))) >= 1:
-        viewing_angle_data = True
-
-    if args.plotvspecpol and os.path.isfile(modelpath / "vpkt.txt"):
+    viewing_angle_data_exists = bool(list(modelpath.glob("*_res.out*")))
+    if args.plotvspecpol and (modelpath / "vpkt.txt").is_file():
         dirbins = args.plotvspecpol
-    elif args.plotviewingangle and args.plotviewingangle[0] == -1 and viewing_angle_data:
+    elif args.plotviewingangle and args.plotviewingangle[0] == -1 and viewing_angle_data_exists:
         dirbins = np.arange(0, 100, 1, dtype=int)
-    elif args.plotviewingangle and viewing_angle_data:
+    elif args.plotviewingangle and viewing_angle_data_exists:
         dirbins = args.plotviewingangle
     elif (
         args.calculate_costheta_phi_from_viewing_angle_numbers
         and args.calculate_costheta_phi_from_viewing_angle_numbers[0] == -1
     ):
         viewing_angles = np.arange(0, 100, 1, dtype=int)
     elif args.calculate_costheta_phi_from_viewing_angle_numbers:
@@ -176,14 +173,15 @@
         dirbin_definition = at.get_vspec_dir_labels(modelpath=modelpath)
     else:
         dirbin_definition = at.get_dirbin_labels(
             dirbins=dirbins,
             modelpath=modelpath,
             average_over_phi=args.average_over_phi_angle,
             average_over_theta=args.average_over_theta_angle,
+            usedegrees=args.usedegrees,
         )
 
         if args.average_over_phi_angle:
             for dirbin in dirbin_definition:
                 assert dirbin % at.get_viewingdirection_phibincount() == 0 or dirbin == -1
 
         if args.average_over_theta_angle:
@@ -283,15 +281,15 @@
         "The --test_viewing_angle_fit flag will allow you to check the fitting is "
         "behaving as expected. In general fitting over a smaller region of the    "
         "light curve tends to produce better fits."
     )
     fxfit, xfit = lightcurve_polyfit(time, magnitude, args)
 
     def match_closest_time_polyfit(reftime_polyfit):
-        return str(f"{min([float(x) for x in xfit], key=lambda x: abs(x - reftime_polyfit))}")
+        return str(f"{min((float(x) for x in xfit), key=lambda x: abs(x - reftime_polyfit))}")
 
     index_min = np.argmin(fxfit)
     tmax_polyfit = xfit[index_min]
     time_after15days_polyfit = match_closest_time_polyfit(tmax_polyfit + 15)
     if args.include_delta_m40:
         time_after40days_polyfit = match_closest_time_polyfit(tmax_polyfit + 40)
     for ii, xfits in enumerate(xfit):
@@ -393,15 +391,15 @@
     key,
     mag_after15days_polyfit,
     tmax_polyfit,
     time_after15days_polyfit,
     modelname,
     angle,
     args,
-) -> None:
+):
     plt.plot(time, magnitude)
     plt.plot(xfit, fxfit)
 
     if key in filternames_conversion_dict:
         plt.ylabel(f"{filternames_conversion_dict[key]} Magnitude")
     else:
         plt.ylabel(f"{key} Magnitude")
@@ -414,50 +412,44 @@
     plt.tick_params(axis="both", which="major", top=True, right=True, length=8, width=2, labelsize=12)
     plt.axhline(y=min(fxfit), color="black", linestyle="--")
     plt.axhline(y=mag_after15days_polyfit, color="black", linestyle="--")
     plt.axvline(x=tmax_polyfit, color="black", linestyle="--")
     plt.axvline(x=float(time_after15days_polyfit), color="black", linestyle="--")
     print("time after 15 days polyfit = ", time_after15days_polyfit)
     plt.tight_layout()
-    plt.savefig(f"{key}_band_{modelname}_viewing_angle" + str(angle) + ".png")
+    plt.savefig(f"{key}_band_{modelname}_viewing_angle{angle!s}.png")
     plt.close()
 
 
 def set_scatterplot_plotkwargs(modelnumber, args):
-    plotkwargsviewingangles = {}
-    plotkwargsviewingangles["marker"] = "x"
-    plotkwargsviewingangles["zorder"] = 0
-    plotkwargsviewingangles["alpha"] = 0.8
+    plotkwargsviewingangles = {"marker": "x", "zorder": 0, "alpha": 0.8}
     if args.colorbarcostheta or args.colorbarphi:
         update_plotkwargs_for_viewingangle_colorbar(plotkwargsviewingangles, args)
     elif args.color:
         plotkwargsviewingangles["color"] = args.color[modelnumber]
     else:
         plotkwargsviewingangles["color"] = define_colours_list2[modelnumber]
 
-    plotkwargsangleaveraged = {}
-    plotkwargsangleaveraged["marker"] = "o"
-    plotkwargsangleaveraged["zorder"] = 10
-    plotkwargsangleaveraged["edgecolor"] = "k"
-    plotkwargsangleaveraged["s"] = 120
-    if args.color:
-        plotkwargsangleaveraged["color"] = args.color[modelnumber]
-    else:
-        plotkwargsangleaveraged["color"] = define_colours_list[modelnumber]
-
+    plotkwargsangleaveraged = {
+        "marker": "o",
+        "zorder": 10,
+        "edgecolor": "k",
+        "s": 120,
+        "color": args.color[modelnumber] if args.color else define_colours_list[modelnumber],
+    }
     if args.colorbarcostheta or args.colorbarphi:
         update_plotkwargs_for_viewingangle_colorbar(plotkwargsviewingangles, args)
 
     return plotkwargsviewingangles, plotkwargsangleaveraged
 
 
 def update_plotkwargs_for_viewingangle_colorbar(
-    plotkwargsviewingangles: dict[str, Any], args: argparse.Namespace
-) -> dict[str, Any]:
-    costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels()
+    plotkwargsviewingangles: dict[str, t.Any], args: argparse.Namespace
+) -> dict[str, t.Any]:
+    costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels(usedegrees=args.usedegrees)
     scaledmap = at.lightcurve.plotlightcurve.make_colorbar_viewingangles_colormap()
 
     angles = np.arange(0, at.get_viewingdirectionbincount())
     colors = []
     for angle in angles:
         _, colorindex = at.lightcurve.plotlightcurve.get_viewinganglecolor_for_colorbar(
             angle,
@@ -479,15 +471,17 @@
     plt.ylim(args.ymin, args.ymax)
     plt.minorticks_on()
     plt.tick_params(axis="both", which="minor", top=False, right=False, length=5, width=2, labelsize=12)
     plt.tick_params(axis="both", which="major", top=False, right=False, length=8, width=2, labelsize=12)
     plt.tight_layout()
 
     if args.colorbarcostheta or args.colorbarphi:
-        costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels()
+        costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels(
+            usedegrees=args.usedegrees
+        )
         scaledmap = at.lightcurve.plotlightcurve.make_colorbar_viewingangles_colormap()
         at.lightcurve.plotlightcurve.make_colorbar_viewingangles(phi_viewing_angle_bins, scaledmap, args)
 
 
 # COMBINED WITH DM15 plotting function now ###
 # def make_viewing_angle_peakmag_risetime_scatter_plot(modelnames, key, args):
 #     for ii, modelname in enumerate(modelnames):
@@ -559,26 +553,26 @@
             p0 = ax.scatter(
                 xvalues_angleaveraged, args.band_peakmag_angle_averaged_polyfit[ii], **plotkwargsangleaveraged
             )
             args.plotvalues.append((a0, p0))
         else:
             args.plotvalues.append((a0, a0))
         if not args.noerrorbars:
-            ecolor = args.color if args.color else define_colours_list
+            ecolor = args.color or define_colours_list
 
             ax.errorbar(
                 xvalues_angleaveraged,
                 args.band_peakmag_angle_averaged_polyfit[ii],
                 xerr=np.std(xvalues_viewingangles),
                 yerr=np.std(band_peak_mag_viewing_angles),
                 ecolor=ecolor[ii],
                 capsize=2,
             )
 
-    linelabels = args.label if args.label else modelnames
+    linelabels = args.label or modelnames
 
     # a0, datalabel = at.lightcurve.get_sn_sample_bol()
     # a0, datalabel = at.lightcurve.plot_phillips_relation_data()
     # args.plotvalues.append((a0, a0))
     # linelabels.append(datalabel)
 
     if not args.nolegend:
@@ -592,15 +586,15 @@
             ncol=args.ncolslegend,
             columnspacing=1,
             frameon=False,
         )
     # ax.set_xlabel(r'Decline Rate ($\Delta$m$_{15}$)', fontsize=14)
 
     if args.make_viewing_angle_peakmag_delta_m15_scatter_plot:
-        xlabel = rf"$\Delta$m$_{15}$({key})"
+        xlabel = rf"$\Delta$m$_{{15}}$({key})"
     if args.make_viewing_angle_peakmag_risetime_scatter_plot:
         xlabel = "Rise Time [days]"
 
     ax.set_xlabel(xlabel, fontsize=14)
     # ax.set_ylabel('Peak ' + key + ' Band Magnitude', fontsize=14)
     ax.set_ylabel(rf"M$_{{\mathrm{{{key}}}}}$, max", fontsize=14)
     set_scatterplot_plot_params(args)
@@ -620,19 +614,17 @@
     )
 
     for modelnumber, modelpath in enumerate(args.modelpath):
         modelname = at.get_model_name(modelpath)
 
         bands = [args.filter[0], args.filter[1]]
 
-        data = {}
-
         datafilename = bands[0] + "band_" + f"{modelname}" + "_viewing_angle_data.txt"
         viewing_angle_plot_data = pd.read_csv(datafilename, delimiter=" ")
-        data[f"{bands[0]}max"] = viewing_angle_plot_data["peak_mag_polyfit"].to_numpy()
+        data = {f"{bands[0]}max": viewing_angle_plot_data["peak_mag_polyfit"].to_numpy()}
         data[f"time_{bands[0]}max"] = viewing_angle_plot_data["risetime_polyfit"].to_numpy()
 
         # Get brightness in second band at time of peak in first band
         if len(data[f"time_{bands[0]}max"]) != 100:
             print(f"All 100 angles are not in file {datafilename}. Quitting")
             sys.exit(1)
 
@@ -792,15 +784,15 @@
 def plot_viewanglebrightness_at_fixed_time(modelpath, args):
     fig, axis = plt.subplots(
         nrows=1, ncols=1, sharey=True, figsize=(8, 5), tight_layout={"pad": 0.2, "w_pad": 0.0, "h_pad": 0.0}
     )
 
     angles, angle_definition = at.lightcurve.parse_directionbin_args(modelpath, args)
 
-    costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels()
+    costheta_viewing_angle_bins, phi_viewing_angle_bins = at.get_costhetabin_phibin_labels(usedegrees=args.usedegrees)
     scaledmap = at.lightcurve.plotlightcurve.make_colorbar_viewingangles_colormap()
 
     plotkwargs = {}
 
     lcdataframes = at.lightcurve.readfile(modelpath / "light_curve_res.out")
 
     timetoplot = at.match_closest_time(reftime=args.timedays, searchtimes=lcdataframes[0]["time"])
```

### Comparing `artistools-2023.5.16.3/artistools/lightcurve/writebollightcurvedata.py` & `artistools-2023.8.1/artistools/lightcurve/writebollightcurvedata.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,31 +38,27 @@
     lcfilename = "light_curve_res.out" if res else "light_curve.out"
     lcdata = pd.read_csv(modelpath / lcfilename, delim_whitespace=True, header=None, names=["time", "lum", "lum_cmf"])
     lcdataframes = at.split_dataframe_dirbins(lcdata, index_of_repeated_value=0)
 
     times = lcdataframes[0]["time"]
     lightcurvedata = {"time": times}
 
-    nangles = len(lcdataframes)
-    if not res:
-        nangles = 1
+    nangles = len(lcdataframes) if res else 1
     for angle in range(nangles):
         lcdata = lcdataframes[angle]
         bol_luminosity = np.array(lcdata["lum"]) * 3.826e33  # Luminosity in erg/s
 
         # lightcurvedata[f'angle={angle}'] = np.log10(bol_luminosity)
         columnname = "lum (erg/s)"
         if res:
             columnname = f"angle={angle}"
         lightcurvedata[columnname] = bol_luminosity
 
     lightcurvedataframe = pd.DataFrame(lightcurvedata)
-    lightcurvedataframe = lightcurvedataframe.replace([np.inf, -np.inf], 0)
-
-    return lightcurvedataframe
+    return lightcurvedataframe.replace([np.inf, -np.inf], 0)
 
 
 # modelnames = ['M08_03', 'M08_05', 'M08_10', 'M09_03', 'M09_05', 'M09_10',
 #               'M10_02_end55', 'M10_03', 'M10_05', 'M10_10', 'M11_05_1']
 modelnames = ["M2a"]
 
 for modelname in modelnames:
@@ -71,15 +67,15 @@
     outfilepath = Path("/Users/ccollins/Desktop/bollightcurvedata")
 
     # lightcurvedataframe = get_bol_lc_from_spec(modelpath)
     lightcurvedataframe = get_bol_lc_from_lightcurveout(modelpath)
 
     lightcurvedataframe.to_csv(outfilepath / f"bol_lightcurvedata_{modelname}.txt", sep=" ", index=False, header=False)
 
-    with open(outfilepath / f"bol_lightcurvedata_{modelname}.txt", "r+") as f:  # add comment to start of file
+    with (outfilepath / f"bol_lightcurvedata_{modelname}.txt").open("r+") as f:  # add comment to start of file
         content = f.read()
         f.seek(0, 0)
         f.write(
             "# 1st col is time in days. Next columns are log10(luminosity) for each model viewing angle".rstrip("\r\n")
             + "\n"
             + content
         )
```

### Comparing `artistools-2023.5.16.3/artistools/linefluxes.py` & `artistools-2023.8.1/artistools/linefluxes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,76 @@
 #!/usr/bin/env python3
 """Artistools - spectra related functions."""
+
+from __future__ import annotations
+
 import argparse
+import contextlib
 import json
 import math
 import multiprocessing
+import typing as t
 from collections import namedtuple
 from functools import partial
 from pathlib import Path
-from typing import Optional
-from typing import Union
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from astropy import units as u
 
 import artistools as at
 
 
-def get_packets_with_emtype_onefile(emtypecolumn, lineindices, packetsfile):
+def print_floers_line_ratio(
+    modelpath: Path, timedays: float, arr_f_lambda: np.ndarray, arr_lambda_angstroms: np.ndarray
+) -> None:
+    def get_line_flux(
+        lambda_low: float, lambda_high: float, arr_f_lambda: np.ndarray, arr_lambda_angstroms: np.ndarray
+    ) -> float:
+        index_low, index_high = (
+            int(np.searchsorted(arr_lambda_angstroms, wl, side="left")) for wl in (lambda_low, lambda_high)
+        )
+        return abs(
+            np.trapz(
+                arr_f_lambda[index_low:index_high],
+                x=arr_lambda_angstroms[index_low:index_high],
+            )
+        )
+
+    f_12570 = get_line_flux(12570 - 200, 12570 + 200, arr_f_lambda, arr_lambda_angstroms)
+    f_7155 = get_line_flux(7000, 7350, arr_f_lambda, arr_lambda_angstroms)
+    print(f"f_12570 {f_12570:.2e} f_7155 {f_7155:.2e}")
+    if f_7155 > 0 and f_12570 > 0:
+        fratio = f_12570 / f_7155
+        print(f"f_12570/f_7122 = {fratio:.2e} (log10 is {math.log10(fratio):.2e})")
+        outfilename = Path(f"fe2_nir_vis_ratio_{modelpath.name}.txt")
+        print(f" saved to {outfilename}")
+        with outfilename.open("a+") as f:
+            f.write(f"{timedays:.1f} {fratio:.3e}\n")
+
+
+def get_packets_with_emtype_onefile(
+    emtypecolumn: str, lineindices: t.Sequence[int], packetsfile: Path | str
+) -> pd.DataFrame:
     import gzip
 
     try:
         dfpackets = at.packets.readfile(packetsfile, packet_type="TYPE_ESCAPE", escape_type="TYPE_RPKT")
     except gzip.BadGzipFile as exc:
         print(f"Bad file: {packetsfile}")
         raise gzip.BadGzipFile from exc
 
     return dfpackets.query(f"{emtypecolumn} in @lineindices", inplace=False).copy()
 
 
-def get_packets_with_emtype(modelpath, emtypecolumn, lineindices, maxpacketfiles=None):
+def get_packets_with_emtype(
+    modelpath: Path | str, emtypecolumn: str, lineindices: t.Sequence[int], maxpacketfiles: int | None = None
+):
     packetsfiles = at.packets.get_packetsfilepaths(modelpath, maxpacketfiles=maxpacketfiles)
     nprocs_read = len(packetsfiles)
     assert nprocs_read > 0
 
     model, _ = at.inputmodel.get_modeldata(modelpath)
     # vmax = model.iloc[-1].velocity_outer * u.km / u.s
     processfile = partial(get_packets_with_emtype_onefile, emtypecolumn, lineindices)
@@ -64,30 +99,30 @@
     return binnedenergysums
 
 
 def get_line_fluxes_from_packets(
     emtypecolumn, emfeatures, modelpath, maxpacketfiles=None, arr_tstart=None, arr_tend=None
 ) -> pd.DataFrame:
     if arr_tstart is None:
-        arr_tstart = at.get_timestep_times_float(modelpath, loc="start")
+        arr_tstart = at.get_timestep_times(modelpath, loc="start")
     if arr_tend is None:
-        arr_tend = at.get_timestep_times_float(modelpath, loc="end")
+        arr_tend = at.get_timestep_times(modelpath, loc="end")
 
     arr_timedelta = np.array(arr_tend) - np.array(arr_tstart)
     arr_tmid = arr_tend = (np.array(arr_tstart) + np.array(arr_tend)) / 2.0
 
     model, _ = at.inputmodel.get_modeldata(modelpath)
     # vmax = model.iloc[-1].velocity_outer * u.km / u.s
     # betafactor = math.sqrt(1 - (vmax / const.c).decompose().value ** 2)
 
     timearrayplusend = np.concatenate([arr_tstart, [arr_tend[-1]]])
 
     dictlcdata = {"time": arr_tmid}
 
-    linelistindices_allfeatures = tuple([l for feature in emfeatures for l in feature.linelistindices])
+    linelistindices_allfeatures = tuple(l for feature in emfeatures for l in feature.linelistindices)
 
     dfpackets, nprocs_read = get_packets_with_emtype(
         modelpath, emtypecolumn, linelistindices_allfeatures, maxpacketfiles=maxpacketfiles
     )
 
     for feature in emfeatures:
         # dictlcdata[feature.colname] = np.zeros_like(arr_tstart, dtype=float)
@@ -99,33 +134,29 @@
         # normfactor = 1. / 4 / math.pi / (mpc_to_cm ** 2) / nprocs_read
 
         energysumsreduced = calculate_timebinned_packet_sum(dfpackets_selected, timearrayplusend)
         # print(energysumsreduced, arr_timedelta)
         fluxdata = np.divide(energysumsreduced * normfactor, arr_timedelta * 86400.0)
         dictlcdata[feature.colname] = fluxdata
 
-    lcdata = pd.DataFrame(dictlcdata)
-    return lcdata
+    return pd.DataFrame(dictlcdata)
 
 
 def get_line_fluxes_from_pops(emfeatures, modelpath, arr_tstart=None, arr_tend=None) -> pd.DataFrame:
     if arr_tstart is None:
-        arr_tstart = at.get_timestep_times_float(modelpath, loc="start")
+        arr_tstart = at.get_timestep_times(modelpath, loc="start")
     if arr_tend is None:
-        arr_tend = at.get_timestep_times_float(modelpath, loc="end")
+        arr_tend = at.get_timestep_times(modelpath, loc="end")
 
     arr_timedelta = np.array(arr_tend) - np.array(arr_tstart)
     arr_tmid = arr_tend = (np.array(arr_tstart) + np.array(arr_tend)) / 2.0
 
     modeldata, _ = at.inputmodel.get_modeldata(modelpath)
 
-    ionlist = []
-    for feature in emfeatures:
-        ionlist.append((feature.atomic_number, feature.ion_stage))
-
+    ionlist = [(feature.atomic_number, feature.ion_stage) for feature in emfeatures]
     adata = at.atomic.get_levels(modelpath, ionlist=tuple(ionlist), get_transitions=True, get_photoionisations=False)
 
     timearrayplusend = np.concatenate([arr_tstart, [arr_tend[-1]]])
 
     dictlcdata = {"time": arr_tmid}
 
     for feature in emfeatures:
@@ -185,27 +216,26 @@
                         unaccounted_shells.append(modelgridindex)
                 if unaccounted_shells:
                     print(f"No data for cells {unaccounted_shells} (expected for empty cells)")
                 assert len(unaccounted_shells) < len(modeldata.index)  # must be data for at least one shell
 
         dictlcdata[feature.colname] = fluxdata
 
-    lcdata = pd.DataFrame(dictlcdata)
-    return lcdata
+    return pd.DataFrame(dictlcdata)
 
 
 def get_closelines(
     modelpath,
     atomic_number: int,
     ion_stage: int,
-    approxlambdalabel: Union[str, int],
-    lambdamin: Optional[float] = None,
-    lambdamax: Optional[float] = None,
-    lowerlevelindex: Optional[int] = None,
-    upperlevelindex: Optional[int] = None,
+    approxlambdalabel: str | int,
+    lambdamin: float | None = None,
+    lambdamax: float | None = None,
+    lowerlevelindex: int | None = None,
+    upperlevelindex: int | None = None,
 ):
     dflinelist = at.get_linelist_dataframe(modelpath)
     dflinelistclosematches = dflinelist.query("atomic_number == @atomic_number and ionstage == @ion_stage").copy()
     if lambdamin is not None:
         dflinelistclosematches = dflinelistclosematches.query("@lambdamin < lambda_angstroms")
     if lambdamax is not None:
         dflinelistclosematches = dflinelistclosematches.query("@lambdamax > lambda_angstroms")
@@ -235,15 +265,15 @@
         upperlevelindicies,
         lowerlevelindicies,
     )
 
 
 def get_labelandlineindices(modelpath, emfeaturesearch):
     featuretuple = namedtuple(
-        "feature",
+        "featuretuple",
         [
             "colname",
             "featurelabel",
             "approxlambda",
             "linelistindices",
             "lowestlambda",
             "highestlamba",
@@ -265,15 +295,15 @@
     # labelandlineindices.append(featuretuple(*get_closelines(dflinelist, 26, 2, 7155, 7150, 7160)))
     # labelandlineindices.append(featuretuple(*get_closelines(dflinelist, 26, 2, 12570, 12470, 12670)))
     # labelandlineindices.append(featuretuple(*get_closelines(dflinelist, 28, 2, 7378, 7373, 7383)))
 
     return labelandlineindices
 
 
-def make_flux_ratio_plot(args):
+def make_flux_ratio_plot(args: argparse.Namespace) -> None:
     # font = {'size': 16}
     # matplotlib.rc('font', **font)
     nrows = 1
     fig, axes = plt.subplots(
         nrows=nrows,
         ncols=1,
         sharey=False,
@@ -292,33 +322,36 @@
     # axis.set_ylabel(r'log$_1$$_0$ F$_\lambda$ at 1 Mpc [erg/s/cm$^2$/$\mathrm{{\AA}}$]')
 
     # axis.set_xlim(left=supxmin, right=supxmax)
     pd.set_option("display.max_rows", 3500)
     pd.set_option("display.width", 150)
     pd.options.display.max_rows = 500
 
-    for _seriesindex, (modelpath, modellabel, modelcolor) in enumerate(zip(args.modelpath, args.label, args.color)):
+    for modelpath, modellabel, modelcolor in zip(args.modelpath, args.label, args.color):
         print(f"====> {modellabel}")
 
         emfeatures = get_labelandlineindices(modelpath, tuple(args.emfeaturesearch))
 
-        if args.frompops:
-            dflcdata = get_line_fluxes_from_pops(
-                emfeatures, modelpath, arr_tstart=args.timebins_tstart, arr_tend=args.timebins_tend
+        dflcdata = (
+            get_line_fluxes_from_pops(
+                emfeatures,
+                modelpath,
+                arr_tstart=args.timebins_tstart,
+                arr_tend=args.timebins_tend,
             )
-        else:
-            dflcdata = get_line_fluxes_from_packets(
+            if args.frompops
+            else get_line_fluxes_from_packets(
                 args.emtypecolumn,
                 emfeatures,
                 modelpath,
                 maxpacketfiles=args.maxpacketfiles,
                 arr_tstart=args.timebins_tstart,
                 arr_tend=args.timebins_tend,
             )
-
+        )
         dflcdata = dflcdata.eval(f"fratio = {emfeatures[1].colname} / {emfeatures[0].colname}")
         axis.set_ylabel(
             r"F$_{\mathrm{" + emfeatures[1].featurelabel + r"}}$ / F$_{\mathrm{" + emfeatures[0].featurelabel + r"}}$"
         )
 
         # \mathrm{\AA}
 
@@ -349,49 +382,48 @@
             ax.plot(arr_tdays, arr_floersfit, color="black", label="Flörs+2020 fit", lw=2.0)
 
         femis = pd.read_csv(
             "/Users/luke/Dropbox/Papers (first-author)/2022 Artis ionisation/"
             "generateplots/floers_model_NIR_VIS_ratio_20201126.csv"
         )
 
-        amodels = {}
+        amodels: dict[str, tuple[list, list]] = {}
         for _index, row in femis.iterrows():
             modelname = row.file.replace("fig-nne_Te_allcells-", "").replace(f"-{row.epoch}d.txt", "")
             if modelname not in amodels:
                 amodels[modelname] = ([], [])
             if int(row.epoch) != 263:
                 amodels[modelname][0].append(row.epoch)
                 amodels[modelname][1].append(row.NIR_VIS_ratio)
 
-        aindex = 0
         # for amodelname, (xlist, ylist) in amodels.items():
-        for amodelname, alabel in [
-            # ('w7', 'W7'),
-            # ('subch', 'S0'),
-            # ('subch_shen2018', r'1M$_\odot$'),
-            # ('subch_shen2018_electronlossboost4x', '1M$_\odot$ (Shen+18) 4x e- loss'),
-            # ('subch_shen2018_electronlossboost8x', r'1M$_\odot$ heatboost8'),
-            # ('subch_shen2018_electronlossboost12x', '1M$_\odot$ (Shen+18) 12x e- loss'),
-        ]:
+        for aindex, (amodelname, alabel) in enumerate(
+            [
+                ("w7", "W7"),
+                ("subch", "S0"),
+                # ('subch_shen2018', r'1M$_\odot$'),
+                # ('subch_shen2018_electronlossboost4x', '1M$_\odot$ (Shen+18) 4x e- loss'),
+                # ('subch_shen2018_electronlossboost8x', r'1M$_\odot$ heatboost8'),
+                # ('subch_shen2018_electronlossboost12x', '1M$_\odot$ (Shen+18) 12x e- loss'),
+            ]
+        ):
             xlist, ylist = amodels[amodelname]
             color = args.color[aindex] if aindex < len(args.color) else None
             print(amodelname, xlist, ylist)
             axis.plot(
                 xlist,
                 ylist,
                 color=color,
                 label="Flörs " + alabel,
                 marker="+",
                 markersize=10,
                 markeredgewidth=2,
                 lw=0,
                 alpha=0.8,
             )
-            aindex += 1
-
     m18_tdays = np.array([206, 229, 303, 339])
     m18_pew = {}
     # m18_pew[(26, 2, 12570)] = np.array([2383, 1941, 2798, 6770])
     m18_pew[(26, 2, 7155)] = np.array([618, 417, 406, 474])
     m18_pew[(28, 2, 7378)] = np.array([157, 256, 236, 309])
     if args.emfeaturesearch[1][:3] in m18_pew and args.emfeaturesearch[0][:3] in m18_pew:
         axis.set_ylim(ymax=12)
@@ -412,24 +444,31 @@
 
     fig.savefig(args.outputfile, format="pdf")
     # plt.show()
     print(f"Saved {args.outputfile}")
     plt.close()
 
 
-def get_packets_with_emission_conditions(modelpath, emtypecolumn, lineindices, tstart, tend, maxpacketfiles=None):
+def get_packets_with_emission_conditions(
+    modelpath: str | Path,
+    emtypecolumn: str,
+    lineindices: t.Sequence[int],
+    tstart: float,
+    tend: float,
+    maxpacketfiles: int | None = None,
+) -> pd.DataFrame:
     estimators = at.estimators.read_estimators(modelpath, get_ion_values=False, get_heatingcooling=False)
 
     modeldata, _ = at.inputmodel.get_modeldata(modelpath)
     ts = at.get_timestep_of_timedays(modelpath, tend)
     allnonemptymgilist = [
         modelgridindex for modelgridindex in modeldata.index if not estimators[(ts, modelgridindex)]["emptycell"]
     ]
 
-    # model_tmids = at.get_timestep_times_float(modelpath, loc='mid')
+    # model_tmids = at.get_timestep_times(modelpath, loc='mid')
     # arr_velocity_mid = tuple(list([(float(v1) + float(v2)) * 0.5 for v1, v2 in zip(
     #     modeldata['velocity_inner'].to_numpy(), modeldata['velocity_outer'].to_numpy())]))
 
     # from scipy.interpolate import interp1d
     # interp_log10nne, interp_te = {}, {}
     # for ts in range(len(model_tmids)):
     #     arr_v = np.zeros_like(allnonemptymgilist, dtype='float')
@@ -467,26 +506,30 @@
             return estimators[(int(packet["em_timestep"]), int(packet[em_mgicolumn]))]["Te"]
 
         dfpackets_selected["em_Te"] = dfpackets_selected.apply(em_Te, axis=1)
 
     return dfpackets_selected
 
 
-def plot_nne_te_points(axis, serieslabel, em_log10nne, em_Te, normtotalpackets, color, marker="o"):
+def plot_nne_te_points(
+    axis: plt.Axes,
+    serieslabel: str,
+    em_log10nne: t.Sequence[float],
+    em_Te: t.Sequence[float],
+    normtotalpackets: float,
+    color: float | str | None,
+    marker: str | None = "o",
+) -> None:
     # color_adj = [(c + 0.3) / 1.3 for c in mpl.colors.to_rgb(color)]
     color_adj = [(c + 0.1) / 1.1 for c in mpl.colors.to_rgb(color)]
-    hitcount = {}
+    hitcount: dict[tuple[float, float], int] = {}
     for log10nne, Te in zip(em_log10nne, em_Te):
         hitcount[(log10nne, Te)] = hitcount.get((log10nne, Te), 0) + 1
 
-    if hitcount:
-        arr_log10nne, arr_te = zip(*hitcount.keys())
-    else:
-        arr_log10nne, arr_te = np.array([]), np.array([])
-
+    arr_log10nne, arr_te = zip(*hitcount.keys()) if hitcount else ([], [])
     arr_weight = np.array([hitcount[(x, y)] for x, y in zip(arr_log10nne, arr_te)])
     arr_weight = (arr_weight / normtotalpackets) * 500
     arr_size = np.sqrt(arr_weight) * 10
 
     # arr_weight = arr_weight / float(max(arr_weight))
     # arr_color = np.zeros((len(arr_x), 4))
     # arr_color[:, :3] = np.array([[c for c in mpl.colors.to_rgb(color)] for x in arr_weight])
@@ -542,15 +585,15 @@
         "Flörs+2020",
     ]  # , 'Floers CMFGEN', 'Floers Smyth']
     refdatacolors = ["0.0", "C1", "C2", "C4"]
     refdatakeys = [None for _ in refdatafilenames]
     refdatatimes = [None for _ in refdatafilenames]
     refdatapoints = [None for _ in refdatafilenames]
     for refdataindex, refdatafilename in enumerate(refdatafilenames):
-        with open(refdatafilename, encoding="utf-8") as data_file:
+        with Path(refdatafilename).open(encoding="utf-8") as data_file:
             floers_te_nne = json.loads(data_file.read())
 
         # give an ordering and index to dict items
         refdatakeys[refdataindex] = sorted(floers_te_nne.keys(), key=float)  # strings, not floats
         refdatatimes[refdataindex] = np.array([float(t) for t in refdatakeys[refdataindex]])
         refdatapoints[refdataindex] = [floers_te_nne[t] for t in refdatakeys[refdataindex]]
         print(f"{refdatafilename} data available for times: {list(refdatatimes[refdataindex])}")
@@ -584,15 +627,15 @@
         if modelpath is not None:
             print(f"Getting packets/nne/Te data for ARTIS model: '{modellabel}'")
 
             emdata_all[modelindex] = {}
 
             emfeatures = get_labelandlineindices(modelpath, tuple(args.emfeaturesearch))
 
-            linelistindices_allfeatures = tuple([l for feature in emfeatures for l in feature.linelistindices])
+            linelistindices_allfeatures = tuple(l for feature in emfeatures for l in feature.linelistindices)
 
             for tmid, tstart, tend in zip(times_days, args.timebins_tstart, args.timebins_tend):
                 dfpackets = get_packets_with_emission_conditions(
                     modelpath,
                     args.emtypecolumn,
                     linelistindices_allfeatures,
                     tstart,
@@ -615,34 +658,35 @@
             estimators = at.estimators.read_estimators(modelpath, get_ion_values=False, get_heatingcooling=False)
             modeldata, _ = at.inputmodel.get_modeldata(modelpath)
             Tedata_all[modelindex] = {}
             log10nnedata_all[modelindex] = {}
             for tmid, tstart, tend in zip(times_days, args.timebins_tstart, args.timebins_tend):
                 Tedata_all[modelindex][tmid] = []
                 log10nnedata_all[modelindex][tmid] = []
-                tstartlist = at.get_timestep_times_float(modelpath, loc="start")
-                tendlist = at.get_timestep_times_float(modelpath, loc="end")
+                tstartlist = at.get_timestep_times(modelpath, loc="start")
+                tendlist = at.get_timestep_times(modelpath, loc="end")
                 tslist = [ts for ts in range(len(tstartlist)) if tendlist[ts] >= tstart and tstartlist[ts] <= tend]
                 for timestep in tslist:
                     for modelgridindex in modeldata.index:
-                        try:
-                            Tedata_all[modelindex][tmid].append(estimators[(timestep, modelgridindex)]["Te"])
-                            log10nnedata_all[modelindex][tmid].append(
-                                math.log10(estimators[(timestep, modelgridindex)]["nne"])
-                            )
-                        except KeyError:
-                            pass
+                        Te, log10nne = None, None
+                        with contextlib.suppress(KeyError):
+                            Te = estimators[(timestep, modelgridindex)]["Te"]
+                            log10nne = math.log10(estimators[(timestep, modelgridindex)]["nne"])
+
+                        if Te is not None and log10nne is not None:
+                            Tedata_all[modelindex][tmid].append(Te)
+                            log10nnedata_all[modelindex][tmid].append(log10nne)
 
         if modeltag != "all":
             continue
 
+        nrows = 1
         for tmid in times_days:
             print(f"  Plot at {tmid} days")
 
-            nrows = 1
             fig, axis = plt.subplots(
                 nrows=nrows,
                 ncols=1,
                 sharey=False,
                 sharex=False,
                 figsize=(
                     args.figscale * at.get_config()["figwidth"],
@@ -856,16 +900,16 @@
             description=(__doc__),
         )
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     if not args.modelpath:
-        args.modelpath = [Path(".")]
-    elif isinstance(args.modelpath, (str, Path)):
+        args.modelpath = [Path()]
+    elif isinstance(args.modelpath, str | Path):
         args.modelpath = [args.modelpath]
 
     args.modelpath = at.flatten_list(args.modelpath)
 
     args.label, args.modeltag, args.color = at.trim_or_pad(len(args.modelpath), args.label, args.modeltag, args.color)
 
     args.emtypecolumn = "emissiontype" if args.use_lastemissiontype else "trueemissiontype"
```

### Comparing `artistools-2023.5.16.3/artistools/logfiles.py` & `artistools-2023.8.1/artistools/logfiles.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
     mpiranklist = at.get_mpiranklist(modelpath)
     nprocs = at.get_nprocs(modelpath)
 
     logfilepaths = []
 
     for folderpath in at.get_runfolders(modelpath):
-        nfilesread_thisfolder = 0
         # for mpirank in range(nprocs):
         for mpirank in mpiranklist:
             logfilename = f"output_{mpirank}-0.txt"
             logfilepath = Path(folderpath, logfilename)
             if not logfilepath.is_file():
                 # logfilepath = Path(folderpath, logfilename + '.gz')
                 # if not logfilepath.is_file():
@@ -29,23 +28,21 @@
             logfilepaths.append(logfilepath)
 
     # print(logfilepaths)
     return logfilepaths
 
 
 def read_time_taken(logfilepaths):
-    logfiledict = {}
-
     updategrid_dict = {}
     updatepackets_dict = {}
     writeestimators_dict = {}
 
     for logfilepath in logfilepaths:
         mpi_process = int(str(logfilepath).split("/")[-1].split("-")[0].split("_")[-1])
-        with open(logfilepath) as logfile:
+        with Path(logfilepath).open() as logfile:
             lineswithtimes = [line.split(" ") for line in logfile if "took" in line]
 
         # for line in lineswithtimes:
         #     print(line)
 
         # get times for update_grid:
         updategridlines = [line for line in lineswithtimes if line[2] == "update_grid:"]
@@ -85,20 +82,19 @@
             # # print(process, timetaken)
             #
             if timestep not in writeestimators_dict:
                 writeestimators_dict[timestep] = {}
             if process not in writeestimators_dict[timestep]:
                 writeestimators_dict[timestep][process] = timetaken
 
-    # print(updatepackets_dict[30])
-    logfiledict["update_grid"] = updategrid_dict
-    logfiledict["update_packets"] = updatepackets_dict
-    logfiledict["write_estimators"] = writeestimators_dict
-    # print(logfiledict['update_packets'][30])
-    return logfiledict
+    return {
+        "update_grid": updategrid_dict,
+        "update_packets": updatepackets_dict,
+        "write_estimators": writeestimators_dict,
+    }
 
 
 def make_plot(logfiledict):
     for timestep in range(55):
         plotvalues = ["update_packets", "update_grid", "write_estimators"]
         for plotvalue in plotvalues:
             # print(logfiledict[plotvalue][timestep])
@@ -133,14 +129,14 @@
             formatter_class=at.CustomArgHelpFormatter, description="Plot durations from log files."
         )
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     if not args.modelpath:
-        args.modelpath = [Path(".")]
+        args.modelpath = [Path()]
 
     # make_plot(logfiledict)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `artistools-2023.5.16.3/artistools/macroatom.py` & `artistools-2023.8.1/artistools/macroatom.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 import argparse
-import glob
-import os.path
 import sys
+from pathlib import Path
 
 import matplotlib.pyplot as plt
+import numpy as np
 import pandas as pd
 
 import artistools as at
 
 defaultoutputfile = "plotmacroatom_cell{0:03d}_{1:03d}-{2:03d}.pdf"
 
 
@@ -31,50 +31,45 @@
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter, description="Plot ARTIS macroatom transitions."
         )
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
-    if os.path.isdir(args.outputfile):
-        args.outputfile = os.path.join(args.outputfile, defaultoutputfile)
+    if Path(args.outputfile).is_dir():
+        args.outputfile = str(Path(args.outputfile, defaultoutputfile))
 
     atomic_number = at.get_atomic_number(args.element.lower())
     if atomic_number < 1:
         print(f"Could not find element '{args.element}'")
         raise AssertionError
 
     timestepmin = args.timestep
 
     timestepmax = timestepmin if not args.timestepmax or args.timestepmax < 0 else args.timestepmax
 
-    input_files = glob.glob(os.path.join(args.modelpath, "macroatom_????.out*"), recursive=True) + glob.glob(
-        os.path.join(args.modelpath, "*/macroatom_????.out*"), recursive=True
-    )
+    input_files = Path(args.modelpath).glob("**/macroatom_????.out*")
 
     if not input_files:
         print("No macroatom files found")
         raise FileNotFoundError
 
     dfall = read_files(input_files, args.modelgridindex, timestepmin, timestepmax, atomic_number)
 
-    specfilename = os.path.join(args.modelpath, "spec.out")
-
-    if not os.path.isfile(specfilename):
-        specfilename = os.path.join(args.modelpath, "../example_run/spec.out")
+    specfilename = Path(args.modelpath, "spec.out")
 
-    if not os.path.isfile(specfilename):
+    if not specfilename.is_file():
         print(f"Could not find {specfilename}")
         raise FileNotFoundError
 
     outputfile = args.outputfile.format(args.modelgridindex, timestepmin, timestepmax)
     make_plot(
         dfall,
         args.modelpath,
-        specfilename,
+        str(specfilename),
         timestepmin,
         timestepmax,
         outputfile,
         xmin=args.xmin,
         xmax=args.xmax,
         modelgridindex=args.modelgridindex,
     )
@@ -109,16 +104,17 @@
         xy=(0.02, 0.96),
         xycoords="axes fraction",
         horizontalalignment="left",
         verticalalignment="top",
         fontsize=8,
     )
 
-    lambda_cmf_in = 2.99792458e18 / dfmacroatom["nu_cmf_in"].to_numpy()
-    lambda_cmf_out = 2.99792458e18 / dfmacroatom["nu_cmf_out"].to_numpy()
+    with np.errstate(divide="ignore"):
+        lambda_cmf_in = 2.99792458e18 / dfmacroatom["nu_cmf_in"].to_numpy()
+        lambda_cmf_out = 2.99792458e18 / dfmacroatom["nu_cmf_out"].to_numpy()
     # axis.scatter(lambda_cmf_in, lambda_cmf_out, s=1, alpha=0.5, edgecolor='none')
     axis.plot(
         lambda_cmf_in,
         lambda_cmf_out,
         linestyle="none",
         marker="o",  # alpha=0.5,
         markersize=2,
@@ -139,15 +135,15 @@
 
 
 def read_files(files, modelgridindex=None, timestepmin=None, timestepmax=None, atomic_number=None):
     dfall = None
     if not files:
         print("No files")
     else:
-        for _, filepath in enumerate(files):
+        for filepath in files:
             print(f"Loading {filepath}...")
 
             df_thisfile = pd.read_csv(filepath, delim_whitespace=True)
             # df_thisfile[['modelgridindex', 'timestep']].apply(pd.to_numeric)
             if modelgridindex:
                 df_thisfile = df_thisfile.query("modelgridindex==@modelgridindex")
             if timestepmin is not None:
```

### Comparing `artistools-2023.5.16.3/artistools/matplotlibrc` & `artistools-2023.8.1/artistools/matplotlibrc`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/misc.py` & `artistools-2023.8.1/artistools/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,32 @@
+from __future__ import annotations
+
 import argparse
+import contextlib
 import gzip
-import io
 import math
-import os
+import typing as t
 from collections import namedtuple
-from collections.abc import Iterable
-from collections.abc import Iterator
-from collections.abc import Sequence
 from functools import lru_cache
 from itertools import chain
 from pathlib import Path
-from typing import Any
-from typing import Callable
-from typing import Literal
-from typing import Optional
-from typing import Union
 
 import lz4.frame
 import numpy as np
 import pandas as pd
 import polars as pl
 import pyzstd
 import xz
+from typeguard import typechecked
 
 import artistools as at
 
+if t.TYPE_CHECKING:
+    import io
+
 roman_numerals = (
     "",
     "I",
     "II",
     "III",
     "IV",
     "V",
@@ -47,101 +45,97 @@
     "XVIII",
     "XIX",
     "XX",
 )
 
 
 class CustomArgHelpFormatter(argparse.ArgumentDefaultsHelpFormatter):
-    def __init__(self, *args: Any, **kwargs: Any) -> None:
+    def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
         kwargs["max_help_position"] = 39
         super().__init__(*args, **kwargs)
 
-    def add_arguments(self, actions: Iterable[argparse.Action]) -> None:
+    def add_arguments(self, actions: t.Iterable[argparse.Action]) -> None:
         getinvocation = super()._format_action_invocation
 
         def my_sort(action: argparse.Action) -> str:
             opstr = getinvocation(action)
-            opstr = opstr.upper().replace("-", "z")  # push dash chars below alphabet
-
-            return opstr
+            return opstr.upper().replace("-", "z")  # push dash chars below alphabet
 
         actions = sorted(actions, key=my_sort)
         super().add_arguments(actions)
 
 
+@typechecked
 class AppendPath(argparse.Action):
     def __call__(self, parser, args, values, option_string=None) -> None:  # type: ignore[no-untyped-def] # noqa: ARG002
         # if getattr(args, self.dest) is None:
         #     setattr(args, self.dest, [])
-        if isinstance(values, Iterable):
+        if isinstance(values, t.Iterable):
             pathlist = getattr(args, self.dest)
             # not pathlist avoids repeated appending of the same items when called from Python
             # instead of from the command line
             if not pathlist:
                 for pathstr in values:
                     # if Path(pathstr) not in pathlist:
                     pathlist.append(Path(pathstr))
         else:
             setattr(args, self.dest, Path(values))
 
 
-def showtimesteptimes(modelpath: Optional[Path] = None, numberofcolumns: int = 5) -> None:
+def showtimesteptimes(modelpath: Path | None = None, numberofcolumns: int = 5) -> None:
     """Print a table showing the timesteps and their corresponding times."""
     if modelpath is None:
         modelpath = Path()
 
     print("Timesteps and midpoint times in days:\n")
 
-    times = get_timestep_times_float(modelpath, loc="mid")
+    times = get_timestep_times(modelpath, loc="mid")
     indexendofcolumnone = math.ceil((len(times) - 1) / numberofcolumns)
-    for rownum in range(0, indexendofcolumnone):
+    for rownum in range(indexendofcolumnone):
         strline = ""
         for colnum in range(numberofcolumns):
             if colnum > 0:
                 strline += "\t"
             newindex = rownum + colnum * indexendofcolumnone
             if newindex + 1 < len(times):
                 strline += f"{newindex:4d}: {float(times[newindex + 1]):.3f}d"
         print(strline)
 
 
 @lru_cache(maxsize=8)
-def get_composition_data(filename: Union[Path, str]) -> pd.DataFrame:
+def get_composition_data(filename: Path | str) -> pd.DataFrame:
     """Return a pandas DataFrame containing details of included elements and ions."""
-    if os.path.isdir(Path(filename)):
-        filename = os.path.join(filename, "compositiondata.txt")
+    filename = Path(filename, "compositiondata.txt") if Path(filename).is_dir() else Path(filename)
 
     columns = ("Z,nions,lowermost_ionstage,uppermost_ionstage,nlevelsmax_readin,abundance,mass,startindex").split(",")
 
     rowdfs = []
-    with open(filename) as fcompdata:
+    with filename.open() as fcompdata:
         nelements = int(fcompdata.readline())
         fcompdata.readline()  # T_preset
         fcompdata.readline()  # homogeneous_abundances
         startindex = 0
         for _ in range(nelements):
             line = fcompdata.readline()
             linesplit = line.split()
             row_list = [int(x) for x in linesplit[:5]] + [float(x) for x in linesplit[5:]] + [startindex]
 
             rowdfs.append(pd.DataFrame([row_list], columns=columns))
 
             startindex += int(rowdfs[-1].iloc[0]["nions"])
 
-    compdf = pd.concat(rowdfs, ignore_index=True)
-
-    return compdf
+    return pd.concat(rowdfs, ignore_index=True)
 
 
 def get_composition_data_from_outputfile(modelpath: Path) -> pd.DataFrame:
     """Read ion list from output file."""
     atomic_composition = {}
 
-    with open(modelpath / "output_0-0.txt") as foutput:
-        Z: Optional[int] = None
+    with (modelpath / "output_0-0.txt").open() as foutput:
+        Z: int | None = None
         ioncount = 0
         for row in foutput:
             if row.split()[0] == "[input.c]":
                 split_row = row.split()
                 if split_row[1] == "element":
                     Z = int(split_row[4])
                     ioncount = 0
@@ -153,28 +147,28 @@
     composition_df = pd.DataFrame([(Z, atomic_composition[Z]) for Z in atomic_composition], columns=["Z", "nions"])
     composition_df["lowermost_ionstage"] = [1] * composition_df.shape[0]
     composition_df["uppermost_ionstage"] = composition_df["nions"]
     return composition_df
 
 
 def split_dataframe_dirbins(
-    res_df: Union[pl.DataFrame, pd.DataFrame], index_of_repeated_value: int = 0, output_polarsdf: bool = False
-) -> dict[int, Union[pd.DataFrame, pl.DataFrame]]:
+    res_df: pl.DataFrame | pd.DataFrame, index_of_repeated_value: int = 0, output_polarsdf: bool = False
+) -> dict[int, pd.DataFrame | pl.DataFrame]:
     """Res files repeat output for each angle.
     index_of_repeated_value is the column index to look for repeating eg. time of ts 0.
     In spec_res files it's 1 , but in lc_res file it's 0.
     """
     if isinstance(res_df, pd.DataFrame):
         res_df = pl.from_pandas(res_df)
 
     indexes_to_split = pl.arg_where(
         res_df[:, index_of_repeated_value] == res_df[0, index_of_repeated_value], eager=True
     )
 
-    res_data: dict[int, pl.DataFrame] = {}
+    res_data: dict[int, pd.DataFrame | pl.DataFrame] = {}
     prev_dfshape = None
     for i, index_value in enumerate(indexes_to_split):
         chunk = (
             res_df[indexes_to_split[i] : indexes_to_split[i + 1], :]
             if index_value != indexes_to_split[-1]
             else res_df[indexes_to_split[i] :, :]
         )
@@ -187,30 +181,30 @@
 
     assert len(res_data) == at.get_viewingdirectionbincount()
     return res_data
 
 
 def average_direction_bins(
     dirbindataframes: dict[int, pl.DataFrame],
-    overangle: Literal["phi", "theta"],
+    overangle: t.Literal["phi", "theta"],
 ) -> dict[int, pl.DataFrame]:
-    """Will average dict of direction-binned polars DataFrames according to the phi or theta angle."""
+    """Average dict of direction-binned polars DataFrames according to the phi or theta angle."""
     dirbincount = at.get_viewingdirectionbincount()
     nphibins = at.get_viewingdirection_phibincount()
 
     assert overangle in ["phi", "theta"]
     if overangle == "phi":
         start_bin_range = range(0, dirbincount, nphibins)
     elif overangle == "theta":
         ncosthetabins = at.get_viewingdirection_costhetabincount()
-        start_bin_range = range(0, nphibins)
+        start_bin_range = range(nphibins)
 
     # we will make a copy to ensure that we don't cause side effects from altering the original DataFrames
     # that might be returned again later by an lru_cached function
-    dirbindataframesout: dict[int, pd.DataFrame] = {}
+    dirbindataframesout: dict[int, pl.DataFrame] = {}
 
     for start_bin in start_bin_range:
         dirbindataframesout[start_bin] = dirbindataframes[start_bin]
 
         contribbins = (
             range(start_bin + 1, start_bin + nphibins)
             if overangle == "phi"
@@ -222,26 +216,28 @@
 
         dirbindataframesout[start_bin] /= 1 + len(contribbins)  # every nth bin is the average of n bins
         print(f"bin number {start_bin} = the average of bins {[start_bin, *list(contribbins)]}")
 
     return dirbindataframesout
 
 
-def match_closest_time(reftime: float, searchtimes: list[Any]) -> str:
+def match_closest_time(reftime: float, searchtimes: list[t.Any]) -> str:
     """Get time closest to reftime in list of times (searchtimes)."""
-    return str(f"{min([float(x) for x in searchtimes], key=lambda x: abs(x - reftime))}")
+    return str(f"{min((float(x) for x in searchtimes), key=lambda x: abs(x - reftime))}")
 
 
-def get_vpkt_config(modelpath: Union[Path, str]) -> dict[str, Any]:
+def get_vpkt_config(modelpath: Path | str) -> dict[str, t.Any]:
     filename = Path(modelpath, "vpkt.txt")
-    vpkt_config: dict[str, Any] = {}
-    with open(filename) as vpkt_txt:
-        vpkt_config["nobsdirections"] = int(vpkt_txt.readline())
-        vpkt_config["cos_theta"] = [float(x) for x in vpkt_txt.readline().split()]
-        vpkt_config["phi"] = [float(x) for x in vpkt_txt.readline().split()]
+
+    with filename.open() as vpkt_txt:
+        vpkt_config: dict[str, t.Any] = {
+            "nobsdirections": int(vpkt_txt.readline()),
+            "cos_theta": [float(x) for x in vpkt_txt.readline().split()],
+            "phi": [float(x) for x in vpkt_txt.readline().split()],
+        }
         nspecflag = int(vpkt_txt.readline())
 
         if nspecflag == 1:
             vpkt_config["nspectraperobs"] = int(vpkt_txt.readline())
             for _ in range(vpkt_config["nspectraperobs"]):
                 vpkt_txt.readline()
         else:
@@ -251,105 +247,104 @@
             int(x) for x in vpkt_txt.readline().split()
         )
 
     return vpkt_config
 
 
 @lru_cache(maxsize=8)
-def get_grid_mapping(modelpath: Union[Path, str]) -> tuple[dict[int, list[int]], dict[int, int]]:
+def get_grid_mapping(modelpath: Path | str) -> tuple[dict[int, list[int]], dict[int, int]]:
     """Return dict with the associated propagation cells for each model grid cell and
     a dict with the associated model grid cell of each propagration cell.
     """
     modelpath = Path(modelpath)
     filename = firstexisting("grid.out", tryzipped=True, folder=modelpath) if modelpath.is_dir() else Path(modelpath)
 
     assoc_cells: dict[int, list[int]] = {}
     mgi_of_propcells: dict[int, int] = {}
-    with open(filename) as fgrid:
+    with filename.open() as fgrid:
         for line in fgrid:
             row = line.split()
             propcellid, mgi = int(row[0]), int(row[1])
             if mgi not in assoc_cells:
                 assoc_cells[mgi] = []
             assoc_cells[mgi].append(propcellid)
             mgi_of_propcells[propcellid] = mgi
 
     return assoc_cells, mgi_of_propcells
 
 
 def get_wid_init_at_tmin(modelpath: Path) -> float:
-    # cell width in cm at time tmin
+    """`Return the Cartesian cell width [cm] at the simulation start time (tmin)."""
     day_to_sec = 86400
-    tmin = get_timestep_times_float(modelpath, loc="start")[0] * day_to_sec
+    tmin = get_timestep_times(modelpath, loc="start")[0] * day_to_sec
     _, modelmeta = at.get_modeldata(modelpath)
 
     rmax: float = modelmeta["vmax_cmps"] * tmin
 
     coordmax0 = rmax
     ncoordgrid0 = 50
 
-    wid_init = 2 * coordmax0 / ncoordgrid0
-    return wid_init
+    return 2 * coordmax0 / ncoordgrid0
 
 
 def get_wid_init_at_tmodel(
-    modelpath: Union[Path, str, None] = None,
-    ngridpoints: Optional[int] = None,
-    t_model_days: Optional[float] = None,
-    xmax: Optional[float] = None,
+    modelpath: Path | str | None = None,
+    ngridpoints: int | None = None,
+    t_model_days: float | None = None,
+    xmax: float | None = None,
 ) -> float:
+    """Return the Cartesian cell width [cm] at the model snapshot time."""
     if ngridpoints is None or t_model_days is None or xmax is None:
         # Luke: ngridpoint only equals the number of model cells if the model is 3D
         assert modelpath is not None
         dfmodel, modelmeta = at.get_modeldata(modelpath, getheadersonly=True)
         assert modelmeta["dimensions"] == 3
         ngridpoints = len(dfmodel)
         xmax = modelmeta["vmax_cmps"] * modelmeta["t_model_init_days"] * 86400
     ncoordgridx: int = round(ngridpoints ** (1.0 / 3.0))
 
     assert xmax is not None
-    wid_init = 2.0 * xmax / ncoordgridx
-
-    return wid_init
+    return 2.0 * xmax / ncoordgridx
 
 
 def get_syn_dir(modelpath: Path) -> tuple[float, float, float]:
+    """Return the direction from which theta angle is measured."""
     if not (modelpath / "syn_dir.txt").is_file():
         print(f"{modelpath / 'syn_dir.txt'} does not exist. using x,y,z = 0,0,1")
         return (0.0, 0.0, 1.0)
 
-    with open(modelpath / "syn_dir.txt") as syn_dir_file:
+    with (modelpath / "syn_dir.txt").open() as syn_dir_file:
         x, y, z = (float(i) for i in syn_dir_file.readline().split())
-        syn_dir = (x, y, z)
-
-    return syn_dir
+        return (x, y, z)
 
 
-def vec_len(vec: Union[Sequence[float], np.ndarray[Any, np.dtype[np.float64]]]) -> float:
+def vec_len(vec: t.Sequence[float] | np.ndarray[t.Any, np.dtype[np.float64]]) -> float:
     return float(np.sqrt(np.dot(vec, vec)))
 
 
 @lru_cache(maxsize=16)
-def get_nu_grid(modelpath: Path) -> np.ndarray[Any, np.dtype[np.float64]]:
-    """Get an array of frequencies at which the ARTIS spectra are binned by exspec."""
+def get_nu_grid(modelpath: Path) -> np.ndarray[t.Any, np.dtype[np.float64]]:
+    """Return an array of frequencies at which the ARTIS spectra are binned by exspec."""
     specfilename = firstexisting(["spec.out", "specpol.out"], folder=modelpath, tryzipped=True)
     specdata = pd.read_csv(specfilename, delim_whitespace=True)
     return specdata.loc[:, "0"].to_numpy()
 
 
-def get_deposition(modelpath: Union[Path, str] = ".") -> pd.DataFrame:
+@typechecked
+def get_deposition(modelpath: Path | str = ".") -> pd.DataFrame:
+    """Return a pandas DataFrame containing the deposition data."""
     if Path(modelpath).is_file():
-        depfilepath = modelpath
+        depfilepath = Path(modelpath)
         modelpath = Path(modelpath).parent
     else:
         depfilepath = Path(modelpath, "deposition.out")
 
-    ts_mids = get_timestep_times_float(modelpath, loc="mid")
+    ts_mids = get_timestep_times(modelpath, loc="mid")
 
-    with open(depfilepath) as fdep:
+    with depfilepath.open() as fdep:
         filepos = fdep.tell()
         line = fdep.readline()
         if line.startswith("#"):
             columns = line.lstrip("#").split()
         else:
             fdep.seek(filepos)  # undo the readline() and go back
             columns = ["tmid_days", "gammadep_Lsun", "positrondep_Lsun", "total_dep_Lsun"]
@@ -363,28 +358,28 @@
     for timestep, row in depdata.iterrows():
         assert abs(ts_mids[timestep] / row["tmid_days"] - 1) < 0.01  # deposition times don't match input.txt
 
     return depdata
 
 
 @lru_cache(maxsize=16)
-def get_timestep_times_float(
-    modelpath: Union[Path, str], loc: Literal["mid", "start", "end", "delta"] = "mid"
-) -> np.ndarray[Any, np.dtype[np.float64]]:
-    """Return a list of the time in days of each timestep."""
+def get_timestep_times(
+    modelpath: Path | str, loc: t.Literal["mid", "start", "end", "delta"] = "mid"
+) -> np.ndarray[t.Any, np.dtype[np.float64]]:
+    """Return a list of the times in days of each timestep."""
     modelpath = Path(modelpath)
     # virtual path to code comparison workshop models
     if not modelpath.exists() and modelpath.parts[0] == "codecomparison":
         import artistools.codecomparison
 
-        return artistools.codecomparison.get_timestep_times_float(modelpath=modelpath, loc=loc)
+        return artistools.codecomparison.get_timestep_times(modelpath=modelpath, loc=loc)
 
     modelpath = modelpath if modelpath.is_dir() else modelpath.parent
 
-    # custom timestep file
+    # use timestep.out if possible (allowing arbitrary timestep lengths)
     tsfilepath = Path(modelpath, "timesteps.out")
     if tsfilepath.exists():
         dftimesteps = pd.read_csv(tsfilepath, delim_whitespace=True, escapechar="#", index_col="timestep")
         if loc == "mid":
             return dftimesteps.tmid_days.to_numpy()
         if loc == "start":
             return dftimesteps.tstart_days.to_numpy()
@@ -398,63 +393,59 @@
 
     # older versions of Artis always used logarithmic timesteps and didn't produce a timesteps.out file
     inputparams = get_inputparams(modelpath)
     tmin = inputparams["tmin"]
     dlogt = (math.log(inputparams["tmax"]) - math.log(tmin)) / inputparams["ntstep"]
     timesteps = range(inputparams["ntstep"])
     if loc == "mid":
-        tmids = np.array([tmin * math.exp((ts + 0.5) * dlogt) for ts in timesteps])
-        return tmids
+        return np.array([tmin * math.exp((ts + 0.5) * dlogt) for ts in timesteps])
     if loc == "start":
-        tstarts = np.array([tmin * math.exp(ts * dlogt) for ts in timesteps])
-        return tstarts
+        return np.array([tmin * math.exp(ts * dlogt) for ts in timesteps])
     if loc == "end":
-        tends = np.array([tmin * math.exp((ts + 1) * dlogt) for ts in timesteps])
-        return tends
+        return np.array([tmin * math.exp((ts + 1) * dlogt) for ts in timesteps])
     if loc == "delta":
-        tdeltas = np.array([tmin * (math.exp((ts + 1) * dlogt) - math.exp(ts * dlogt)) for ts in timesteps])
-        return tdeltas
-
+        return np.array([tmin * (math.exp((ts + 1) * dlogt) - math.exp(ts * dlogt)) for ts in timesteps])
     msg = "loc must be one of 'mid', 'start', 'end', or 'delta'"
     raise ValueError(msg)
 
 
-def get_timestep_of_timedays(modelpath: Path, timedays: Union[str, float]) -> int:
+def get_timestep_of_timedays(modelpath: Path | str, timedays: str | float) -> int:
     """Return the timestep containing the given time in days."""
     if isinstance(timedays, str):
         # could be a string like '330d'
         timedays = timedays.rstrip("d")
 
     timedays_float = float(timedays)
 
-    arr_tstart = get_timestep_times_float(modelpath, loc="start")
-    arr_tend = get_timestep_times_float(modelpath, loc="end")
+    arr_tstart = get_timestep_times(modelpath, loc="start")
+    arr_tend = get_timestep_times(modelpath, loc="end")
     # to avoid roundoff errors, use the next timestep's tstart at each timestep's tend (t_width is not exact)
     arr_tend[:-1] = arr_tstart[1:]
 
     for ts, (tstart, tend) in enumerate(zip(arr_tstart, arr_tend)):
         if timedays_float >= tstart and timedays_float < tend:
             return ts
 
     msg = f"Could not find timestep bracketing time {timedays_float}"
     raise ValueError(msg)
 
 
+@typechecked
 def get_time_range(
     modelpath: Path,
-    timestep_range_str: Optional[str] = None,
-    timemin: Optional[float] = None,
-    timemax: Optional[float] = None,
-    timedays_range_str: Union[None, str, float] = None,
-) -> tuple[int, int, Optional[float], Optional[float]]:
+    timestep_range_str: str | None = None,
+    timemin: float | None = None,
+    timemax: float | None = None,
+    timedays_range_str: None | str | float = None,
+) -> tuple[int, int, float | None, float | None]:
     """Handle a time range specified in either days or timesteps."""
     # assertions make sure time is specified either by timesteps or times in days, but not both!
-    tstarts = get_timestep_times_float(modelpath, loc="start")
-    tmids = get_timestep_times_float(modelpath, loc="mid")
-    tends = get_timestep_times_float(modelpath, loc="end")
+    tstarts = get_timestep_times(modelpath, loc="start")
+    tmids = get_timestep_times(modelpath, loc="mid")
+    tends = get_timestep_times(modelpath, loc="end")
 
     if timemin and timemin > tends[-1]:
         print(f"{get_model_name(modelpath)}: WARNING timemin {timemin} is after the last timestep at {tends[-1]:.1f}")
         return -1, -1, timemin, timemax
     if timemax and timemax < tstarts[0]:
         print(
             f"{get_model_name(modelpath)}: WARNING timemax {timemax} is before the first timestep at {tstarts[0]:.1f}"
@@ -517,39 +508,38 @@
     time_days_upper = float(tends[timestepmax])
     assert timestepmin is not None
     assert timestepmax is not None
 
     return timestepmin, timestepmax, time_days_lower, time_days_upper
 
 
-def get_timestep_time(modelpath: Union[Path, str], timestep: int) -> float:
+def get_timestep_time(modelpath: Path | str, timestep: int) -> float:
     """Return the time in days of the midpoint of a timestep number."""
-    timearray = get_timestep_times_float(modelpath, loc="mid")
-    if timearray is not None:
-        return timearray[timestep]
-
-    return -1
+    timearray = get_timestep_times(modelpath, loc="mid")
+    return timearray[timestep]
 
 
-def get_escaped_arrivalrange(modelpath: Union[Path, str]) -> tuple[int, Optional[float], Optional[float]]:
+@typechecked
+def get_escaped_arrivalrange(modelpath: Path | str) -> tuple[int, float | None, float | None]:
+    """Return the time range for which the entire model can send light signals the observer."""
     modelpath = Path(modelpath)
     dfmodel, modelmeta = at.inputmodel.get_modeldata(modelpath, printwarningsonly=True, getheadersonly=True)
     vmax = modelmeta["vmax_cmps"]
     cornervmax = math.sqrt(3 * vmax**2)
 
     # find the earliest possible escape time and add the largest possible travel time
 
     # for 3D models, the box corners can have non-zero density (allowing packet escape from tmin)
     # for 1D and 2D, the largest escape radius at tmin is the box side radius
     vmax_tmin = cornervmax if at.inputmodel.get_dfmodel_dimensions(dfmodel) == 3 else vmax
 
     # earliest completely valid time is tmin plus maximum possible travel time from corner to origin
-    validrange_start_days = at.get_timestep_times_float(modelpath, loc="start")[0] * (1 + vmax_tmin / 29979245800)
+    validrange_start_days = at.get_timestep_times(modelpath, loc="start")[0] * (1 + vmax_tmin / 29979245800)
 
-    t_end = at.get_timestep_times_float(modelpath, loc="end")
+    t_end = at.get_timestep_times(modelpath, loc="end")
     # find the last possible escape time and subtract the largest possible travel time (observer time correction)
     try:
         depdata = at.get_deposition(modelpath=modelpath)  # use this file to find the last computed timestep
         nts_last = depdata.ts.max() if "ts" in depdata.columns else len(depdata) - 1
     except FileNotFoundError:
         print("WARNING: No deposition.out file found. Assuming all timesteps have been computed")
         nts_last = len(t_end) - 1
@@ -562,100 +552,112 @@
     if validrange_start_days > validrange_end_days:
         validrange_start_days, validrange_end_days = None, None
 
     return nts_last, validrange_start_days, validrange_end_days
 
 
 @lru_cache(maxsize=8)
-def get_model_name(path: Union[Path, str]) -> str:
+def get_model_name(path: Path | str) -> str:
     """Get the name of an ARTIS model from the path to any file inside it.
 
     Name will be either from a special plotlabel.txt file if it exists or the enclosing directory name
     """
     path = Path(path)
     if not path.exists() and path.parts[0] == "codecomparison":
         return str(path)
 
     abspath = path.resolve()
 
     modelpath = abspath if abspath.is_dir() else abspath.parent
 
     try:
         plotlabelfile = Path(modelpath, "plotlabel.txt")
-        with open(plotlabelfile) as f:
+        with plotlabelfile.open() as f:
             return f.readline().strip()
     except FileNotFoundError:
-        return os.path.basename(modelpath)
+        return Path(modelpath).name
 
 
 def get_z_a_nucname(nucname: str) -> tuple[int, int]:
     """Return atomic number and mass number from a string like 'Pb208' (returns 92, 208)."""
-    if nucname.startswith("X_"):
-        nucname = nucname[2:]
+    nucname = nucname.removeprefix("X_")
     z = get_atomic_number(nucname.rstrip("0123456789"))
     assert z > 0
     a = int(nucname.lower().lstrip("abcdefghijklmnopqrstuvwxyz"))
     return z, a
 
 
 @lru_cache(maxsize=1)
 def get_elsymbolslist() -> list[str]:
-    elsymbols = [
+    """Return a list of element symbols.
+
+
+    Example:
+    -------
+    elsymbolslist()[26] = 'Fe'.
+    """
+    return [
         "n",
-        *list(pd.read_csv(at.get_config()["path_datadir"] / "elements.csv", usecols=["symbol"])["symbol"].to_numpy()),
+        *list(
+            pd.read_csv(
+                at.get_config()["path_datadir"] / "elements.csv",
+                usecols=["symbol"],
+            )["symbol"].to_numpy()
+        ),
     ]
 
-    return elsymbols
-
 
 def get_atomic_number(elsymbol: str) -> int:
+    """Return the atomic number of an element symbol."""
     assert elsymbol is not None
-    if elsymbol.startswith("X_"):
-        elsymbol = elsymbol[2:]
-
+    elsymbol = elsymbol.removeprefix("X_")
     elsymbol = elsymbol.split("_")[0].split("-")[0].rstrip("0123456789")
 
     if elsymbol.title() in get_elsymbolslist():
         return get_elsymbolslist().index(elsymbol.title())
 
     return -1
 
 
 def decode_roman_numeral(strin: str) -> int:
+    """Return the integer corresponding to a Roman numeral."""
     if strin.upper() in roman_numerals:
         return roman_numerals.index(strin.upper())
     return -1
 
 
 def get_elsymbol(atomic_number: int) -> str:
+    """Return the element symbol of an atomic number."""
     return get_elsymbolslist()[atomic_number]
 
 
 @lru_cache(maxsize=16)
 def get_ionstring(
-    atomic_number: int, ionstage: Union[int, Literal["ALL"], None], spectral: bool = True, nospace: bool = False
+    atomic_number: int, ionstage: int | None | t.Literal["ALL"], spectral: bool = True, nospace: bool = False
 ) -> str:
-    if ionstage == "ALL" or ionstage is None:
+    """Return a string with the element symbol and ionisation stage."""
+    if ionstage is None or ionstage == "ALL":
         return f"{get_elsymbol(atomic_number)}"
 
     if spectral:
-        return f"{get_elsymbol(atomic_number)}{' ' if not nospace else ''}{roman_numerals[ionstage]}"
+        return f"{get_elsymbol(atomic_number)}{'' if nospace else ' '}{roman_numerals[ionstage]}"
 
     # ion notion e.g. Co+, Fe2+
     if ionstage > 2:
         strcharge = r"$^{" + str(ionstage - 1) + r"{+}}$"
     elif ionstage == 2:
         strcharge = r"$^{+}$"
     else:
         strcharge = ""
     return f"{get_elsymbol(atomic_number)}{strcharge}"
 
 
 # based on code from https://gist.github.com/kgaughan/2491663/b35e9a117b02a3567c8107940ac9b2023ba34ced
-def parse_range(rng: str, dictvars: dict[str, int]) -> Iterable[Any]:
+@typechecked
+def parse_range(rng: str, dictvars: dict[str, int]) -> t.Iterable[t.Any]:
     """Parse a string with an integer range and return a list of numbers, replacing special variables in dictvars."""
     strparts = rng.split("-")
 
     if len(strparts) not in [1, 2]:
         msg = f"Bad range: '{rng}'"
         raise ValueError(msg)
 
@@ -665,100 +667,105 @@
 
     if start > end:
         end, start = start, end
 
     return range(start, end + 1)
 
 
-def parse_range_list(rngs: Union[str, list], dictvars: Optional[dict] = None) -> list[Any]:
+def parse_range_list(rngs: str | list, dictvars: dict | None = None) -> list[t.Any]:
     """Parse a string with comma-separated ranges or a list of range strings.
 
     Return a sorted list of integers in any of the ranges.
     """
     if isinstance(rngs, list):
         rngs = ",".join(rngs)
     elif not hasattr(rngs, "split"):
         return [rngs]
 
     return sorted(set(chain.from_iterable([parse_range(rng, dictvars or {}) for rng in rngs.split(",")])))
 
 
-def makelist(x: Union[None, list, Sequence, str, Path]) -> list[Any]:
+@typechecked
+def makelist(x: None | list | t.Sequence | str | Path) -> list[t.Any]:
     """If x is not a list (or is a string), make a list containing x."""
     if x is None:
         return []
-    if isinstance(x, (str, Path)):
-        return [x]
-    return list(x)
+    return [x] if isinstance(x, str | Path) else list(x)
 
 
-def trim_or_pad(requiredlength: int, *listoflistin: list[list[Any]]) -> Iterator[list[Any]]:
+def trim_or_pad(requiredlength: int, *listoflistin: list[t.Any]) -> t.Iterator[list[t.Any]]:
     """Make lists equal in length to requiredlength either by padding with None or truncating."""
     for listin in listoflistin:
         listin = makelist(listin)
 
         listout = [listin[i] if i < len(listin) else None for i in range(requiredlength)]
 
         assert len(listout) == requiredlength
         yield listout
 
 
-def flatten_list(listin: list) -> list:
+@typechecked
+def flatten_list(listin: list[t.Any]) -> list[t.Any]:
+    """Flatten a list of lists."""
     listout = []
     for elem in listin:
         if isinstance(elem, list):
             listout.extend(elem)
         else:
             listout.append(elem)
     return listout
 
 
-def zopen(filename: Union[Path, str], mode: str = "rt", encoding: Optional[str] = None) -> Any:
+@typechecked
+def zopen(filename: Path | str, mode: str = "rt", encoding: str | None = None) -> t.Any:
     """Open filename, filename.gz or filename.xz."""
     ext_fopen = [(".lz4", lz4.frame.open), (".zst", pyzstd.open), (".gz", gzip.open), (".xz", xz.open)]
 
     for ext, fopen in ext_fopen:
         file_ext = str(filename) if str(filename).endswith(ext) else str(filename) + ext
         if Path(file_ext).exists():
             return fopen(file_ext, mode=mode, encoding=encoding)
 
     # open() can raise file not found if this file doesn't exist
-    return open(filename, mode=mode, encoding=encoding)  # noqa: SIM115
+    return Path(filename).open(mode=mode, encoding=encoding)
 
 
+@typechecked
 def firstexisting(
-    filelist: Union[Sequence[Union[str, Path]], str, Path],
-    folder: Union[Path, str] = Path("."),
+    filelist: t.Sequence[str | Path] | str | Path,
+    folder: Path | str = Path(),
     tryzipped: bool = True,
 ) -> Path:
     """Return the first existing file in file list. If none exist, raise exception."""
-    if isinstance(filelist, (str, Path)):
+    if isinstance(filelist, str | Path):
         filelist = [filelist]
+    folder = Path(folder)
 
     fullpaths = []
     for filename in filelist:
         fullpaths.append(Path(folder) / filename)
 
         if tryzipped:
             for ext in [".lz4", ".zst", ".gz", ".xz"]:
                 filenameext = str(filename) if str(filename).endswith(ext) else str(filename) + ext
                 if filenameext not in filelist:
-                    fullpaths.append(Path(folder) / filenameext)
+                    fullpaths.append(folder / filenameext)
 
     for fullpath in fullpaths:
         if fullpath.exists():
             return fullpath
 
-    msg = f"None of these files exist in {folder}: {', '.join([str(x) for x in fullpaths])}"
+    filelist = "\n  ".join([str(x.relative_to(folder)) for x in fullpaths])
+    msg = f"None of these files exist in {folder}: \n  {filelist}"
     raise FileNotFoundError(msg)
 
 
 def anyexist(
-    filelist: Sequence[Union[str, Path]],
-    folder: Union[Path, str] = Path("."),
+    filelist: t.Sequence[str | Path],
+    folder: Path | str = Path(),
     tryzipped: bool = True,
 ) -> bool:
     """Return true if any files in file list exist."""
     try:
         firstexisting(filelist=filelist, folder=folder, tryzipped=tryzipped)
     except FileNotFoundError:
         return False
@@ -782,33 +789,34 @@
     while not line.strip() or line.strip().lstrip().startswith("#"):
         line = file.readline()
 
     return line
 
 
 @lru_cache(maxsize=24)
-def get_file_metadata(filepath: Union[Path, str]) -> dict[str, Any]:
+def get_file_metadata(filepath: Path | str) -> dict[str, t.Any]:
+    """Return a dict of metadata for a file, either from a metadata file or from the big combined metadata file."""
     filepath = Path(filepath)
 
-    def add_derived_metadata(metadata: dict[str, Any]) -> dict[str, Any]:
+    def add_derived_metadata(metadata: dict[str, t.Any]) -> dict[str, t.Any]:
         if "a_v" in metadata and "e_bminusv" in metadata and "r_v" not in metadata:
             metadata["r_v"] = metadata["a_v"] / metadata["e_bminusv"]
         elif "e_bminusv" in metadata and "r_v" in metadata and "a_v" not in metadata:
             metadata["a_v"] = metadata["e_bminusv"] * metadata["r_v"]
         elif "a_v" in metadata and "r_v" in metadata and "e_bminusv" not in metadata:
             metadata["e_bminusv"] = metadata["a_v"] / metadata["r_v"]
 
         return metadata
 
     import yaml
 
     filepath = Path(str(filepath).replace(".xz", "").replace(".gz", "").replace(".lz4", "").replace(".zst", ""))
 
     # check if the reference file (e.g. spectrum.txt) has an metadata file (spectrum.txt.meta.yml)
-    individualmetafile = filepath.with_suffix(filepath.suffix + ".meta.yml")
+    individualmetafile = filepath.with_suffix(f"{filepath.suffix}.meta.yml")
     if individualmetafile.exists():
         with individualmetafile.open("r") as yamlfile:
             metadata = yaml.load(yamlfile, Loader=yaml.FullLoader)
 
         return add_derived_metadata(metadata)
 
     # check if the metadata is in the big combined metadata file (todo: eliminate this file)
@@ -821,64 +829,66 @@
         return add_derived_metadata(metadata)
 
     return {}
 
 
 def get_filterfunc(
     args: argparse.Namespace, mode: str = "interp"
-) -> Optional[Callable[[Union[list[float], np.ndarray]], np.ndarray]]:
+) -> t.Callable[[list[float] | np.ndarray], np.ndarray] | None:
     """Use command line arguments to determine the appropriate filter function."""
-    filterfunc: Optional[Callable[[Union[list[float], np.ndarray]], np.ndarray]] = None
+    filterfunc: t.Callable[[list[float] | np.ndarray], np.ndarray] | None = None
     dictargs = vars(args)
 
     if dictargs.get("filtermovingavg", False):
 
-        def movavgfilterfunc(ylist: Union[list[float], np.ndarray]) -> np.ndarray:
+        def movavgfilterfunc(ylist: list[float] | np.ndarray) -> np.ndarray:
             n = args.filtermovingavg
             arr_padded = np.pad(ylist, (n // 2, n - 1 - n // 2), mode="edge")
             return np.convolve(arr_padded, np.ones((n,)) / n, mode="valid")
 
         assert filterfunc is None
         filterfunc = movavgfilterfunc
 
     if dictargs.get("filtersavgol", False):
         import scipy.signal
 
         window_length, poly_order = (int(x) for x in args.filtersavgol)
 
-        def savgolfilterfunc(ylist: Union[list[float], np.ndarray]) -> np.ndarray:
+        def savgolfilterfunc(ylist: list[float] | np.ndarray) -> np.ndarray:
             return scipy.signal.savgol_filter(ylist, window_length, poly_order, mode=mode)
 
         assert filterfunc is None
         filterfunc = savgolfilterfunc
 
         print("Applying Savitzky-Golay filter")
 
     return filterfunc
 
 
 def join_pdf_files(pdf_list: list[str], modelpath_list: list[Path]) -> None:
+    """Merge a list of PDF files into a single PDF file."""
     from PyPDF2 import PdfFileMerger
 
     merger = PdfFileMerger()
 
     for pdf, modelpath in zip(pdf_list, modelpath_list):
         fullpath = firstexisting([pdf], folder=modelpath)
-        merger.append(open(fullpath, "rb"))  # noqa: SIM115
+        merger.append(fullpath.open("rb"))
         fullpath.unlink()
 
     resultfilename = f'{pdf_list[0].split(".")[0]}-{pdf_list[-1].split(".")[0]}'
-    with open(f"{resultfilename}.pdf", "wb") as resultfile:
+    with Path(f"{resultfilename}.pdf").open("wb") as resultfile:
         merger.write(resultfile)
 
     print(f"Files merged and saved to {resultfilename}.pdf")
 
 
 @lru_cache(maxsize=2)
-def get_bflist(modelpath: Union[Path, str]) -> dict[int, tuple[int, int, int, int]]:
+def get_bflist(modelpath: Path | str) -> dict[int, tuple[int, int, int, int]]:
+    """Return a dict of bound-free transitions from bflist.out."""
     compositiondata = get_composition_data(modelpath)
     bflist = {}
     bflistpath = firstexisting(["bflist.out", "bflist.dat"], folder=modelpath, tryzipped=True)
     with zopen(bflistpath) as filein:
         bflistcount = int(filein.readline())
 
         for _ in range(bflistcount):
@@ -891,17 +901,16 @@
 
     return bflist
 
 
 linetuple = namedtuple("linetuple", "lambda_angstroms atomic_number ionstage upperlevelindex lowerlevelindex")
 
 
-def read_linestatfile(
-    filepath: Union[Path, str]
-) -> tuple[int, list[float], list[int], list[int], list[int], list[int]]:
+@typechecked
+def read_linestatfile(filepath: Path | str) -> tuple[int, list[float], list[int], list[int], list[int], list[int]]:
     """Load linestat.out containing transitions wavelength, element, ion, upper and lower levels."""
     print(f"Loading {filepath}")
 
     data = np.loadtxt(zopen(filepath))
     lambda_angstroms = data[0] * 1e8
     nlines = len(lambda_angstroms)
 
@@ -917,15 +926,15 @@
 
     lower_levels = data[4].astype(int)
     assert len(lower_levels) == nlines
 
     return nlines, lambda_angstroms, atomic_numbers, ion_stages, upper_levels, lower_levels
 
 
-def get_linelist_pldf(modelpath: Union[Path, str]) -> pl.LazyFrame:
+def get_linelist_pldf(modelpath: Path | str) -> pl.LazyFrame:
     textfile = at.firstexisting("linestat.out", folder=modelpath)
     parquetfile = Path(modelpath, "linelist.out.parquet")
     if not parquetfile.is_file() or parquetfile.stat().st_mtime < textfile.stat().st_mtime:
         _, lambda_angstroms, atomic_numbers, ion_stages, upper_levels, lower_levels = read_linestatfile(textfile)
 
         pldf = (
             pl.DataFrame(
@@ -944,36 +953,41 @@
         print(f"Saved {parquetfile}")
     else:
         print(f"Reading {parquetfile}")
 
     return pl.scan_parquet(parquetfile)
 
 
-def get_linelist_dict(modelpath: Union[Path, str]) -> dict[int, linetuple]:
+def get_linelist_dict(modelpath: Path | str) -> dict[int, linetuple]:
+    """Return a dict of line tuples from linestat.out."""
     nlines, lambda_angstroms, atomic_numbers, ion_stages, upper_levels, lower_levels = read_linestatfile(
         Path(modelpath, "linestat.out")
     )
-    linelistdict = {
+    return {
         index: linetuple(lambda_a, Z, ionstage, upper, lower)
         for index, lambda_a, Z, ionstage, upper, lower in zip(
-            range(nlines), lambda_angstroms, atomic_numbers, ion_stages, upper_levels, lower_levels
+            range(nlines),
+            lambda_angstroms,
+            atomic_numbers,
+            ion_stages,
+            upper_levels,
+            lower_levels,
         )
     }
-    return linelistdict
 
 
 @lru_cache(maxsize=8)
 def get_linelist_dataframe(
-    modelpath: Union[Path, str],
+    modelpath: Path | str,
 ) -> pd.DataFrame:
     nlines, lambda_angstroms, atomic_numbers, ion_stages, upper_levels, lower_levels = read_linestatfile(
         Path(modelpath, "linestat.out")
     )
 
-    dflinelist = pd.DataFrame(
+    return pd.DataFrame(
         {
             "lambda_angstroms": lambda_angstroms,
             "atomic_number": atomic_numbers,
             "ionstage": ion_stages,
             "upperlevelindex": upper_levels,
             "lowerlevelindex": lower_levels,
         },
@@ -981,45 +995,41 @@
             "lambda_angstroms": float,
             "atomic_number": int,
             "ionstage": int,
             "upperlevelindex": int,
             "lowerlevelindex": int,
         },
     )
-    dflinelist.index.name = "linelistindex"
-
-    return dflinelist
 
 
 @lru_cache(maxsize=8)
 def get_npts_model(modelpath: Path) -> int:
     """Return the number of cell in the model.txt."""
     modelfilepath = (
         Path(modelpath)
         if Path(modelpath).is_file()
         else at.firstexisting("model.txt", folder=modelpath, tryzipped=True)
     )
     with zopen(modelfilepath) as modelfile:
-        npts_model = int(readnoncommentline(modelfile))
-    return npts_model
+        return int(readnoncommentline(modelfile))
 
 
 @lru_cache(maxsize=8)
 def get_nprocs(modelpath: Path) -> int:
     """Return the number of MPI processes specified in input.txt."""
     return int(Path(modelpath, "input.txt").read_text().split("\n")[21].split("#")[0])
 
 
 @lru_cache(maxsize=8)
-def get_inputparams(modelpath: Path) -> dict[str, Any]:
+def get_inputparams(modelpath: Path) -> dict[str, t.Any]:
     """Return parameters specified in input.txt."""
     from astropy import constants as const
     from astropy import units as u
 
-    params: dict[str, Any] = {}
+    params: dict[str, t.Any] = {}
     with Path(modelpath, "input.txt").open("r") as inputfile:
         params["pre_zseed"] = int(readnoncommentline(inputfile).split("#")[0])
 
         # number of time steps
         params["ntstep"] = int(readnoncommentline(inputfile).split("#")[0])
 
         # number of start and end time step
@@ -1043,79 +1053,77 @@
 
         # there are more parameters in the file that are not read yet...
 
     return params
 
 
 @lru_cache(maxsize=16)
-def get_runfolder_timesteps(folderpath: Union[Path, str]) -> tuple[int, ...]:
+def get_runfolder_timesteps(folderpath: Path | str) -> tuple[int, ...]:
     """Get the set of timesteps covered by the output files in an ARTIS run folder."""
     folder_timesteps = set()
-    try:
-        with zopen(Path(folderpath, "estimators_0000.out")) as estfile:
-            restart_timestep = -1
-            for line in estfile:
-                if line.startswith("timestep "):
-                    timestep = int(line.split()[1])
-
-                    if restart_timestep < 0 and timestep != 0 and 0 not in folder_timesteps:
-                        # the first timestep of a restarted run is duplicate and should be ignored
-                        restart_timestep = timestep
+    with contextlib.suppress(FileNotFoundError), zopen(Path(folderpath, "estimators_0000.out")) as estfile:
+        restart_timestep = -1
+        for line in estfile:
+            if line.startswith("timestep "):
+                timestep = int(line.split()[1])
+
+                if restart_timestep < 0 and timestep != 0 and 0 not in folder_timesteps:
+                    # the first timestep of a restarted run is duplicate and should be ignored
+                    restart_timestep = timestep
 
-                    if timestep != restart_timestep:
-                        folder_timesteps.add(timestep)
-
-    except FileNotFoundError:
-        pass
+                if timestep != restart_timestep:
+                    folder_timesteps.add(timestep)
 
     return tuple(folder_timesteps)
 
 
+@typechecked
 def get_runfolders(
-    modelpath: Union[Path, str], timestep: Optional[int] = None, timesteps: Optional[Sequence[int]] = None
-) -> Sequence[Path]:
+    modelpath: Path | str, timestep: int | None = None, timesteps: t.Sequence[int] | None = None
+) -> t.Sequence[Path]:
     """Get a list of folders containing ARTIS output files from a modelpath, optionally with a timestep restriction.
 
     The folder list may include non-ARTIS folders if a timestep is not specified.
     """
     folderlist_all = (*sorted([child for child in Path(modelpath).iterdir() if child.is_dir()]), Path(modelpath))
-    folder_list_matching = []
     if (timestep is not None and timestep > -1) or (timesteps is not None and len(timesteps) > 0):
+        folder_list_matching = []
         for folderpath in folderlist_all:
             folder_timesteps = get_runfolder_timesteps(folderpath)
             if timesteps is None and timestep is not None and timestep in folder_timesteps:
                 return (folderpath,)
             if timesteps is not None and any(ts in folder_timesteps for ts in timesteps):
                 folder_list_matching.append(folderpath)
 
         return tuple(folder_list_matching)
 
     return [folderpath for folderpath in folderlist_all if get_runfolder_timesteps(folderpath)]
 
 
+@typechecked
 def get_mpiranklist(
-    modelpath: Union[Path, str],
-    modelgridindex: Optional[Union[Iterable[int], int]] = None,
+    modelpath: Path | str,
+    modelgridindex: t.Iterable[int] | int | None = None,
     only_ranks_withgridcells: bool = False,
-) -> Sequence[int]:
+) -> t.Sequence[int]:
     """Get a list of rank ids.
 
     - modelpath:
         pathlib.Path() to ARTIS model folder
     - modelgridindex:
         give a cell number to only return the rank number that updates this cell (and outputs its estimators)
     - only_ranks_withgridcells:
         set True to skip ranks that only update packets (i.e. that don't update any grid cells/output estimators).
     """
     if modelgridindex is None or modelgridindex == []:
         if only_ranks_withgridcells:
             return range(min(get_nprocs(modelpath), get_npts_model(modelpath)))
         return range(get_nprocs(modelpath))
 
-    if isinstance(modelgridindex, Iterable):
+    if isinstance(modelgridindex, t.Iterable):
         mpiranklist = set()
         for mgi in modelgridindex:
             if mgi < 0:
                 if only_ranks_withgridcells:
                     return range(min(get_nprocs(modelpath), get_npts_model(modelpath)))
                 return range(get_nprocs(modelpath))
 
@@ -1126,15 +1134,15 @@
     # in case modelgridindex is a single number rather than an iterable
     if modelgridindex < 0:
         return range(min(get_nprocs(modelpath), get_npts_model(modelpath)))
 
     return [get_mpirankofcell(modelgridindex, modelpath=modelpath)]
 
 
-def get_cellsofmpirank(mpirank: int, modelpath: Union[Path, str]) -> Iterable[int]:
+def get_cellsofmpirank(mpirank: int, modelpath: Path | str) -> t.Iterable[int]:
     """Return an iterable of the cell numbers processed by a given MPI rank."""
     npts_model = get_npts_model(modelpath)
     nprocs = get_nprocs(modelpath)
 
     assert mpirank < nprocs
 
     nblock = npts_model // nprocs
@@ -1147,24 +1155,23 @@
         ndo = nblock
         nstart = n_leftover + mpirank * nblock
 
     return list(range(nstart, nstart + ndo))
 
 
 @lru_cache(maxsize=16)
-def get_dfrankassignments(modelpath: Union[Path, str]) -> Optional[pd.DataFrame]:
+def get_dfrankassignments(modelpath: Path | str) -> pd.DataFrame | None:
     filerankassignments = Path(modelpath, "modelgridrankassignments.out")
     if filerankassignments.is_file():
         df = pd.read_csv(filerankassignments, delim_whitespace=True)
-        df = df.rename(columns={df.columns[0]: df.columns[0].lstrip("#")})
-        return df
+        return df.rename(columns={df.columns[0]: str(df.columns[0]).lstrip("#")})
     return None
 
 
-def get_mpirankofcell(modelgridindex: int, modelpath: Union[Path, str]) -> int:
+def get_mpirankofcell(modelgridindex: int, modelpath: Path | str) -> int:
     """Return the rank number of the MPI process responsible for handling a specified cell's updating and output."""
     modelpath = Path(modelpath)
     npts_model = get_npts_model(modelpath)
     assert modelgridindex < npts_model
 
     dfrankassignments = get_dfrankassignments(modelpath)
     if dfrankassignments is not None:
@@ -1201,15 +1208,15 @@
     return 10
 
 
 def get_viewingdirection_costhetabincount() -> int:
     return 10
 
 
-def get_phi_bins() -> tuple[np.ndarray, np.ndarray, list[str]]:
+def get_phi_bins(usedegrees: bool) -> tuple[np.ndarray, np.ndarray, list[str]]:
     nphibins = at.get_viewingdirection_phibincount()
     # pi/2 must be an exact boundary because of the change in behaviour there
     assert nphibins % 2 == 0
 
     # for historical reasons, phi bins ordered by ascending phi are
     # [0, 1, 2, 3, 4, 9, 8, 7, 6, 5] for nphibins == 10
 
@@ -1217,68 +1224,103 @@
     phisteps = list(range(nphibins // 2)) + list(reversed(range(nphibins // 2, nphibins)))
 
     phi_lower = np.array([step * 2 * math.pi / nphibins for step in phisteps])
     phi_upper = np.array([(step + 1) * 2 * math.pi / nphibins for step in phisteps])
 
     binlabels = []
     for phibin, step in enumerate(phisteps):
-        str_phi_lower = f"{step}π/{nphibins // 2}" if step > 0 else "0"
+        if usedegrees:
+            str_phi_lower = f"{phi_lower[step]/math.pi*180:.0f}°"
+            str_phi_upper = f"{phi_upper[step]/math.pi*180:.0f}°"
+        else:
+            str_phi_lower = f"{step}π/{nphibins // 2}" if step > 0 else "0"
+            str_phi_upper = f"{step+1}π/{nphibins // 2}" if step < nphibins - 1 else "2π"
+
         lower_compare = "≤" if phibin < (nphibins // 2) else "<"
-        str_phi_upper = f"{step+1}π/{nphibins // 2}" if step < nphibins - 1 else "2π"
         upper_compare = "≤" if phibin > (nphibins // 2) else "<"
         binlabels.append(f"{str_phi_lower} {lower_compare} ϕ {upper_compare} {str_phi_upper}")
 
     return phi_lower, phi_upper, binlabels
 
 
-def get_costheta_bins() -> tuple[np.ndarray, np.ndarray, list[str]]:
+def get_costheta_bins(usedegrees: bool, usepiminustheta: bool = False) -> tuple[np.ndarray, np.ndarray, list[str]]:
     ncosthetabins = at.get_viewingdirection_costhetabincount()
     costhetabins_lower = np.arange(-1.0, 1.0, 2.0 / ncosthetabins)
     costhetabins_upper = costhetabins_lower + 2.0 / ncosthetabins
-    binlabels = [f"{lower:.1f} ≤ cos θ < {upper:.1f}" for lower, upper in zip(costhetabins_lower, costhetabins_upper)]
+    if usedegrees:
+        if usepiminustheta:
+            thetabins_upper = (np.pi - np.arccos(costhetabins_upper)) / np.pi * 180
+            thetabins_lower = (np.pi - np.arccos(costhetabins_lower)) / np.pi * 180
+            binlabels = [
+                rf"{lower:.0f}° < $\pi$-$\theta$ < {upper:.0f}°"
+                for lower, upper in zip(thetabins_lower, thetabins_upper)
+            ]
+        else:
+            thetabins_upper = np.arccos(costhetabins_lower) / np.pi * 180
+            thetabins_lower = np.arccos(costhetabins_upper) / np.pi * 180
+
+            binlabels = [f"{lower:.0f}° < θ < {upper:.0f}°" for lower, upper in zip(thetabins_lower, thetabins_upper)]
+    else:
+        binlabels = [
+            f"{lower:.1f} ≤ cos θ < {upper:.1f}" for lower, upper in zip(costhetabins_lower, costhetabins_upper)
+        ]
     return costhetabins_lower, costhetabins_upper, binlabels
 
 
-def get_costhetabin_phibin_labels() -> tuple[list[str], list[str]]:
-    _, _, costhetabinlabels = get_costheta_bins()
-    _, _, phibinlabels = get_phi_bins()
+def get_costhetabin_phibin_labels(usedegrees: bool) -> tuple[list[str], list[str]]:
+    _, _, costhetabinlabels = get_costheta_bins(usedegrees=usedegrees)
+    _, _, phibinlabels = get_phi_bins(usedegrees=usedegrees)
     return costhetabinlabels, phibinlabels
 
 
-def get_vspec_dir_labels(modelpath: Union[str, Path], viewinganglelabelunits: str = "rad") -> dict[int, str]:
+def get_vspec_dir_labels(modelpath: str | Path, viewinganglelabelunits: str = "rad") -> dict[int, str]:
     vpkt_config = at.get_vpkt_config(modelpath)
     dirlabels = {}
     for dirindex in range(vpkt_config["nobsdirections"]):
         phi_angle = round(vpkt_config["phi"][dirindex])
         if viewinganglelabelunits == "deg":
             theta_angle = round(math.degrees(math.acos(vpkt_config["cos_theta"][dirindex])))
             dirlabels[dirindex] = rf"v$\theta$ = {theta_angle}$^\circ$, $\phi$ = {phi_angle}$^\circ$"
         elif viewinganglelabelunits == "rad":
             dirlabels[dirindex] = rf"cos $\theta$ = {vpkt_config['cos_theta'][dirindex]}, $\phi$ = {phi_angle}$^\circ$"
     return dirlabels
 
 
 def get_dirbin_labels(
-    dirbins: Union[np.ndarray[Any, np.dtype[Any]], Sequence[int]],
-    modelpath: Union[Path, str, None] = None,
+    dirbins: np.ndarray[t.Any, np.dtype[t.Any]] | t.Sequence[int] | None = None,
+    modelpath: Path | str | None = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
+    usedegrees: bool = False,
+    usepiminustheta: bool = False,
 ) -> dict[int, str]:
+    """Return a dict of text labels for viewing direction bins."""
     if modelpath:
         modelpath = Path(modelpath)
         MABINS = at.get_viewingdirectionbincount()
-        if len(list(Path(modelpath).glob("*_res_00.out*"))) > 0:  # if the first direction bin file exists
-            assert len(list(Path(modelpath).glob(f"*_res_{MABINS-1:02d}.out*"))) > 0  # check last bin exists
-            assert len(list(Path(modelpath).glob(f"*_res_{MABINS:02d}.out*"))) == 0  # check one beyond does not exist
+        if list(modelpath.glob("*_res_00.out*")):
+            # if the first direction bin file exists, check:
+            # check last bin exists
+            assert list(modelpath.glob(f"*_res_{MABINS-1:02d}.out*"))
+            # check one beyond does not exist
+            assert not list(modelpath.glob(f"*_res_{MABINS:02d}.out*"))
 
-    _, _, costhetabinlabels = get_costheta_bins()
-    _, _, phibinlabels = get_phi_bins()
+    _, _, costhetabinlabels = get_costheta_bins(usedegrees=usedegrees, usepiminustheta=usepiminustheta)
+    _, _, phibinlabels = get_phi_bins(usedegrees=usedegrees)
 
     nphibins = at.get_viewingdirection_phibincount()
 
+    if dirbins is None:
+        if average_over_phi:
+            dirbins = np.arange(at.get_viewingdirection_costhetabincount()) * 10
+        elif average_over_theta:
+            dirbins = np.arange(nphibins)
+        else:
+            dirbins = np.arange(at.get_viewingdirectionbincount())
+
     angle_definitions: dict[int, str] = {}
     for dirbin in dirbins:
         if dirbin == -1:
             angle_definitions[dirbin] = ""
             continue
 
         costheta_index = dirbin // nphibins
```

### Comparing `artistools-2023.5.16.3/artistools/nltepops/nltepops.py` & `artistools-2023.8.1/artistools/nltepops/nltepops.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Artistools - NLTE population related functions."""
+from __future__ import annotations
+
 import math
 import multiprocessing
 import re
 from functools import lru_cache
 from functools import partial
 from pathlib import Path
-from typing import Optional
-from typing import Union
 
 import pandas as pd
 from astropy import constants as const
 
 import artistools as at
-from artistools.configuration import get_config
 
 
 def texifyterm(strterm: str) -> str:
     """Replace a term string with TeX notation equivalent."""
     strtermtex = ""
     passed_term_Lchar = False
 
@@ -35,16 +34,15 @@
         elif re.match(r"[0-9]?.*\]", termpiece) is not None:
             # J value
             strtermtex += termpiece.split("[")[0] + r"$_{" + termpiece.lstrip("0123456789").strip("[]") + r"}$"
         elif re.match("[0-9]", termpiece) is not None and passed_term_Lchar:
             # extra number after S char
             strtermtex += termpiece
 
-    strtermtex = strtermtex.replace("$$", "")
-    return strtermtex
+    return strtermtex.replace("$$", "")
 
 
 def texifyconfiguration(levelname: str) -> str:
     """Replace a level configuration with the formatted LaTeX equivalent."""
     # the underscore gets confused with LaTeX subscript operator, so switch it to the hash symbol
     strout = "#".join(levelname.split("_")[:-1]) + "#"
     for strorbitalocc in re.findall(r"[0-9][a-z][0-9]?[#(]", strout):
@@ -57,17 +55,15 @@
     for parentterm in re.findall(r"\([0-9][A-Z][^)]?\)", strout):
         parentermtex = f'({texifyterm(parentterm.strip("()"))})'
         strout = strout.replace(parentterm, parentermtex)
     strterm = levelname.split("_")[-1]
     strout += " " + texifyterm(strterm)
 
     strout = strout.replace("#", "")
-    strout = strout.replace("$$", "")
-    # print(f"Replacing levelname '{levelname}' with '{strout}'")
-    return strout
+    return strout.replace("$$", "")
 
 
 def add_lte_pops(modelpath, dfpop, columntemperature_tuples, noprint=False, maxlevel=-1):
     """Add columns to dfpop with LTE populations.
 
     columntemperature_tuples is a sequence of tuples of column name and temperature, e.g., ('mycolumn', 3000)
     """
@@ -141,19 +137,19 @@
                     )
 
             dfpop.loc[masksuperlevel, "level"] = levelnumber_sl + 2
 
     return dfpop
 
 
-def read_file(nltefilepath: Union[str, Path]) -> pd.DataFrame:
+def read_file(nltefilepath: str | Path) -> pd.DataFrame:
     """Read NLTE populations from one file."""
     if not Path(nltefilepath).is_file():
-        nltefilepathgz = Path(str(nltefilepath) + ".gz")
-        nltefilepathxz = Path(str(nltefilepath) + ".xz")
+        nltefilepathgz = Path(f"{nltefilepath!s}.gz")
+        nltefilepathxz = Path(f"{nltefilepath!s}.xz")
         if nltefilepathxz.is_file():
             nltefilepath = nltefilepathxz
         elif nltefilepathgz.is_file():
             nltefilepath = nltefilepathgz
         else:
             # print(f'Warning: Could not find {nltefilepath}')
             return pd.DataFrame()
@@ -176,15 +172,15 @@
         dfpopfile = dfpopfile.query(strquery, local_dict=dfqueryvars)
 
     return dfpopfile
 
 
 @lru_cache(maxsize=2)
 def read_files(
-    modelpath, timestep=-1, modelgridindex=-1, dfquery=None, dfqueryvars: Optional[dict] = None
+    modelpath, timestep=-1, modelgridindex=-1, dfquery=None, dfqueryvars: dict | None = None
 ) -> pd.DataFrame:
     """Read in NLTE populations from a model for a particular timestep and grid cell."""
     if dfqueryvars is None:
         dfqueryvars = {}
 
     mpiranklist = at.get_mpiranklist(modelpath, modelgridindex=modelgridindex)
 
@@ -195,35 +191,30 @@
         for folderpath in at.get_runfolders(modelpath, timestep=timestep)
         for mpirank in mpiranklist
     ]
 
     dfqueryvars["modelgridindex"] = modelgridindex
     dfqueryvars["timestep"] = timestep
 
-    dfquery_full = ""
-    if timestep >= 0:
-        dfquery_full = "timestep==@timestep"
-
+    dfquery_full = "timestep==@timestep" if timestep >= 0 else ""
     if modelgridindex >= 0:
         if dfquery_full:
             dfquery_full += " and "
         dfquery_full += "modelgridindex==@modelgridindex"
 
     if dfquery:
         if dfquery_full:
             dfquery_full = f"({dfquery_full}) and "
         dfquery_full += f"({dfquery})"
 
-    if get_config()["num_processes"] > 1:
-        with multiprocessing.get_context("fork").Pool(processes=get_config()["num_processes"]) as pool:
+    if at.get_config()["num_processes"] > 1:
+        with multiprocessing.get_context("fork").Pool(processes=at.get_config()["num_processes"]) as pool:
             arr_dfnltepop = pool.map(
                 partial(read_file_filtered, strquery=dfquery_full, dfqueryvars=dfqueryvars), nltefilepaths
             )
             pool.close()
             pool.join()
             pool.terminate()
     else:
         arr_dfnltepop = [read_file_filtered(f, strquery=dfquery_full, dfqueryvars=dfqueryvars) for f in nltefilepaths]
 
-    dfpop = pd.concat(arr_dfnltepop).copy()
-
-    return dfpop
+    return pd.concat(arr_dfnltepop).copy()
```

### Comparing `artistools-2023.5.16.3/artistools/nltepops/plotnltepops.py` & `artistools-2023.8.1/artistools/nltepops/plotnltepops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 #!/usr/bin/env python3
 """Artistools - NLTE population related functions."""
+
+from __future__ import annotations
+
 import argparse
+import contextlib
 import math
-import os
 import sys
 from pathlib import Path
-from typing import Union
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from astropy import constants as const
 from matplotlib import ticker
 
 import artistools as at
 
 defaultoutputfile = "plotnlte_{elsymbol}_cell{cell:03d}_ts{timestep:02d}_{time_days:.0f}d.pdf"
 
 
-def annotate_emission_line(ax, y, upperlevel, lowerlevel, label):
+def annotate_emission_line(ax: plt.Axes, y: float, upperlevel: int, lowerlevel: int, label: str) -> None:
     ax.annotate(
         "",
         xy=(lowerlevel, y),
         xycoords=("data", "axes fraction"),
         xytext=(upperlevel, y),
         textcoords=("data", "axes fraction"),
         arrowprops={"facecolor": "black", "width": 0.1, "headwidth": 6},
@@ -35,15 +37,15 @@
         xycoords=("data", "axes fraction"),
         size=10,
         va="bottom",
         ha="center",
     )
 
 
-def plot_reference_data(ax, atomic_number, ion_stage, estimators_celltimestep, dfpopthision, annotatelines):
+def plot_reference_data(ax, atomic_number: int, ion_stage: int, estimators_celltimestep, dfpopthision, annotatelines):
     nne, Te, TR, W = (estimators_celltimestep[s] for s in ["nne", "Te", "TR", "W"])
     # comparison to Chianti file
     elsym = at.get_elsymbol(atomic_number)
     elsymlower = elsym.lower()
     if Path("data", f"{elsymlower}_{ion_stage}-levelmap.txt").exists():
         # ax.set_ylim(bottom=2e-3)
         # ax.set_ylim(top=4)
@@ -76,26 +78,24 @@
                     print(f"Plotting reference data from {depfilepath},")
                     print(
                         f"nne = {file_nne} (ARTIS {nne}) cm^-3, Te = {file_Te} (ARTIS {Te}) K, "
                         f"TR = {file_TR} (ARTIS {TR}) K, W = {file_W} (ARTIS {W})"
                     )
                     levelnums = []
                     depcoeffs = []
-                    firstdep = -1
+                    firstdep = -1.0
                     for line in depfile:
                         row = line.split()
-                        try:
+                        with contextlib.suppress(KeyError, IndexError, ValueError):
                             levelnum = levelnumofconfigterm[(row[1], row[2])]
                             if levelnum in dfpopthision["level"].to_numpy():
                                 levelnums.append(levelnum)
                                 if firstdep < 0:
                                     firstdep = float(row[0])
                                 depcoeffs.append(float(row[0]) / firstdep)
-                        except (KeyError, IndexError, ValueError):
-                            pass
                     ionstr = at.get_ionstring(atomic_number, ion_stage, spectral=False)
                     ax.plot(
                         levelnums,
                         depcoeffs,
                         linewidth=1.5,
                         color=color,
                         label=f"{ionstr} CHIANTI NLTE{bbstr}",
@@ -116,15 +116,15 @@
 
 def get_floers_data(dfpopthision, atomic_number, ion_stage, modelpath, T_e, modelgridindex):
     floers_levelnums, floers_levelpop_values = None, None
 
     # comparison to Andeas Floers's NLTE pops for Shingles et al. (2022)
     if atomic_number == 26 and ion_stage in [2, 3]:
         floersfilename = "andreas_level_populations_fe2.txt" if ion_stage == 2 else "andreas_level_populations_fe3.txt"
-        if os.path.isfile(modelpath / floersfilename):
+        if Path(modelpath / floersfilename).is_file():
             print(f"reading {floersfilename}")
             floers_levelpops = pd.read_csv(modelpath / floersfilename, comment="#", delim_whitespace=True)
             # floers_levelnums = floers_levelpops['index'].values - 1
             floers_levelpops = floers_levelpops.sort_values(by="energypercm")
             floers_levelnums = list(range(len(floers_levelpops)))
             floers_levelpop_values = floers_levelpops["frac_ionpop"].to_numpy() * dfpopthision["n_NLTE"].sum()
 
@@ -143,16 +143,16 @@
             elif "lossboost8x" in modelpath.parts[-1]:
                 print("Shen2018 SubMch lossboost8x detected")
                 floersmultizonefilename = "level_pops_subch_shen2018_electronlossboost8x-247d.csv"
             elif "lossboost" not in modelpath.parts[-1]:
                 print("Shen2018 SubMch detected")
                 floersmultizonefilename = "level_pops_subch_shen2018-247d.csv"
 
-        if floersmultizonefilename and os.path.isfile(floersmultizonefilename):
-            modeldata, _ = at.inputmodel.get_modeldata(modelpath)  # todo: move into modelpath loop
+        if floersmultizonefilename and Path(floersmultizonefilename).is_file():
+            modeldata, _ = at.inputmodel.get_modeldata(modelpath)  # TODO: move into modelpath loop
             vel_outer = modeldata.iloc[modelgridindex].velocity_outer
             print(f"  reading {floersmultizonefilename}", vel_outer, T_e)
             dffloers = pd.read_csv(floersmultizonefilename)
             for _, row in dffloers.iterrows():
                 if abs(row["vel_outer"] - vel_outer) < 0.5:
                     print(f"  ARTIS cell vel_outter: {vel_outer}, Floersfile: {row['vel_outer']}")
                     print(f"  ARTIS cell Te: {T_e}, Floersfile: {row['Te']}")
@@ -180,18 +180,16 @@
     args,
     lastsubplot,
 ):
     """Plot the level populations the specified ion, cell, and timestep."""
     ionstr = at.get_ionstring(atomic_number, ion_stage, spectral=False)
 
     dfpopthision = dfpop.query(
-        (
-            "modelgridindex == @modelgridindex and timestep == @timestep "
-            "and Z == @atomic_number and ion_stage == @ion_stage"
-        ),
+        "modelgridindex == @modelgridindex and timestep == @timestep "
+        "and Z == @atomic_number and ion_stage == @ion_stage",
         inplace=False,
     ).copy()
 
     lte_columns = [("n_LTE_T_e", T_e)]
     if not args.hide_lte_tr:
         lte_columns.append(("n_LTE_T_R", T_R))
 
@@ -419,15 +417,15 @@
         plot_populations_with_time_or_velocity(
             axis, modelpaths, timedays, ionstage, ionlevels, Z, levelconfignames, args
         )
 
     labelfontsize = 20
     if args.x == "time":
         xlabel = "Time Since Explosion [days]"
-    if args.x == "velocity":
+    elif args.x == "velocity":
         xlabel = r"Zone outer velocity [km s$^{-1}$]"
     ylabel = r"Level population [cm$^{-3}$]"
 
     at.plottools.set_axis_labels(fig, ax, xlabel, ylabel, labelfontsize, args)
     if args.subplots:
         for plotnumber, axis in enumerate(ax):
             axis.set_yscale("log")
@@ -440,15 +438,15 @@
         ax.legend(loc="best", frameon=True, fontsize="x-small", ncol=1)
         ax.set_yscale("log")
 
     if not args.notitle:
         title = f"Z={Z}, ionstage={ionstage}"
         if args.x == "time":
             title = title + f", mgi = {args.modelgridindex[0]}"
-        if args.x == "velocity":
+        elif args.x == "velocity":
             title = title + f", {args.timedays} days"
         plt.title(title)
 
     at.plottools.set_axis_properties(ax, args)
 
     figname = f"plotnltelevelpopsZ{Z}.pdf"
     plt.savefig(modelpaths[0] / figname, format="pdf")
@@ -463,15 +461,15 @@
             print("Please specify modelgridindex")
             sys.exit(1)
 
         modelgridindex_list = np.ones_like(timesteps)
         modelgridindex_list = modelgridindex_list * int(args.modelgridindex[0])
 
     if args.x == "velocity":
-        modeldata, _ = at.inputmodel.get_modeldata(modelpaths[0])  # todo: move into modelpath loop
+        modeldata, _ = at.inputmodel.get_modeldata(modelpaths[0])  # TODO: move into modelpath loop
         velocity = modeldata["velocity_outer"]
         modelgridindex_list = [mgi for mgi, _ in enumerate(velocity)]
 
         timesteps = np.ones_like(modelgridindex_list)
         timesteps = timesteps * at.get_timestep_of_timedays(modelpaths[0], timedays)
 
     markers = ["o", "x", "^", "s", "8"]
@@ -599,15 +597,15 @@
 
         # top_ion = 9999
         max_ion_stage = dfpop.ion_stage.max()
 
         if len(dfpop.query("ion_stage == @max_ion_stage")) == 1:  # single-level ion, so skip it
             max_ion_stage -= 1
 
-        # timearray = at.get_timestep_times_float(modelpath)
+        # timearray = at.get_timestep_times(modelpath)
         nne = estimators[(timestep, modelgridindex)]["nne"]
         W = estimators[(timestep, modelgridindex)]["W"]
 
         subplot_title = f"{modelname}"
         if len(modelname) > 10:
             subplot_title += "\n"
         velocity = at.inputmodel.get_modeldata_tuple(modelpath)[0]["velocity_outer"][modelgridindex]
@@ -616,15 +614,15 @@
         try:
             time_days = float(at.get_timestep_time(modelpath, timestep))
         except FileNotFoundError:
             time_days = 0
             subplot_title += f" timestep {timestep:d}"
         else:
             subplot_title += f" {time_days:.0f}d"
-        subplot_title += rf" (Te={T_e:.0f} K, nne={nne:.1e} cm$^{-3}$, T$_R$={T_R:.0f} K, W={W:.1e})"
+        subplot_title += rf" (Te={T_e:.0f} K, nne={nne:.1e} cm$^{{-3}}$, T$_R$={T_R:.0f} K, W={W:.1e})"
 
         if not args.notitle:
             axes[mgifirstaxindex].set_title(subplot_title, fontsize=10)
 
         for ax, ion_stage in zip(axes[mgifirstaxindex : mgilastaxindex + 1], ion_stage_list):
             ion_data = adata.query("Z == @atomic_number and ion_stage == @ion_stage").iloc[0]
             lastsubplot = modelgridindex == mgilist[-1] and ion_stage == ion_stage_list[-1]
@@ -744,66 +742,57 @@
         parser = argparse.ArgumentParser(description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     at.set_mpl_style()
 
+    modelpath = args.modelpath
     if args.x in ["time", "velocity"]:
-        # if len(args.modelpath) == 1:
-        #     modelpath = args.modelpath
-        modelpath = args.modelpath
         args.modelpath = [args.modelpath]
 
         # if not args.timedays:
         #     print("Please specify time range with -timedays")
         #     sys.exit(1)
         if not args.ionstages:
             print("Please specify ionstage")
             sys.exit(1)
         if not args.levels:
             print("Please specify levels")
             sys.exit(1)
-    else:
-        modelpath = args.modelpath
 
     if args.timedays:
         if "-" in args.timedays:
             args.timestepmin, args.timestepmax, time_days_lower, time_days_upper = at.get_time_range(
                 modelpath, timedays_range_str=args.timedays
             )
         else:
-            timestep = at.get_timestep_of_timedays(modelpath, args.timedays)  # todo: use args.timestep instead
+            timestep = at.get_timestep_of_timedays(modelpath, args.timedays)  # TODO: use args.timestep instead
             args.timestep = at.get_timestep_of_timedays(modelpath, args.timedays)
     elif args.timedayslist:
         print(args.timedayslist)
     else:
         timestep = int(args.timestep)
 
-    if os.path.isdir(args.outputfile):
-        args.outputfile = os.path.join(args.outputfile, defaultoutputfile)
+    if Path(args.outputfile).is_dir():
+        args.outputfile = Path(args.outputfile, defaultoutputfile)
 
     ionstages_permitted = at.parse_range_list(args.ionstages) if args.ionstages else None
 
     if isinstance(args.modelgridindex, str):
         args.modelgridindex = [args.modelgridindex]
 
     if isinstance(args.elements, str):
         args.elements = [args.elements]
 
-    if isinstance(args.velocity, (float, int)):
+    if isinstance(args.velocity, float | int):
         args.velocity = [args.velocity]
 
-    mgilist: list[Union[int, float]] = []
-    for mgi in args.modelgridindex:
-        mgilist.append(int(mgi))
-
-    for vel in args.velocity:
-        mgilist.append(at.inputmodel.get_mgi_of_velocity_kms(modelpath, vel))
-
+    mgilist: list[int | float] = [int(mgi) for mgi in args.modelgridindex]
+    mgilist.extend(at.inputmodel.get_mgi_of_velocity_kms(modelpath, vel) for vel in args.velocity)
     if not mgilist:
         mgilist.append(0)
 
     if args.x in ["time", "velocity"]:
         make_plot_populations_with_time_or_velocity(args.modelpath, args)
         return
```

### Comparing `artistools-2023.5.16.3/artistools/nonthermal/__init__.py` & `artistools-2023.8.1/artistools/nonthermal/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/nonthermal/_nonthermal_core.py` & `artistools-2023.8.1/artistools/nonthermal/_nonthermal_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
+from __future__ import annotations
+
 import math
-import os
 from collections import namedtuple
 from math import atan
 from pathlib import Path
-from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 import artistools as at
 from artistools.configuration import get_config
@@ -16,15 +16,14 @@
 # cgs units to match artis
 EV = 1.6021772e-12  # in erg
 H = 6.6260755e-27
 ME = 9.1093897e-28
 QE = 4.80325e-10
 H_ionpot = 13.5979996 * EV
 CLIGHT = 2.99792458e10
-PI = math.pi
 
 use_collstrengths = False
 
 
 def get_nntot(ions: list[tuple[int, int]], ionpopdict: dict[tuple[int, int], float]) -> float:
     # total number density of all nuclei [cm^-3]
     nntot = 0.0
@@ -76,20 +75,20 @@
 
     return nnetot
 
 
 def read_binding_energies(modelpath: str = ".") -> np.ndarray:
     collionfilename = at.firstexisting(
         [
-            os.path.join(modelpath, "binding_energies.txt"),
-            os.path.join(get_config()["path_artistools_dir"], "data", "binding_energies.txt"),
+            Path(modelpath, "binding_energies.txt"),
+            Path(get_config()["path_artistools_dir"], "data", "binding_energies.txt"),
         ]
     )
 
-    with open(collionfilename) as f:
+    with collionfilename.open() as f:
         nt_shells, n_z_binding = (int(x) for x in f.readline().split())
         electron_binding = np.zeros((n_z_binding, nt_shells))
 
         for i in range(n_z_binding):
             electron_binding[i] = np.array([float(x) for x in f.readline().split()]) * EV
 
     return electron_binding
@@ -167,18 +166,15 @@
                 # is for 8 (corresponding to that shell) then just use the M4 value
                 print(
                     "WARNING: I'm trying to use a binding energy when I have no data. "
                     f"element {atomic_number} ionstage {ion_stage}\n"
                 )
                 assert electron_loop == 8
                 # print("Z = %d, ion_stage = %d\n", get_element(element), get_ionstage(element, ion));
-        if use2 < use3:
-            total += electronsinshell / use3
-        else:
-            total += electronsinshell / use2
+        total += electronsinshell / use3 if use2 < use3 else electronsinshell / use2
         # print("total total)
 
     return total
 
 
 def get_mean_binding_energy_alt(atomic_number, ion_stage, electron_binding, ionpot_ev):
     # LJS: this should be mean binding energy [erg] per electron
@@ -202,19 +198,15 @@
                 # is for 8 (corresponding to that shell) then just use the M4 value
                 print(
                     "WARNING: I'm trying to use a binding energy when I have no data. "
                     f"element {atomic_number} ionstage {ion_stage}\n"
                 )
                 assert electron_loop == 8
                 # print("Z = %d, ion_stage = %d\n", get_element(element), get_ionstage(element, ion));
-        if use2 < use3:
-            total += electronsinshell * use3
-        else:
-            total += electronsinshell * use2
-
+        total += electronsinshell * use3 if use2 < use3 else electronsinshell * use2
     assert ecount == (atomic_number - ion_stage + 1)
 
     return total / ecount
 
 
 def get_lotz_xs_ionisation(atomic_number, ion_stage, electron_binding, ionpot_ev, en_ev):
     # Axelrod 1980 Eq 3.38
@@ -244,15 +236,15 @@
                 print(
                     "WARNING: I'm trying to use a binding energy when I have no data. "
                     f"element {atomic_number} ionstage {ion_stage}\n"
                 )
                 assert electron_loop == 8
                 # print("Z = %d, ion_stage = %d\n", get_element(element), get_ionstage(element, ion));
 
-        p = use3 if use2 < use3 else use2
+        p = max(use2, use3)
 
         if 0.5 * beta**2 * ME * CLIGHT**2 > p:
             part_sigma += (
                 electronsinshell
                 / p
                 * (math.log(beta**2 * ME * CLIGHT**2 / 2.0 / p) - math.log10(1 - beta**2) - beta**2)
             )
@@ -348,19 +340,15 @@
         1e-14
         * (A * (1 - 1 / u) + B * pow((1 - 1 / u), 2) + C * math.log(u) + D * math.log(u) / u)
         / (u * pow(ionpot_ev, 2))
     )
 
 
 def get_arxs_array_shell(arr_enev, shell):
-    ar_xs_array = np.array(
-        [ar_xs(energy_ev, shell.ionpot_ev, shell.A, shell.B, shell.C, shell.D) for energy_ev in arr_enev]
-    )
-
-    return ar_xs_array
+    return np.array([ar_xs(energy_ev, shell.ionpot_ev, shell.A, shell.B, shell.C, shell.D) for energy_ev in arr_enev])
 
 
 def get_arxs_array_ion(arr_enev, dfcollion, Z, ionstage):
     ar_xs_array = np.zeros(len(arr_enev))
     dfcollion_thision = dfcollion.query("Z == @Z and ionstage == @ionstage")
     for _index, shell in dfcollion_thision.iterrows():
         ar_xs_array += get_arxs_array_shell(arr_enev, shell)
@@ -454,30 +442,28 @@
                 xs_excitation_vec[j] = constantfactor * g_bar / U
     else:
         xs_excitation_vec[startindex:] = 0.0
 
     return xs_excitation_vec
 
 
-def read_colliondata(collionfilename="collion.txt", modelpath: Union[None, str, Path] = None):
+def read_colliondata(collionfilename="collion.txt", modelpath: None | str | Path = None):
     if modelpath is None:
         modelpath = get_config()["path_datadir"]
 
     collionrow = namedtuple("collionrow", ["Z", "nelec", "n", "l", "ionpot_ev", "A", "B", "C", "D"])
 
     nrows = -1
-    with open(Path(modelpath, collionfilename)) as collionfile:
+    with Path(modelpath, collionfilename).open() as collionfile:
         nrows = int(collionfile.readline().strip())
         # print(f'Collionfile: expecting {nrows} rows')
         dfcollion = pd.read_csv(collionfile, delim_whitespace=True, header=None, names=collionrow._fields)
 
     # assert len(dfcollion) == nrows  # artis enforces this, but last 10 rows were not inportant anyway (high ionized Ni)
-    dfcollion = dfcollion.eval("ionstage = Z - nelec + 1")
-
-    return dfcollion
+    return dfcollion.eval("ionstage = Z - nelec + 1")
 
 
 def calculate_nt_frac_excitation(engrid, dftransitions, yvec, deposition_density_ev):
     # Kozma & Fransson equation 4, but summed over all transitions for given ion
     # integral in Kozma & Fransson equation 9
     deltaen = engrid[1] - engrid[0]
     npts = len(engrid)
@@ -495,36 +481,24 @@
     # find energy bin lower boundary is less than or equal to search value
     # assert en_ev >= engrid[0]
     deltaen = engrid[1] - engrid[0]
     # assert en_ev < (engrid[-1] + deltaen)
 
     index = math.floor((en_ev - engrid[0]) / deltaen)
 
-    if index < 0:
-        return 0
-
-    if index > len(engrid) - 1:
-        return len(engrid) - 1
-
-    return index
+    return 0 if index < 0 else min(index, len(engrid) - 1)
 
 
 def get_energyindex_gteq(en_ev, engrid):
     # find energy bin lower boundary is greater than or equal to search value
     deltaen = engrid[1] - engrid[0]
 
     index = math.ceil((en_ev - engrid[0]) / deltaen)
 
-    if index < 0:
-        return 0
-
-    if index > len(engrid) - 1:
-        return len(engrid) - 1
-
-    return index
+    return 0 if index < 0 else min(index, len(engrid) - 1)
 
 
 def calculate_N_e(energy_ev, engrid, ions, ionpopdict, dfcollion, yvec, dftransitions, noexcitation):
     # Kozma & Fransson equation 6.
     # Something related to a number of electrons, needed to calculate the heating fraction in equation 3
     # not valid for energy > E_0
     if energy_ev == 0.0:
@@ -536,18 +510,18 @@
 
     for Z, ionstage in ions:
         N_e_ion = 0.0
         nnion = ionpopdict[(Z, ionstage)]
 
         if not noexcitation and (Z, ionstage) in dftransitions:
             for _, row in dftransitions[(Z, ionstage)].iterrows():
-                nnlevel = row.lower_pop
                 epsilon_trans_ev = row.epsilon_trans_ev
                 if energy_ev + epsilon_trans_ev >= engrid[0]:
                     i = get_energyindex_lteq(en_ev=energy_ev + epsilon_trans_ev, engrid=engrid)
+                    nnlevel = row.lower_pop
                     N_e_ion += (nnlevel / nnion) * yvec[i] * get_xs_excitation(engrid[i], row)
                     # enbelow = engrid[i]
                     # enabove = engrid[i + 1]
                     # x = (energy_ev - enbelow) / (enabove - enbelow)
                     # yvecinterp = (1 - x) * yvec[i] + x * yvec[i + 1]
                     # N_e_ion += (nnlevel / nnion) * yvecinterp * get_xs_excitation(energy_ev + epsilon_trans_ev, row)
 
@@ -582,20 +556,23 @@
                 # x = (energy_ev - enbelow) / (enabove - enbelow)
                 # yvecinterp = (1 - x) * yvec[k] + x * yvec[k + 1]
                 # N_e_ion += deltaen * yvecinterp * xs * Psecondary(e_p=energy_ev + endash, epsilon=endash, ionpot_ev=ionpot_ev, J=J)
 
             # integral from 2E + I up to E_max
             integral2startindex = get_energyindex_lteq(en_ev=2 * energy_ev + ionpot_ev, engrid=engrid)
             N_e_ion += deltaen * sum(
-                [
-                    yvec[j]
-                    * ar_xs_array[j]
-                    * Psecondary(e_p=engrid[j], epsilon=energy_ev + ionpot_ev, ionpot_ev=ionpot_ev, J=J)
-                    for j in range(integral2startindex, len(engrid))
-                ]
+                yvec[j]
+                * ar_xs_array[j]
+                * Psecondary(
+                    e_p=engrid[j],
+                    epsilon=energy_ev + ionpot_ev,
+                    ionpot_ev=ionpot_ev,
+                    J=J,
+                )
+                for j in range(integral2startindex, len(engrid))
             )
 
         N_e += nnion * N_e_ion
 
     # source term not here because it should be zero at the low end anyway
 
     return N_e
@@ -607,15 +584,15 @@
     # Kozma & Fransson equation 8
 
     frac_heating = 0.0
     E_0 = engrid[0]
 
     deltaen = engrid[1] - engrid[0]
     frac_heating += (
-        deltaen / deposition_density_ev * sum([lossfunction(en_ev, nne) * yvec[i] for i, en_ev in enumerate(engrid)])
+        deltaen / deposition_density_ev * sum(lossfunction(en_ev, nne) * yvec[i] for i, en_ev in enumerate(engrid))
     )
 
     frac_heating_E_0_part = E_0 * yvec[0] * lossfunction(E_0, nne) / deposition_density_ev
 
     frac_heating += frac_heating_E_0_part
 
     print(f"            frac_heating E_0 * y * l(E_0) part: {frac_heating_E_0_part:.5f}")
@@ -637,24 +614,24 @@
 
     return frac_heating
 
 
 def sfmatrix_add_excitation(engrid, dftransitions_ion, nnion, sfmatrix):
     deltaen = engrid[1] - engrid[0]
     for _, row in dftransitions_ion.iterrows():
-        nnlevel = row.lower_pop
         epsilon_trans_ev = row.epsilon_trans_ev
         if epsilon_trans_ev >= engrid[0]:
+            nnlevel = row.lower_pop
             vec_xs_excitation_nnlevel_deltae = nnlevel * deltaen * get_xs_excitation_vector(engrid, row)
             xsstartindex = get_energyindex_lteq(en_ev=epsilon_trans_ev, engrid=engrid)
 
             for i, en in enumerate(engrid):
                 stopindex = get_energyindex_lteq(en_ev=en + epsilon_trans_ev, engrid=engrid)
 
-                startindex = i if i > xsstartindex else xsstartindex
+                startindex = max(i, xsstartindex)
                 # for j in range(startindex, stopindex):
                 sfmatrix[i, startindex:stopindex] += vec_xs_excitation_nnlevel_deltae[startindex:stopindex]
 
                 # do the last bit separately because we're not using the full deltaen interval
 
                 delta_en_actual = en + epsilon_trans_ev - engrid[stopindex]
                 sfmatrix[i, stopindex] += vec_xs_excitation_nnlevel_deltae[stopindex] * delta_en_actual / deltaen
@@ -669,19 +646,15 @@
     npts = len(engrid)
 
     ar_xs_array = at.nonthermal.get_arxs_array_shell(engrid, shell)
 
     if ionpot_ev <= engrid[0]:
         xsstartindex = 0
     else:
-        xsstartindex = npts + 1
-        for i in range(npts):
-            if ar_xs_array[i] > 0.0:
-                xsstartindex = i
-                break
+        xsstartindex = next((i for i in range(npts) if ar_xs_array[i] > 0.0), npts + 1)
         xsstartindex = get_energyindex_gteq(en_ev=ionpot_ev, engrid=engrid)
 
     # J * atan[(epsilon - ionpot_ev) / J] is the indefinite integral of
     # 1/(1 + (epsilon - ionpot_ev)^2/ J^2) d_epsilon
     # in Kozma & Fransson 1992 equation 4
 
     prefactors = [nnion * ar_xs_array[j] / atan((engrid[j] - ionpot_ev) / 2.0 / J) * deltaen for j in range(npts)]
@@ -1203,42 +1176,39 @@
         print(f"prob_e_s_can_ionise: {prob_e_s_can_ionise:.2f}")
         print(f"prob_e_s_cannot_ionise: {prob_e_s_cannot_ionise:.2f}")
     return eps_avg
 
 
 def calculate_Latom_excitation(ions, ionpopdict, nntot, en_ev, adata, T_exc=5000):
     L_atom_sum = 0.0
+    maxnlevelslower = 5
+    maxnlevelsupper = 250
+
+    k_b = 8.617333262145179e-05  # eV / K
     for Z, ionstage in ions:
         nnion = ionpopdict[(Z, ionstage)]
 
         ion = adata.query("Z == @Z and ion_stage == @ionstage").iloc[0]
-        dftransitions_ion = ion.transitions
-
-        maxnlevelslower = 5
-        maxnlevelsupper = 250
-
         # filterquery = 'collstr >= 0 or forbidden == False'
         filterquery = "collstr != -999"
         if maxnlevelslower is not None:
             filterquery += " and lower < @maxnlevelslower"
         if maxnlevelsupper is not None:
             filterquery += " and upper < @maxnlevelsupper"
 
+        dftransitions_ion = ion.transitions
         dftransitions_ion = dftransitions_ion.query(filterquery, inplace=False).copy()
 
-        k_b = 8.617333262145179e-05  # eV / K
         energy_boltzfac_sum = ion.levels.eval("energy_ev * g * exp(- energy_ev / @k_b / @T_exc)").sum()
 
         populations = ion.levels.eval("g * exp(- energy_ev / @k_b / @T_exc)").to_numpy() / energy_boltzfac_sum
 
         dftransitions_ion = dftransitions_ion.eval(
-            (
-                "epsilon_trans_ev = @ion.levels.loc[upper].energy_ev.to_numpy() -"
-                " @ion.levels.loc[lower].energy_ev.to_numpy()"
-            ),
+            "epsilon_trans_ev = @ion.levels.loc[upper].energy_ev.to_numpy() -"
+            " @ion.levels.loc[lower].energy_ev.to_numpy()",
         )
 
         dftransitions_ion = dftransitions_ion.eval("upper_g = @ion.levels.loc[upper].g.to_numpy()")
         dftransitions_ion = dftransitions_ion.eval("lower_g = @ion.levels.loc[lower].g.to_numpy()")
 
         for _, row in dftransitions_ion.iterrows():
             nnlevel = populations[row.lower] * nnion
@@ -1295,20 +1265,16 @@
     axes = [axes]
 
     ionpopdict = {
         # (16, 2): 3e5,
         (26, 2): 1e5,
     }
 
-    ions = []
-    for key in ionpopdict:
-        # keep only the ion populations, not element or total populations
-        if isinstance(key, tuple) and len(key) == 2:
-            ions.append(key)
-
+    # keep only the ion populations, not element or total populations
+    ions = [key for key in ionpopdict if isinstance(key, tuple) and len(key) == 2]
     ions.sort()
 
     nntot = get_nntot(ions=ions, ionpopdict=ionpopdict)
     nnetot = get_nnetot(ions=ions, ionpopdict=ionpopdict)  # total electrons: free and bound included
     nne = get_nne(ions=ions, ionpopdict=ionpopdict)
     nnebound = nnetot - nne
     # x_e = nne / nntot
@@ -1408,15 +1374,15 @@
         Aconst = 1.33e-14 * EV * EV
         binding = get_mean_binding_energy(Z, ionstage, electron_binding, ionpot_ev=ionpot_valence_ev)  # binding in erg
         oneoverW_limit_sim = Aconst * binding / Zbar / (2 * 3.14159 * pow(QE, 4))  # per erg
         workfn_limit_ev_sim = 1.0 / oneoverW_limit_sim / EV
         print(f"\n workfn_limit_ev_sim {workfn_limit_ev_sim:.2f} eV")
         print(f"   eta_ion  {ionpot_valence_ev / workfn_limit_ev_sim:.3f}")
         print(f"   eta_heat {1 - ionpot_valence_ev / workfn_limit_ev_sim:.3f}")
-        arr_workfn_limit_sim = np.array([workfn_limit_ev_sim for x in arr_en_ev])
+        arr_workfn_limit_sim = np.array([workfn_limit_ev_sim for _ in arr_en_ev])
 
         arr_xs_ar92 = at.nonthermal.get_arxs_array_ion(arr_en_ev, dfcollion_thision, Z, ionstage)
         Latom_ionisation_ar92 = arr_xs_ar92 * (ionpot_valence_ev * EV)
 
         arr_xs_lotz = np.array(
             [
                 get_lotz_xs_ionisation(Z, ionstage, electron_binding, ionpot_ev=ionpot_valence_ev, en_ev=en_ev)
@@ -1431,15 +1397,15 @@
         Latom_ionisation_lotz = arr_xs_lotz * (ionpot_valence_ev * EV)
 
         L_over_sigma = (Lelec_axelrod_nne[-1] + Latom_axelrod[-1]) / arr_xs_lotz[-1]
         workfn_limit_axelrod = L_over_sigma / EV
         print(f"\n workfn_limit_axelrod: {workfn_limit_axelrod:.2f} eV")
         print(f"   eta_ion  {ionpot_valence_ev / workfn_limit_axelrod:.3f}")
         print(f"   eta_heat {1 - ionpot_valence_ev / workfn_limit_axelrod:.3f}")
-        arr_workfn_limit_axelrod = np.array([workfn_limit_axelrod for x in arr_en_ev])
+        arr_workfn_limit_axelrod = np.array([workfn_limit_axelrod for _ in arr_en_ev])
 
         # Approximation to Axelrod 1980 Eq 3.20 (left Latom part) where the transition energy
         # of every ionisation is just the valence potential
         # Latom_ionisation = arr_xs * (ionpot_valence_ev * EV)
         # print(Latom[-1], Latom2[-1], Latom3[-1])
 
         # arr_xs_latom = Latom1 / (ionpot_valence_ev * EV)
```

### Comparing `artistools-2023.5.16.3/artistools/nonthermal/leptontransport.py` & `artistools-2023.8.1/artistools/nonthermal/leptontransport.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,16 +112,16 @@
         dE_on_dx_ionexc = calculate_dE_on_dx_ionexc(energy, n_e_bound)
         arr_dE_on_dx_ionexc.append(-dE_on_dx_ionexc / CONST_EV_IN_J)
         dE_on_dx_plasma = calculate_dE_on_dx_plasma(energy, n_e_free)
         arr_dE_on_dx_plasma.append(-dE_on_dx_plasma / CONST_EV_IN_J)
         dE_on_dx = dE_on_dx_ionexc
         if steps % 100000 == 0:
             print(
-                f"E: {energy / CONST_EV_IN_J:.1f} eV x: {x:.1e} dE_on_dx_ionexc: "
-                f"{dE_on_dx_ionexc}, dE_on_dx_plasma: {dE_on_dx_plasma}"
+                f"E: {energy / CONST_EV_IN_J:.1f} eV x: {x:.1e} dE_on_dx_ionexc: {dE_on_dx}, dE_on_dx_plasma:"
+                f" {dE_on_dx_plasma}"
             )
         x += delta_energy / dE_on_dx
         mean_free_path += -x * delta_energy / E_0
         energy += delta_energy
 
         steps += 1
         if energy <= 0:
```

### Comparing `artistools-2023.5.16.3/artistools/nonthermal/plotnonthermal.py` & `artistools-2023.8.1/artistools/nonthermal/plotnonthermal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python3
+from __future__ import annotations
+
 import argparse
-import os
 from functools import lru_cache
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pynonthermal
 from astropy import units as u
 
 import artistools as at
 
-DEFAULTSPECPATH = "../example_run/spec.out"
 defaultoutputfile = "plotnonthermal_cell{0:03d}_timestep{1:03d}.pdf"
 
 
 @lru_cache(maxsize=4)
-def read_files(modelpath, timestep=-1, modelgridindex=-1):
+def read_files(modelpath: Path, timestep: int = -1, modelgridindex: int = -1) -> pd.DataFrame:
     """Read ARTIS -thermal spectrum data into a pandas DataFrame."""
     nonthermaldata = pd.DataFrame()
 
     mpiranklist = at.get_mpiranklist(modelpath, modelgridindex=modelgridindex)
     for folderpath in at.get_runfolders(modelpath, timestep=timestep):
         for mpirank in mpiranklist:
             filepath = at.firstexisting(f"nonthermalspec_{mpirank:04d}.out", folder=folderpath, tryzipped=True)
@@ -44,15 +44,15 @@
                     return nonthermaldata_thisfile
 
                 nonthermaldata = nonthermaldata.append(nonthermaldata_thisfile.copy(), ignore_index=True)
 
     return nonthermaldata
 
 
-def make_xs_plot(axis, nonthermaldata, args):
+def make_xs_plot(axis: plt.Axes, nonthermaldata: pd.DataFrame, args: argparse.Namespace) -> None:
     dfcollion = at.nonthermal.read_colliondata()
 
     arr_en = nonthermaldata["energy_ev"].unique()
 
     # arr_xs_old = [xs_fe2_old(en) for en in arr_en]
     # arr_xs_times_y = [xs_fe1(en) * y for en, y in zip(nonthermaldata['energy_ev'], nonthermaldata['y'])]
 
@@ -61,25 +61,19 @@
 
     axis.set_ylabel(r"cross section (cm2)")
 
     if not args.nolegend:
         axis.legend(loc="upper center", handlelength=2, frameon=False, numpoints=1, prop={"size": 13})
 
 
-def inteuler(x, y):
-    dx = y[1:] - y[:-1]
-    return np.dot(x[:-1], dx)
-
-
 def plot_contributions(axis, modelpath, timestep, modelgridindex, nonthermaldata, args):
     estimators = at.estimators.read_estimators(
         modelpath, get_ion_values=True, get_heatingcooling=True, modelgridindex=modelgridindex, timestep=timestep
     )
 
-    # print(estimators[(timestep, modelgridindex)].keys())
     total_depev = estimators[(timestep, modelgridindex)]["total_dep"] * u.erg.to("eV")
 
     print(f"Deposition: {total_depev:.1f} [eV/cm3/s]")
 
     arr_enev = nonthermaldata["energy_ev"].to_numpy()
     arr_y = nonthermaldata["y"].to_numpy()
 
@@ -137,15 +131,15 @@
     print(f"frac_ionisation: {frac_ionisation}")
 
     axis.plot(arr_enev, arr_heating, label="Heating")
 
     axis.legend(loc="best", handlelength=2, frameon=False, numpoints=1, prop={"size": 11})
 
 
-def make_plot(modelpaths, args):
+def make_plot(modelpaths: list[Path], args: argparse.Namespace) -> None:
     nplots = 1
     if args.xsplot:
         nplots += 1
     if args.showcontributions:
         nplots += 1
     fig, axes = plt.subplots(
         nrows=nplots,
@@ -189,15 +183,15 @@
             continue
 
         if index < len(args.modellabels):
             model_label = args.modellabels[index]
         else:
             model_label = f"{modelname} cell {modelgridindex} at timestep {timestep}"
             try:
-                time_days = float(at.get_timestep_time(Path("."), timestep))
+                time_days = float(at.get_timestep_time(Path(), timestep))
             except FileNotFoundError:
                 time_days = 0
             else:
                 model_label += f" ({time_days:.2f}d)"
 
         outputfile = str(args.outputfile).format(modelgridindex, timestep)
         print(f"Plotting timestep {timestep:d}")
@@ -283,38 +277,38 @@
     )
 
     parser.add_argument(
         "-o", action="store", dest="outputfile", type=Path, default=defaultoutputfile, help="Filename for PDF file"
     )
 
 
-def main(args=None, argsraw=None, **kwargs):
+def main(args=None, argsraw=None, **kwargs) -> None:
     """Plot ARTIS non-thermal electron energy spectrum."""
     if args is None:
         parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
 
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     if not args.modelpath:
-        args.modelpath = [Path(".")]
-    elif isinstance(args.modelpath, (str, Path)):
+        args.modelpath = [Path()]
+    elif isinstance(args.modelpath, str | Path):
         args.modelpath = [args.modelpath]
 
     # flatten the list
     modelpaths = []
     for elem in args.modelpath:
         if isinstance(elem, list):
             modelpaths.extend(elem)
         else:
             modelpaths.append(elem)
 
-    if os.path.isdir(args.outputfile):
-        args.outputfile = os.path.join(args.outputfile, defaultoutputfile)
+    if Path(args.outputfile).is_dir():
+        args.outputfile = Path(args.outputfile, defaultoutputfile)
 
     if args.listtimesteps:
         at.showtimesteptimes()
     else:
         make_plot(modelpaths, args)
```

### Comparing `artistools-2023.5.16.3/artistools/nonthermal/solvespencerfanocmd.py` & `artistools-2023.8.1/artistools/nonthermal/solvespencerfanocmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python3
+from __future__ import annotations
+
 import argparse
 import sys
 from pathlib import Path
-from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pynonthermal as pynt
 
 import artistools as at
 
 minionfraction = 0.0  # minimum number fraction of the total population to include in SF solution
 
 defaultoutputfile = "spencerfano_cell{cell:03d}_ts{timestep:02d}_{timedays:.0f}d.pdf"
 
 
-def make_ntstats_plot(ntstatfile: Union[str, Path]) -> None:
+def make_ntstats_plot(ntstatfile: str | Path) -> None:
     fig, ax = plt.subplots(
         nrows=1, ncols=1, sharex=True, figsize=(4, 3), tight_layout={"pad": 0.5, "w_pad": 0.3, "h_pad": 0.3}
     )
 
     dfstats = pd.read_csv(ntstatfile, delim_whitespace=True, escapechar="#")
     dfstats = dfstats.fillna(0)
 
@@ -278,55 +279,55 @@
     # ionpopdict[(at.get_atomic_number('Fe'), 1)] = 0.012 * nntot
 
     stepcount = 9 if args.vary else 1
     for step in range(stepcount):
         emin = args.emin
         emax = args.emax
         npts = args.npts
-        if args.vary == "emin":
-            emin *= 2**step
-        elif args.vary == "emax":
+        if args.vary == "emax":
             emax *= 2**step
+        elif args.vary == "emax,npts":
+            npts *= 2**step
+            emax *= 2**step
+
+        elif args.vary == "emin":
+            emin *= 2**step
         elif args.vary == "npts":
             npts *= 2**step
         elif args.vary == "x_e":
             assert args.composition != "artis"
-        if args.vary == "emax,npts":
-            npts *= 2**step
-            emax *= 2**step
-
         if args.composition != "artis":
             compelement = args.composition
             compelement_atomicnumber = at.get_atomic_number(compelement)
             deposition_density_ev = 5.0e3
             nntot = 1.0
             x_e = (args.x_e * 10 ** (0.5 * step)) if args.vary == "x_e" else args.x_e
             ionpopdict = {}
             dfpops = {}
             T_e = 3000
             assert x_e <= 1.0
             ionpopdict[(compelement_atomicnumber, 1)] = nntot * (1.0 - x_e)
             ionpopdict[(compelement_atomicnumber, 2)] = nntot * x_e
 
-        ions = []
-        for key in ionpopdict:
-            # keep only the ion populations, not element or total populations
-            if isinstance(key, tuple) and len(key) == 2 and ionpopdict[key] / nntot >= minionfraction:
-                ions.append(key)
-
+        # keep only the ion populations, not element or total populations
+        ions = [
+            key
+            for key in ionpopdict
+            if isinstance(key, tuple) and len(key) == 2 and ionpopdict[key] / nntot >= minionfraction
+        ]
         ions.sort()
 
         if args.noexcitation:
             adata = None
             dfpops = None
         else:
             adata = at.atomic.get_levels(modelpath, get_transitions=True, ionlist=tuple(ions))
 
         if step == 0 and args.ostat:
-            with open(args.ostat, "w") as fstat:
+            with Path(args.ostat).open("w") as fstat:
                 strheader = "#emin emax npts x_e frac_sum frac_excitation frac_ionization frac_heating"
                 for atomic_number, ion_stage in ions:
                     strheader += " frac_ionization_" + at.get_ionstring(atomic_number, ion_stage, nospace=True)
                 fstat.write(strheader + "\n")
 
         with pynt.SpencerFanoSolver(emin_ev=emin, emax_ev=emax, npts=npts, verbose=True) as sf:
             for Z, ionstage in ions:
@@ -347,15 +348,15 @@
                 outputfilename = str(args.outputfile).format(
                     cell=args.modelgridindex, timestep=args.timestep, timedays=args.timedays
                 )
                 # outputfilename = "spencerfano.pdf"
                 sf.plot_spec_channels(outputfilename=outputfilename)
 
             if args.ostat:
-                with open(args.ostat, "a") as fstat:
+                with Path(args.ostat).open("a") as fstat:
                     strlineout = (
                         f"{emin} {emax} {npts} {x_e:7.2e} {sf.get_frac_sum():6.3f} "
                         f"{sf.get_frac_excitation_tot():6.3f} {sf.get_frac_ionisation_tot():6.3f} "
                         f" {sf.get_frac_heating():6.3f}"
                     )
                     for atomic_number, ionstage in ions:
                         nnion = ionpopdict[(atomic_number, ionstage)]
```

### Comparing `artistools-2023.5.16.3/artistools/packets/__init__.py` & `artistools-2023.8.1/artistools/packets/__init__.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/packets/packets.py` & `artistools-2023.8.1/artistools/packets/packets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+from __future__ import annotations
+
 import calendar
 import gzip
 import math
 import multiprocessing
-from collections.abc import Sequence
+import typing as t
 from functools import lru_cache
 from pathlib import Path
-from typing import Literal
-from typing import Optional
-from typing import Union
 
 import numpy as np
 import pandas as pd
 import polars as pl
+from typeguard import typechecked
 
 import artistools as at
 
 # for the parquet files
 time_parquetschemachange = (2023, 4, 22, 12, 31, 0)
 
 CLIGHT = 2.99792458e10
@@ -80,28 +80,25 @@
     "true_emission_velocity",
     "trueem_time",
     "pellet_nucindex",
 ]
 
 
 @lru_cache(maxsize=16)
-def get_column_names_artiscode(modelpath: Union[str, Path]) -> Optional[list[str]]:
+def get_column_names_artiscode(modelpath: str | Path) -> list[str] | None:
     modelpath = Path(modelpath)
     if Path(modelpath, "artis").is_dir():
         print("detected artis code directory")
-        packet_properties = []
+        packet_properties: list[str] = []
         inputfilename = at.firstexisting(["packet_init.cc", "packet_init.c"], folder=modelpath / "artis")
         print(f"found {inputfilename}: getting packet column names from artis code")
         with inputfilename.open() as inputfile:
             packet_print_lines = [line.split(",") for line in inputfile if "fprintf(packets_file," in line]
             for line in packet_print_lines:
-                for element in line:
-                    if "pkt[i]." in element:
-                        packet_properties.append(element)
-
+                packet_properties.extend(element for element in line if "pkt[i]." in element)
         for i, element in enumerate(packet_properties):
             packet_properties[i] = element.split(".")[1].split(")")[0]
 
         columns = packet_properties
         replacements_dict = {
             "type": "type_id",
             "pos[0]": "posx",
@@ -135,34 +132,36 @@
         return columns
 
     return None
 
 
 def add_derived_columns(
     dfpackets: pd.DataFrame,
-    modelpath: Path,
-    colnames: Sequence[str],
-    allnonemptymgilist: Optional[Sequence[int]] = None,
+    modelpathin: Path | str,
+    colnames: t.Sequence[str],
+    allnonemptymgilist: t.Sequence[int] | None = None,
 ) -> pd.DataFrame:
+    """Add columns to a packets DataFrame that are derived from the values that are stored in the packets files."""
+    modelpath = Path(modelpathin)
     cm_to_km = 1e-5
     day_in_s = 86400
-    if isinstance(dfpackets, pd.DataFrame) and dfpackets.empty:
+    if dfpackets.empty:
         return dfpackets
 
     colnames = at.makelist(colnames)
     dimensions = at.get_inputparams(modelpath)["n_dimensions"]
 
-    def em_modelgridindex(packet) -> Union[int, float]:
+    def em_modelgridindex(packet) -> int | float:
         assert dimensions == 1
 
         return at.inputmodel.get_mgi_of_velocity_kms(
             modelpath, packet.emission_velocity * cm_to_km, mgilist=allnonemptymgilist
         )
 
-    def emtrue_modelgridindex(packet) -> Union[int, float]:
+    def emtrue_modelgridindex(packet) -> int | float:
         assert dimensions == 1
 
         return at.inputmodel.get_mgi_of_velocity_kms(
             modelpath, packet.true_emission_velocity * cm_to_km, mgilist=allnonemptymgilist
         )
 
     def em_timestep(packet) -> int:
@@ -199,17 +198,20 @@
 
     if any(x in colnames for x in ["angle_bin", "dirbin", "costhetabin", "phibin"]):
         dfpackets = bin_packet_directions(modelpath, dfpackets)
 
     return dfpackets
 
 
-def add_derived_columns_lazy(dfpackets: pl.LazyFrame, modelmeta: Optional[dict] = None) -> pl.LazyFrame:
-    # we might as well add everything, since the columns only get calculated when they are actually used
+@typechecked
+def add_derived_columns_lazy(dfpackets: pl.LazyFrame, modelmeta: dict | None = None) -> pl.LazyFrame:
+    """Add columns to a packets DataFrame that are derived from the values that are stored in the packets files.
 
+    We might as well add everything, since the columns only get calculated when they are actually used (polars LazyFrame).
+    """
     dfpackets = dfpackets.with_columns(
         [
             (
                 (pl.col("em_posx") ** 2 + pl.col("em_posy") ** 2 + pl.col("em_posz") ** 2).sqrt() / pl.col("em_time")
             ).alias("emission_velocity")
         ]
     )
@@ -246,19 +248,19 @@
                 ).alias("em_modelgridindex")
             ]
         )
 
     return dfpackets
 
 
-def readfile_text(packetsfile: Union[Path, str], modelpath: Path = Path(".")) -> pl.DataFrame:
+def readfile_text(packetsfile: Path | str, modelpath: Path = Path()) -> pl.DataFrame:
     """Read a packets*.out(.xz) space-separated text file into a polars DataFrame."""
     print(f"Reading {packetsfile}")
     skiprows: int = 0
-    column_names: Optional[list[str]] = None
+    column_names: list[str] | None = None
     try:
         fpackets = at.zopen(packetsfile, mode="rb")
 
         datastartpos = fpackets.tell()  # will be updated if this was actually the start of a header
         firstline = fpackets.readline().decode()
 
         if firstline.lstrip().startswith("#"):
@@ -310,32 +312,30 @@
         # some packets don't have this set, which confused read_csv to mark it as str
         dfpackets = dfpackets.with_columns([pl.col("true_emission_velocity").cast(pl.Float32)])
 
     if "originated_from_positron" in dfpackets.columns:
         dfpackets = dfpackets.with_columns([pl.col("originated_from_positron").cast(pl.Boolean)])
 
     # Luke: packet energies in ergs can be huge (>1e39) which is too large for Float32
-    dfpackets = dfpackets.with_columns(
+    return dfpackets.with_columns(
         [pl.col(pl.Int64).cast(pl.Int32), pl.col(pl.Float64).exclude(["e_rf", "e_cmf"]).cast(pl.Float32)]
     )
 
-    return dfpackets
-
 
 def readfile(
-    packetsfile: Union[Path, str],
-    packet_type: Optional[str] = None,
-    escape_type: Optional[Literal["TYPE_RPKT", "TYPE_GAMMA"]] = None,
+    packetsfile: Path | str,
+    packet_type: str | None = None,
+    escape_type: t.Literal["TYPE_RPKT", "TYPE_GAMMA"] | None = None,
 ) -> pd.DataFrame:
     """Read a packet file into a Pandas DataFrame."""
     return readfile_pl(packetsfile, packet_type=packet_type, escape_type=escape_type).collect().to_pandas()
 
 
 def convert_text_to_parquet(
-    packetsfiletext: Union[Path, str],
+    packetsfiletext: Path | str,
 ) -> Path:
     packetsfiletext = Path(packetsfiletext)
     packetsfileparquet = at.stripallsuffixes(packetsfiletext).with_suffix(".out.parquet")
 
     dfpackets = readfile_text(packetsfiletext).lazy()
     dfpackets = dfpackets.with_columns(
         [
@@ -352,35 +352,33 @@
                 / 86400.0
             )
             .cast(pl.Float32)
             .alias("t_arrive_d"),
         ]
     )
 
-    syn_dir = (0.0, 0.0, 1.0)
-    for p in packetsfiletext.parents:
-        if Path(p, "syn_dir.txt").is_file():
-            syn_dir = at.get_syn_dir(p)
-            break
-
+    syn_dir = next(
+        (at.get_syn_dir(p) for p in packetsfiletext.parents if Path(p, "syn_dir.txt").is_file()),
+        (0.0, 0.0, 1.0),
+    )
     dfpackets = add_packet_directions_lazypolars(dfpackets, syn_dir)
     dfpackets = bin_packet_directions_lazypolars(dfpackets)
 
     # print(f"Saving {packetsfileparquet}")
     dfpackets = dfpackets.sort(by=["type_id", "escape_type_id", "t_arrive_d"])
     dfpackets.collect().write_parquet(packetsfileparquet, compression="zstd", statistics=True)
 
     return packetsfileparquet
 
 
 def readfile_pl(
-    packetsfile: Union[Path, str],
-    modelpath: Union[None, Path, str] = None,
-    packet_type: Optional[str] = None,
-    escape_type: Optional[Literal["TYPE_RPKT", "TYPE_GAMMA"]] = None,
+    packetsfile: Path | str,
+    modelpath: None | Path | str = None,
+    packet_type: str | None = None,
+    escape_type: t.Literal["TYPE_RPKT", "TYPE_GAMMA"] | None = None,
 ) -> pl.LazyFrame:
     """Read a packets file into a Polars LazyFrame from either a parquet file or a text file (and save .parquet)."""
     dfpackets = pl.scan_parquet(packetsfile)
 
     if escape_type is not None:
         assert packet_type is None or packet_type == "TYPE_ESCAPE"
         dfpackets = dfpackets.filter(
@@ -389,15 +387,15 @@
     elif packet_type is not None and packet_type:
         dfpackets = dfpackets.filter(pl.col("type_id") == type_ids[packet_type])
 
     return dfpackets
 
 
 def get_packetsfilepaths(
-    modelpath: Union[str, Path], maxpacketfiles: Optional[int] = None, printwarningsonly: bool = False
+    modelpath: str | Path, maxpacketfiles: int | None = None, printwarningsonly: bool = False
 ) -> list[Path]:
     nprocs = at.get_nprocs(modelpath)
 
     searchfolders = [Path(modelpath, "packets"), Path(modelpath)]
     # in descending priority (based on speed of reading)
     suffix_priority = [".out.zst", ".out.lz4", ".out.zst", ".out", ".out.gz", ".out.xz"]
     t_lastschemachange = calendar.timegm(time_parquetschemachange)
@@ -457,18 +455,18 @@
         else:
             print(f"Reading from {len(parquetpacketsfiles)} packets files")
 
     return parquetpacketsfiles
 
 
 def get_packets_pl(
-    modelpath: Union[str, Path],
-    maxpacketfiles: Optional[int] = None,
-    packet_type: Optional[str] = None,
-    escape_type: Optional[Literal["TYPE_RPKT", "TYPE_GAMMA"]] = None,
+    modelpath: str | Path,
+    maxpacketfiles: int | None = None,
+    packet_type: str | None = None,
+    escape_type: t.Literal["TYPE_RPKT", "TYPE_GAMMA"] | None = None,
 ) -> tuple[int, pl.LazyFrame]:
     if escape_type is not None:
         assert packet_type in [None, "TYPE_ESCAPE"]
         if packet_type is None:
             packet_type = "TYPE_ESCAPE"
 
     packetsfiles = get_packetsfilepaths(modelpath, maxpacketfiles)
@@ -578,24 +576,23 @@
                 .then(pl.col("cosphi").arccos())
                 .otherwise(pl.col("cosphi").mul(-1.0).arccos() + np.pi)
             )
             .cast(pl.Float32)
             .alias("phi"),
         )
 
-    dfpackets = dfpackets.drop(["dirmag", "vec1_x", "vec1_y", "vec1_z"])
-
-    return dfpackets
+    return dfpackets.drop(["dirmag", "vec1_x", "vec1_y", "vec1_z"])
 
 
+@typechecked
 def bin_packet_directions_lazypolars(
     dfpackets: pl.LazyFrame,
-    nphibins: Optional[int] = None,
-    ncosthetabins: Optional[int] = None,
-    phibintype: Literal["artis_pi_reversal", "monotonic"] = "artis_pi_reversal",
+    nphibins: int | None = None,
+    ncosthetabins: int | None = None,
+    phibintype: t.Literal["artis_pi_reversal", "monotonic"] = "artis_pi_reversal",
 ) -> pl.LazyFrame:
     if nphibins is None:
         nphibins = at.get_viewingdirection_phibincount()
 
     if ncosthetabins is None:
         ncosthetabins = at.get_viewingdirection_costhetabincount()
 
@@ -617,22 +614,21 @@
                 .otherwise((pl.col("cosphi").arccos() + np.pi) / 2.0 / np.pi * nphibins)
             )
             .fill_nan(0.0)
             .cast(pl.Int32)
             .alias("phibin"),
         )
 
-    dfpackets = dfpackets.with_columns(
+    return dfpackets.with_columns(
         (pl.col("costhetabin") * nphibins + pl.col("phibin")).cast(pl.Int32).alias("dirbin"),
     )
 
-    return dfpackets
-
 
-def bin_packet_directions(modelpath: Union[Path, str], dfpackets: pd.DataFrame) -> pd.DataFrame:
+@typechecked
+def bin_packet_directions(modelpath: Path | str, dfpackets: pd.DataFrame) -> pd.DataFrame:
     nphibins = at.get_viewingdirection_phibincount()
     ncosthetabins = at.get_viewingdirection_costhetabincount()
 
     syn_dir = at.get_syn_dir(Path(modelpath))
     xhat = np.array([1.0, 0.0, 0.0])
     vec2 = np.cross(xhat, syn_dir)
 
@@ -667,38 +663,38 @@
 
 
 def make_3d_histogram_from_packets(modelpath, timestep_min, timestep_max=None, em_time=True):
     if timestep_max is None:
         timestep_max = timestep_min
     modeldata, _, vmax_cms = at.inputmodel.get_modeldata_tuple(modelpath)
 
-    timeminarray = at.get_timestep_times_float(modelpath=modelpath, loc="start")
-    # timedeltaarray = at.get_timestep_times_float(modelpath=modelpath, loc="delta")
-    timemaxarray = at.get_timestep_times_float(modelpath=modelpath, loc="end")
+    timeminarray = at.get_timestep_times(modelpath=modelpath, loc="start")
+    # timedeltaarray = at.get_timestep_times(modelpath=modelpath, loc="delta")
+    timemaxarray = at.get_timestep_times(modelpath=modelpath, loc="end")
 
     # timestep = 63 # 82 73 #63 #54 46 #27
     # print([(ts, time) for ts, time in enumerate(timeminarray)])
     if em_time:
         print("Binning by packet emission time")
     else:
         print("Binning by packet arrival time")
 
     packetsfiles = at.packets.get_packetsfilepaths(modelpath)
 
     emission_position3d = [[], [], []]
     e_rf = []
     e_cmf = []
 
+    only_packets_0_scatters = False
     for packetsfile in packetsfiles:
         # for npacketfile in range(0, 1):
         dfpackets = at.packets.readfile(packetsfile)
         at.packets.add_derived_columns(dfpackets, modelpath, ["emission_velocity"])
         dfpackets = dfpackets.dropna(subset=["emission_velocity"])  # drop rows where emission_vel is NaN
 
-        only_packets_0_scatters = False
         if only_packets_0_scatters:
             print("Only using packets with 0 scatters")
             # print(dfpackets[['scat_count', 'interactions', 'nscatterings']])
             dfpackets = dfpackets.query("nscatterings == 0")
 
         # print(dfpackets[['emission_velocity', 'em_velx', 'em_vely', 'em_velz']])
         # select only type escape and type r-pkt (don't include gamma-rays)
@@ -754,17 +750,17 @@
 
 def make_3d_grid(modeldata, vmax_cms):
     # modeldata, _, vmax_cms = at.inputmodel.get_modeldata_tuple(modelpath)
     grid = round(len(modeldata["inputcellid"]) ** (1.0 / 3.0))
     xgrid = np.zeros(grid)
     vmax = vmax_cms / CLIGHT
     i = 0
-    for _z in range(0, grid):
-        for _y in range(0, grid):
-            for x in range(0, grid):
+    for _z in range(grid):
+        for _y in range(grid):
+            for x in range(grid):
                 xgrid[x] = -vmax + 2 * x * vmax / grid
                 i += 1
 
     x, y, z = np.meshgrid(xgrid, xgrid, xgrid)
     grid_3d = np.array([xgrid, xgrid, xgrid])
     # grid_Te = np.zeros((grid, grid, grid))
     # print(grid_Te.shape)
@@ -774,19 +770,19 @@
 def get_mean_packet_emission_velocity_per_ts(
     modelpath, packet_type="TYPE_ESCAPE", escape_type="TYPE_RPKT", maxpacketfiles=None, escape_angles=None
 ) -> pd.DataFrame:
     packetsfiles = at.packets.get_packetsfilepaths(modelpath, maxpacketfiles=maxpacketfiles)
     nprocs_read = len(packetsfiles)
     assert nprocs_read > 0
 
-    timearray = at.get_timestep_times_float(modelpath=modelpath, loc="mid")
-    arr_timedelta = at.get_timestep_times_float(modelpath=modelpath, loc="delta")
+    timearray = at.get_timestep_times(modelpath=modelpath, loc="mid")
+    arr_timedelta = at.get_timestep_times(modelpath=modelpath, loc="delta")
     timearrayplusend = np.concatenate([timearray, [timearray[-1] + arr_timedelta[-1]]])
 
-    dfpackets_escape_velocity_and_arrive_time = pd.DataFrame
+    dfpackets_escape_velocity_and_arrive_time = pd.DataFrame()
     emission_data = pd.DataFrame(
         {"t_arrive_d": timearray, "mean_emission_velocity": np.zeros_like(timearray, dtype=float)}
     )
 
     for i, packetsfile in enumerate(packetsfiles):
         dfpackets = at.packets.readfile(packetsfile, packet_type=packet_type, escape_type=escape_type)
         at.packets.add_derived_columns(dfpackets, modelpath, ["emission_velocity"])
@@ -814,52 +810,50 @@
     ):
         emission_data["mean_emission_velocity"][binindex] += emission_velocity  # / 2.99792458e10
 
     return emission_data
 
 
 def bin_and_sum(
-    df: Union[pl.DataFrame, pl.LazyFrame],
+    df: pl.DataFrame | pl.LazyFrame,
     bincol: str,
-    bins: list[Union[float, int]],
-    sumcols: Optional[list[str]] = None,
+    bins: list[float | int],
+    sumcols: list[str] | None = None,
     getcounts: bool = False,
 ) -> pl.DataFrame:
     """Bins is a list of lower edges, and the final upper edge."""
     # Polars method
 
-    binindex = (
-        df.select(bincol)
-        .lazy()
-        .collect()
-        .get_column(bincol)
-        .cut(bins=list(bins), category_label=bincol + "_bin", maintain_order=True)
-        .get_column(bincol + "_bin")
-        .cast(pl.Int32)
-        - 1  # subtract 1 because the returned index 0 is the bin below the start of the first supplied bin
+    df = df.with_columns(
+        (
+            pl.col(bincol)
+            .cut(breaks=list(bins), labels=[str(x) for x in range(-1, len(bins))])
+            .cast(str)
+            .cast(pl.Int32)
+        ).alias(f"{bincol}_bin")
     )
-    df = df.with_columns([binindex])
 
-    if sumcols is not None:
-        aggs = [pl.col(col).sum().alias(col + "_sum") for col in sumcols]
+    aggs = [pl.col(col).sum().alias(col + "_sum") for col in sumcols] if sumcols is not None else []
 
     if getcounts:
         aggs.append(pl.col(bincol).count().alias("count"))
 
-    wlbins = df.groupby(bincol + "_bin").agg(aggs).lazy().collect()
+    wlbins = df.groupby(f"{bincol}_bin").agg(aggs).lazy().collect()
 
     # now we will include the empty bins
-    dfout = pl.DataFrame(pl.Series(name=bincol + "_bin", values=np.arange(0, len(bins) - 1), dtype=pl.Int32))
-    dfout = dfout.join(wlbins, how="left", on=bincol + "_bin").fill_null(0)
+    dfout = pl.DataFrame(pl.Series(name=f"{bincol}_bin", values=np.arange(0, len(bins) - 1), dtype=pl.Int32))
+    return dfout.join(wlbins, how="left", on=f"{bincol}_bin").fill_null(0)
 
     # pandas method
 
-    # dfout2 = pd.DataFrame({bincol + "_bin": np.arange(0, len(bins) - 1)})
+    # dfout2 = pd.DataFrame({f"{bincol}_bin": np.arange(0, len(bins) - 1)})
     # if isinstance(df, pl.DataFrame):
     #     df2 = df.to_pandas(use_pyarrow_extension_array=True)
+    # elif isinstance(df, pl.LazyFrame):
+    #     df2 = df.collect().to_pandas(use_pyarrow_extension_array=True)
 
     # pdbins = pd.cut(
     #     x=df2[bincol],
     #     bins=bins,
     #     right=True,
     #     labels=range(len(bins) - 1),
     #     include_lowest=True,
@@ -871,8 +865,9 @@
     #         #     [pl.Series(col + "_sum", df[col].groupby(pdbins).sum().values) for col in sumcols]
     #         # )
     #         dfout2[col + "_sum"] = df2[col].groupby(pdbins).sum().values
     # if getcounts:
     #     # dfout = dfout.with_columns([pl.Series("count", df[bincol].groupby(pdbins).count().values)])
     #     dfout2["count"] = df2[bincol].groupby(pdbins).count().values
 
-    return dfout
+    # print(dfout2)
+    # return dfout2
```

### Comparing `artistools-2023.5.16.3/artistools/packets/packetsplots.py` & `artistools-2023.8.1/artistools/packets/packetsplots.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     # for z in range(0, grid):
     #     for y in range(0, grid):
     #         for x in range(0, grid):
     #             if modeldata["rho"][i] == 0.0:
     #                 hist[x, y, z] = None
     #             i += 1
 
-    timeminarray = at.get_timestep_times_float(modelpath=modelpath, loc="start")
-    timemaxarray = at.get_timestep_times_float(modelpath=modelpath, loc="end")
+    timeminarray = at.get_timestep_times(modelpath=modelpath, loc="start")
+    timemaxarray = at.get_timestep_times(modelpath=modelpath, loc="end")
     time_lower = timeminarray[timestep_min]
     time_upper = timemaxarray[timestep_max]
     title = f"{time_lower:.2f} - {time_upper:.2f} days"
     print(f"plotting packets between {title}")
     escapetitle = "pktemissiontime" if em_time else "pktarrivetime"
     title = title + "\n" + escapetitle
 
@@ -96,15 +96,15 @@
         use_2d=True,
         font_size=26,
         bold=False,
     )
     # labels = dict(xlabel='vx / c', ylabel='vy / c', zlabel='vz / c')
     # p.show_grid(**labels)
     p.camera_position = "zx"
-    timeminarray = at.get_timestep_times_float(modelpath=modelpath, loc="start")
+    timeminarray = at.get_timestep_times(modelpath=modelpath, loc="start")
     time = timeminarray[timestep]
     p.add_title(f"{time:.2f} - {timeminarray[timestep + 1]:.2f} days")
     print(pv.global_theme)
 
     p.show(screenshot=modelpath / f"3Dplot_pktsemitted{time:.1f}days_disk.png")
```

### Comparing `artistools-2023.5.16.3/artistools/plotspherical.py` & `artistools-2023.8.1/artistools/plotspherical.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
+# mypy: warn-unused-configs, disallow-any-generics, disallow-subclassing-any, disallow-untyped-calls,
+# mypy: disallow-untyped-defs, disallow-incomplete-defs, check-untyped-defs, disallow-untyped-decorators,
+# mypy: warn-redundant-casts, warn-unused-ignores, warn-return-any, no-implicit-reexport, strict-equality, strict-concatenate
+from __future__ import annotations
+
 import argparse
+import typing as t
 from pathlib import Path
-from typing import Optional
-from typing import Union
 
 import argcomplete
 import matplotlib.pyplot as plt
 import numpy as np
 import polars as pl
+from typeguard import typechecked
 
 import artistools as at
 
 
+@typechecked
 def plot_spherical(
-    modelpath: Union[str, Path],
-    timemindays: Optional[float],
-    timemaxdays: Optional[float],
+    modelpath: str | Path,
+    timemindays: float | None,
+    timemaxdays: float | None,
     nphibins: int,
     ncosthetabins: int,
-    outputfile: Union[Path, str],
-    maxpacketfiles: Optional[int] = None,
-    atomic_number: Optional[int] = None,
-    ion_stage: Optional[int] = None,
-    interpolate: bool = False,
-    gaussian_sigma: Optional[int] = None,
-    plotvars: Optional[list[str]] = None,
-    cmap: Optional[str] = None,
-) -> None:
+    maxpacketfiles: int | None = None,
+    atomic_number: int | None = None,
+    ion_stage: int | None = None,
+    gaussian_sigma: int | None = None,
+    plotvars: list[str] | None = None,
+    figscale: float = 1.0,
+    cmap: str | None = None,
+) -> tuple[plt.Figure, np.ndarray[t.Any, np.dtype[plt.Axes]]]:
     if plotvars is None:
         plotvars = ["luminosity", "emvelocityoverc", "emlosvelocityoverc"]
 
     _, modelmeta = at.get_modeldata(modelpath=modelpath, getheadersonly=True, printwarningsonly=True)
 
-    dfpackets: Union[pl.LazyFrame, pl.DataFrame]
     nprocs_read, dfpackets = at.packets.get_packets_pl(
         modelpath, maxpacketfiles, packet_type="TYPE_ESCAPE", escape_type="TYPE_RPKT"
     )
 
     _, tmin_d_valid, tmax_d_valid = at.get_escaped_arrivalrange(modelpath)
     if tmin_d_valid is None or tmax_d_valid is None:
         print("WARNING! The observer never gets light from the entire ejecta. Plotting all packets anyway")
@@ -65,39 +69,28 @@
                 f" ({tmax_d_valid:.2f} d)"
             )
         dfpackets = dfpackets.filter((pl.col("t_arrive_d") >= timemindays) & (pl.col("t_arrive_d") <= timemaxdays))
 
     assert timemindays is not None
     assert timemaxdays is not None
 
-    fig, axes = plt.subplots(
-        len(plotvars),
-        1,
-        figsize=(4, 3 * len(plotvars)),
-        subplot_kw={"projection": "mollweide"},
-        tight_layout={"pad": 0.1, "w_pad": 1.5, "h_pad": 0.0},
-    )
-
-    if len(plotvars) == 1:
-        axes = [axes]
-
     # phi definition (with syn_dir=[0 0 1])
     # x=math.cos(-phi)
     # y=math.sin(-phi)
 
     dfpackets = at.packets.bin_packet_directions_lazypolars(
         dfpackets=dfpackets, nphibins=nphibins, ncosthetabins=ncosthetabins, phibintype="monotonic"
     )
 
     # for figuring out where the axes are on the plot, make a cut
-    # dfpackets = dfpackets.filter(pl.col("dirz") < -0.9)
+    # dfpackets = dfpackets.filter(pl.col("dirz") > 0.9)
 
-    solidanglefactor = nphibins * ncosthetabins
     aggs = []
     dfpackets = at.packets.add_derived_columns_lazy(dfpackets, modelmeta=modelmeta)
+
     if "emvelocityoverc" in plotvars:
         aggs.append(
             ((pl.col("emission_velocity") * pl.col("e_rf")).mean() / pl.col("e_rf").mean() / 29979245800).alias(
                 "emvelocityoverc"
             )
         )
 
@@ -105,46 +98,45 @@
         aggs.append(
             (
                 (pl.col("emission_velocity_lineofsight") * pl.col("e_rf")).mean() / pl.col("e_rf").mean() / 29979245800
             ).alias("emlosvelocityoverc")
         )
 
     if "luminosity" in plotvars:
+        solidanglefactor = nphibins * ncosthetabins
         aggs.append(
             (pl.col("e_rf").sum() / nprocs_read * solidanglefactor / (timemaxdays - timemindays) / 86400).alias(
                 "luminosity"
             )
         )
 
     if "temperature" in plotvars:
         timebins = [
-            *at.get_timestep_times_float(modelpath, loc="start") * 86400.0,
-            at.get_timestep_times_float(modelpath, loc="end")[-1] * 86400.0,
+            *at.get_timestep_times(modelpath, loc="start") * 86400.0,
+            at.get_timestep_times(modelpath, loc="end")[-1] * 86400.0,
         ]
-
-        binindex = (
-            dfpackets.select("em_time")
-            .lazy()
-            .collect()
-            .get_column("em_time")
-            .cut(bins=list(timebins), category_label="em_timestep", maintain_order=True)
-            .get_column("em_timestep")
-            .cast(pl.Int32)
-            - 1  # subtract 1 because the returned index 0 is the bin below the start of the first supplied bin
+        dfpackets = dfpackets.with_columns(
+            (
+                pl.col("em_time")
+                .cut(breaks=list(timebins), labels=[str(x) for x in range(-1, len(timebins))])
+                .cast(str)
+                .cast(pl.Int32)
+            ).alias("em_timestep")
         )
-        dfpackets = dfpackets.with_columns([binindex])
+
         dfest_parquetfile = Path(modelpath, "temperatures.parquet.tmp")
 
         if not dfest_parquetfile.is_file():
             estimators = at.estimators.read_estimators(
                 modelpath,
                 get_ion_values=False,
                 get_heatingcooling=False,
                 skip_emptycells=True,
             )
+            assert len(estimators) > 0
             pl.DataFrame(
                 {
                     "timestep": (tsmgi[0] for tsmgi in estimators),
                     "modelgridindex": (tsmgi[1] for tsmgi in estimators),
                     "TR": (estimators[tsmgi].get("TR", -1) for tsmgi in estimators),
                 },
             ).filter(pl.col("TR") >= 0).with_columns(pl.col(pl.Int64).cast(pl.Int32)).write_parquet(
@@ -187,83 +179,83 @@
         .fill_null(0)
         .sort(["costhetabin", "phibin"])
     )
 
     print(f'total packets contributed: {alldirbins.select("count").sum().to_numpy()[0][0]:.1e}')
 
     # these phi and theta angle ranges are defined differently to artis
-    phigrid = np.linspace(-np.pi, np.pi, nphibins + 1, endpoint=True)
+    phigrid = np.linspace(-np.pi, np.pi, nphibins + 1, endpoint=True, dtype=np.float64)
 
     # costhetabin zero is (0,0,-1) so theta angle
-    costhetagrid = np.linspace(-1, 1, ncosthetabins + 1, endpoint=True)
+    costhetagrid = np.linspace(-1, 1, ncosthetabins + 1, endpoint=True, dtype=np.float64)
     # for Molleweide projection, theta range is [-pi/2, +pi/2]
-    thetagrid = np.arccos(costhetagrid) - np.pi / 2
+    thetagrid = np.pi / 2 - np.arccos(costhetagrid)
 
     meshgrid_phi, meshgrid_theta = np.meshgrid(phigrid, thetagrid)
 
+    fig, axes = plt.subplots(
+        len(plotvars),
+        1,
+        figsize=(figscale * at.get_config()["figwidth"], 3.7 * len(plotvars)),
+        subplot_kw={"projection": "mollweide"},
+        tight_layout={"pad": 0.1, "w_pad": 0.0, "h_pad": 0.0},
+    )
+
+    if len(plotvars) == 1:
+        axes = np.array([axes])
+
     for ax, plotvar in zip(axes, plotvars):
         data = alldirbins.get_column(plotvar).to_numpy().reshape((ncosthetabins, nphibins))
 
         if gaussian_sigma is not None and gaussian_sigma > 0:
             import scipy.ndimage
 
             sigma_bins = gaussian_sigma / 360 * nphibins
             data = scipy.ndimage.gaussian_filter(data, sigma=sigma_bins, mode="wrap")
 
-        if not interpolate:
-            colormesh = ax.pcolormesh(meshgrid_phi, meshgrid_theta, data, rasterized=True, cmap=cmap)
-        else:
-            ngridhighres = 1024
-            print(f"interpolating onto {ngridhighres}^2 grid")
-
-            from scipy.interpolate import CloughTocher2DInterpolator
-
-            meshgrid_phi_input, meshgrid_theta_input = np.meshgrid(
-                np.linspace(-np.pi, np.pi, nphibins, endpoint=True),
-                np.arccos(np.linspace(-1, 1, ncosthetabins, endpoint=True)) - np.pi / 2,
-            )
-            finterp = CloughTocher2DInterpolator(
-                list(zip(meshgrid_phi_input.flatten(), meshgrid_theta_input.flatten())), data.flatten()
-            )
-
-            meshgrid_phi_highres, meshgrid_theta_highres = np.meshgrid(
-                np.linspace(-np.pi, np.pi, ngridhighres + 1, endpoint=True),
-                np.linspace(-np.pi / 2.0, np.pi / 2.0, ngridhighres + 1, endpoint=True),
-            )
-            data_interp = finterp(meshgrid_phi_highres, meshgrid_theta_highres)
-
-            colormesh = ax.pcolormesh(
-                meshgrid_phi_highres, meshgrid_theta_highres, data_interp, rasterized=True, cmap=cmap
-            )
+        colormesh = ax.pcolormesh(meshgrid_phi, meshgrid_theta, data, rasterized=True, cmap=cmap)
 
-        if plotvar == "emvelocityoverc":
-            colorbartitle = r"Last interaction ejecta velocity [c]"
-        elif plotvar == "emlosvelocityoverc":
+        if plotvar == "emlosvelocityoverc":
             colorbartitle = r"Mean line of sight velocity [c]"
+        elif plotvar == "emvelocityoverc":
+            colorbartitle = r"Last interaction ejecta velocity [c]"
         elif plotvar == "luminosity":
-            colorbartitle = r"$I_{e,\Omega}\cdot4\pi/\Omega$ [erg/s]"
+            colorbartitle = r"Radiant intensity $\cdot\,4π$ [{}erg/s]"
         elif plotvar == "temperature":
-            colorbartitle = r"Temperature [K]"
+            colorbartitle = r"Temperature [{}K]"
         else:
             raise AssertionError
 
-        cbar = fig.colorbar(colormesh, location="bottom")
-        cbar.ax.set_title(colorbartitle)
+        cbar = fig.colorbar(colormesh, ax=ax, location="bottom")
         cbar.outline.set_linewidth(0)
+        cbar.ax.tick_params(axis="both", direction="out")
+        cbar.ax.xaxis.set_ticks_position("top")
+        # cbar.ax.set_title(colorbartitle)
+        cbar.ax.set_xlabel(colorbartitle)
+        cbar.ax.xaxis.set_label_position("top")
+        if r"{}" in colorbartitle:
+            cbar.ax.xaxis.set_major_formatter(at.plottools.ExponentLabelFormatter(colorbartitle, useMathText=True))
 
         # ax.set_xlabel("Azimuthal angle")
         # ax.set_ylabel("Polar angle")
-        # ax.tick_params(colors="white", axis="x", which="both")
-        ax.set_xticklabels([])
-        ax.set_yticklabels([])
-        # ax.grid(True)
+        # ax.set_xlabel(r"$\phi$")
+        # ax.set_ylabel(r"$\theta$")
+        # ax.set_xticklabels([])
+        # ax.set_yticklabels([])
+        # ax.grid(visible=True, color="black")
         ax.axis("off")
+        # xticks_deg = np.arange(0, 360, 90)[1:]
+        # ax.set_xticks(ticks=xticks_deg / 180 * np.pi - np.pi, labels=[rf"${deg:.0f}\degree$" for deg in xticks_deg])
 
-    fig.savefig(outputfile)
-    print(f"Saved {outputfile}")
+        # yticks_deg = np.linspace(0, 180, 7)
+        # ax.set_yticks(
+        #     ticks=-yticks_deg / 180 * np.pi + np.pi / 2.0, labels=[rf"${deg:.0f}\degree$" for deg in yticks_deg]
+        # )
+
+    return fig, axes
 
 
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument(
         "-modelpath",
         type=Path,
         default=Path(),
@@ -287,27 +279,29 @@
         "-atomic_number", type=int, default=None, help="Filter emitted packets by element of last emission"
     )
     parser.add_argument(
         "-ion_stage", type=int, default=None, help="Filter emitted packets by ionistion stage of last emission"
     )
     parser.add_argument("-cmap", default=None, type=str, help="Matplotlib color map name")
 
-    parser.add_argument("--interpolate", action="store_true", help="Interpolate grid to higher resolution")
+    parser.add_argument(
+        "-figscale", type=float, default=1.0, help="Scale factor for plot area. 1.0 is for single-column"
+    )
 
     parser.add_argument(
         "-o",
         action="store",
         dest="outputfile",
         type=Path,
         default=Path("plotspherical.pdf"),
         help="Filename for PDF file",
     )
 
 
-def main(args=None, argsraw=None, **kwargs) -> None:
+def main(args: argparse.Namespace | None = None, argsraw: list[str] | None = None, **kwargs: t.Any) -> None:
     """Plot direction maps based on escaped packets."""
     if args is None:
         parser = argparse.ArgumentParser(formatter_class=at.CustomArgHelpFormatter, description=__doc__)
         addargs(parser)
         parser.set_defaults(**kwargs)
         argcomplete.autocomplete(parser)
         args = parser.parse_args(argsraw)
@@ -315,26 +309,28 @@
     if not args.modelpath:
         args.modelpath = ["."]
 
     if args.elem is not None:
         assert args.atomic_number is None
         args.atomic_number = at.get_atomic_number(args.elem)
 
-    plot_spherical(
+    fig, axes = plot_spherical(
         modelpath=args.modelpath,
         timemindays=args.timemin,
         timemaxdays=args.timemax,
         nphibins=args.nphibins,
         ncosthetabins=args.ncosthetabins,
         maxpacketfiles=args.maxpacketfiles,
-        outputfile=args.outputfile,
-        interpolate=args.interpolate,
         gaussian_sigma=args.gaussian_sigma,
         atomic_number=args.atomic_number,
         ion_stage=args.ion_stage,
         plotvars=args.plotvars,
         cmap=args.cmap,
+        figscale=args.figscale,
     )
 
+    fig.savefig(args.outputfile)
+    print(f"Saved {args.outputfile}")
+
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `artistools-2023.5.16.3/artistools/plottools.py` & `artistools-2023.8.1/artistools/plottools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Matplotlib-related plotting functions."""
 import sys
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import ticker
 
 from .configuration import get_config
@@ -18,44 +19,59 @@
         self.set_labeltemplate(labeltemplate)
         self.decimalplaces = decimalplaces
         super().__init__(useOffset=True, useMathText=useMathText)
         # ticker.ScalarFormatter.__init__(self, useOffset=useOffset, useMathText=useMathText)
 
     def _set_formatted_label_text(self):
         # or use self.orderOfMagnitude
-        stroffset = self.get_offset().replace(r"$\times", "$") + " "
+        stroffset = self.get_offset()
+        if stroffset:
+            stroffset = stroffset.replace(r"$\times", "$") + " "
         strnewlabel = self.labeltemplate.format(stroffset)
         self.axis.set_label_text(strnewlabel)
         assert self.offset == 0
         self.axis.offsetText.set_visible(False)
 
     def set_labeltemplate(self, labeltemplate):
         assert "{" in labeltemplate
         self.labeltemplate = labeltemplate
 
     def set_locs(self, locs):
         if self.decimalplaces is not None:
-            self.format = "%1." + str(self.decimalplaces) + "f"
+            self.format = f"%1.{self.decimalplaces!s}f"
             if self._usetex:
-                self.format = "$%s$" % self.format
+                self.format = f"${self.format}$"
             elif self._useMathText:
                 self.format = "$%s$" % ("\\mathdefault{%s}" % self.format)
         super().set_locs(locs)
 
         if self.decimalplaces is not None:
             # rounding the tick labels will make the locations incorrect unless we round these too
             newlocs = [
-                float(("%1." + str(self.decimalplaces) + "f") % (x / (10**self.orderOfMagnitude)))
-                * (10**self.orderOfMagnitude)
+                (
+                    float(f"%1.{self.decimalplaces!s}f" % (x / (10**self.orderOfMagnitude)))
+                    * 10**self.orderOfMagnitude
+                )
                 for x in self.locs
             ]
             super().set_locs(newlocs)
 
         self._set_formatted_label_text()
 
+    def _set_format(self, *args, **kwargs):
+        if self.decimalplaces is None:
+            return super()._set_format(*args, **kwargs)
+
+        sigfigs = self.decimalplaces
+        self.format = f"%1.{sigfigs}f"
+        if self._usetex or self._useMathText:
+            self.format = r"$\mathdefault{%s}$" % self.format
+
+        return None
+
     def set_axis(self, axis):
         super().set_axis(axis)
         self._set_formatted_label_text()
 
 
 def set_axis_properties(ax, args):
     if "subplots" not in args:
@@ -140,17 +156,17 @@
     data = np.zeros((ngrid, ngrid))
 
     plot_axes_choices = ["xy", "xz"]
     if plot_axes not in plot_axes_choices:
         print(f"Choose plot axes from {plot_axes_choices}")
         sys.exit(1)
 
-    for z in range(0, ngrid):
-        for y in range(0, ngrid):
-            for x in range(0, ngrid):
+    for z in range(ngrid):
+        for y in range(ngrid):
+            for x in range(ngrid):
                 if plot_axes == "xy":
                     if z == round(ngrid / 2) - 1:
                         data[y, x] = plot_variable_3d_array[x, y, z]
                 elif plot_axes == "xz" and y == round(ngrid / 2) - 1:
                     data[z, x] = plot_variable_3d_array[x, y, z]
 
     return data, extent
@@ -162,17 +178,15 @@
     with margins in fraction of the width of the plot.
 
     Defaults to current axes object if not specified.
     From https://stackoverflow.com/questions/29461608/matplotlib-fixing-x-axis-scale-and-autoscale-y-axis
     """
 
     def calculate_new_limit(fixed, dependent, limit):
-        """Calculates the min/max of the dependent axis given
-        a fixed axis with limits.
-        """
+        """Calculate the min/max of the dependent axis given a fixed axis with limits."""
         if len(fixed) > 2:
             mask = (fixed > limit[0]) & (fixed < limit[1]) & (~np.isnan(dependent)) & (~np.isnan(fixed))
             window = dependent[mask]
             try:
                 low, high = window.min(), window.max()
             except ValueError:  # Will throw ValueError if `window` has zero elements
                 low, high = np.inf, -np.inf
```

### Comparing `artistools-2023.5.16.3/artistools/radfield.py` & `artistools-2023.8.1/artistools/radfield.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
+from __future__ import annotations
+
 import argparse
 import math
 from functools import lru_cache
 from pathlib import Path
-from typing import Optional
-from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from astropy import units as u
 
 import artistools as at
@@ -107,17 +107,15 @@
             return [W * 1.4745007e-47 * pow(nu_hz, 3) * 1.0 / (math.expm1(H * nu_hz / T / KB)) for nu_hz in arr_nu_hz]
         except OverflowError:
             print(f"WARNING: overflow error W {W}, T {T} (Did this happen in ARTIS too?)")
 
     return [0.0 for _ in arr_nu_hz]
 
 
-def get_fullspecfittedfield(
-    radfielddata, xmin, xmax, modelgridindex: Optional[int] = None, timestep: Optional[int] = None
-):
+def get_fullspecfittedfield(radfielddata, xmin, xmax, modelgridindex: int | None = None, timestep: int | None = None):
     row = (
         radfielddata.query(
             "bin_num == -1"
             + (" & modelgridindex==@modelgridindex" if modelgridindex else "")
             + (" & timestep==@timestep" if timestep else "")
         )
         .copy()
@@ -132,19 +130,19 @@
     arr_j_lambda = arr_j_nu * arr_nu_hz / arr_lambda
 
     return arr_lambda, arr_j_lambda
 
 
 def get_fitted_field(
     radfielddata,
-    modelgridindex: Optional[int] = None,
-    timestep: Optional[int] = None,
+    modelgridindex: int | None = None,
+    timestep: int | None = None,
     print_bins: bool = False,
-    lambdamin: Optional[float] = None,
-    lambdamax: Optional[float] = None,
+    lambdamin: float | None = None,
+    lambdamax: float | None = None,
 ) -> tuple[list[float], list[float]]:
     """Return the fitted dilute blackbody (list of lambda, list of j_nu) made up of all bins."""
     arr_lambda = []
     j_lambda_fitted = []
 
     radfielddata_subset = radfielddata.copy().query(
         "bin_num >= 0"
@@ -227,18 +225,18 @@
         )
 
     return ymax
 
 
 def plot_specout(
     axis,
-    specfilename: Union[str, Path],
+    specfilename: str | Path,
     timestep: int,
-    peak_value: Optional[float] = None,
-    scale_factor: Optional[float] = None,
+    peak_value: float | None = None,
+    scale_factor: float | None = None,
     **plotkwargs,
 ) -> None:
     """Plot the ARTIS spectrum."""
     print(f"Plotting {specfilename}")
 
     specfilename = Path(specfilename)
     if specfilename.is_dir():
@@ -299,18 +297,17 @@
     T_e = estimators[(timestep, modelgridindex)]["Te"]
 
     ion_data = adata.query("Z == @atomic_number and ion_stage == @lower_ion_stage").iloc[0]
     upper_ion_data = adata.query("Z == @atomic_number and ion_stage == (@lower_ion_stage + 1)").iloc[0]
 
     lowerionpopdensity = estimators[(timestep, modelgridindex)]["populations"][(atomic_number, lower_ion_stage)]
 
-    ion_popfactor_sum = 0
-    for _, level in ion_data.levels[:max_levels].iterrows():
-        ion_popfactor_sum += level.g * math.exp(-level.energy_ev * EV / KB / T_e)
-
+    ion_popfactor_sum = sum(
+        level.g * math.exp(-level.energy_ev * EV / KB / T_e) for _, level in ion_data.levels[:max_levels].iterrows()
+    )
     array_kappa_bf_nu_ion = np.zeros_like(arr_nu_hz)
     for levelnum, lowerlevel in ion_data.levels[:max_levels].iterrows():
         levelpopfrac = lowerlevel.g * math.exp(-lowerlevel.energy_ev * EV / KB / T_e) / ion_popfactor_sum
 
         for upperlevelnum, phixsfrac in lowerlevel.phixstargetlist:
             upperlevel = upper_ion_data.levels.iloc[upperlevelnum]
 
@@ -343,17 +340,18 @@
     T_e = estimators[(timestep, modelgridindex)]["Te"]
     nne = estimators[(timestep, modelgridindex)]["nne"]
 
     upperionpopdensity = estimators[(timestep, modelgridindex)]["populations"][(atomic_number, upper_ion_stage)]
     print(f"Recombination from {upperionstr} -> {lowerionstr} ({upperionstr} pop = {upperionpopdensity:.1e}/cm3)")
 
     if use_lte_pops:
-        upper_level_popfactor_sum = 0
-        for _upperlevelnum, upperlevel in lower_ion_data.levels[:200].iterrows():
-            upper_level_popfactor_sum += upperlevel.g * math.exp(-upperlevel.energy_ev * EV / KB / T_e)
+        upper_level_popfactor_sum = sum(
+            upperlevel.g * math.exp(-upperlevel.energy_ev * EV / KB / T_e)
+            for _upperlevelnum, upperlevel in lower_ion_data.levels[:200].iterrows()
+        )
     else:
         dfnltepops = at.nltepops.read_files(modelpath, modelgridindex=modelgridindex, timestep=timestep)
         dfnltepops_upperion = dfnltepops.query("Z==@atomic_number & ion_stage==@upper_ion_stage")
         upperion_nltepops = {x.level: x["n_NLTE"] for _, x in dfnltepops_upperion.iterrows()}
 
     arr_j_nu_lowerlevel = {}
     arr_alpha_dnu = np.zeros_like(arr_nu_hz)
@@ -425,15 +423,15 @@
             )
 
     alpha_ion = np.abs(np.trapz(arr_alpha_dnu, x=arr_nu_hz))
     print(f"  {upperionstr} Alpha_R = {alpha_ion:.2e}   Alpha_R*nne = {nne*alpha_ion:.2e}")
     print(f"  {upperionstr} Alpha_R2 = {alpha_ion2:.2e} Alpha_R2*nne = {nne*alpha_ion2:.2e}")
 
     # vmax = at.inputmodel.get_modeldata_tuple(modelpath)[0]['velocity_outer'].iloc[-1] * 1e5
-    # t_seconds = at.get_timestep_times_float(modelpath, loc="start")[timestep] * 86400.0
+    # t_seconds = at.get_timestep_times(modelpath, loc="start")[timestep] * 86400.0
 
     # mean_free_path = vmax * t_seconds
 
     arr_j_nu = arr_alpha_dnu / 4 / math.pi * H * arr_nu_hz * upperionpopdensity * nne
     return arr_j_nu, arr_j_nu_lowerlevel
 
 
@@ -445,18 +443,17 @@
     T_R = estimators[(timestep, modelgridindex)]["TR"]
 
     adata = at.atomic.get_levels(modelpath, get_photoionisations=True)
     ion_data = adata.query("Z == @atomic_number and ion_stage == @ion_stage").iloc[0]
     upper_ion_data = adata.query("Z == @atomic_number and ion_stage == (@ion_stage + 1)").iloc[0]
     ionstr = at.get_ionstring(atomic_number, ion_stage)
 
-    ion_popfactor_sum = 0
-    for _, level in ion_data.levels[:max_levels].iterrows():
-        ion_popfactor_sum += level.g * math.exp(-level.energy_ev * EV / KB / T_e)
-
+    ion_popfactor_sum = sum(
+        level.g * math.exp(-level.energy_ev * EV / KB / T_e) for _, level in ion_data.levels[:max_levels].iterrows()
+    )
     arr_gamma_dnu = np.zeros_like(arr_nu_hz)
     for levelnum, level in ion_data.levels[:max_levels].iterrows():
         levelpopfrac = level.g * math.exp(-level.energy_ev * EV / KB / T_e) / ion_popfactor_sum
 
         for upperlevelnum, phixsfrac in level.phixstargetlist:
             upperlevel = upper_ion_data.levels.iloc[upperlevelnum]
             nu_threshold = ONEOVERH * (ion_data.ion_pot - level.energy_ev + upperlevel.energy_ev) * EV
@@ -608,14 +605,15 @@
 
         fieldlist += [
             (arraylambda_angstrom_em, contribrow.array_flambda_emission, contribrow.linelabel)
             for contribrow in contribution_list
         ]
         fieldlist += [(arraylambda_angstrom_em, array_jlambda_emission_total, "Total emission")]
 
+    lw = 1.0
     # fieldlist += [(arr_lambda_fitted, j_lambda_fitted, 'binned field')]
 
     for atomic_number, ion_stage in photoionlist:
         ionstr = at.get_ionstring(atomic_number, ion_stage)
         ion_data = adata.query("Z == @atomic_number and ion_stage == @ion_stage").iloc[0]
 
         for levelnum, level in ion_data.levels[:max_levels].iterrows():
@@ -624,15 +622,14 @@
                 modelpath, atomic_number, ion_stage, levelnum, nu_threshold, tuple(arr_nu_hz_recomb)
             )
             if levelnum < 5:
                 axes[0].plot(
                     arraylambda_angstrom_recomb, arr_sigma_bf, label=rf"$\sigma_{{bf}}$({ionstr} {level.levelname})"
                 )
 
-        lw = 1.0
         for arraylambda_angstrom, J_lambda_arr, linelabel in fieldlist:
             # lw -= 0.4
             arr_nu_hz = 2.99792458e18 / np.array(arraylambda_angstrom)
             print(f"{ionstr} photoionisation rate coeffs using radiation field due to {linelabel}")
             J_nu_arr = np.array(J_lambda_arr) * arraylambda_angstrom / arr_nu_hz
 
             arr_gamma_dnu = get_ion_gamma_dnu(
@@ -666,20 +663,20 @@
     """Plot a cell at a timestep things like the bin edges, fitted field, and emergent spectrum (from all cells)."""
     radfielddata = read_files(modelpath, timestep=timestep, modelgridindex=modelgridindex)
     if radfielddata.empty:
         print(f"No data for timestep {timestep:d} modelgridindex {modelgridindex:d}")
         return False
 
     modelname = at.get_model_name(modelpath)
-    time_days = at.get_timestep_times_float(modelpath)[timestep]
+    time_days = at.get_timestep_times(modelpath)[timestep]
     print(f"Plotting {modelname} timestep {timestep:d} (t={time_days:.3f}d)")
     T_R = radfielddata.query("bin_num == -1").iloc[0].T_R
     print(f"T_R = {T_R}")
 
-    nrows = 1 if not args.photoionrates else 3
+    nrows = 3 if args.photoionrates else 1
     fig, axes = plt.subplots(
         nrows=nrows,
         ncols=1,
         sharex=True,
         figsize=(
             args.figscale * at.get_config()["figwidth"],
             args.figscale * at.get_config()["figwidth"] * (0.25 + nrows * 0.4),
@@ -710,18 +707,15 @@
 
     axis.plot(arr_lambda_fitted, j_lambda_fitted, label="Radiation field model", alpha=0.8, color="blue", linewidth=1.5)
 
     ymax3 = plot_line_estimators(
         axis, radfielddata, xmin, xmax, modelgridindex=modelgridindex, timestep=timestep, zorder=-2, color="red"
     )
 
-    ymax = max(ymax, ymax3)
-    if args.ymax >= 0:
-        ymax = args.ymax
-
+    ymax = args.ymax if args.ymax >= 0 else max(ymax, ymax3)
     try:
         specfilename = at.firstexisting("spec.out", folder=modelpath, tryzipped=True)
     except FileNotFoundError:
         print("Could not find spec.out")
         args.nospec = True
 
     if not args.nospec:
@@ -883,15 +877,15 @@
     timestep = at.get_timestep_of_timedays(modelpath, 330)
     time_days = float(at.get_timestep_time(modelpath, timestep))
 
     dftopestimators = radfielddataselected.query("timestep==@timestep and bin_num < -1").copy()
     dftopestimators = dftopestimators.eval("lambda_angstroms = 2.99792458e18 / nu_upper")
     dftopestimators = dftopestimators.eval("Jb_lambda = J_nu_avg * (nu_upper ** 2) / 2.99792458e18")
     dftopestimators = dftopestimators.sort_values(by="Jb_lambda", ascending=False)
-    dftopestimators = dftopestimators.iloc[0:nlinesplotted]
+    dftopestimators = dftopestimators.iloc[:nlinesplotted]
 
     print(f"Top estimators at timestep {timestep} t={time_days:.1f}")
     print(dftopestimators)
 
     for ax, bin_num_estimator, nu_line in zip(
         axes, dftopestimators.bin_num.to_numpy(), dftopestimators.nu_upper.to_numpy()
     ):
@@ -999,38 +993,37 @@
     if args.velocity >= 0.0:
         modelgridindexlist = [at.inputmodel.get_mgi_of_velocity_kms(modelpath, args.velocity)]
     elif args.modelgridindex is None:
         modelgridindexlist = [0]
     else:
         modelgridindexlist = at.parse_range_list(args.modelgridindex)
 
-    timesteplast = len(at.get_timestep_times_float(modelpath))
+    timesteplast = len(at.get_timestep_times(modelpath))
     if args.timedays:
         timesteplist = [at.get_timestep_of_timedays(modelpath, args.timedays)]
     elif args.timestep:
         timesteplist = at.parse_range_list(args.timestep, dictvars={"last": timesteplast})
     else:
         print("Using last timestep.")
         timesteplist = [timesteplast]
 
     for modelgridindex in modelgridindexlist:
         if args.xaxis == "lambda":
             for timestep in timesteplist:
                 outputfile = str(args.outputfile).format(modelgridindex=modelgridindex, timestep=timestep)
-                make_plot = plot_celltimestep(
+                if make_plot := plot_celltimestep(
                     modelpath,
                     timestep,
                     outputfile,
                     xmin=args.xmin,
                     xmax=args.xmax,
                     modelgridindex=modelgridindex,
                     args=args,
                     normalised=args.normalised,
-                )
-                if make_plot:
+                ):
                     pdf_list.append(outputfile)
                     modelpath_list.append(args.modelpath)
         elif args.xaxis == "timestep":
             outputfile = args.outputfile.format(modelgridindex=modelgridindex)
             plot_timeevolution(modelpath, outputfile, modelgridindex, args)
         else:
             print("Unknown plot type {args.plot}")
```

### Comparing `artistools-2023.5.16.3/artistools/spectra/__init__.py` & `artistools-2023.8.1/artistools/spectra/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Artistools - spectra related functions."""
 from .plotspectra import main
 from .plotspectra import main as plot
 from .spectra import get_exspec_bins
 from .spectra import get_flux_contributions
 from .spectra import get_flux_contributions_from_packets
 from .spectra import get_from_packets
-from .spectra import get_line_flux
 from .spectra import get_reference_spectrum
 from .spectra import get_specpol_data
 from .spectra import get_spectrum
 from .spectra import get_spectrum_at_time
 from .spectra import get_vspecpol_data
 from .spectra import get_vspecpol_spectrum
 from .spectra import make_averaged_vspecfiles
 from .spectra import make_virtual_spectra_summed_file
-from .spectra import print_floers_line_ratio
 from .spectra import print_integrated_flux
 from .spectra import read_spec_res
 from .spectra import sort_and_reduce_flux_contribution_list
 from .spectra import stackspectra
 from .spectra import timeshift_fluxscale_co56law
 from .spectra import write_flambda_spectra
```

### Comparing `artistools-2023.5.16.3/artistools/spectra/plotspectra.py` & `artistools-2023.8.1/artistools/spectra/plotspectra.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,46 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
 """Artistools - spectra plotting functions."""
+from __future__ import annotations
+
 import argparse
-import os
 import sys
-from collections.abc import Collection
+import typing as t
 from pathlib import Path
-from typing import Any
-from typing import Callable
-from typing import Optional
-from typing import Union
 
 import argcomplete
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib import ticker
 from matplotlib.artist import Artist
+from typeguard import typechecked
 
 import artistools as at
-import artistools.packets
-
-from .spectra import get_from_packets
-from .spectra import get_reference_spectrum
-from .spectra import get_specpol_data
-from .spectra import get_spectrum
-from .spectra import get_vspecpol_spectrum
-from .spectra import make_averaged_vspecfiles
-from .spectra import make_virtual_spectra_summed_file
-from .spectra import print_integrated_flux
-from .spectra import timeshift_fluxscale_co56law
 
 hatches = ["", "x", "-", "\\", "+", "O", ".", "", "x", "*", "\\", "+", "O", "."]  # ,
 
 
 def plot_polarisation(modelpath: Path, args) -> None:
     angle = args.plotviewingangle[0]
-    stokes_params = get_specpol_data(angle=angle, modelpath=modelpath)
+    stokes_params = at.spectra.get_specpol_data(angle=angle, modelpath=modelpath)
     stokes_params[args.stokesparam] = stokes_params[args.stokesparam].eval("lambda_angstroms = 2.99792458e18 / nu")
 
     timearray = stokes_params[args.stokesparam].keys()[1:-1]
     (timestepmin, timestepmax, args.timemin, args.timemax) = at.get_time_range(
         modelpath, args.timestep, args.timemin, args.timemax, args.timedays
     )
     assert args.timemin is not None
     assert args.timemax is not None
     timeavg = (args.timemin + args.timemax) / 2.0
 
     def match_closest_time(reftime):
-        return str(f"{min([float(x) for x in timearray], key=lambda x: abs(x - reftime)):.4f}")
+        return str(f"{min((float(x) for x in timearray), key=lambda x: abs(x - reftime)):.4f}")
 
     timeavg = match_closest_time(timeavg)
 
     filterfunc = at.get_filterfunc(args)
     if filterfunc is not None:
         print("Applying filter to ARTIS spectrum")
         stokes_params[args.stokesparam][timeavg] = filterfunc(stokes_params[args.stokesparam][timeavg])
@@ -102,57 +89,70 @@
     plt.ylabel(f"{args.stokesparam}")
     plt.xlabel(r"Wavelength ($\mathrm{{\AA}}$)")
     figname = f"plotpol_{timeavg}_days_{args.stokesparam.split('/')[0]}_{args.stokesparam.split('/')[1]}.pdf"
     plt.savefig(modelpath / figname, format="pdf")
     print(f"Saved {figname}")
 
 
+@typechecked
 def plot_reference_spectrum(
-    filename: Union[Path, str],
+    filename: Path | str,
     axis: plt.Axes,
     xmin: float,
     xmax: float,
-    flambdafilterfunc: Optional[Callable[[np.ndarray], np.ndarray]] = None,
-    scale_to_peak: Optional[float] = None,
+    flambdafilterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
+    scale_to_peak: float | None = None,
     scale_to_dist_mpc: float = 1,
-    scaletoreftime: Optional[float] = None,
+    scaletoreftime: float | None = None,
     **plotkwargs,
 ):
     """Plot a single reference spectrum.
 
     The filename must be in space separated text formated with the first two
     columns being wavelength in Angstroms, and F_lambda
     """
-    specdata, metadata = get_reference_spectrum(filename)
+    specdata, metadata = at.spectra.get_reference_spectrum(filename)
 
     # scale to flux at required distance
     if scale_to_dist_mpc:
         print(f"Scale to {scale_to_dist_mpc} Mpc")
         assert metadata["dist_mpc"] > 0  # we must know the true distance in order to scale to some other distance
         specdata["f_lambda"] = specdata["f_lambda"] * (metadata["dist_mpc"] / scale_to_dist_mpc) ** 2
 
     if "label" not in plotkwargs:
         plotkwargs["label"] = metadata["label"] if "label" in metadata else filename
 
     if scaletoreftime is not None:
-        timefactor = timeshift_fluxscale_co56law(scaletoreftime, float(metadata["t"]))
+        timefactor = at.spectra.timeshift_fluxscale_co56law(scaletoreftime, float(metadata["t"]))
         print(f" Scale from time {metadata['t']} to {scaletoreftime}, factor {timefactor} using Co56 decay law")
         specdata["f_lambda"] *= timefactor
         plotkwargs["label"] += f" * {timefactor:.2f}"
     if "scale_factor" in metadata:
         specdata["f_lambda"] *= metadata["scale_factor"]
-
+    if metadata.get("mask_telluric", False):
+        print("Masking telluric regions")
+        z = metadata["z"]
+        bands = [(1.35e4, 1.44e4), (1.8e4, 1.94e4)]  # [Angstroms]
+        for band_low_rest, band_high_rest in bands:
+            band_low = band_low_rest / (1 + z)
+            band_high = band_high_rest / (1 + z)
+            # specdata = specdata.query("lambda_angstroms < @band_low or lambda_angstroms > @band_high")
+            specdata.loc[
+                (specdata["lambda_angstroms"] >= band_low) & (specdata["lambda_angstroms"] <= band_high), "f_lambda"
+            ] = float("nan")
     print(f"Reference spectrum '{plotkwargs['label']}' has {len(specdata)} points in the plot range")
     print(f" file: {filename}")
 
     print(" metadata: " + ", ".join([f"{k}='{v}'" if hasattr(v, "lower") else f"{k}={v}" for k, v in metadata.items()]))
 
     specdata = specdata.query("lambda_angstroms > @xmin and lambda_angstroms < @xmax")
 
-    print_integrated_flux(specdata["f_lambda"], specdata["lambda_angstroms"], distance_megaparsec=metadata["dist_mpc"])
+    at.spectra.print_integrated_flux(
+        specdata["f_lambda"], specdata["lambda_angstroms"], distance_megaparsec=metadata["dist_mpc"]
+    )
 
     # if len(specdata) > 5000:
     #     # specdata = scipy.signal.resample(specdata, 10000)
     #     # specdata = specdata.iloc[::3, :].copy()
     #     print(f" downsampling to {len(specdata)} points")
     #     specdata = specdata.query("index % 3 == 0")
 
@@ -165,52 +165,54 @@
     if scale_to_peak:
         specdata["f_lambda_scaled"] = specdata["f_lambda"] / specdata["f_lambda"].max() * scale_to_peak
         ycolumnname = "f_lambda_scaled"
     else:
         ycolumnname = "f_lambda"
 
     ymax = max(specdata[ycolumnname])
-    lineplot = specdata.plot(x="lambda_angstroms", y=ycolumnname, ax=axis, legend=None, **plotkwargs)
+    (lineplot,) = axis.plot(specdata["lambda_angstroms"], specdata[ycolumnname], **plotkwargs)
 
-    return mpatches.Patch(color=lineplot.get_lines()[0].get_color()), plotkwargs["label"], ymax
+    return lineplot, plotkwargs["label"], ymax
 
 
 def plot_filter_functions(axis: plt.Axes) -> None:
     filter_names = ["U", "B", "V", "I"]
     colours = ["r", "b", "g", "c", "m"]
 
-    filterdir = os.path.join(at.get_config()["path_artistools_dir"], "data/filters/")
+    filterdir = Path(at.get_config()["path_artistools_dir"], "data/filters/")
     for index, filter_name in enumerate(filter_names):
         filter_data = pd.read_csv(
-            filterdir / Path(f"{filter_name}.txt"),
+            filterdir / f"{filter_name}.txt",
             delim_whitespace=True,
             header=None,
             skiprows=4,
             names=["lamba_angstroms", "flux_normalised"],
         )
         filter_data.plot(
             x="lamba_angstroms", y="flux_normalised", ax=axis, label=filter_name, color=colours[index], alpha=0.3
         )
 
 
+@typechecked
 def plot_artis_spectrum(
-    axes: Collection[plt.Axes],
-    modelpath: Union[Path, str],
+    axes: t.Collection[plt.Axes],
+    modelpath: Path | str,
     args,
-    scale_to_peak: Optional[float] = None,
+    scale_to_peak: float | None = None,
     from_packets: bool = False,
-    filterfunc: Optional[Callable[[np.ndarray], np.ndarray]] = None,
-    linelabel: Optional[str] = None,
+    filterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
+    linelabel: str | None = None,
     plotpacketcount: bool = False,
-    directionbins: Optional[list[int]] = None,
+    directionbins: list[int] | None = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
-    maxpacketfiles: Optional[int] = None,
+    usedegrees: bool = False,
+    maxpacketfiles: int | None = None,
     **plotkwargs,
-) -> Optional[pd.DataFrame]:
+) -> pd.DataFrame | None:
     """Plot an ARTIS output spectrum. The data plotted are also returned as a DataFrame."""
     modelpath = Path(modelpath)
     if Path(modelpath).is_file():  # handle e.g. modelpath = 'modelpath/spec.out'
         specfilename = Path(modelpath).parts[-1]
         print(f"WARNING: ignoring filename of {specfilename}")
         modelpath = Path(modelpath).parent
 
@@ -242,15 +244,15 @@
         assert args.timemax is not None
         timeavg = (args.timemin + args.timemax) / 2.0
         timedelta = (args.timemax - args.timemin) / 2
         if linelabel is None:
             linelabel = f"{modelname}" if len(modelname) < 70 else f"...{modelname[-67:]}"
 
             if not args.hidemodeltime and not args.multispecplot:
-                # todo: fix this for multispecplot - use args.showtime for now
+                # TODO: fix this for multispecplot - use args.showtime for now
                 linelabel += f" +{timeavg:.1f}d"
             if not args.hidemodeltimerange and not args.multispecplot:
                 linelabel += rf" ($\pm$ {timedelta:.1f}d)"
         # Luke: disabled below because line label has already been formatted with e.g. timeavg values
         # formatting for a second time makes it impossible to use curly braces in line labels (needed for LaTeX math)
         # else:
         #     linelabel = linelabel.format(**locals())
@@ -265,15 +267,15 @@
         dbins_get = list(directionbins).copy()
         if -1 not in dbins_get:
             dbins_get.append(-1)
 
         supxmin, supxmax = axis.get_xlim()
         if from_packets:
             assert args.plotvspecpol is None
-            viewinganglespectra = get_from_packets(
+            viewinganglespectra = at.spectra.get_from_packets(
                 modelpath,
                 args.timemin,
                 args.timemax,
                 lambda_min=supxmin * 0.9,
                 lambda_max=supxmax * 1.1,
                 use_escapetime=args.use_escapetime,
                 maxpacketfiles=maxpacketfiles,
@@ -281,66 +283,66 @@
                 useinternalpackets=args.internalpackets,
                 getpacketcount=plotpacketcount,
                 directionbins=dbins_get,
                 average_over_phi=average_over_phi,
                 average_over_theta=average_over_theta,
                 fnufilterfunc=filterfunc,
             )
-        else:
-            if args.plotvspecpol is not None:  # noqa: PLR5501
-                # read virtual packet files (after running plotartisspectrum --makevspecpol)
-                vpkt_config = at.get_vpkt_config(modelpath)
-                if vpkt_config["time_limits_enabled"] and (
-                    args.timemin < vpkt_config["initial_time"] or args.timemax > vpkt_config["final_time"]
-                ):
-                    print(
-                        f"Timestep out of range of virtual packets: start time {vpkt_config['initial_time']} days "
-                        f"end time {vpkt_config['final_time']} days"
-                    )
-                    sys.exit(1)
-
-                viewinganglespectra = {
-                    dirbin: get_vspecpol_spectrum(modelpath, timeavg, dirbin, args, fnufilterfunc=filterfunc)
-                    for dirbin in dbins_get
-                    if dirbin >= 0
-                }
-            else:
-                viewinganglespectra = get_spectrum(
-                    modelpath=modelpath,
-                    directionbins=dbins_get,
-                    timestepmin=timestepmin,
-                    timestepmax=timestepmax,
-                    average_over_phi=average_over_phi,
-                    average_over_theta=average_over_theta,
-                    fnufilterfunc=filterfunc,
+        elif args.plotvspecpol is not None:
+            # read virtual packet files (after running plotartisspectrum --makevspecpol)
+            vpkt_config = at.get_vpkt_config(modelpath)
+            if vpkt_config["time_limits_enabled"] and (
+                args.timemin < vpkt_config["initial_time"] or args.timemax > vpkt_config["final_time"]
+            ):
+                print(
+                    f"Timestep out of range of virtual packets: start time {vpkt_config['initial_time']} days "
+                    f"end time {vpkt_config['final_time']} days"
                 )
+                sys.exit(1)
+
+            viewinganglespectra = {
+                dirbin: at.spectra.get_vspecpol_spectrum(modelpath, timeavg, dirbin, args, fnufilterfunc=filterfunc)
+                for dirbin in dbins_get
+                if dirbin >= 0
+            }
+        else:
+            viewinganglespectra = at.spectra.get_spectrum(
+                modelpath=modelpath,
+                directionbins=dbins_get,
+                timestepmin=timestepmin,
+                timestepmax=timestepmax,
+                average_over_phi=average_over_phi,
+                average_over_theta=average_over_theta,
+                fnufilterfunc=filterfunc,
+            )
 
         dirbin_definitions = (
-            at.get_dirbin_labels(
+            at.get_vspec_dir_labels(modelpath=modelpath, viewinganglelabelunits=args.viewinganglelabelunits)
+            if args.plotvspecpol
+            else at.get_dirbin_labels(
                 dirbins=directionbins,
                 modelpath=modelpath,
                 average_over_phi=average_over_phi,
                 average_over_theta=average_over_theta,
+                usedegrees=usedegrees,
             )
-            if not args.plotvspecpol
-            else at.get_vspec_dir_labels(modelpath=modelpath, viewinganglelabelunits=args.viewinganglelabelunits)
         )
 
         for dirbin in directionbins:
             dfspectrum = (
                 viewinganglespectra[dirbin]
                 .query("@supxmin * 0.9 <= lambda_angstroms and lambda_angstroms <= @supxmax * 1.1")
                 .copy()
             )
 
             if dirbin != -1:
                 linelabel = dirbin_definitions[dirbin]
                 print(f" direction {dirbin:4d}  {dirbin_definitions[dirbin]}")
 
-            print_integrated_flux(dfspectrum["f_lambda"], dfspectrum["lambda_angstroms"])
+            at.spectra.print_integrated_flux(dfspectrum["f_lambda"], dfspectrum["lambda_angstroms"])
 
             if scale_to_peak:
                 dfspectrum["f_lambda_scaled"] = dfspectrum["f_lambda"] / dfspectrum["f_lambda"].max() * scale_to_peak
                 if args.plotvspecpol is not None:
                     for angle in args.plotvspecpol:
                         viewinganglespectra[angle]["f_lambda_scaled"] = (
                             viewinganglespectra[angle]["f_lambda"]
@@ -360,18 +362,16 @@
                 binned_flux = []
 
                 wavelengths = dfspectrum["lambda_angstroms"]
                 fluxes = dfspectrum[ycolumnname]
                 nbins = 5
 
                 for i in np.arange(0, len(wavelengths - nbins), nbins):
-                    new_lambda_angstroms.append(wavelengths[i + int(nbins / 2)])
-                    sum_flux = 0
-                    for j in range(i, i + nbins):
-                        sum_flux += fluxes[j]
+                    new_lambda_angstroms.append(wavelengths[i + nbins // 2])
+                    sum_flux = sum(fluxes[j] for j in range(i, i + nbins))
                     binned_flux.append(sum_flux / nbins)
 
                 dfspectrum = pd.DataFrame({"lambda_angstroms": new_lambda_angstroms, ycolumnname: binned_flux})
 
             axis.plot(
                 dfspectrum["lambda_angstroms"],
                 dfspectrum[ycolumnname],
@@ -379,32 +379,30 @@
                 **plotkwargs,
             )
 
     return dfspectrum[["lambda_angstroms", "f_lambda"]]
 
 
 def make_spectrum_plot(
-    speclist: Collection[Union[Path, str]],
+    speclist: t.Collection[Path | str],
     axes: plt.Axes,
-    filterfunc: Optional[Callable[[np.ndarray], np.ndarray]],
+    filterfunc: t.Callable[[np.ndarray], np.ndarray] | None,
     args,
-    scale_to_peak: Optional[float] = None,
+    scale_to_peak: float | None = None,
 ) -> pd.DataFrame:
     """Plot reference spectra and ARTIS spectra."""
     dfalldata = pd.DataFrame()
     artisindex = 0
     refspecindex = 0
     seriesindex = 0
 
     for seriesindex, specpath in enumerate(speclist):
         specpath = Path(specpath)
-        plotkwargs: dict[str, Any] = {}
-        plotkwargs["alpha"] = 0.95
+        plotkwargs: dict[str, t.Any] = {"alpha": args.linealpha[seriesindex], "linestyle": args.linestyle[seriesindex]}
 
-        plotkwargs["linestyle"] = args.linestyle[seriesindex]
         if not args.plotviewingangle and not args.plotvspecpol:
             plotkwargs["color"] = args.color[seriesindex]
         if args.dashes[seriesindex]:
             plotkwargs["dashes"] = args.dashes[seriesindex]
         if args.linewidth[seriesindex]:
             plotkwargs["linewidth"] = args.linewidth[seriesindex]
 
@@ -444,15 +442,15 @@
             refspecindex += 1
         elif not specpath.exists() and specpath.parts[0] == "codecomparison":
             # timeavg = (args.timemin + args.timemax) / 2.
             (timestepmin, timestepmax, args.timemin, args.timemax) = at.get_time_range(
                 specpath, args.timestep, args.timemin, args.timemax, args.timedays
             )
             timeavg = args.timedays
-            artistools.codecomparison.plot_spectrum(specpath, timedays=timeavg, ax=axes[0], **plotkwargs)
+            at.codecomparison.plot_spectrum(specpath, timedays=timeavg, ax=axes[0], **plotkwargs)
             refspecindex += 1
         else:
             # ARTIS model spectrum
             # plotkwargs['dash_capstyle'] = dash_capstyleList[artisindex]
             if "linewidth" not in plotkwargs:
                 plotkwargs["linewidth"] = 1.3
 
@@ -463,17 +461,18 @@
                 specpath,
                 args=args,
                 scale_to_peak=scale_to_peak,
                 from_packets=args.frompackets,
                 maxpacketfiles=args.maxpacketfiles,
                 filterfunc=filterfunc,
                 plotpacketcount=args.plotpacketcount,
-                directionbins=args.plotviewingangle if not args.plotvspecpol else args.plotvspecpol,
+                directionbins=args.plotvspecpol or args.plotviewingangle,
                 average_over_phi=args.average_over_phi_angle,
                 average_over_theta=args.average_over_theta_angle,
+                usedegrees=args.usedegrees,
                 **plotkwargs,
             )
             if seriesdata is not None:
                 seriesname = at.get_model_name(specpath)
                 artisindex += 1
 
         if args.write_data and not seriesdata.empty:
@@ -520,25 +519,38 @@
         if args.stokesparam == "I":
             axis.set_ylim(bottom=0.0)
         if args.normalised:
             axis.set_ylim(top=1.25)
             axis.set_ylabel(r"Scaled F$_\lambda$")
         if args.plotpacketcount:
             axis.set_ylabel(r"Monte Carlo packets per bin")
+        if not args.notitle and args.title:
+            if args.inset_title:
+                axis.annotate(
+                    args.title,
+                    xy=(0.03, 0.97),
+                    xycoords="axes fraction",
+                    horizontalalignment="left",
+                    verticalalignment="top",
+                    fontsize="x-large",
+                )
+            else:
+                axis.set_title(args.title, fontsize=11)
 
     return dfalldata
 
 
+@typechecked
 def make_emissionabsorption_plot(
     modelpath: Path,
     axis: plt.Axes,
-    filterfunc: Optional[Callable[[np.ndarray], np.ndarray]] = None,
+    filterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
     args=None,
-    scale_to_peak: Optional[float] = None,
-) -> tuple[list[Artist], list[str], Optional[pd.DataFrame]]:
+    scale_to_peak: float | None = None,
+) -> tuple[list[Artist], list[str], pd.DataFrame | None]:
     """Plot the emission and absorption contribution spectra, grouped by ion/line/term for an ARTIS model."""
     modelname = at.get_model_name(modelpath)
 
     print(f"====> {modelname}")
     arraynu = at.get_nu_grid(modelpath)
 
     (timestepmin, timestepmax, args.timemin, args.timemax) = at.get_time_range(
@@ -603,46 +615,43 @@
         greyscale=args.greyscale,
     )
 
     plotobjectlabels = []
     plotobjects = []
 
     max_flambda_emission_total = max(
-        [
-            flambda if (xmin < lambda_ang < xmax) else -99.0
-            for lambda_ang, flambda in zip(arraylambda_angstroms, array_flambda_emission_total)
-        ]
+        flambda if (xmin < lambda_ang < xmax) else -99.0
+        for lambda_ang, flambda in zip(arraylambda_angstroms, array_flambda_emission_total)
     )
 
     scalefactor = scale_to_peak / max_flambda_emission_total if scale_to_peak else 1.0
 
     if not args.hidenetspectrum:
-        plotobjectlabels.append("Net spectrum")
-        line = axis.plot(
+        plotobjectlabels.append("Spectrum")
+        (line,) = axis.plot(
             arraylambda_angstroms, array_flambda_emission_total * scalefactor, linewidth=1.5, color="black", zorder=100
         )
-        linecolor = line[0].get_color()
-        plotobjects.append(mpatches.Patch(color=linecolor))
+        plotobjects.append(line)
 
     dfaxisdata = pd.DataFrame(index=arraylambda_angstroms)
     dfaxisdata.index.name = "lambda_angstroms"
     # dfaxisdata['nu_hz'] = arraynu
     for x in contributions_sorted_reduced:
         dfaxisdata["emission_flambda." + x.linelabel] = x.array_flambda_emission
         if args.showabsorption:
             dfaxisdata["absorption_flambda." + x.linelabel] = x.array_flambda_absorption
 
     if args.nostack:
         for x in contributions_sorted_reduced:
             if args.showemission:
-                emissioncomponentplot = axis.plot(
+                (emissioncomponentplot,) = axis.plot(
                     arraylambda_angstroms, x.array_flambda_emission * scalefactor, linewidth=1, color=x.color
                 )
 
-                linecolor = emissioncomponentplot[0].get_color()
+                linecolor = emissioncomponentplot.get_color()
             else:
                 linecolor = None
             plotobjects.append(mpatches.Patch(color=linecolor))
 
             if args.showabsorption:
                 axis.plot(
                     arraylambda_angstroms,
@@ -685,14 +694,16 @@
     ymaxrefall = 0.0
     plotkwargs = {}
     for index, filepath in enumerate(args.specpath):
         if Path(filepath).is_dir() or Path(filepath).name.endswith(".out"):
             continue
         if index < len(args.color):
             plotkwargs["color"] = args.color[index]
+            plotkwargs["label"] = args.label[index]
+            plotkwargs["alpha"] = args.linealpha[index]
 
         supxmin, supxmax = axis.get_xlim()
         plotobj, serieslabel, ymaxref = plot_reference_spectrum(
             filepath,
             axis,
             supxmin,
             supxmax,
@@ -702,42 +713,58 @@
             **plotkwargs,
         )
         ymaxrefall = max(ymaxrefall, ymaxref)
 
         plotobjects.append(plotobj)
         plotobjectlabels.append(serieslabel)
 
-    axis.axhline(color="white", linewidth=0.5)
+    axis.axhline(color="black", linewidth=1)
 
-    plotlabel = f"{modelname}\n{args.timemin:.2f}d to {args.timemax:.2f}d"
-    if args.plotviewingangle:
-        dirbin_definitions = at.get_dirbin_labels(
-            dirbins=args.plotviewingangle,
-            modelpath=modelpath,
-            average_over_phi=args.average_over_phi_angle,
-            average_over_theta=args.average_over_theta_angle,
-        )
-        plotlabel += f", directionbin {dirbin_definitions[args.plotviewingangle[0]]}"
+    if args.title:
+        plotlabel = args.title
+    else:
+        plotlabel = f"{modelname}\n{args.timemin:.2f}d to {args.timemax:.2f}d"
+        if args.plotviewingangle:
+            dirbin_definitions = at.get_dirbin_labels(
+                dirbins=args.plotviewingangle,
+                modelpath=modelpath,
+                average_over_phi=args.average_over_phi_angle,
+                average_over_theta=args.average_over_theta_angle,
+                usedegrees=args.usedegrees,
+            )
+            plotlabel += f", directionbin {dirbin_definitions[args.plotviewingangle[0]]}"
 
     if not args.notitle:
-        axis.set_title(plotlabel, fontsize=11)
+        if args.inset_title:
+            axis.annotate(
+                plotlabel,
+                xy=(0.03, 0.96),
+                xycoords="axes fraction",
+                horizontalalignment="left",
+                verticalalignment="top",
+                fontsize="large",
+            )
+        else:
+            axis.set_title(plotlabel, fontsize=11)
+
     # axis.annotate(plotlabel, xy=(0.97, 0.03), xycoords='axes fraction',
     #               horizontalalignment='right', verticalalignment='bottom', fontsize=7)
 
     ymax = max(ymaxrefall, scalefactor * max_flambda_emission_total * 1.2)
     axis.set_ylim(top=ymax)
 
-    if scale_to_peak:
-        axis.set_ylabel(r"Scaled F$_\lambda$")
-    elif args.internalpackets:
-        if args.logscale:
-            # don't include the {} that will be replaced with the power of 10 by the custom formatter
-            axis.set_ylabel(r"J$_\lambda$ [erg/s/cm$^2$/$\mathrm{{\AA}}$]")
-        else:
-            axis.set_ylabel(r"J$_\lambda$ [{}erg/s/cm$^2$/$\mathrm{{\AA}}$]")
+    if not args.hideyticklabels:
+        if scale_to_peak:
+            axis.set_ylabel(r"Scaled F$_\lambda$")
+        elif args.internalpackets:
+            if args.logscale:
+                # don't include the {} that will be replaced with the power of 10 by the custom formatter
+                axis.set_ylabel(r"J$_\lambda$ [erg/s/cm$^2$/$\mathrm{{\AA}}$]")
+            else:
+                axis.set_ylabel(r"J$_\lambda$ [{}erg/s/cm$^2$/$\mathrm{{\AA}}$]")
 
     if args.showbinedges:
         radfielddata = at.radfield.read_files(modelpath, timestep=timestepmax, modelgridindex=30)
         binedges = at.radfield.get_binedges(radfielddata)
         axis.vlines(binedges, ymin=0.0, ymax=ymax, linewidth=0.5, color="red", label="", zorder=-1, alpha=0.4)
 
     return plotobjects, plotobjectlabels, dfaxisdata
@@ -748,23 +775,23 @@
         modelpath, args.timestep, args.timemin, args.timemax, args.timedays
     )
 
     modeldata, _ = at.inputmodel.get_modeldata(modelpath)
 
     if args.classicartis:
         modeldata, _ = at.inputmodel.get_modeldata(modelpath)
-        estimators = artistools.estimators.estimators_classic.read_classic_estimators(modelpath, modeldata)
+        estimators = at.estimators.estimators_classic.read_classic_estimators(modelpath, modeldata)
         allnonemptymgilist = list(modeldata.index)
 
     else:
         estimators = at.estimators.read_estimators(modelpath=modelpath)
         allnonemptymgilist = [
             modelgridindex for modelgridindex in modeldata.index if not estimators[(0, modelgridindex)]["emptycell"]
         ]
-
+    assert estimators is not None
     packetsfiles = at.packets.get_packetsfilepaths(modelpath, args.maxpacketfiles)
     assert args.timemin is not None
     assert args.timemax is not None
     # tdays_min = float(args.timemin)
     # tdays_max = float(args.timemax)
 
     c_ang_s = 2.99792458e18
@@ -776,15 +803,15 @@
     for packetsfile in packetsfiles:
         dfpackets = at.packets.readfile(packetsfile, packet_type="TYPE_ESCAPE", escape_type="TYPE_RPKT")
 
         dfpackets_selected = dfpackets.query(
             "@nu_min <= nu_rf < @nu_max and t_arrive_d >= @tdays_min and t_arrive_d <= @tdays_max", inplace=False
         ).copy()
 
-        # todo: optimize this to avoid calculating unused columns
+        # TODO: optimize this to avoid calculating unused columns
         dfpackets_selected = at.packets.add_derived_columns(
             dfpackets_selected,
             modelpath,
             ["em_timestep", "emtrue_modelgridindex", "emission_velocity"],
             allnonemptymgilist=allnonemptymgilist,
         )
 
@@ -805,77 +832,83 @@
                         list_lambda[v].append(c_ang_s / packet.nu_rf)
                         lists_y[v].append(packet.emission_velocity / 1e5)
                 elif v == "true_emission_velocity":
                     if not np.isnan(packet.true_emission_velocity) and not np.isinf(packet.true_emission_velocity):
                         list_lambda[v].append(c_ang_s / packet.nu_rf)
                         lists_y[v].append(packet.true_emission_velocity / 1e5)
                 else:
-                    k = (packet["em_timestep"], packet["emtrue_modelgridindex"])
+                    k: tuple[int, int] = (packet["em_timestep"], packet["emtrue_modelgridindex"])
                     if k in estimators:
                         list_lambda[v].append(c_ang_s / packet.nu_rf)
                         lists_y[v].append(estimators[k][v])
 
     for ax, yvar in zip(axes, densityplotyvars):
         # ax.set_ylabel(r'velocity [{} km/s]')
-        ax.set_ylabel(yvar + " " + at.estimators.get_units_string(yvar))
+        if not args.hideyticklabels:
+            ax.set_ylabel(yvar + " " + at.estimators.get_units_string(yvar))
         # ax.plot(list_lambda, list_yvar, lw=0, marker='o', markersize=0.5)
         # ax.hexbin(list_lambda[yvar], lists_y[yvar], gridsize=100, cmap=plt.cm.BuGn_r)
         ax.hist2d(list_lambda[yvar], lists_y[yvar], bins=(50, 30), cmap=plt.cm.Greys)  # pylint: disable=no-member
         # plt.cm.Greys
         # x = np.array(list_lambda[yvar])
         # y = np.array(lists_y[yvar])
         # from scipy.stats import kde
         #
         # nbins = 30
         # xi, yi = np.mgrid[x.min():x.max():nbins*1j, y.min():y.max():nbins*1j]
         # zi = k(np.vstack([xi.flatten(), yi.flatten()]))
         # ax.pcolormesh(xi, yi, zi.reshape(xi.shape), shading='gouraud', cmap=plt.cm.BuGn_r)
 
 
-def make_plot(args) -> None:
+def make_plot(args) -> tuple[plt.Figure, plt.Axes, pd.DataFrame]:
     # font = {'size': 16}
     # mpl.rc('font', **font)
 
     densityplotyvars: list[str] = []
     # densityplotyvars = ['emission_velocity', 'Te', 'nne']
     # densityplotyvars = ['true_emission_velocity', 'emission_velocity', 'Te', 'nne']
 
     nrows = len(args.timedayslist) if args.multispecplot else 1 + len(densityplotyvars)
 
+    figwidth = args.figscale * at.get_config()["figwidth"]
+    figheight = args.figscale * at.get_config()["figwidth"] * (0.25 + nrows * 0.4)
+    if args.showabsorption:
+        figheight *= 1.56
+    if args.hidexticklabels:
+        figheight *= 0.87
+
     fig, axes = plt.subplots(
         nrows=nrows,
         ncols=1,
         sharey=False,
         sharex=True,
         squeeze=True,
-        figsize=(
-            args.figscale * at.get_config()["figwidth"],
-            args.figscale * at.get_config()["figwidth"] * (0.25 + nrows * 0.4),
-        ),
+        figsize=(figwidth, figheight),
         tight_layout={"pad": 0.2, "w_pad": 0.0, "h_pad": 0.0},
     )
 
     if nrows == 1:
         axes = [axes]
 
     filterfunc = at.get_filterfunc(args)
 
     scale_to_peak = 1.0 if args.normalised else None
 
     dfalldata = pd.DataFrame()
 
-    if args.multispecplot:
-        for ax in axes:
-            ax.set_ylabel(r"F$_\lambda$ at 1 Mpc [{}erg/s/cm$^2$/$\mathrm{{\AA}}$]")
-
-    elif args.logscale:
-        # don't include the {} that will be replaced with the power of 10 by the custom formatter
-        axes[-1].set_ylabel(r"F$_\lambda$ at 1 Mpc [erg/s/cm$^2$/$\mathrm{{\AA}}$]")
-    else:
-        axes[-1].set_ylabel(r"F$_\lambda$ at 1 Mpc [{}erg/s/cm$^2$/$\mathrm{{\AA}}$]")
+    if not args.hideyticklabels:
+        if args.multispecplot:
+            for ax in axes:
+                ax.set_ylabel(r"F$_\lambda$ at 1 Mpc [{}erg/s/cm$^2$/$\mathrm{{\AA}}$]")
+
+        elif args.logscale:
+            # don't include the {} that will be replaced with the power of 10 by the custom formatter
+            axes[-1].set_ylabel(r"F$_\lambda$ at 1 Mpc [erg/s/cm$^2$/$\mathrm{{\AA}}$]")
+        else:
+            axes[-1].set_ylabel(r"F$_\lambda$ at 1 Mpc [{}erg/s/cm$^2$/$\mathrm{{\AA}}$]")
 
     for axis in axes:
         if args.logscale:
             axis.set_yscale("log")
         axis.set_xlim(left=args.xmin, right=args.xmax)
 
         if (args.xmax - args.xmin) < 2000:
@@ -883,14 +916,17 @@
             axis.xaxis.set_minor_locator(ticker.MultipleLocator(base=10))
         elif (args.xmax - args.xmin) < 11000:
             axis.xaxis.set_major_locator(ticker.MultipleLocator(base=1000))
             axis.xaxis.set_minor_locator(ticker.MultipleLocator(base=100))
         elif (args.xmax - args.xmin) < 14000:
             axis.xaxis.set_major_locator(ticker.MultipleLocator(base=2000))
             axis.xaxis.set_minor_locator(ticker.MultipleLocator(base=500))
+        else:
+            axis.xaxis.set_major_locator(ticker.MultipleLocator(base=2000))
+            axis.xaxis.set_minor_locator(ticker.MultipleLocator(base=500))
 
     if densityplotyvars:
         make_contrib_plot(axes[:-1], args.specpath[0], densityplotyvars, args)
 
     if args.showemission or args.showabsorption:
         legendncol = 2
         if args.internalpackets:
@@ -911,30 +947,30 @@
             dfalldata = make_spectrum_plot(args.specpath, axes, filterfunc, args, scale_to_peak=scale_to_peak)
             plotobjects, plotobjectlabels = axes[0].get_legend_handles_labels()
         else:
             dfalldata = make_spectrum_plot(args.specpath, [axes[-1]], filterfunc, args, scale_to_peak=scale_to_peak)
             plotobjects, plotobjectlabels = axes[-1].get_legend_handles_labels()
 
     if not args.nolegend:
-        if args.reverselegendorder:
+        if args.reverselegendorder:  # TODO: consider ax.legend(reverse=True)
             plotobjects, plotobjectlabels = plotobjects[::-1], plotobjectlabels[::-1]
 
-        fs = 12 if (args.showemission or args.showabsorption) else None
         leg = axes[-1].legend(
             plotobjects,
             plotobjectlabels,
             loc="upper right",
             frameon=False,
-            handlelength=2,
+            handlelength=1 if args.showemission or args.showabsorption else 2,
             ncol=legendncol,
             numpoints=1,
-            fontsize=fs,
+            columnspacing=1.0,
         )
         leg.set_zorder(200)
 
+        # Luke: I don't know what this code is for
         for artist, text in zip(leg.legend_handles, leg.get_texts()):
             if hasattr(artist, "get_color"):
                 col = artist.get_color()
                 artist.set_linewidth(2.0)
                 # artist.set_visible(False)  # hide line next to text
             elif hasattr(artist, "get_facecolor"):
                 col = artist.get_facecolor()
@@ -958,38 +994,36 @@
                 at.plottools.ExponentLabelFormatter(ax.get_ylabel(), useMathText=True, decimalplaces=1)
             )
 
         if args.hidexticklabels:
             ax.tick_params(
                 axis="x",
                 which="both",
-                # bottom=True, top=True,
                 labelbottom=False,
             )
+        if args.hideyticklabels:
+            ax.tick_params(
+                axis="y",
+                which="both",
+                labelleft=False,
+            )
         ax.set_xlabel("")
 
         if args.multispecplot and args.showtime:
             ymin, ymax = ax.get_ylim()
             ax.text(5500, ymax * 0.9, f"{args.timedayslist[index]} days")  # multispecplot text
 
-    axes[-1].set_xlabel(args.xlabel)
+    if not args.hidexticklabels:
+        axes[-1].set_xlabel(args.xlabel)
 
     if not args.outputfile:
         args.outputfile = defaultoutputfile
     elif not Path(args.outputfile).suffixes:
         args.outputfile = args.outputfile / defaultoutputfile
 
-    strdirectionbins = ""
-    if args.plotviewingangle:
-        strdirectionbins = "_direction" + "_".join([f"{angle:02d}" for angle in args.plotviewingangle])
-
-    filenameout = str(args.outputfile).format(
-        time_days_min=args.timemin, time_days_max=args.timemax, directionbins=strdirectionbins
-    )
-
     # plt.text(6000, (args.ymax * 0.9), f'{round(args.timemin) + 1} days', fontsize='large')
 
     if args.showtime and not args.multispecplot:
         if not args.ymax:
             ymin, ymax = ax.get_ylim()
         else:
             ymax = args.ymax
@@ -1000,28 +1034,15 @@
             xy=(0.03, 0.97),
             xycoords="axes fraction",
             horizontalalignment="left",
             verticalalignment="top",
             fontsize="x-large",
         )
 
-    if args.write_data and not dfalldata.empty:
-        print(dfalldata)
-        datafilenameout = Path(filenameout).with_suffix(".txt")
-        dfalldata.to_csv(datafilenameout)
-        print(f"Saved {datafilenameout}")
-
-    # plt.minorticks_on()
-    # plt.tick_params(axis='x', which='minor', length=5, width=2, labelsize=18)
-    # plt.tick_params(axis='both', which='major', length=8, width=2, labelsize=18)
-
-    fig.savefig(filenameout)
-    # plt.show()
-    print(f"Saved {filenameout}")
-    plt.close()
+    return fig, axes, dfalldata
 
 
 def addargs(parser) -> None:
     parser.add_argument(
         "specpath",
         default=[],
         nargs="*",
@@ -1033,14 +1054,16 @@
 
     parser.add_argument("-color", "-colors", dest="color", default=[], nargs="*", help="List of line colors")
 
     parser.add_argument("-linestyle", default=[], nargs="*", help="List of line styles")
 
     parser.add_argument("-linewidth", default=[], nargs="*", help="List of line widths")
 
+    parser.add_argument("-linealpha", default=[], nargs="*", help="List of line alphas (opacities)")
+
     parser.add_argument("-dashes", default=[], nargs="*", help="Dashes property of lines")
 
     parser.add_argument("--greyscale", action="store_true", help="Plot in greyscale")
 
     parser.add_argument(
         "--frompackets", action="store_true", help="Read packets files directly instead of exspec results"
     )
@@ -1177,22 +1200,28 @@
 
     parser.add_argument("--hidenetspectrum", action="store_true", help="Hide net spectrum")
 
     parser.add_argument("--hideother", action="store_true", help="Hide other contributions")
 
     parser.add_argument("--notitle", action="store_true", help="Suppress the top title from the plot")
 
+    parser.add_argument("-title", action="store_true", help="Set the plot title")
+
+    parser.add_argument("--inset_title", action="store_true", help="Place title inside the plot")
+
     parser.add_argument("--nolegend", action="store_true", help="Suppress the legend from the plot")
 
     parser.add_argument("--reverselegendorder", action="store_true", help="Reverse the order of legend items")
 
-    parser.add_argument("--hidexticklabels", action="store_true", help="Dont show numbers on the x axis")
+    parser.add_argument("--hidexticklabels", action="store_true", help="Don't show numbers or a label on the x axis")
 
     parser.add_argument("-xlabel", default=r"Wavelength $\left[\mathrm{{\AA}}\right]$", help="Label for the x axis")
 
+    parser.add_argument("--hideyticklabels", action="store_true", help="Don't show numbers or a label on the y axis")
+
     parser.add_argument("--write_data", action="store_true", help="Save data used to generate the plot in a CSV file")
 
     parser.add_argument(
         "-outputfile", "-o", action="store", dest="outputfile", type=Path, help="path/filename for PDF file"
     )
 
     parser.add_argument(
@@ -1222,15 +1251,21 @@
     )
 
     parser.add_argument(
         "-plotviewingangle",
         type=int,
         metavar="n",
         nargs="+",
-        help="Plot viewing angles. Expects int for angle number in specpol_res.out",
+        help="Plot viewing angles. Expects int for direction bin in specpol_res.out",
+    )
+
+    parser.add_argument(
+        "--usedegrees",
+        action="store_true",
+        help="Use degrees instead of radians for viewing angles. Only works with -plotviewingangle",
     )
 
     parser.add_argument(
         "--average_over_phi_angle",
         action="store_true",
         help="Average over phi (azimuthal) viewing angles to make direction bins into polar angle bins",
     )
@@ -1290,16 +1325,16 @@
     at.set_mpl_style()
 
     assert (
         not args.plotvspecpol or not args.plotviewingangle
     )  # choose either virtual packet directions or real packet direction bins
 
     if not args.specpath:
-        args.specpath = [Path(".")]
-    elif isinstance(args.specpath, (str, Path)):  # or not not isinstance(args.specpath, Iterable)
+        args.specpath = [Path()]
+    elif isinstance(args.specpath, str | Path):  # or not not isinstance(args.specpath, Iterable)
         args.specpath = [args.specpath]
 
     args.specpath = at.flatten_list(args.specpath)
 
     if args.timedayslist:
         args.multispecplot = True
         args.timedays = args.timedayslist[0]
@@ -1314,27 +1349,27 @@
             if Path(filepath).is_dir() or Path(filepath).name.endswith(".out"):
                 args.color.append(artismodelcolors[artismodelnum])
                 artismodelnum += 1
             else:
                 args.color.append(refspeccolors[refspecnum])
                 refspecnum += 1
 
-    args.color, args.label, args.linestyle, args.dashes, args.linewidth = at.trim_or_pad(
-        len(args.specpath), args.color, args.label, args.linestyle, args.dashes, args.linewidth
+    args.color, args.label, args.linestyle, args.linealpha, args.dashes, args.linewidth = at.trim_or_pad(
+        len(args.specpath), args.color, args.label, args.linestyle, args.linealpha, args.dashes, args.linewidth
     )
 
     if args.emissionvelocitycut:
         args.frompackets = True
 
     if args.makevspecpol:
-        make_virtual_spectra_summed_file(args.specpath[0])
+        at.spectra.make_virtual_spectra_summed_file(args.specpath[0])
         return
 
     if args.averagevspecpolfiles:
-        make_averaged_vspecfiles(args)
+        at.spectra.make_averaged_vspecfiles(args)
         return
 
     if "/" in args.stokesparam:
         plot_polarisation(args.specpath[0], args)
         return
 
     if args.output_spectra:
@@ -1342,12 +1377,33 @@
             at.spectra.write_flambda_spectra(modelpath, args)
 
     else:
         if args.emissionabsorption:
             args.showemission = True
             args.showabsorption = True
 
-        make_plot(args)
+        fig, axes, dfalldata = make_plot(args)
+        strdirectionbins = (
+            "_direction" + "_".join([f"{angle:02d}" for angle in args.plotviewingangle])
+            if args.plotviewingangle
+            else ""
+        )
+        filenameout = str(args.outputfile).format(
+            time_days_min=args.timemin, time_days_max=args.timemax, directionbins=strdirectionbins
+        )
+
+        if args.write_data and not dfalldata.empty:
+            print(dfalldata)
+            datafilenameout = Path(filenameout).with_suffix(".txt")
+            dfalldata.to_csv(datafilenameout)
+            print(f"Saved {datafilenameout}")
+
+        # plt.minorticks_on()
+
+        fig.savefig(filenameout)
+        # plt.show()
+        print(f"Saved {filenameout}")
+        plt.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `artistools-2023.5.16.3/artistools/spectra/sampleblackbodyfrompacketTR.py` & `artistools-2023.8.1/artistools/spectra/sampleblackbodyfrompacketTR.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 DAY = 86400
 TWOHOVERCLIGHTSQUARED = 1.4745007e-47
 HOVERKB = 4.799243681748932e-11
 PARSEC = 3.086e18
 c_cgs = const.c.to("cm/s").value
 c_ang_s = const.c.to("angstrom/s").value
 
-modelpath = Path(".")
+modelpath = Path()
 
 xmin = 2500  # Angstroms
 xmax = 30000
 n_nu_bins = 500  # number of frequency bins
 delta_lambda = xmax - xmin
 
 nu_lower = const.c.to("angstrom/s").value / xmin
@@ -69,16 +69,16 @@
     return 0.0
 
 
 # with open(modelpath / 'specpol_res.out', 'r') as specpol_res_file:  # get timesteps
 #     time_list = [float(x) for x in specpol_res_file.readline().split()]
 #
 # column_names = time_list[:int(len(time_list)/3)+1]
-arr_tstart = at.get_timestep_times_float(modelpath, loc="start")
-arr_tend = at.get_timestep_times_float(modelpath, loc="end")
+arr_tstart = at.get_timestep_times(modelpath, loc="start")
+arr_tend = at.get_timestep_times(modelpath, loc="end")
 column_names = np.append(arr_tstart, arr_tend[-1])
 column_names = np.insert(column_names, 0, 0.0, axis=0)
 
 timemin_seconds = column_names[1] * u.day.to("s")
 timemax_seconds = arr_tend[-1] * u.day.to("s")
 
 specpol_data_bb = {column_names[0]: arr_min_nu_hz}
@@ -90,15 +90,15 @@
 specpol_res_data_bb = [copy.deepcopy(specpol_data_bb) for _ in range(n_angle_bins)]
 # need deep copy to make new empty array of same size
 
 
 packetsfiles = at.packets.get_packetsfilepaths(modelpath)
 nprocs = at.get_nprocs(modelpath)
 # nprocs = 100
-for npacketfile in range(0, nprocs):
+for npacketfile in range(nprocs):
     dfpackets = at.packets.readfile(packetsfiles[npacketfile])  # , type='TYPE_ESCAPE', escape_type='TYPE_RPKT')
     dfpackets = at.packets.bin_packet_directions(modelpath, dfpackets)
     dfpackets = dfpackets.query(f'type_id == {type_ids["TYPE_ESCAPE"]} and escape_type_id == {type_ids["TYPE_RPKT"]}')
 
     # print(max(dfpackets['t_arrive_d']))
     # print(dfpackets)
```

### Comparing `artistools-2023.5.16.3/artistools/spectra/spectra.py` & `artistools-2023.8.1/artistools/spectra/spectra.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 """Artistools - spectra related functions."""
+from __future__ import annotations
+
 import argparse
 import math
 import os
 import re
+import typing as t
 from collections import namedtuple
-from collections.abc import Collection
-from collections.abc import Sequence
 from functools import lru_cache
 from pathlib import Path
-from typing import Any
-from typing import Callable
-from typing import Literal
-from typing import Optional
-from typing import Union
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
+import numpy.typing as npt
 import pandas as pd
 import polars as pl
 from astropy import constants as const
 from astropy import units as u
+from typeguard import typechecked
 
 import artistools as at
 
 fluxcontributiontuple = namedtuple(
     "fluxcontributiontuple", "fluxcontrib linelabel array_flambda_emission array_flambda_absorption color"
 )
 
 
-def timeshift_fluxscale_co56law(scaletoreftime: Optional[float], spectime: float) -> float:
+def timeshift_fluxscale_co56law(scaletoreftime: float | None, spectime: float) -> float:
     if scaletoreftime is not None:
         # Co56 decay flux scaling
         assert spectime > 150
         return math.exp(float(spectime) / 113.7) / math.exp(scaletoreftime / 113.7)
 
     return 1.0
 
@@ -62,76 +60,73 @@
     array_lambda = c_ang_s / np.flip(bins_nu_centre)
     delta_lambda = np.flip(c_ang_s / bins_nu_lower - c_ang_s / bins_nu_upper)
 
     return array_lambdabinedges, array_lambda, delta_lambda
 
 
 def stackspectra(
-    spectra_and_factors: list[tuple[np.ndarray[Any, np.dtype[np.float64]], float]]
-) -> np.ndarray[Any, np.dtype[np.float64]]:
+    spectra_and_factors: list[tuple[np.ndarray[t.Any, np.dtype[np.float64]], float]]
+) -> np.ndarray[t.Any, np.dtype[np.float64]]:
     """Add spectra using weighting factors, i.e., specout[nu] = spec1[nu] * factor1 + spec2[nu] * factor2 + ...
     spectra_and_factors should be a list of tuples: spectra[], factor.
     """
-    factor_sum = sum([factor for _, factor in spectra_and_factors])
+    factor_sum = sum(factor for _, factor in spectra_and_factors)
 
     stackedspectrum = np.zeros_like(spectra_and_factors[0][0], dtype=float)
     for spectrum, factor in spectra_and_factors:
         stackedspectrum += spectrum * factor / factor_sum
 
     return stackedspectrum
 
 
 def get_spectrum_at_time(
     modelpath: Path,
     timestep: int,
     time: float,
-    args: Optional[argparse.Namespace],
+    args: argparse.Namespace | None,
     dirbin: int = -1,
-    average_over_phi: Optional[bool] = None,
-    average_over_theta: Optional[bool] = None,
+    average_over_phi: bool | None = None,
+    average_over_theta: bool | None = None,
 ) -> pd.DataFrame:
     if dirbin >= 0:
-        if args is not None and args.plotvspecpol and os.path.isfile(modelpath / "vpkt.txt"):
-            spectrum = get_vspecpol_spectrum(modelpath, time, dirbin, args)
-            return spectrum
-
+        if args is not None and args.plotvspecpol and (modelpath / "vpkt.txt").is_file():
+            return get_vspecpol_spectrum(modelpath, time, dirbin, args)
         assert average_over_phi is not None
         assert average_over_theta is not None
     else:
         average_over_phi = False
         average_over_theta = False
 
-    spectrum = get_spectrum(
+    return get_spectrum(
         modelpath=modelpath,
         directionbins=[dirbin],
         timestepmin=timestep,
         timestepmax=timestep,
         average_over_phi=average_over_phi,
         average_over_theta=average_over_theta,
     )[dirbin]
 
-    return spectrum
-
 
+@typechecked
 def get_from_packets(
     modelpath: Path,
     timelowdays: float,
     timehighdays: float,
     lambda_min: float,
     lambda_max: float,
-    delta_lambda: Union[None, float, np.ndarray] = None,
+    delta_lambda: None | float | np.ndarray = None,
     use_escapetime: bool = False,
-    maxpacketfiles: Optional[int] = None,
+    maxpacketfiles: int | None = None,
     useinternalpackets: bool = False,
     getpacketcount: bool = False,
-    directionbins: Optional[Collection[int]] = None,
+    directionbins: t.Collection[int] | None = None,
     average_over_phi: bool = False,
     average_over_theta: bool = False,
-    fnufilterfunc: Optional[Callable[[np.ndarray], np.ndarray]] = None,
-) -> pd.DataFrame:
+    fnufilterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
+) -> dict[int, pd.DataFrame]:
     """Get a spectrum dataframe using the packets files as input."""
     assert not useinternalpackets
     if directionbins is None:
         directionbins = [-1]
 
     if use_escapetime:
         modeldata, _ = at.inputmodel.get_modeldata(modelpath)
@@ -183,14 +178,15 @@
         elif average_over_theta:
             getcols.append("phibin")
         else:
             getcols.append("dirbin")
     dfpackets = dfpackets.select(getcols).collect().lazy()
 
     dfdict = {}
+    megaparsec_to_cm = 3.085677581491367e24
     for dirbin in directionbins:
         if dirbin == -1:
             solidanglefactor = 1.0
             pldfpackets_dirbin_lazy = dfpackets
         elif average_over_phi:
             assert not average_over_theta
             solidanglefactor = ncosthetabins
@@ -210,22 +206,22 @@
             pldfpackets_dirbin,
             bincol="lambda_angstroms",
             bins=list(array_lambdabinedges),
             sumcols=[encol],
             getcounts=getpacketcount,
         )
         array_flambda = (
-            dfbinned[encol + "_sum"]
+            dfbinned[f"{encol}_sum"]
             / delta_lambda
             / (timehigh - timelow)
             / (4 * math.pi)
             * solidanglefactor
-            / (u.megaparsec.to("cm") ** 2)
+            / (megaparsec_to_cm**2)
             / nprocs_read
-        )
+        ).to_numpy()
 
         if use_escapetime:
             assert escapesurfacegamma is not None
             array_flambda /= escapesurfacegamma
 
         if fnufilterfunc:
             arr_nu = 2.99792458e18 / array_lambda
@@ -243,32 +239,34 @@
         if getpacketcount:
             dfdict[dirbin]["packetcount"] = dfbinned["count"]
 
     return dfdict
 
 
 @lru_cache(maxsize=16)
-def read_spec_res(modelpath: Path) -> dict[int, pd.DataFrame]:
-    """Return dataframe of time-series spectra for every viewing direction."""
+def read_spec_res(modelpath: Path) -> dict[int, pl.DataFrame]:
+    """Return a dataframe of time-series spectra for every viewing direction."""
     specfilename = (
         modelpath
         if Path(modelpath).is_file()
         else at.firstexisting(["spec_res.out", "specpol_res.out"], folder=modelpath, tryzipped=True)
     )
 
     print(f"Reading {specfilename} (in read_spec_res)")
     res_specdata_in = pl.read_csv(at.zopen(specfilename, "rb"), separator=" ", has_header=False, infer_schema_length=0)
 
     # drop last column of nulls (caused by trailing space on each line)
     if res_specdata_in[res_specdata_in.columns[-1]].is_null().all():
         res_specdata_in = res_specdata_in.drop(res_specdata_in.columns[-1])
 
-    res_specdata: dict[int, pl.DataFrame] = at.split_dataframe_dirbins(res_specdata_in, output_polarsdf=True)
+    res_specdata = at.split_dataframe_dirbins(res_specdata_in, output_polarsdf=True)
+
     prev_dfshape = None
     for dirbin in res_specdata:
+        assert isinstance(res_specdata[dirbin], pl.DataFrame)
         newcolnames = [str(x) for x in res_specdata[dirbin][0, :].to_numpy()[0]]
         newcolnames[0] = "nu"
 
         newcolnames_unique = set(newcolnames)
         oldcolnames = res_specdata[dirbin].columns
         if len(newcolnames) > len(newcolnames_unique):
             # for POL_ON, the time columns repeat for Q, U, and V stokes params.
@@ -288,15 +286,15 @@
         assert prev_dfshape is None or prev_dfshape == res_specdata[dirbin].shape
         prev_dfshape = res_specdata[dirbin].shape
 
     return res_specdata
 
 
 @lru_cache(maxsize=200)
-def read_emission_absorption_file(emabsfilename: Union[str, Path]) -> pl.DataFrame:
+def read_emission_absorption_file(emabsfilename: str | Path) -> pl.DataFrame:
     """Read into a DataFrame one of: emission.out. emissionpol.out, emissiontrue.out, absorption.out."""
     try:
         emissionfilesize = Path(emabsfilename).stat().st_size / 1024 / 1024
         print(f" Reading {emabsfilename} ({emissionfilesize:.2f} MiB)")
 
     except AttributeError:
         print(f" Reading {emabsfilename}")
@@ -313,33 +311,34 @@
 
 
 @lru_cache(maxsize=4)
 def get_spec_res(
     modelpath: Path,
     average_over_theta: bool = False,
     average_over_phi: bool = False,
-) -> dict[int, pd.DataFrame]:
+) -> dict[int, pl.DataFrame]:
     res_specdata = read_spec_res(modelpath)
     if average_over_theta:
         res_specdata = at.average_direction_bins(res_specdata, overangle="theta")
     if average_over_phi:
         res_specdata = at.average_direction_bins(res_specdata, overangle="phi")
 
     return res_specdata
 
 
+@typechecked
 def get_spectrum(
     modelpath: Path,
     timestepmin: int,
-    timestepmax: Optional[int] = None,
-    directionbins: Optional[Sequence[int]] = None,
-    fnufilterfunc: Optional[Callable[[np.ndarray], np.ndarray]] = None,
+    timestepmax: int | None = None,
+    directionbins: t.Sequence[int] | None = None,
+    fnufilterfunc: t.Callable[[npt.NDArray[np.floating]], npt.NDArray[np.floating]] | None = None,
     average_over_theta: bool = False,
     average_over_phi: bool = False,
-    stokesparam: Literal["I", "Q", "U"] = "I",
+    stokesparam: t.Literal["I", "Q", "U"] = "I",
 ) -> dict[int, pd.DataFrame]:
     """Return a pandas DataFrame containing an ARTIS emergent spectrum."""
     if timestepmax is None or timestepmax < 0:
         timestepmax = timestepmin
 
     if directionbins is None:
         directionbins = [-1]
@@ -354,32 +353,35 @@
 
                 print(f"Reading {specfilename}")
 
                 specdata[-1] = (
                     pl.read_csv(at.zopen(specfilename, mode="rb"), separator=" ", infer_schema_length=0)
                     .with_columns(pl.all().cast(pl.Float64))
                     .rename({"0": "nu"})
+                    .to_pandas()
                 )
 
             except FileNotFoundError:
                 specdata[-1] = get_specpol_data(angle=-1, modelpath=modelpath)[stokesparam]
 
         else:
             specdata[-1] = get_specpol_data(angle=-1, modelpath=modelpath)[stokesparam]
 
     if any(dirbin != -1 for dirbin in directionbins):
         assert stokesparam == "I"
-        specdata.update(
-            get_spec_res(modelpath=modelpath, average_over_theta=average_over_theta, average_over_phi=average_over_phi)
+        specdata |= get_spec_res(
+            modelpath=modelpath,
+            average_over_theta=average_over_theta,
+            average_over_phi=average_over_phi,
         )
 
     specdataout: dict[int, pd.DataFrame] = {}
     for dirbin in directionbins:
         arr_nu = specdata[dirbin]["nu"].to_numpy()
-        arr_tdelta = at.get_timestep_times_float(modelpath, loc="delta")
+        arr_tdelta = at.get_timestep_times(modelpath, loc="delta")
 
         arr_f_nu = stackspectra(
             [
                 (specdata[dirbin][specdata[dirbin].columns[timestep + 1]].to_numpy(), arr_tdelta[timestep])
                 for timestep in range(timestepmin, timestepmax + 1)
             ]
         )
@@ -426,15 +428,15 @@
 
         vspecpolfile = pd.read_csv(vspecpolpath, delim_whitespace=True, header=None)
         # Where times of timesteps are written out a new virtual spectrum starts
         # Find where the time in row 0, column 1 repeats in any column 1
         index_of_new_spectrum = vspecpolfile.index[vspecpolfile.iloc[:, 1] == vspecpolfile.iloc[0, 1]]
         vspecpol_data = []  # list of all predefined vspectra
         for i, index_spectrum_starts in enumerate(index_of_new_spectrum[:nvirtual_spectra]):
-            # todo: this is different to at.split_dataframe_dirbins() -- could be made to be same format to not repeat code
+            # TODO: this is different to at.split_dataframe_dirbins() -- could be made to be same format to not repeat code
             chunk = (
                 vspecpolfile.iloc[index_spectrum_starts : index_of_new_spectrum[i + 1], :]
                 if index_spectrum_starts != index_of_new_spectrum[-1]
                 else vspecpolfile.iloc[index_spectrum_starts:, :]
             )
             vspecpol_data.append(chunk)
 
@@ -460,60 +462,58 @@
 def make_averaged_vspecfiles(args: argparse.Namespace) -> None:
     filenames = []
     for vspecfile in os.listdir(args.modelpath[0]):
         if vspecfile.startswith("vspecpol_total-"):
             filenames.append(vspecfile)
 
     def sorted_by_number(l: list) -> list:
-        def convert(text: str) -> Union[int, str]:
+        def convert(text: str) -> int | str:
             return int(text) if text.isdigit() else text
 
-        def alphanum_key(key: str) -> list[Union[int, str]]:
+        def alphanum_key(key: str) -> list[int | str]:
             return [convert(c) for c in re.split("([0-9]+)", key)]
 
         return sorted(l, key=alphanum_key)
 
     filenames = sorted_by_number(filenames)
 
     for spec_index, filename in enumerate(filenames):  # vspecpol-total files
-        vspecdata = []
-        for modelpath in args.modelpath:
-            vspecdata.append(pd.read_csv(modelpath / filename, delim_whitespace=True, header=None))
+        vspecdata = [
+            pd.read_csv(modelpath / filename, delim_whitespace=True, header=None) for modelpath in args.modelpath
+        ]
         for i in range(1, len(vspecdata)):
             vspecdata[0].iloc[1:, 1:] += vspecdata[i].iloc[1:, 1:]
 
         vspecdata[0].iloc[1:, 1:] = vspecdata[0].iloc[1:, 1:] / len(vspecdata)
         vspecdata[0].to_csv(
             args.modelpath[0] / f"vspecpol_averaged-{spec_index}.out", sep=" ", index=False, header=False
         )
 
 
 @lru_cache(maxsize=4)
 def get_specpol_data(
-    angle: int = -1, modelpath: Optional[Path] = None, specdata: Optional[pd.DataFrame] = None
+    angle: int = -1, modelpath: Path | None = None, specdata: pd.DataFrame | None = None
 ) -> dict[str, pd.DataFrame]:
     if specdata is None:
         assert modelpath is not None
         specfilename = (
             at.firstexisting("specpol.out", folder=modelpath, tryzipped=True)
             if angle == -1
             else at.firstexisting(f"specpol_res_{angle}.out", folder=modelpath, tryzipped=True)
         )
 
         print(f"Reading {specfilename}")
         specdata = pd.read_csv(specfilename, delim_whitespace=True)
 
-    stokes_params = split_dataframe_stokesparams(specdata)
-
-    return stokes_params
+    return split_dataframe_stokesparams(specdata)
 
 
 @lru_cache(maxsize=4)
 def get_vspecpol_data(
-    vspecangle: Optional[int] = None, modelpath: Optional[Path] = None, specdata: Optional[pd.DataFrame] = None
+    vspecangle: int | None = None, modelpath: Path | None = None, specdata: pd.DataFrame | None = None
 ) -> dict[str, pd.DataFrame]:
     if specdata is None:
         assert modelpath is not None
         # alternatively use f'vspecpol_averaged-{angle}.out' ?
         vspecpath = modelpath
         if (modelpath / "vspecpol").is_dir():
             vspecpath = modelpath / "vspecpol"
@@ -523,65 +523,64 @@
         except FileNotFoundError:
             print(f"vspecpol_total-{vspecangle}.out does not exist. Generating all-rank summed vspec files..")
             specfilename = make_virtual_spectra_summed_file(modelpath=modelpath)
 
         print(f"Reading {specfilename}")
         specdata = pd.read_csv(specfilename, delim_whitespace=True)
 
-    stokes_params = split_dataframe_stokesparams(specdata)
-
-    return stokes_params
+    return split_dataframe_stokesparams(specdata)
 
 
 def split_dataframe_stokesparams(specdata: pd.DataFrame) -> dict[str, pd.DataFrame]:
     """DataFrames read from specpol*.out and vspecpol*.out are repeated over I, Q, U
     parameters. Split these into a dictionary of DataFrames.
     """
     specdata = specdata.rename({"0": "nu", "0.0": "nu"}, axis="columns")
-    cols_to_split = []
-    stokes_params = {}
-    for i, key in enumerate(specdata.keys()):
-        if specdata.keys()[1] in key:
-            cols_to_split.append(i)
-
-    stokes_params["I"] = pd.concat(
-        [specdata["nu"], specdata.iloc[:, cols_to_split[0] : cols_to_split[1]]], axis="columns"
-    )
+    cols_to_split = [i for i, key in enumerate(specdata.keys()) if specdata.keys()[1] in key]
+    stokes_params = {
+        "I": pd.concat(
+            [
+                specdata["nu"],
+                specdata.iloc[:, cols_to_split[0] : cols_to_split[1]],
+            ],
+            axis="columns",
+        )
+    }
     stokes_params["Q"] = pd.concat(
         [specdata["nu"], specdata.iloc[:, cols_to_split[1] : cols_to_split[2]]], axis="columns"
     )
     stokes_params["U"] = pd.concat([specdata["nu"], specdata.iloc[:, cols_to_split[2] :]], axis="columns")
 
     for param in ["Q", "U"]:
         stokes_params[param].columns = stokes_params["I"].keys()
         stokes_params[param + "/I"] = pd.concat(
             [specdata["nu"], stokes_params[param].iloc[:, 1:] / stokes_params["I"].iloc[:, 1:]], axis="columns"
         )
     return stokes_params
 
 
 def get_vspecpol_spectrum(
-    modelpath: Union[Path, str],
+    modelpath: Path | str,
     timeavg: float,
     angle: int,
     args: argparse.Namespace,
-    fnufilterfunc: Optional[Callable[[np.ndarray], np.ndarray]] = None,
+    fnufilterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
 ) -> pd.DataFrame:
     stokes_params = get_vspecpol_data(vspecangle=angle, modelpath=Path(modelpath))
     if "stokesparam" not in args:
         args.stokesparam = "I"
     vspecdata = stokes_params[args.stokesparam]
 
     nu = vspecdata.loc[:, "nu"].to_numpy()
 
     arr_tmid = [float(i) for i in vspecdata.columns.to_numpy()[1:] if i[-2] != "."]
     arr_tdelta = [l1 - l2 for l1, l2 in zip(arr_tmid[1:], arr_tmid[:-1])] + [arr_tmid[-1] - arr_tmid[-2]]
 
     def match_closest_time(reftime: float) -> str:
-        return str(f"{min([float(x) for x in arr_tmid], key=lambda x: abs(x - reftime))}")
+        return str(f"{min((float(x) for x in arr_tmid), key=lambda x: abs(x - reftime))}")
 
     # if 'timemin' and 'timemax' in args:
     #     timelower = match_closest_time(args.timemin)  # how timemin, timemax are used changed at some point
     #     timeupper = match_closest_time(args.timemax)  # to average over multiple timesteps needs to fix this
     # else:
     timelower = match_closest_time(timeavg)
     timeupper = match_closest_time(timeavg)
@@ -601,34 +600,32 @@
         print("Applying filter to ARTIS spectrum")
         f_nu = fnufilterfunc(f_nu)
 
     dfspectrum = pd.DataFrame({"nu": nu, "f_nu": f_nu})
     dfspectrum = dfspectrum.sort_values(by="nu", ascending=False)
 
     dfspectrum = dfspectrum.eval("lambda_angstroms = @c / nu", local_dict={"c": 2.99792458e18})
-    dfspectrum = dfspectrum.eval("f_lambda = f_nu * nu / lambda_angstroms")
-
-    return dfspectrum
+    return dfspectrum.eval("f_lambda = f_nu * nu / lambda_angstroms")
 
 
 @lru_cache(maxsize=4)
 def get_flux_contributions(
     modelpath: Path,
-    filterfunc: Optional[Callable[[np.ndarray], np.ndarray]] = None,
+    filterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
     timestepmin: int = -1,
     timestepmax: int = -1,
     getemission: bool = True,
     getabsorption: bool = True,
     use_lastemissiontype: bool = True,
-    directionbin: Optional[int] = None,
+    directionbin: int | None = None,
     averageoverphi: bool = False,
     averageovertheta: bool = False,
-) -> tuple[list[fluxcontributiontuple], np.ndarray]:
-    arr_tmid = at.get_timestep_times_float(modelpath, loc="mid")
-    arr_tdelta = at.get_timestep_times_float(modelpath, loc="delta")
+) -> tuple[list[fluxcontributiontuple], npt.NDArray[np.float64]]:
+    arr_tmid = at.get_timestep_times(modelpath, loc="mid")
+    arr_tdelta = at.get_timestep_times(modelpath, loc="delta")
     arraynu = at.get_nu_grid(modelpath)
     arraylambda = 2.99792458e18 / arraynu
     if not Path(modelpath, "compositiondata.txt").is_file():
         print("WARNING: compositiondata.txt not found. Using output*.txt instead")
         elementlist = at.get_composition_data_from_outputfile(modelpath)
     else:
         elementlist = at.get_composition_data(modelpath)
@@ -645,15 +642,15 @@
         assert directionbin < at.get_viewingdirection_phibincount()
         dbinlist = list(range(directionbin, at.get_viewingdirectionbincount(), at.get_viewingdirection_phibincount()))
     else:
         dbinlist = [directionbin]
 
     emissiondata: dict[int, pd.DataFrame] = {}
     absorptiondata: dict[int, pd.DataFrame] = {}
-    maxion: Optional[int] = None
+    maxion: int | None = None
     for dbin in dbinlist:
         if getemission:
             emissionfilenames = ["emission.out", "emissionpol.out"] if use_lastemissiontype else ["emissiontrue.out"]
 
             if dbin != -1:
                 emissionfilenames = [x.replace(".out", f"_res_{dbin:02d}.out") for x in emissionfilenames]
 
@@ -788,25 +785,25 @@
 @lru_cache(maxsize=4)
 def get_flux_contributions_from_packets(
     modelpath: Path,
     timelowerdays: float,
     timeupperdays: float,
     lambda_min: float,
     lambda_max: float,
-    delta_lambda: Union[None, float, np.ndarray] = None,
+    delta_lambda: None | float | np.ndarray = None,
     getemission: bool = True,
     getabsorption: bool = True,
-    maxpacketfiles: Optional[int] = None,
-    filterfunc: Optional[Callable[[np.ndarray], np.ndarray]] = None,
-    groupby: Optional[Literal["ion", "line", "upperterm", "terms"]] = "ion",
-    modelgridindex: Optional[int] = None,
+    maxpacketfiles: int | None = None,
+    filterfunc: t.Callable[[np.ndarray], np.ndarray] | None = None,
+    groupby: t.Literal["ion", "line", "upperterm", "terms"] | None = "ion",
+    modelgridindex: int | None = None,
     use_escapetime: bool = False,
     use_lastemissiontype: bool = True,
     useinternalpackets: bool = False,
-    emissionvelocitycut: Optional[float] = None,
+    emissionvelocitycut: float | None = None,
 ) -> tuple[list[fluxcontributiontuple], np.ndarray, np.ndarray]:
     assert groupby in [None, "ion", "line", "upperterm", "terms"]
 
     if groupby in ["terms", "upperterm"]:
         adata = at.atomic.get_levels(modelpath)
 
     def get_emprocesslabel(
@@ -871,17 +868,15 @@
                     f"{at.get_ionstring(line.atomic_number, line.ionstage)} "
                     f"λ{line.lambda_angstroms:.0f} "
                     f"({line.upperlevelindex}-{line.lowerlevelindex})"
                 )
             return f"{at.get_ionstring(line.atomic_number, line.ionstage)} bound-bound"
         if abstype == -1:
             return "free-free"
-        if abstype == -2:
-            return "bound-free"
-        return "? other absorp."
+        return "bound-free" if abstype == -2 else "? other absorp."
 
     array_lambdabinedges: np.ndarray
     if delta_lambda is not None:
         array_lambdabinedges = np.arange(lambda_min, lambda_max + delta_lambda, delta_lambda)
         array_lambda = 0.5 * (array_lambdabinedges[:-1] + array_lambdabinedges[1:])  # bin centres
     else:
         array_lambdabinedges, array_lambda, delta_lambda = get_exspec_bins()
@@ -910,15 +905,15 @@
     emtypecolumn = (
         "emissiontype" if useinternalpackets else "emissiontype" if use_lastemissiontype else "trueemissiontype"
     )
 
     for _index, packetsfile in enumerate(packetsfiles):
         if useinternalpackets:
             # if we're using packets*.out files, these packets are from the last timestep
-            t_seconds = at.get_timestep_times_float(modelpath, loc="start")[-1] * 86400.0
+            t_seconds = at.get_timestep_times(modelpath, loc="start")[-1] * 86400.0
 
             if modelgridindex is not None:
                 v_inner = at.inputmodel.get_modeldata_tuple(modelpath)[0]["velocity_inner"].iloc[modelgridindex] * 1e5
                 v_outer = at.inputmodel.get_modeldata_tuple(modelpath)[0]["velocity_outer"].iloc[modelgridindex] * 1e5
             else:
                 v_inner = 0.0
                 v_outer = at.inputmodel.get_modeldata_tuple(modelpath)[0]["velocity_outer"].iloc[-1] * 1e5
@@ -937,17 +932,17 @@
                 dfpackets = dfpackets.query("where in @assoc_cells[@modelgridindex]")
             print(f"  {len(dfpackets)} internal r-packets matching frequency range")
         else:
             dfpackets = at.packets.readfile(packetsfile, packet_type="TYPE_ESCAPE", escape_type="TYPE_RPKT")
             dfpackets = dfpackets.query(
                 "@nu_min <= nu_rf < @nu_max and trueemissiontype >= 0 and "
                 + (
-                    "@timelow < (escape_time - (posx * dirx + posy * diry + posz * dirz) / @c_cgs) < @timehigh"
-                    if not use_escapetime
-                    else "@timelow < escape_time * @betafactor < @timehigh"
+                    "@timelow < escape_time * @betafactor < @timehigh"
+                    if use_escapetime
+                    else "@timelow < (escape_time - (posx * dirx + posy * diry + posz * dirz) / @c_cgs) < @timehigh"
                 ),
             )
             print(f"  {len(dfpackets)} escaped r-packets matching frequency and arrival time ranges")
 
             if emissionvelocitycut:
                 dfpackets = at.packets.add_derived_columns(dfpackets, modelpath, ["emission_velocity"])
 
@@ -1015,17 +1010,16 @@
             assoc_cells, mgi_of_propcells = at.get_grid_mapping(modelpath=modelpath)
             volume = (
                 at.get_wid_init_at_tmin(modelpath) * t_seconds / (at.get_inputparams(modelpath)["tmin"] * 86400.0)
             ) ** 3 * len(assoc_cells[modelgridindex])
             print("volume", volume, "shell volume", volume_shells, "-------------------------------------------------")
         normfactor = c_cgs / 4 / math.pi / delta_lambda / volume / nprocs_read
     else:
-        normfactor = (
-            1.0 / delta_lambda / (timehigh - timelow) / 4 / math.pi / (u.megaparsec.to("cm") ** 2) / nprocs_read
-        )
+        megaparsec_to_cm = 3.085677581491367e24
+        normfactor = 1.0 / delta_lambda / (timehigh - timelow) / 4 / math.pi / (megaparsec_to_cm**2) / nprocs_read
 
     array_flambda_emission_total = energysum_spectrum_emission_total * normfactor
 
     contribution_list = []
     for groupname, (energysum_spec_emission, energysum_spec_absorption) in array_energysum_spectra.items():
         array_flambda_emission = energysum_spec_emission * normfactor
 
@@ -1050,15 +1044,15 @@
     return contribution_list, array_flambda_emission_total, array_lambda
 
 
 def sort_and_reduce_flux_contribution_list(
     contribution_list_in: list[fluxcontributiontuple],
     maxseriescount: int,
     arraylambda_angstroms: np.ndarray,
-    fixedionlist: Optional[list[str]] = None,
+    fixedionlist: list[str] | None = None,
     hideother: bool = False,
     greyscale: bool = False,
 ) -> list[fluxcontributiontuple]:
     if fixedionlist:
         unrecognised_items = [x for x in fixedionlist if x not in [y.linelabel for y in contribution_list_in]]
         if unrecognised_items:
             print(f"WARNING: did not understand these items in fixedionlist: {unrecognised_items}")
@@ -1152,61 +1146,38 @@
 
     return contribution_list_out
 
 
 def print_integrated_flux(
     arr_f_lambda: np.ndarray, arr_lambda_angstroms: np.ndarray, distance_megaparsec: float = 1.0
 ) -> float:
-    integrated_flux = abs(np.trapz(arr_f_lambda, x=arr_lambda_angstroms)) * u.erg / u.s / (u.cm**2)
+    integrated_flux = (
+        abs(np.trapz(np.nan_to_num(arr_f_lambda, nan=0.0), x=arr_lambda_angstroms)) * u.erg / u.s / (u.cm**2)
+    )
     print(
         f" integrated flux ({arr_lambda_angstroms.min():.1f} to "
         f"{arr_lambda_angstroms.max():.1f} A): {integrated_flux:.3e}"
     )
     # luminosity = integrated_flux * 4 * math.pi * (distance_megaparsec * u.megaparsec ** 2)
     # print(f'(L={luminosity.to("Lsun"):.3e})')
     return integrated_flux
 
 
-def get_line_flux(
-    lambda_low: float, lambda_high: float, arr_f_lambda: np.ndarray, arr_lambda_angstroms: np.ndarray
-) -> float:
-    index_low, index_high = (
-        int(np.searchsorted(arr_lambda_angstroms, wl, side="left")) for wl in (lambda_low, lambda_high)
-    )
-    flux_integral = abs(np.trapz(arr_f_lambda[index_low:index_high], x=arr_lambda_angstroms[index_low:index_high]))
-    return flux_integral
-
-
-def print_floers_line_ratio(
-    modelpath: Path, timedays: float, arr_f_lambda: np.ndarray, arr_lambda_angstroms: np.ndarray
-) -> None:
-    f_12570 = get_line_flux(12570 - 200, 12570 + 200, arr_f_lambda, arr_lambda_angstroms)
-    f_7155 = get_line_flux(7000, 7350, arr_f_lambda, arr_lambda_angstroms)
-    print(f"f_12570 {f_12570:.2e} f_7155 {f_7155:.2e}")
-    if f_7155 > 0 and f_12570 > 0:
-        fratio = f_12570 / f_7155
-        print(f"f_12570/f_7122 = {fratio:.2e} (log10 is {math.log10(fratio):.2e})")
-        outfilename = f"fe2_nir_vis_ratio_{os.path.basename(modelpath)}.txt"
-        print(f" saved to {outfilename}")
-        with open(outfilename, "a+") as f:
-            f.write(f"{timedays:.1f} {fratio:.3e}\n")
-
-
-def get_reference_spectrum(filename: Union[Path, str]) -> tuple[pd.DataFrame, dict[str, Any]]:
+def get_reference_spectrum(filename: Path | str) -> tuple[pd.DataFrame, dict[str, t.Any]]:
     if Path(filename).is_file():
         filepath = Path(filename)
     else:
         filepath = Path(at.get_config()["path_artistools_dir"], "data", "refspectra", filename)
 
         if not filepath.is_file():
-            filepathxz = filepath.with_suffix(filepath.suffix + ".xz")
+            filepathxz = filepath.with_suffix(f"{filepath.suffix}.xz")
             if filepathxz.is_file():
                 filepath = filepathxz
             else:
-                filepathgz = filepath.with_suffix(filepath.suffix + ".gz")
+                filepathgz = filepath.with_suffix(f"{filepath.suffix}.gz")
                 if filepathgz.is_file():
                     filepath = filepathgz
 
     metadata = at.get_file_metadata(filepath)
 
     flambdaindex = metadata.get("f_lambda_columnindex", 1)
 
@@ -1286,31 +1257,31 @@
     if not args.timestep:
         args.timestep = f"0-{number_of_timesteps - 1}"
 
     (timestepmin, timestepmax, args.timemin, args.timemax) = at.get_time_range(
         modelpath, args.timestep, args.timemin, args.timemax, args.timedays
     )
 
-    with open(outdirectory / "spectra_list.txt", "w+") as spectra_list:
-        arr_tmid = at.get_timestep_times_float(modelpath, loc="mid")
+    with (outdirectory / "spectra_list.txt").open("w+") as spectra_list:
+        arr_tmid = at.get_timestep_times(modelpath, loc="mid")
 
         for timestep in range(timestepmin, timestepmax + 1):
             dfspectrum = get_spectrum(modelpath=modelpath, timestepmin=timestep, timestepmax=timestep)[-1]
             tmid = arr_tmid[timestep]
 
             outfilepath = outdirectory / f"spectrum_ts{timestep:02.0f}_{tmid:.2f}d.txt"
 
-            with open(outfilepath, "w") as spec_file:
+            with outfilepath.open("w") as spec_file:
                 spec_file.write("#lambda f_lambda_1Mpc\n")
                 spec_file.write("#[A] [erg/s/cm2/A]\n")
 
                 dfspectrum.to_csv(
                     spec_file, header=False, sep=" ", index=False, columns=["lambda_angstroms", "f_lambda"]
                 )
 
             spectra_list.write(str(outfilepath.absolute()) + "\n")
 
-    with open(outdirectory / "time_list.txt", "w+") as time_list:
+    with (outdirectory / "time_list.txt").open("w+") as time_list:
         for time in arr_tmid:
             time_list.write(f"{time} \n")
 
     print(f"Saved in {outdirectory}")
```

### Comparing `artistools-2023.5.16.3/artistools/spectra/test_spectra.py` & `artistools-2023.8.1/artistools/spectra/test_spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import math
 from pathlib import Path
 from unittest import mock
 
 import matplotlib.axes
 import numpy as np
 import pandas as pd
-from astropy import constants as const
 
 import artistools as at
 
 modelpath = at.get_config()["path_testartismodel"]
 outputpath = at.get_config()["path_testoutput"]
 
 
@@ -91,16 +90,16 @@
     assert abs(dfspectrum["lambda_angstroms"].to_numpy()[-1] - 29920.601421214415) < 1e-5
     assert abs(dfspectrum["lambda_angstroms"].to_numpy()[0] - 600.75759482509852) < 1e-5
 
     check_spectrum(dfspectrum)
 
     lambda_min = dfspectrum["lambda_angstroms"].to_numpy()[0]
     lambda_max = dfspectrum["lambda_angstroms"].to_numpy()[-1]
-    timelowdays = at.get_timestep_times_float(modelpath)[55]
-    timehighdays = at.get_timestep_times_float(modelpath)[65]
+    timelowdays = at.get_timestep_times(modelpath)[55]
+    timehighdays = at.get_timestep_times(modelpath)[65]
 
     dfspectrumpkts = at.spectra.get_from_packets(
         modelpath, timelowdays=timelowdays, timehighdays=timehighdays, lambda_min=lambda_min, lambda_max=lambda_max
     )[-1]
 
     check_spectrum(dfspectrumpkts)
 
@@ -112,15 +111,16 @@
         modelpath=modelpath, timestepmin=timestepmin, timestepmax=timestepmax, fnufilterfunc=None
     )[-1]
 
     integrated_flux_specout = np.trapz(dfspectrum["f_lambda"], x=dfspectrum["lambda_angstroms"])
 
     specdata = pd.read_csv(modelpath / "spec.out", delim_whitespace=True)
     arraynu = specdata.loc[:, "0"].to_numpy()
-    arraylambda_angstroms = const.c.to("angstrom/s").value / arraynu
+    c_ang_per_s = 2.99792458e18
+    arraylambda_angstroms = c_ang_per_s / arraynu
 
     contribution_list, array_flambda_emission_total = at.spectra.get_flux_contributions(
         modelpath,
         timestepmin=timestepmin,
         timestepmax=timestepmax,
         use_lastemissiontype=False,
     )
```

### Comparing `artistools-2023.5.16.3/artistools/spectra/test_vspectra.py` & `artistools-2023.8.1/artistools/spectra/test_vspectra.py`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistools/stats.py` & `artistools-2023.8.1/artistools/stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 #!/usr/bin/env python3
-import glob
 import sys
+from pathlib import Path
 
 import matplotlib.pyplot as plt
 
 xminvalue, xmaxvalue = 3500, 7000
 
 h = 6.62607004e-34  # m^2 kg / s
 c = 299792458  # m / s
 
 
-def main():
-    logfiles = glob.glob("output_0-0.txt") + glob.glob("*/output_0-0.txt") + glob.glob("*/*/output_0-0.txt")
+def main() -> None:
+    logfiles = list(Path().glob("**/output_0-0.txt"))
     if not logfiles:
         print("no output log files found")
         sys.exit()
 
     fig, axes = plt.subplots(
         nrows=2, ncols=1, sharey=True, figsize=(8, 5), tight_layout={"pad": 0.2, "w_pad": 0.0, "h_pad": 0.0}
     )
 
     for index, logfilename in enumerate(logfiles):
-        runfolder = logfilename.split("/output_0-0.txt")[0]
+        runfolder = logfilename.parent
 
-        timesteptimes = []
-        with open(runfolder + "/light_curve.out") as lcfile:
-            for line in lcfile:
-                timesteptimes.append(line.split()[0])
+        timesteptimes: list[str] = []
+        with (runfolder / "light_curve.out").open() as lcfile:
+            timesteptimes.extend(line.split()[0] for line in lcfile)
+        timesteptimes = timesteptimes[: len(timesteptimes) // 2]
 
-        timesteptimes = timesteptimes[: int(len(timesteptimes) / 2)]
+        stats: list[dict[str, int]] = []
 
-        stats = []
-
-        with open(logfilename) as flog:
+        with logfilename.open() as flog:
             for line in flog:
                 if line.startswith("timestep "):
                     currenttimestep = int(line.split(" ")[1].split(",")[0])
                     stats.append({})
                     if len(stats) != currenttimestep + 1:
                         print("WRONG TIMESTEP!")
                 if line.startswith("k_stat_"):
```

### Comparing `artistools-2023.5.16.3/artistools/test_artistools.py` & `artistools-2023.8.1/artistools/test_artistools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 import hashlib
 import math
-from typing import Any
+import typing as t
 
 import numpy as np
 
 import artistools as at
 
 modelpath = at.get_config()["path_testartismodel"]
 outputpath = at.get_config()["path_testoutput"]
@@ -15,31 +15,31 @@
     import importlib
 
     # ensure that the commands are pointing to valid submodule.function() targets
     for _command, (submodulename, funcname) in sorted(at.commands.get_commandlist().items()):
         submodule = importlib.import_module(submodulename, package="artistools")
         assert hasattr(submodule, funcname)
 
-    def recursive_check(dictcmd: dict[str, Any]) -> None:
+    def recursive_check(dictcmd: dict[str, t.Any]) -> None:
         for cmdtarget in dictcmd.values():
             if isinstance(cmdtarget, dict):
                 recursive_check(cmdtarget)
             else:
                 submodulename, funcname = cmdtarget
                 namestr = f"artistools.{submodulename.removeprefix('artistools.')}" if submodulename else "artistools"
                 submodule = importlib.import_module(namestr, package="artistools")
                 assert hasattr(submodule, funcname)
 
     recursive_check(at.commands.dictcommands)
 
 
 def test_timestep_times() -> None:
-    timestartarray = at.get_timestep_times_float(modelpath, loc="start")
-    timedeltarray = at.get_timestep_times_float(modelpath, loc="delta")
-    timemidarray = at.get_timestep_times_float(modelpath, loc="mid")
+    timestartarray = at.get_timestep_times(modelpath, loc="start")
+    timedeltarray = at.get_timestep_times(modelpath, loc="delta")
+    timemidarray = at.get_timestep_times(modelpath, loc="mid")
     assert len(timestartarray) == 100
     assert math.isclose(float(timemidarray[0]), 250.421, abs_tol=1e-3)
     assert math.isclose(float(timemidarray[-1]), 349.412, abs_tol=1e-3)
 
     assert all(
         tstart < tmid < (tstart + tdelta) for tstart, tdelta, tmid in zip(timestartarray, timedeltarray, timemidarray)
     )
@@ -96,15 +96,15 @@
 
 
 def test_get_ionrecombratecalibration() -> None:
     at.atomic.get_ionrecombratecalibration(modelpath=modelpath)
 
 
 def test_plotspherical() -> None:
-    at.plotspherical.main(argsraw=[], modelpath=modelpath, interpolate=True, outputfile=outputpath)
+    at.plotspherical.main(argsraw=[], modelpath=modelpath, outputfile=outputpath)
 
 
 def test_spencerfano() -> None:
     at.nonthermal.solvespencerfanocmd.main(
         argsraw=[], modelpath=modelpath, timedays=300, makeplot=True, npts=200, noexcitation=True, outputfile=outputpath
     )
```

### Comparing `artistools-2023.5.16.3/artistools/transitions.py` & `artistools-2023.8.1/artistools/transitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 #!/usr/bin/env python3
+from __future__ import annotations
+
 import argparse
 import math
 import sys
 from collections import namedtuple
 from pathlib import Path
 
 import matplotlib.pyplot as plt
@@ -13,22 +15,22 @@
 import artistools as at
 
 defaultoutputfile = "plottransitions_cell{cell:03d}_ts{timestep:02d}_{time_days:.0f}d.pdf"
 
 iontuple = namedtuple("iontuple", "Z ion_stage")
 
 
-def get_kurucz_transitions():
+def get_kurucz_transitions() -> tuple[pd.DataFrame, list[iontuple]]:
     hc_evcm = (const.h * const.c).to("eV cm").value
     transitiontuple = namedtuple(
-        "transition", "Z ionstage lambda_angstroms A lower_energy_ev upper_energy_ev lower_g upper_g"
+        "transitiontuple", "Z ionstage lambda_angstroms A lower_energy_ev upper_energy_ev lower_g upper_g"
     )
     translist = []
     ionlist = []
-    with open("gfall.dat") as fnist:
+    with Path("gfall.dat").open() as fnist:
         for line in fnist:
             row = line.split()
             if len(row) >= 24:
                 Z, ionstage = int(row[2].split(".")[0]), int(row[2].split(".")[1]) + 1
                 if Z < 44 or ionstage >= 2:  # and Z not in [26, 27]
                     continue
                 lambda_angstroms = float(line[:12]) * 10
@@ -46,18 +48,20 @@
                 if iontuple(Z, ionstage) not in ionlist:
                     ionlist.append(iontuple(Z, ionstage))
 
     dftransitions = pd.DataFrame(translist, columns=transitiontuple._fields)
     return dftransitions, ionlist
 
 
-def get_nist_transitions(filename):
-    transitiontuple = namedtuple("transition", "lambda_angstroms A lower_energy_ev upper_energy_ev lower_g upper_g")
+def get_nist_transitions(filename: Path | str) -> pd.DataFrame:
+    transitiontuple = namedtuple(
+        "transitiontuple", "lambda_angstroms A lower_energy_ev upper_energy_ev lower_g upper_g"
+    )
     translist = []
-    with open(filename) as fnist:
+    with Path(filename).open() as fnist:
         for line in fnist:
             row = line.split("|")
             if len(row) == 17 and "-" in row[5]:
                 if len(row[0].strip()) > 0:
                     lambda_angstroms = float(row[0])
                 elif len(row[1].strip()) > 0:
                     lambda_angstroms = float(row[1])
@@ -66,16 +70,15 @@
                 A = float(row[3]) if len(row[3].strip()) > 0 else 1e8
                 lower_energy_ev, upper_energy_ev = (float(x.strip(" []")) for x in row[5].split("-"))
                 lower_g, upper_g = (float(x.strip()) for x in row[12].split("-"))
                 translist.append(
                     transitiontuple(lambda_angstroms, A, lower_energy_ev, upper_energy_ev, lower_g, upper_g)
                 )
 
-    dftransitions = pd.DataFrame(translist, columns=transitiontuple._fields)
-    return dftransitions
+    return pd.DataFrame(translist, columns=transitiontuple._fields)
 
 
 def generate_ion_spectrum(transitions, xvalues, popcolumn, plot_resolution, args):
     yvalues = np.zeros(len(xvalues))
 
     # iterate over lines
     for _, line in transitions.iterrows():
@@ -174,16 +177,15 @@
 
 
 def add_upper_lte_pop(dftransitions, T_exc, ionpop, ltepartfunc, columnname=None) -> pd.DataFrame:
     K_B = const.k_B.to("eV / K").value
     scalefactor = ionpop / ltepartfunc
     if columnname is None:
         columnname = f"upper_pop_lte_{T_exc:.0f}K"
-    dftransitions = dftransitions.eval(f"{columnname} = @scalefactor * upper_g * exp(-upper_energy_ev / @K_B / @T_exc)")
-    return dftransitions
+    return dftransitions.eval(f"{columnname} = @scalefactor * upper_g * exp(-upper_energy_ev / @K_B / @T_exc)")
 
 
 def addargs(parser: argparse.ArgumentParser) -> None:
     parser.add_argument("-modelpath", default=None, type=Path, help="Path to ARTIS folder")
 
     parser.add_argument("-xmin", type=int, default=3500, help="Plot range: minimum wavelength in Angstroms")
 
@@ -262,22 +264,22 @@
 
     # also calculate wavelengths outside the plot range to include lines whose
     # edges pass through the plot range
     plot_xmin_wide = args.xmin * (1 - args.gaussian_window * args.sigma_v / const.c.to("km / s").value)
     plot_xmax_wide = args.xmax * (1 + args.gaussian_window * args.sigma_v / const.c.to("km / s").value)
 
     ionlist = [
-        (26, 1),
-        (26, 2),
-        (26, 3),
-        (27, 2),
-        (27, 3),
-        (28, 2),
-        (28, 3),
-        # (28, 2),
+        iontuple(26, 1),
+        iontuple(26, 2),
+        iontuple(26, 3),
+        iontuple(27, 2),
+        iontuple(27, 3),
+        iontuple(28, 2),
+        iontuple(28, 3),
+        # iontuple(28, 2),
         # iontuple(45, 1),
         # iontuple(54, 1),
         # iontuple(54, 2),
         # iontuple(55, 1),
         # iontuple(55, 2),
         # iontuple(58, 1),
         # iontuple(79, 1),
@@ -350,15 +352,15 @@
 
     hc = (const.h * const.c).to("eV Angstrom").value
 
     xvalues = np.arange(args.xmin, args.xmax, step=plot_resolution)
     yvalues = np.zeros((len(temperature_list) + 1, len(ionlist), len(xvalues)))
 
     for _, ion in adata.iterrows() if args.atomicdatabase == "artis" else enumerate(ionlist):
-        ionid = (ion.Z, ion.ion_stage)
+        ionid = iontuple(ion.Z, ion.ion_stage)
         if ionid not in ionlist:
             continue
 
         ionindex = ionlist.index(ionid)
 
         if args.atomicdatabase == "kurucz":
             dftransitions = dftransgfall.query("Z == @ion.Z and ionstage == @ion.ion_stage", inplace=False).copy()
@@ -443,15 +445,15 @@
                 if args.print_lines:
                     dftransitions = dftransitions.eval(f"flux_factor_{popcolumnname} = flux_factor * {popcolumnname}")
 
                 yvalues[seriesindex][ionindex] = generate_ion_spectrum(
                     dftransitions, xvalues, popcolumnname, plot_resolution, args
                 )
                 if args.normalised:
-                    yvalues[seriesindex][ionindex] /= max(yvalues[seriesindex][ionindex])  # todo: move to ax.plot line
+                    yvalues[seriesindex][ionindex] /= max(yvalues[seriesindex][ionindex])  # TODO: move to ax.plot line
 
         if args.print_lines:
             print(dftransitions.columns)
             print(
                 dftransitions[
                     ["lower", "upper", "forbidden", "A", "lambda_angstroms", "flux_factor_upper_pop_lte_3000K"]
                 ].to_string(index=False)
```

### Comparing `artistools-2023.5.16.3/artistools/viewing_angles_visualization.py` & `artistools-2023.8.1/artistools/viewing_angles_visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,15 @@
     )
 
     if outfile:
         if outfile.endswith("html"):
             fig.write_html(outfile, auto_play=False)
         else:
             fig.write_image(outfile)
-        print("Figure saved as %s" % outfile)
+        print(f"Figure saved as {outfile}")
 
     if show_plot:
         fig.show()
 
     return (isomin, isomax)
```

### Comparing `artistools-2023.5.16.3/artistools/writecomparisondata.py` & `artistools-2023.8.1/artistools/writecomparisondata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 #!/usr/bin/env python3
 """Tools to get artis output in the required format for the code comparison workshop."""
+from __future__ import annotations
+
 import argparse
+import typing as t
 from pathlib import Path
 
 import numpy as np
 
 import artistools as at
 
+if t.TYPE_CHECKING:
+    from io import TextIOWrapper
+
 
-def write_spectra(modelpath, model_id, selected_timesteps, outfile):
+def write_spectra(modelpath: str | Path, model_id: str, selected_timesteps: t.Sequence[int], outfilepath: Path) -> None:
     spec_data = np.loadtxt(Path(modelpath, "spec.out"))
 
     times = spec_data[0, 1:]
     freqs = spec_data[1:, 0]
     lambdas = 2.99792458e18 / freqs
 
     # print("\n".join(["{0}, {1}".format(*x) for x in enumerate(times)]))
@@ -26,32 +32,34 @@
     lum_lambda = np.zeros((len(lambdas), len(times)))
 
     # convert flux to power by multiplying by area
     for n in range(1000):
         # 2.99792458e18 is c in Angstrom / second
         lum_lambda[n, :] = fluxes_nu[n, :] * 2.99792458e18 / lambdas[n] / lambdas[n] * area
 
-    with open(outfile, "w") as f:
-        f.write(f"#NTIMES: {len(selected_timesteps)}\n")
-        f.write(f"#NWAVE: {len(lambdas)}\n")
-        f.write("#TIMES[d]: {}\n".format(" ".join([f"{times[ts]:.2f}" for ts in selected_timesteps])))
-        f.write("#wavelength[Ang] flux_t0[erg/s/Ang] flux_t1[erg/s/Ang] ... flux_tn[erg/s/Ang]\n")
+    with outfilepath.open("w") as outfile:
+        outfile.write(f"#NTIMES: {len(selected_timesteps)}\n")
+        outfile.write(f"#NWAVE: {len(lambdas)}\n")
+        outfile.write(f'#TIMES[d]: {" ".join([f"{times[ts]:.2f}" for ts in selected_timesteps])}\n')
+        outfile.write("#wavelength[Ang] flux_t0[erg/s/Ang] flux_t1[erg/s/Ang] ... flux_tn[erg/s/Ang]\n")
 
         for n in reversed(range(len(lambdas))):
-            f.write(f"{lambdas[n]:.2f} " + " ".join([f"{lum_lambda[n, ts]:.2e}" for ts in selected_timesteps]) + "\n")
+            outfile.write(
+                f"{lambdas[n]:.2f} " + " ".join([f"{lum_lambda[n, ts]:.2e}" for ts in selected_timesteps]) + "\n"
+            )
 
-        f.close()
+        outfile.close()
 
 
-def write_ntimes_nvel(f, selected_timesteps, modelpath):
-    times = at.get_timestep_times_float(modelpath)
+def write_ntimes_nvel(outfile: TextIOWrapper, selected_timesteps: t.Sequence[int], modelpath: str | Path) -> None:
+    times = at.get_timestep_times(modelpath)
     modeldata, t_model_init_days, _ = at.inputmodel.get_modeldata_tuple(modelpath)
-    f.write(f"#NTIMES: {len(selected_timesteps)}\n")
-    f.write(f"#NVEL: {len(modeldata)}\n")
-    f.write(f'#TIMES[d]: {" ".join([f"{times[ts]:.2f}" for ts in selected_timesteps])}\n')
+    outfile.write(f"#NTIMES: {len(selected_timesteps)}\n")
+    outfile.write(f"#NVEL: {len(modeldata)}\n")
+    outfile.write(f'#TIMES[d]: {" ".join([f"{times[ts]:.2f}" for ts in selected_timesteps])}\n')
 
 
 def write_single_estimator(modelpath, selected_timesteps, estimators, allnonemptymgilist, outfile, keyname) -> None:
     modeldata, t_model_init_days, _ = at.inputmodel.get_modeldata_tuple(modelpath)
     with Path(outfile).open("w") as f:
         write_ntimes_nvel(f, selected_timesteps, modelpath)
         if keyname == "total_dep":
@@ -72,26 +80,33 @@
                 # except KeyError:
                 #     cellvalue = (estimators[(timestep - 1, modelgridindex)][keyname]
                 #                  + estimators[(timestep + 1, modelgridindex)][keyname]) / 2.
                 f.write(f" {cellvalue:.3e}")
             f.write("\n")
 
 
-def write_ionfracts(modelpath, model_id, selected_timesteps, estimators, allnonemptymgilist, outputpath):
-    times = at.get_timestep_times_float(modelpath)
+def write_ionfracts(
+    modelpath: Path | str,
+    model_id: str,
+    selected_timesteps: t.Sequence[int],
+    estimators: dict,
+    allnonemptymgilist: t.Sequence[int],
+    outputpath,
+) -> None:
+    times = at.get_timestep_times(modelpath)
     modeldata, t_model_init_days, _ = at.inputmodel.get_modeldata_tuple(modelpath)
     elementlist = at.get_composition_data(modelpath)
     nelements = len(elementlist)
     for element in range(nelements):
         atomic_number = elementlist.Z[element]
         elsymb = at.get_elsymbol(atomic_number).lower()
         nions = elementlist.nions[element]
         pathfileout = Path(outputpath, f"ionfrac_{elsymb}_{model_id}_artisnebular.txt")
         fileisallzeros = True  # will be changed when a non-zero is encountered
-        with open(pathfileout, "w") as f:
+        with pathfileout.open("w") as f:
             f.write(f"#NTIMES: {len(selected_timesteps)}\n")
             f.write(f"#NSTAGES: {nions}\n")
             f.write(f'#TIMES[d]: {" ".join([f"{times[ts]:.2f}" for ts in selected_timesteps])}\n')
             f.write("#\n")
             for timestep in selected_timesteps:
                 f.write(f"#TIME: {times[timestep]:.2f}\n")
                 f.write(f"#NVEL: {len(allnonemptymgilist)}\n")
@@ -114,17 +129,17 @@
                     f.write("\n")
         if fileisallzeros:
             print(f"Deleting {pathfileout} because it is all zeros")
             pathfileout.unlink()
 
 
 def write_phys(modelpath, model_id, selected_timesteps, estimators, allnonemptymgilist, outputpath) -> None:
-    times = at.get_timestep_times_float(modelpath)
+    times = at.get_timestep_times(modelpath)
     modeldata, t_model_init_days, _ = at.inputmodel.get_modeldata_tuple(modelpath)
-    with open(Path(outputpath, f"phys_{model_id}_artisnebular.txt"), "w") as f:
+    with Path(outputpath, f"phys_{model_id}_artisnebular.txt").open("w") as f:
         f.write(f"#NTIMES: {len(selected_timesteps)}\n")
         f.write(f'#TIMES[d]: {" ".join([f"{times[ts]:.2f}" for ts in selected_timesteps])}\n')
         f.write("#\n")
         for timestep in selected_timesteps:
             f.write(f"#TIME: {times[timestep]:.2f}\n")
             f.write(f"#NVEL: {len(modeldata)}\n")
             f.write("#vel_mid[km/s] temp[K] rho[gcc] ne[/cm^3] natom[/cm^3]\n")
@@ -144,22 +159,24 @@
                 f.write(f"{v_mid:.2f}")
                 for keyname in ("Te", "rho", "nne", "nntot"):
                     estvalue = estimators[(timestep, modelgridindex)][keyname]
                     f.write(f" {estvalue:.4e}")
                 f.write("\n")
 
 
-def write_lbol_edep(modelpath, model_id, selected_timesteps, estimators, outputpath):
-    # times = at.get_timestep_times_float(modelpath)
-    dflightcurve = at.lightcurve.readfile(Path(modelpath, "light_curve.out"))[-1]
+def write_lbol_edep(
+    modelpath: str | Path, model_id: str, selected_timesteps: t.Sequence[int], outputpath: Path
+) -> None:
+    # times = at.get_timestep_times(modelpath)
+    dflightcurve = at.lightcurve.readfile(Path(modelpath, "light_curve.out"))[-1].to_pandas()
     dfdep = at.get_deposition(modelpath)
 
     df = dflightcurve.merge(dfdep, left_index=True, right_index=True, suffixes=("", "_dep"))
 
-    with open(outputpath, "w") as f:
+    with outputpath.open("w") as f:
         f.write(f"#NTIMES: {len(selected_timesteps)}\n")
         f.write("#time[d] Lbol[erg/s] Edep[erg/s] \n")
 
         for timestep, row in df.iterrows():
             if timestep not in selected_timesteps:
                 continue
             f.write(f"{row.time:.2f} {row.lum * 3.826e33:.2e} {row.total_dep_Lsun * 3.826e33:.2e}\n")
@@ -171,28 +188,28 @@
     parser.add_argument("-modelpath", default=[], nargs="*", action=at.AppendPath, help="Paths to ARTIS folders")
 
     parser.add_argument("-selected_timesteps", default=[], nargs="*", type=int, help="Selected ARTIS timesteps")
 
     parser.add_argument("-outputpath", "-o", action="store", type=Path, default=Path(), help="path for output files")
 
 
-def main(args=None, argsraw=None, **kwargs):
+def main(args=None, argsraw=None, **kwargs) -> None:
     """Write ARTIS model data out in code comparison workshop format."""
     if args is None:
         parser = argparse.ArgumentParser(
             formatter_class=at.CustomArgHelpFormatter,
             description=__doc__,
         )
         addargs(parser)
         parser.set_defaults(**kwargs)
         args = parser.parse_args(argsraw)
 
     if not args.modelpath:
-        args.modelpath = [Path(".")]
-    elif isinstance(args.modelpath, (str, Path)):
+        args.modelpath = [Path()]
+    elif isinstance(args.modelpath, str | Path):
         args.modelpath = [args.modelpath]
 
     modelpathlist = args.modelpath
     selected_timesteps = args.selected_timesteps
 
     args.outputpath.mkdir(parents=True, exist_ok=True)
 
@@ -209,33 +226,35 @@
         ]
 
         try:
             write_lbol_edep(
                 modelpath,
                 model_id,
                 selected_timesteps,
-                estimators,
-                Path(args.outputpath, "lbol_edep_" + model_id + "_artisnebular.txt"),
+                Path(args.outputpath, f"lbol_edep_{model_id}_artisnebular.txt"),
             )
         except FileNotFoundError:
             print("Can't write deposition because files are missing")
 
         write_spectra(
-            modelpath, model_id, selected_timesteps, Path(args.outputpath, "spectra_" + model_id + "_artisnebular.txt")
+            modelpath,
+            model_id,
+            selected_timesteps,
+            Path(args.outputpath, f"spectra_{model_id}_artisnebular.txt"),
         )
 
         # write_single_estimator(modelpath, selected_timesteps, estimators, allnonemptymgilist,
         #                        Path(args.outputpath, "eden_" + model_id + "_artisnebular.txt"), keyname='nne')
 
         write_single_estimator(
             modelpath,
             selected_timesteps,
             estimators,
             allnonemptymgilist,
-            Path(args.outputpath, "edep_" + model_id + "_artisnebular.txt"),
+            Path(args.outputpath, f"edep_{model_id}_artisnebular.txt"),
             keyname="total_dep",
         )
 
         # write_single_estimator(modelpath, selected_timesteps, estimators, allnonemptymgilist,
         #                        Path(args.outputpath, "tgas_" + model_id + "_artisnebular.txt"), keyname='Te')
 
         write_phys(modelpath, model_id, selected_timesteps, estimators, allnonemptymgilist, args.outputpath)
```

### Comparing `artistools-2023.5.16.3/artistools.egg-info/SOURCES.txt` & `artistools-2023.8.1/artistools.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,212 +1,44 @@
-.codeclimate.yml
 .codecov.yml
 .git-blame-ignore-revs
 .gitattributes
 .gitignore
-.landscape.yml
 .pre-commit-config.yaml
 .python-version
+.sourcery.yaml
+CITATION.cff
 CODEOWNERS
 LICENSE.txt
 MANIFEST.in
 README.md
 artistoolscompletions.sh
 pyproject.toml
 requirements.txt
-setup.cfg
 setup.py
 ./artistools/__init__.py
 ./artistools/__main__.py
 ./artistools/codecomparison.py
 ./artistools/commands.py
 ./artistools/configuration.py
 ./artistools/deposition.py
 ./artistools/gsinetwork.py
 ./artistools/hesma_scripts.py
 ./artistools/initial_composition.py
 ./artistools/linefluxes.py
 ./artistools/logfiles.py
 ./artistools/macroatom.py
-./artistools/matplotlibrc
 ./artistools/misc.py
 ./artistools/plotspherical.py
 ./artistools/plottools.py
 ./artistools/radfield.py
 ./artistools/stats.py
 ./artistools/test_artistools.py
 ./artistools/transitions.py
 ./artistools/viewing_angles_visualization.py
 ./artistools/writecomparisondata.py
-./artistools/atomic/__init__.py
-./artistools/atomic/_atomic_core.py
-./artistools/data/ElBiEn_2007.txt
-./artistools/data/__init__.py
-./artistools/data/atomic_properties.txt
-./artistools/data/betaminusdecays.txt
-./artistools/data/binding_energies.txt
-./artistools/data/collion-AR1985.txt
-./artistools/data/collion-reference.txt
-./artistools/data/collion.txt
-./artistools/data/elements.csv
-./artistools/data/solar_r_abundance_pattern.txt
-./artistools/data/splitmetadata.py
-./artistools/data/filters/400.txt
-./artistools/data/filters/520.txt
-./artistools/data/filters/B.txt
-./artistools/data/filters/FUV.txt
-./artistools/data/filters/H.txt
-./artistools/data/filters/H_ab.txt
-./artistools/data/filters/I.txt
-./artistools/data/filters/J.txt
-./artistools/data/filters/J_ab.txt
-./artistools/data/filters/K.txt
-./artistools/data/filters/K_ab.txt
-./artistools/data/filters/NUV.txt
-./artistools/data/filters/R.txt
-./artistools/data/filters/U.txt
-./artistools/data/filters/V.txt
-./artistools/data/filters/gs.txt
-./artistools/data/filters/is.txt
-./artistools/data/filters/rs.txt
-./artistools/data/filters/us.txt
-./artistools/data/filters/uvm2.txt
-./artistools/data/filters/uvm2_ab.txt
-./artistools/data/filters/uvw1.txt
-./artistools/data/filters/uvw1_ab.txt
-./artistools/data/filters/uvw2.txt
-./artistools/data/filters/uvw2_ab.txt
-./artistools/data/filters/zs.txt
-./artistools/data/filters/ASIAGO/B.txt
-./artistools/data/filters/ASIAGO/U.txt
-./artistools/data/filters/ASIAGO/V.txt
-./artistools/data/filters/ASIAGO/gs.txt
-./artistools/data/filters/ASIAGO/is.txt
-./artistools/data/filters/ASIAGO/rs.txt
-./artistools/data/filters/ASIAGO/zs.txt
-./artistools/data/filters/LCOGT/B.txt
-./artistools/data/filters/LCOGT/I.txt
-./artistools/data/filters/LCOGT/R.txt
-./artistools/data/filters/LCOGT/U.txt
-./artistools/data/filters/LCOGT/V.txt
-./artistools/data/filters/LCOGT/gs.txt
-./artistools/data/filters/LCOGT/is.txt
-./artistools/data/filters/LCOGT/rs.txt
-./artistools/data/filters/LCOGT/us.txt
-./artistools/data/filters/LCOGT/zs.txt
-./artistools/data/filters/LSQ/rs.txt
-./artistools/data/filters/LT/gs.txt
-./artistools/data/filters/LT/is.txt
-./artistools/data/filters/LT/rs.txt
-./artistools/data/filters/LT/us.txt
-./artistools/data/filters/LT/zs.txt
-./artistools/data/filters/NOT/B.txt
-./artistools/data/filters/NOT/I.txt
-./artistools/data/filters/NOT/R.txt
-./artistools/data/filters/NOT/U.txt
-./artistools/data/filters/NOT/V.txt
-./artistools/data/filters/NOT/gs.txt
-./artistools/data/filters/NOT/is.txt
-./artistools/data/filters/NOT/rs.txt
-./artistools/data/filters/NOT/us.txt
-./artistools/data/filters/NOT/zs.txt
-./artistools/data/filters/NTT/B.txt
-./artistools/data/filters/NTT/I.txt
-./artistools/data/filters/NTT/R.txt
-./artistools/data/filters/NTT/U.txt
-./artistools/data/filters/NTT/V.txt
-./artistools/data/filters/NTT/gs.txt
-./artistools/data/filters/NTT/rs.txt
-./artistools/data/filters/NTT/zs.txt
-./artistools/data/filters/OGLE/I.txt
-./artistools/data/filters/OGLE/V.txt
-./artistools/data/filters/PS1/gs.txt
-./artistools/data/filters/PS1/is.txt
-./artistools/data/filters/PS1/rs.txt
-./artistools/data/filters/PS1/ws.txt
-./artistools/data/filters/PS1/zs.txt
-./artistools/data/filters/SKYMAPPER/gs.txt
-./artistools/data/filters/SKYMAPPER/is.txt
-./artistools/data/filters/SKYMAPPER/rs.txt
-./artistools/data/filters/SKYMAPPER/us.txt
-./artistools/data/filters/SKYMAPPER/zs.txt
-./artistools/data/lightcurves/bollightcurves/AT2017gfo_smarttetal2017.txt
-./artistools/data/lightcurves/bollightcurves/AT2017gfo_waxmanetal2018.txt
-./artistools/data/refspectra/2003du_20031213_3219_8822_00.txt
-./artistools/data/refspectra/2010lp_20110928_fors2.txt
-./artistools/data/refspectra/FranssonJerkstrand2015_W7_330d_10Mpc.txt
-./artistools/data/refspectra/PSNJ11492548_20160202_3Ang.txt
-./artistools/data/refspectra/PTF11kly_20120402_norm.dat.txt
-./artistools/data/refspectra/SN2013aa_20140216_3Ang.txt
-./artistools/data/refspectra/SN2013aa_20140421_3Ang.txt
-./artistools/data/refspectra/SN2013cs_20140325_3Ang.txt
-./artistools/data/refspectra/SN2013ct_20131119_3Ang.txt
-./artistools/data/refspectra/maurer2011_RTJ_W7_338d_1Mpc.txt
-./artistools/data/refspectra/sn2011fe_PTF11kly_20120822_norm.txt
-./artistools/estimators/__init__.py
-./artistools/estimators/__main__.py
-./artistools/estimators/estimators.py
-./artistools/estimators/estimators_classic.py
-./artistools/estimators/exportmassfractions.py
-./artistools/estimators/plot3destimators_classic.py
-./artistools/estimators/plotestimators.py
-./artistools/inputmodel/1dslicefrom3d.py
-./artistools/inputmodel/__init__.py
-./artistools/inputmodel/botyanski2017.py
-./artistools/inputmodel/describeinputmodel.py
-./artistools/inputmodel/downscale3dgrid.py
-./artistools/inputmodel/energyinputfiles.py
-./artistools/inputmodel/fullymixed.py
-./artistools/inputmodel/inputmodel_misc.py
-./artistools/inputmodel/lapuente.py
-./artistools/inputmodel/makeartismodel.py
-./artistools/inputmodel/maketardismodelfromartis.py
-./artistools/inputmodel/map_1d_to_3d_grid.py
-./artistools/inputmodel/maptogrid.py
-./artistools/inputmodel/modelfromhydro.py
-./artistools/inputmodel/opacityinputfile.py
-./artistools/inputmodel/plotdensity.py
-./artistools/inputmodel/recombinationenergy.py
-./artistools/inputmodel/rprocess_from_trajectory.py
-./artistools/inputmodel/rprocess_solar.py
-./artistools/inputmodel/scalevelocity.py
-./artistools/inputmodel/shen2018.py
-./artistools/inputmodel/slice1Dfromconein3dmodel.py
-./artistools/inputmodel/test_inputmodel.py
-./artistools/inputmodel/fromcmfgen/__init__.py
-./artistools/inputmodel/fromcmfgen/convert_to_artis_neartimezero.py
-./artistools/inputmodel/fromcmfgen/rd_cmfgen.py
-./artistools/lightcurve/__init__.py
-./artistools/lightcurve/__main__.py
-./artistools/lightcurve/lightcurve.py
-./artistools/lightcurve/plotlightcurve.py
-./artistools/lightcurve/test_lightcurve.py
-./artistools/lightcurve/viewingangleanalysis.py
-./artistools/lightcurve/writebollightcurvedata.py
-./artistools/nltepops/__init__.py
-./artistools/nltepops/__main__.py
-./artistools/nltepops/nltepops.py
-./artistools/nltepops/plotnltepops.py
-./artistools/nonthermal/__init__.py
-./artistools/nonthermal/__main__.py
-./artistools/nonthermal/_nonthermal_core.py
-./artistools/nonthermal/leptontransport.py
-./artistools/nonthermal/plotnonthermal.py
-./artistools/nonthermal/solvespencerfanocmd.py
-./artistools/packets/__init__.py
-./artistools/packets/packets.py
-./artistools/packets/packetsplots.py
-./artistools/spectra/__init__.py
-./artistools/spectra/__main__.py
-./artistools/spectra/plotspectra.py
-./artistools/spectra/sampleblackbodyfrompacketTR.py
-./artistools/spectra/spectra.py
-./artistools/spectra/test_spectra.py
-./artistools/spectra/test_vspectra.py
-./tests/__init__.py
 .github/dependabot.yml
 .github/workflows/deploypypi.yml
 .github/workflows/deploytestpypi.yml
 .github/workflows/linter.yml
 .github/workflows/pytest.yml
 artistools/__init__.py
 artistools/__main__.py
@@ -220,14 +52,15 @@
 artistools/linefluxes.py
 artistools/logfiles.py
 artistools/macroatom.py
 artistools/matplotlibrc
 artistools/misc.py
 artistools/plotspherical.py
 artistools/plottools.py
+artistools/py.typed
 artistools/radfield.py
 artistools/stats.py
 artistools/test_artistools.py
 artistools/transitions.py
 artistools/viewing_angles_visualization.py
 artistools/writecomparisondata.py
 artistools.egg-info/PKG-INFO
```

### Comparing `artistools-2023.5.16.3/artistools.egg-info/entry_points.txt` & `artistools-2023.8.1/artistools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/artistoolscompletions.sh` & `artistools-2023.8.1/artistoolscompletions.sh`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/images/fig-emission.pdf` & `artistools-2023.8.1/images/fig-emission.pdf`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/images/fig-emission.png` & `artistools-2023.8.1/images/fig-emission.png`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/images/fig-estimators.pdf` & `artistools-2023.8.1/images/fig-estimators.pdf`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/images/fig-estimators.png` & `artistools-2023.8.1/images/fig-estimators.png`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/images/fig-nlte-Ni.pdf` & `artistools-2023.8.1/images/fig-nlte-Ni.pdf`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/images/fig-nlte-Ni.png` & `artistools-2023.8.1/images/fig-nlte-Ni.png`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/setup.py` & `artistools-2023.8.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 #!/usr/bin/env python3
 # mypy: ignore-errors
 """Plotting and analysis tools for the ARTIS 3D supernova radiative transfer code."""
 import importlib.util
 from pathlib import Path
 
-from setuptools import find_namespace_packages
 from setuptools import setup
 from setuptools_scm import get_version
 
 spec = importlib.util.spec_from_file_location("commands", "./artistools/commands.py")
 commands = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(commands)
 
 setup(
     name="artistools",
     version=get_version(),
-    use_scm_version={"local_scheme": "no-local-version"},
     author="ARTIS Collaboration",
     author_email="luke.shingles@gmail.com",
-    packages=find_namespace_packages(where="."),
     package_dir={"": "."},
-    package_data={"artistools": ["**/*.txt", "**/*.csv", "**/*.md", "matplotlibrc"]},
     url="https://www.github.com/artis-mcrt/artistools/",
     long_description=(Path(__file__).absolute().parent / "README.md").open().read(),
     long_description_content_type="text/markdown",
-    install_requires=(Path(__file__).absolute().parent / "requirements.txt").open().read().splitlines(),
     entry_points={
         "console_scripts": commands.get_console_scripts(),
     },
     scripts=["artistoolscompletions.sh"],
-    setup_requires=["psutil>=5.9.0", "setuptools>=45", "setuptools_scm[toml]>=6.2", "wheel"],
-    tests_require=["pytest", "pytest-runner", "pytest-cov"],
-    include_package_data=True,
 )
```

### Comparing `artistools-2023.5.16.3/tests/data/testmodel_3d_10^3/abundances.txt.xz` & `artistools-2023.8.1/tests/data/testmodel_3d_10^3/abundances.txt.xz`

 * *Files identical despite different names*

### Comparing `artistools-2023.5.16.3/tests/data/testmodel_3d_10^3/model.txt.xz` & `artistools-2023.8.1/tests/data/testmodel_3d_10^3/model.txt.xz`

 * *Files identical despite different names*

