# Comparing `tmp/fsps-0.4.3rc1.tar.gz` & `tmp/fsps-0.4.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsps-0.4.3rc1.tar", last modified: Mon May  1 10:34:45 2023, max compression
+gzip compressed data, was "fsps-0.4.4rc1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `fsps-0.4.3rc1.tar` & `fsps-0.4.4rc1.tar`

### file list

```diff
@@ -1,100 +1,55 @@
--rw-r--r--   0        0        0       24 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/.gitattributes
--rw-r--r--   0        0        0      157 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/.gitignore
--rw-r--r--   0        0        0       97 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/.gitmodules
--rw-r--r--   0        0        0      203 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/AUTHORS.rst
--rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/LICENSE.rst
--rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/README.rst
--rw-r--r--   0        0        0        7 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/demos/.gitignore
--rw-r--r--   0        0        0     1598 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/demos/dao69.py
--rw-r--r--   0        0        0     3952 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/demos/feature_demo.py
--rwxr-xr-x   0        0        0     1444 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/demos/plot_sdss_2mass_transmission.py
--rw-r--r--   0        0        0     6026 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/demos/specbymass.py
--rw-r--r--   0        0        0       37 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/.gitignore
--rw-r--r--   0        0        0     5647 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/Makefile
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/README.rst
--rw-r--r--   0        0        0    10307 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_static/pyfsps_logo.svg
--rwxr-xr-x   0        0        0      340 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_templates/sidebarintro.html
--rwxr-xr-x   0        0        0      340 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_templates/sidebarlogo.html
--rwxr-xr-x   0        0        0     1923 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/LICENSE
--rwxr-xr-x   0        0        0      346 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/README.rst
--rwxr-xr-x   0        0        0      799 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/dfm/layout.html
--rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/dfm/localtoc.html
--rwxr-xr-x   0        0        0      590 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/dfm/relations.html
--rwxr-xr-x   0        0        0     8516 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/dfm/static/flasky.css_t
--rwxr-xr-x   0        0        0      122 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/dfm/theme.conf
--rwxr-xr-x   0        0        0     4875 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/_themes/flask_theme_support.py
--rw-r--r--   0        0        0     1171 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/conf.py
--rw-r--r--   0        0        0    18397 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/filter_table.rst
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/filters.rst
--rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/filters_api.rst
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/index.rst
--rw-r--r--   0        0        0     4298 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/installation.rst
--rw-r--r--   0        0        0     3080 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/docs/stellarpop_api.rst
--rw-r--r--   0        0        0     1300 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/meson.build
--rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/noxfile.py
--rw-r--r--   0        0        0     1114 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/pyproject.toml
--rw-r--r--   0        0        0        6 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/requirements.txt
--rwxr-xr-x   0        0        0     2230 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/scripts/fsps_filter_table.py
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/__init__.py
--rwxr-xr-x   0        0        0     5807 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/filters.py
--rw-r--r--   0        0        0    17442 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/fsps.f90
--rw-r--r--   0        0        0    51091 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/fsps.py
--rw-r--r--   0        0        0      163 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/fsps_version.py
--rw-r--r--   0        0        0      129 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/.gitignore
--rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/LICENSE
--rw-r--r--   0        0        0     2965 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/README.md
--rw-r--r--   0        0        0     2063 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/Makefile
--rw-r--r--   0        0        0     4887 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/add_agb_dust.f90
--rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/add_bs.f90
--rw-r--r--   0        0        0     7263 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/add_dust.f90
--rw-r--r--   0        0        0     4284 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/add_nebular.f90
--rw-r--r--   0        0        0     1386 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/add_remnants.f90
--rw-r--r--   0        0        0     1309 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/add_xrb.f90
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/agn_dust.f90
--rw-r--r--   0        0        0     6368 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/attn_curve.f90
--rw-r--r--   0        0        0     4571 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/autosps.f90
--rw-r--r--   0        0        0    17238 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/compsp.f90
--rw-r--r--   0        0        0    14221 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/csp_gen.f90
--rw-r--r--   0        0        0     3701 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/funcint.f90
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/get_lumdist.f90
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/get_tuniv.f90
--rw-r--r--   0        0        0     3538 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/getindx.f90
--rw-r--r--   0        0        0     2342 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/getmags.f90
--rw-r--r--   0        0        0     9004 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/getspec.f90
--rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/igm_absorb.f90
--rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/imf.f90
--rw-r--r--   0        0        0     1716 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/imf_weight.f90
--rw-r--r--   0        0        0     7368 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/intsfwght.f90
--rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/lesssimple.f90
--rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/linterp.f90
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/linterparr.f90
--rw-r--r--   0        0        0      530 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/locate.f90
--rw-r--r--   0        0        0     2379 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/mod_gb.f90
--rw-r--r--   0        0        0     5619 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/mod_hb.f90
--rw-r--r--   0        0        0     2796 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/pz_convol.f90
--rw-r--r--   0        0        0     3136 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sbf.f90
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/setup_tabular_sfh.f90
--rw-r--r--   0        0        0     4603 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sfh_weight.f90
--rw-r--r--   0        0        0     6986 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sfhinfo.f90
--rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sfhlimit.f90
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sfhstat.f90
--rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/simple.f90
--rw-r--r--   0        0        0     4620 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/smoothspec.f90
--rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/spec_bin.f90
--rw-r--r--   0        0        0    46130 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sps_setup.f90
--rw-r--r--   0        0        0    11720 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sps_utils.f90
--rw-r--r--   0        0        0    22246 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/sps_vars.f90
--rw-r--r--   0        0        0     9606 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/ssp_gen.f90
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/tsum.f90
--rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/vacairconv.f90
--rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/write_isochrone.f90
--rw-r--r--   0        0        0     4368 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/libfsps/src/ztinterp.f90
--rw-r--r--   0        0        0     2438 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/meson.build
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/src/fsps/sps_home.py
--rw-r--r--   0        0        0      176 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/tests/options.py
--rw-r--r--   0        0        0       99 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/tests/simple.py
--rw-r--r--   0        0        0    13125 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/tests/tests.py
--rwxr-xr-x   0        0        0      660 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/tools/dist.py
--rwxr-xr-x   0        0        0      191 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/tools/f2py_include.py
--rwxr-xr-x   0        0        0      303 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/tools/version.py
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 fsps-0.4.3rc1/PKG-INFO
+-rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/.cirrus.yml
+-rw-r--r--   0        0        0       24 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/.gitattributes
+-rw-r--r--   0        0        0      119 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2213 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2619 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      718 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/.github/workflows/update-fsps.yml
+-rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/.gitignore
+-rw-r--r--   0        0        0       97 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/.gitmodules
+-rw-r--r--   0        0        0      459 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      203 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/AUTHORS.rst
+-rw-r--r--   0        0        0      421 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/CMakeLists.txt
+-rw-r--r--   0        0        0     1072 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/LICENSE.rst
+-rw-r--r--   0        0        0      499 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/README.rst
+-rw-r--r--   0        0        0        7 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/demos/.gitignore
+-rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/demos/dao69.py
+-rw-r--r--   0        0        0     3934 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/demos/feature_demo.py
+-rwxr-xr-x   0        0        0     1475 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/demos/plot_sdss_2mass_transmission.py
+-rw-r--r--   0        0        0     6054 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/demos/specbymass.py
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/.gitignore
+-rw-r--r--   0        0        0     5647 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/Makefile
+-rw-r--r--   0        0        0    10307 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/_static/pyfsps_logo.svg
+-rwxr-xr-x   0        0        0      340 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/_templates/sidebarintro.html
+-rwxr-xr-x   0        0        0      340 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/_templates/sidebarlogo.html
+-rwxr-xr-x   0        0        0     1921 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/_themes/LICENSE
+-rwxr-xr-x   0        0        0      346 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/_themes/README.rst
+-rwxr-xr-x   0        0        0      799 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/_themes/dfm/layout.html
+-rw-r--r--   0        0        0      340 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/_themes/dfm/localtoc.html
+-rwxr-xr-x   0        0        0      590 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/_themes/dfm/relations.html
+-rwxr-xr-x   0        0        0     8516 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/_themes/dfm/static/flasky.css_t
+-rwxr-xr-x   0        0        0      121 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/_themes/dfm/theme.conf
+-rwxr-xr-x   0        0        0     3905 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/_themes/flask_theme_support.py
+-rw-r--r--   0        0        0     1212 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/conf.py
+-rw-r--r--   0        0        0    14145 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/filter_table.rst
+-rw-r--r--   0        0        0      423 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/filters.rst
+-rw-r--r--   0        0        0      844 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/filters_api.rst
+-rw-r--r--   0        0        0     1108 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/index.rst
+-rw-r--r--   0        0        0     4298 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/installation.rst
+-rw-r--r--   0        0        0     3080 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/docs/stellarpop_api.rst
+-rw-r--r--   0        0        0      944 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/noxfile.py
+-rw-r--r--   0        0        0     2054 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/pyproject.toml
+-rw-r--r--   0        0        0      279 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/readthedocs.yml
+-rw-r--r--   0        0        0        6 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/requirements.txt
+-rwxr-xr-x   0        0        0     2218 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/scripts/fsps_filter_table.py
+-rw-r--r--   0        0        0     3451 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/src/fsps/CMakeLists.txt
+-rw-r--r--   0        0        0      387 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/src/fsps/__init__.py
+-rwxr-xr-x   0        0        0     5806 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/src/fsps/filters.py
+-rw-r--r--   0        0        0    17733 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/src/fsps/fsps.f90
+-rw-r--r--   0        0        0    51485 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/src/fsps/fsps.py
+-rw-r--r--   0        0        0      163 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/src/fsps/fsps_version.py
+-rw-r--r--   0        0        0      563 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/src/fsps/sps_home.py
+-rw-r--r--   0        0        0      176 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/tests/options.py
+-rw-r--r--   0        0        0       99 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/tests/simple.py
+-rw-r--r--   0        0        0    13120 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/tests/tests.py
+-rwxr-xr-x   0        0        0      191 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/tools/f2py_include.py
+-rw-r--r--   0        0        0     1334 2022-11-09 12:37:21.000000 fsps-0.4.4rc1/PKG-INFO
```

