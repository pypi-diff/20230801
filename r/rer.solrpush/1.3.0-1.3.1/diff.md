# Comparing `tmp/rer.solrpush-1.3.0.tar.gz` & `tmp/rer.solrpush-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rer.solrpush-1.3.0.tar", last modified: Thu Sep 29 15:18:38 2022, max compression
+gzip compressed data, was "rer.solrpush-1.3.1.tar", last modified: Tue Aug  1 09:12:43 2023, max compression
```

## Comparing `rer.solrpush-1.3.0.tar` & `rer.solrpush-1.3.1.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.191344 rer.solrpush-1.3.0/
--rw-r--r--   0 cekk       (501) staff       (20)     4159 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       67 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      652 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      525 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)    16361 2022-09-29 15:18:38.191615 rer.solrpush-1.3.0/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     7496 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)      171 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/docker-compose.yml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.155384 rer.solrpush-1.3.0/docs/
--rw-r--r--   0 cekk       (501) staff       (20)   213611 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/docs/Solr-Push_Configurazione.jpg
--rw-r--r--   0 cekk       (501) staff       (20)     7885 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)       59 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)    32560 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/docs/rer-logo.png
--rw-r--r--   0 cekk       (501) staff       (20)     3432 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/publiccode.yml
--rw-r--r--   0 cekk       (501) staff       (20)      321 2022-09-29 15:18:38.192134 rer.solrpush-1.3.0/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2586 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.146141 rer.solrpush-1.3.0/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.155770 rer.solrpush-1.3.0/src/rer/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.160505 rer.solrpush-1.3.0/src/rer/solrpush/
--rw-r--r--   0 cekk       (501) staff       (20)      130 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.161251 rer.solrpush-1.3.0/src/rer/solrpush/adapters/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/adapters/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      282 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/adapters/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1439 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/adapters/file.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.161959 rer.solrpush-1.3.0/src/rer/solrpush/behaviors/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/behaviors/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      458 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/behaviors/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1148 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/behaviors/solr_fields.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.163935 rer.solrpush-1.3.0/src/rer/solrpush/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     3421 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     3304 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/controlpanel.py
--rw-r--r--   0 cekk       (501) staff       (20)     1205 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/elevate_settings.py
--rw-r--r--   0 cekk       (501) staff       (20)    16058 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/maintenance.py
--rw-r--r--   0 cekk       (501) staff       (20)      350 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/query_debug.py
--rw-r--r--   0 cekk       (501) staff       (20)     6247 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/querybuilder.py
--rw-r--r--   0 cekk       (501) staff       (20)     2322 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/scales.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.165480 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/.gitkeep
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.147264 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/dist/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.168904 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/dist/dev/
--rw-r--r--   0 cekk       (501) staff       (20)  2311368 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/dist/dev/main.js
--rw-r--r--   0 cekk       (501) staff       (20)  1783747 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/dist/dev/main.js.map
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.172447 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/dist/prod/
--rw-r--r--   0 cekk       (501) staff       (20)   294024 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/dist/prod/main.js
--rw-r--r--   0 cekk       (501) staff       (20)      159 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/dist/prod/main.js.map
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.172733 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/javascripts/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.173005 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/javascripts/FacetsContainer/
--rw-r--r--   0 cekk       (501) staff       (20)     1025 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/javascripts/FacetsContainer/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.173274 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/javascripts/ProgressBar/
--rw-r--r--   0 cekk       (501) staff       (20)      946 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/javascripts/ProgressBar/index.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.173558 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/javascripts/ProgressBarContainer/
--rw-r--r--   0 cekk       (501) staff       (20)     1737 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/javascripts/ProgressBarContainer/index.js
--rw-r--r--   0 cekk       (501) staff       (20)      455 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/javascripts/index.js
--rw-r--r--   0 cekk       (501) staff       (20)      258 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/package.json
--rw-r--r--   0 cekk       (501) staff       (20)      618 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/styles.css
--rw-r--r--   0 cekk       (501) staff       (20)      174 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/styles.css.map
--rw-r--r--   0 cekk       (501) staff       (20)      431 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/styles.scss
--rw-r--r--   0 cekk       (501) staff       (20)    57992 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/static/yarn.lock
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.174334 rer.solrpush-1.3.0/src/rer/solrpush/browser/templates/
--rw-r--r--   0 cekk       (501) staff       (20)     1822 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/templates/controlpanel_layout.pt
--rw-r--r--   0 cekk       (501) staff       (20)      498 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/templates/query_debug.pt
--rw-r--r--   0 cekk       (501) staff       (20)     1453 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/browser/templates/reindex_solr.pt
--rw-r--r--   0 cekk       (501) staff       (20)     2423 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     4078 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/indexer.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.175839 rer.solrpush-1.3.0/src/rer/solrpush/interfaces/
--rw-r--r--   0 cekk       (501) staff       (20)      282 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/interfaces/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      307 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/interfaces/adapter.py
--rw-r--r--   0 cekk       (501) staff       (20)     3344 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/interfaces/elevate.py
--rw-r--r--   0 cekk       (501) staff       (20)      197 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/interfaces/layer.py
--rw-r--r--   0 cekk       (501) staff       (20)      153 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/interfaces/queueprocessor.py
--rw-r--r--   0 cekk       (501) staff       (20)     6735 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/interfaces/settings.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.177201 rer.solrpush-1.3.0/src/rer/solrpush/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/locales/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.148532 rer.solrpush-1.3.0/src/rer/solrpush/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.177744 rer.solrpush-1.3.0/src/rer/solrpush/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)      458 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/locales/en/LC_MESSAGES/rer.solrpush.mo
--rw-r--r--   0 cekk       (501) staff       (20)    11576 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/locales/en/LC_MESSAGES/rer.solrpush.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.148779 rer.solrpush-1.3.0/src/rer/solrpush/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.178266 rer.solrpush-1.3.0/src/rer/solrpush/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     9126 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.mo
--rw-r--r--   0 cekk       (501) staff       (20)    16564 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.po
--rw-r--r--   0 cekk       (501) staff       (20)    11694 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/locales/rer.solrpush.pot
--rw-r--r--   0 cekk       (501) staff       (20)     1528 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      473 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)     5977 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/parser.py
--rw-r--r--   0 cekk       (501) staff       (20)      424 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.149899 rer.solrpush-1.3.0/src/rer/solrpush/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.179940 rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      854 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/actions.xml
--rw-r--r--   0 cekk       (501) staff       (20)      162 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      105 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      953 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      257 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/metadata.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.180717 rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/registry/
--rw-r--r--   0 cekk       (501) staff       (20)      891 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/registry/bundle.xml
--rw-r--r--   0 cekk       (501) staff       (20)     2828 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/registry/criteria.xml
--rw-r--r--   0 cekk       (501) staff       (20)      278 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/registry/settings.xml
--rw-r--r--   0 cekk       (501) staff       (20)      387 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.180985 rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/types/
--rw-r--r--   0 cekk       (501) staff       (20)      299 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/types/Document.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.181495 rer.solrpush-1.3.0/src/rer/solrpush/profiles/to_1100/
--rw-r--r--   0 cekk       (501) staff       (20)      232 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/to_1100/componentregistry.xml
--rw-r--r--   0 cekk       (501) staff       (20)       97 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/to_1100/metadata.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.182005 rer.solrpush-1.3.0/src/rer/solrpush/profiles/to_1300/
--rw-r--r--   0 cekk       (501) staff       (20)      322 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/to_1300/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      211 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/to_1300/registry.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.182766 rer.solrpush-1.3.0/src/rer/solrpush/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      122 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      536 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      605 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/profiles/uninstall/registry.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.183240 rer.solrpush-1.3.0/src/rer/solrpush/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      216 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/restapi/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.183688 rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      200 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.184403 rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/elevate_schema/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/elevate_schema/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      344 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/elevate_schema/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      355 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/elevate_schema/get.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.185639 rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/solr_search/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/solr_search/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     3891 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/solr_search/batch.py
--rw-r--r--   0 cekk       (501) staff       (20)      334 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/solr_search/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      919 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/solr_search/get.py
--rw-r--r--   0 cekk       (501) staff       (20)     3064 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/solr_search/solr_search_handler.py
--rw-r--r--   0 cekk       (501) staff       (20)      610 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     5232 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.188961 rer.solrpush-1.3.0/src/rer/solrpush/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.190006 rer.solrpush-1.3.0/src/rer/solrpush/tests/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     6207 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/docs/example.docx
--rw-r--r--   0 cekk       (501) staff       (20)     8355 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/docs/example.ods
--rw-r--r--   0 cekk       (501) staff       (20)    13430 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/docs/example.pdf
--rw-r--r--   0 cekk       (501) staff       (20)    14135 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/docs/plone_logo.png
--rw-r--r--   0 cekk       (501) staff       (20)     2079 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/test_behaviors.py
--rw-r--r--   0 cekk       (501) staff       (20)     4328 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/test_elevate.py
--rw-r--r--   0 cekk       (501) staff       (20)     6398 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/test_events.py
--rw-r--r--   0 cekk       (501) staff       (20)     3137 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/test_image_tags.py
--rw-r--r--   0 cekk       (501) staff       (20)     6364 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/test_maintenance.py
--rw-r--r--   0 cekk       (501) staff       (20)     9366 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/test_querybuilder.py
--rw-r--r--   0 cekk       (501) staff       (20)     4467 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/test_restapi_search.py
--rw-r--r--   0 cekk       (501) staff       (20)     5992 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/test_search.py
--rw-r--r--   0 cekk       (501) staff       (20)     2295 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/test_setup.py
--rw-r--r--   0 cekk       (501) staff       (20)    14837 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/test_solr_interface.py
--rw-r--r--   0 cekk       (501) staff       (20)     3137 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/test_tika.py
--rw-r--r--   0 cekk       (501) staff       (20)     3700 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/tests/test_vocabularies.py
--rw-r--r--   0 cekk       (501) staff       (20)     2213 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/upgrades.py
--rw-r--r--   0 cekk       (501) staff       (20)     2288 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/upgrades.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.191105 rer.solrpush-1.3.0/src/rer/solrpush/utils/
--rw-r--r--   0 cekk       (501) staff       (20)      345 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/utils/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     3813 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/utils/solr_common.py
--rw-r--r--   0 cekk       (501) staff       (20)     8729 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/utils/solr_indexer.py
--rw-r--r--   0 cekk       (501) staff       (20)    10807 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/utils/solr_search.py
--rw-r--r--   0 cekk       (501) staff       (20)     1599 2022-09-29 15:18:37.000000 rer.solrpush-1.3.0/src/rer/solrpush/vocabularies.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-09-29 15:18:38.157854 rer.solrpush-1.3.0/src/rer.solrpush.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)    16361 2022-09-29 15:18:38.000000 rer.solrpush-1.3.0/src/rer.solrpush.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     5322 2022-09-29 15:18:38.000000 rer.solrpush-1.3.0/src/rer.solrpush.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2022-09-29 15:18:38.000000 rer.solrpush-1.3.0/src/rer.solrpush.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      137 2022-09-29 15:18:38.000000 rer.solrpush-1.3.0/src/rer.solrpush.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)        4 2022-09-29 15:18:38.000000 rer.solrpush-1.3.0/src/rer.solrpush.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2022-09-29 15:18:38.000000 rer.solrpush-1.3.0/src/rer.solrpush.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      245 2022-09-29 15:18:38.000000 rer.solrpush-1.3.0/src/rer.solrpush.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)        4 2022-09-29 15:18:38.000000 rer.solrpush-1.3.0/src/rer.solrpush.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.645226 rer.solrpush-1.3.1/
+-rw-r--r--   0 cekk       (501) staff       (20)     4231 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       67 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      652 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      525 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)    16489 2023-08-01 09:12:43.645506 rer.solrpush-1.3.1/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     7496 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      171 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/docker-compose.yml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.607678 rer.solrpush-1.3.1/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)   213611 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/docs/Solr-Push_Configurazione.jpg
+-rw-r--r--   0 cekk       (501) staff       (20)     7885 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)       59 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    32560 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/docs/rer-logo.png
+-rw-r--r--   0 cekk       (501) staff       (20)     3432 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/publiccode.yml
+-rw-r--r--   0 cekk       (501) staff       (20)      321 2023-08-01 09:12:43.646040 rer.solrpush-1.3.1/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2586 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.597076 rer.solrpush-1.3.1/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.608034 rer.solrpush-1.3.1/src/rer/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.613530 rer.solrpush-1.3.1/src/rer/solrpush/
+-rw-r--r--   0 cekk       (501) staff       (20)      130 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.614394 rer.solrpush-1.3.1/src/rer/solrpush/adapters/
+-rw-r--r--   0 cekk       (501) staff       (20)       24 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/adapters/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      282 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/adapters/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1439 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/adapters/file.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.615165 rer.solrpush-1.3.1/src/rer/solrpush/behaviors/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/behaviors/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      458 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/behaviors/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     1148 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/behaviors/solr_fields.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.617359 rer.solrpush-1.3.1/src/rer/solrpush/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3421 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     3304 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/controlpanel.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1205 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/elevate_settings.py
+-rw-r--r--   0 cekk       (501) staff       (20)    16058 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/maintenance.py
+-rw-r--r--   0 cekk       (501) staff       (20)      350 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/query_debug.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6247 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/querybuilder.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2322 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/scales.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.618917 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/.gitkeep
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.598305 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/dist/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.622702 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/dist/dev/
+-rw-r--r--   0 cekk       (501) staff       (20)  2311368 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/dist/dev/main.js
+-rw-r--r--   0 cekk       (501) staff       (20)  1783747 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/dist/dev/main.js.map
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.625824 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/dist/prod/
+-rw-r--r--   0 cekk       (501) staff       (20)   294024 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/dist/prod/main.js
+-rw-r--r--   0 cekk       (501) staff       (20)      159 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/dist/prod/main.js.map
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.626097 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/javascripts/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.626438 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/javascripts/FacetsContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)     1025 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/javascripts/FacetsContainer/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.626732 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/javascripts/ProgressBar/
+-rw-r--r--   0 cekk       (501) staff       (20)      946 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/javascripts/ProgressBar/index.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.627019 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/javascripts/ProgressBarContainer/
+-rw-r--r--   0 cekk       (501) staff       (20)     1737 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/javascripts/ProgressBarContainer/index.js
+-rw-r--r--   0 cekk       (501) staff       (20)      455 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/javascripts/index.js
+-rw-r--r--   0 cekk       (501) staff       (20)      258 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/package.json
+-rw-r--r--   0 cekk       (501) staff       (20)      618 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/styles.css
+-rw-r--r--   0 cekk       (501) staff       (20)      174 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/styles.css.map
+-rw-r--r--   0 cekk       (501) staff       (20)      431 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/styles.scss
+-rw-r--r--   0 cekk       (501) staff       (20)    57992 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/static/yarn.lock
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.628042 rer.solrpush-1.3.1/src/rer/solrpush/browser/templates/
+-rw-r--r--   0 cekk       (501) staff       (20)     1822 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/templates/controlpanel_layout.pt
+-rw-r--r--   0 cekk       (501) staff       (20)      498 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/templates/query_debug.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     1453 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/browser/templates/reindex_solr.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     2423 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     4080 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/indexer.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.629643 rer.solrpush-1.3.1/src/rer/solrpush/interfaces/
+-rw-r--r--   0 cekk       (501) staff       (20)      282 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/interfaces/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      307 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/interfaces/adapter.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3344 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/interfaces/elevate.py
+-rw-r--r--   0 cekk       (501) staff       (20)      197 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/interfaces/layer.py
+-rw-r--r--   0 cekk       (501) staff       (20)      153 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/interfaces/queueprocessor.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6735 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/interfaces/settings.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.630913 rer.solrpush-1.3.1/src/rer/solrpush/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/locales/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.599860 rer.solrpush-1.3.1/src/rer/solrpush/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.631432 rer.solrpush-1.3.1/src/rer/solrpush/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      458 2023-08-01 09:12:43.000000 rer.solrpush-1.3.1/src/rer/solrpush/locales/en/LC_MESSAGES/rer.solrpush.mo
+-rw-r--r--   0 cekk       (501) staff       (20)    11576 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/locales/en/LC_MESSAGES/rer.solrpush.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.600129 rer.solrpush-1.3.1/src/rer/solrpush/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.631984 rer.solrpush-1.3.1/src/rer/solrpush/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     9142 2023-08-01 09:12:43.000000 rer.solrpush-1.3.1/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.mo
+-rw-r--r--   0 cekk       (501) staff       (20)    16580 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.po
+-rw-r--r--   0 cekk       (501) staff       (20)    11694 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/locales/rer.solrpush.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     1528 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      473 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)     5977 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/parser.py
+-rw-r--r--   0 cekk       (501) staff       (20)      424 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.601174 rer.solrpush-1.3.1/src/rer/solrpush/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.633639 rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      854 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/actions.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      162 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      953 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      257 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.634456 rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/registry/
+-rw-r--r--   0 cekk       (501) staff       (20)      891 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/registry/bundle.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     2828 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/registry/criteria.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      278 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/registry/settings.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      387 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.634714 rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/types/
+-rw-r--r--   0 cekk       (501) staff       (20)      299 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/types/Document.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.635229 rer.solrpush-1.3.1/src/rer/solrpush/profiles/to_1100/
+-rw-r--r--   0 cekk       (501) staff       (20)      232 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/to_1100/componentregistry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)       97 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/to_1100/metadata.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.635741 rer.solrpush-1.3.1/src/rer/solrpush/profiles/to_1300/
+-rw-r--r--   0 cekk       (501) staff       (20)      322 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/to_1300/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      211 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/to_1300/registry.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.636491 rer.solrpush-1.3.1/src/rer/solrpush/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      122 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      536 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/uninstall/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      605 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/profiles/uninstall/registry.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.636936 rer.solrpush-1.3.1/src/rer/solrpush/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      216 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/restapi/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.637374 rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      200 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.638280 rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/elevate_schema/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/elevate_schema/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      344 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/elevate_schema/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      355 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/elevate_schema/get.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.639698 rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/solr_search/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/solr_search/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3891 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/solr_search/batch.py
+-rw-r--r--   0 cekk       (501) staff       (20)      334 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/solr_search/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      919 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/solr_search/get.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3064 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/solr_search/solr_search_handler.py
+-rw-r--r--   0 cekk       (501) staff       (20)      610 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5232 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.642943 rer.solrpush-1.3.1/src/rer/solrpush/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.644000 rer.solrpush-1.3.1/src/rer/solrpush/tests/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     6207 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/docs/example.docx
+-rw-r--r--   0 cekk       (501) staff       (20)     8355 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/docs/example.ods
+-rw-r--r--   0 cekk       (501) staff       (20)    13430 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/docs/example.pdf
+-rw-r--r--   0 cekk       (501) staff       (20)    14135 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/docs/plone_logo.png
+-rw-r--r--   0 cekk       (501) staff       (20)     2079 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/test_behaviors.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4328 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/test_elevate.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6398 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/test_events.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3137 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/test_image_tags.py
+-rw-r--r--   0 cekk       (501) staff       (20)     6364 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/test_maintenance.py
+-rw-r--r--   0 cekk       (501) staff       (20)     9366 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/test_querybuilder.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4467 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/test_restapi_search.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5992 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/test_search.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2295 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/test_setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)    14837 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/test_solr_interface.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3137 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/test_tika.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3700 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/tests/test_vocabularies.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2213 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/upgrades.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2288 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/upgrades.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.645010 rer.solrpush-1.3.1/src/rer/solrpush/utils/
+-rw-r--r--   0 cekk       (501) staff       (20)      345 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/utils/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3813 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/utils/solr_common.py
+-rw-r--r--   0 cekk       (501) staff       (20)     8729 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/utils/solr_indexer.py
+-rw-r--r--   0 cekk       (501) staff       (20)    10807 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/utils/solr_search.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1599 2023-08-01 09:12:42.000000 rer.solrpush-1.3.1/src/rer/solrpush/vocabularies.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-08-01 09:12:43.610633 rer.solrpush-1.3.1/src/rer.solrpush.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)    16489 2023-08-01 09:12:43.000000 rer.solrpush-1.3.1/src/rer.solrpush.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     5322 2023-08-01 09:12:43.000000 rer.solrpush-1.3.1/src/rer.solrpush.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-08-01 09:12:43.000000 rer.solrpush-1.3.1/src/rer.solrpush.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      137 2023-08-01 09:12:43.000000 rer.solrpush-1.3.1/src/rer.solrpush.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        4 2023-08-01 09:12:43.000000 rer.solrpush-1.3.1/src/rer.solrpush.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-08-01 09:12:43.000000 rer.solrpush-1.3.1/src/rer.solrpush.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      245 2023-08-01 09:12:43.000000 rer.solrpush-1.3.1/src/rer.solrpush.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        4 2023-08-01 09:12:43.000000 rer.solrpush-1.3.1/src/rer.solrpush.egg-info/top_level.txt
```

### Comparing `rer.solrpush-1.3.0/CHANGES.rst` & `rer.solrpush-1.3.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+1.3.1 (2023-08-01)
+------------------
+
+- Update translation.
+  [cekk]
+
+
 1.3.0 (2022-09-29)
 ------------------
 
 - Add ``search_enabled`` flag to temporary disable search on SOLR.
   [cekk]
