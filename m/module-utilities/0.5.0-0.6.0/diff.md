# Comparing `tmp/module-utilities-0.5.0.tar.gz` & `tmp/module-utilities-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "module-utilities-0.5.0.tar", last modified: Mon Jul 10 16:25:34 2023, max compression
+gzip compressed data, was "module-utilities-0.6.0.tar", last modified: Tue Aug  1 20:26:44 2023, max compression
```

## Comparing `module-utilities-0.5.0.tar` & `module-utilities-0.6.0.tar`

### file list

```diff
@@ -1,135 +1,147 @@
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.441504 module-utilities-0.5.0/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1367 2023-07-10 16:24:53.000000 module-utilities-0.5.0/.cruft.json
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      540 2023-05-02 03:09:02.000000 module-utilities-0.5.0/.editorconfig
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.374016 module-utilities-0.5.0/.github/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      368 2023-05-02 03:09:02.000000 module-utilities-0.5.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1409 2023-07-10 16:24:53.000000 module-utilities-0.5.0/.gitignore
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-04-27 23:45:36.000000 module-utilities-0.5.0/.markdownlint.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3635 2023-07-10 16:24:53.000000 module-utilities-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       20 2023-04-27 23:45:36.000000 module-utilities-0.5.0/.prettierrc.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      527 2023-06-29 17:23:57.000000 module-utilities-0.5.0/.recipe-append.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      122 2023-04-27 23:45:36.000000 module-utilities-0.5.0/AUTHORS.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      789 2023-07-10 16:24:53.000000 module-utilities-0.5.0/CHANGELOG.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    11143 2023-07-10 16:24:53.000000 module-utilities-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1789 2023-06-29 17:24:09.000000 module-utilities-0.5.0/LICENSE
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      258 2023-04-27 23:45:36.000000 module-utilities-0.5.0/MANIFEST.in
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9644 2023-07-10 16:24:53.000000 module-utilities-0.5.0/Makefile
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9430 2023-07-10 16:25:34.440140 module-utilities-0.5.0/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5615 2023-06-29 17:24:16.000000 module-utilities-0.5.0/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.375119 module-utilities-0.5.0/changelog.d/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-04-27 23:45:36.000000 module-utilities-0.5.0/changelog.d/README.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.375818 module-utilities-0.5.0/changelog.d/templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.377562 module-utilities-0.5.0/changelog.d/templates/auto-changelog/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      213 2023-04-27 23:45:36.000000 module-utilities-0.5.0/changelog.d/templates/auto-changelog/macros.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      774 2023-04-27 23:45:36.000000 module-utilities-0.5.0/changelog.d/templates/auto-changelog/template.jinja2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      269 2023-04-27 23:45:36.000000 module-utilities-0.5.0/changelog.d/templates/new_fragment.md.j2
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      204 2023-04-27 23:45:36.000000 module-utilities-0.5.0/conftest.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.384057 module-utilities-0.5.0/docs/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1401 2023-05-03 02:36:13.000000 module-utilities-0.5.0/docs/Makefile
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.357670 module-utilities-0.5.0/docs/_static/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.384807 module-utilities-0.5.0/docs/_static/css/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     2937 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_static/css/nist-combined.css
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.386361 module-utilities-0.5.0/docs/_static/js/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_static/js/leave_notice.js
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      706 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_static/js/nist-header-footer.js
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.391048 module-utilities-0.5.0/docs/_templates/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.394871 module-utilities-0.5.0/docs/_templates/autodocsumm/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      289 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autodocsumm/class-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      249 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autodocsumm/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      405 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autodocsumm/module-inherit.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      424 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autodocsumm/module-noindex.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      374 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autodocsumm/module.rst
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.397029 module-utilities-0.5.0/docs/_templates/autosummary/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      106 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1119 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1418 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/class-individual-pages.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1255 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/class-single-page.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1186 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/custom-module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1212 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/module-custom-imported.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1177 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/module-custom.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1071 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/module-single.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1179 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/_templates/module-template.rst
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       69 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/authors.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       71 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/changelog.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    15101 2023-07-10 16:24:53.000000 module-utilities-0.5.0/docs/conf.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       74 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/contributing.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.397779 module-utilities-0.5.0/docs/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       75 2023-06-29 17:24:43.000000 module-utilities-0.5.0/docs/examples/index.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.399407 module-utilities-0.5.0/docs/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.5.0/docs/examples/usage/cached.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.5.0/docs/examples/usage/docfiller.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      224 2023-06-29 17:24:47.000000 module-utilities-0.5.0/docs/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      940 2023-06-29 17:24:47.000000 module-utilities-0.5.0/docs/installation.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       40 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/license.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      767 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/make.bat
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/navigation.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.400196 module-utilities-0.5.0/docs/reference/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      192 2023-06-29 17:24:47.000000 module-utilities-0.5.0/docs/reference/index.md
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.5.0/docs/spelling_wordlist.txt
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.409736 module-utilities-0.5.0/environment/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      227 2023-07-10 16:25:24.000000 module-utilities-0.5.0/environment/base.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      419 2023-07-10 16:25:25.000000 module-utilities-0.5.0/environment/dev.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      280 2023-07-10 16:25:26.000000 module-utilities-0.5.0/environment/dist-conda.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      161 2023-07-10 16:25:26.000000 module-utilities-0.5.0/environment/dist-pypi.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      225 2023-07-10 16:25:25.000000 module-utilities-0.5.0/environment/dist-pypi.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      406 2023-07-10 16:25:25.000000 module-utilities-0.5.0/environment/docs.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      136 2023-05-02 03:09:02.000000 module-utilities-0.5.0/environment/lint.yaml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.420925 module-utilities-0.5.0/environment/lock/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    37993 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py310-dev-conda-lock.yml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    73122 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py310-dist-conda-conda-lock.yml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23235 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py310-dist-pypi-conda-lock.yml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13842 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py310-test-conda-lock.yml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    15181 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py310-typing-conda-lock.yml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-06-14 21:18:50.000000 module-utilities-0.5.0/environment/lock/py310.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14231 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py311-test-conda-lock.yml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    15570 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py311-typing-conda-lock.yml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       64 2023-06-14 21:18:50.000000 module-utilities-0.5.0/environment/lock/py311.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13457 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py38-test-conda-lock.yml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    14788 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py38-typing-conda-lock.yml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       63 2023-06-14 21:18:50.000000 module-utilities-0.5.0/environment/lock/py38.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13831 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py39-test-conda-lock.yml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    15164 2023-07-10 16:24:53.000000 module-utilities-0.5.0/environment/lock/py39-typing-conda-lock.yml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       63 2023-06-14 21:18:50.000000 module-utilities-0.5.0/environment/lock/py39.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      193 2023-07-10 16:25:26.000000 module-utilities-0.5.0/environment/test-extras.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      265 2023-07-10 16:25:26.000000 module-utilities-0.5.0/environment/test-extras.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      287 2023-07-10 16:25:24.000000 module-utilities-0.5.0/environment/test.yaml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      296 2023-07-10 16:25:24.000000 module-utilities-0.5.0/environment/typing.yaml
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.421911 module-utilities-0.5.0/examples/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      222 2023-04-27 23:45:36.000000 module-utilities-0.5.0/examples/README.md
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.423762 module-utilities-0.5.0/examples/usage/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    13498 2023-05-03 02:36:13.000000 module-utilities-0.5.0/examples/usage/cached.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    18227 2023-05-03 20:28:18.000000 module-utilities-0.5.0/examples/usage/docfiller.ipynb
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    32098 2023-07-10 16:24:53.000000 module-utilities-0.5.0/noxfile.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     7499 2023-07-10 16:24:53.000000 module-utilities-0.5.0/pyproject.toml
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       38 2023-07-10 16:25:34.441887 module-utilities-0.5.0/setup.cfg
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.360910 module-utilities-0.5.0/src/
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.428319 module-utilities-0.5.0/src/module_utilities/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      340 2023-07-10 16:24:53.000000 module-utilities-0.5.0/src/module_utilities/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3199 2023-07-10 16:24:53.000000 module-utilities-0.5.0/src/module_utilities/_doc.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      382 2023-05-02 03:09:02.000000 module-utilities-0.5.0/src/module_utilities/_typing.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      160 2023-07-10 16:25:34.000000 module-utilities-0.5.0/src/module_utilities/_version.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     5930 2023-05-03 20:28:18.000000 module-utilities-0.5.0/src/module_utilities/attributedict.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9991 2023-05-03 20:28:18.000000 module-utilities-0.5.0/src/module_utilities/cached.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    21356 2023-07-10 16:24:53.000000 module-utilities-0.5.0/src/module_utilities/docfiller.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-05-02 03:09:02.000000 module-utilities-0.5.0/src/module_utilities/py.typed
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.434895 module-utilities-0.5.0/src/module_utilities/vendored/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     1298 2023-06-14 21:18:50.000000 module-utilities-0.5.0/src/module_utilities/vendored/LICENSE.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       93 2023-06-14 21:18:50.000000 module-utilities-0.5.0/src/module_utilities/vendored/README.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       24 2023-06-14 21:18:50.000000 module-utilities-0.5.0/src/module_utilities/vendored/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    23449 2023-06-14 21:18:50.000000 module-utilities-0.5.0/src/module_utilities/vendored/docscrape.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.431587 module-utilities-0.5.0/src/module_utilities.egg-info/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     9430 2023-07-10 16:25:34.000000 module-utilities-0.5.0/src/module_utilities.egg-info/PKG-INFO
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)     3205 2023-07-10 16:25:34.000000 module-utilities-0.5.0/src/module_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-07-10 16:25:34.000000 module-utilities-0.5.0/src/module_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      696 2023-07-10 16:25:34.000000 module-utilities-0.5.0/src/module_utilities.egg-info/requires.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       17 2023-07-10 16:25:34.000000 module-utilities-0.5.0/src/module_utilities.egg-info/top_level.txt
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        1 2023-05-04 19:05:27.000000 module-utilities-0.5.0/src/module_utilities.egg-info/zip-safe
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.438091 module-utilities-0.5.0/tests/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)       46 2023-04-27 23:45:36.000000 module-utilities-0.5.0/tests/__init__.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)        0 2023-04-27 23:45:36.000000 module-utilities-0.5.0/tests/conftest.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10864 2023-05-02 03:09:02.000000 module-utilities-0.5.0/tests/test_cached.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    10075 2023-07-10 16:24:53.000000 module-utilities-0.5.0/tests/test_docfiller.py
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)      169 2023-06-29 17:27:13.000000 module-utilities-0.5.0/tests/test_module_utilities.py
-drwxr-xr-x   0 wpk      (42033) NIST\646DIV (36681)        0 2023-07-10 16:25:34.438794 module-utilities-0.5.0/tools/
--rw-r--r--   0 wpk      (42033) NIST\646DIV (36681)    24175 2023-07-10 16:24:53.000000 module-utilities-0.5.0/tools/noxtools.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.657085 module-utilities-0.6.0/
+-rw-r--r--   0 wpk      (42033)    36681     1367 2023-08-01 20:26:00.000000 module-utilities-0.6.0/.cruft.json
+-rw-r--r--   0 wpk      (42033)    36681      540 2023-05-02 03:09:02.000000 module-utilities-0.6.0/.editorconfig
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.570939 module-utilities-0.6.0/.github/
+-rw-r--r--   0 wpk      (42033)    36681      368 2023-05-02 03:09:02.000000 module-utilities-0.6.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 wpk      (42033)    36681     1409 2023-07-10 16:24:53.000000 module-utilities-0.6.0/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-04-27 23:45:36.000000 module-utilities-0.6.0/.markdownlint.yaml
+-rw-r--r--   0 wpk      (42033)    36681     3680 2023-08-01 20:26:00.000000 module-utilities-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 wpk      (42033)    36681       20 2023-04-27 23:45:36.000000 module-utilities-0.6.0/.prettierrc.yaml
+-rw-r--r--   0 wpk      (42033)    36681      527 2023-06-29 17:23:57.000000 module-utilities-0.6.0/.recipe-append.yaml
+-rw-r--r--   0 wpk      (42033)    36681      121 2023-08-01 20:26:00.000000 module-utilities-0.6.0/AUTHORS.md
+-rw-r--r--   0 wpk      (42033)    36681     1003 2023-08-01 20:26:00.000000 module-utilities-0.6.0/CHANGELOG.md
+-rw-r--r--   0 wpk      (42033)    36681    11143 2023-07-10 16:24:53.000000 module-utilities-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 wpk      (42033)    36681     1789 2023-06-29 17:24:09.000000 module-utilities-0.6.0/LICENSE
+-rw-r--r--   0 wpk      (42033)    36681      258 2023-04-27 23:45:36.000000 module-utilities-0.6.0/MANIFEST.in
+-rw-r--r--   0 wpk      (42033)    36681     9680 2023-08-01 20:26:00.000000 module-utilities-0.6.0/Makefile
+-rw-r--r--   0 wpk      (42033)    36681    10311 2023-08-01 20:26:44.656013 module-utilities-0.6.0/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     6179 2023-08-01 20:26:00.000000 module-utilities-0.6.0/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.571781 module-utilities-0.6.0/changelog.d/
+-rw-r--r--   0 wpk      (42033)    36681       64 2023-04-27 23:45:36.000000 module-utilities-0.6.0/changelog.d/README.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.572378 module-utilities-0.6.0/changelog.d/templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.573673 module-utilities-0.6.0/changelog.d/templates/auto-changelog/
+-rw-r--r--   0 wpk      (42033)    36681      213 2023-04-27 23:45:36.000000 module-utilities-0.6.0/changelog.d/templates/auto-changelog/macros.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      774 2023-04-27 23:45:36.000000 module-utilities-0.6.0/changelog.d/templates/auto-changelog/template.jinja2
+-rw-r--r--   0 wpk      (42033)    36681      269 2023-04-27 23:45:36.000000 module-utilities-0.6.0/changelog.d/templates/new_fragment.md.j2
+-rw-r--r--   0 wpk      (42033)    36681      204 2023-04-27 23:45:36.000000 module-utilities-0.6.0/conftest.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.580727 module-utilities-0.6.0/docs/
+-rw-r--r--   0 wpk      (42033)    36681     1401 2023-05-03 02:36:13.000000 module-utilities-0.6.0/docs/Makefile
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.558198 module-utilities-0.6.0/docs/_static/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.581352 module-utilities-0.6.0/docs/_static/css/
+-rw-r--r--   0 wpk      (42033)    36681     2937 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_static/css/nist-combined.css
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.582701 module-utilities-0.6.0/docs/_static/js/
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_static/js/leave_notice.js
+-rw-r--r--   0 wpk      (42033)    36681      706 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_static/js/nist-header-footer.js
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.587313 module-utilities-0.6.0/docs/_templates/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.591512 module-utilities-0.6.0/docs/_templates/autodocsumm/
+-rw-r--r--   0 wpk      (42033)    36681      289 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/autodocsumm/class-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      249 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/autodocsumm/class.rst
+-rw-r--r--   0 wpk      (42033)    36681      405 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/autodocsumm/module-inherit.rst
+-rw-r--r--   0 wpk      (42033)    36681      424 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/autodocsumm/module-noindex.rst
+-rw-r--r--   0 wpk      (42033)    36681      374 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/autodocsumm/module.rst
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.593885 module-utilities-0.6.0/docs/_templates/autosummary/
+-rw-r--r--   0 wpk      (42033)    36681      106 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 wpk      (42033)    36681     1119 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 wpk      (42033)    36681     1418 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/class-individual-pages.rst
+-rw-r--r--   0 wpk      (42033)    36681     1255 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/class-single-page.rst
+-rw-r--r--   0 wpk      (42033)    36681     1186 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/custom-module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681     1212 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/module-custom-imported.rst
+-rw-r--r--   0 wpk      (42033)    36681     1177 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/module-custom.rst
+-rw-r--r--   0 wpk      (42033)    36681     1071 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/module-single.rst
+-rw-r--r--   0 wpk      (42033)    36681     1179 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/_templates/module-template.rst
+-rw-r--r--   0 wpk      (42033)    36681       69 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/authors.md
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/changelog.md
+-rw-r--r--   0 wpk      (42033)    36681    15285 2023-08-01 20:26:00.000000 module-utilities-0.6.0/docs/conf.py
+-rw-r--r--   0 wpk      (42033)    36681       74 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/contributing.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.594732 module-utilities-0.6.0/docs/examples/
+-rw-r--r--   0 wpk      (42033)    36681       75 2023-06-29 17:24:43.000000 module-utilities-0.6.0/docs/examples/index.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.596305 module-utilities-0.6.0/docs/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681    13498 2023-05-03 02:36:13.000000 module-utilities-0.6.0/docs/examples/usage/cached.ipynb
+-rw-r--r--   0 wpk      (42033)    36681    24493 2023-08-01 20:26:00.000000 module-utilities-0.6.0/docs/examples/usage/docfiller.ipynb
+-rw-r--r--   0 wpk      (42033)    36681      224 2023-06-29 17:24:47.000000 module-utilities-0.6.0/docs/index.md
+-rw-r--r--   0 wpk      (42033)    36681     1152 2023-08-01 20:26:00.000000 module-utilities-0.6.0/docs/installation.md
+-rw-r--r--   0 wpk      (42033)    36681       40 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/license.md
+-rw-r--r--   0 wpk      (42033)    36681      767 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/make.bat
+-rw-r--r--   0 wpk      (42033)    36681      169 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/navigation.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.597118 module-utilities-0.6.0/docs/reference/
+-rw-r--r--   0 wpk      (42033)    36681      217 2023-08-01 20:26:00.000000 module-utilities-0.6.0/docs/reference/index.md
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-04-27 23:45:36.000000 module-utilities-0.6.0/docs/spelling_wordlist.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.615314 module-utilities-0.6.0/environment/
+-rw-r--r--   0 wpk      (42033)    36681      161 2023-08-01 19:47:18.000000 module-utilities-0.6.0/environment/dist-pypi.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.627582 module-utilities-0.6.0/environment/lock/
+-rw-r--r--   0 wpk      (42033)    36681       71 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/lock/.gitignore
+-rw-r--r--   0 wpk      (42033)    36681    37993 2023-07-10 16:24:53.000000 module-utilities-0.6.0/environment/lock/py310-dev-conda-lock.yml
+-rw-r--r--   0 wpk      (42033)    36681    73122 2023-07-10 16:24:53.000000 module-utilities-0.6.0/environment/lock/py310-dist-conda-conda-lock.yml
+-rw-r--r--   0 wpk      (42033)    36681    23235 2023-07-10 16:24:53.000000 module-utilities-0.6.0/environment/lock/py310-dist-pypi-conda-lock.yml
+-rw-r--r--   0 wpk      (42033)    36681    13842 2023-07-10 16:24:53.000000 module-utilities-0.6.0/environment/lock/py310-test-conda-lock.yml
+-rw-r--r--   0 wpk      (42033)    36681    15181 2023-07-10 16:24:53.000000 module-utilities-0.6.0/environment/lock/py310-typing-conda-lock.yml
+-rw-r--r--   0 wpk      (42033)    36681    14231 2023-07-10 16:24:53.000000 module-utilities-0.6.0/environment/lock/py311-test-conda-lock.yml
+-rw-r--r--   0 wpk      (42033)    36681    15570 2023-07-10 16:24:53.000000 module-utilities-0.6.0/environment/lock/py311-typing-conda-lock.yml
+-rw-r--r--   0 wpk      (42033)    36681    13457 2023-07-10 16:24:53.000000 module-utilities-0.6.0/environment/lock/py38-test-conda-lock.yml
+-rw-r--r--   0 wpk      (42033)    36681    14788 2023-07-10 16:24:53.000000 module-utilities-0.6.0/environment/lock/py38-typing-conda-lock.yml
+-rw-r--r--   0 wpk      (42033)    36681    13831 2023-07-10 16:24:53.000000 module-utilities-0.6.0/environment/lock/py39-test-conda-lock.yml
+-rw-r--r--   0 wpk      (42033)    36681    15164 2023-07-10 16:24:53.000000 module-utilities-0.6.0/environment/lock/py39-typing-conda-lock.yml
+-rw-r--r--   0 wpk      (42033)    36681      456 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py310-dev.yaml
+-rw-r--r--   0 wpk      (42033)    36681      280 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py310-dist-conda.yaml
+-rw-r--r--   0 wpk      (42033)    36681      225 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py310-dist-pypi.yaml
+-rw-r--r--   0 wpk      (42033)    36681      432 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py310-docs.yaml
+-rw-r--r--   0 wpk      (42033)    36681      291 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py310-test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      287 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py310-test-noopt.yaml
+-rw-r--r--   0 wpk      (42033)    36681      313 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py310-test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      333 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py310-typing.yaml
+-rw-r--r--   0 wpk      (42033)    36681      291 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py311-test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      287 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py311-test-noopt.yaml
+-rw-r--r--   0 wpk      (42033)    36681      313 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py311-test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      322 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py311-typing.yaml
+-rw-r--r--   0 wpk      (42033)    36681      290 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py38-test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      286 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py38-test-noopt.yaml
+-rw-r--r--   0 wpk      (42033)    36681      312 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py38-test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      332 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py38-typing.yaml
+-rw-r--r--   0 wpk      (42033)    36681      290 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py39-test-extras.yaml
+-rw-r--r--   0 wpk      (42033)    36681      286 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py39-test-noopt.yaml
+-rw-r--r--   0 wpk      (42033)    36681      312 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py39-test.yaml
+-rw-r--r--   0 wpk      (42033)    36681      332 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/py39-typing.yaml
+-rw-r--r--   0 wpk      (42033)    36681      215 2023-08-01 20:26:00.000000 module-utilities-0.6.0/environment/test-extras.txt
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.628469 module-utilities-0.6.0/examples/
+-rw-r--r--   0 wpk      (42033)    36681      222 2023-04-27 23:45:36.000000 module-utilities-0.6.0/examples/README.md
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.629906 module-utilities-0.6.0/examples/usage/
+-rw-r--r--   0 wpk      (42033)    36681    13498 2023-05-03 02:36:13.000000 module-utilities-0.6.0/examples/usage/cached.ipynb
+-rw-r--r--   0 wpk      (42033)    36681    24493 2023-08-01 20:26:00.000000 module-utilities-0.6.0/examples/usage/docfiller.ipynb
+-rw-r--r--   0 wpk      (42033)    36681    35923 2023-08-01 20:26:00.000000 module-utilities-0.6.0/noxfile.py
+-rw-r--r--   0 wpk      (42033)    36681     8243 2023-08-01 20:26:00.000000 module-utilities-0.6.0/pyproject.toml
+-rw-r--r--   0 wpk      (42033)    36681       38 2023-08-01 20:26:44.657328 module-utilities-0.6.0/setup.cfg
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.561557 module-utilities-0.6.0/src/
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.638350 module-utilities-0.6.0/src/module_utilities/
+-rw-r--r--   0 wpk      (42033)    36681      380 2023-08-01 20:26:00.000000 module-utilities-0.6.0/src/module_utilities/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681     3268 2023-08-01 20:26:00.000000 module-utilities-0.6.0/src/module_utilities/_doc.py
+-rw-r--r--   0 wpk      (42033)    36681     1657 2023-08-01 20:26:00.000000 module-utilities-0.6.0/src/module_utilities/_typing.py
+-rw-r--r--   0 wpk      (42033)    36681      160 2023-08-01 20:26:44.000000 module-utilities-0.6.0/src/module_utilities/_version.py
+-rw-r--r--   0 wpk      (42033)    36681     6557 2023-08-01 20:26:00.000000 module-utilities-0.6.0/src/module_utilities/attributedict.py
+-rw-r--r--   0 wpk      (42033)    36681    17212 2023-08-01 20:26:00.000000 module-utilities-0.6.0/src/module_utilities/cached.py
+-rw-r--r--   0 wpk      (42033)    36681    26554 2023-08-01 20:26:00.000000 module-utilities-0.6.0/src/module_utilities/docfiller.py
+-rw-r--r--   0 wpk      (42033)    36681     5776 2023-08-01 20:26:00.000000 module-utilities-0.6.0/src/module_utilities/docinherit.py
+-rw-r--r--   0 wpk      (42033)    36681      275 2023-08-01 20:26:00.000000 module-utilities-0.6.0/src/module_utilities/options.py
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-05-02 03:09:02.000000 module-utilities-0.6.0/src/module_utilities/py.typed
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.647760 module-utilities-0.6.0/src/module_utilities/vendored/
+-rw-r--r--   0 wpk      (42033)    36681     1298 2023-06-14 21:18:50.000000 module-utilities-0.6.0/src/module_utilities/vendored/LICENSE.txt
+-rw-r--r--   0 wpk      (42033)    36681       93 2023-06-14 21:18:50.000000 module-utilities-0.6.0/src/module_utilities/vendored/README.txt
+-rw-r--r--   0 wpk      (42033)    36681       24 2023-06-14 21:18:50.000000 module-utilities-0.6.0/src/module_utilities/vendored/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681    23449 2023-06-14 21:18:50.000000 module-utilities-0.6.0/src/module_utilities/vendored/docscrape.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.642990 module-utilities-0.6.0/src/module_utilities.egg-info/
+-rw-r--r--   0 wpk      (42033)    36681    10311 2023-08-01 20:26:44.000000 module-utilities-0.6.0/src/module_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 wpk      (42033)    36681     3645 2023-08-01 20:26:44.000000 module-utilities-0.6.0/src/module_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-08-01 20:26:44.000000 module-utilities-0.6.0/src/module_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 wpk      (42033)    36681      955 2023-08-01 20:26:44.000000 module-utilities-0.6.0/src/module_utilities.egg-info/requires.txt
+-rw-r--r--   0 wpk      (42033)    36681       17 2023-08-01 20:26:44.000000 module-utilities-0.6.0/src/module_utilities.egg-info/top_level.txt
+-rw-r--r--   0 wpk      (42033)    36681        1 2023-05-04 19:05:27.000000 module-utilities-0.6.0/src/module_utilities.egg-info/zip-safe
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.653480 module-utilities-0.6.0/tests/
+-rw-r--r--   0 wpk      (42033)    36681       46 2023-04-27 23:45:36.000000 module-utilities-0.6.0/tests/__init__.py
+-rw-r--r--   0 wpk      (42033)    36681        0 2023-04-27 23:45:36.000000 module-utilities-0.6.0/tests/conftest.py
+-rw-r--r--   0 wpk      (42033)    36681     2199 2023-08-01 20:26:00.000000 module-utilities-0.6.0/tests/test_attributedict.py
+-rw-r--r--   0 wpk      (42033)    36681    14300 2023-08-01 20:26:00.000000 module-utilities-0.6.0/tests/test_cached.py
+-rw-r--r--   0 wpk      (42033)    36681    14004 2023-08-01 20:26:00.000000 module-utilities-0.6.0/tests/test_docfiller.py
+-rw-r--r--   0 wpk      (42033)    36681    17498 2023-08-01 20:26:00.000000 module-utilities-0.6.0/tests/test_inherit.py
+-rw-r--r--   0 wpk      (42033)    36681      190 2023-08-01 20:26:00.000000 module-utilities-0.6.0/tests/test_module_utilities.py
+drwxr-xr-x   0 wpk      (42033)    36681        0 2023-08-01 20:26:44.654567 module-utilities-0.6.0/tools/
+-rw-r--r--   0 wpk      (42033)    36681    24357 2023-08-01 20:26:00.000000 module-utilities-0.6.0/tools/noxtools.py
```

### Comparing `module-utilities-0.5.0/.cruft.json` & `module-utilities-0.6.0/.cruft.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'b55db074cda402d62ebaad27e1f191ad0c27bf4f'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": "feature/nox",
-    "commit": "c205c8acb0c3f69df17cbdfc00c03f806e0eef9b",
+    "commit": "b55db074cda402d62ebaad27e1f191ad0c27bf4f",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "*.html",
                 "docs/_templates/*.rst",
                 "docs/_templates/autosummary/*.rst",
                 "docs/_templates/autodocsumm/*.rst",