### Comparing `fsps-0.4.3rc1/LICENSE.rst` & `fsps-0.4.4rc1/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2013-2021 Python-FSPS developers.
+Copyright 2013-2023 Python-FSPS developers.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `fsps-0.4.3rc1/demos/dao69.py` & `fsps-0.4.4rc1/demos/dao69.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from __future__ import (division, print_function, absolute_import,
-                        unicode_literals)
-import pyfits
-import numpy as np
+from __future__ import absolute_import, division, print_function, unicode_literals
+
 import matplotlib.pyplot as pl
+import numpy as np
+import pyfits
+
 import fsps
 
 # Measurements of cluster parameters.
-tage = 10. ** (8.04 - 9)
+tage = 10.0 ** (8.04 - 9)
 logmass = 4.09
 dist_mod = 24.5
 
 # Set up the stellar population model.
 sp = fsps.StellarPopulation(imf_type=2, dust_type=1, mwr=3.1, dust2=0.3)
 
 # The measured magnitudes from the literature.
-data = {"wfc3_f160w": 16.386,
-        "wfc3_f275w": 17.398,
-        "wfc_acs_f814w": 17.155}
+data = {"wfc3_f160w": 16.386, "wfc3_f275w": 17.398, "wfc_acs_f814w": 17.155}
 
 # There are also a few filters that we have data for but aren't included in
 # the standard FSPS install:
 #   "F110W": 16.877,
 #   "F336W": 17.349,
 #   "F475W": 17.762,
 
@@ -35,23 +34,22 @@
 obs_spec /= 5e-20
 
 # The observed wavelength grid in the data is magically this:
 obs_lambda = np.arange(0, 4540) * 1.2 + 3700
 
 # Compute the model magnitudes.
 for b, v in data.iteritems():
-    print(b, v, sp.get_mags(zmet=20, tage=tage, band=b) - 2.5 * logmass
-          + dist_mod)
+    print(b, v, sp.get_mags(zmet=20, tage=tage, band=b) - 2.5 * logmass + dist_mod)
 
 # Compute the model spectrum in ``L_sun / A``.
 lam, spec = sp.get_spectrum(zmet=20, tage=tage, peraa=True)
-spec *= 3.839e33 * 10. ** (logmass - dist_mod / 2.5)
+spec *= 3.839e33 * 10.0 ** (logmass - dist_mod / 2.5)
 
 f = 1.0  # obs_spec[0, obs_lambda < 5000.][-1] / spec[lam < 5000.][-1]
-print(obs_spec[0, obs_lambda < 5000.][-1] / spec[lam < 5000.][-1])
+print(obs_spec[0, obs_lambda < 5000.0][-1] / spec[lam < 5000.0][-1])
 
 pl.loglog(obs_lambda, obs_spec[0], "k")
 pl.loglog(lam, spec * f, "r")
 
 pl.xlim(3700, 7000)
 # pl.ylim(10 ** 3, 10 ** 4.5)
 pl.savefig("spectrum.png")
```

### Comparing `fsps-0.4.3rc1/demos/feature_demo.py` & `fsps-0.4.4rc1/demos/feature_demo.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,133 +3,132 @@
 
 """feature_demo.py - This script creates a set of PDFs that illustrate the
 effect on the SED of successively turning on various options or changing the
 value of some variables.
 """
 
 import os
-import numpy as np
+
 import matplotlib.pyplot as pl
 from matplotlib.backends.backend_pdf import PdfPages
 
 import fsps
 
 
 def makefig(sps, tage=13.7, oldspec=None, **plotkwargs):
     w, spec = sps.get_spectrum(tage=tage)
     fig, ax = pl.subplots()
     if oldspec is not None:
-        ax.plot(w, oldspec / w * 1e19, color='gray', linewidth=2, alpha=0.5)
-    ax.plot(w, spec / w * 1e19, 'C2', linewidth=2)
+        ax.plot(w, oldspec / w * 1e19, color="gray", linewidth=2, alpha=0.5)
+    ax.plot(w, spec / w * 1e19, "C2", linewidth=2)
     return fig, ax, spec
 
 
 def prettify(fig, ax, label=None):
     ax.set_xlim(0.9e3, 1e6)
-    ax.set_xscale('log')
+    ax.set_xscale("log")
     ax.set_ylim(0.01, 2)
-    #ax.set_yscale('log')
-    ax.set_xlabel(r'rest-frame $\lambda$ ($\AA$)', fontsize=20)
-    ax.set_ylabel(r'$\lambda \, f_\lambda$', fontsize=20)
-    ax.tick_params(axis='both', which='major', labelsize=16)
+    # ax.set_yscale('log')
+    ax.set_xlabel(r"rest-frame $\lambda$ ($\AA$)", fontsize=20)
+    ax.set_ylabel(r"$\lambda \, f_\lambda$", fontsize=20)
+    ax.tick_params(axis="both", which="major", labelsize=16)
     if label is not None:
         ax.text(0.63, 0.85, label, transform=ax.transAxes, fontsize=16)
 
     fig.tight_layout()
     return fig, ax
 
 
 if __name__ == "__main__":
-
-    pl.rc('text', usetex=True)
-    pl.rc('font', family='serif')
-    pl.rc('axes', grid=False)
-    pl.rc('xtick', direction='in')
-    pl.rc('ytick', direction='in')
-    pl.rc('xtick', top=True)
-    pl.rc('ytick', right=True)
+    pl.rc("text", usetex=True)
+    pl.rc("font", family="serif")
+    pl.rc("axes", grid=False)
+    pl.rc("xtick", direction="in")
+    pl.rc("ytick", direction="in")
+    pl.rc("xtick", top=True)
+    pl.rc("ytick", right=True)
 
     sps = fsps.StellarPopulation(zcontinuous=1)
     ilib, slib, dlib = sps.libraries
     print(ilib, slib)
     os.makedirs("./figures", exist_ok=True)
-    pdf = PdfPages('./figures/features.pdf')
+    pdf = PdfPages("./figures/features.pdf")
 
     # Basic spectrum
-    sps.params['sfh'] = 4
-    sps.params['tau'] = 5.0
-    sps.params['logzsol'] = 0.0
-    sps.params['dust_type'] = 4  # kriek and Conroy
-    sps.params['imf_type'] = 2  # kroupa
-    sps.params['imf3'] = 2.3
+    sps.params["sfh"] = 4
+    sps.params["tau"] = 5.0
+    sps.params["logzsol"] = 0.0
+    sps.params["dust_type"] = 4  # kriek and Conroy
+    sps.params["imf_type"] = 2  # kroupa
+    sps.params["imf3"] = 2.3
     fig, ax, spec = makefig(sps)
     fig, ax = prettify(fig, ax, label=r"$\tau=5$, Age$=13.7$,\\n$\log Z/Z_\odot=0.0$")
     pdf.savefig(fig)
     pl.close(fig)
 
     # change IMF
-    sps.params['imf3'] = 2.5
+    sps.params["imf3"] = 2.5
     fig, ax, spec = makefig(sps, oldspec=spec)
     fig, ax = prettify(fig, ax, label=r"IMF slope")
     pdf.savefig(fig)
 
     # Attenuate
-    sps.params['add_dust_emission'] = False
-    sps.params['dust2'] = 0.2
+    sps.params["add_dust_emission"] = False
+    sps.params["dust2"] = 0.2
     fig, ax, spec = makefig(sps, oldspec=spec)
     fig, ax = prettify(fig, ax, label=r"Dust Attenuation")
     pdf.savefig(fig)
     pl.close(fig)
 
     # Dust emission
-    sps.params['add_dust_emission'] = True
+    sps.params["add_dust_emission"] = True
     fig, ax, spec = makefig(sps, oldspec=spec)
     fig, ax = prettify(fig, ax, label=r"Dust Emission")
     pdf.savefig(fig)
     pl.close(fig)
 
     # Dust temperature
-    sps.params['duste_umin'] = 10
+    sps.params["duste_umin"] = 10
     fig, ax, spec = makefig(sps, oldspec=spec)
     fig, ax = prettify(fig, ax, label=r"Dust SED\\n({})".format(dlib))
     pdf.savefig(fig)
     pl.close(fig)
 
     # AGN emission
-    sps.params['fagn'] = 0.3
+    sps.params["fagn"] = 0.3
     fig, ax, spec = makefig(sps, oldspec=spec)
     fig, ax = prettify(fig, ax, label=r"AGN dust\\n(Nenkova)")
     pdf.savefig(fig)
     pl.close(fig)
 
     # Nebular emission
-    sps.params['add_neb_emission'] = True
-    sps.params['gas_logu'] = -3.5
+    sps.params["add_neb_emission"] = True
+    sps.params["gas_logu"] = -3.5
     fig, ax, spec = makefig(sps, oldspec=spec)
     fig, ax = prettify(fig, ax, label=r"Neb. emission\\n(Byler)")
     pdf.savefig(fig)
     pl.close(fig)
 
     # change logu
-    sps.params['gas_logu'] = -1.0
+    sps.params["gas_logu"] = -1.0
     fig, ax, spec = makefig(sps, oldspec=spec)
     fig, ax = prettify(fig, ax, label=r"Change U$_{neb}$")
     pdf.savefig(fig)
     pl.close(fig)
 
     # change logz
-    sps.params['logzsol'] = -0.5
-    sps.params['gas_logz'] = -0.5
+    sps.params["logzsol"] = -0.5
+    sps.params["gas_logz"] = -0.5
     fig, ax, spec = makefig(sps, oldspec=spec)
     fig, ax = prettify(fig, ax, label=r"$\log Z/Z_\odot=-0.5$")
     pdf.savefig(fig)
     pl.close(fig)
 
     # IGM absorption
-    sps.params['zred'] = 6.0
-    sps.params['add_igm_absorption'] = True
+    sps.params["zred"] = 6.0
+    sps.params["add_igm_absorption"] = True
     fig, ax, spec = makefig(sps, oldspec=spec)
     fig, ax = prettify(fig, ax, label=r"IGM attenuation\\n(Madau, $z=6$)")
     pdf.savefig(fig)
     pl.close(fig)
 
     pdf.close()
```

### Comparing `fsps-0.4.3rc1/demos/specbymass.py` & `fsps-0.4.4rc1/demos/specbymass.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,48 @@
 # This demo shows how to make a plot of the fractional contribution of differnt
 # stellar mass ranges to the total spectrum, for different properties of the
 # stellar population.  There is also some use of the filter objects.
 
 from itertools import product
-import numpy as np
+
 import matplotlib.pyplot as pl
+import numpy as np
+
 import fsps
 
 # make an SPS object with interpolation in metallicity enabled, and
 # set a few parameters
 sps = fsps.StellarPopulation(zcontinuous=1)
-sps.params['imf_type'] = 0   # Salpeter IMF
-sps.params['sfh'] = 1  # Tau model SFH
+sps.params["imf_type"] = 0  # Salpeter IMF
+sps.params["sfh"] = 1  # Tau model SFH
 
 # Get a few filter transmission curves
-filterlist = {'galex_fuv': 'FUV', 'galex_nuv': 'NUV', 'sdss_u': 'u',
-              'sdss_g': 'g', 'sdss_i': 'i', '2mass_j': 'J'}
+filterlist = {
+    "galex_fuv": "FUV",
+    "galex_nuv": "NUV",
+    "sdss_u": "u",
+    "sdss_g": "g",
+    "sdss_i": "i",
+    "2mass_j": "J",
+}
 filters = [fsps.filters.get_filter(f) for f in filterlist]
 
 
 # This is the main function
-def specplots(tage=10.0, const=1.0, tau=1.0, neb=False, z=0.0, savefig=True,
-              masslims=[1.0, 3.0, 15.0, 30.0, 120.0], **kwargs):
-    """Make a number of plots showing the fraction of the total light due to
+def specplots(
+    tage=10.0,
+    const=1.0,
+    tau=1.0,
+    neb=False,
+    z=0.0,
+    savefig=True,
+    masslims=[1.0, 3.0, 15.0, 30.0, 120.0],
+    **kwargs,
+):
+    r"""Make a number of plots showing the fraction of the total light due to
     stars within certain stellar mass ranges.
 
     :param tage:
         The age of the stellar population
 
     :param const:
         0 or 1.  fraction of SF in constant SFR fraction