```

### Comparing `rer.solrpush-1.3.0/DEVELOP.rst` & `rer.solrpush-1.3.1/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/LICENSE.GPL` & `rer.solrpush-1.3.1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/LICENSE.rst` & `rer.solrpush-1.3.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/MANIFEST.in` & `rer.solrpush-1.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/PKG-INFO` & `rer.solrpush-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.solrpush
-Version: 1.3.0
+Version: 1.3.1
 Summary: Prodotto per Regione Emilia-Romagna relativo all'indicizzazione dei contenuti con solr
 Home-page: https://github.com/collective/rer.solrpush
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.solrpush
 Project-URL: Source, https://github.com/collective/rer.solrpush
@@ -220,14 +220,21 @@
         - RedTurtle, sviluppoplone@redturtle.it
         
         
         Changelog
         =========
         
         
+        1.3.1 (2023-08-01)
+        ------------------
+        
+        - Update translation.
+          [cekk]
+        
+        
         1.3.0 (2022-09-29)
         ------------------
         
         - Add ``search_enabled`` flag to temporary disable search on SOLR.
           [cekk]
```

### Comparing `rer.solrpush-1.3.0/README.rst` & `rer.solrpush-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/docs/Solr-Push_Configurazione.jpg` & `rer.solrpush-1.3.1/docs/Solr-Push_Configurazione.jpg`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/docs/conf.py` & `rer.solrpush-1.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/docs/rer-logo.png` & `rer.solrpush-1.3.1/docs/rer-logo.png`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/publiccode.yml` & `rer.solrpush-1.3.1/publiccode.yml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/setup.py` & `rer.solrpush-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="rer.solrpush",
-    version="1.3.0",
+    version="1.3.1",
     description="Prodotto per Regione Emilia-Romagna relativo all'indicizzazione dei contenuti con solr",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/adapters/file.py` & `rer.solrpush-1.3.1/src/rer/solrpush/adapters/file.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/behaviors/solr_fields.py` & `rer.solrpush-1.3.1/src/rer/solrpush/behaviors/solr_fields.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/configure.zcml` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/controlpanel.py` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/elevate_settings.py` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/elevate_settings.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/maintenance.py` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/maintenance.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/querybuilder.py` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/querybuilder.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/scales.py` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/scales.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/static/dist/dev/main.js` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/static/dist/dev/main.js`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/static/dist/dev/main.js.map` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/static/dist/dev/main.js.map`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/static/dist/prod/main.js` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/static/dist/prod/main.js`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/static/javascripts/FacetsContainer/index.js` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/static/javascripts/FacetsContainer/index.js`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/static/javascripts/ProgressBar/index.js` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/static/javascripts/ProgressBar/index.js`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/static/javascripts/ProgressBarContainer/index.js` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/static/javascripts/ProgressBarContainer/index.js`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/static/styles.css` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/static/styles.css`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/static/yarn.lock` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/static/yarn.lock`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/templates/controlpanel_layout.pt` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/templates/controlpanel_layout.pt`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/browser/templates/reindex_solr.pt` & `rer.solrpush-1.3.1/src/rer/solrpush/browser/templates/reindex_solr.pt`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/configure.zcml` & `rer.solrpush-1.3.1/src/rer/solrpush/configure.zcml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/indexer.py` & `rer.solrpush-1.3.1/src/rer/solrpush/indexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                     message = _(
                         "content_indexed_error",
                         default=u"There was a problem indexing or unindexing "
                         u"this content. Please take note of this address and "
                         u"contact site administrator.",
                     )
                     api.portal.show_message(
-                        message=message, request=getRequest(), type="error"
+                        message=message, request=getRequest(), type="warning"
                     )
             self.queue = []
 
     def abort(self):
         self.queue = []
```

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/interfaces/elevate.py` & `rer.solrpush-1.3.1/src/rer/solrpush/interfaces/elevate.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/interfaces/settings.py` & `rer.solrpush-1.3.1/src/rer/solrpush/interfaces/settings.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/locales/README.rst` & `rer.solrpush-1.3.1/src/rer/solrpush/locales/README.rst`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/locales/en/LC_MESSAGES/rer.solrpush.po` & `rer.solrpush-1.3.1/src/rer/solrpush/locales/en/LC_MESSAGES/rer.solrpush.po`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.mo` & `rer.solrpush-1.3.1/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -166,18 +166,18 @@
 msgstr "bq (boost query)"
 
 msgid "cancel_label"
 msgstr "Annulla"
 
 msgid "content_indexed_error"
 msgstr ""