```

### Comparing `module-utilities-0.5.0/.editorconfig` & `module-utilities-0.6.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/.gitignore` & `module-utilities-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/.pre-commit-config.yaml` & `module-utilities-0.6.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0"
     hooks:
       - id: prettier
         stages: [commit]
         additional_dependencies:
           - prettier-plugin-toml
+        exclude: ^environment/lock/.*[.]yaml
   #** markdown
   - repo: https://github.com/DavidAnson/markdownlint-cli2
     rev: v0.8.1
     hooks:
       - id: markdownlint-cli2
         args: ["--style prettier"]
   #* Linting
```

### Comparing `module-utilities-0.5.0/.recipe-append.yaml` & `module-utilities-0.6.0/.recipe-append.yaml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/CHANGELOG.md` & `module-utilities-0.6.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 ## Unreleased
 
 See the fragment files in
 [changelog.d](https://github.com/usnistgov/module-utilities)
 
 <!-- scriv-insert-here -->
 
+## v0.6.0 — 2023-08-01
+
+### Added
+
+- Now include module `docinhert` to interface with
+  [docstring-inheritance](https://github.com/AntoineD/docstring-inheritance)
+- Fully support mypy and pyright type checking.
+
 ## v0.5.0 — 2023-07-10
 
 ### Added
 
 - Add `_prepend` option to docfiller. Default behavior is now to append current
   docstring to templates.
```

### Comparing `module-utilities-0.5.0/CONTRIBUTING.md` & `module-utilities-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/LICENSE` & `module-utilities-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/Makefile` & `module-utilities-0.6.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -169,20 +169,20 @@
 
 ################################################################################
 # NOX
 ###############################################################################
 ## dev env
 NOX=nox
 .PHONY: dev-env
-dev-env: environment/dev.yaml ## create development environment using nox
+dev-env: environment/py310-dev.yaml ## create development environment using nox
 	$(NOX) -e dev
 
 ## testing
 .PHONY: test-all
-test-all: environment/test.yaml ## run tests on every Python version with nox.
+test-all: environment/py310-test.yaml ## run tests on every Python version with nox.
 	$(NOX) -s test
 
 ## docs
 .PHONY: docs-build docs-release docs-clean docs-command
 docs-build: ## build docs in isolation
 	$(NOX) -s docs -- -d build
 docs-clean: ## clean docs
@@ -201,51 +201,51 @@
 docs-livehtml: ## use autobuild for docs
 	$(NOX) -s docs -- -d livehtml
 docs-open: ## open the build
 	$(NOX) -s docs -- -d open
 docs-linkcheck: ## check links
 	$(NOX) -s docs -- -d linkcheck
 
-docs-build docs-release docs-command docs-clean docs-livehtml docs-linkcheck: environment/docs.yaml
+docs-build docs-release docs-command docs-clean docs-livehtml docs-linkcheck: environment/py310-docs.yaml
 
 ## typing
 .PHONY: typing-mypy typing-pyright typing-pytype typing-all typing-command
 typing-mypy: ## run mypy mypy_args=...
 	$(NOX) -s typing -- -m mypy
 typing-pyright: ## run pyright pyright_args=...
 	$(NOX) -s typing -- -m pyright
 typing-pytype: ## run pytype pytype_args=...
 	$(NOX) -s typing -- -m pytype
 typing-all:
 	$(NOX) -s typing -- -m mypy pyright pytype
 typing-command:
 	$(NOX) -s typing -- --typing-run $(command)
-typing-mypy typing-pyright typing-pytype typing-all typing-command: environment/typing.yaml
+typing-mypy typing-pyright typing-pytype typing-all typing-command: environment/py310-typing.yaml
 
 ## distribution
 .PHONY: dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command
 
 dist-pypi-build: ## build dist
 	$(NOX) -s dist-pypi -- -p build
 dist-pypi-testrelease: ## test release on testpypi
 	$(NOX) -s dist-pypi -- -p testrelease
 dist-pypi-release: ## release to pypi, can pass posargs=...
 	$(NOX) -s dist-pypi -- -p release
 dist-pypi-command: ## run command with command=...
 	$(NOX) -s dist-pypi -- --dist-pypi-run $(command)
-dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command: environment/dist-pypi.yaml
+dist-pypi-build dist-pypi-testrelease dist-pypi-release dist-pypi-command: environment/py310-dist-pypi.yaml
 
 .PHONY: dist-conda-recipe dist-conda-build dist-conda-command
 dist-conda-recipe: ## build conda recipe can pass posargs=...
 	$(NOX) -s dist-conda -- -c recipe
 dist-conda-build: ## build conda recipe can pass posargs=...
 	$(NOX) -s dist-conda -- -c build
 dist-conda-command: ## run command with command=...
 	$(NOX) -s dist-conda -- -dist-conda-run $(command)
-dist-conda-build dist-conda-recipe dist-conda-command: environment/dist-conda.yaml
+dist-conda-build dist-conda-recipe dist-conda-command: environment/py310-dist-conda.yaml
 
 
 ## list all options
 .PHONY: nox-list
 nox-list:
 	$(NOX) --list
```

### Comparing `module-utilities-0.5.0/PKG-INFO` & `module-utilities-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-utilities
-Version: 0.5.0
+Version: 0.6.0
 Summary: Collection of utilities to aid working with python modules.
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/module-utilities
 Project-URL: documentation, https://pages.nist.gov/module-utilities/
 Keywords: module-utilities
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,25 +16,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: inherit
+Provides-Extra: opt-all
+Provides-Extra: test-extras
 Provides-Extra: test
 Provides-Extra: dev-extras
 Provides-Extra: typing-extras
 Provides-Extra: typing
 Provides-Extra: nox
 Provides-Extra: dev
 Provides-Extra: tools
 Provides-Extra: dev-complete
 Provides-Extra: docs
 Provides-Extra: dist-pypi
 Provides-Extra: dist-conda
+Provides-Extra: test-noopt
 License-File: LICENSE
 
 <!-- markdownlint-disable MD041 -->
 
 [![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
@@ -80,14 +84,20 @@
   a standard python dictionary for storage. Future versions will hopefully
   integrate with something like [cachetools].
 
 - `docfiller`: A module to share documentation. This is addapted from the
   [pandas `doc` decorator](https://github.com/pandas-dev/pandas/blob/main/pandas/util/_decorators.py).
   There are some convenience functions and classes for sharing documentation.
 
+- `docinhert`: An interface to [docstring-inheritance] module. This can be
+  combined with `docfiller` to make creating related function/class
+  documentation easy.
+
+[docstring-inheritance]: https://github.com/AntoineD/docstring-inheritance
+
 ## Status
 
 This package is actively used by the author. Please feel free to create a pull
 request for wanted features and suggestions!
 
 ## Quick start
 
@@ -99,14 +109,23 @@
 
 or
 
 ```bash
 conda install -c conda-forge module-utilities
 ```
 
+Optionally, you can install [docstring-inheritance] to use the `docinherit`
+module:
+
+```base
+pip install docstring-inheritance
+# or
+conda install -c conda-forge docstring-inheritance
+```
+
 ## Example usage
 
 Simple example of using `cached` module.
 
 ```pycon
 >>> from module_utilities import cached
 >>>
@@ -146,15 +165,15 @@
 [1]
 
 ```
 
 Simple example of using `DocFiller`.
 
 ```pycon
->>> from module_utilities.docfiller import DocFiller
+>>> from module_utilities.docfiller import DocFiller, indent_docstring
 >>> d = DocFiller.from_docstring(
 ...     """
 ...     Parameters
 ...     ----------
 ...     x : int
 ...         x param
 ...     y : int
@@ -184,27 +203,27 @@
 ...     {z0}
 ...     Returns
 ...     --------
 ...     {returns.output0}
 ...     """
 ...     return x + y + z
 ...
->>> print(func.__doc__.strip())
-Parameters
-----------
-x : int
-    x param
-y : int
-    y param
-z : int
-    z int param
-Returns
---------
-output : int
-    Integer output.
+>>> print(indent_docstring(func))
++  Parameters
++  ----------
++  x : int
++      x param
++  y : int
++      y param
++  z : int
++      z int param
++  Returns
++  --------
++  output : int
++      Integer output.
 
 # Note that for python version <= 3.8 that method chaining
 # in decorators doesn't work, so have to do the following.
 # For newer python, you can inline this.
 >>> dd = d.assign_keys(z='z0', out='returns.output0')
 >>> @dd.decorate
 ... def func1(x, y, z):
@@ -216,46 +235,46 @@
 ...     {z}
 ...     Returns
 ...     -------
 ...     {out}
 ...     """
 ...     pass
 ...
->>> print(func1.__doc__.strip())
-Parameters
-----------
-x : int
-    x param
-y : int
-    y param
-z : int
-    z int param
-Returns
--------
-output : int
-    Integer output.
+>>> print(indent_docstring(func1))
++  Parameters
++  ----------
++  x : int
++      x param
++  y : int
++      y param
++  z : int
++      z int param
++  Returns
++  -------
++  output : int
++      Integer output.
 
 >>> dd = d.assign_keys(z='z1', out='returns.output1')
 >>> @dd(func1)
 ... def func2(x, y, z):
 ...     pass
 
->>> print(func2.__doc__.strip())
-Parameters
-----------
-x : int
-    x param
-y : int
-    y param
-z : float
-    z float param
-Returns
--------
-output : float
-    Float output
+>>> print(indent_docstring(func2))
++  Parameters
++  ----------
++  x : int
++      x param
++  y : int
++      y param
++  z : float
++      z float param
++  Returns
++  -------
++  output : float
++      Float output
 
 
 ```
 
 <!-- end-docs -->
 
 ## Documentation
@@ -278,15 +297,15 @@
 [cmomy]: https://github.com/usnistgov/cmomy
 [analphipy]: https://github.com/usnistgov/analphipy
 [tmmc-lnpy]: https://github.com/usnistgov/tmmc-lnpy
 [thermoextrap]: https://github.com/usnistgov/thermoextrap
 
 ## Contact
 
-The author can be reached at wpk@nist.gov.
+The author can be reached at <wpk@nist.gov>.
 
 ## Credits
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
 Project template forked from
@@ -301,14 +320,22 @@
 ## Unreleased
 
 See the fragment files in
 [changelog.d](https://github.com/usnistgov/module-utilities)
 
 <!-- scriv-insert-here -->
 
+## v0.6.0 — 2023-08-01
+
+### Added
+
+- Now include module `docinhert` to interface with
+  [docstring-inheritance](https://github.com/AntoineD/docstring-inheritance)
+- Fully support mypy and pyright type checking.
+
 ## v0.5.0 — 2023-07-10
 
 ### Added
 
 - Add `_prepend` option to docfiller. Default behavior is now to append current
   docstring to templates.
```

### Comparing `module-utilities-0.5.0/README.md` & `module-utilities-0.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -45,14 +45,20 @@
   a standard python dictionary for storage. Future versions will hopefully
   integrate with something like [cachetools].
 
 - `docfiller`: A module to share documentation. This is addapted from the
   [pandas `doc` decorator](https://github.com/pandas-dev/pandas/blob/main/pandas/util/_decorators.py).
   There are some convenience functions and classes for sharing documentation.
 
+- `docinhert`: An interface to [docstring-inheritance] module. This can be
+  combined with `docfiller` to make creating related function/class
+  documentation easy.
+
+[docstring-inheritance]: https://github.com/AntoineD/docstring-inheritance
+
 ## Status
 
 This package is actively used by the author. Please feel free to create a pull
 request for wanted features and suggestions!
 
 ## Quick start
 
@@ -64,14 +70,23 @@
 
 or
 
 ```bash
 conda install -c conda-forge module-utilities
 ```
 
+Optionally, you can install [docstring-inheritance] to use the `docinherit`
+module:
+
+```base
+pip install docstring-inheritance
+# or
+conda install -c conda-forge docstring-inheritance
+```
+
 ## Example usage
 
 Simple example of using `cached` module.
 
 ```pycon
 >>> from module_utilities import cached
 >>>
@@ -111,15 +126,15 @@
 [1]
 
 ```
 
 Simple example of using `DocFiller`.
 
 ```pycon
->>> from module_utilities.docfiller import DocFiller
+>>> from module_utilities.docfiller import DocFiller, indent_docstring
 >>> d = DocFiller.from_docstring(
 ...     """
 ...     Parameters
 ...     ----------
 ...     x : int
 ...         x param
 ...     y : int
@@ -149,27 +164,27 @@
 ...     {z0}
 ...     Returns
 ...     --------
 ...     {returns.output0}
 ...     """
 ...     return x + y + z
 ...
->>> print(func.__doc__.strip())
-Parameters
-----------
-x : int
-    x param
-y : int
-    y param
-z : int
-    z int param
-Returns
---------
-output : int
-    Integer output.
+>>> print(indent_docstring(func))
++  Parameters
++  ----------
++  x : int
++      x param
++  y : int
++      y param
++  z : int
++      z int param
++  Returns
++  --------
++  output : int
++      Integer output.
 
 # Note that for python version <= 3.8 that method chaining
 # in decorators doesn't work, so have to do the following.
 # For newer python, you can inline this.
 >>> dd = d.assign_keys(z='z0', out='returns.output0')
 >>> @dd.decorate
 ... def func1(x, y, z):
@@ -181,46 +196,46 @@
 ...     {z}
 ...     Returns
 ...     -------
 ...     {out}
 ...     """
 ...     pass
 ...
->>> print(func1.__doc__.strip())
-Parameters
-----------
-x : int
-    x param
-y : int
-    y param
-z : int
-    z int param
-Returns
--------
-output : int
-    Integer output.
+>>> print(indent_docstring(func1))
++  Parameters
++  ----------
++  x : int
++      x param
++  y : int
++      y param
++  z : int
++      z int param
++  Returns
++  -------
++  output : int
++      Integer output.
 
 >>> dd = d.assign_keys(z='z1', out='returns.output1')
 >>> @dd(func1)
 ... def func2(x, y, z):
 ...     pass
 
->>> print(func2.__doc__.strip())
-Parameters
-----------
-x : int
-    x param
-y : int
-    y param
-z : float
-    z float param
-Returns
--------
-output : float
-    Float output
+>>> print(indent_docstring(func2))
++  Parameters
++  ----------
++  x : int
++      x param
++  y : int
++      y param
++  z : float
++      z float param
++  Returns
++  -------
++  output : float
++      Float output
 
 
 ```
 
 <!-- end-docs -->
 
 ## Documentation
@@ -243,15 +258,15 @@
 [cmomy]: https://github.com/usnistgov/cmomy
 [analphipy]: https://github.com/usnistgov/analphipy
 [tmmc-lnpy]: https://github.com/usnistgov/tmmc-lnpy
 [thermoextrap]: https://github.com/usnistgov/thermoextrap
 
 ## Contact
 
-The author can be reached at wpk@nist.gov.
+The author can be reached at <wpk@nist.gov>.
 
 ## Credits
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
 Project template forked from
```

### Comparing `module-utilities-0.5.0/changelog.d/templates/auto-changelog/template.jinja2` & `module-utilities-0.6.0/changelog.d/templates/auto-changelog/template.jinja2`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/Makefile` & `module-utilities-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/_static/css/nist-combined.css` & `module-utilities-0.6.0/docs/_static/css/nist-combined.css`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/_static/js/leave_notice.js` & `module-utilities-0.6.0/docs/_static/js/leave_notice.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/_static/js/nist-header-footer.js` & `module-utilities-0.6.0/docs/_static/js/nist-header-footer.js`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/_templates/autosummary/class.rst` & `module-utilities-0.6.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/_templates/autosummary/module.rst` & `module-utilities-0.6.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/_templates/class-individual-pages.rst` & `module-utilities-0.6.0/docs/_templates/class-individual-pages.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/_templates/class-single-page.rst` & `module-utilities-0.6.0/docs/_templates/class-single-page.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/_templates/custom-module-template.rst` & `module-utilities-0.6.0/docs/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/_templates/module-custom-imported.rst` & `module-utilities-0.6.0/docs/_templates/module-custom-imported.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/_templates/module-custom.rst` & `module-utilities-0.6.0/docs/_templates/module-custom.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/_templates/module-single.rst` & `module-utilities-0.6.0/docs/_templates/module-single.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/_templates/module-template.rst` & `module-utilities-0.6.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/conf.py` & `module-utilities-0.6.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,16 @@
     "sphinx_copybutton",
     ## redirect stuff?
     # "sphinxext.rediraffe",
     ## pretty things up?
     # "sphinx_design"
     ## myst stuff
     "myst_nb",
+    ## type hings
+    # "sphinx_autodoc_typehints",
 ]
 
 nitpicky = True
 autosectionlabel_prefix_document = True
 
 # -- myst stuff ---------------------------------------------------------
 myst_enable_extensions = [
@@ -139,14 +141,16 @@
     "members",
     "inherited-members",
     "private-members",
     "show-inheritance",
 ]
 autodoc_typehints = "none"
 
+autodoc_type_aliases = {"NestedMap": "module_utilities._typing.NestedMap"}
+
 # -- napoleon ------------------------------------------------------------------
 napoleon_google_docstring = False
 napoleon_numpy_docstring = True
 
 napoleon_use_param = False
 napoleon_use_rtype = False
 napoleon_preprocess_types = True
@@ -202,14 +206,15 @@
     "DataFrame": "~pandas.DataFrame",
     "Categorical": "~pandas.Categorical",
     "Path": "~~pathlib.Path",
     # objects with abbreviated namespace (from pandas)
     "pd.Index": "~pandas.Index",
     "pd.NaT": "~pandas.NaT",
     "DocFiller": "~module_utilities.docfiller.DocFiller",
+    "NestedMap": "~module_utilities._typing.NestedMap",
 }
 
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
```

### Comparing `module-utilities-0.5.0/docs/examples/usage/cached.ipynb` & `module-utilities-0.6.0/docs/examples/usage/cached.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/docs/examples/usage/docfiller.ipynb` & `module-utilities-0.6.0/docs/examples/usage/docfiller.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9596664186507936%*

 * *Differences: {"'cells'": "{22: {'execution_count': 12}, 23: {'execution_count': 13}, insert: [(24, "*

 * *            "OrderedDict([('cell_type', 'markdown'), ('id', 'cf9afec1'), ('metadata', "*

 * *            'OrderedDict()), (\'source\', ["There are cases where you\'d like to update the '*

 * *            'documentation from one implementation to another.  For example, say you have the '*

 * *            'following functions:"])])), (25, OrderedDict([(\'cell_type\', \'code\'), '*

 * *            "('execution_count', 15), ('id', '57942b42'),  […]*

```diff
@@ -671,15 +671,15 @@
                 "## Works with classes\n",
                 "\n",
                 "This also works with classes"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 12,
             "id": "bf6b8405",
             "metadata": {},
             "outputs": [],
             "source": [
                 "expected = \"\"\"\n",
                 "A summary\n",
                 "\n",
@@ -700,15 +700,15 @@
                 "\"\"\"\n",
                 "\n",
                 "d = DocFiller.from_docstring(expected, combine_keys=\"parameters\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 13,
             "id": "2eb1580a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -770,33 +770,303 @@
                 "    pass\n",
                 "\n",
                 "\n",
                 "assert hello2.__doc__ == expected\n",
                 "\n",
                 "help(hello)"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "cf9afec1",
+            "metadata": {},
+            "source": [
+                "There are cases where you'd like to update the documentation from one implementation to another.  For example, say you have the following functions:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 15,
+            "id": "57942b42",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n",
+                        "Add numbers\n",
+                        "\n",
+                        "Parameters\n",
+                        "----------\n",
+                        "x : float\n",
+                        "    x param\n",
+                        "    some other stuff\n",
+                        "y : float\n",
+                        "    y param\n",
+                        "\n",
+                        "Returns\n",
+                        "-------\n",
+                        "output : float\n",
+                        "    Sum of input\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "@d.decorate\n",
+                "def func_xy(x, y):\n",
+                "    \"\"\"\n",
+                "    Add numbers\n",
+                "\n",
+                "\n",
+                "    Parameters\n",
+                "    ----------\n",
+                "    {x}\n",
+                "    {y}\n",
+                "\n",
+                "\n",
+                "    Returns\n",
+                "    -------\n",
+                "    output : float\n",
+                "        Sum of input\n",
+                "    \"\"\"\n",
+                "\n",
+                "    return x + y\n",
+                "\n",
+                "\n",
+                "print(func_xy.__doc__)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "16db1a4c",
+            "metadata": {},
+            "source": [
+                "But what if you want a new version that adds three numbers `func_xyz(x, y, z)`?  Most everything is the same as for `func_xy` above, but we need to add `z`.  For this, we have an interface to [docstring-inheritance](https://github.com/AntoineD/docstring-inheritance)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 17,
+            "id": "d018e5ac",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Add numbers\n",
+                        "\n",
+                        "Parameters\n",
+                        "----------\n",
+                        "x : float\n",
+                        "    x param\n",
+                        "    some other stuff\n",
+                        "y : float\n",
+                        "    y param\n",
+                        "z : float\n",
+                        "    Another parameter\n",
+                        "\n",
+                        "Returns\n",
+                        "-------\n",
+                        "output : float\n",
+                        "    Sum of input\n"
+                    ]
+                }
+            ],
+            "source": [
+                "@d.inherit(func_xy)\n",
+                "def func_xyz(x, y, z):\n",
+                "    \"\"\"\n",
+                "    Parameters\n",
+                "    ----------\n",
+                "    z : float\n",
+                "        Another parameter\n",
+                "    \"\"\"\n",
+                "    return x + y + z\n",
+                "\n",
+                "\n",
+                "print(func_xyz.__doc__)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "576e8513",
+            "metadata": {},
+            "source": [
+                "For the special case that you want to inherit from methods of a baseclass, you can use the following:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 22,
+            "id": "58e5a50f",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "class Base:\n",
+                "    def prop(self):\n",
+                "        \"\"\"A property\"\"\"\n",
+                "        return 1\n",
+                "\n",
+                "    @d.decorate\n",
+                "    def meth(self, x):\n",
+                "        \"\"\"\n",
+                "        A method\n",
+                "\n",
+                "\n",
+                "        Parameters\n",
+                "        ----------\n",
+                "        {x}\n",
+                "\n",
+                "\n",
+                "        Returns\n",
+                "        -------\n",
+                "        float\n",
+                "            Double x\n",
+                "        \"\"\"\n",
+                "\n",
+                "        return x * 2\n",
+                "\n",
+                "\n",
+                "d_from_base = d.factory_inherit_from_parent(Base)\n",
+                "\n",
+                "\n",
+                "class Derived:\n",
+                "    @d_from_base()\n",
+                "    def prop(self):\n",
+                "        pass\n",
+                "\n",
+                "    @d_from_base()\n",
+                "    def meth(self, x, y):\n",
+                "        \"\"\"\n",
+                "        Parameters\n",
+                "        ----------\n",
+                "        {y}\n",
+                "        \"\"\"\n",
+                "        return (x + y) * 2"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 23,
+            "id": "f986e10a",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Help on class Base in module __main__:\n",
+                        "\n",
+                        "class Base(builtins.object)\n",
+                        " |  Methods defined here:\n",
+                        " |  \n",
+                        " |  meth(self, x)\n",
+                        " |      A method\n",
+                        " |      \n",
+                        " |      Parameters\n",
+                        " |      ----------\n",
+                        " |      x : float\n",
+                        " |          x param\n",
+                        " |          some other stuff\n",
+                        " |      \n",
+                        " |      Returns\n",
+                        " |      -------\n",
+                        " |      float\n",
+                        " |          Double x\n",
+                        " |  \n",
+                        " |  prop(self)\n",
+                        " |      A property\n",
+                        " |  \n",
+                        " |  ----------------------------------------------------------------------\n",
+                        " |  Data descriptors defined here:\n",
+                        " |  \n",
+                        " |  __dict__\n",
+                        " |      dictionary for instance variables (if defined)\n",
+                        " |  \n",
+                        " |  __weakref__\n",
+                        " |      list of weak references to the object (if defined)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "help(Base)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 24,
+            "id": "9f7eaeef",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Help on class Derived in module __main__:\n",
+                        "\n",
+                        "class Derived(builtins.object)\n",
+                        " |  Methods defined here:\n",
+                        " |  \n",
+                        " |  meth(self, x, y)\n",
+                        " |      A method\n",
+                        " |      \n",
+                        " |      Parameters\n",
+                        " |      ----------\n",
+                        " |      x : float\n",
+                        " |          x param\n",
+                        " |          some other stuff\n",
+                        " |      y : float\n",
+                        " |          y param\n",
+                        " |      \n",
+                        " |      Returns\n",
+                        " |      -------\n",
+                        " |      float\n",
+                        " |          Double x\n",
+                        " |  \n",
+                        " |  prop(self)\n",
+                        " |      A property\n",
+                        " |  \n",
+                        " |  ----------------------------------------------------------------------\n",
+                        " |  Data descriptors defined here:\n",
+                        " |  \n",
+                        " |  __dict__\n",
+                        " |      dictionary for instance variables (if defined)\n",
+                        " |  \n",
+                        " |  __weakref__\n",
+                        " |      list of weak references to the object (if defined)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "help(Derived)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "module-utilities-dev [conda env:dev-3]",
+            "display_name": "module-utilities-dev [conda env:dev-4]",
             "language": "python",
-            "name": "conda-env-dev-3-py"
+            "name": "conda-env-dev-4-py"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.10.12"
         },
         "toc": {
             "base_numbering": 1,
             "nav_menu": {},
             "number_sections": true,
             "sideBar": true,
             "skip_h1_title": false,
```

### Comparing `module-utilities-0.5.0/docs/installation.md` & `module-utilities-0.6.0/docs/installation.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,23 @@
 ```bash
 conda install -c conda-forge module-utilities
 ```
 
 This is the preferred method to install module-utilities, as it will always
 install the most recent stable release.
 
+Optionally, you can install
+[docstring-inheritance](https://github.com/AntoineD/docstring-inheritance) with
+
+```base
+pip install docstring-inheritance
+# or
+conda install -c conda-forge docstring-inheritance
+```
+
 ## From sources
 
 The sources for module-utilities can be downloaded from the [Github repo].
 
 You can either clone the public repository:
 
 ```bash
```

### Comparing `module-utilities-0.5.0/docs/make.bat` & `module-utilities-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/environment/lock/py310-dev-conda-lock.yml` & `module-utilities-0.6.0/environment/lock/py310-dev-conda-lock.yml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/environment/lock/py310-dist-conda-conda-lock.yml` & `module-utilities-0.6.0/environment/lock/py310-dist-conda-conda-lock.yml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/environment/lock/py310-dist-pypi-conda-lock.yml` & `module-utilities-0.6.0/environment/lock/py310-dist-pypi-conda-lock.yml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/environment/lock/py310-test-conda-lock.yml` & `module-utilities-0.6.0/environment/lock/py310-test-conda-lock.yml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/environment/lock/py310-typing-conda-lock.yml` & `module-utilities-0.6.0/environment/lock/py310-typing-conda-lock.yml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/environment/lock/py311-test-conda-lock.yml` & `module-utilities-0.6.0/environment/lock/py311-test-conda-lock.yml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/environment/lock/py311-typing-conda-lock.yml` & `module-utilities-0.6.0/environment/lock/py311-typing-conda-lock.yml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/environment/lock/py38-test-conda-lock.yml` & `module-utilities-0.6.0/environment/lock/py38-test-conda-lock.yml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/environment/lock/py38-typing-conda-lock.yml` & `module-utilities-0.6.0/environment/lock/py38-typing-conda-lock.yml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/environment/lock/py39-test-conda-lock.yml` & `module-utilities-0.6.0/environment/lock/py39-test-conda-lock.yml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/environment/lock/py39-typing-conda-lock.yml` & `module-utilities-0.6.0/environment/lock/py39-typing-conda-lock.yml`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/examples/usage/cached.ipynb` & `module-utilities-0.6.0/examples/usage/cached.ipynb`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/examples/usage/docfiller.ipynb` & `module-utilities-0.6.0/examples/usage/docfiller.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9596664186507936%*

 * *Differences: {"'cells'": "{22: {'execution_count': 12}, 23: {'execution_count': 13}, insert: [(24, "*

 * *            "OrderedDict([('cell_type', 'markdown'), ('id', 'cf9afec1'), ('metadata', "*

 * *            'OrderedDict()), (\'source\', ["There are cases where you\'d like to update the '*

 * *            'documentation from one implementation to another.  For example, say you have the '*

 * *            'following functions:"])])), (25, OrderedDict([(\'cell_type\', \'code\'), '*

 * *            "('execution_count', 15), ('id', '57942b42'),  […]*

```diff
@@ -671,15 +671,15 @@
                 "## Works with classes\n",
                 "\n",
                 "This also works with classes"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 12,
             "id": "bf6b8405",
             "metadata": {},
             "outputs": [],
             "source": [
                 "expected = \"\"\"\n",
                 "A summary\n",
                 "\n",
@@ -700,15 +700,15 @@
                 "\"\"\"\n",
                 "\n",
                 "d = DocFiller.from_docstring(expected, combine_keys=\"parameters\")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 13,
             "id": "2eb1580a",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -770,33 +770,303 @@
                 "    pass\n",
                 "\n",
                 "\n",
                 "assert hello2.__doc__ == expected\n",
                 "\n",
                 "help(hello)"
             ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "cf9afec1",
+            "metadata": {},
+            "source": [
+                "There are cases where you'd like to update the documentation from one implementation to another.  For example, say you have the following functions:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 15,
+            "id": "57942b42",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n",
+                        "Add numbers\n",
+                        "\n",
+                        "Parameters\n",
+                        "----------\n",
+                        "x : float\n",
+                        "    x param\n",
+                        "    some other stuff\n",
+                        "y : float\n",
+                        "    y param\n",
+                        "\n",
+                        "Returns\n",
+                        "-------\n",
+                        "output : float\n",
+                        "    Sum of input\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "@d.decorate\n",
+                "def func_xy(x, y):\n",
+                "    \"\"\"\n",
+                "    Add numbers\n",
+                "\n",
+                "\n",
+                "    Parameters\n",
+                "    ----------\n",
+                "    {x}\n",
+                "    {y}\n",
+                "\n",
+                "\n",
+                "    Returns\n",
+                "    -------\n",
+                "    output : float\n",
+                "        Sum of input\n",
+                "    \"\"\"\n",
+                "\n",
+                "    return x + y\n",
+                "\n",
+                "\n",
+                "print(func_xy.__doc__)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "16db1a4c",
+            "metadata": {},
+            "source": [
+                "But what if you want a new version that adds three numbers `func_xyz(x, y, z)`?  Most everything is the same as for `func_xy` above, but we need to add `z`.  For this, we have an interface to [docstring-inheritance](https://github.com/AntoineD/docstring-inheritance)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 17,
+            "id": "d018e5ac",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Add numbers\n",
+                        "\n",
+                        "Parameters\n",
+                        "----------\n",
+                        "x : float\n",
+                        "    x param\n",
+                        "    some other stuff\n",
+                        "y : float\n",
+                        "    y param\n",
+                        "z : float\n",
+                        "    Another parameter\n",
+                        "\n",
+                        "Returns\n",
+                        "-------\n",
+                        "output : float\n",
+                        "    Sum of input\n"
+                    ]
+                }
+            ],
+            "source": [
+                "@d.inherit(func_xy)\n",
+                "def func_xyz(x, y, z):\n",
+                "    \"\"\"\n",
+                "    Parameters\n",
+                "    ----------\n",
+                "    z : float\n",
+                "        Another parameter\n",
+                "    \"\"\"\n",
+                "    return x + y + z\n",
+                "\n",
+                "\n",
+                "print(func_xyz.__doc__)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "576e8513",
+            "metadata": {},
+            "source": [
+                "For the special case that you want to inherit from methods of a baseclass, you can use the following:"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 22,
+            "id": "58e5a50f",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "class Base:\n",
+                "    def prop(self):\n",
+                "        \"\"\"A property\"\"\"\n",
+                "        return 1\n",
+                "\n",
+                "    @d.decorate\n",
+                "    def meth(self, x):\n",
+                "        \"\"\"\n",
+                "        A method\n",
+                "\n",
+                "\n",
+                "        Parameters\n",
+                "        ----------\n",
+                "        {x}\n",
+                "\n",
+                "\n",
+                "        Returns\n",
+                "        -------\n",
+                "        float\n",
+                "            Double x\n",
+                "        \"\"\"\n",
+                "\n",
+                "        return x * 2\n",
+                "\n",
+                "\n",
+                "d_from_base = d.factory_inherit_from_parent(Base)\n",
+                "\n",
+                "\n",
+                "class Derived:\n",
+                "    @d_from_base()\n",
+                "    def prop(self):\n",
+                "        pass\n",
+                "\n",
+                "    @d_from_base()\n",
+                "    def meth(self, x, y):\n",
+                "        \"\"\"\n",
+                "        Parameters\n",
+                "        ----------\n",
+                "        {y}\n",
+                "        \"\"\"\n",
+                "        return (x + y) * 2"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 23,
+            "id": "f986e10a",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Help on class Base in module __main__:\n",
+                        "\n",
+                        "class Base(builtins.object)\n",
+                        " |  Methods defined here:\n",
+                        " |  \n",
+                        " |  meth(self, x)\n",
+                        " |      A method\n",
+                        " |      \n",
+                        " |      Parameters\n",
+                        " |      ----------\n",
+                        " |      x : float\n",
+                        " |          x param\n",
+                        " |          some other stuff\n",
+                        " |      \n",
+                        " |      Returns\n",
+                        " |      -------\n",
+                        " |      float\n",
+                        " |          Double x\n",
+                        " |  \n",
+                        " |  prop(self)\n",
+                        " |      A property\n",
+                        " |  \n",
+                        " |  ----------------------------------------------------------------------\n",
+                        " |  Data descriptors defined here:\n",
+                        " |  \n",
+                        " |  __dict__\n",
+                        " |      dictionary for instance variables (if defined)\n",
+                        " |  \n",
+                        " |  __weakref__\n",
+                        " |      list of weak references to the object (if defined)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "help(Base)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 24,
+            "id": "9f7eaeef",
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Help on class Derived in module __main__:\n",
+                        "\n",
+                        "class Derived(builtins.object)\n",
+                        " |  Methods defined here:\n",
+                        " |  \n",
+                        " |  meth(self, x, y)\n",
+                        " |      A method\n",
+                        " |      \n",
+                        " |      Parameters\n",
+                        " |      ----------\n",
+                        " |      x : float\n",
+                        " |          x param\n",
+                        " |          some other stuff\n",
+                        " |      y : float\n",
+                        " |          y param\n",
+                        " |      \n",
+                        " |      Returns\n",
+                        " |      -------\n",
+                        " |      float\n",
+                        " |          Double x\n",
+                        " |  \n",
+                        " |  prop(self)\n",
+                        " |      A property\n",
+                        " |  \n",
+                        " |  ----------------------------------------------------------------------\n",
+                        " |  Data descriptors defined here:\n",
+                        " |  \n",
+                        " |  __dict__\n",
+                        " |      dictionary for instance variables (if defined)\n",
+                        " |  \n",
+                        " |  __weakref__\n",
+                        " |      list of weak references to the object (if defined)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "help(Derived)"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "module-utilities-dev [conda env:dev-3]",
+            "display_name": "module-utilities-dev [conda env:dev-4]",
             "language": "python",
-            "name": "conda-env-dev-3-py"
+            "name": "conda-env-dev-4-py"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.10.12"
         },
         "toc": {
             "base_numbering": 1,
             "nav_menu": {},
             "number_sections": true,
             "sideBar": true,
             "skip_h1_title": false,
```

### Comparing `module-utilities-0.5.0/noxfile.py` & `module-utilities-0.6.0/noxfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,26 @@
-"""Config file for nox"""
+"""Config file for nox."""
 from __future__ import annotations
 
 import shutil
 from dataclasses import replace  # noqa
+from itertools import product
 from pathlib import Path
 from textwrap import dedent
-from typing import Annotated, Any, Callable, Collection, TypeVar, cast
+from typing import (
+    Annotated,
+    Any,
+    Callable,
+    Collection,
+    Literal,
+    Sequence,
+    TypeAlias,
+    TypeVar,
+    cast,
+)
 
 import nox
 from noxopt import NoxOpt, Option, Session
 
 from tools.noxtools import (
     combine_list_str,
     load_nox_config,
@@ -55,21 +66,21 @@
 
 CONFIG = load_nox_config()
 
 # * noxopt -----------------------------------------------------------------------------
 group = NoxOpt(auto_tag=True)
 
 F = TypeVar("F", bound=Callable[..., Any])
-C = Callable[[F], F]
+C: TypeAlias = Callable[[F], F]
 
-DEFAULT_SESSION = cast(C, group.session(**SESSION_DEFAULT_KWS))  # type: ignore
-ALL_SESSION = cast(C, group.session(**SESSION_ALL_KWS))  # type: ignore
+DEFAULT_SESSION = cast(C[F], group.session(**SESSION_DEFAULT_KWS))  # type: ignore
+ALL_SESSION = cast(C[F], group.session(**SESSION_ALL_KWS))  # type: ignore
 
-DEFAULT_SESSION_VENV = cast(C, group.session(python=PYTHON_DEFAULT_VERSION))  # type: ignore
-ALL_SESSION_VENV = cast(C, group.session(python=PYTHON_ALL_VERSIONS))  # type: ignore
+DEFAULT_SESSION_VENV = cast(C[F], group.session(python=PYTHON_DEFAULT_VERSION))  # type: ignore
+ALL_SESSION_VENV = cast(C[F], group.session(python=PYTHON_ALL_VERSIONS))  # type: ignore
 
 OPTS_OPT = Option(nargs="*", type=str)
 # SET_KERNEL_OPT = Option(type=bool, help="If True, try to set the kernel name")
 RUN_OPT = Option(
     nargs="*",
     type=str,
     action="append",
@@ -116,44 +127,82 @@
         type=bool,
         help="If flag included, log python and package (if installed) version",
     ),
 ]
 
 
 # * Installation command ---------------------------------------------------------------
+def py_prefix(python_version: Any) -> str:
+    if isinstance(python_version, str):
+        return "py" + python_version.replace(".", "")
+    else:
+        raise ValueError(f"passed non-string value {python_version}")
+
+
+def session_environment_filename(
+    name: str,
+    ext: str | None = None,
+    python_version=None,
+) -> str:
+    if name is None:
+        raise ValueError("must supply name")
+
+    filename = name
+    if ext is not None:
+        filename = filename + ext
+    if python_version is not None:
+        filename = f"{py_prefix(python_version)}-{filename}"
+    return f"./environment/{filename}"
+
+
 def pkg_install_condaenv(
     session: nox.Session,
     name: str,
     lock: bool = False,
     display_name: str | None = None,
     install_package: bool = True,
     force_reinstall: bool = False,
     log_session: bool = False,
     deps: Collection[str] | None = None,
     reqs: Collection[str] | None = None,
     channels: Collection[str] | None = None,
+    filename: str | None = None,
     **kwargs,
 ):
-    """Install requirements.  If need fine control, do it in calling func"""
+    """Install requirements.  If need fine control, do it in calling func."""
+
+    def check_filename(filename):
+        if not Path(filename).exists():
+            raise ValueError(f"file {filename} does not exist")
+        session.log(f"Environment file: {filename}")
+        return str(filename)
 
     if lock:
-        py = session.python.replace(".", "")  # type: ignore
+        filename = (
+            filename
+            or f"./environment/lock/{py_prefix(session.python)}-{name}-conda-lock.yml"
+        )
         session_install_envs_lock(
             session=session,
-            lockfile=f"./environment/lock/py{py}-{name}-conda-lock.yml",
+            lockfile=check_filename(filename),
             display_name=display_name,
             force_reinstall=force_reinstall,
             install_package=install_package,
             **kwargs,
         )
 
     else:
+        filename = filename or session_environment_filename(
+            name=name,
+            ext=".yaml",
+            python_version=session.python,
+        )
         session_install_envs(
             session,
-            f"./environment/{name}.yaml",
+            check_filename(filename),
             display_name=display_name,
             force_reinstall=force_reinstall,
             deps=deps,
             reqs=reqs,
             channels=channels,
             install_package=install_package,
             **kwargs,
@@ -218,15 +267,15 @@
 def dev(
     session: Session,
     dev_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
 ):
-    """Create dev env"""
+    """Create dev env."""
     # using conda
 
     pkg_install_condaenv(
         session=session,
         name="dev",
         lock=lock,
         display_name=f"{PACKAGE_NAME}-dev",
@@ -241,15 +290,15 @@
 def dev_venv(
     session: Session,
     dev_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
 ):
-    """Create dev env"""
+    """Create dev env."""
     # using conda
 
     pkg_install_venv(
         session=session,
         name="dev-venv",
         lock=lock,
         extras=["dev"],
@@ -272,55 +321,101 @@
     pkg_install_venv(
         session=session,
         name="pyporject2conda",
         reqs=["pyproject2conda>=0.4.0"],
         force_reinstall=force_reinstall,
     )
 
-    def create_env(output, extras=None, python="get", base=True, cmd="yaml"):
-        def _to_args(flag, val):
+    def create_env(
+        python_version: str | None = None,
+        cmd: Literal["yaml", "requirements"] = "yaml",
+        name: str | None = None,
+        output: str | None = None,
+        extras: str | Sequence[str] | None = None,
+        python_include: str | bool = True,
+        base: bool = True,
+    ):
+        def _to_args(flag: str, val: str | Sequence[str] | None) -> list[str]:
             if val is None:
                 return []
             if isinstance(val, str):
                 val = [val]
-            return prepend_flag(flag, val)
+            return prepend_flag(flag, *val)
+
+        if output is None:
+            assert name is not None
+            output = session_environment_filename(
+                python_version=python_version,
+                name=name,
+                ext={"yaml": ".yaml", "requirements": ".txt"}[cmd],
+            )
 
         if pyproject2conda_force or update_target(output, "pyproject.toml"):
             args = [cmd, "-o", output] + _to_args("-e", extras)
 
-            if python and cmd == "yaml":
-                args.extend(["--python-include", python])
+            if cmd == "yaml":
+                if python_version is not None:
+                    args.extend(["--python-version", python_version])
+                if isinstance(python_include, bool) and python_include:
+                    python_include = f"python={python_version}"
+                if isinstance(python_include, str):
+                    args.extend(["--python-include", python_include])
 
             if not base:
                 args.append("--no-base")
 
             session.run("pyproject2conda", *args)
         else:
             session.log(
                 f"{output} up to data.  Pass --pyproject2conda-force to force recreation"
             )
 
-    # create root environment
-    create_env("environment/base.yaml")
-
     extras = CONFIG["environment-extras"]
-    for k in ["test", "typing", "docs", "dev"]:
-        create_env(f"environment/{k}.yaml", extras=extras.get(k, k), base=True)
 
-    # isolated
-    for k in ["dist-pypi", "dist-conda"]:
-        create_env(f"environment/{k}.yaml", extras=k, base=False)
-        if k == "dist-pypi":
-            create_env(f"environment/{k}.txt", extras=k, base=False, cmd="requirements")
+    # All versions:
+    for env, python_version in product(
+        ["test", "typing", "test-noopt"], PYTHON_ALL_VERSIONS
+    ):
+        create_env(
+            name=env,
+            extras=extras.get(env, env),
+            base=True,
+            python_version=python_version,
+        )
+
+    for env, python_version in product(["docs", "dev"], [PYTHON_DEFAULT_VERSION]):
+        create_env(
+            name=env,
+            extras=extras.get(env, env),
+            base=True,
+            python_version=python_version,
+        )
 
     # need an isolated set of test requirements
-    create_env("environment/test-extras.yaml", extras="test", base=False)
-    create_env(
-        "environment/test-extras.txt", extras="test", base=False, cmd="requirements"
-    )
+    for python_version in PYTHON_ALL_VERSIONS:
+        create_env(
+            name="test-extras",
+            extras="test",
+            base=False,
+            python_version=python_version,
+        )
+
+    # isolated
+    for env in ["dist-pypi", "dist-conda"]:
+        create_env(
+            name=f"{env}",
+            extras=env,
+            base=False,
+            python_version=PYTHON_DEFAULT_VERSION,
+        )
+
+    # isolated requirement files.
+    # no python versioning for these
+    for env, extras in [("test-extras", "test"), ("dist-pypi", "dist-pypi")]:
+        create_env(name=f"{env}", cmd="requirements", extras=extras, base=False)
 
 
 # ** conda-lock
 @DEFAULT_SESSION_VENV
 def conda_lock(
     session: Session,
     force_reinstall: FORCE_REINSTALL_CLI = False,
@@ -333,15 +428,15 @@
         help="lock files to create",
         choices=["test", "typing", "dev", "dist-pypi", "dist-conda", "all"],
     ) = (),
     conda_lock_run: RUN_CLI = [],  # noqa
     conda_lock_mamba: bool = False,
     conda_lock_force: bool = False,
 ):
-    """Create lock files using conda-lock"""
+    """Create lock files using conda-lock."""
 
     pkg_install_venv(
         session,
         name="conda-lock",
         reqs=["conda-lock>=2.0.0"],
         force_reinstall=force_reinstall,
     )
@@ -363,21 +458,21 @@
         py,
         name,
         env_path=None,
     ):
         py = "py" + py.replace(".", "")
 
         if env_path is None:
-            env_path = f"environment/{name}.yaml"
+            env_path = f"environment/{py}-{name}.yaml"
 
         lockfile = lock_dir / f"{py}-{name}-conda-lock.yml"
 
         deps = [env_path]
         # make sure this is last to make python version last
-        deps.append(lock_dir / f"{py}.yaml")
+        # deps.append(lock_dir / f"{py}.yaml")
 
         if conda_lock_force or update_target(lockfile, *deps):
             session.log(f"creating {lockfile}")
             # insert -f for each arg
             if lockfile.exists():
                 lockfile.unlink()
             session.run(
@@ -436,15 +531,15 @@
     test_opts: TEST_OPTS_CLI = (),  # type: ignore
     test_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
     no_cov: bool = False,
 ):
-    """Test environments with conda installs"""
+    """Test environments with conda installs."""
 
     pkg_install_condaenv(
         session=session,
         name="test",
         lock=lock,
         install_package=True,
         force_reinstall=force_reinstall,
@@ -456,30 +551,61 @@
         run=test_run,
         test_no_pytest=test_no_pytest,
         test_opts=test_opts,
         no_cov=no_cov,
     )
 
 
+@ALL_SESSION
+def test_noopt(
+    session: Session,
+    test_no_pytest: bool = False,
+    test_opts: TEST_OPTS_CLI = (),  # type: ignore
+    test_run: RUN_CLI = [],  # noqa
+    lock: LOCK_CLI = False,
+    force_reinstall: FORCE_REINSTALL_CLI = False,
+    log_session: bool = False,
+    no_cov: bool = False,
+):
+    """Test environments with conda installs."""
+
+    pkg_install_condaenv(
+        session=session,
+        name="test-noopt",
+        lock=lock,
+        install_package=True,
+        force_reinstall=force_reinstall,
+        log_session=log_session,
+    )
+
+    _test(
+        session=session,
+        run=test_run,
+        test_no_pytest=test_no_pytest,
+        test_opts=test_opts,
+        no_cov=no_cov,
+    )
+
+
 @ALL_SESSION_VENV
 def test_venv(
     session: Session,
     test_no_pytest: bool = False,
     test_opts: TEST_OPTS_CLI = (),  # type: ignore
     test_run: RUN_CLI = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
     no_cov: bool = False,
 ):
-    """Test environments virtualenv and pip installs"""
+    """Test environments virtualenv and pip installs."""
 
     pkg_install_venv(
         session=session,
-        name="test-pip",
+        name="test-venv",
         extras="test",
         install_package=True,
         force_reinstall=force_reinstall,
         log_session=log_session,
     )
 
     _test(
@@ -498,15 +624,15 @@
     if not cmd and not run and not run_internal:
         cmd = ["combine", "report"]
 
     session.log(f"{cmd}")
 
     for c in cmd:
         if c == "combine":
-            paths = list(Path(".nox").glob("test*/tmp/.coverage"))
+            paths = list(Path(".nox").glob("test-3*/tmp/.coverage"))
             if update_target(".coverage", *paths):
                 session.run("coverage", "combine", "--keep", "-a", *map(str, paths))
         elif c == "open":
             open_webpage(path="htmlcov/index.html")
         else:
             session.run("coverage", c)
 
@@ -678,20 +804,20 @@
         flags=("--dist-pypi-cmd", "-p"),
     ) = (),
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     version: VERSION_CLI = "",
     log_session: bool = False,
 ):
-    """Run 'nox -s dist-pypi -- {clean, build, testrelease, release}'"""
+    """Run 'nox -s dist-pypi -- {clean, build, testrelease, release}'."""
 
     pkg_install_venv(
         session=session,
         name="dist-pypi",
-        requirement_paths=["environment/dist-pypi.txt"],
+        requirement_paths=[session_environment_filename(name="dist-pypi.txt")],
         force_reinstall=force_reinstall,
         install_package=False,
     )
 
     _dist_pypi(
         session=session,
         run=dist_pypi_run,
@@ -709,15 +835,15 @@
         flags=("--dist-pypi-cmd", "-p"),
     ) = (),
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     version: VERSION_CLI = "",
     log_session: bool = False,
 ):
-    """Run 'nox -s dist_pypi -- {clean, build, testrelease, release}'"""
+    """Run 'nox -s dist_pypi -- {clean, build, testrelease, release}'."""
     # conda
 
     pkg_install_condaenv(
         session=session,
         name="dist-pypi",
         install_package=False,
         force_reinstall=force_reinstall,
@@ -750,15 +876,15 @@
     ) = (),
     # lock: LOCK_CLI = False,
     sdist_path: str = "",
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
     version: VERSION_CLI = "",
 ):
-    """Runs make -C dist-conda posargs"""
+    """Runs make -C dist-conda posargs."""
     pkg_install_condaenv(
         session=session,
         name="dist-conda",
         install_package=False,
         force_reinstall=force_reinstall,
         log_session=log_session,
     )
@@ -847,40 +973,47 @@
 
 
 # type checking
 def _typing(session, run, cmd, run_internal):
     session_run_commands(session, run)
     if not run and not run_internal and not cmd:
         cmd = ["mypy"]
+
+    if "all" in cmd:
+        cmd = ["mypy", "pyright", "pytype"]
+
+    # set the cache directory for mypy
+    session.env["MYPY_CACHE_DIR"] = str(Path(session.create_tmp()) / ".mypy_cache")
+
     for c in cmd:
         if c == "mypy":
             session.run("mypy", "--color-output")
         elif c == "pyright":
             session.run("pyright", external=True)
         elif c == "pytype":
-            session.run("pytype")
+            session.run("pytype", "-o", str(Path(session.create_tmp()) / ".pytype"))
     session_run_commands(session, run_internal, external=False)
 
 
 @ALL_SESSION
 def typing(
     session: nox.Session,
     typing_cmd: cmd_annotated(  # type: ignore
-        choices=["mypy", "pyright", "pytype"],
+        choices=["mypy", "pyright", "pytype", "all"],
         flags=("--typing-cmd", "-m"),
     ) = (),
     typing_run: RUN_CLI = [],  # noqa
     typing_run_internal: run_annotated(  # type: ignore
         help="run arbitrary (internal) commands.  For example, --typing-run-internal 'mypy --some-option'",
     ) = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
 ):
-    """Run type checkers (mypy, pyright, pytype)"""
+    """Run type checkers (mypy, pyright, pytype)."""
 
     pkg_install_condaenv(
         session=session,
         name="typing",
         lock=lock,
         install_package=True,
         force_reinstall=force_reinstall,
@@ -895,26 +1028,26 @@
     )
 
 
 @ALL_SESSION_VENV
 def typing_venv(
     session: nox.Session,
     typing_cmd: cmd_annotated(  # type: ignore
-        choices=["mypy", "pyright", "pytype"],
+        choices=["mypy", "pyright", "pytype", "all"],
         flags=("--typing-cmd", "-m"),
     ) = (),
     typing_run: RUN_CLI = [],  # noqa
     typing_run_internal: run_annotated(  # type: ignore
         help="run arbitrary (internal) commands.  For example, --typing-run-internal 'mypy --some-option'",
     ) = [],  # noqa
     lock: LOCK_CLI = False,
     force_reinstall: FORCE_REINSTALL_CLI = False,
     log_session: bool = False,
 ):
-    """Run type checkers (mypy, pyright, pytype)"""
+    """Run type checkers (mypy, pyright, pytype)."""
 
     pkg_install_venv(
         session=session,
         name="typing",
         lock=lock,
         install_package=True,
         force_reinstall=force_reinstall,
@@ -937,23 +1070,25 @@
     test_no_pytest: bool = False,
     test_opts: TEST_OPTS_CLI = (),  # type: ignore
     testdist_conda_run: RUN_CLI = [],  # noqa
     force_reinstall: FORCE_REINSTALL_CLI = False,
     version: VERSION_CLI = "",
     log_session: bool = False,
 ):
-    """Test conda distribution"""
+    """Test conda distribution."""
 
     install_str = PACKAGE_NAME
     if version:
         install_str = f"{install_str}=={version}"
 
     session_install_envs(
         session,
-        "environment/test-extras.yaml",
+        session_environment_filename(
+            python_version=session.python, name="test-extras.yaml"
+        ),
         deps=[install_str],
         channels=["conda-forge"],
         force_reinstall=force_reinstall,
         install_package=False,
     )
 
     if log_session:
@@ -974,28 +1109,28 @@
     test_opts: TEST_OPTS_CLI = (),  # type: ignore
     testdist_pypi_run: RUN_CLI = [],  # noqa
     testdist_pypi_extras: cmd_annotated(help="extras to install") = (),  # type: ignore
     force_reinstall: FORCE_REINSTALL_CLI = False,
     version: VERSION_CLI = "",
     log_session: bool = False,
 ):
-    """Test pypi distribution"""
+    """Test pypi distribution."""
     extras = testdist_pypi_extras
     install_str = PACKAGE_NAME
 
     if extras:
         install_str = "{}[{}]".format(install_str, ",".join(extras))
 
     if version:
         install_str = f"{install_str}=={version}"
 
     pkg_install_venv(
         session=session,
         name="testdist-pypi",
-        requirement_paths=["environment/test-extras.txt"],
+        requirement_paths=[session_environment_filename(name="test-extras.txt")],
         reqs=[install_str],
         force_reinstall=force_reinstall,
         install_package=False,
     )
 
     if log_session:
         session_log_session(session, False)
@@ -1016,27 +1151,29 @@
     test_opts: TEST_OPTS_CLI = (),  # type: ignore
     testdist_pypi_run: RUN_CLI = [],  # noqa
     testdist_pypi_extras: cmd_annotated(help="extras to install") = (),  # type: ignore
     force_reinstall: FORCE_REINSTALL_CLI = False,
     version: VERSION_CLI = "",
     log_session: bool = False,
 ):
-    """Test pypi distribution"""
+    """Test pypi distribution."""
     extras = testdist_pypi_extras
     install_str = PACKAGE_NAME
 
     if extras:
         install_str = "{}[{}]".format(install_str, ",".join(extras))
 
     if version:
         install_str = f"{install_str}=={version}"
 
     session_install_envs(
         session,
-        "environment/test-extras.yaml",
+        session_environment_filename(
+            python_version=session.python, name="test-extras.yaml"
+        ),
         reqs=[install_str],
         channels=["conda-forge"],
         force_reinstall=force_reinstall,
         install_package=False,
     )
     if log_session:
         session_log_session(session, False)
```

### Comparing `module-utilities-0.5.0/pyproject.toml` & `module-utilities-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -28,28 +28,34 @@
 dependencies = ["typing-extensions"]
 
 [project.urls]
 homepage = "https://github.com/usnistgov/module-utilities"
 documentation = "https://pages.nist.gov/module-utilities/"
 
 [project.optional-dependencies]
-test = [
+inherit = ["docstring-inheritance"]
+opt-all = [
+    "module-utilities[inherit]", #
+
+]
+test-extras = [
     "pytest", #
     "pytest-xdist",
     "pytest-cov",
     "pytest-sugar",
 ]
+test = ["module-utilities[test-extras]", "module-utilities[opt-all]"]
 dev-extras = [
     "setuptools-scm", #
     "pytest-accept", # p2c: -p
     "ipython",
     "ipykernel",
 ]
 typing-extras = [
-    # "pytype; python_version < '3.11'",
+    "pytype; python_version < '3.11'", #
     "mypy",
 ]
 typing = [
     "module-utilities[typing-extras]", #
     "module-utilities[test]",
 ]
 nox = [
@@ -79,25 +85,33 @@
     "sphinx>=5.3.0",
     "sphinx-copybutton",
     "sphinxcontrib-spelling",
     "sphinx-autobuild",
     "myst-nb",
     "sphinx-book-theme",
     "autodocsumm",
+    # "sphinx-autodoc-typehints",
+    "module-utilities[opt-all]",
 ]
 # to be parsed with pyproject2conda with --no-base option
 dist-pypi = ["twine", "build"]
 dist-conda = [
     "anaconda-client", #
     "grayskull",
     "conda-build",
     "conda-verify",
     "boa",
 ]
+# testing with out optional deps
+test-noopt = ["module-utilities[test-extras]"]
 
+# typing-noopt = [
+#     "module-utilities[typing-extras]",
+#     "module-utilities[test-extras]",
+# ]
 [tool.pyproject2conda]
 channels = ["conda-forge"]
 
 ## grayskull still messes some things up, but use scripts/recipe-append.sh for this
 [tool.setuptools]
 zip-safe = true # if using mypy, must be False
 include-package-data = true
@@ -123,14 +137,20 @@
 [tool.aliases]
 test = "pytest"
 
 [tool.pytest.ini_options]
 addopts = "-n 4 --doctest-modules --doctest-glob='*.md'"
 # testpaths = ["src/module_utilities", "tests", "./README.md"]
 testpaths = ["src", "tests", "README.md"]
+markers = ["inherit: docstring_inheritance dependent code"]
+
+[tool.coverage.report]
+exclude_also = ["if TYPE_CHECKING:", "@overload"]
+omit = ["*/vendored/*"]
+include = ["src/*"]
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
 known_first_party = ["module_utilities"]
 
 [tool.ruff]
@@ -289,18 +309,19 @@
 # files = ["src", "tests"]
 show_error_codes = true
 warn_unused_ignores = true
 warn_return_any = true
 warn_unused_configs = true
 exclude = [".eggs", ".tox", "doc", "docs", ".nox"]
 check_untyped_defs = true
+strict = true
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
-module = []
+module = ["custom_inherit.*"]
 
 [[tool.mypy.overrides]]
 ignore_errors = true
 module = ["module_utilities.vendored.docscrape"]
 
 [tool.pyright]
 include = ["src", "tests"]
@@ -308,25 +329,28 @@
     "**/__pycache__",
     ".tox/**",
     ".nox/**",
     "**/.mypy_cache",
     "src/module_utilities/vendored"
 ]
 pythonVersion = "3.10"
+strict = ["src"]
+# Would like to use strict throughtout, but need to update tests first.
+# typeCheckingMode = "strict"
 typeCheckingMode = "basic"
-# enable subset of "strict"
+## enable subset of "strict"
 reportDuplicateImport = true
 reportInvalidStubStatement = true
 reportOverlappingOverload = true
 reportPropertyTypeMismatch = true
 reportUntypedClassDecorator = true
 reportUntypedFunctionDecorator = true
 reportUntypedNamedTuple = true
 reportUnusedImport = true
-# disable subset of "basic"
+## disable subset of "basic"
 reportGeneralTypeIssues = false
 reportMissingModuleSource = false
 reportOptionalCall = false
 reportOptionalIterable = false
 reportOptionalMemberAccess = false
 reportOptionalOperand = false
 reportOptionalSubscript = false
```

### Comparing `module-utilities-0.5.0/src/module_utilities/_doc.py` & `module-utilities-0.6.0/src/module_utilities/_doc.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 would just use the pandas version, but since it's a private
 module, feel it's better to have static version here.
 """
 
 from __future__ import annotations
 
 from textwrap import dedent
-from typing import TYPE_CHECKING, Callable
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
+    from typing import Any, Callable
+
     from ._typing import F
 
 
 def doc(
-    *docstrings: None | str | Callable, _prepend: bool = False, **params
-) -> Callable[[F], F]:
+    *docstrings: None | str | Callable[..., Any], _prepend: bool = False, **params: str
+) -> Callable[[F], F]:  # pyre-ignore
     """
     A decorator to take docstring templates, concatenate them and perform string
     substitution on them.
     This decorator will add a variable "_docstring_components" to the wrapped
     callable to keep track the original docstring template for potential usage.
     If it should be consider as a template, it will be saved as a string.
     Otherwise, it will be saved as callable, and later user __doc__ and dedent
@@ -36,37 +38,37 @@
     **params
         The string which would be used to format docstring template.
 
     """
 
     def decorator(decorated: F) -> F:
         # collecting docstring and docstring templates
-        docstring_components: list[str | Callable] = []
+        docstring_components: list[str | Callable[..., Any]] = []
         # if decorated.__doc__:
         #     docstring_components.append(dedent(decorated.__doc__))
 
         for docstring in docstrings:
             if docstring is None:
                 continue
             if hasattr(docstring, "_docstring_components"):
                 docstring_components.extend(
-                    docstring._docstring_components  # pyright: ignore[reportGeneralTypeIssues] # noqa: E501
+                    docstring._docstring_components  # pyright: ignore # noqa: E501 # pyre-ignore
                 )
             elif isinstance(docstring, str):
                 docstring_components.append(docstring)
             elif docstring.__doc__:
                 # docstring_components.append(docstring)
                 docstring_components.append(dedent(docstring.__doc__ or ""))
 
         # make default to append
         if decorated.__doc__:
             if _prepend:
-                docstring_components.insert(0, dedent(decorated.__doc__))
+                docstring_components.insert(0, dedent(decorated.__doc__ or ""))
             else:
-                docstring_components.append(dedent(decorated.__doc__))
+                docstring_components.append(dedent(decorated.__doc__ or ""))
 
         params_applied = [
             # component.format(**params)
             component.format_map(params)
             if isinstance(component, str) and len(params) > 0
             else component
             for component in docstring_components
```

### Comparing `module-utilities-0.5.0/src/module_utilities/attributedict.py` & `module-utilities-0.6.0/src/module_utilities/attributedict.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,46 @@
 """
 Attribute dictionary (:mod:`~module_utilities.attributedict`)
 =============================================================
 """
 from __future__ import annotations
 
-from collections.abc import Mapping, MutableMapping
-from typing import Any
+from typing import Any, Iterator, Mapping, MutableMapping, overload
 
-# from typing import TypeVar, Type
+from ._typing import NestedMap, NestedMapVal
 
-# AttibuteDictT = TypeVar('AttributeDictT', bound="AttributeDict")
 
+@overload
+def _get_nested_values(d: NestedMap, join_string: None) -> list[str]:
+    ...
 
-def _get_nested_values(d, join_string="\n"):
-    out = []
+
+@overload
+def _get_nested_values(d: NestedMap, join_string: str = ...) -> str:
+    ...
+
+
+def _get_nested_values(d: NestedMap, join_string: str | None = "\n") -> str | list[str]:
+    out: list[str] = []
     for k in d:
         v = d[k]
         if isinstance(v, str):
             out.append(v)
         else:
-            out.extend(_get_nested_values(v, join_string=None))
+            # fmt: off
+            out.extend(_get_nested_values(v, join_string=None))  # pytype: disable=wrong-arg-types
+            # fmt: on
 
     if join_string is not None:
-        out = join_string.join(out)
-
-    return out
+        return join_string.join(out)
+    else:
+        return out
 
 
-class AttributeDict(MutableMapping):
+class AttributeDict(MutableMapping[str, NestedMapVal]):
     """
     Dictionary with recursive attribute like access.
 
     To be used in str.format calls, so can expand on fields like
     `{name.property}` in a nested manner.
 
     Parameters
@@ -53,20 +62,22 @@
     2
     """
 
     __slots__ = ("_entries", "_recursive", "_allow_missing")
 
     def __init__(
         self,
-        entries: dict[str, Any] | None = None,
+        entries: Mapping[str, NestedMapVal] | None = None,
         recursive: bool = True,
         allow_missing: bool = True,
     ):
         if entries is None:
             entries = {}
+        if not isinstance(entries, dict):
+            entries = dict(entries)
         self._entries = entries
         self._recursive = recursive
         self._allow_missing = allow_missing
 
     def __getitem__(self, key: str | slice) -> Any:
         if isinstance(key, slice):
             return _get_nested_values(self._getslice(key), join_string="\n")
@@ -78,15 +89,15 @@
             return "\n".join(self[x] for x in (x.strip() for x in key.split(",")))
 
         if self._allow_missing and key not in self._entries:
             return f"{{{key}}}"
         else:
             return self._entries[key]
 
-    def _getslice(self, s) -> AttributeDict:
+    def _getslice(self, s: slice) -> AttributeDict:
         start = s.start
         stop = s.stop
 
         keys = list(self._entries.keys())
 
         if isinstance(s.start, int) or s.start is None and isinstance(s.stop, int):
             slc = s
@@ -103,36 +114,36 @@
                 stop = keys.index(s.stop) + 1
 
             slc = slice(start, stop, s.step)
 
         subset = {k: self._entries[k] for k in keys[slc]}
         return type(self)(subset)
 
-    def __setitem__(self, key: str, value) -> None:
+    def __setitem__(self, key: str, value: NestedMapVal) -> None:
         self._entries[key] = value
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[str]:
         return iter(self._entries)
 
     def __len__(self) -> int:
         return len(self._entries)
 
-    def __delitem__(self, key):
+    def __delitem__(self, key: str) -> None:
         del self._entries[key]
 
-    def _items(self):
+    def _items(self) -> Iterator[tuple[str, NestedMapVal]]:
         yield from self._entries.items()
 
-    def __dir__(self):
+    def __dir__(self) -> list[str]:  # pragma: no cover
         return list(self.keys()) + list(super().__dir__())
 
-    def _update(self, *args, **kwargs):
+    def _update(self, *args: Any, **kwargs: Any) -> None:
         self._entries.update(*args, **kwargs)
 
-    def __getattr__(self, attr):
+    def __getattr__(self, attr: str) -> Any:
         if attr in self._entries:
             out = self._entries[attr]
             if self._recursive and isinstance(out, dict):
                 out = type(self)(out)
             return out
         else:
             try:
@@ -144,35 +155,42 @@
                 # But we only want to see an error when building the docs;
                 # not something users should see, so this slight inconsistency is fine.
                 if __debug__:
                     raise err
                 else:
                     pass
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__}({repr(self._entries)})"
 
     @classmethod
     def _from_dict(
-        cls, params: Mapping, max_level: int = 1, level: int = 0, recursive: bool = True
+        cls,
+        params: Mapping[str, NestedMapVal],
+        max_level: int = 1,
+        level: int = 0,
+        recursive: bool = True,
     ) -> AttributeDict:
         # to hide level parameter
         out = cls(recursive=recursive)
         for k in params:
             v = params[k]
             if isinstance(v, dict) and level < max_level:
                 v = cls._from_dict(
                     v, max_level=max_level, level=level + 1, recursive=recursive
                 )
             out[k] = v
         return out
 
     @classmethod
     def from_dict(
-        cls, params: Mapping, max_level: int = 1, recursive: bool = True
+        cls,
+        params: Mapping[str, NestedMapVal],
+        max_level: int = 1,
+        recursive: bool = True,
     ) -> AttributeDict:
         """
         Create AttributeDict recursively for nested dictionaries.
 
         To be used in cases where need to apply AttributeDict to parameters
         passed with ``func(**params)``.
```

### Comparing `module-utilities-0.5.0/src/module_utilities/docfiller.py` & `module-utilities-0.6.0/src/module_utilities/docfiller.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,58 @@
 """
-Fill and share documentation (:mod:`module_utilities.docfiller`)
-================================================================
+Fill and share documentation (:mod:`~module_utilities.docfiller`)
+=================================================================
 """
 from __future__ import annotations
 
 import inspect
-import os
-from textwrap import dedent
-from typing import TYPE_CHECKING, Any, Callable
+from collections.abc import Mapping
+from textwrap import dedent, indent
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    List,
+    NamedTuple,
+    Union,
+    cast,
+)
 
 from . import cached
 from ._doc import doc as _pd_doc
 from .attributedict import AttributeDict
-
-# from ._docscrape import NumpyDocString, Parameter  # type: ignore
+from .options import DOC_SUB
 from .vendored.docscrape import NumpyDocString, Parameter
 
 if TYPE_CHECKING:
-    from collections.abc import Mapping, Sequence
+    from collections.abc import Sequence
+
+    from ._typing import F, NestedMap, NestedMapVal
 
-    from ._typing import F
 
-try:
-    # Default is DOC_SUB is True
-    DOC_SUB = os.getenv("DOCFILLER_SUB", "True").lower() not in (
-        "0",
-        "f",
-        "false",
-    )
-except KeyError:
-    DOC_SUB = True
+def indent_docstring(
+    docstring: str | Callable[..., Any], prefix: str | None = "+  "
+) -> str:
+    """Create indented docstring"""
+    if callable(docstring):
+        docstring = (docstring.__doc__ or "").strip()
+
+    if prefix is not None:
+        return indent(docstring, prefix)
+    else:
+        return docstring
 
 
 # Factory method to create doc_decorate
 def doc_decorate(
-    *docstrings: str | Callable, _prepend: bool = False, **params
+    *docstrings: str | Callable[..., Any] | None,
+    _prepend: bool = False,
+    **params: str,
 ) -> Callable[[F], F]:
     """
     A decorator take docstring templates, concatenate them and perform string
     substitution on it.
 
     This decorator will add a variable "_docstring_components" to the wrapped
     callable to keep track the original docstring template for potential usage.
@@ -56,33 +70,80 @@
     **params
         The string which would be used to format docstring template.
 
     Notes
     -----
     Doc filling can be turned off by setting the environment variable
     ``DOCFILLER_SUB`` to one of ``0, f, false``.
+
+
+    Examples
+    --------
+    >>> @doc_decorate(type_='int')
+    ... def func0(x, y):
+    ...     '''
+    ...     Parameters
+    ...     ----------
+    ...     x : {type_}
+    ...         x parameter.
+    ...     y : {type_}
+    ...         y parameter.
+    ...     Returns
+    ...     -------
+    ...     output : {type_}
+    ...     '''
+    ...     pass
+    >>> print(indent_docstring(func0))
+    +  Parameters
+    +  ----------
+    +  x : int
+    +      x parameter.
+    +  y : int
+    +      y parameter.
+    +  Returns
+    +  -------
+    +  output : int
+
+
+    To inherit from a function/docstring, pass it:
+
+
+    >>> @doc_decorate(func0, type_='float')
+    ... def func1(x, y):
+    ...     pass
+    >>> print(indent_docstring(func1))
+    +  Parameters
+    +  ----------
+    +  x : float
+    +      x parameter.
+    +  y : float
+    +      y parameter.
+    +  Returns
+    +  -------
+    +  output : float
     """
 
     if DOC_SUB:
         return _pd_doc(*docstrings, _prepend=_prepend, **params)
     else:
 
-        def decorated(func):
+        def decorated(func: F) -> F:
             return func
 
         return decorated
 
 
-def _build_param_docstring(name: str, ptype: str, desc: str | Sequence[str]) -> str:
+def _build_param_docstring(
+    name: str | None, ptype: str | None, desc: str | Sequence[str]
+) -> str:
     """
     Create multiline documentation of single name, type, desc.
 
     Parameters
     ----------
-    ==========
     name : str
         Parameter Name
     ptype : str
         Parameter type
     desc : list of str
         Parameter description
 
@@ -116,15 +177,26 @@
 
     if len(desc) > 0:
         desc = "\n    ".join(desc)
         s += f"\n    {desc}"
     return s
 
 
-def _params_to_string(params, key_char: str = "|") -> str | dict[str, Any]:
+class TParameter(NamedTuple):
+    """Interface to Parameters namedtuple in docscrape"""
+
+    name: str
+    type: str
+    desc: str
+
+
+def _params_to_string(
+    params: str | list[str] | Parameter | list[Parameter] | tuple[Parameter, ...],
+    key_char: str = "|",
+) -> str | dict[str, str]:
     """
     Parse list of Parameters objects to string
 
     Examples
     --------
     >>> from module_utilities.docfiller import Parameter
     >>> p = Parameter(name="a", type="int", desc=["A parameter"])
@@ -140,32 +212,32 @@
     if isinstance(params, Parameter):
         params = [params]
 
     if not isinstance(params, (list, tuple)):
         params = [params]
 
     if isinstance(params[0], str):
-        return "\n".join(params)
+        return "\n".join(cast(List[str], params))
 
-    out = {}
-    for p in params:
+    out: dict[str, str] = {}
+    for p in cast(List[TParameter], params):
         name = p.name
         if key_char in name:
             key, name = (x.strip() for x in name.split(key_char))
         else:
             key = name
 
         out[key] = _build_param_docstring(name=name, ptype=p.type, desc=p.desc)
 
     return out
 
 
 def _parse_docstring(
-    func_or_doc: Callable | str, key_char: str = "|", expand: bool = True
-):
+    func_or_doc: Callable[..., Any] | str, key_char: str = "|", expand: bool = True
+) -> dict[str, str | dict[str, str]]:
     """
     Parse numpy style docstring from function or string to dictionary.
 
     Parameters
     ----------
     func_or_doc : callable or str
         If function, extract docstring from function.
@@ -208,26 +280,30 @@
     >>> print(p["parameters"]["y_alt"])
     y : float
         y parameter
     >>> print(p["returns"]["output"])
     output : float
         an output
 
+    >>> p2 = _parse_docstring(doc_string, expand=False)
+    >>> print(p2["Parameters"])
+    [Parameter(name='x', type='int', desc=['x parameter']), Parameter(name='y_alt | y', type='float', desc=['y parameter'])]
+
 
     """
 
     if callable(func_or_doc):
         doc = inspect.getdoc(func_or_doc)
     else:
         doc = func_or_doc
 
-    parsed = NumpyDocString(doc)._parsed_data
+    parsed = cast(Dict[str, Union[str, List[str], List[Parameter]]], NumpyDocString(doc)._parsed_data)  # type: ignore[no-untyped-call]
 
     if expand:
-        parsed = {
+        parsed_out = {
             k.replace(" ", "_").lower(): _params_to_string(parsed[k], key_char=key_char)
             for k in [
                 "Summary",
                 "Extended Summary",
                 "Parameters",
                 "Returns",
                 "Yields",
@@ -236,18 +312,20 @@
                 "Other Parameters",
                 "Attributes",
                 "Methods",
                 "References",
                 "Examples",
             ]
         }
-    return parsed
+    else:
+        parsed_out = cast(Dict[str, Union[str, Dict[str, str]]], parsed)
+    return parsed_out
 
 
-def dedent_recursive(data: Mapping[str, Any]) -> dict[str, Any]:
+def dedent_recursive(data: NestedMap) -> NestedMap:
     """
     Dedent nested mapping of strings.
 
     Parameters
     ----------
     data : dict
 
@@ -269,27 +347,42 @@
              A thing
     <BLANKLINE>
     >>> data = dedent_recursive(data)
     >>> print(data['a']['value'])
     a : int
         A thing
     """
-    out = {}
+    out: dict[str, NestedMapVal] = {}
     for k in data:
         v = data[k]
         if isinstance(v, str):
             v = dedent(v).strip()
         else:
             v = dedent_recursive(v)
         out[k] = v
     return out
 
 
-def _recursive_keys(data) -> list[str]:
-    keys = []
+def _recursive_keys(data: NestedMap) -> list[str]:
+    """
+    Examples
+    --------
+    >>> d = {'a': 'a', 'b': {'c': "hello"}}
+    >>> _recursive_keys(d)
+    ['a', 'b.c']
+
+    >>> d = {'a': 1}
+    >>> _recursive_keys(d)
+    Traceback (most recent call last):
+    ...
+    ValueError: unknown type <class 'int'>
+
+
+    """
+    keys: list[str] = []
     for k, v in data.items():
         if isinstance(v, dict):
             key_list = [f"{k}.{x}" for x in _recursive_keys(v)]
         elif isinstance(v, str):
             key_list = [k]
         else:
             raise ValueError(f"unknown type {type(v)}")
@@ -305,36 +398,95 @@
 
     Parameters
     ----------
     func_or_doc : callable or str
         Docstring to parse.  If callable, extract from function signature.
     key_char : str, default='|'
         Optional string to split name into key/name pair.
+
+
+    Examples
+    --------
+    >>> d = DocFiller.from_docstring(
+    ...     '''
+    ...     Parameters
+    ...     ----------
+    ...     x : int
+    ...         x param
+    ...     y : int
+    ...         y param
+    ...     z0 | z : int
+    ...         z int param
+    ...     z1 | z : float
+    ...         z float param
+    ...
+    ...     Returns
+    ...     -------
+    ...     output0 | output : int
+    ...         Integer output.
+    ...     output1 | output : float
+    ...         Float output
+    ...     ''',
+    ...     combine_keys='parameters'
+    ... )
+    ...
+    >>> print(d.keys()[-4:])
+    ['x', 'y', 'z0', 'z1']
+    >>> @d.decorate
+    ... def func(x, y, z):
+    ...     '''
+    ...     Parameters
+    ...     ----------
+    ...     {x}
+    ...     {y}
+    ...     {z0}
+    ...     Returns
+    ...     --------
+    ...     {returns.output0}
+    ...     '''
+    ...     return x + y + z
+    ...
+    >>> print(indent_docstring(func))
+    +  Parameters
+    +  ----------
+    +  x : int
+    +      x param
+    +  y : int
+    +      y param
+    +  z : int
+    +      z int param
+    +  Returns
+    +  --------
+    +  output : int
+    +      Integer output.
     """
 
-    def __init__(self, params: Mapping[str, Any] | None = None) -> None:
+    def __init__(self, params: NestedMap | None = None) -> None:
+        self.data: dict[str, NestedMapVal]
+
         if params is None:
             self.data = {}
         elif isinstance(params, dict):
             self.data = params
         else:
             self.data = dict(params)
+        self._cache: dict[str, Any] = {}
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({repr(self.data)})"
 
-    def new_like(self, data: dict | None = None) -> DocFiller:
+    def new_like(self, data: NestedMap | None = None) -> DocFiller:
         """Create new object with optional data."""
         if data is None:
             data = self.data.copy()
         return type(self)(data)
 
-    def __getitem__(self, key: str):
+    def __getitem__(self, key: str) -> DocFiller | str:
         val = self.data[key]
-        if isinstance(val, dict):
+        if isinstance(val, Mapping):
             return self.new_like(val)
         else:
             return val
 
     def dedent(self) -> DocFiller:
         """Recursively dedent params"""
         return self.new_like(dedent_recursive(self.data))
@@ -343,18 +495,27 @@
     def keys(self) -> list[str]:
         """List of keys"""
         return _recursive_keys(self.data)
 
     def assign_combined_key(self, new_key: str, keys: Sequence[str]) -> DocFiller:
         """Combine multiple keys into single key"""
         new = self.new_like()
-        new.data[new_key] = "\n".join([self.data[k] for k in keys])
+
+        new_data: list[str] = []
+        for k in keys:
+            d = self.data[k]
+            if isinstance(d, str):
+                new_data.append(d)
+            else:
+                raise ValueError(f"trying to combine key {k} with non-string value {d}")
+
+        new.data[new_key] = "\n".join(new_data)
         return new
 
-    def _gen_get_val(self, key):
+    def _gen_get_val(self, key: str) -> Any:
         from operator import attrgetter
 
         f = attrgetter(key)
         return f(self.params)
 
     def assign_keys(self, **kwargs: str | Sequence[str]) -> DocFiller:
         """
@@ -393,15 +554,15 @@
 
     def assign_param(
         self,
         name: str,
         ptype: str = "",
         desc: str | list[str] | None = None,
         key: str | None = None,
-    ):
+    ) -> DocFiller:
         """
         Add in a new parameter
 
         Parameters
         ----------
         name : str
             Parameters name
@@ -447,16 +608,16 @@
         new.data[key] = _build_param_docstring(name=name, ptype=ptype, desc=desc)
 
         return new
 
     @classmethod
     def concat(
         cls,
-        *args: Mapping[str, Any] | DocFiller,
-        **kwargs: Mapping[str, Any] | DocFiller,
+        *args: NestedMap | DocFiller,
+        **kwargs: NestedMap | DocFiller,
     ) -> DocFiller:
         """
         Create new object from multiple DocFiller or dict objects.
 
         Parameters
         ----------
         *args
@@ -474,30 +635,33 @@
         -----
         Use unnamed `args` to pass in underlying data.
         Use names ``kwargs`` to add namespace.
         """
 
         # create
 
-        data: dict[str, Any] = {}
+        data: dict[str, NestedMapVal] = {}
 
-        def _update_data(x):
+        def _update_data(x: DocFiller | NestedMap | dict[str, NestedMap]) -> None:
             if isinstance(x, DocFiller):
                 # x = x.params
                 x = x.data
             data.update(**x)
 
         for a in args:
             _update_data(a)
 
+        kws: dict[str, NestedMap] = {}
         for k, v in kwargs.items():
-            if isinstance(v, cls):
-                kwargs[k] = v.data
+            if isinstance(v, DocFiller):
+                kws[k] = v.data
+            else:
+                kws[k] = v
 
-        _update_data(kwargs)
+        _update_data(kws)
         return cls(data)
 
     def append(
         self,
         *args: Mapping[str, Any] | DocFiller,
         **kwargs: Mapping[str, Any] | DocFiller,
     ) -> DocFiller:
@@ -513,156 +677,224 @@
 
         new = self.new_like()
         for name in names:
             d = self.data[name]
             if isinstance(d, str):
                 raise ValueError(f"level {name} is not a dict")
             else:
-                for k, v in self.data[name].items():
+                for k, v in d.items():
                     new.data[k] = v
         return new
 
     def rename_levels(self, **kws: str) -> DocFiller:
         """Rename a keys at top level."""
         params = {}
         for k, v in self.data.items():
             key = kws.get(k, k)
             params[key] = v
         return self.new_like(params)
 
-    # def rename(self, mapping: Mapping[Any, Hashable] | None = None, **kwargs) -> DocFiller:
-    #     """
-    #     New DocFiller with new names at top level.
-    #     """
-
-    #     if mapping is not None:
-    #         m = dict(mapping)
-    #     else:
-    #         m = {}
-
-    #     m = dict(m, **kwargs)
-
-    #     data = self.data.copy()
-    #     for old_name, v in m.items():
-    #         data[]
-
     @cached.prop
     def params(self) -> AttributeDict:
         """An AttributeDict view of parameters."""
         return AttributeDict.from_dict(self.data, max_level=1)
 
     @cached.prop
     def _default_decorator(self) -> Callable[[F], F]:
         return doc_decorate(**self.params)
 
-    def update(self, *args, **kwargs) -> DocFiller:
+    def update(self, *args: Any, **kwargs: Any) -> DocFiller:
         """Update parameters"""
         new = self.new_like()
         new.data.update(*args, **kwargs)
         return new
 
-    def assign(self, **kwargs) -> DocFiller:
+    def assign(self, **kwargs: Any) -> DocFiller:
         """Assign new key/value pairs"""
         return self.update(**kwargs)
 
     def decorate(self, func: F) -> F:
         """
         Default decorator.
 
-        This uses `self.params` and the decorated funciton docstring as a template.
+        This uses `self.params` and the decorated function docstring as a template.
+        If need to pass parameters, use self.__call__
+
+
+        See Also
+        --------
+        __call__
+
+
         """
-        return self._default_decorator(func)  # type: ignore
+        return self._default_decorator(func)
 
     def __call__(
-        self, *templates: Callable | str, _prepend: bool = False, **params
+        self,
+        *templates: Callable[..., Any] | str,
+        _prepend: bool = False,
+        **params: str,
     ) -> Callable[[F], F]:
         """
-        General decorator.
+        Factory function to create docfiller decorator.
 
         This should always be used in a callable manner.
 
         If want to call without any parameter use decorate()
 
         Parameters
         ----------
         *templates : callable
             docstrings to be used as templates.
+        _prepend : bool, default=False
+            If `True`, then prepend `templates` with docstring of decorated function.
+            Otherwise, append to end.
         **params
             Extra parameters to be substituted.
+
+
+        Example
+        -------
+        Using the default decorator
+
+
+        >>> d = DocFiller({"x": "hello", "y": "there"})
+        >>> @d.decorate
+        ... def func():
+        ...     '''
+        ...     A function with  x={x} and y={y}
+        ...     '''
+        ...     pass
+        >>> print(indent_docstring(func))
+        +  A function with  x=hello and y=there
+
+
+        Using call without args
+
+
+        >>> @d()
+        ... def func1():
+        ...     '''
+        ...     A new function with x={x} and y={y}
+        ...     '''
+        ...     pass
+        >>> print(indent_docstring(func1))
+        +  A new function with x=hello and y=there
+
+        Using call with args. This inherits from passed template
+
+
+        >>> @d(func, x="new_x")
+        ... def func2():
+        ...     pass
+        >>> print(indent_docstring(func2))
+        +  A function with  x=new_x and y=there
         """
         ntemplates, nparams = len(templates), len(params)
 
         if ntemplates == nparams == 0 and not _prepend:
             return self.decorate
         elif nparams == 0:
             return doc_decorate(*templates, _prepend=_prepend, **self.params)
         else:
             return self.update(params)(*templates, _prepend=_prepend)
 
-    # NOTE: This is dangerous.
-    # if you pass a function as a template, but forget to explicitly pass it,
-    # you overwrite the docstring for that function.  Just really confusing
-    # def dec(self, *funcs, docstrings=None, **params) -> Callable[[F], F]:
-    #     """
-    #     General decorator.
-
-    #     Parameters
-    #     ----------
-    #     *funcs : callable
-
-    #     This should always be used in a callable manner.
-
-    #     If want to call without any parameter use decorate()
-    #     """
-
-    #     nfuncs = len(funcs)
-
-    #     if nfuncs == 0:
-    #         func = None
-    #     elif nfuncs == 1 and callable(funcs[0]):
-    #         func = funcs[0]
-    #     else:
-    #         func = None    #         raise ValueError("Must call with zero or one functions.  If trying to set docstrings, be explicit")
-
-    #     if docstrings is None:
-    #         docstrings = ()
-    #     elif callable(docstrings) or isinstance(docstrings, str):
-    #         docstrings = (docstrings,)
-
-    #     ndocstrings, nparams = (len(x) for x in (docstrings, params))
-
-    #     if ndocstrings == nparams == 0:
-    #         dec = self.default_decorator
-    #     else:
-    #         if nparams > 0:
-    #             params = AttributeDict.from_dict({**self.data, **params}, max_level=1)
-    #         else:
-    #             params = self.params
-    #         dec = doc_decorate(*docstrings, **params)
-
-    #     if func:
-    #         dec = dec(func)
-    #     return dec
-
-    # def __call__(self, *funcs, docstrings=None, **params) -> Callable[[F], F]:
-    #     """
-    #     Simplified decorator.
-
-    #     Does not handle templates.
-    #     """
-    #     return self.dec(*funcs, docstrings=docstrings, **params)
+    def inherit(
+        self,
+        template: Callable[..., Any],
+        _prepend: bool = False,
+        **params: str,
+    ) -> Callable[[F], F]:
+        """
+        Factor function to create decorator.
+
+        Use combination of docstring_inheritance.inherit_numpy_docstring and
+        DocFiller.
+
+        Parameters
+        ----------
+        template : callable
+            Template method to inherit from.
+        _prepend : bool, default=False
+            Prepend parameter.
+        **params :
+            Extra parameter specificiations.
+
+        Returns
+        -------
+        decorator : callable
+            Decorator
+
+        See Also
+        --------
+        ~module_utilities.docinherit.doc_inherit
+        """
+        from . import docinherit
+
+        docfiller = self.update(params)
+
+        def decorator(func: F) -> F:
+            @docfiller(template)
+            def dummy() -> None:
+                pass
+
+            func = docfiller(_prepend=_prepend)(func)
+
+            return docinherit.doc_inherit(parent=dummy)(func)
+
+        return decorator
+
+    def factory_from_parent(
+        self,
+        cls: type,
+    ) -> Callable[..., Callable[[F], F]]:
+        """
+        Interface to docinherit.factory_docfiller_from_parent.
+
+        Parameters
+        ----------
+        cls : type
+            Class to inherit from.
+
+        See Also
+        --------
+        ~module_utilities.docinherit.factory_docfiller_from_parent
+        """
+        from . import docinherit
+
+        return docinherit.factory_docfiller_from_parent(cls, self)
+
+    def factory_inherit_from_parent(
+        self,
+        cls: type,
+    ) -> Callable[..., Callable[[F], F]]:
+        """
+        Interface to docinherit.factory_docfiller_inherit_from_parent.
+
+        Parameters
+        ----------
+        cls : type
+            Class to inherit from
+
+        See Also
+        --------
+        ~module_utilities.docinherit.factory_docfiller_inherit_from_parent
+        """
+        from . import docinherit
+
+        return docinherit.factory_docfiller_inherit_from_parent(cls, self)
 
     @classmethod
     def from_dict(
         cls,
         params: Mapping[str, Any],
         namespace: str | None = None,
         combine_keys: str | Sequence[str] | None = None,
         keep_keys: bool | str | Sequence[str] = True,
-        key_map: Mapping[str, str] | Callable | None = None,
+        key_map: Mapping[str, str] | Callable[[str], str] | None = None,
     ) -> DocFiller:
         """
         Create a Docfiller instance from a dictionary.
 
         Parameters
         ----------
         params : mapping
@@ -686,14 +918,16 @@
         if not keep_keys:
             keep_keys = []
         elif keep_keys is True:
             keep_keys = [k for k in params]
         elif isinstance(keep_keys, str):
             keep_keys = [keep_keys]
 
+        assert isinstance(keep_keys, Iterable)
+
         if combine_keys:
             if isinstance(combine_keys, str):
                 combine_keys = [combine_keys]
 
             updated_params = {k: params[k] for k in keep_keys}
 
             # if isinstance(combine_keys, (list, tuple)):
@@ -706,36 +940,36 @@
 
             for k in combine_keys:
                 updated_params.update(**params[k])
 
         else:
             updated_params = {k: params[k] for k in keep_keys}
 
-        if key_map is not None:
-            if callable(key_map):
-                mapper = key_map
-            else:
-                mapper = lambda x: key_map[x]  # type: ignore
-
-            updated_params = {mapper(k): updated_params[k] for k in updated_params}
+        if key_map is None:
+            pass
+        elif callable(key_map):
+            updated_params = {key_map(k): v for k, v in updated_params.items()}
+        else:
+            assert isinstance(key_map, Mapping)
+            updated_params = {key_map[k]: v for k, v in updated_params.items()}
 
         if namespace:
             updated_params = {namespace: updated_params}
 
         return cls(params=updated_params)
 
     @classmethod
     def from_docstring(
         cls,
-        func_or_doc: Callable | str,
+        func_or_doc: Callable[..., Any] | str,
         namespace: str | None = None,
         combine_keys: str | Sequence[str] | None = None,
         key_char: str = "|",
-        keep_keys: bool = True,
-        key_map: Mapping | Callable | None = None,
+        keep_keys: bool | str | Sequence[str] = True,
+        key_map: Mapping[str, str] | Callable[[str], str] | None = None,
     ) -> DocFiller:
         """
         Create a Docfiller instance from a function or docstring.
 
         Parameters
         ----------
         func_or_doc : str or callable
```

### Comparing `module-utilities-0.5.0/src/module_utilities/vendored/LICENSE.txt` & `module-utilities-0.6.0/src/module_utilities/vendored/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/src/module_utilities/vendored/docscrape.py` & `module-utilities-0.6.0/src/module_utilities/vendored/docscrape.py`

 * *Files identical despite different names*

### Comparing `module-utilities-0.5.0/src/module_utilities.egg-info/PKG-INFO` & `module-utilities-0.6.0/src/module_utilities.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-utilities
-Version: 0.5.0
+Version: 0.6.0
 Summary: Collection of utilities to aid working with python modules.
 Author-email: "William P. Krekelberg" <wpk@nist.gov>
 License: NIST-PD
 Project-URL: homepage, https://github.com/usnistgov/module-utilities
 Project-URL: documentation, https://pages.nist.gov/module-utilities/
 Keywords: module-utilities
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,25 +16,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: inherit
+Provides-Extra: opt-all
+Provides-Extra: test-extras
 Provides-Extra: test
 Provides-Extra: dev-extras
 Provides-Extra: typing-extras
 Provides-Extra: typing
 Provides-Extra: nox
 Provides-Extra: dev
 Provides-Extra: tools
 Provides-Extra: dev-complete
 Provides-Extra: docs
 Provides-Extra: dist-pypi
 Provides-Extra: dist-conda
+Provides-Extra: test-noopt
 License-File: LICENSE
 
 <!-- markdownlint-disable MD041 -->
 
 [![Repo][repo-badge]][repo-link] [![Docs][docs-badge]][docs-link]
 [![PyPI license][license-badge]][license-link]
 [![PyPI version][pypi-badge]][pypi-link]
@@ -80,14 +84,20 @@
   a standard python dictionary for storage. Future versions will hopefully
   integrate with something like [cachetools].
 
 - `docfiller`: A module to share documentation. This is addapted from the
   [pandas `doc` decorator](https://github.com/pandas-dev/pandas/blob/main/pandas/util/_decorators.py).
   There are some convenience functions and classes for sharing documentation.
 
+- `docinhert`: An interface to [docstring-inheritance] module. This can be
+  combined with `docfiller` to make creating related function/class
+  documentation easy.
+
+[docstring-inheritance]: https://github.com/AntoineD/docstring-inheritance
+
 ## Status
 
 This package is actively used by the author. Please feel free to create a pull
 request for wanted features and suggestions!
 
 ## Quick start
 
@@ -99,14 +109,23 @@
 
 or
 
 ```bash
 conda install -c conda-forge module-utilities
 ```
 
+Optionally, you can install [docstring-inheritance] to use the `docinherit`
+module:
+
+```base
+pip install docstring-inheritance
+# or
+conda install -c conda-forge docstring-inheritance
+```
+
 ## Example usage
 
 Simple example of using `cached` module.
 
 ```pycon
 >>> from module_utilities import cached
 >>>
@@ -146,15 +165,15 @@
 [1]
 
 ```
 
 Simple example of using `DocFiller`.
 
 ```pycon
->>> from module_utilities.docfiller import DocFiller
+>>> from module_utilities.docfiller import DocFiller, indent_docstring
 >>> d = DocFiller.from_docstring(
 ...     """
 ...     Parameters
 ...     ----------
 ...     x : int
 ...         x param
 ...     y : int
@@ -184,27 +203,27 @@
 ...     {z0}
 ...     Returns
 ...     --------
 ...     {returns.output0}
 ...     """
 ...     return x + y + z
 ...
->>> print(func.__doc__.strip())
-Parameters
-----------
-x : int
-    x param
-y : int
-    y param
-z : int
-    z int param
-Returns
---------
-output : int
-    Integer output.
+>>> print(indent_docstring(func))
++  Parameters
++  ----------
++  x : int
++      x param
++  y : int
++      y param
++  z : int
++      z int param
++  Returns
++  --------
++  output : int
++      Integer output.
 
 # Note that for python version <= 3.8 that method chaining
 # in decorators doesn't work, so have to do the following.
 # For newer python, you can inline this.
 >>> dd = d.assign_keys(z='z0', out='returns.output0')
 >>> @dd.decorate
 ... def func1(x, y, z):
@@ -216,46 +235,46 @@
 ...     {z}
 ...     Returns
 ...     -------
 ...     {out}
 ...     """
 ...     pass
 ...
->>> print(func1.__doc__.strip())
-Parameters
-----------
-x : int
-    x param
-y : int
-    y param
-z : int
-    z int param
-Returns
--------
-output : int
-    Integer output.
+>>> print(indent_docstring(func1))
++  Parameters
++  ----------
++  x : int
++      x param
++  y : int
++      y param
++  z : int
++      z int param
++  Returns
++  -------
++  output : int
++      Integer output.
 
 >>> dd = d.assign_keys(z='z1', out='returns.output1')
 >>> @dd(func1)
 ... def func2(x, y, z):
 ...     pass
 
->>> print(func2.__doc__.strip())
-Parameters
-----------
-x : int
-    x param
-y : int
-    y param
-z : float
-    z float param
-Returns
--------
-output : float
-    Float output
+>>> print(indent_docstring(func2))
++  Parameters
++  ----------
++  x : int
++      x param
++  y : int
++      y param
++  z : float
++      z float param
++  Returns
++  -------
++  output : float
++      Float output
 
 
 ```
 
 <!-- end-docs -->
 
 ## Documentation
@@ -278,15 +297,15 @@
 [cmomy]: https://github.com/usnistgov/cmomy
 [analphipy]: https://github.com/usnistgov/analphipy
 [tmmc-lnpy]: https://github.com/usnistgov/tmmc-lnpy
 [thermoextrap]: https://github.com/usnistgov/thermoextrap
 
 ## Contact
 
-The author can be reached at wpk@nist.gov.
+The author can be reached at <wpk@nist.gov>.
 
 ## Credits
 
 This package was created with
 [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
 [wpk-nist-gov/cookiecutter-pypackage](https://github.com/wpk-nist-gov/cookiecutter-pypackage)
 Project template forked from
@@ -301,14 +320,22 @@
 ## Unreleased
 
 See the fragment files in
 [changelog.d](https://github.com/usnistgov/module-utilities)
 
 <!-- scriv-insert-here -->
 
+## v0.6.0 — 2023-08-01
+
+### Added
+
+- Now include module `docinhert` to interface with
+  [docstring-inheritance](https://github.com/AntoineD/docstring-inheritance)
+- Fully support mypy and pyright type checking.
+
 ## v0.5.0 — 2023-07-10
 
 ### Added
 
 - Add `_prepend` option to docfiller. Default behavior is now to append current
   docstring to templates.
```

### Comparing `module-utilities-0.5.0/src/module_utilities.egg-info/SOURCES.txt` & `module-utilities-0.6.0/src/module_utilities.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -49,60 +49,72 @@
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/module.rst
 docs/examples/index.md
 docs/examples/usage/cached.ipynb
 docs/examples/usage/docfiller.ipynb
 docs/reference/index.md
-environment/base.yaml
-environment/dev.yaml
-environment/dist-conda.yaml
 environment/dist-pypi.txt
-environment/dist-pypi.yaml
-environment/docs.yaml
-environment/lint.yaml
+environment/py310-dev.yaml
+environment/py310-dist-conda.yaml
+environment/py310-dist-pypi.yaml
+environment/py310-docs.yaml
+environment/py310-test-extras.yaml
+environment/py310-test-noopt.yaml
+environment/py310-test.yaml
+environment/py310-typing.yaml
+environment/py311-test-extras.yaml
+environment/py311-test-noopt.yaml
+environment/py311-test.yaml
+environment/py311-typing.yaml
+environment/py38-test-extras.yaml
+environment/py38-test-noopt.yaml
+environment/py38-test.yaml
+environment/py38-typing.yaml
+environment/py39-test-extras.yaml
+environment/py39-test-noopt.yaml
+environment/py39-test.yaml
+environment/py39-typing.yaml
 environment/test-extras.txt
-environment/test-extras.yaml
-environment/test.yaml
-environment/typing.yaml
+environment/lock/.gitignore
 environment/lock/py310-dev-conda-lock.yml
 environment/lock/py310-dist-conda-conda-lock.yml
 environment/lock/py310-dist-pypi-conda-lock.yml
 environment/lock/py310-test-conda-lock.yml
 environment/lock/py310-typing-conda-lock.yml
-environment/lock/py310.yaml
 environment/lock/py311-test-conda-lock.yml
 environment/lock/py311-typing-conda-lock.yml
-environment/lock/py311.yaml
 environment/lock/py38-test-conda-lock.yml
 environment/lock/py38-typing-conda-lock.yml
-environment/lock/py38.yaml
 environment/lock/py39-test-conda-lock.yml
 environment/lock/py39-typing-conda-lock.yml
-environment/lock/py39.yaml
 examples/README.md
 examples/usage/cached.ipynb
 examples/usage/docfiller.ipynb
 src/module_utilities/__init__.py
 src/module_utilities/_doc.py
 src/module_utilities/_typing.py
 src/module_utilities/_version.py
 src/module_utilities/attributedict.py
 src/module_utilities/cached.py
 src/module_utilities/docfiller.py
+src/module_utilities/docinherit.py
+src/module_utilities/options.py
 src/module_utilities/py.typed
 src/module_utilities.egg-info/PKG-INFO
 src/module_utilities.egg-info/SOURCES.txt
 src/module_utilities.egg-info/dependency_links.txt
 src/module_utilities.egg-info/requires.txt
 src/module_utilities.egg-info/top_level.txt
 src/module_utilities.egg-info/zip-safe
 src/module_utilities/vendored/LICENSE.txt
 src/module_utilities/vendored/README.txt
 src/module_utilities/vendored/__init__.py
 src/module_utilities/vendored/docscrape.py
 tests/__init__.py
 tests/conftest.py
+tests/test_attributedict.py
 tests/test_cached.py
 tests/test_docfiller.py
+tests/test_inherit.py
 tests/test_module_utilities.py
 tools/noxtools.py
```

### Comparing `module-utilities-0.5.0/tests/test_cached.py` & `module-utilities-0.6.0/tests/test_cached.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,77 @@
+# mypy: disable-error-code="no-untyped-def, no-untyped-call"
+
 from __future__ import annotations
 from typing import Any
 
 import pytest
 
 from module_utilities import cached
 
 
+# checking typeproperty
+
+
+def test_typeproperty():
+    class tmp:
+        _cache: dict[str, Any] = {}
+
+        @cached.TypedProperty
+        def thing(self):
+            return 1
+
+    x = tmp()
+    with pytest.raises(AttributeError):
+        x.thing = 2
+
+
+def test_meth_bad_hash():
+    # test that passing unhashable just returns the func
+    class tmp:
+        _cache: dict[str, Any] = {}
+
+        @cached.meth
+        def thing(self, x):
+            return x
+
+    x = tmp()
+
+    assert x.thing(1) == 1
+
+    assert "thing" in x._cache
+
+    x._cache = {}
+    v = {"a": 1}
+    assert x.thing(v) == v
+    assert len(x._cache["thing"]) == 0
+
+    # class tmp2:
+    #     def __init__(self):
+    #         self._cache: dict[str, Any] = {}
+
+    #     @cached.prop
+    #     def prop(self) -> int:
+    #         return 1
+
+    #     @cached.meth
+    #     def meth(self) -> int:
+    #         return 2
+
+    # y = tmp2()
+
+    # reveal_type(y.prop)
+    # reveal_type(y.meth)
+    # reveal_type(y.meth())
+
+
 class Baseclass:
     def __init__(self, a, b) -> None:
         self.a = a
         self.b = b
+        self._cache: dict[str, Any] = {}
 
     def get_value(self) -> tuple[Any, ...]:
         return self.a, self.b
 
     def get_xy(self, x, y) -> tuple[Any, ...]:
         return self.get_value() + (x, y)
 
@@ -37,20 +95,28 @@
     """test a single property"""
 
     if args is None:
         args = ()
     if kws is None:
         kws = {}
 
+    param = None
     if key is None:
         key = meth
+    elif isinstance(key, tuple):
+        key, param = key
 
     assert getattr(obj, meth)(*args, **kws) == value
     # test coming from cache
-    assert getattr(obj, meth)(*args, **kws) is obj._cache[key]
+
+    if param is None:
+        assert getattr(obj, meth)(*args, **kws) is obj._cache[key]
+    else:
+        assert getattr(obj, meth)(*args, **kws) is obj._cache[key][param]
+
     # test is same
     assert getattr(obj, meth)(*args, **kws) is getattr(obj, meth)(*args, **kws)
 
     if docstring is not None:
         assert getattr(type(obj), meth).__doc__ == docstring
 
 
@@ -127,50 +193,55 @@
     do_prop_test(test(1, 2), key="there")
 
 
 def do_meth_test(x, key=None, docstring="a doc string", check_empty=True) -> None:
     if key is None:
         key = "meth"
 
-    key_tot: tuple[str, tuple[Any, ...], frozenset[Any]] = (key, (3, 4), frozenset())
+    key_param: tuple[tuple[Any, ...], frozenset[Any]] = ((3, 4), frozenset())
+
+    key_tot = (key, key_param)
+
+    def test_keys(x):
+        assert tuple(x._cache.keys()) == (key,)
+        assert tuple(x._cache[key].keys()) == (key_param,)
 
     target = (1, 2, 3, 4)
     if check_empty:
         assert not hasattr(x, "_cache") or len(x._cache) == 0
     meth_test(x, "meth", target, args=(3, 4), key=key_tot, docstring=docstring)
-
-    assert tuple(x._cache.keys()) == (key_tot,)  # pytype: disable=attribute-error
+    test_keys(x)
 
     # change value
     x.a = 2
     x.b = 4
 
     meth_test(x, "meth", target, args=(3, 4), key=key_tot, docstring=docstring)
-    assert tuple(x._cache.keys()) == (key_tot,)  # pytype: disable=attribute-error
+    test_keys(x)
 
     # remove cache:
     del x._cache
     target = (2, 4, 3, 4)
     meth_test(x, "meth", target, args=(3, 4), key=key_tot, docstring=docstring)
-    assert tuple(x._cache.keys()) == (key_tot,)  # pytype: disable=attribute-error
+    test_keys(x)
 
     # getting write signature
     del x._cache
     meth_test(x, "meth", target, kws=dict(x=3, y=4), key=key_tot, docstring=docstring)
-    assert tuple(x._cache.keys()) == (key_tot,)  # pytype: disable=attribute-error
+    test_keys(x)
 
     del x._cache
     meth_test(x, "meth", target, kws=dict(y=4, x=3), key=key_tot, docstring=docstring)
-    assert tuple(x._cache.keys()) == (key_tot,)  # pytype: disable=attribute-error
+    test_keys(x)
 
     del x._cache
     meth_test(
         x, "meth", target, args=(3,), kws=dict(y=4), key=key_tot, docstring=docstring
     )
-    assert tuple(x._cache.keys()) == (key_tot,)  # pytype: disable=attribute-error
+    test_keys(x)
 
 
 def test_meth() -> None:
     class test(Baseclass):
         @cached.decorate(as_property=False)
         def meth(self, x, y):
             "a doc string"
@@ -266,31 +337,42 @@
             pass
 
         @cached.meth
         def meth(self, x, y):
             "a doc string"
             return self.get_xy(x, y)
 
+        # check that clearing unknown key is fine
+        @cached.clear("a_meth_that_isnt_there")
+        def clear_missing(self) -> None:
+            pass
+
     x = test(1, 2)
     key_prop = "prop"
-    key_meth = ("meth", (3, 4), frozenset())  # type: ignore
+    key_meth = ("meth", ((3, 4), frozenset()))  # type: ignore
     docstring = "a doc string"
     prop_test(x, prop="prop", value=(1, 2), key=key_prop, docstring=docstring)
     meth_test(
         x,
         meth="meth",
         value=(1, 2, 3, 4),
         args=(3, 4),
         key=key_meth,
         docstring=docstring,
     )
 
+    keys0 = list(x._cache.keys())
+
+    x.clear_missing()
+
+    assert list(x._cache.keys()) == keys0
+
     # this clears the cache
     x.a, x.b = 2, 4
-    key_meth = ("meth", (3, 4), frozenset())
+    key_meth = ("meth", ((3, 4), frozenset()))
     docstring = "a doc string"
     prop_test(x, prop="prop", value=(2, 4), key=key_prop, docstring=docstring)
     meth_test(
         x,
         meth="meth",
         value=(2, 4, 3, 4),
         args=(3, 4),
@@ -302,36 +384,40 @@
 
     x.clear_all()
     assert len(x._cache) == 0
 
     x.prop
     x.meth(3, 4)
 
+    def _test_key_meth(key_meth, x):
+        assert key_meth[0] in x._cache
+        assert key_meth[1] in x._cache[key_meth[0]]
+
     assert key_prop in x._cache
-    assert key_meth in x._cache
+    _test_key_meth(key_meth, x)
 
     x.test_prop
     assert "test_prop" in x._cache
     x.aprop = 2
     assert key_prop not in x._cache
     assert "test_prop" not in x._cache
-    assert key_meth in x._cache
+    _test_key_meth(key_meth, x)
 
     x.prop
     x.meth(3, 4)
     x.meth(5, 6)
-    key_meth2 = ("meth", (5, 6), frozenset())  # type: ignore
+    key_meth2 = ("meth", ((5, 6), frozenset()))  # type: ignore
 
     assert key_prop in x._cache
-    assert key_meth in x._cache
-    assert key_meth2 in x._cache
+    _test_key_meth(key_meth, x)
+    _test_key_meth(key_meth2, x)
 
     x.clear_meth()
-    assert key_meth not in x._cache
-    assert key_meth2 not in x._cache
+    assert key_meth[0] not in x._cache
+    assert key_meth2[0] not in x._cache
     assert key_prop in x._cache
 
 
 def test_use_cache() -> None:
     class tmp:
         _use_cache = False
 
@@ -350,24 +436,38 @@
         def prop2(self):
             return [1, 2]
 
         @cached.decorate()
         def prop3(self):
             return [1, 2]
 
+        @cached.meth
+        def meth0(self):
+            return [1, 2]
+
+        @cached.meth(check_use_cache=True)
+        def meth1(self):
+            return [1, 2]
+
     x = tmp()
 
     for p in ["prop0", "prop2"]:
         assert getattr(x, p) is not getattr(x, p)
         assert not hasattr(x, "_cache") or p not in x._cache
 
     for p in ["prop1", "prop3"]:
         assert getattr(x, p) is getattr(x, p)
         assert p in x._cache
 
+    assert x.meth0() is x.meth0()
+    assert x.meth1() is not x.meth1()
+
+    assert "meth0" in x._cache
+    assert "meth1" not in x._cache
+
 
 def test_use_cache2() -> None:
     class tmp:
         _use_cache = True
 
         def __init__(self):
             self._cache = {}
@@ -376,24 +476,65 @@
         def prop0(self):
             return [1, 2]
 
         @cached.prop
         def prop1(self):
             return [2, 3]
 
-        @cached.decorate(check_use_cache=True)
-        def prop2(self):
+        @cached.decorate(check_use_cache=True, key="prop2")
+        def prop2(self) -> list[int]:
             return [1, 2]
 
         @cached.decorate()
-        def prop3(self):
+        def prop3(self) -> list[int]:
             return [1, 2]
 
+        @cached.decorate(check_use_cache=True, as_property=False)
+        def meth(self) -> list[int]:
+            return [1, 2, 3]
+
+        @cached.meth
+        def meth1(self) -> list[int]:
+            return [1, 2, 3]
+
+        @cached.meth(key="a thing")
+        def meth2(self, a: int) -> list[int]:
+            return [a] + self.prop3
+
+        @cached.decorate(key="there", as_property=False)
+        def there(self) -> list[int]:
+            return [1, 2]
+
+        @cached.decorate(key="something")
+        def prop4(self) -> list[int]:
+            return [1, 2]
+
+        @property
+        @cached.clear
+        def prop_test(self) -> list[int]:
+            return [1, 2]
+
+        @cached.clear("meth1")
+        def clearer(self) -> list[int]:
+            return [1, 2]
+
+        clearer = cached.clear(clearer, "meth2")
+
     x = tmp()
 
+    # if TYPE_CHECKING:
+    #     reveal_type(x.prop2)
+    #     reveal_type(x.meth())
+    #     reveal_type(x.there())
+    #     reveal_type(x.prop4)
+    #     reveal_type(x.meth1())
+    #     reveal_type(x.meth2(2))
+    #     reveal_type(x.prop_test)
+    #     reveal_type(x.clearer())
+
     for p in ["prop0", "prop1", "prop2", "prop3"]:
         assert getattr(x, p) is getattr(x, p)
         assert p in x._cache
 
 
 def test_use_cache3() -> None:
     # if not have _use_cache parameter
@@ -425,38 +566,59 @@
 
     for p in ["prop1", "prop3"]:
         assert getattr(x, p) is getattr(x, p)
         assert p in x._cache
 
 
 def test_error_with_slots():
+    # ignore type errors here
+    # the point is to make sure errors happen here.
     class test:
         __slots__ = ["a", "b"]
 
         def __init__(self, a, b):
             self.a = a
             self.b = b
 
-        @cached.prop
+        @cached.prop  # type: ignore
         def prop(self):
             return self.a, self.b
 
     x = test(1, 2)
 
     with pytest.raises(AttributeError):
         x.prop
 
+    # but this should work fine:
+    class test2:
+        __slots__ = ["a", "b", "_cache"]
+
+        def __init__(self, a, b):
+            self.a = a
+            self.b = b
+            self._cache: dict[str, Any] = {}
+
+        @cached.prop
+        def prop(self):
+            return self.a, self.b
+
+    x2 = test2(1, 2)
+
+    assert x2.prop == (1, 2)
+    assert x2._cache["prop"] == (1, 2)
+
 
 def test_error_with_slots2():
     class test:
         __slots__ = ["a", "b", "_cache"]
 
         def __init__(self, a, b):
             self.a = a
             self.b = b
+            self._cache: dict[str, Any] = {}
 
         @cached.prop
         def prop(self):
             "a doc string"
             return self.a, self.b
 
     x = test(1, 2)
```

### Comparing `module-utilities-0.5.0/tests/test_docfiller.py` & `module-utilities-0.6.0/tests/test_docfiller.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,206 @@
+# mypy: disable-error-code="no-untyped-def"
 from __future__ import annotations
 from textwrap import dedent
+from typing import cast
 
 # from typing import TYPE_CHECKING
 # from typing_extensions import reveal_type
 
 import pytest
 
 from module_utilities import docfiller
 from module_utilities.docfiller import DocFiller, dedent_recursive
 
 # just testing on doc routine:
 
 
+# --- simple (coverage filler) tests ---------------------------------------------------
+
+
+def test_append():
+    def func():
+        """Hello"""
+
+    @docfiller.doc_decorate(func, x="there")
+    def func1():
+        """{x}"""
+
+    assert func1.__doc__.strip() == "Hellothere"  # type: ignore
+
+    @docfiller.doc_decorate(func, x="some", _prepend=True)
+    def func2():
+        """Yell"""
+
+    assert func2.__doc__ == "YellHello"
+
+    def func_none():
+        pass
+
+    func_none.__doc__ = None
+
+    @docfiller.doc_decorate(None, x="there")
+    def func3():
+        """Hello {x}"""
+        pass
+
+    assert func3.__doc__ == "Hello there"
+
+    docfiller.DOC_SUB = False  # type: ignore
+
+    @docfiller.doc_decorate(func1, x="hello")
+    def func4a():
+        """{x}"""
+
+    docfiller.DOC_SUB = True  # type: ignore
+
+    assert func4a.__doc__ == "{x}"
+
+
+def test_indent_docstring():
+    assert docfiller.indent_docstring("hello", prefix=" ") == " hello"
+    assert docfiller.indent_docstring("hello", prefix=None) == "hello"
+
+
+def test_build_params_docstring():
+    with pytest.raises(ValueError):
+        s = docfiller._build_param_docstring(name="", ptype="", desc=["hello"])
+
+    s = docfiller._build_param_docstring(name="hello", ptype=None, desc="stuff")
+
+    assert (
+        s
+        == dedent(
+            """
+    hello
+        stuff
+    """
+        ).strip()
+    )
+
+    s = docfiller._build_param_docstring(name="hello", ptype=None, desc="")
+
+    assert s == "hello"
+
+    s = docfiller._build_param_docstring(name="hello", ptype=None, desc=[""])
+
+    assert s == "hello"
+
+
+def test_params_to_string():
+    s = docfiller._params_to_string("hello")
+    assert s == "hello"
+
+
+def test_func_or_doc():
+    def template():
+        """
+        Parameters
+        ----------
+        x : int
+        """
+
+    d = DocFiller.from_docstring(template, combine_keys="parameters")
+
+    @d.decorate
+    def func():
+        """{x}"""
+
+    assert func.__doc__ == "x : int"
+
+
+def test_docfiller_creation():
+    d = DocFiller([("x", "hello")])  # type: ignore
+
+    @d.decorate
+    def func():
+        "{x}"
+
+    assert func.__doc__ == "hello"
+
+    assert repr(d) == "DocFiller({'x': 'hello'})"
+
+
+def test_DocFiller_getitem():
+    d = DocFiller.from_docstring(
+        """
+    Parameters
+    ----------
+    x : int
+    y : float
+    """,
+        keep_keys="parameters",
+    )
+
+    dd = cast(DocFiller, d["parameters"])
+
+    @dd.decorate
+    def func():
+        """{x}"""
+
+    assert func.__doc__ == "x : int"
+
+    @dd.decorate
+    def func1():
+        """
+        {x}
+        {y}
+        """
+
+    ddd = dd.assign_combined_key("z", ["x", "y"])
+
+    @ddd.decorate
+    def func2():
+        """
+        {z}
+        """
+
+    assert func1.__doc__ == func2.__doc__
+
+    with pytest.raises(ValueError):
+        ddd = d.assign_combined_key("zz", ["parameters"])
+
+    d = DocFiller.from_docstring(
+        """
+    Parameters
+    ----------
+    x : int
+    y : float
+    """,
+        keep_keys=False,
+        combine_keys="parameters",
+        key_map=lambda x: "hello_" + x,
+    )
+
+    @d.decorate
+    def func3():
+        """{hello_x}"""
+
+    assert func3.__doc__ == "x : int"
+
+    d = DocFiller.from_docstring(
+        """
+    Parameters
+    ----------
+    x : int
+    y : float
+    """,
+        keep_keys=False,
+        combine_keys="parameters",
+        key_map={"x": "hello_x", "y": "hello_y"},
+        namespace="top",
+    )
+
+    @d.decorate
+    def func4():
+        """{top.hello_x}"""
+
+    assert func4.__doc__ == "x : int"
+
+
 @pytest.fixture
 def params():
     return dedent_recursive(
         dict(
             summary="A thing",
             a="""
             a : int
@@ -219,15 +404,15 @@
         ----------
         {a}
         {b}
         {hello}
         {there}
         """
 
-    expected = docfiller.dedent(
+    expected = dedent(
         """
     A summary line
 
     Parameters
     ----------
     a : int
         A parameter
@@ -295,17 +480,19 @@
     """
 
     d0 = docfiller.DocFiller.from_docstring(s0)
     d1 = docfiller.DocFiller.from_docstring(s1)
 
     dd0 = d0.insert_level("a").append(d1.insert_level("b"))
 
-    dd1 = docfiller.DocFiller.concat(a=d0, b=d1)
+    dd1 = docfiller.DocFiller.concat(a=d0, b=d1, c={"type_": "int"})
+
+    assert dd1["c"]["type_"] == "int"  # type: ignore
 
-    expected = docfiller.dedent(
+    expected = dedent(
         """
         Parameters
         ----------
         a : int
             A param
         b : float
             BB param
@@ -332,19 +519,23 @@
             {b.returns.out}
             """
 
             pass
 
         assert func.__doc__ == expected
 
+    with pytest.raises(ValueError):
+        d0.assign(x="hello").levels_to_top("x")
+
     dd0 = (
         d0.rename_levels(parameters="p", returns="r")
         .levels_to_top("p", "r")
         .insert_level("a")
     )
+
     dd1 = (
         d1.rename_levels(parameters="p", returns="r")
         .levels_to_top("p", "r")
         .insert_level("b")
     )
 
     dd = dd0.append(dd1)
@@ -571,37 +762,44 @@
         output
     """
 
     expected = dedent(expected)
 
     d = DocFiller.from_docstring(expected, combine_keys="parameters")
 
-    def template():
+    def template(x: float, y: float) -> float:
         """
         {summary}
 
         {extended_summary}
 
         Parameters
         ----------
         {x}
         {y}
         """
+        return x + y
+
+    # reveal_type(template)
+    # reveal_type(template(1.0, 2.0))
 
     @d(template)
-    def hello():
+    def hello(x: float, y: float) -> float:
         """
         Returns
         -------
         {returns.out}
         """
-        pass
+        return x + y
 
     assert hello.__doc__ == expected
 
+    # reveal_type(hello)
+    # reveal_type(hello(1., 2.))
+
     # prepend
     @d(template, _prepend=True)
     def there():
         """
         Returns
         -------
         {returns.out}
```

### Comparing `module-utilities-0.5.0/tools/noxtools.py` & `module-utilities-0.6.0/tools/noxtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-"""Utilities to work with nox"""
+"""Utilities to work with nox."""
 
 from __future__ import annotations
 
 import shlex
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Iterable, Literal, cast
+from typing import TYPE_CHECKING, Any, Iterable, Literal, Sequence, cast
 
 from ruamel.yaml import safe_load
 
 if TYPE_CHECKING:
-    from collections.abc import Collection, Sequence
+    from collections.abc import Collection
 
     import nox
 
 
 # --- Basic utilities -------------------------------------------------------------------
 def combine_list_str(opts: list[str]) -> list[str]:
     if opts:
@@ -48,27 +48,30 @@
     else:
         target_time = target_path.stat().st_mtime
         update = any(target_time < dep.stat().st_mtime for dep in deps_path)
 
     return update
 
 
-def prepend_flag(flag: str, *args: str) -> list[str]:
+def prepend_flag(flag: str, *args: str | Sequence[str]) -> list[str]:
     """
     Add in a flag before each arg.
 
     >>> prepent_flag("-k", "a", "b")
     ["-k", "a", "-k", "b"]
-
     """
 
-    if len(args) == 1 and not isinstance(args[0], str):
-        args = args[0]
+    args_ = []
+    for x in args:
+        if isinstance(x, str):
+            args_.append(x)
+        else:
+            args_.extend(x)
 
-    return sum([[flag, _] for _ in args], [])
+    return sum([[flag, _] for _ in args_], [])
 
 
 def open_webpage(path: str | Path | None = None, url: str | None = None):
     """
     Open webpage from path or url.
 
     Useful if want to view webpage with javascript, etc., as well as static html.
@@ -93,22 +96,21 @@
     paths = ["~/.conda/envs/test-3.*/bin"]
 
     # Extras for environments
     # for example, could have
     # dev = ["dev", "nox", "tools"]
     [nox.extras]
     dev = ["dev", "nox"]
-
     """
     import os
     from glob import glob
 
     import tomli
 
-    config = {}
+    config: dict[str, Any] = {}
 
     path = Path(path)
     if not path.exists():
         return config
 
     with path.open("rb") as f:
         data = tomli.load(f)
@@ -148,15 +150,15 @@
     """
     return session._runner.global_config.no_install and session._runner.venv._reused  # type: ignore
 
 
 def session_run_commands(
     session: nox.Session, commands: list[list[str]], external: bool = True, **kws: Any
 ) -> None:
-    """Run commands command"""
+    """Run commands command."""
 
     if commands:
         kws.update(external=external)
         for opt in combine_list_list_str(commands):
             session.run(*opt, **kws)
 
 
@@ -203,15 +205,15 @@
     session: nox.Session,
     lockfile: str | Path,
     extras: str | list[str] | None = None,
     display_name: str | None = None,
     force_reinstall: bool = False,
     install_package: bool = False,
 ) -> bool:
-    """Install depedencies using conda-lock"""
+    """Install depedencies using conda-lock."""
 
     if session_skip_install(session):
         return True
 
     unchanged, hashes = env_unchanged(
         session, lockfile, prefix="lock", other=dict(install_package=install_package)
     )
@@ -367,21 +369,23 @@
     force_reinstall: bool = False,
     install_package: bool = False,
     no_deps: bool = False,
 ):
     if session_skip_install(session):
         return True
 
-    def _check_param(x):
+    def _check_param(x) -> list[str]:
         if x is None:
             return []
         elif isinstance(x, str):
             return [x]
-        else:
+        elif isinstance(x, list):
             return x
+        else:
+            return list(x)
 
     extras = _check_param(extras)
     if extras:
         install_package = True
         extras = ",".join(extras)
         install_package_args = ["-e", f".[{extras}]"]
     elif install_package:
@@ -455,18 +459,18 @@
 
     return unchanged, hashes
 
 
 def get_hashes(
     *paths: str | Path,
     other: dict[str, Any] | None = None,
-) -> dict[str, str]:
-    """Get md5 hashes for paths"""
+) -> dict[str, Any]:
+    """Get md5 hashes for paths."""
 
-    out = {"path": {str(path): _get_file_hash(path) for path in paths}}
+    out: dict[str, Any] = {"path": {str(path): _get_file_hash(path) for path in paths}}
 
     if other:
         import hashlib
 
         other_hashes = {}
         for k, v in other.items():
             if isinstance(v, str):
@@ -480,15 +484,15 @@
 
         out["other"] = other_hashes
 
     return out
 
 
 def hashfile_path(session: nox.Session, prefix: PREFIX_HASH_EXTS) -> Path:
-    """Path for hashfile for this session"""
+    """Path for hashfile for this session."""
     return Path(session.create_tmp()) / f"{prefix}.json"
 
 
 def write_hashfile(
     hashes: dict[str, str],
     session: nox.Session,
     prefix: PREFIX_HASH_EXTS,
```