@@ -56,30 +72,30 @@
         ranges.
 
     :returns ffig:
         matplotlib figure giving a plot of the fraction of total flux due to
         stars in given mass ranges, as a function of wavelength.
     """
     # Set the FSPS params
-    sps.params['const'] = const
-    sps.params['tau'] = tau
-    sps.params['add_neb_emission'] = neb
-    sps.params['masscut'] = 120
-    sps.params['logzsol'] = z
+    sps.params["const"] = const
+    sps.params["tau"] = tau
+    sps.params["add_neb_emission"] = neb
+    sps.params["masscut"] = 120
+    sps.params["logzsol"] = z
     # Try to set any extra params
     for k, v in kwargs.items():
         try:
             sps.params[k] = v
-        except(KeyError):
+        except KeyError:
             pass
 
     # Make a pretty string with the FSPS parameters
-    sfh = {1: 'Constant SFR', 0: r'$\tau_{{SF}}={}$'.format(sps.params['tau'])}
-    sfhname = {1: 'const', 0: 'tau{}'.format(sps.params['tau'])}
-    name = '{}_z{}_neb{}'.format(sfhname[int(const)], z, neb)
+    sfh = {1: "Constant SFR", 0: r"$\tau_{{SF}}={}$".format(sps.params["tau"])}
+    sfhname = {1: "const", 0: "tau{}".format(sps.params["tau"])}
+    name = "{}_z{}_neb{}".format(sfhname[int(const)], z, neb)
 
     # get the total spectrum due to *all* stars
     wave, spec_tot = sps.get_spectrum(tage=tage)
 
     # Set up stellar mass ranges and arrays to hold output spectra
     mspec = np.zeros([len(sps.wavelengths), len(masslims)])
     dmspec = np.zeros_like(mspec)
@@ -89,72 +105,70 @@
     dfig, dax = pl.subplots(figsize=(12.4, 7.5))
     ffig, fax = pl.subplots(figsize=(12.4, 7.5))
     [ax.set_xlim(0.9e3, 1e4) for ax in [cax, fax, dax]]
 
     # Loop over upper mass limits, generating spectrum for each one
     for i, mc in enumerate(masslims):
         # set the upper stellar mass limit
-        sps.params['masscut'] = mc
+        sps.params["masscut"] = mc
         # get the spectrum at age = tage and store it
         w, spec = sps.get_spectrum(tage=tage)
         mspec[:, i] = spec.copy()
         # plot the spectrum due to stars less massive than the limit
-        cax.plot(w, spec, label='M < {}'.format(mc))
+        cax.plot(w, spec, label="M < {}".format(mc))
 
         if i == 0:
             # Plot the lowest mass bin spectrum
-            dax.plot(w, spec, label='{} < M < {}'.format(0.08, mc))
-            fax.plot(w, spec / spec_tot, label='{} < M < {}'.format(0.08, mc))
+            dax.plot(w, spec, label="{} < M < {}".format(0.08, mc))
+            fax.plot(w, spec / spec_tot, label="{} < M < {}".format(0.08, mc))
             # skip the rest of the loop
             continue
 
         # Subtract the spectrum from the last upper limit to ge tthe
         #  spectrum due to stars within the bin
-        dmspec[:, i] = spec - mspec[:, i-1]
+        dmspec[:, i] = spec - mspec[:, i - 1]
         # Plot it
-        label = '{} < M < {}'.format(masslims[i-1], mc)
+        label = "{} < M < {}".format(masslims[i - 1], mc)
         dax.plot(w, dmspec[:, i], label=label)
         # Plot the total spectrum
         if mc == masslims[-1]:
-            dax.plot(w, spec, label='Total', color='black')
+            dax.plot(w, spec, label="Total", color="black")
 
         # plot the fractional
         fax.plot(w, dmspec[:, i] / spec_tot, label=label)
 
     # prettify the axes, titles, etc
     [ax.legend(loc=0) for ax in [cax, dax, fax]]
-    [ax.set_xlabel('$\lambda (\AA)$') for ax in [cax, dax, fax]]
-    [ax.set_ylabel('$F_\lambda$') for ax in [cax, dax]]
-    [ax.set_yscale('log') for ax in [cax, dax]]
+    [ax.set_xlabel(r"$\lambda (\AA)$") for ax in [cax, dax, fax]]
+    [ax.set_ylabel(r"$F_\lambda$") for ax in [cax, dax]]
+    [ax.set_yscale("log") for ax in [cax, dax]]
     [ax.set_ylim(1e-20, 1e-14) for ax in [cax, dax]]
-    fstring = 'Age = {} Gyr, {}, log$Z/Z_\odot$={}'
-    vals = 10.0, sfh[int(sps.params['const'])], sps.params['logzsol']
+    fstring = r"Age = {} Gyr, {}, log$Z/Z_\odot$={}"
+    vals = 10.0, sfh[int(sps.params["const"])], sps.params["logzsol"]
     [ax.set_title(fstring.format(*vals)) for ax in [cax, dax, fax]]
-    fax.set_ylabel('$F/F_{tot}$')
+    fax.set_ylabel("$F/F_{tot}$")
 
     # plot filter transmission curves as shaded regions
     for f in filters:
         wavelength, transmission = f.transmission
         tmax = transmission.max()
         wmax = wavelength[transmission.argmax()]
-        fax.fill_between(wavelength, transmission / tmax * 0.8,
-                         alpha=0.3, color='grey')
-        fax.text(wmax, 0.83, filterlist[f.name], fontdict={'size': 16})
+        fax.fill_between(wavelength, transmission / tmax * 0.8, alpha=0.3, color="grey")
+        fax.text(wmax, 0.83, filterlist[f.name], fontdict={"size": 16})
 
     if savefig:
         # save to pdf
-        cfig.savefig('cspec_'+name+'.pdf')
-        dfig.savefig('dspec_'+name+'.pdf')
-        ffig.savefig('fspec_'+name+'.pdf')
+        cfig.savefig("cspec_" + name + ".pdf")
+        dfig.savefig("dspec_" + name + ".pdf")
+        ffig.savefig("fspec_" + name + ".pdf")
 
     return cfig, dfig, ffig
 
 
 if __name__ == "__main__":
-
     # set the stellar population age
     tage = 10.0  # in Gyr
 
     # Parameters to loop over
     # ----------
     # log Z/Z_sun
     zs = [-1.0, 0.0]
```

### Comparing `fsps-0.4.3rc1/docs/Makefile` & `fsps-0.4.4rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fsps-0.4.3rc1/docs/_static/pyfsps_logo.svg` & `fsps-0.4.4rc1/docs/_static/pyfsps_logo.svg`

 * *Files identical despite different names*

### Comparing `fsps-0.4.3rc1/docs/_themes/LICENSE` & `fsps-0.4.4rc1/docs/_themes/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Further modifications:
 
 Copyright 2012 Dan Foreman-Mackey
 
 
-Modifications: 
+Modifications:
 
 Copyright (c) 2011 Kenneth Reitz.
 
 
-Original Project: 
+Original Project:
 
 Copyright (c) 2010 by Armin Ronacher.
 
 
 Some rights reserved.
 
 Redistribution and use in source and binary forms of the theme, with or
```

### Comparing `fsps-0.4.3rc1/docs/_themes/dfm/layout.html` & `fsps-0.4.4rc1/docs/_themes/dfm/layout.html`

 * *Files identical despite different names*

### Comparing `fsps-0.4.3rc1/docs/_themes/dfm/relations.html` & `fsps-0.4.4rc1/docs/_themes/dfm/relations.html`

 * *Files identical despite different names*

### Comparing `fsps-0.4.3rc1/docs/_themes/dfm/static/flasky.css_t` & `fsps-0.4.4rc1/docs/_themes/dfm/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `fsps-0.4.3rc1/docs/_themes/flask_theme_support.py` & `fsps-0.4.4rc1/docs/_themes/flask_theme_support.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,89 @@
 # flasky extensions.  flasky pygments style based on tango style
 from pygments.style import Style
-from pygments.token import Keyword, Name, Comment, String, Error, \
-     Number, Operator, Generic, Whitespace, Punctuation, Other, Literal
+from pygments.token import (
+    Comment,
+    Error,
+    Generic,
+    Keyword,
+    Literal,
+    Name,
+    Number,
+    Operator,
+    Other,
+    Punctuation,
+    String,
+    Whitespace,
+)
 
 
 class FlaskyStyle(Style):
     background_color = "#f8f8f8"
     default_style = ""
 
     styles = {
         # No corresponding class for the following:
-        #Text:                     "", # class:  ''
-        Whitespace:                "underline #f8f8f8",      # class: 'w'
-        Error:                     "#a40000 border:#ef2929", # class: 'err'
-        Other:                     "#000000",                # class 'x'
-
-        Comment:                   "italic #8f5902", # class: 'c'
-        Comment.Preproc:           "noitalic",       # class: 'cp'
-
-        Keyword:                   "bold #004461",   # class: 'k'
-        Keyword.Constant:          "bold #004461",   # class: 'kc'
-        Keyword.Declaration:       "bold #004461",   # class: 'kd'
-        Keyword.Namespace:         "bold #004461",   # class: 'kn'
-        Keyword.Pseudo:            "bold #004461",   # class: 'kp'
-        Keyword.Reserved:          "bold #004461",   # class: 'kr'
-        Keyword.Type:              "bold #004461",   # class: 'kt'
-
-        Operator:                  "#582800",   # class: 'o'
-        Operator.Word:             "bold #004461",   # class: 'ow' - like keywords
-
-        Punctuation:               "bold #000000",   # class: 'p'
-
+        # Text:                     "", # class:  ''
+        Whitespace: "underline #f8f8f8",  # class: 'w'
+        Error: "#a40000 border:#ef2929",  # class: 'err'
+        Other: "#000000",  # class 'x'
+        Comment: "italic #8f5902",  # class: 'c'
+        Comment.Preproc: "noitalic",  # class: 'cp'
+        Keyword: "bold #004461",  # class: 'k'
+        Keyword.Constant: "bold #004461",  # class: 'kc'
+        Keyword.Declaration: "bold #004461",  # class: 'kd'
+        Keyword.Namespace: "bold #004461",  # class: 'kn'
+        Keyword.Pseudo: "bold #004461",  # class: 'kp'
+        Keyword.Reserved: "bold #004461",  # class: 'kr'
+        Keyword.Type: "bold #004461",  # class: 'kt'
+        Operator: "#582800",  # class: 'o'
+        Operator.Word: "bold #004461",  # class: 'ow' - like keywords
+        Punctuation: "bold #000000",  # class: 'p'
         # because special names such as Name.Class, Name.Function, etc.
         # are not recognized as such later in the parsing, we choose them
         # to look the same as ordinary variables.
-        Name:                      "#000000",        # class: 'n'
-        Name.Attribute:            "#c4a000",        # class: 'na' - to be revised
-        Name.Builtin:              "#004461",        # class: 'nb'
-        Name.Builtin.Pseudo:       "#3465a4",        # class: 'bp'
-        Name.Class:                "#000000",        # class: 'nc' - to be revised
-        Name.Constant:             "#000000",        # class: 'no' - to be revised
-        Name.Decorator:            "#888",           # class: 'nd' - to be revised
-        Name.Entity:               "#ce5c00",        # class: 'ni'
-        Name.Exception:            "bold #cc0000",   # class: 'ne'
-        Name.Function:             "#000000",        # class: 'nf'
-        Name.Property:             "#000000",        # class: 'py'
-        Name.Label:                "#f57900",        # class: 'nl'
-        Name.Namespace:            "#000000",        # class: 'nn' - to be revised
-        Name.Other:                "#000000",        # class: 'nx'
-        Name.Tag:                  "bold #004461",   # class: 'nt' - like a keyword
-        Name.Variable:             "#000000",        # class: 'nv' - to be revised
-        Name.Variable.Class:       "#000000",        # class: 'vc' - to be revised
-        Name.Variable.Global:      "#000000",        # class: 'vg' - to be revised
-        Name.Variable.Instance:    "#000000",        # class: 'vi' - to be revised
-
-        Number:                    "#990000",        # class: 'm'
-
-        Literal:                   "#000000",        # class: 'l'
-        Literal.Date:              "#000000",        # class: 'ld'
-
-        String:                    "#4e9a06",        # class: 's'
-        String.Backtick:           "#4e9a06",        # class: 'sb'
-        String.Char:               "#4e9a06",        # class: 'sc'
-        String.Doc:                "italic #8f5902", # class: 'sd' - like a comment
-        String.Double:             "#4e9a06",        # class: 's2'
-        String.Escape:             "#4e9a06",        # class: 'se'
-        String.Heredoc:            "#4e9a06",        # class: 'sh'
-        String.Interpol:           "#4e9a06",        # class: 'si'
-        String.Other:              "#4e9a06",        # class: 'sx'
-        String.Regex:              "#4e9a06",        # class: 'sr'
-        String.Single:             "#4e9a06",        # class: 's1'
-        String.Symbol:             "#4e9a06",        # class: 'ss'
-
-        Generic:                   "#000000",        # class: 'g'
-        Generic.Deleted:           "#a40000",        # class: 'gd'
-        Generic.Emph:              "italic #000000", # class: 'ge'
-        Generic.Error:             "#ef2929",        # class: 'gr'
-        Generic.Heading:           "bold #000080",   # class: 'gh'
-        Generic.Inserted:          "#00A000",        # class: 'gi'
-        Generic.Output:            "#888",           # class: 'go'
-        Generic.Prompt:            "#745334",        # class: 'gp'
-        Generic.Strong:            "bold #000000",   # class: 'gs'
-        Generic.Subheading:        "bold #800080",   # class: 'gu'
-        Generic.Traceback:         "bold #a40000",   # class: 'gt'
+        Name: "#000000",  # class: 'n'
+        Name.Attribute: "#c4a000",  # class: 'na' - to be revised
+        Name.Builtin: "#004461",  # class: 'nb'
+        Name.Builtin.Pseudo: "#3465a4",  # class: 'bp'
+        Name.Class: "#000000",  # class: 'nc' - to be revised
+        Name.Constant: "#000000",  # class: 'no' - to be revised
+        Name.Decorator: "#888",  # class: 'nd' - to be revised
+        Name.Entity: "#ce5c00",  # class: 'ni'
+        Name.Exception: "bold #cc0000",  # class: 'ne'
+        Name.Function: "#000000",  # class: 'nf'
+        Name.Property: "#000000",  # class: 'py'
+        Name.Label: "#f57900",  # class: 'nl'
+        Name.Namespace: "#000000",  # class: 'nn' - to be revised
+        Name.Other: "#000000",  # class: 'nx'
+        Name.Tag: "bold #004461",  # class: 'nt' - like a keyword
+        Name.Variable: "#000000",  # class: 'nv' - to be revised
+        Name.Variable.Class: "#000000",  # class: 'vc' - to be revised
+        Name.Variable.Global: "#000000",  # class: 'vg' - to be revised
+        Name.Variable.Instance: "#000000",  # class: 'vi' - to be revised
+        Number: "#990000",  # class: 'm'
+        Literal: "#000000",  # class: 'l'
+        Literal.Date: "#000000",  # class: 'ld'
+        String: "#4e9a06",  # class: 's'
+        String.Backtick: "#4e9a06",  # class: 'sb'
+        String.Char: "#4e9a06",  # class: 'sc'
+        String.Doc: "italic #8f5902",  # class: 'sd' - like a comment
+        String.Double: "#4e9a06",  # class: 's2'
+        String.Escape: "#4e9a06",  # class: 'se'
+        String.Heredoc: "#4e9a06",  # class: 'sh'
+        String.Interpol: "#4e9a06",  # class: 'si'
+        String.Other: "#4e9a06",  # class: 'sx'
+        String.Regex: "#4e9a06",  # class: 'sr'
+        String.Single: "#4e9a06",  # class: 's1'
+        String.Symbol: "#4e9a06",  # class: 'ss'
+        Generic: "#000000",  # class: 'g'
+        Generic.Deleted: "#a40000",  # class: 'gd'
+        Generic.Emph: "italic #000000",  # class: 'ge'
+        Generic.Error: "#ef2929",  # class: 'gr'
+        Generic.Heading: "bold #000080",  # class: 'gh'
+        Generic.Inserted: "#00A000",  # class: 'gi'
+        Generic.Output: "#888",  # class: 'go'
+        Generic.Prompt: "#745334",  # class: 'gp'
+        Generic.Strong: "bold #000000",  # class: 'gs'
+        Generic.Subheading: "bold #800080",  # class: 'gu'
+        Generic.Traceback: "bold #a40000",  # class: 'gt'
     }
```

### Comparing `fsps-0.4.3rc1/docs/conf.py` & `fsps-0.4.4rc1/docs/conf.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-from __future__ import (
-    division,
-    print_function,
-    absolute_import,
-    unicode_literals,
-)
-
 import os
 import sys
+from importlib.metadata import version as get_version
+from pathlib import Path
 
-# Patch the path to get the local version.
-d = os.path.dirname
-sys.path.insert(0, d(d(os.path.abspath(__file__))))
+if "SPS_HOME" not in os.environ:
+    path = Path(__file__).absolute()
+    sps_home = path.parent.parent / "src" / "fsps" / "libfsps"
+    os.environ["SPS_HOME"] = str(sps_home)
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
 ]
 
@@ -26,17 +22,16 @@
 exclude_patterns = ["_build", "_themes"]
 html_static_path = ["_static"]
 html_theme_path = ["_themes"]
 templates_path = ["_templates"]
 
 # General information about the project.
 project = "Python FSPS"
-copyright = "2013-2021 Python-FSPS developers"
-# version =
-# release =
+copyright = "2013-2023 Python-FSPS developers"
+version = get_version("fsps")
 
 html_show_sphinx = True
 html_show_sourcelink = False
 html_use_smartypants = True
 pygments_style = "sphinx"
 sys.path.append(os.path.abspath("_themes"))
 html_theme_path = ["_themes"]
```

### Comparing `fsps-0.4.3rc1/docs/filter_table.rst` & `fsps-0.4.4rc1/docs/filter_table.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,124 +1,124 @@
 === ================ ========== ======== =============== ========================================================================================
-ID  Name             M_sun Vega M_sun AB lambda_eff (Å)  Description                                                                             
+ID  Name             M_sun Vega M_sun AB lambda_eff (Å)  Description
 === ================ ========== ======== =============== ========================================================================================
-1   v                4.81       4.81     5477.6          Johnson V (from Bessell 1990 via M. Blanton) - this defines the Vega system             
-2   u                5.55       6.35     3584.8          Johnson U (from Bessell 1990 via M. Blanton)                                            
-3   b                5.46       5.35     4370.9          Johnson B (from Bessell 1990 via M. Blanton)                                            
-4   buser_b2         5.41       5.30     4433.5          Buser B2  (from BC03)                                                                   
-5   cousins_r        4.41       4.60     6576.9          Cousins R (from Bessell 1990 via M. Blanton)                                            
-6   cousins_i        4.10       4.52     7891.2          Cousins I (from Bessell 1990 via M. Blanton)                                            
-7   cfht_b           5.41       5.28     4418.6          CFHT B-band (from Blanton's kcorrect)                                                   
-8   cfht_r           4.37       4.59     6616.0          CFHT R-band (from Blanton's kcorrect)                                                   
-9   cfht_i           4.08       4.52     8166.0          CFHT I-band (from Blanton's kcorrect)                                                   
-10  2mass_j          3.67       4.56     12387.7         2MASS J filter (total response w/atm)                                                   
-11  2mass_h          3.34       4.70     16488.9         2MASS H filter (total response w/atm)                                                   
-12  2mass_ks         3.30       5.14     21635.6         2MASS Ks filter (total response w/atm)                                                  
-13  sdss_u           5.47       6.39     3556.5          SDSS Camera u Response Function, airmass = 1.3 (June 2001)                              
-14  sdss_g           5.23       5.12     4702.5          SDSS Camera g Response Function, airmass = 1.3 (June 2001)                              
-15  sdss_r           4.50       4.64     6175.6          SDSS Camera r Response Function, airmass = 1.3 (June 2001)                              
-16  sdss_i           4.18       4.53     7489.9          SDSS Camera i Response Function, airmass = 1.3 (June 2001)                              
-17  sdss_z           4.00       4.51     8946.8          SDSS Camera z Response Function, airmass = 1.3 (June 2001)                              
-18  wfpc2_f255w      7.44       9.06     2601.0          HST WFPC2 F255W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                    
-19  wfpc2_f300w      6.05       7.40     2994.3          HST WFPC2 F300W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                    
-20  wfpc2_f336w      5.46       6.64     3359.2          HST WFPC2 F336W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                    
-21  wfpc2_f439w      5.51       5.36     4311.7          HST WFPC2 F439W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                    
-22  wfpc2_f450w      5.31       5.22     4555.6          HST WFPC2 F450W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                    
-23  wfpc2_f555w      4.83       4.82     5438.9          HST WFPC2 F555W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                    
-24  wfpc2_f606w      4.61       4.70     5996.8          HST WFPC2 F606W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                    
-25  wfpc2_f814w      4.11       4.52     8012.3          HST WFPC2 F814W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                    
-26  wfpc2_f850lp     4.00       4.52     9129.0          HST WFPC2 F850LP (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                   
-27  wfc_acs_f435w    5.48       5.38     4318.1          HST ACS F435W  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                     
-28  wfc_acs_f475w    5.21       5.10     4744.3          HST ACS F475W  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                     
-29  wfc_acs_f555w    4.85       4.84     5359.5          HST ACS F555W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                      
-30  wfc_acs_f606w    4.64       4.72     5912.4          HST ACS F606W  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                     
-31  wfc_acs_f625w    4.47       4.63     6310.5          HST ACS F625W  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                     
-32  wfc_acs_f775w    4.14       4.53     7693.3          HST ACS F775W  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                     
-33  wfc_acs_f814w    4.10       4.52     8059.6          HST ACS F814W  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                     
-34  wfc_acs_f850lp   4.00       4.51     9054.5          HST ACS F850LP  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)                    
-35  wfc3_uvis_f218w  8.95       10.71    2226.5          HST WFC3 UVIS F218W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1    
-36  wfc3_uvis_f225w  8.37       10.10    2372.5          HST WFC3 UVIS F225W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1    
-37  wfc3_uvis_f275w  6.99       8.54     2710.1          HST WFC3 UVIS F275W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1    
-38  wfc3_uvis_f336w  5.47       6.65     3355.1          HST WFC3 UVIS F336W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1    
-39  wfc3_uvis_f390w  5.64       5.85     3924.4          HST WFC3 UVIS F390W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1    
-40  wfc3_uvis_f438w  5.49       5.34     4326.5          HST WFC3 UVIS F438W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1    
-41  wfc3_uvis_f475w  5.19       5.08     4773.7          HST WFC3 UVIS F475W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1    
-42  wfc3_uvis_f555w  4.89       4.86     5308.2          HST WFC3 UVIS F555W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1    
-43  wfc3_uvis_f606w  4.65       4.73     5887.4          HST WFC3 UVIS F606W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1    
-44  wfc3_uvis_f775w  4.15       4.53     7648.5          HST WFC3 UVIS F775W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1    
-45  wfc3_uvis_f814w  4.11       4.52     8029.5          HST WFC3 UVIS F814W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1    
-46  wfc3_uvis_f850lp 4.00       4.52     9168.9          HST WFC3 UVIS F850LP (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1   
-47  wfc3_ir_f098m    3.96       4.51     9862.9          HST WFC3 IR F098M (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_)              
-48  wfc3_ir_f105w    3.89       4.53     10550.7         HST WFC3 IR F105W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_)              
-49  wfc3_ir_f110w    3.79       4.54     11534.4         HST WFC3 IR F110W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_)              
-50  wfc3_ir_f125w    3.67       4.56     12486.1         HST WFC3 IR F125W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_)              
-51  wfc3_ir_f140w    3.52       4.60     13923.9         HST WFC3 IR F140W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_)              
-52  wfc3_ir_f160w    3.40       4.65     15370.8         HST WFC3 IR F160W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_)              
-53  irac_1           3.21       5.99     35569.7         Spitzer IRAC Channel 1 (3.6um)                                                          
-54  irac_2           3.16       6.41     45020.4         Spitzer IRAC Channel 2 (4.5um)                                                          
-55  irac_3           3.12       6.87     57454.1         Spitzer IRAC Channel 3 (5.8um)                                                          
-56  irac_4           3.09       7.47     79162.1         Spitzer IRAC Channel 4 (8.0um)                                                          
-57  isaac_ks         3.30       5.13     21622.1         ISAAC Ks                                                                                
-58  fors_v           4.78       4.79     5536.1          FORS V                                                                                  
-59  fors_r           4.41       4.60     6564.6          FORS R                                                                                  
-60  nicmos_f110w     3.82       4.54     11248.6         HST NICMOS F110W                                                                        
-61  nicmos_f160w     3.37       4.68     16060.4         HST NICMOS F160W                                                                        
-62  galex_fuv        14.91      17.24    1535.1          GALEX FUV                                                                               
-63  galex_nuv        8.41       10.15    2300.7          GALEX NUV                                                                               
-64  des_g            5.17       5.08     4800.9          DES g  (from Huan Lin, for DES camera)                                                  
-65  des_r            4.46       4.62     6362.6          DES r  (from Huan Lin, for DES camera)                                                  
-66  des_i            4.13       4.52     7750.1          DES i  (from Huan Lin, for DES camera)                                                  
-67  des_z            4.00       4.52     9153.7          DES z  (from Huan Lin, for DES camera)                                                  
-68  des_y            3.96       4.51     9907.8          DES Y  (from Huan Lin, for DES camera)                                                  
-69  wfcam_z          4.01       4.52     8826.3          WFCAM (UKIRT) Z  (from Hewett et al. 2006, via A. Smith)                                
-70  wfcam_y          3.91       4.51     10314.1         WFCAM (UKIRT) Y  (from Hewett et al. 2006, via A. Smith)                                
-71  wfcam_j          3.65       4.56     12500.9         WFCAM (UKIRT) J  (from Hewett et al. 2006, via A. Smith)                                
-72  wfcam_h          3.35       4.70     16359.1         WFCAM (UKIRT) H  (from Hewett et al. 2006, via A. Smith)                                
-73  wfcam_k          3.30       5.17     22084.0         WFCAM (UKIRT) K  (from Hewett et al. 2006, via A. Smith)                                
-74  steidel_un       5.44       6.34     3602.5          Steidel Un (via A. Shapley; see Steidel et al. 2003)                                    
-75  steidel_g        5.19       5.08     4753.2          Steidel G  (via A. Shapley; see Steidel et al. 2003)                                    
-76  steidel_rs       4.33       4.58     6781.4          Steidel Rs (via A. Shapley; see Steidel et al. 2003)                                    
-77  steidel_i        4.09       4.52     7985.7          Steidel I  (via A. Shapley; see Steidel et al. 2003)                                    
-78  megacam_u        5.68       6.03     3802.9          CFHT MegaCam u* (`<cadcwww.dao.nrc.ca/megapipe/docs/filters.html>`_, Dec 2010)          
-79  megacam_g        5.14       5.05     4844.4          CFHT MegaCam g' (`<cadcwww.dao.nrc.ca/megapipe/docs/filters.html>`_, Dec 2010)          
-80  megacam_r        4.48       4.63     6247.7          CFHT MegaCam r' (`<cadcwww.dao.nrc.ca/megapipe/docs/filters.html>`_, Dec 2010)          
-81  megacam_i        4.17       4.53     7538.7          CFHT MegaCam i' (`<cadcwww.dao.nrc.ca/megapipe/docs/filters.html>`_, Dec 2010)          
-82  megacam_z        4.00       4.51     8860.0          CFHT MegaCam z' (`<cadcwww.dao.nrc.ca/megapipe/docs/filters.html>`_, Dec 2010)          
-83  wise_w1          3.22       5.89     33682.1         WISE W1, 3.4um (`<http://www.astro.ucla.edu/~wright/WISE/passbands.html>`_)             
-84  wise_w2          3.16       6.45     46178.9         WISE W2, 4.6um (`<http://www.astro.ucla.edu/~wright/WISE/passbands.html>`_)             
-85  wise_w3          3.06       8.19     120717.6        WISE W3, 12um (`<http://www.astro.ucla.edu/~wright/WISE/passbands.html>`_)              
-86  wise_w4          3.01       9.62     221933.5        WISE W4, 22um (`<http://www.astro.ucla.edu/~wright/WISE/passbands.html>`_)              
-87  uvot_w2          8.47       10.29    2057.9          UVOT W2 (from Erik Hoversten, 2011)                                                     
-88  uvot_m2          8.84       10.60    2246.9          UVOT M2 (from Erik Hoversten, 2011)                                                     
-89  uvot_w1          6.91       8.47     2582.6          UVOT W1 (from Erik Hoversten, 2011)                                                     
-90  mips_24          3.00       9.74     235917.9        Spitzer MIPS 24um                                                                       
-91  mips_70          2.95       12.05    708981.4        Spitzer MIPS 70um                                                                       
-92  mips_160         2.92       13.78    1553640.7       Spitzer MIPS 160um                                                                      
-93  scuba_450wb      2.87       16.13    4561884.3       SCUBA 450WB (`<www.jach.hawaii.edu/JCMT/continuum/background/background.html>`_)        
-94  scuba_850wb      2.84       17.50    8563901.9       SCUBA 850WB (`<www.jach.hawaii.edu/JCMT/continuum/background/background.html>`_)        
-95  pacs_70          2.95       12.07    707688.0        Herschel PACS   70um                                                                    
-96  pacs_100         2.94       12.82    1007889.7       Herschel PACS  100um                                                                    
-97  pacs_160         2.92       13.81    1618854.2       Herschel PACS  160um                                                                    
-98  spire_250        2.90       14.78    2482638.8       Herschel SPIRE 250um                                                                    
-99  spire_350        2.88       15.52    3483962.4       Herschel SPIRE 350um                                                                    
-100 spire_500        2.86       16.27    5000972.5       Herschel SPIRE 500um                                                                    
-101 iras_12          3.06       8.05     110332.1        IRAS 12um                                                                               
-102 iras_25          3.01       9.62     230701.4        IRAS 25um                                                                               
-103 iras_60          2.97       11.50    581751.6        IRAS 60um                                                                               
-104 iras_100         2.94       12.77    994956.5        IRAS 100um                                                                              
-105 bessell_l        3.21       5.96     34800.1         Bessell L band  (Bessell & Brett 1988)                                                  
-106 bessell_lp       3.19       6.12     38275.9         Bessell L' band (Bessell & Brett 1988)                                                  
-107 bessell_m        3.15       6.51     47328.3         Bessell M band  (Bessell & Brett 1988)                                                  
-108 stromgren_u      5.34       6.47     3478.5          Stromgren u (Bessell 2011)                                                              
-109 stromgren_v      5.67       5.53     4107.9          Stromgren v (Bessell 2011)                                                              
-110 stromgren_b      5.22       5.06     4665.3          Stromgren b (Bessell 2011)                                                              
-111 stromgren_y      4.81       4.80     5459.0          Stromgren y (Bessell 2011)                                                              
-112 1500a            15.67      18.05    1498.5          Idealized 1500A bandpass with 15% bandwidth, FWHM = 225A from M. Dickinson              
-113 2300a            8.85       10.62    2297.7          Idealized 2300A bandpass with 15% bandwidth, FWHM = 345A from M. Dickinson              
-114 2800a            6.72       8.20     2797.1          Idealized 2800A bandpass with 15% bandwidth, FWHM = 420A from M. Dickinson              
+1   v                4.81       4.81     5477.6          Johnson V (from Bessell 1990 via M. Blanton) - this defines the Vega system
+2   u                5.55       6.35     3584.8          Johnson U (from Bessell 1990 via M. Blanton)
+3   b                5.46       5.35     4370.9          Johnson B (from Bessell 1990 via M. Blanton)
+4   buser_b2         5.41       5.30     4433.5          Buser B2  (from BC03)
+5   cousins_r        4.41       4.60     6576.9          Cousins R (from Bessell 1990 via M. Blanton)
+6   cousins_i        4.10       4.52     7891.2          Cousins I (from Bessell 1990 via M. Blanton)
+7   cfht_b           5.41       5.28     4418.6          CFHT B-band (from Blanton's kcorrect)
+8   cfht_r           4.37       4.59     6616.0          CFHT R-band (from Blanton's kcorrect)
+9   cfht_i           4.08       4.52     8166.0          CFHT I-band (from Blanton's kcorrect)
+10  2mass_j          3.67       4.56     12387.7         2MASS J filter (total response w/atm)
+11  2mass_h          3.34       4.70     16488.9         2MASS H filter (total response w/atm)
+12  2mass_ks         3.30       5.14     21635.6         2MASS Ks filter (total response w/atm)
+13  sdss_u           5.47       6.39     3556.5          SDSS Camera u Response Function, airmass = 1.3 (June 2001)
+14  sdss_g           5.23       5.12     4702.5          SDSS Camera g Response Function, airmass = 1.3 (June 2001)
+15  sdss_r           4.50       4.64     6175.6          SDSS Camera r Response Function, airmass = 1.3 (June 2001)
+16  sdss_i           4.18       4.53     7489.9          SDSS Camera i Response Function, airmass = 1.3 (June 2001)
+17  sdss_z           4.00       4.51     8946.8          SDSS Camera z Response Function, airmass = 1.3 (June 2001)
+18  wfpc2_f255w      7.44       9.06     2601.0          HST WFPC2 F255W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+19  wfpc2_f300w      6.05       7.40     2994.3          HST WFPC2 F300W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+20  wfpc2_f336w      5.46       6.64     3359.2          HST WFPC2 F336W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+21  wfpc2_f439w      5.51       5.36     4311.7          HST WFPC2 F439W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+22  wfpc2_f450w      5.31       5.22     4555.6          HST WFPC2 F450W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+23  wfpc2_f555w      4.83       4.82     5438.9          HST WFPC2 F555W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+24  wfpc2_f606w      4.61       4.70     5996.8          HST WFPC2 F606W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+25  wfpc2_f814w      4.11       4.52     8012.3          HST WFPC2 F814W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+26  wfpc2_f850lp     4.00       4.52     9129.0          HST WFPC2 F850LP (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+27  wfc_acs_f435w    5.48       5.38     4318.1          HST ACS F435W  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+28  wfc_acs_f475w    5.21       5.10     4744.3          HST ACS F475W  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+29  wfc_acs_f555w    4.85       4.84     5359.5          HST ACS F555W (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+30  wfc_acs_f606w    4.64       4.72     5912.4          HST ACS F606W  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+31  wfc_acs_f625w    4.47       4.63     6310.5          HST ACS F625W  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+32  wfc_acs_f775w    4.14       4.53     7693.3          HST ACS F775W  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+33  wfc_acs_f814w    4.10       4.52     8059.6          HST ACS F814W  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+34  wfc_acs_f850lp   4.00       4.51     9054.5          HST ACS F850LP  (`<http://acs.pha.jhu.edu/instrument/photometry/>`_)
+35  wfc3_uvis_f218w  8.95       10.71    2226.5          HST WFC3 UVIS F218W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1
+36  wfc3_uvis_f225w  8.37       10.10    2372.5          HST WFC3 UVIS F225W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1
+37  wfc3_uvis_f275w  6.99       8.54     2710.1          HST WFC3 UVIS F275W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1
+38  wfc3_uvis_f336w  5.47       6.65     3355.1          HST WFC3 UVIS F336W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1
+39  wfc3_uvis_f390w  5.64       5.85     3924.4          HST WFC3 UVIS F390W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1
+40  wfc3_uvis_f438w  5.49       5.34     4326.5          HST WFC3 UVIS F438W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1
+41  wfc3_uvis_f475w  5.19       5.08     4773.7          HST WFC3 UVIS F475W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1
+42  wfc3_uvis_f555w  4.89       4.86     5308.2          HST WFC3 UVIS F555W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1
+43  wfc3_uvis_f606w  4.65       4.73     5887.4          HST WFC3 UVIS F606W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1
+44  wfc3_uvis_f775w  4.15       4.53     7648.5          HST WFC3 UVIS F775W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1
+45  wfc3_uvis_f814w  4.11       4.52     8029.5          HST WFC3 UVIS F814W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1
+46  wfc3_uvis_f850lp 4.00       4.52     9168.9          HST WFC3 UVIS F850LP (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_) Chip #1
+47  wfc3_ir_f098m    3.96       4.51     9862.9          HST WFC3 IR F098M (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_)
+48  wfc3_ir_f105w    3.89       4.53     10550.7         HST WFC3 IR F105W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_)
+49  wfc3_ir_f110w    3.79       4.54     11534.4         HST WFC3 IR F110W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_)
+50  wfc3_ir_f125w    3.67       4.56     12486.1         HST WFC3 IR F125W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_)
+51  wfc3_ir_f140w    3.52       4.60     13923.9         HST WFC3 IR F140W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_)
+52  wfc3_ir_f160w    3.40       4.65     15370.8         HST WFC3 IR F160W (`<http://www.stsci.edu/~WFC3/UVIS/SystemThroughput/>`_)
+53  irac_1           3.21       5.99     35569.7         Spitzer IRAC Channel 1 (3.6um)
+54  irac_2           3.16       6.41     45020.4         Spitzer IRAC Channel 2 (4.5um)
+55  irac_3           3.12       6.87     57454.1         Spitzer IRAC Channel 3 (5.8um)
+56  irac_4           3.09       7.47     79162.1         Spitzer IRAC Channel 4 (8.0um)
+57  isaac_ks         3.30       5.13     21622.1         ISAAC Ks
+58  fors_v           4.78       4.79     5536.1          FORS V
+59  fors_r           4.41       4.60     6564.6          FORS R
+60  nicmos_f110w     3.82       4.54     11248.6         HST NICMOS F110W
+61  nicmos_f160w     3.37       4.68     16060.4         HST NICMOS F160W
+62  galex_fuv        14.91      17.24    1535.1          GALEX FUV
+63  galex_nuv        8.41       10.15    2300.7          GALEX NUV
+64  des_g            5.17       5.08     4800.9          DES g  (from Huan Lin, for DES camera)
+65  des_r            4.46       4.62     6362.6          DES r  (from Huan Lin, for DES camera)
+66  des_i            4.13       4.52     7750.1          DES i  (from Huan Lin, for DES camera)
+67  des_z            4.00       4.52     9153.7          DES z  (from Huan Lin, for DES camera)
+68  des_y            3.96       4.51     9907.8          DES Y  (from Huan Lin, for DES camera)
+69  wfcam_z          4.01       4.52     8826.3          WFCAM (UKIRT) Z  (from Hewett et al. 2006, via A. Smith)
+70  wfcam_y          3.91       4.51     10314.1         WFCAM (UKIRT) Y  (from Hewett et al. 2006, via A. Smith)
+71  wfcam_j          3.65       4.56     12500.9         WFCAM (UKIRT) J  (from Hewett et al. 2006, via A. Smith)
+72  wfcam_h          3.35       4.70     16359.1         WFCAM (UKIRT) H  (from Hewett et al. 2006, via A. Smith)
+73  wfcam_k          3.30       5.17     22084.0         WFCAM (UKIRT) K  (from Hewett et al. 2006, via A. Smith)
+74  steidel_un       5.44       6.34     3602.5          Steidel Un (via A. Shapley; see Steidel et al. 2003)
+75  steidel_g        5.19       5.08     4753.2          Steidel G  (via A. Shapley; see Steidel et al. 2003)
+76  steidel_rs       4.33       4.58     6781.4          Steidel Rs (via A. Shapley; see Steidel et al. 2003)
+77  steidel_i        4.09       4.52     7985.7          Steidel I  (via A. Shapley; see Steidel et al. 2003)
+78  megacam_u        5.68       6.03     3802.9          CFHT MegaCam u* (`<cadcwww.dao.nrc.ca/megapipe/docs/filters.html>`_, Dec 2010)
+79  megacam_g        5.14       5.05     4844.4          CFHT MegaCam g' (`<cadcwww.dao.nrc.ca/megapipe/docs/filters.html>`_, Dec 2010)
+80  megacam_r        4.48       4.63     6247.7          CFHT MegaCam r' (`<cadcwww.dao.nrc.ca/megapipe/docs/filters.html>`_, Dec 2010)
+81  megacam_i        4.17       4.53     7538.7          CFHT MegaCam i' (`<cadcwww.dao.nrc.ca/megapipe/docs/filters.html>`_, Dec 2010)
+82  megacam_z        4.00       4.51     8860.0          CFHT MegaCam z' (`<cadcwww.dao.nrc.ca/megapipe/docs/filters.html>`_, Dec 2010)
+83  wise_w1          3.22       5.89     33682.1         WISE W1, 3.4um (`<http://www.astro.ucla.edu/~wright/WISE/passbands.html>`_)
+84  wise_w2          3.16       6.45     46178.9         WISE W2, 4.6um (`<http://www.astro.ucla.edu/~wright/WISE/passbands.html>`_)
+85  wise_w3          3.06       8.19     120717.6        WISE W3, 12um (`<http://www.astro.ucla.edu/~wright/WISE/passbands.html>`_)
+86  wise_w4          3.01       9.62     221933.5        WISE W4, 22um (`<http://www.astro.ucla.edu/~wright/WISE/passbands.html>`_)
+87  uvot_w2          8.47       10.29    2057.9          UVOT W2 (from Erik Hoversten, 2011)
+88  uvot_m2          8.84       10.60    2246.9          UVOT M2 (from Erik Hoversten, 2011)
+89  uvot_w1          6.91       8.47     2582.6          UVOT W1 (from Erik Hoversten, 2011)
+90  mips_24          3.00       9.74     235917.9        Spitzer MIPS 24um
+91  mips_70          2.95       12.05    708981.4        Spitzer MIPS 70um
+92  mips_160         2.92       13.78    1553640.7       Spitzer MIPS 160um
+93  scuba_450wb      2.87       16.13    4561884.3       SCUBA 450WB (`<www.jach.hawaii.edu/JCMT/continuum/background/background.html>`_)
+94  scuba_850wb      2.84       17.50    8563901.9       SCUBA 850WB (`<www.jach.hawaii.edu/JCMT/continuum/background/background.html>`_)
+95  pacs_70          2.95       12.07    707688.0        Herschel PACS   70um
+96  pacs_100         2.94       12.82    1007889.7       Herschel PACS  100um
+97  pacs_160         2.92       13.81    1618854.2       Herschel PACS  160um
+98  spire_250        2.90       14.78    2482638.8       Herschel SPIRE 250um
+99  spire_350        2.88       15.52    3483962.4       Herschel SPIRE 350um
+100 spire_500        2.86       16.27    5000972.5       Herschel SPIRE 500um
+101 iras_12          3.06       8.05     110332.1        IRAS 12um
+102 iras_25          3.01       9.62     230701.4        IRAS 25um
+103 iras_60          2.97       11.50    581751.6        IRAS 60um
+104 iras_100         2.94       12.77    994956.5        IRAS 100um
+105 bessell_l        3.21       5.96     34800.1         Bessell L band  (Bessell & Brett 1988)
+106 bessell_lp       3.19       6.12     38275.9         Bessell L' band (Bessell & Brett 1988)
+107 bessell_m        3.15       6.51     47328.3         Bessell M band  (Bessell & Brett 1988)
+108 stromgren_u      5.34       6.47     3478.5          Stromgren u (Bessell 2011)
+109 stromgren_v      5.67       5.53     4107.9          Stromgren v (Bessell 2011)
+110 stromgren_b      5.22       5.06     4665.3          Stromgren b (Bessell 2011)
+111 stromgren_y      4.81       4.80     5459.0          Stromgren y (Bessell 2011)
+112 1500a            15.67      18.05    1498.5          Idealized 1500A bandpass with 15% bandwidth, FWHM = 225A from M. Dickinson
+113 2300a            8.85       10.62    2297.7          Idealized 2300A bandpass with 15% bandwidth, FWHM = 345A from M. Dickinson
+114 2800a            6.72       8.20     2797.1          Idealized 2800A bandpass with 15% bandwidth, FWHM = 420A from M. Dickinson
 115 jwst_f070w       nan        nan      nan             JWST F070W (`<http://www.stsci.edu/jwst/instruments/nircam/instrumentdesign/filters/>`_)
 116 jwst_f090w       nan        nan      nan             JWST F090W (`<http://www.stsci.edu/jwst/instruments/nircam/instrumentdesign/filters/>`_)
 117 jwst_f115w       nan        nan      nan             JWST F115W (`<http://www.stsci.edu/jwst/instruments/nircam/instrumentdesign/filters/>`_)
 118 jwst_f150w       nan        nan      nan             JWST F150W (`<http://www.stsci.edu/jwst/instruments/nircam/instrumentdesign/filters/>`_)
 119 jwst_f200w       nan        nan      nan             JWST F200W (`<http://www.stsci.edu/jwst/instruments/nircam/instrumentdesign/filters/>`_)
 120 jwst_f277w       nan        nan      nan             JWST F277W (`<http://www.stsci.edu/jwst/instruments/nircam/instrumentdesign/filters/>`_)
 121 jwst_f356w       nan        nan      nan             JWST F356W (`<http://www.stsci.edu/jwst/instruments/nircam/instrumentdesign/filters/>`_)
```

### Comparing `fsps-0.4.3rc1/docs/filters_api.rst` & `fsps-0.4.4rc1/docs/filters_api.rst`

 * *Files identical despite different names*

### Comparing `fsps-0.4.3rc1/docs/index.rst` & `fsps-0.4.4rc1/docs/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 .. include:: ../AUTHORS.rst
 
 
 License
 -------
 
-*Copyright 2013-2021 Python-FSPS developers.*
+*Copyright 2013-2023 Python-FSPS developers.*
 
 These bindings are available under the `MIT License
 <https://raw.github.com/dfm/python-fsps/main/LICENSE.rst>`_.
 
 If you make use of this code, please reference these Python bindings,
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.591505.svg
```

### Comparing `fsps-0.4.3rc1/docs/installation.rst` & `fsps-0.4.4rc1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `fsps-0.4.3rc1/docs/stellarpop_api.rst` & `fsps-0.4.4rc1/docs/stellarpop_api.rst`

 * *Files identical despite different names*

### Comparing `fsps-0.4.3rc1/noxfile.py` & `fsps-0.4.4rc1/noxfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 import os
 from pathlib import Path
 
 import nox
 
-ALL_PYTHON_VS = ["3.8", "3.9", "3.10"]
+ALL_PYTHON_VS = ["3.8", "3.9", "3.10", "3.11"]
 
 
-def _run_with_sps_home(session, *args, **kwargs):
+def _run_with_sps_home(session: nox.Session, *args, **kwargs):
     sps_home = os.environ.get(
         "SPS_HOME", Path(__file__).parent / "src" / "fsps" / "libfsps"
     )
     kwargs["env"] = dict(kwargs.get("env", {}), SPS_HOME=str(sps_home))
-    return session.run(*args, **kwargs)
+    return session.run(*args, **kwargs, external=True)
 
 
 @nox.session(python=ALL_PYTHON_VS)
 def tests(session):
     session.install(".[test]")
     _run_with_sps_home(session, "python", "tests/simple.py")
     _run_with_sps_home(
         session,
         "python",
         "-m",
         "pytest",
         "-n",
         "2",
         "--durations=0",
-        "-v",
         "tests/tests.py",
     )
 
 
 @nox.session(python=ALL_PYTHON_VS)
 def options(session):
     session.install(
```

### Comparing `fsps-0.4.3rc1/scripts/fsps_filter_table.py` & `fsps-0.4.4rc1/scripts/fsps_filter_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,63 +3,72 @@
 """
 Print a table of filters implemented by FSPS.
 
 The table is formatted in restructured text for use with the python-fsps's
 Sphinx documentation.
 """
 
-from __future__ import print_function, absolute_import
+from __future__ import absolute_import, print_function
 
 import re
+
 import fsps
 
 # Pattern via https://gist.github.com/uogbuji/705383
-URL_P = re.compile(ur'(?i)\b((?:https?://|www\d{0,3}[.]|[a-z0-9.\-]+[.][a-z]{2,4}/)(?:[^\s()<>]+|\(([^\s()<>]+|(\([^\s()<>]+\)))*\))+(?:\(([^\s()<>]+|(\([^\s()<>]+\)))*\)|[^\s`!()\[\]{};:\'".,<>?\xab\xbb\u201c\u201d\u2018\u2019]))')  # NOQA
+URL_P = re.compile(
+    r'(?i)\b((?:https?://|www\d{0,3}[.]|[a-z0-9.\-]+[.][a-z]{2,4}/)(?:[^\s()<>]+|\(([^\s()<>]+|(\([^\s()<>]+\)))*\))+(?:\(([^\s()<>]+|(\([^\s()<>]+\)))*\)|[^\s`!()\[\]{};:\'".,<>?\xab\xbb\u201c\u201d\u2018\u2019]))'
+)
 
 
 def main():
-    colnames = ("ID", "Name", "M_sun Vega", "M_sun AB", "lambda_eff (Å)",
-                "Description")
+    colnames = ("ID", "Name", "M_sun Vega", "M_sun AB", "lambda_eff (Å)", "Description")
     filters = [fsps.get_filter(name) for name in fsps.list_filters()]
     filter_list = make_filter_list(filters)
     txt = make_table(filter_list, colnames)
     print(txt)
 
 
 def make_filter_list(filters):
     """Transform filters into list of table rows."""
     filter_list = []
     filter_ids = []
     for f in filters:
         filter_ids.append(f.index)
-        fullname = URL_P.sub(r'`<\1>`_', f.fullname)
-        filter_list.append((str(f.index + 1),
-                            f.name,
-                            "{0:.2f}".format(f.msun_vega),
-                            "{0:.2f}".format(f.msun_ab),
-                            "{0:.1f}".format(f.lambda_eff),
-                            fullname))
-    sortf = lambda item: int(item[0])
+        fullname = URL_P.sub(r"`<\1>`_", f.fullname)
+        filter_list.append(
+            (
+                str(f.index + 1),
+                f.name,
+                "{0:.2f}".format(f.msun_vega),
+                "{0:.2f}".format(f.msun_ab),
+                "{0:.1f}".format(f.lambda_eff),
+                fullname,
+            )
+        )
+
+    def sortf(item):
+        return int(item[0])
+
     filter_list.sort(key=sortf)
     return filter_list
 
 
 def make_table(data, col_names):
     """Code for this RST-formatted table generator comes from
     http://stackoverflow.com/a/11350643
     """
     n_cols = len(data[0])
     assert n_cols == len(col_names)
     col_sizes = [max(len(r[i]) for r in data) for i in range(n_cols)]
     for i, cname in enumerate(col_names):
         if col_sizes[i] < len(cname):
             col_sizes[i] = len(cname)
-    formatter = ' '.join('{:<%d}' % c for c in col_sizes)
-    rows = '\n'.join([formatter.format(*row) for row in data])
+    formatter = " ".join("{:<%d}" % c for c in col_sizes)
+    rows = "\n".join([formatter.format(*row) for row in data])
     header = formatter.format(*col_names)
-    divider = formatter.format(*['=' * c for c in col_sizes])
-    output = '\n'.join((divider, header, divider, rows, divider))
+    divider = formatter.format(*["=" * c for c in col_sizes])
+    output = "\n".join((divider, header, divider, rows, divider))
     return output
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `fsps-0.4.3rc1/src/fsps/filters.py` & `fsps-0.4.4rc1/src/fsps/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 This module uses filter information shipped with FSPS itself in
 ``$SPS_HOME/data``.
 """
 
 __all__ = ["find_filter", "FILTERS", "get_filter", "list_filters"]
 
 import os