-"Si è verificato un problema: questo contenuto non può essere indicizzato o "
-"rimosso da SOLR e quindi non verrà mostrato nelle ricerche e nelle "
-"collezioni fatte con SOLR. Avvisa subito gli amministratori del sito "
-"indicando l'URL di questo contenuto."
+"Questo contenuto è stato correttamente aggiornato ma in questo momento non "
+"può essere indicizzato o rimosso dal nostro motore di ricerca, quindi non "
+"verrà mostrato nelle ricerche e nelle collezioni multiportale. Il motore di "
+"ricerca verrà allineato questa notte."
 
 msgid "content_remove_error"
 msgstr ""
 "Si è verificato un problema rimuovendo questo contenuto da SOLR. Contatta "
 "l'amministratore per maggiori informazioni."
 
 msgid "elevate_row_schema_text_help"
```

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.po` & `rer.solrpush-1.3.1/src/rer/solrpush/locales/it/LC_MESSAGES/rer.solrpush.po`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 #: rer/solrpush/browser/maintenance.py:73
 msgid "cancel_label"
 msgstr "Annulla"
 
 #. Default: "There was a problem indexing or unindexing this content. Please take note of this address and contact site administrator."
 #: rer/solrpush/indexer.py:92
 msgid "content_indexed_error"