+
 import numpy as np
 
 # Cache for $SPS_HOME/data/magsun.dat parsed by numpy
 MSUN_TABLE = None
 
 # Cache for $SPS_HOME/data/filter_lambda_eff.dat parsed by numpy
 LAMBDA_EFF_TABLE = None
@@ -113,15 +114,15 @@
                     filter_index += 1
                     lambdas, trans = [], []
                 else:
                     try:
                         l, t = line.split()
                         lambdas.append(float(l))
                         trans.append(float(t))
-                    except (ValueError):
+                    except ValueError:
                         pass
         # Close out the last filter
         TRANS_CACHE[names[filter_index]] = (np.array(lambdas), np.array(trans))
 
 
 def _load_filter_dict():
     """
```

### Comparing `fsps-0.4.3rc1/src/fsps/fsps.f90` & `fsps-0.4.4rc1/src/fsps/fsps.f90`

 * *Files 1% similar despite different names*

```diff
@@ -376,14 +376,27 @@
     implicit none
     integer, intent(in) :: n_age,n_z
     double precision, dimension(n_age,n_z), intent(inout) :: ssp_wghts_out
     ssp_wghts_out = weight_ssp
 
   end subroutine
 
+  subroutine get_csp_components(ns, csp1, csp2)
+
+    ! Return the unattenuated 'young' and 'old' stellar continuua
+
+    implicit none
+    integer, intent(in) :: ns
+    double precision, dimension(ns), intent(inout) :: csp1, csp2
+    csp1 = spec_young
+    csp2 = spec_old
+
+  end subroutine
+
+
   subroutine get_ssp_spec(ns,n_age,n_z,ssp_spec_out,ssp_mass_out,ssp_lbol_out)
 
     ! Return the contents of the ssp spectral array,
     ! regenerating the ssps if necessary
 
     implicit none
     integer, intent(in) :: ns,n_age,n_z
```

### Comparing `fsps-0.4.3rc1/src/fsps/fsps.py` & `fsps-0.4.4rc1/src/fsps/fsps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 __all__ = ["StellarPopulation"]
 
 import os
+
 import numpy as np
 
 from fsps._fsps import driver
 from fsps.filters import FILTERS
 
 
 class StellarPopulation(object):
@@ -93,16 +94,16 @@
         Gyr) at every wavelength, the returned magnitudes are filter
         transmission weighted averages of these, the ``log_lbol`` attribute is
         the bolometric luminosity weighted age, and the ``stellar_mass``
         attribute gives the mass-weighted age.
 
     :param nebemlineinspec: (default: True)
         Flag to include the emission line fluxes in the spectrum. Turning this off
-        is a significant speedup in model calculation time. If not set, the line luminosities
-        are still computed.
+        is a significant speedup in model calculation time. If not set, the line
+        luminosities are still computed.
 
     :param smooth_velocity: (default: True)
         Switch to choose smoothing in velocity space (``True``) or wavelength
         space.
 
     :param smooth_lsf: (default: False)
         Switch to apply smoothing of the SSPs by a wavelength dependent line
@@ -214,16 +215,17 @@
         M_\odot`. Only used if ``imf_type=2``.
 
     :param imf2: (default: 2.3)
         Logarithmic slope of the IMF over the range :math:`0.5 < M < 1
         M_\odot`. Only used if ``imf_type=2``.
 
     :param imf3: (default: 2.3)
-        Logarithmic slope of the IMF over the range :math:`1.0 < M < \mathrm{imf\_upper\_limit}
-        M_\odot`. Only used if ``imf_type=2``.
+        Logarithmic slope of the IMF over the range
+        :math:`1.0 < M < \mathrm{imf\_upper\_limit} M_\odot`.
+        Only used if ``imf_type=2``.
 
     :param vdmc: (default: 0.08)
         IMF parameter defined in van Dokkum (2008). Only used if
         ``imf_type=3``.
 
     :param mdave: (default: 0.5)
         IMF parameter defined in Dave (2008). Only used if ``imf_type=4``.
@@ -442,15 +444,14 @@
         SED.  Outside the range (5, 150) the AGN SED is an
         extrapolation.
     """
 
     def __init__(
         self, compute_vega_mags=False, vactoair_flag=False, zcontinuous=0, **kwargs
     ):
-
         # Set up the parameters to their default values.
         self.params = ParameterSet(
             add_agb_dust_model=True,
             add_dust_emission=True,
             add_igm_absorption=False,
             add_neb_emission=False,
             add_neb_continuum=True,
@@ -605,15 +606,15 @@
             self.params["zmet"] = zmet
 
         if self.params.dirty:
             self._compute_csp()
 
         wavegrid = self.wavelengths
         if peraa:
-            factor = 3e18 / wavegrid ** 2
+            factor = 3e18 / wavegrid**2
 
         else:
             factor = np.ones_like(wavegrid)
 
         NSPEC = driver.get_nspec()
         if (tage > 0.0) or (tage == -99):
             return wavegrid, driver.get_spec(NSPEC, 1)[0] * factor
@@ -689,19 +690,18 @@
         mags = driver.get_mags(NSPEC, NTFULL, zr, inds)
 
         if tage > 0.0:
             if bands is not None:
                 return mags[0, user_sorted_inds]
             else:
                 return mags[0, :]
+        elif bands is not None:
+            return mags[:, user_sorted_inds]
         else:
-            if bands is not None:
-                return mags[:, user_sorted_inds]
-            else:
-                return mags
+            return mags
 
     def _ztinterp(self, zpos, tpos, peraa=False):
         r"""
         Return an SSP spectrum, mass, and luminosity interpolated to a target
         metallicity and age.  This effectively wraps the ZTINTERP subroutine.
         Only the SSPs bracketing a given metallicity will be regenerated, if
         parameters are dirty.
@@ -731,15 +731,15 @@
         NSPEC = driver.get_nspec()
         spec, mass, lbol = np.zeros(NSPEC), np.zeros(1), np.zeros(1)
         logt_yrs = np.log10(tpos * 1e9)
         driver.interp_ssp(zpos, logt_yrs, spec, mass, lbol)
 
         if peraa:
             wavegrid = self.wavelengths
-            factor = 3e18 / wavegrid ** 2
+            factor = 3e18 / wavegrid**2
             spec *= factor
 
         return spec, mass, lbol
 
     def _all_ssp_spec(self, update=True, peraa=False):
         r"""
         Return the contents of the ssp_spec_zz array.
@@ -772,33 +772,50 @@
         spec = np.zeros([NSPEC, NTFULL, NZ], order="F")
         mass = np.zeros([NTFULL, NZ], order="F")
         lbol = np.zeros([NTFULL, NZ], order="F")
         driver.get_ssp_spec(spec, mass, lbol)
 
         if peraa:
             wavegrid = self.wavelengths
-            factor = 3e18 / wavegrid ** 2
+            factor = 3e18 / wavegrid**2
             spec *= factor[:, None, None]
 
         return spec, mass, lbol
 
+    @property
+    def _csp_young_old(self):
+        """Get the (unattenuated) young and old component spectra of the CSP
+
+        :returns young:
+            The young stellar spectrum
+
+        :returns old:
+            The old stellar spectrum
+        """
+
+        NS = driver.get_nspec()
+        young, old = np.zeros(NS), np.zeros(NS)
+        driver.get_csp_components(young, old)
+        return young, old
+
+    @property
     def _ssp_weights(self):
-         """Get the weights of the SSPs for the CSP
+        r"""Get the weights of the SSPs for the CSP
+
+        :returns weights:
+            The weights ``w`` of each SSP s.t. the total spectrum is the sum
+            :math:`L_{\lambda} = \sum_i,j w_i,j \, S_{i,j,\lambda}` where
+            math:`i,j` run over age and metallicity.
+        """
 
-         :returns weights:
-             The weights ``w`` of each SSP s.t. the total spectrum is the sum
-             :math:`L_{\lambda} = \sum_i,j w_i,j \, S_{i,j,\lambda}` where
-             math:`i,j` run over age and metallicity.
-         """
-
-         NTFULL = driver.get_ntfull()
-         NZ = driver.get_nz()
-         weights = np.zeros([NTFULL, NZ], order="F")
-         driver.get_ssp_weights(weights)
-         return weights
+        NTFULL = driver.get_ntfull()
+        NZ = driver.get_nz()
+        weights = np.zeros([NTFULL, NZ], order="F")
+        driver.get_ssp_weights(weights)
+        return weights
 
     def _get_stellar_spectrum(
         self,
         mact,
         logt,
         lbol,
         logg,
@@ -854,15 +871,15 @@
         NSPEC = driver.get_nspec()
         outspec = np.zeros(NSPEC)
         driver.stellar_spectrum(
             mact, logt, lbol, logg, phase, comp, mdot, weight, outspec
         )
         if peraa:
             wavegrid = self.wavelengths
-            factor = 3e18 / wavegrid ** 2
+            factor = 3e18 / wavegrid**2
             outspec *= factor
 
         return outspec
 
     def isochrones(self, outfile="pyfsps_tmp"):
         r"""
         Write the isochrone data (age, mass, weights, phases, magnitudes, etc.)
@@ -1061,16 +1078,16 @@
             NSPEC = driver.get_nspec()
             self._wavelengths = driver.get_lambda(NSPEC)
         return self._wavelengths.copy()
 
     @property
     def resolutions(self):
         r"""The resolution array, in km/s dispersion. Negative numbers indicate
-         poorly defined, approximate, resolution (based on coarse opacity
-         binning in theoretical spectra)"""
+        poorly defined, approximate, resolution (based on coarse opacity
+        binning in theoretical spectra)"""
         if self._resolutions is None:
             NSPEC = driver.get_nspec()
             self._resolutions = driver.get_res(NSPEC)
         return self._resolutions.copy()
 
     @property
     def emline_wavelengths(self):
@@ -1210,15 +1227,16 @@
             * (1 - self.params["const"] - (tb < tmax) * self.params["fburst"])
             + self.params["const"] * normalized_times / tmax
             + burst_in_past * self.params["fburst"]
         )
 
         avsfr = (mass[..., 0] - mass[..., 1]) / dt / 1e9  # Msun/yr
 
-        # These lines change behavior when you request sfrs outside the range (sf_start + dt, tage)
+        # These lines change behavior when you request sfrs outside the range
+        # (sf_start + dt, tage)
         # avsfr[times > tage] = np.nan  # does not work for scalars
         avsfr *= times <= tage
         # avsfr[np.isfinite(avsfr)] = 0.0 # does not work for scalars
 
         return np.clip(avsfr, 0, np.inf)
 
     @property
@@ -1240,15 +1258,14 @@
     def libraries(self):
         if self._libraries is None:
             self._libraries = driver.get_libraries()
         return self._libraries
 
 
 class ParameterSet(object):
-
     ssp_params = [
         "imf_type",
         "imf_upper_limit",
         "imf_lower_limit",
         "imf1",
         "imf2",
         "imf3",
```

### Comparing `fsps-0.4.3rc1/src/fsps/sps_home.py` & `fsps-0.4.4rc1/src/fsps/sps_home.py`

 * *Files identical despite different names*

### Comparing `fsps-0.4.3rc1/tests/tests.py` & `fsps-0.4.4rc1/tests/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- coding: utf-8 -*-
 
 import os
 import sys
+
 import numpy as np
 import pytest
-from fsps import StellarPopulation, filters
 from numpy.testing import assert_allclose
 
+from fsps import StellarPopulation, filters
+
 skip_slow_tests = pytest.mark.skipif(
     (sys.platform.startswith("win") or sys.platform.startswith("darwin"))
     and "CI" in os.environ,
     reason="Slow tests only run on Linux CI",
 )
 
 
@@ -32,15 +34,15 @@
     """Just test that `isochrones()` method runs"""
 
     # recomputes SSPs
 
     pop, params = pop_and_params
     _reset_default_params(pop, params)
     pop.params["imf_type"] = 0
-    iso = pop.isochrones()
+    pop.isochrones()
 
 
 @skip_slow_tests
 def test_imf3(pop_and_params):
     """Make sure that changing the (upper) imf changes the parameter dirtiness
     and also the SSP spectrum"""
 
@@ -64,15 +66,14 @@
     w, model1b = pop.get_spectrum(tage=0.2)
     assert pop.params.dirtiness == 0
 
     assert_allclose(model1 / model1b - 1.0, 0.0)
 
 
 def test_param_checks(pop_and_params):
-
     # recomputes SSPs
 
     pop, params = pop_and_params
     _reset_default_params(pop, params)
     pop.params["sfh"] = 1
     pop.params["tage"] = 2
     pop.params["sf_start"] = 0.5
@@ -88,15 +89,14 @@
         w, s = pop.get_spectrum(tage=pop.params["tage"])
     pop.params["tage"] = 1.0
     pop.params["sf_start"] = 0.1
     w, s = pop.get_spectrum(tage=pop.params["tage"])
 
 
 def test_smooth_lsf(pop_and_params):
-
     # recomputes SSPs
 
     pop, params = pop_and_params
     _reset_default_params(pop, params)
     tmax = 1.0
     wave_lsf = np.arange(4000, 7000.0, 10)
     x = (wave_lsf - 5500) / 1500.0
@@ -381,24 +381,25 @@
 
     # uses default SSPs
 
     pop, params = pop_and_params
     _reset_default_params(pop, params)
 
     import os
+
     fn = os.path.join(os.environ["SPS_HOME"], "data/sfh.dat")
     age, sfr, z = np.genfromtxt(fn, unpack=True, skip_header=0)
     pop.params["sfh"] = 3
     pop.set_tabular_sfh(age, sfr)
     zind = -3
-    pop.params["logzsol"] = np.log10(pop.zlegend[zind]/pop.solar_metallicity)
+    pop.params["logzsol"] = np.log10(pop.zlegend[zind] / pop.solar_metallicity)
 
     wave, spec = pop.get_spectrum(tage=age.max())
     mstar = pop.stellar_mass
-    wght = pop._ssp_weights()
+    wght = pop._ssp_weights
     ssp, smass, slbol = pop._all_ssp_spec()
 
     assert np.allclose((smass[:, zind] * wght[:, 0]).sum(), mstar)
 
 
 # Requires scipy
 # def test_sfr_avg():
```

### Comparing `fsps-0.4.3rc1/PKG-INFO` & `fsps-0.4.4rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: fsps
-Version: 0.4.3rc1
+Version: 0.4.4rc1
 Summary: Python bindings for Charlie Conroy's FSPS
 Author-Email: Dan Foreman-Mackey <foreman.mackey@gmail.com>
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Project-URL: Homepage, https://dfm.io/python-fsps
 Project-URL: Source, https://github.com/dfm/python-fsps
 Project-URL: Bug tracker, https://github.com/dfm/python-fsps/issues
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Requires-Dist: numpy
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Provides-Extra: test
 Description-Content-Type: text/x-rst
 
 .. image:: https://github.com/dfm/python-fsps/workflows/Tests/badge.svg
```