-msgstr "Si è verificato un problema: questo contenuto non può essere indicizzato o rimosso da SOLR e quindi non verrà mostrato nelle ricerche e nelle collezioni fatte con SOLR. Avvisa subito gli amministratori del sito indicando l'URL di questo contenuto."
+msgstr "Questo contenuto è stato correttamente aggiornato ma in questo momento non può essere indicizzato o rimosso dal nostro motore di ricerca, quindi non verrà mostrato nelle ricerche e nelle collezioni multiportale. Il motore di ricerca verrà allineato questa notte."
 
 #. Default: "There was a problem removing this content from SOLR.  Please contact site administrator."
 #: rer/solrpush/utils/solr_indexer.py:275
 msgid "content_remove_error"
 msgstr "Si è verificato un problema rimuovendo questo contenuto da SOLR. Contatta l'amministratore per maggiori informazioni."
 
 #. Default: "The word that should match in the search."
```

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/locales/rer.solrpush.pot` & `rer.solrpush-1.3.1/src/rer/solrpush/locales/rer.solrpush.pot`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/locales/update.py` & `rer.solrpush-1.3.1/src/rer/solrpush/locales/update.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/parser.py` & `rer.solrpush-1.3.1/src/rer/solrpush/parser.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/actions.xml` & `rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/controlpanel.xml` & `rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/registry/bundle.xml` & `rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/registry/bundle.xml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/profiles/default/registry/criteria.xml` & `rer.solrpush-1.3.1/src/rer/solrpush/profiles/default/registry/criteria.xml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/profiles/uninstall/controlpanel.xml` & `rer.solrpush-1.3.1/src/rer/solrpush/profiles/uninstall/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/profiles/uninstall/registry.xml` & `rer.solrpush-1.3.1/src/rer/solrpush/profiles/uninstall/registry.xml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/solr_search/batch.py` & `rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/solr_search/batch.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/solr_search/get.py` & `rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/solr_search/get.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/restapi/services/solr_search/solr_search_handler.py` & `rer.solrpush-1.3.1/src/rer/solrpush/restapi/services/solr_search/solr_search_handler.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/setuphandlers.py` & `rer.solrpush-1.3.1/src/rer/solrpush/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/testing.py` & `rer.solrpush-1.3.1/src/rer/solrpush/testing.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/docs/example.docx` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/docs/example.docx`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/docs/example.ods` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/docs/example.ods`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/docs/example.pdf` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/docs/example.pdf`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/docs/plone_logo.png` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/docs/plone_logo.png`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/test_behaviors.py` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/test_behaviors.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/test_elevate.py` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/test_elevate.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/test_events.py` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/test_image_tags.py` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/test_image_tags.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/test_maintenance.py` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/test_maintenance.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/test_querybuilder.py` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/test_querybuilder.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/test_restapi_search.py` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/test_restapi_search.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/test_search.py` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/test_setup.py` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/test_solr_interface.py` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/test_solr_interface.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/test_tika.py` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/test_tika.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/tests/test_vocabularies.py` & `rer.solrpush-1.3.1/src/rer/solrpush/tests/test_vocabularies.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/upgrades.py` & `rer.solrpush-1.3.1/src/rer/solrpush/upgrades.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/upgrades.zcml` & `rer.solrpush-1.3.1/src/rer/solrpush/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/utils/solr_common.py` & `rer.solrpush-1.3.1/src/rer/solrpush/utils/solr_common.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/utils/solr_indexer.py` & `rer.solrpush-1.3.1/src/rer/solrpush/utils/solr_indexer.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/utils/solr_search.py` & `rer.solrpush-1.3.1/src/rer/solrpush/utils/solr_search.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer/solrpush/vocabularies.py` & `rer.solrpush-1.3.1/src/rer/solrpush/vocabularies.py`

 * *Files identical despite different names*

### Comparing `rer.solrpush-1.3.0/src/rer.solrpush.egg-info/PKG-INFO` & `rer.solrpush-1.3.1/src/rer.solrpush.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rer.solrpush
-Version: 1.3.0
+Version: 1.3.1
 Summary: Prodotto per Regione Emilia-Romagna relativo all'indicizzazione dei contenuti con solr
 Home-page: https://github.com/collective/rer.solrpush
 Author: RedTurtle
 Author-email: sviluppoplone@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/rer.solrpush
 Project-URL: Source, https://github.com/collective/rer.solrpush
@@ -220,14 +220,21 @@
         - RedTurtle, sviluppoplone@redturtle.it
         
         
         Changelog
         =========
         
         
+        1.3.1 (2023-08-01)
+        ------------------
+        
+        - Update translation.
+          [cekk]
+        
+        
         1.3.0 (2022-09-29)
         ------------------
         
         - Add ``search_enabled`` flag to temporary disable search on SOLR.
           [cekk]
```

### Comparing `rer.solrpush-1.3.0/src/rer.solrpush.egg-info/SOURCES.txt` & `rer.solrpush-1.3.1/src/rer.solrpush.egg-info/SOURCES.txt`

 * *Files identical despite different names*

