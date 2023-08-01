# Comparing `tmp/fprime-tools-3.2.1.tar.gz` & `tmp/fprime-tools-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fprime-tools-3.2.1.tar", last modified: Sun Apr 23 06:08:27 2023, max compression
+gzip compressed data, was "fprime-tools-3.3.0.tar", last modified: Tue Aug  1 20:55:21 2023, max compression
```

## Comparing `fprime-tools-3.2.1.tar` & `fprime-tools-3.3.0.tar`

### file list

```diff
@@ -1,164 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.821006 fprime-tools-3.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.809006 fprime-tools-3.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.809006 fprime-tools-3.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/ISSUE_TEMPLATE/feature-request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.805006 fprime-tools-3.2.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.809006 fprime-tools-3.2.1/.github/actions/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/actions/codeql/security-pack.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.809006 fprime-tools-3.2.1/.github/actions/spelling/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/actions/spelling/allow.txt
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/actions/spelling/excludes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/actions/spelling/expect.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/actions/spelling/patterns.txt
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.809006 fprime-tools-3.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/workflows/codeql-security-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/workflows/fprime-tools-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/workflows/integration-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.github/workflows/spelling.yml
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-23 06:08:27.821006 fprime-tools-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.809006 fprime-tools-3.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.805006 fprime-tools-3.2.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.809006 fprime-tools-3.2.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/docs/_static/css/rtd_width.css
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      162 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/docs/gendoc.bash
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/pylama.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-23 06:08:27.821006 fprime-tools-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.805006 fprime-tools-3.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.809006 fprime-tools-3.2.1/src/fprime/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.809006 fprime-tools-3.2.1/src/fprime/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.809006 fprime-tools-3.2.1/src/fprime/common/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.813006 fprime-tools-3.2.1/src/fprime/common/models/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/models/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/models/serialize/array_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/models/serialize/bool_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/models/serialize/enum_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/models/serialize/numerical_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/models/serialize/serializable_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/models/serialize/string_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/models/serialize/time_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/models/serialize/type_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/models/serialize/type_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.813006 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/CMakeLists_template.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.813006 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.813006 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/pre_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.813006 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.813006 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/docs/sdd.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.fpp
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.813006 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.813006 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.813006 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/instances.fpp
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/topology.fpp
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Packets.xml
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Topology.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Topology.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}TopologyDefs.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/settings.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.813006 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.813006 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/hooks/post_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.813006 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/project.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/cookiecutter_templates/port_template.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.817006 fprime-tools-3.2.1/src/fprime/fbuild/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/fbuild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22534 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/fbuild/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/fbuild/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    27170 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/fbuild/cmake.py
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/fbuild/gcovr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/fbuild/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/fbuild/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/fbuild/target_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/fbuild/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.817006 fprime-tools-3.2.1/src/fprime/fpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/fpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/fpp/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/fpp/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.817006 fprime-tools-3.2.1/src/fprime/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/util/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/util/build_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10577 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/util/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/util/code_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/util/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    17944 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/util/cookiecutter_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18728 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/util/help_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/util/string_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/src/fprime/util/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.817006 fprime-tools-3.2.1/src/fprime_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-23 06:08:27.000000 fprime-tools-3.2.1/src/fprime_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-23 06:08:27.000000 fprime-tools-3.2.1/src/fprime_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:08:27.000000 fprime-tools-3.2.1/src/fprime_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-23 06:08:27.000000 fprime-tools-3.2.1/src/fprime_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-23 06:08:27.000000 fprime-tools-3.2.1/src/fprime_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 06:08:27.000000 fprime-tools-3.2.1/src/fprime_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.805006 fprime-tools-3.2.1/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.805006 fprime-tools-3.2.1/test/fprime/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.805006 fprime-tools-3.2.1/test/fprime/common/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.805006 fprime-tools-3.2.1/test/fprime/common/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.817006 fprime-tools-3.2.1/test/fprime/common/models/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)    18469 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/common/models/serialize/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/common/models/serialize/time_type_unit_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.817006 fprime-tools-3.2.1/test/fprime/fbuild/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.809006 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.817006 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/external/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/external/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.817006 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/grand-unified/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/grand-unified/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.817006 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/subdir/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/subdir/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.817006 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.817006 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/build-fprime-automatic-native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/build-fprime-automatic-native/CMakeCache.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/build-fprime-automatic-native/hashes.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/settings.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.821006 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/subdir1/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/subdir1/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.821006 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/subdir1/build-fprime-automatic-abcdefg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/subdir1/build-fprime-automatic-abcdefg/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.809006 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.809006 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/subdir3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.821006 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/subdir3/build-fprime-automatic-default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/subdir3/build-fprime-automatic-default/CMakeCache.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:08:27.821006 fprime-tools-3.2.1/test/fprime/fbuild/settings-data/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/settings-data/settings-custom-install.ini
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/settings-data/settings-custom-toolchain.ini
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/settings-data/settings-empty.ini
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/settings-data/settings-multi-line-default-options.ini
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/settings-data/settings-outside-cookiecutter.ini
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-23 06:07:59.000000 fprime-tools-3.2.1/test/fprime/fbuild/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.559655 fprime-tools-3.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.535654 fprime-tools-3.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.539654 fprime-tools-3.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/ISSUE_TEMPLATE/feature-request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.523653 fprime-tools-3.3.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.539654 fprime-tools-3.3.0/.github/actions/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/actions/codeql/security-pack.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.539654 fprime-tools-3.3.0/.github/actions/spelling/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/actions/spelling/allow.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/actions/spelling/excludes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/actions/spelling/expect.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/actions/spelling/patterns.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.543654 fprime-tools-3.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/workflows/codeql-security-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/workflows/fprime-tools-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/workflows/integration-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.github/workflows/spelling.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-01 20:55:21.559655 fprime-tools-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.543654 fprime-tools-3.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.523653 fprime-tools-3.3.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.543654 fprime-tools-3.3.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/docs/_static/css/rtd_width.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      162 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/docs/gendoc.bash
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/pylama.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-01 20:55:21.559655 fprime-tools-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.527654 fprime-tools-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.543654 fprime-tools-3.3.0/src/fprime/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.543654 fprime-tools-3.3.0/src/fprime/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.543654 fprime-tools-3.3.0/src/fprime/common/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.547655 fprime-tools-3.3.0/src/fprime/common/models/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/models/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/models/serialize/array_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/models/serialize/bool_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/models/serialize/enum_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/models/serialize/numerical_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6727 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/models/serialize/serializable_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/models/serialize/string_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/models/serialize/time_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/models/serialize/type_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/models/serialize/type_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.527654 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.551655 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.551655 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/pre_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.551655 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.551655 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/docs/sdd.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.fpp
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.551655 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.551655 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.551655 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/instances.fpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/topology.fpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Packets.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Topology.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Topology.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}TopologyDefs.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.551655 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.551655 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/hooks/post_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.551655 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.551655 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/Components/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/Components/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/project.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/settings.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.551655 fprime-tools-3.3.0/src/fprime/fbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/fbuild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/fbuild/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/fbuild/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27192 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/fbuild/cmake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/fbuild/gcovr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/fbuild/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/fbuild/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/fbuild/target_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/fbuild/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.555655 fprime-tools-3.3.0/src/fprime/fpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/fpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/fpp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/fpp/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/fpp/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.555655 fprime-tools-3.3.0/src/fprime/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/util/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/util/build_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/util/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/util/code_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/util/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/util/cookiecutter_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/util/help_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/util/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/src/fprime/util/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.555655 fprime-tools-3.3.0/src/fprime_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-01 20:55:21.000000 fprime-tools-3.3.0/src/fprime_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-08-01 20:55:21.000000 fprime-tools-3.3.0/src/fprime_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:55:21.000000 fprime-tools-3.3.0/src/fprime_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-01 20:55:21.000000 fprime-tools-3.3.0/src/fprime_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-01 20:55:21.000000 fprime-tools-3.3.0/src/fprime_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 20:55:21.000000 fprime-tools-3.3.0/src/fprime_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.527654 fprime-tools-3.3.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.531654 fprime-tools-3.3.0/test/fprime/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.531654 fprime-tools-3.3.0/test/fprime/common/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.531654 fprime-tools-3.3.0/test/fprime/common/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.555655 fprime-tools-3.3.0/test/fprime/common/models/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)    18462 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/common/models/serialize/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/common/models/serialize/time_type_unit_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.555655 fprime-tools-3.3.0/test/fprime/fbuild/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.531654 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.555655 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/external/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.555655 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/grand-unified/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/grand-unified/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.555655 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/subdir/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/subdir/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.555655 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.555655 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/build-fprime-automatic-native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/build-fprime-automatic-native/CMakeCache.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/build-fprime-automatic-native/hashes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/settings.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.559655 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/subdir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/subdir1/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.559655 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/subdir1/build-fprime-automatic-abcdefg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/subdir1/build-fprime-automatic-abcdefg/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.535654 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.535654 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/subdir3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.559655 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/subdir3/build-fprime-automatic-default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/cmake-data/testbuild/subdir1/subdir2/subdir3/build-fprime-automatic-default/CMakeCache.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:55:21.559655 fprime-tools-3.3.0/test/fprime/fbuild/settings-data/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/settings-data/settings-custom-install.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/settings-data/settings-custom-toolchain.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/settings-data/settings-empty.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/settings-data/settings-multi-line-default-options.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/settings-data/settings-outside-cookiecutter.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-08-01 20:54:58.000000 fprime-tools-3.3.0/test/fprime/fbuild/test_settings.py
```

### Comparing `fprime-tools-3.2.1/.github/actions/spelling/expect.txt` & `fprime-tools-3.3.0/.github/actions/spelling/expect.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 cfg
 ci
 cls
 cmake
 cmakelists
 cmp
 commonprefix
+Comms
 config
 configparser
 configs
 confparse
 consts
 contextlib
 contextmanager
@@ -28,15 +29,15 @@
 ctor
 cwd
 CXX
 datetime
 dedent
 deduplicated
 deepcopy
-Deframer
+deframer
 deframing
 DEPS
 deser
 deserialization
 deserialize
 deserialized
 deserializer
@@ -46,15 +47,15 @@
 dfl
 dinkel
 dirname
 dirone
 dirs
 distutils
 doctest
-Drv
+drv
 dumpable
 Dxyz
 elif
 endfor
 endif
 endswith
 entrypoint
@@ -70,14 +71,15 @@
 filecmp
 FILEID
 fileobj
 filepath
 firest
 floordiv
 FPGA
+fpl
 fpp
 fprime
 fromkeys
 fromtimestamp
 func
 funcs
 functools
@@ -219,19 +221,21 @@
 stackoverflow
 startswith
 staticmethod
 stderr
 stdin
 stdint
 stdout
+STest
 strftime
 stylesheet
 subdir
 subparser
 Subproc
+subtopology
 sys
 tcanham
 Tcp
 td
 tempdir
 tempfile
 testbuild
```

### Comparing `fprime-tools-3.2.1/.github/actions/spelling/patterns.txt` & `fprime-tools-3.3.0/.github/actions/spelling/patterns.txt`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/.github/pull_request_template.md` & `fprime-tools-3.3.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/.github/workflows/codeql-security-scan.yml` & `fprime-tools-3.3.0/.github/workflows/codeql-security-scan.yml`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/.github/workflows/fprime-tools-ci.yml` & `fprime-tools-3.3.0/.github/workflows/fprime-tools-ci.yml`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/.github/workflows/integration-tests.yml` & `fprime-tools-3.3.0/.github/workflows/integration-tests.yml`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/.github/workflows/publish.yml` & `fprime-tools-3.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/.github/workflows/spelling.yml` & `fprime-tools-3.3.0/.github/workflows/spelling.yml`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/LICENSE.txt` & `fprime-tools-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/NOTICE.txt` & `fprime-tools-3.3.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/PKG-INFO` & `fprime-tools-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fprime-tools
-Version: 3.2.1
+Version: 3.3.0
 Summary: F Prime Flight Software core data types
 Home-page: https://github.com/nasa/fprime
 Author: Michael Starch
 Author-email: Michael.D.Starch@jpl.nasa.gov
 License: Apache 2.0 License
 Project-URL: Issue Tracker, https://github.com/nasa/fprime/issues
 Keywords: fprime,embedded,nasa
```

### Comparing `fprime-tools-3.2.1/README.md` & `fprime-tools-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/docs/_static/css/rtd_width.css` & `fprime-tools-3.3.0/docs/_static/css/rtd_width.css`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/docs/conf.py` & `fprime-tools-3.3.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import re
 from datetime import datetime
 from importlib import import_module
 from pathlib import Path
 
 import sphinx_rtd_theme  # pylint: disable=unused-import
 
-
 # importlib.metadata is implemented in Python 3.8
 # Previous versions require the backport, https://pypi.org/project/importlib-metadata/
 try:
     metadata = import_module("importlib.metadata")
 except ModuleNotFoundError:
     metadata = import_module("importlib_metadata")
```

### Comparing `fprime-tools-3.2.1/docs/index.rst` & `fprime-tools-3.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/pylama.cfg` & `fprime-tools-3.3.0/pylama.cfg`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/setup.py` & `fprime-tools-3.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,16 +82,17 @@
     python_requires=">=3.7",
     install_requires=[
         "lxml>=4.6.3",
         "Markdown>=3.3.4",
         "pexpect>=4.8.0",
         "pytest>=6.2.4",
         "Cheetah3>=3.2.6",
-        "cookiecutter>=1.7.2",
-        "gcovr>=5.0",
+        "cookiecutter>=2.2.3",
+        "gcovr>=6.0",
+        "urllib3<2.0.0",
     ],
     extras_require={
         "dev": [
             "black",
             "pylama",
             "pylint",
             "pre-commit",
```

### Comparing `fprime-tools-3.2.1/src/fprime/common/models/serialize/__init__.py` & `fprime-tools-3.3.0/src/fprime/common/models/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/common/models/serialize/array_type.py` & `fprime-tools-3.3.0/src/fprime/common/models/serialize/array_type.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """ Generic representation of autocoded array types
 
 Created on May 29, 2020
 @author: jishii
 """
+from fprime.util.string_util import format_string_template
+
+from . import serializable_type
 from .type_base import DictionaryType
 from .type_exceptions import (
     ArrayLengthException,
     NotInitializedException,
     TypeMismatchException,
 )
 
-from . import serializable_type
-from fprime.util.string_util import format_string_template
-
 
 class ArrayType(DictionaryType):
     """Generic fixed-size array type representation.
 
     Represents a custom named type of a fixed number of like members, each of which are other types in the system.
     """
```

### Comparing `fprime-tools-3.2.1/src/fprime/common/models/serialize/bool_type.py` & `fprime-tools-3.3.0/src/fprime/common/models/serialize/bool_type.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/common/models/serialize/enum_type.py` & `fprime-tools-3.3.0/src/fprime/common/models/serialize/enum_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,17 +72,16 @@
     def deserialize(self, data, offset):
         """
         Deserialize the enumeration using an int type
         """
         try:
             int_val = struct.unpack_from(">i", data, offset)[0]
         except struct.error:
-            raise DeserializeException(
-                f"Could not deserialize enum value. Needed: {self.getSize()} bytes Found: {len(data[offset:])}"
-            )
+            msg = f"Could not deserialize enum value. Needed: {self.getSize()} bytes Found: {len(data[offset:])}"
+            raise DeserializeException(msg)
         for key, val in self.ENUM_DICT.items():
             if int_val == val:
                 self._val = key
                 break
         # Value not found, invalid enumeration value
         else:
             raise TypeRangeException(int_val)
```

### Comparing `fprime-tools-3.2.1/src/fprime/common/models/serialize/numerical_types.py` & `fprime-tools-3.3.0/src/fprime/common/models/serialize/numerical_types.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/common/models/serialize/serializable_type.py` & `fprime-tools-3.3.0/src/fprime/common/models/serialize/serializable_type.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 Created on Dec 18, 2014
 
 @author: tcanham
 
 """
+from fprime.util.string_util import format_string_template
+
+from . import array_type
 from .type_base import BaseType, DictionaryType
 from .type_exceptions import (
     IncorrectMembersException,
     MissingMemberException,
     NotInitializedException,
     TypeMismatchException,
 )
 
-from . import array_type
-from fprime.util.string_util import format_string_template
-
 
 class SerializableType(DictionaryType):
     """
     Representation of the Serializable type (comparable to the ANY type)
 
     The serializable type is a container for other instances of
     BaseType, including itself.
```

### Comparing `fprime-tools-3.2.1/src/fprime/common/models/serialize/string_type.py` & `fprime-tools-3.3.0/src/fprime/common/models/serialize/string_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,17 +56,16 @@
         """
         Deserializes a string from the given data buffer.
         """
         try:
             val_size = struct.unpack_from(">H", data, offset)[0]
             # Deal with not enough data left in the buffer
             if len(data[offset + 2 :]) < val_size:
-                raise DeserializeException(
-                    f"Not enough data to deserialize string data. Needed: {val_size} Left: {len(data[offset + 2 :])}"
-                )
+                msg = f"Not enough data to deserialize string data. Needed: {val_size} Left: {len(data[offset + 2:])}"
+                raise DeserializeException(msg)
             # Deal with a string that is larger than max string
             if self.MAX_LENGTH is not None and val_size > self.MAX_LENGTH:
                 raise StringSizeException(val_size, self.MAX_LENGTH)
             self.val = data[offset + 2 : offset + 2 + val_size].decode(DATA_ENCODING)
         except struct.error:
             raise DeserializeException("Not enough bytes to deserialize string length.")
```

### Comparing `fprime-tools-3.2.1/src/fprime/common/models/serialize/time_type.py` & `fprime-tools-3.3.0/src/fprime/common/models/serialize/time_type.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 @bug No known bugs
 """
 
 import datetime
 import math
 from enum import Enum
 
+from fprime.common.models.serialize import type_base
+
 # Custom Python Modules
 from fprime.common.models.serialize.numerical_types import U8Type, U16Type, U32Type
-from fprime.common.models.serialize import type_base
 from fprime.common.models.serialize.type_exceptions import TypeRangeException
 
 TimeBase = Enum(
     "TimeBase",
     # No time base has been established
     {
         "TB_NONE": 0,
@@ -308,15 +309,14 @@
             be determined.
         """
 
         tb = TimeBase(self.__timeBase.val)
         dt = None
 
         if tb in [TimeBase["TB_WORKSTATION_TIME"], TimeBase["TB_SC_TIME"]]:
-
             # This finds the local time corresponding to the timestamp and
             # timezone object, or local time zone if tz=None
             dt = datetime.datetime.fromtimestamp(self.__secs.val, tz)
 
             dt = dt.replace(microsecond=self.__usecs.val)
 
         return dt
```

### Comparing `fprime-tools-3.2.1/src/fprime/common/models/serialize/type_base.py` & `fprime-tools-3.3.0/src/fprime/common/models/serialize/type_base.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/common/models/serialize/type_exceptions.py` & `fprime-tools-3.3.0/src/fprime/common/models/serialize/type_exceptions.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/common/utils.py` & `fprime-tools-3.3.0/src/fprime/common/utils.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/constants.py` & `fprime-tools-3.3.0/src/fprime/constants.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/pre_gen_project.py` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/pre_gen_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from fprime.util.cookiecutter_wrapper import is_valid_name
 
+
 # Check to ensure Component Name is valid
 def verify_inputs(component_name, commands, events, telemetry, parameters):
     if is_valid_name(component_name) != "valid":
         raise ValueError(
             "Unacceptable component name. Do not use spaces or special characters"
         )
     if commands == "no" and events == "no" and telemetry == "no" and parameters == "no":
```

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/CMakeLists.txt` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/docs/sdd.md` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/docs/sdd.md`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.fpp` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.fpp`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Main.cpp` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Main.cpp`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/README.md` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/README.md`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/CMakeLists.txt` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/instances.fpp` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/instances.fpp`

 * *Files 8% similar despite different names*

```diff
@@ -39,25 +39,30 @@
     priority 101
 
   instance cmdSeq: Svc.CmdSequencer base id 0x0600 \
     queue size Default.QUEUE_SIZE \
     stack size Default.STACK_SIZE \
     priority 100
 
-  instance fileDownlink: Svc.FileDownlink base id 0x0700 \
+  instance comQueue: Svc.ComQueue base id 0x0700 \
+      queue size Default.QUEUE_SIZE \
+      stack size Default.STACK_SIZE \
+      priority 100 \
+
+  instance fileDownlink: Svc.FileDownlink base id 0x0800 \
     queue size 30 \
     stack size Default.STACK_SIZE \
     priority 100
 
-  instance fileManager: Svc.FileManager base id 0x0800 \
+  instance fileManager: Svc.FileManager base id 0x0900 \
     queue size 30 \
     stack size Default.STACK_SIZE \
     priority 100
 
-  instance fileUplink: Svc.FileUplink base id 0x0900 \
+  instance fileUplink: Svc.FileUplink base id 0x0A00 \
     queue size 30 \
     stack size Default.STACK_SIZE \
     priority 100
 
   instance eventLogger: Svc.ActiveLogger base id 0x0B00 \
     queue size Default.QUEUE_SIZE \
     stack size Default.STACK_SIZE \
@@ -91,34 +96,34 @@
 
   # ----------------------------------------------------------------------
   # Passive component instances
   # ----------------------------------------------------------------------
 
   @ Communications driver. May be swapped with other comm drivers like UART
   @ Note: Here we have TCP reliable uplink and UDP (low latency) downlink
-  instance comm: Drv.ByteStreamDriverModel base id 0x4000 \
+  instance comDriver: Drv.ByteStreamDriverModel base id 0x4000 \
     type "Drv::TcpClient" \ # type specified to select implementor of ByteStreamDriverModel
     at "../../Drv/TcpClient/TcpClient.hpp" # location of above implementor must also be specified
 
-  instance downlink: Svc.Framer base id 0x4100
+  instance framer: Svc.Framer base id 0x4100
 
   instance fatalAdapter: Svc.AssertFatalAdapter base id 0x4200
 
   instance fatalHandler: Svc.FatalHandler base id 0x4300
 
-  instance fileUplinkBufferManager: Svc.BufferManager base id 0x4400
+  instance bufferManager: Svc.BufferManager base id 0x4400
 
   instance linuxTime: Svc.Time base id 0x4500 \
     type "Svc::LinuxTime" \
     at "../../Svc/LinuxTime/LinuxTime.hpp"
 
   instance rateGroupDriver: Svc.RateGroupDriver base id 0x4600
 
-  instance staticMemory: Svc.StaticMemory base id 0x4700
-
   instance textLogger: Svc.PassiveTextLogger base id 0x4800
 
-  instance uplink: Svc.Deframer base id 0x4900
+  instance deframer: Svc.Deframer base id 0x4900
 
   instance systemResources: Svc.SystemResources base id 0x4A00
 
+  instance comStub: Svc.ComStub base id 0x4B00
+
 }
```

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/topology.fpp` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/topology.fpp`

 * *Files 16% similar despite different names*

```diff
@@ -6,48 +6,44 @@
 
     enum Ports_RateGroups {
       rateGroup1
       rateGroup2
       rateGroup3
     }
 
-    enum Ports_StaticMemory {
-      downlink
-      uplink
-    }
-
   topology {{cookiecutter.deployment_name}} {
 
     # ----------------------------------------------------------------------
     # Instances used in the topology
     # ----------------------------------------------------------------------
 
     instance $health
     instance blockDrv
     instance tlmSend
     instance cmdDisp
     instance cmdSeq
-    instance comm
-    instance downlink
+    instance comDriver
+    instance comQueue
+    instance comStub
+    instance deframer
     instance eventLogger
     instance fatalAdapter
     instance fatalHandler
     instance fileDownlink
     instance fileManager
     instance fileUplink
-    instance fileUplinkBufferManager
+    instance bufferManager
+    instance framer
     instance linuxTime
     instance prmDb
     instance rateGroup1
     instance rateGroup2
     instance rateGroup3
     instance rateGroupDriver
-    instance staticMemory
     instance textLogger
-    instance uplink
     instance systemResources
 
     # ----------------------------------------------------------------------
     # Pattern graph specifiers
     # ----------------------------------------------------------------------
 
     command connections instance cmdDisp
@@ -66,23 +62,31 @@
 
     # ----------------------------------------------------------------------
     # Direct graph specifiers
     # ----------------------------------------------------------------------
 
     connections Downlink {
 
-      tlmSend.PktSend -> downlink.comIn
-      eventLogger.PktSend -> downlink.comIn
-      fileDownlink.bufferSendOut -> downlink.bufferIn
-
-      downlink.framedAllocate -> staticMemory.bufferAllocate[Ports_StaticMemory.downlink]
-      downlink.framedOut -> comm.send
-      downlink.bufferDeallocate -> fileDownlink.bufferReturn
-
-      comm.deallocate -> staticMemory.bufferDeallocate[Ports_StaticMemory.downlink]
+      eventLogger.PktSend -> comQueue.comQueueIn[0]
+      tlmSend.PktSend -> comQueue.comQueueIn[1]
+      fileDownlink.bufferSendOut -> comQueue.buffQueueIn[0]
+
+      comQueue.comQueueSend -> framer.comIn
+      comQueue.buffQueueSend -> framer.bufferIn
+
+      framer.framedAllocate -> bufferManager.bufferGetCallee
+      framer.framedOut -> comStub.comDataIn
+      framer.bufferDeallocate -> fileDownlink.bufferReturn
+
+      comDriver.deallocate -> bufferManager.bufferSendIn
+      comDriver.ready -> comStub.drvConnected
+
+      comStub.comStatus -> framer.comStatusIn
+      framer.comStatusOut -> comQueue.comStatusIn
+      comStub.drvDataOut -> comDriver.send
 
     }
 
     connections FaultProtection {
       eventLogger.FatalAnnounce -> fatalHandler.FatalReceive
     }
 
@@ -100,35 +104,37 @@
       rateGroupDriver.CycleOut[Ports_RateGroups.rateGroup2] -> rateGroup2.CycleIn
       rateGroup2.RateGroupMemberOut[0] -> cmdSeq.schedIn
 
       # Rate group 3
       rateGroupDriver.CycleOut[Ports_RateGroups.rateGroup3] -> rateGroup3.CycleIn
       rateGroup3.RateGroupMemberOut[0] -> $health.Run
       rateGroup3.RateGroupMemberOut[1] -> blockDrv.Sched
-      rateGroup3.RateGroupMemberOut[2] -> fileUplinkBufferManager.schedIn
+      rateGroup3.RateGroupMemberOut[2] -> bufferManager.schedIn
     }
 
     connections Sequencer {
       cmdSeq.comCmdOut -> cmdDisp.seqCmdBuff
       cmdDisp.seqCmdStatus -> cmdSeq.cmdResponseIn
     }
 
     connections Uplink {
 
-      comm.allocate -> staticMemory.bufferAllocate[Ports_StaticMemory.uplink]
-      comm.$recv -> uplink.framedIn
-      uplink.framedDeallocate -> staticMemory.bufferDeallocate[Ports_StaticMemory.uplink]
-
-      uplink.comOut -> cmdDisp.seqCmdBuff
-      cmdDisp.seqCmdStatus -> uplink.cmdResponseIn
-
-      uplink.bufferAllocate -> fileUplinkBufferManager.bufferGetCallee
-      uplink.bufferOut -> fileUplink.bufferSendIn
-      uplink.bufferDeallocate -> fileUplinkBufferManager.bufferSendIn
-      fileUplink.bufferSendOut -> fileUplinkBufferManager.bufferSendIn
+      comDriver.allocate -> bufferManager.bufferGetCallee
+      comDriver.$recv -> comStub.drvDataIn
+      comStub.comDataOut -> deframer.framedIn
+
+      deframer.framedDeallocate -> bufferManager.bufferSendIn
+      deframer.comOut -> cmdDisp.seqCmdBuff
+
+      cmdDisp.seqCmdStatus -> deframer.cmdResponseIn
+
+      deframer.bufferAllocate -> bufferManager.bufferGetCallee
+      deframer.bufferOut -> fileUplink.bufferSendIn
+      deframer.bufferDeallocate -> bufferManager.bufferSendIn
+      fileUplink.bufferSendOut -> bufferManager.bufferSendIn
     }
 
     connections {{cookiecutter.deployment_name}} {
       # Add here connections to user-defined components
     }
 
   }
```

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Packets.xml` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Packets.xml`

 * *Files 5% similar despite different names*

#### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Packets.xml` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Packets.xml`

```diff
@@ -8,17 +8,17 @@
     <channel name="rateGroup3.RgMaxTime"/>
     <channel name="cmdSeq.CS_LoadCommands"/>
     <channel name="cmdSeq.CS_CancelCommands"/>
     <channel name="cmdSeq.CS_CommandsExecuted"/>
     <channel name="cmdSeq.CS_SequencesCompleted"/>
     <channel name="fileUplink.FilesReceived"/>
     <channel name="fileUplink.PacketsReceived"/>
-    <channel name="fileUplinkBufferManager.TotalBuffs"/>
-    <channel name="fileUplinkBufferManager.CurrBuffs"/>
-    <channel name="fileUplinkBufferManager.HiBuffs"/>
+    <channel name="bufferManager.TotalBuffs"/>
+    <channel name="bufferManager.CurrBuffs"/>
+    <channel name="bufferManager.HiBuffs"/>
     <channel name="fileDownlink.FilesSent"/>
     <channel name="fileDownlink.PacketsSent"/>
     <channel name="fileManager.CommandsExecuted"/>
     <!-- Uncomment to use Svc::TlmPacketizer -->
     <!--channel name="tlmSend.SendLevel"/-->
   </packet>
   <packet name="CDHErrors" id="2" level="1">
@@ -26,21 +26,25 @@
     <channel name="rateGroup2.RgCycleSlips"/>
     <channel name="rateGroup3.RgCycleSlips"/>
     <channel name="cmdSeq.CS_Errors"/>
     <channel name="fileUplink.Warnings"/>
     <channel name="fileDownlink.Warnings"/>
     <channel name="health.PingLateWarnings"/>
     <channel name="fileManager.Errors"/>
-    <channel name="fileUplinkBufferManager.NoBuffs"/>
-    <channel name="fileUplinkBufferManager.EmptyBuffs"/>
+    <channel name="bufferManager.NoBuffs"/>
+    <channel name="bufferManager.EmptyBuffs"/>
     <channel name="fileManager.Errors"/>
   </packet>
   <packet name="DriveTlm" id="3" level="1">
     <channel name="blockDrv.BD_Cycles"/>
   </packet>
+  <packet name="Comms" id="4" level="1">
+    <channel name="comQueue.comQueueDepth"/>
+    <channel name="comQueue.buffQueueDepth"/>
+  </packet>
   <packet name="SystemRes1" id="5" level="2">
     <channel name="systemResources.MEMORY_TOTAL"/>
     <channel name="systemResources.MEMORY_USED"/>
     <channel name="systemResources.NON_VOLATILE_TOTAL"/>
     <channel name="systemResources.NON_VOLATILE_FREE"/>
   </packet>
   <packet name="SystemRes2" id="6" level="2">
```

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Topology.cpp` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Topology.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 Fw::MallocAllocator mallocator;
 
 // The reference topology uses the F´ packet protocol when communicating with the ground and therefore uses the F´
 // framing and deframing implementations.
 Svc::FprimeFraming framing;
 Svc::FprimeDeframing deframing;
 
+Svc::ComQueue::QueueConfigurationTable configurationTable;
+
 // The reference topology divides the incoming clock signal (1Hz) into sub-signals: 1Hz, 1/2Hz, and 1/4Hz
 NATIVE_INT_TYPE rateGroupDivisors[Svc::RateGroupDriver::DIVIDER_SIZE] = {1, 2, 4};
 
 // Rate groups may supply a context token to each of the attached children whose purpose is set by the project. The
 // reference topology sets each token to zero as these contexts are unused in this project.
 NATIVE_INT_TYPE rateGroup1Context[Svc::ActiveRateGroup::CONNECTION_COUNT_MAX] = {};
 NATIVE_INT_TYPE rateGroup2Context[Svc::ActiveRateGroup::CONNECTION_COUNT_MAX] = {};
@@ -44,17 +46,22 @@
     CMD_SEQ_BUFFER_SIZE = 5 * 1024,
     FILE_DOWNLINK_TIMEOUT = 1000,
     FILE_DOWNLINK_COOLDOWN = 1000,
     FILE_DOWNLINK_CYCLE_TIME = 1000,
     FILE_DOWNLINK_FILE_QUEUE_DEPTH = 10,
     HEALTH_WATCHDOG_CODE = 0x123,
     COMM_PRIORITY = 100,
-    UPLINK_BUFFER_MANAGER_STORE_SIZE = 3000,
-    UPLINK_BUFFER_MANAGER_QUEUE_SIZE = 30,
-    UPLINK_BUFFER_MANAGER_ID = 200
+    // bufferManager constants
+    FRAMER_BUFFER_SIZE = FW_MAX(FW_COM_BUFFER_MAX_SIZE, FW_FILE_BUFFER_MAX_SIZE + sizeof(U32)) + HASH_DIGEST_LENGTH + Svc::FpFrameHeader::SIZE,
+    FRAMER_BUFFER_COUNT = 30,
+    DEFRAMER_BUFFER_SIZE = FW_MAX(FW_COM_BUFFER_MAX_SIZE, FW_FILE_BUFFER_MAX_SIZE + sizeof(U32)),
+    DEFRAMER_BUFFER_COUNT = 30,
+    COM_DRIVER_BUFFER_SIZE = 3000,
+    COM_DRIVER_BUFFER_COUNT = 30,
+    BUFFER_MANAGER_ID = 200
 };
 
 // Ping entries are autocoded, however; this code is not properly exported. Thus, it is copied here.
 Svc::Health::PingEntry pingEntries[] = {
     {PingEntries::blockDrv::WARN, PingEntries::blockDrv::FATAL, "blockDrv"},
     {PingEntries::tlmSend::WARN, PingEntries::tlmSend::FATAL, "chanTlm"},
     {PingEntries::cmdDisp::WARN, PingEntries::cmdDisp::FATAL, "cmdDisp"},
@@ -98,24 +105,37 @@
 
     // Health is supplied a set of ping entires.
     health.setPingEntries(pingEntries, FW_NUM_ARRAY_ELEMENTS(pingEntries), HEALTH_WATCHDOG_CODE);
 
     // Buffer managers need a configured set of buckets and an allocator used to allocate memory for those buckets.
     Svc::BufferManager::BufferBins upBuffMgrBins;
     memset(&upBuffMgrBins, 0, sizeof(upBuffMgrBins));
-    upBuffMgrBins.bins[0].bufferSize = UPLINK_BUFFER_MANAGER_STORE_SIZE;
-    upBuffMgrBins.bins[0].numBuffers = UPLINK_BUFFER_MANAGER_QUEUE_SIZE;
-    fileUplinkBufferManager.setup(UPLINK_BUFFER_MANAGER_ID, 0, mallocator, upBuffMgrBins);
+    upBuffMgrBins.bins[0].bufferSize = FRAMER_BUFFER_SIZE;
+    upBuffMgrBins.bins[0].numBuffers = FRAMER_BUFFER_COUNT;
+    upBuffMgrBins.bins[1].bufferSize = DEFRAMER_BUFFER_SIZE;
+    upBuffMgrBins.bins[1].numBuffers = DEFRAMER_BUFFER_COUNT;
+    upBuffMgrBins.bins[2].bufferSize = COM_DRIVER_BUFFER_SIZE;
+    upBuffMgrBins.bins[2].numBuffers = COM_DRIVER_BUFFER_COUNT;
+    bufferManager.setup(BUFFER_MANAGER_ID, 0, mallocator, upBuffMgrBins);
 
     // Framer and Deframer components need to be passed a protocol handler
-    downlink.setup(framing);
-    uplink.setup(deframing);
+    framer.setup(framing);
+    deframer.setup(deframing);
 
     // Note: Uncomment when using Svc:TlmPacketizer
     //tlmSend.setPacketList({{cookiecutter.deployment_name}}PacketsPkts, {{cookiecutter.deployment_name}}PacketsIgnore, 1);
+
+    // Events (highest-priority)
+    configurationTable.entries[0] = {.depth = 100, .priority = 0};
+    // Telemetry
+    configurationTable.entries[1] = {.depth = 500, .priority = 2};
+    // File Downlink
+    configurationTable.entries[2] = {.depth = 100, .priority = 1};
+    // Allocation identifier is 0 as the MallocAllocator discards it
+    comQueue.configure(configurationTable, 0, mallocator);
 }
 
 // Public functions for use in main program are namespaced with deployment name {{cookiecutter.deployment_name}}
 namespace {{cookiecutter.deployment_name}} {
 void setupTopology(const TopologyState& state) {
     // Autocoded initialization. Function provided by autocoder.
     initComponents(state);
@@ -131,16 +151,16 @@
     // loadParameters();
     // Autocoded task kick-off (active components). Function provided by autocoder.
     startTasks(state);
     // Initialize socket client communication if and only if there is a valid specification
     if (state.hostname != nullptr && state.port != 0) {
         Os::TaskString name("ReceiveTask");
         // Uplink is configured for receive so a socket task is started
-        comm.configure(state.hostname, state.port);
-        comm.startSocketTask(name, true, COMM_PRIORITY, Default::STACK_SIZE);
+        comDriver.configure(state.hostname, state.port);
+        comDriver.startSocketTask(name, true, COMM_PRIORITY, Default::STACK_SIZE);
     }
 }
 
 // Variables used for cycle simulation
 Os::Mutex cycleLock;
 volatile bool cycleFlag = true;
 
@@ -168,15 +188,15 @@
 
 void teardownTopology(const TopologyState& state) {
     // Autocoded (active component) task clean-up. Functions provided by topology autocoder.
     stopTasks(state);
     freeThreads(state);
 
     // Other task clean-up.
-    comm.stopSocketTask();
-    (void)comm.joinSocketTask(nullptr);
+    comDriver.stopSocketTask();
+    (void)comDriver.joinSocketTask(nullptr);
 
     // Resource deallocation
     cmdSeq.deallocateBuffer(mallocator);
-    fileUplinkBufferManager.cleanup();
+    bufferManager.cleanup();
 }
 };  // namespace {{cookiecutter.deployment_name}}
```

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Topology.hpp` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Topology.hpp`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}TopologyDefs.hpp` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}TopologyDefs.hpp`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/hooks/post_gen_project.py` & `fprime-tools-3.3.0/src/fprime/cookiecutter_templates/cookiecutter-fprime-project/hooks/post_gen_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 - Initializes a git repository
 - Adds F' as a submodule
 - Checks out the requested branch/tag
 - Installs the virtual environment if requested
 
 @author thomas-bc
 """
-import sys
 import subprocess
+import sys
 
-DEFAULT_BRANCH = "devel"
+# Fail-safe in case user input is invalid branch/tag
+DEFAULT_BRANCH = "{{ cookiecutter.__default_branch }}"
 
 # Add F' as a submodule
 subprocess.run(["git", "init"])
 subprocess.run(
     [
         "git",
         "submodule",
```

### Comparing `fprime-tools-3.2.1/src/fprime/fbuild/builder.py` & `fprime-tools-3.3.0/src/fprime/fbuild/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,70 +3,69 @@
 build system handler underneath.
 """
 import os
 import re
 from pathlib import Path
 from typing import Iterable, List, Union
 
+# Forces targets into existence
+import fprime.fbuild.target_definitions  # lgtm[py/unused-import]
+from fprime.common.error import FprimeException
+from fprime.fbuild.cmake import CMakeException, CMakeHandler
+from fprime.fbuild.settings import IniSettings
+from fprime.fbuild.target import Target, TargetScope
 from fprime.fbuild.types import (
+    AmbiguousToolchainException,
     BuildType,
     InvalidBuildCacheException,
     MissingBuildCachePath,
     NoSuchToolchainException,
-    AmbiguousToolchainException,
-    UnableToDetectDeploymentException,
+    UnableToDetectProjectException,
 )
-from fprime.fbuild.target import TargetScope, Target
-from fprime.common.error import FprimeException
-from fprime.fbuild.settings import IniSettings
-from fprime.fbuild.cmake import CMakeHandler, CMakeException
-
-# Forces targets into existence
-import fprime.fbuild.target_definitions  # lgtm[py/unused-import]
 
 
 class Build:
     """Represents a build configuration
 
-    Builds in F´ consist of a build type (normal, testing), a deployment directory, a set of settings, and a target
+    Builds in F´ consist of a build type (normal, testing), a cmake project directory, a set of settings, and a target
     platform. These are tracked as part of this Build class. This helps setup a build cache directory, load default
     settings, and track what type of build is being run.
 
     BuildType represents the type of build as explained in that enum type.
-    Deployments are an individual build of fprime, and should define the CMakeLists.txt file as a child of this
+    Projects are an individual build of fprime, and should define the CMakeLists.txt file as a child of this
     directory. A default settings.ini file may be found here.
     Platforms represent the target hardware to build from. This is translated to the CMake toolchain file.
 
     After creation, a user must use invent to handle new builds (e.g. during the generation step), or load to load a
     previously generated build.
 
     Examples:
         To use in generation run the following code.
 
-        build = Build(BuildType.BUILD_NORMAL, path/to/deployment)
+        build = Build(BuildType.BUILD_NORMAL, path/to/project)
         build.invent("raspberrypi")
 
         To use at any step after generation:
 
-        build = Build(BuildType.BUILD_NORMAL, path/to/deployment)
+        build = Build(BuildType.BUILD_NORMAL, path/to/project)
         build.load()
     """
 
     VALID_CMAKE_LIST = re.compile(r"^\s*project\(.*\)", re.MULTILINE)
     CMAKE_DEFAULT_BUILD_NAME = "build-fprime-automatic-{platform}{suffix}"
 
-    def __init__(self, build_type: BuildType, deployment: Path, verbose: bool = False):
+    def __init__(self, build_type: BuildType, project: Path, verbose: bool = False):
         """Constructs a build object from its constituent parts
 
         Args:
             build_type: member of the enum BuildType specifying fprime build type
-            deployment: path to deployment that this build represents
+            project: path to cmake project that this build represents
         """
         self.build_type = build_type
-        self.deployment = deployment
+        self.cmake_root = project
         self.settings = None
         self.platform = None
         self.build_dir = None
         self.cmake = CMakeHandler()
         self.cmake.set_verbose(verbose)
 
     def invent(self, platform: str = None, build_dir: Path = None):
@@ -86,15 +85,16 @@
             build_dir:  explicitly sets the build path to allow for user override of default
 
         Raises:
             InvalidBuildCacheException: a build cache already exists as it should not
         """
         self.__setup_default(platform, build_dir)
         if self.build_dir.exists():
-            raise InvalidBuildCacheException(f"{self.build_dir} already exists.")
+            msg = f"{self.build_dir} already exists."
+            raise InvalidBuildCacheException(msg)
 
     def load(self, platform: str = None, build_dir: Path = None, skip_validation=False):
         """Load an existing build cache
 
         Sets this build up from an existing build cache. This can be used after a previous run that has generated a
         build cache in order to prepare for other build steps.
 
@@ -120,16 +120,17 @@
                 gen_args += (
                     " " + platform
                     if platform is not None
                     and platform != "native"
                     and platform != "default"
                     else ""
                 )
+            msg = f"'{self.build_dir}' is not a valid build cache. Generate this build cache with 'fprime-util generate{gen_args} ...'"
             raise InvalidBuildCacheException(
-                f"'{self.build_dir}' is not a valid build cache. Generate this build cache with 'fprime-util generate{gen_args} ...'",
+                msg,
                 self.build_dir,
             )
 
     def get_settings(
         self,
         setting: Union[None, str, Iterable[Union[None, str]]],
         default: Union[None, str, Iterable[Union[None, str]]],
@@ -161,16 +162,17 @@
             hash_value: hash number to lookup
 
         Returns:
             stored file path(s) associated with hash
         """
         hashes_file = self.build_dir / "hashes.txt"
         if not hashes_file.exists():
+            msg = f"Failed to find {hashes_file}, was the build generated?"
             raise InvalidBuildCacheException(
-                f"Failed to find {hashes_file}, was the build generated?",
+                msg,
                 self.build_dir,
             )
         with open(hashes_file) as file_handle:
             lines = filter(
                 lambda line: hash_value == int(line.split(" ")[-1], 0),
                 file_handle.readlines(),
             )
@@ -183,15 +185,15 @@
         specified as false. A valid build cache has been created from the generate step, and thus when using this call
         as part of the generate step, validate should be set to false.
 
         Returns:
             Path to a build cache directory
 
         """
-        return self.deployment / Build.CMAKE_DEFAULT_BUILD_NAME.format(
+        return self.cmake_root / Build.CMAKE_DEFAULT_BUILD_NAME.format(
             platform=self.platform, suffix=self.build_type.get_suffix()
         )
 
     def get_build_info(self, context: Path) -> dict:
         """Constructs an informational packet about this build
 
         Constructs a packet that allows for users to get meta-build information. This includes: location of build, file
@@ -226,22 +228,22 @@
         return {
             "local_targets": local_targets,
             "global_targets": global_targets,
             "auto_location": auto_location,
             "build_dir": self.build_dir,
         }
 
-    def is_deployment(self, context: Path) -> bool:
-        """Check if given path represents a deployment
+    def is_project_root(self, context: Path) -> bool:
+        """Check if given path represents a project root
 
         Args:
             context: contextual path to list various information about the build
 
         Returns:
-            True if the context is a deployment, false otherwise
+            True if the context is a project, false otherwise
         """
         try:
             self.cmake.cmake_validate_source_dir(context)
             return True
         except CMakeException:
             return False
 
@@ -254,15 +256,15 @@
         Returns:
             path to CMake toolchain file or None to use builtin
         """
         assert (
             self.platform != "default"
         ), "Default toolchain should have been decided already"
         toolchain_locations = self.get_settings(
-            ["framework_path", "project_root"], [None, self.deployment]
+            ["framework_path", "project_root"], [None, self.cmake_root]
         )
         toolchain_locations += self.get_settings("library_locations", [])
 
         # If toolchain is the native target, this is supplied by CMake and we exit here.
         if self.platform == "native":
             return None
         # Otherwise, find locations of toolchain files using the specified locations from settings.
@@ -276,25 +278,23 @@
             {
                 toolchain_path
                 for toolchain_path in toolchains_paths
                 if os.path.exists(toolchain_path)
             }
         )
         if not toolchains:
-            raise NoSuchToolchainException(
-                f'Could not find toolchain file for {self.platform} at any of: {" ".join(toolchains_paths)}'
-            )
+            msg = f"Could not find toolchain file for {self.platform} at any of: {' '.join(toolchains_paths)}"
+            raise NoSuchToolchainException(msg)
         if len(toolchains) > 1:
-            raise AmbiguousToolchainException(
-                f'Found conflicting toolchain files for {self.platform} at: {" ".join(toolchains)}'
-            )
+            msg = f"Found conflicting toolchain files for {self.platform} at: {' '.join(toolchains)}"
+            raise AmbiguousToolchainException(msg)
         return toolchains[0]
 
     def get_cmake_args(self) -> dict:
-        """Generates CMake arguments from deployment settings (settings.ini file)
+        """Generates CMake arguments from project settings (settings.ini file)
 
         Returns:
             A dictionary of cmake settings
         """
         needed = [
             ("FPRIME_FRAMEWORK_PATH", "framework_path"),
             ("FPRIME_LIBRARY_LOCATIONS", "library_locations"),
@@ -346,15 +346,16 @@
             context: contextual path to return
         """
         project_relative_path = self.get_relative_path(context)
         for possible in [".", "F-Prime"]:
             possible_path = self.build_dir / possible / project_relative_path
             if possible_path.exists():
                 return possible_path
-        raise MissingBuildCachePath(f"{context} has no associated build cache path")
+        msg = f"{context} has no associated build cache path"
+        raise MissingBuildCachePath(msg)
 
     def get_relative_path(self, path: Path) -> Path:
         """Gets path relative to project"""
         relative_path, _ = self.cmake.get_include_info(path, self.build_dir)
         return Path(relative_path)
 
     def execute_build_target(
@@ -401,15 +402,15 @@
             default_cmake_args = {
                 option: value
                 for (option, value) in [split_pair(item) for item in default_options]
                 if option != ""
             }
 
             self.cmake.generate_build(
-                self.deployment,
+                self.cmake_root,
                 self.build_dir,
                 {**default_cmake_args, **cmake_args, **self.get_cmake_args()},
                 environment=self.settings.get("environment", None),
             )
         except CMakeException as cexc:
             raise GenerateException(str(cexc), cexc.exit_code) from cexc
 
@@ -429,41 +430,41 @@
         assert (
             "install_destination" in self.settings
         ), "install_destination not present in settings"
         path = Path(self.settings["install_destination"])
         return path if path.exists() else None
 
     @staticmethod
-    def find_nearest_deployment(path: Path) -> Path:
-        """Recurse up the directory stack looking for a valid deployment
+    def find_nearest_parent_project(path: Path) -> Path:
+        """Recurse up the directory stack looking for a valid CMake project.
 
-        Recurse up the directory tree from the given path, looking for a deployment definition directory. This means it
+        Recurse up the directory tree from the given path, looking for a project definition directory. This means it
         defines a CMakeLists.txt with a project call. This finds where the automatic build directories are allowed to
         exist.
 
         Notes:
-            This replaced the former build directory recursive detector as that can "slip" past a deployment should the
-            build directory not be generated yet.
+            Historically, the root of the CMake project was an F' deployment. In F' > v3.2.0, this is more often an
+            F' project root.
 
         Returns;
-            Path to the nearest deployment directory searching up the directory tree
+            Path to the nearest project directory searching up the directory tree
 
         Raises;
-            UnableToDetectDeploymentException: was unable to detect a deployment directory
+            UnableToDetectProjectException: was unable to detect a project directory
         """
         full_path = path.resolve()
         list_file = full_path / "CMakeLists.txt"
         if not full_path.parents:
-            raise UnableToDetectDeploymentException()
+            raise UnableToDetectProjectException()
         if list_file.exists():
             with open(list_file, encoding="utf8") as file_handle:
                 text = file_handle.read()
             if Build.VALID_CMAKE_LIST.search(text):
                 return full_path
-        return Build.find_nearest_deployment(full_path.parent)
+        return Build.find_nearest_parent_project(full_path.parent)
 
     @staticmethod
     def get_build_list(base, build_cache=None, ignore_invalid=False):
         """Returns a list of builds that the tool will process
 
         Will return a list of builds the tool will process. This will be a build for each public build type unless the
         cache has been overridden.  If overridden, this will be one build pointed at that cache.
@@ -479,15 +480,15 @@
         build_types = (
             [BuildType.BUILD_CUSTOM]
             if build_cache is not None
             else BuildType.get_public_types()
         )
         builds = []
         for build_type in build_types:
-            build = Build(build_type, base.deployment, verbose=base.cmake.verbose)
+            build = Build(build_type, base.cmake_root, verbose=base.cmake.verbose)
             try:
                 build.load(
                     base.platform, build_dir=build_cache, skip_validation=ignore_invalid
                 )
                 builds.append(build)
             except InvalidBuildCacheException as error:
                 # Warnings only issued when not using an explicit build cache
@@ -513,15 +514,15 @@
             build_dir:  explicitly sets the build path to allow for user override of default
         """
         assert self.settings is None, "Already setup it is invalid to re-setup"
         assert self.platform is None, "Already setup it is invalid to re-setup"
         assert self.build_dir is None, "Already setup it is invalid to re-setup"
 
         self.settings = IniSettings.load(
-            self.deployment / "settings.ini",
+            self.cmake_root / "settings.ini",
             platform,
             self.build_type == BuildType.BUILD_TESTING,
         )
 
         if platform is not None and platform != "default":
             self.platform = platform
         elif self.build_type == BuildType.BUILD_TESTING:
```

### Comparing `fprime-tools-3.2.1/src/fprime/fbuild/cli.py` & `fprime-tools-3.3.0/src/fprime/fbuild/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 Command line processing functions for fbuild (fprime build system targets) of "generate", "purge", and build system
 target operations.
 
 @author mstarch
 """
 import argparse
 from pathlib import Path
-from typing import Dict, List, Tuple, Callable
-from fprime.fbuild.types import BuildType
-from fprime.fbuild.target import Target
-from fprime.fbuild.builder import Build
+from typing import Callable, Dict, List, Tuple
+
 from fprime.common.utils import confirm
+from fprime.fbuild.builder import Build
+from fprime.fbuild.target import Target
+from fprime.fbuild.types import BuildType
 
 
 def get_target(parsed: argparse.Namespace) -> Target:
     """Gets the target given the argparse namespace
 
     Takes the parsed namespace and processes it to a known matching target.
 
@@ -189,18 +190,18 @@
     Returns:
         ["generate", "purge"] list of special targets
     """
 
     generate_parser = subparsers.add_parser(
         "generate",
         help=help_text.short(
-            "generate", "Generate a build cache for specified deployment"
+            "generate", "Generate a build cache for specified project"
         ),
         description=help_text.long(
-            "generate", "Generate a build cache for specified deployment"
+            "generate", "Generate a build cache for specified project"
         ),
         parents=[common],
         add_help=False,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     generate_parser.add_argument(
         "--disable-sanitizers",
@@ -213,17 +214,17 @@
         action="append",
         help="Pass -D flags through to CMakes",
         nargs=1,
         default=[],
     )
     purge_parser = subparsers.add_parser(
         "purge",
-        help=help_text.short("purge", "Remove build caches for specified deployment"),
+        help=help_text.short("purge", "Remove build caches for specified project"),
         description=help_text.long(
-            "purge", "Remove build caches for specified deployment"
+            "purge", "Remove build caches for specified project"
         ),
         add_help=False,
         parents=[common],
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     purge_parser.add_argument(
         "-f",
```

### Comparing `fprime-tools-3.2.1/src/fprime/fbuild/cmake.py` & `fprime-tools-3.3.0/src/fprime/fbuild/cmake.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,16 +505,17 @@
         os.close(pty_err_w)
         ret, stdout, stderr = self._communicate(
             proc, open(pty_out_r, mode="rb"), open(pty_err_r, mode="rb"), print_output
         )
         # Raising an exception when the return code is non-zero allows us to handle the exception internally if it is
         # needed. Thus we do not just exit.
         if ret != 0:
+            msg = f"CMake erred with return code {proc.returncode}"
             raise CMakeExecutionException(
-                f"CMake erred with return code {proc.returncode}",
+                msg,
                 stderr,
                 print_output,
                 ret,
             )
         return stdout, stderr
 
     @staticmethod
```

### Comparing `fprime-tools-3.2.1/src/fprime/fbuild/gcovr.py` & `fprime-tools-3.3.0/src/fprime/fbuild/gcovr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """ fprime.fbuild.gcovr: coverage target implementations """
-import atexit
 import itertools
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 from typing import Dict, List, Tuple, Union
 
-from .target import ExecutableAction, Target, TargetScope, CompositeTarget
+from .target import CompositeTarget, ExecutableAction, Target, TargetScope
 
 
 def _get_project_path(builder: "Build", module: Union[str, Path]) -> Path:
     """Get the project path from a given module string
 
     Get the project path for a given module or path. Paths are assumed to be contexts and returned verbatim. Modules are
     converted to a project string and then that is returned.
@@ -28,15 +27,15 @@
         "project_root", builder.get_settings("framework_path", builder.build_dir.parent)
     )
     return Path(project_root) / module.replace("_", "/")
 
 
 def _using_root(builder: "Build", context: Path, scope: TargetScope):
     """Are we using repository root for things"""
-    return builder.is_deployment(context) or scope == TargetScope.GLOBAL
+    return builder.is_project_root(context) or scope == TargetScope.GLOBAL
 
 
 class GcovClean(ExecutableAction):
     """Target used to scrub gcov files before a coverage run
 
     The way fprime builds unittests means it is easy to see gcov coverage files leak into the coverage report from other
     runs. This target finds all gcov created files (.gcda) and removes them before the build. This applies to the
@@ -102,32 +101,50 @@
                 f"[ERROR] Cannot find executable: {self.EXECUTABLE}. Unable to run coverage report.",
                 file=sys.stderr,
             )
             return
         build_cache_resolved = Path(builder.build_dir).resolve()
 
         _, pass_through_args, options = args
-        include_all_ac = options["--all-ac"]
-        include_comp_ac = include_all_ac or options["--comp-ac"]
-        include_port_ac = include_all_ac or options["--port-ac"]
-        include_type_ac = include_all_ac or options["--type-ac"]
-
-        exclusion_filter_bases = [
+        include_all = options["--all-sources"]
+        include_comp_ac = include_all or options["--comp-ac"]
+        include_port_ac = include_all or options["--port-ac"]
+        include_type_ac = include_all or options["--type-ac"]
+        include_test_ac = include_all or options["--test-ac"]
+        include_test = include_all or options["--test-sources"]
+        build_cache_exclusion_filter_bases = [
             None if include_comp_ac else ".*ComponentAc.[ch]pp",
             None if include_port_ac else ".*PortAc.[ch]pp",
             None if include_type_ac else ".*SerializableAc.[ch]pp",
             None if include_type_ac else ".*ArrayAc.[ch]pp",
             None if include_type_ac else ".*EnumAc.[ch]pp",
+            None if include_test_ac else ".*/GTestBase.[ch]pp",
+            None if include_test_ac else ".*/TesterBase.[ch]pp",
+            None if include_test_ac else ".*/TesterHelpers.[ch]pp",
+        ]
+        raw_source_exclusion_filter_bases = [
+            None if include_test else ".*/test/ut/.*",
+            None if include_test else ".*/GTest/.*",
+            None if include_test else "test/ut/.*",
         ]
-        exclusion_filter_bases = filter(
-            lambda item: item is not None, exclusion_filter_bases
+
+        build_cache_exclusion_filter_bases = filter(
+            lambda item: item is not None, build_cache_exclusion_filter_bases
+        )
+
+        raw_source_exclusion_filter_bases = filter(
+            lambda item: item is not None, raw_source_exclusion_filter_bases
         )
+
         exclusion_filter_bases = [
             ["--exclude", f"{build_cache_resolved}/{exclusion}"]
-            for exclusion in exclusion_filter_bases
+            for exclusion in build_cache_exclusion_filter_bases
+        ] + [
+            ["--exclude", f"{exclusion}"]
+            for exclusion in raw_source_exclusion_filter_bases
         ]
 
         build_cache_path = (
             builder.build_dir
             if _using_root(builder, context, self.scope)
             else builder.get_build_cache_path(context)
         ).resolve()
@@ -139,63 +156,61 @@
             builder.get_settings("framework_path", builder.build_dir.parent.parent),
         ).resolve()
         filter_path = (
             Path(project_root).resolve()
             if _using_root(builder, context, self.scope)
             else _get_project_path(builder, context)
         ).resolve()
-        exclude_autocoders = (
-            builder.get_settings("framework_path", builder.build_dir.parent.parent)
-            / "Autocoders"
-        )
-        exclude_gtest = (
-            builder.get_settings("framework_path", builder.build_dir.parent.parent)
-            / "gtest"
+        framework_path = builder.get_settings(
+            "framework_path", builder.build_dir.parent.parent
         )
-
         # gcovr is an unhappy beast
         cli_args = (
             [
                 "gcovr",
                 "-r",
                 str(project_root),
                 str(build_cache_path),  # For efficiency in searching on modules
             ]
             + list(itertools.chain.from_iterable(exclusion_filter_bases))
             + [
                 "--exclude",
-                f"{exclude_autocoders}",
+                f"{framework_path}/Autocoders",
+                "--exclude",
+                f"{framework_path}/gtest",
                 "--exclude",
-                f"{exclude_gtest}",
+                f"{framework_path}/STest",
                 "--filter",
                 f"{filter_path}",
                 "--filter",
                 f"{build_cache_path}",
                 "--print-summary",
                 "--txt",
                 f"{coverage_output_dir}/summary.txt",
                 "--html-details",
                 f"{coverage_output_dir}/coverage{'-all' if self.scope == TargetScope.GLOBAL else ''}.html",
             ]
         )
         cli_args.extend(pass_through_args)
 
         if builder.cmake.verbose:
-            joined_args = " ".join(cli_args)
-            print(f'[INFO] Running "{ joined_args }"')
+            joined_args = "' '".join(cli_args)
+            print(f"[INFO] Running \"'{ joined_args }'\"")
         # gcovr must run in the ac_temporary_path or html details cannot find the Ac files
         subprocess.call(cli_args)
 
     def option_args(self):
         """Option arguments"""
         return [
-            ("--all-ac", "[coverage only] Include all autocode in coverage"),
+            ("--all-sources", "[coverage only] Include all sources in coverage"),
             ("--comp-ac", "[coverage only] Include component autocode in coverage"),
             ("--port-ac", "[coverage only] Include port autocode in coverage"),
             ("--type-ac", "[coverage only] Include data type autocode in coverage"),
+            ("--test-ac", "[coverage only] Include data test autocode in coverage"),
+            ("--test-sources", "[coverage only] Include unit test sources in coverage"),
         ]
 
     def allows_pass_args(self):
         """Gcovr allows pass-through arguments"""
         return True
 
     def pass_handler(self):
```

### Comparing `fprime-tools-3.2.1/src/fprime/fbuild/settings.py` & `fprime-tools-3.3.0/src/fprime/fbuild/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
 fprime.fbuild.settings:
 
-An implementation used to pull settings into the fprime build.  This version uses INI files in order to load the
-settings from the settings.default file that is part of the F prime deployment directory.
+An implementation used to pull settings into the fprime build. This version uses INI files in order
+to load the settings from the settings.default file that is part of the F prime project directory.
 
 @author mstarch
 """
-import os
 import configparser
-from functools import partial
+import os
 from enum import Enum
-from typing import Dict, List, Union, Callable, Any
+from functools import partial
 from pathlib import Path
+from typing import Any, Callable, Dict, List, Union
 
 
 class SettingType(Enum):
     """Designates the type of the setting"""
 
     PATH = 0
     PATH_LIST = 1
     STRING = 2
 
 
 def find_fprime(settings: dict) -> Path:
     """
     Finds F prime by recursing parent to parent until a matching directory is found.
     """
-    needle = Path("cmake/FPrime.cmake")
-    path = settings["_deployment"]
+    needle = Path("fprime/cmake/FPrime.cmake")
+    path = settings["_cmake_project_root"]
     while path != path.parent:
         if (path / needle).is_file():
-            return path
+            return path / "fprime"
         path = path.parent
     raise FprimeLocationUnknownException(
         "Please set 'framework_path' in [fprime] section in 'settings.ini"
     )
 
 
 def join(key: Path, addition: str, settings: dict):
@@ -51,14 +51,15 @@
     FPRIME_FIELDS = [
         ("framework_path", SettingType.PATH, find_fprime),
         ("project_root", SettingType.PATH, lambda settings: settings["framework_path"]),
         ("default_toolchain", SettingType.STRING, "native"),
         ("default_ut_toolchain", SettingType.STRING, "native"),
         ("library_locations", SettingType.PATH_LIST, []),
         ("component_cookiecutter", SettingType.STRING, "default"),
+        ("deployment_cookiecutter", SettingType.STRING, "default"),
     ]
 
     PLATFORM_FIELDS = [
         (
             "config_directory",
             SettingType.PATH,
             partial(join, "framework_path", "config"),
@@ -67,15 +68,15 @@
             "ac_constants",
             SettingType.PATH,
             partial(join, "config_directory", "AcConstants.ini"),
         ),
         (
             "install_destination",
             SettingType.PATH,
-            partial(join, "_deployment", "build-artifacts"),
+            partial(join, "_cmake_project_root", "build-artifacts"),
         ),
         (
             "environment_file",
             SettingType.PATH,
             lambda settings: settings["settings_file"],
         ),
         ("default_cmake_options", SettingType.STRING, ""),
@@ -104,17 +105,16 @@
         all_paths = parser.get(section, key, fallback="").split(":")
         expanded = []
         for path in all_paths:
             if not path:
                 continue
             full_path = os.path.abspath(os.path.normpath(os.path.join(base_dir, path)))
             if exists and not os.path.exists(full_path):
-                raise FprimeSettingsException(
-                    f"Nonexistent path '{path}' found in section '{section}' option '{key}' of file '{ini_file}'"
-                )
+                msg = f"Nonexistent path '{path}' found in section '{section}' option '{key}' of file '{ini_file}'"
+                raise FprimeSettingsException(msg)
             expanded.append(Path(full_path).resolve())
         return expanded
 
     @staticmethod
     def read_setting(
         config_parser: configparser.ConfigParser,
         settings: Dict[str, Any],
@@ -175,15 +175,18 @@
         confparse = None
         if settings_file.exists():
             confparse = configparser.ConfigParser()
             confparse.read(settings_file)
         else:
             print(f"[WARNING] {settings_file} does not exist")
 
-        settings = {"settings_file": settings_file, "_deployment": settings_file.parent}
+        settings = {
+            "settings_file": settings_file,
+            "_cmake_project_root": settings_file.parent,
+        }
 
         # Read fprime and platform settings from the "fprime" section
         for key, settings_type, default in (
             IniSettings.FPRIME_FIELDS + IniSettings.PLATFORM_FIELDS
         ):
             settings[key] = IniSettings.read_setting(
                 confparse, settings, "fprime", key, settings_type, default
@@ -207,15 +210,15 @@
                 settings_type,
                 settings.get(key, default),
             )
 
         settings["environment"] = IniSettings.load_environment(
             settings["environment_file"]
         )
-        del settings["_deployment"]
+        del settings["_cmake_project_root"]
         return settings
 
     @staticmethod
     def load_environment(env_file):
         """
         Load the environment from the given parser.
```

### Comparing `fprime-tools-3.2.1/src/fprime/fbuild/target.py` & `fprime-tools-3.3.0/src/fprime/fbuild/target.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 """
 import functools
 import itertools
 from abc import ABC, abstractmethod
 from enum import Enum
 from pathlib import Path
 from typing import Dict, List, Set, Tuple
+
 from .types import BuildType, NoSuchTargetException
 
 
 class TargetScope(Enum):
     """Scoping for target execution: GLOBAL, LOCAL
 
     GLOBAL targets trigger top-level (global) build system targets. LOCAL targets trigger per-directory build system
@@ -211,17 +212,16 @@
         """
         matching = [
             target
             for target in cls.get_all_targets()
             if target.mnemonic == mnemonic and flags == target.flags
         ]
         if not matching:
-            raise NoSuchTargetException(
-                f"Could not find target '{cls.config_string(mnemonic, flags)}'"
-            )
+            msg = f"Could not find target '{cls.config_string(mnemonic, flags)}'"
+            raise NoSuchTargetException(msg)
         assert len(matching) == 1, "Conflicting targets specified in code"
         return matching[0]
 
 
 class CompositeTarget(Target):
     """Target whose execution is a composition of other targets"""
```

### Comparing `fprime-tools-3.2.1/src/fprime/fbuild/target_definitions.py` & `fprime-tools-3.3.0/src/fprime/fbuild/target_definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ fprime.fbuild.target_definitions: targets definitions for fprime-util
 
 Defines all the targets for fprime-util. Each target is a singleton that is registered into the list of all targets and
 as such, each target need only be instantiated but need not be assigned to anything.
 
 """
-from .types import BuildType
-from .target import TargetScope, BuildSystemTarget
 from .gcovr import GcovrTarget
+from .target import BuildSystemTarget, TargetScope
+from .types import BuildType
 
 #### "build" targets for components, deployments, unittests for both normal and testing builds ####
 BuildSystemTarget(
     "",
     mnemonic="build",
     desc="Build components, ports, and deployments",
     scope=TargetScope.BOTH,
```

### Comparing `fprime-tools-3.2.1/src/fprime/fbuild/types.py` & `fprime-tools-3.3.0/src/fprime/fbuild/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """An exception indicating a build cache"""
 
     def __init__(self, message, build_cache=""):
         super().__init__(message)
         self.cache = build_cache
 
 
-class UnableToDetectDeploymentException(FprimeException):
+class UnableToDetectProjectException(FprimeException):
     """An exception indicating a build cache"""
 
 
 class NoSuchTargetException(FprimeException):
     """Could not find a matching build target"""
 
 
@@ -53,25 +53,27 @@
 
     def get_suffix(self):
         """Get the suffix of a directory supporting this build"""
         if self == BuildType.BUILD_NORMAL:
             return ""
         if self == BuildType.BUILD_TESTING:
             return "-ut"
-        raise InvalidBuildTypeException(f"{self.name} is not a supported build type")
+        msg = f"{self.name} is not a supported build type"
+        raise InvalidBuildTypeException(msg)
 
     def get_cmake_build_type(self):
         """Get the suffix of a directory supporting this build"""
         if self == BuildType.BUILD_NORMAL:
             return "Release"
         if self == BuildType.BUILD_TESTING:
             return "Testing"
         if self == BuildType.BUILD_FPP_LOCS:
             return "Release"
         if self == BuildType.BUILD_CUSTOM:
             return "Custom"
-        raise InvalidBuildTypeException(f"{self.name} is not a supported build type")
+        msg = f"{self.name} is not a supported build type"
+        raise InvalidBuildTypeException(msg)
 
     @staticmethod
     def get_public_types() -> List["BuildType"]:
         """Returns public build types"""
         return [BuildType.BUILD_NORMAL, BuildType.BUILD_TESTING]
```

### Comparing `fprime-tools-3.2.1/src/fprime/fpp/cli.py` & `fprime-tools-3.3.0/src/fprime/fpp/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ fprime.fpp.cli: FPP command line targets
 
 Processing and command line functions for FPP tools wrappers in fprime-util.
 
 @mstarch
 """
 import argparse
-from typing import Dict, List, Tuple, Callable
+from typing import Callable, Dict, List, Tuple
+
 from fprime.fpp.common import FppUtility
 
 
 def run_fpp_check(
     build: "Build",
     parsed: argparse.Namespace,
     _: Dict[str, str],
@@ -30,14 +31,37 @@
     FppUtility("fpp-check").execute(
         build,
         parsed.path,
         args=({}, ["-u", parsed.unconnected] if parsed.unconnected else []),
     )
 
 
+def run_fpp_to_xml(
+    build: "Build",
+    parsed: argparse.Namespace,
+    _: Dict[str, str],
+    __: Dict[str, str],
+    ___: List[str],
+):
+    """Run the fpp-to-xml utility
+
+    Args:
+        build: build directory output
+        parsed: parsed input arguments
+        _: unused cmake_args
+        __: unused make_args
+        ___: unused pass-through arguments
+    """
+    FppUtility("fpp-to-xml").execute(
+        build,
+        parsed.path,
+        args=({}, ["--directory", parsed.directory] if parsed.directory else []),
+    )
+
+
 def add_fpp_parsers(
     subparsers, common: argparse.ArgumentParser
 ) -> Tuple[Dict[str, Callable], Dict[str, argparse.ArgumentParser]]:
     """Sets up the fpp command line parsers
 
     Creates command line parsers for fpp commands and associates these commands to processing functions for those fpp
     commands.
@@ -51,8 +75,15 @@
     """
     check_parser = subparsers.add_parser(
         "fpp-check", help="Runs fpp-check utility", parents=[common], add_help=False
     )
     check_parser.add_argument(
         "-u", "--unconnected", default=None, help="write unconnected ports to file"
     )
-    return {"fpp-check": run_fpp_check}, {"fpp-check": check_parser}
+    fpp_to_xml_parser = subparsers.add_parser(
+        "fpp-to-xml", help="Runs fpp-to-xml utility", parents=[common], add_help=False
+    )
+    fpp_to_xml_parser.add_argument("--directory", default=None, help="Output directory")
+    return {"fpp-check": run_fpp_check, "fpp-to-xml": run_fpp_to_xml}, {
+        "fpp-check": check_parser,
+        "fpp-to-xml": fpp_to_xml_parser,
+    }
```

### Comparing `fprime-tools-3.2.1/src/fprime/fpp/common.py` & `fprime-tools-3.3.0/src/fprime/fpp/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 Common implementations for FPP tool wrapping.
 
 @author mstarch
 """
 import itertools
 import subprocess
-from typing import List, Dict, Tuple
 from pathlib import Path
+import shutil
+import sys
+from typing import Dict, List, Tuple
 
 from fprime.common.error import FprimeException
 from fprime.fbuild.builder import Build
 from fprime.fbuild.target import ExecutableAction, TargetScope
 
 
 class FppMissingSupportFiles(FprimeException):
     """FPP is missing its support files and cannot run"""
 
     def __init__(self, file):
         super().__init__(
-            f"Current directory does not define any FPP files. Did you intend to run in the topology directory?"
+            "Current directory does not define any FPP files. Did you intend to run in the topology directory?"
         )
 
 
 class FppUtility(ExecutableAction):
     """Action built around executing FPP
 
     When executing FPP, the utilities often require a set of input or dependency FPP files as well as a locations file
@@ -39,14 +41,18 @@
 
         Args:
             name: name of the fpp utility to run
         """
         super().__init__(TargetScope.LOCAL)
         self.utility = name
 
+    def is_supported(self, _=None, __=None):
+        """Returns whether this utility is supported"""
+        return bool(shutil.which(self.utility))
+
     @staticmethod
     def get_locations_file(builder: Build) -> Path:
         """Returns the location of the FPP locations file
 
         Returns a path to the FPP locations index within the build cache managed by the supplied build object.
 
         Args:
@@ -94,14 +100,22 @@
 
         Args:
             builder: build object to run the utility with
             context: context path of module FPP is running on
             args: extra arguments to supply to the utility
         """
         # First refresh the cache but only if it detects it needs too
+
+        if not self.is_supported():
+            print(
+                f"[ERROR] Cannot find executable: {self.utility}.",
+                file=sys.stderr,
+            )
+            return 1
+
         builder.cmake.cmake_refresh_cache(builder.build_dir, False)
 
         # Read files and arguments
         locations = self.get_locations_file(builder)
         inputs = self.get_fpp_inputs(builder, context)
 
         if not inputs:
```

### Comparing `fprime-tools-3.2.1/src/fprime/util/build_helper.py` & `fprime-tools-3.3.0/src/fprime/util/build_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,18 +11,19 @@
  - build_ut: build the current UTs
  - check: run modules unit tests
 
 @author mstarch
 """
 from pathlib import Path
 
-from fprime.fbuild.target import NoSuchTargetException
 from fprime.fbuild.builder import Build, BuildType
-from .versioning import get_version, VersionException
 from fprime.fbuild.cli import get_target
+from fprime.fbuild.target import NoSuchTargetException
+
+from .versioning import VersionException, get_version
 
 # Attempt to get pkg_resources from "setuptools"
 try:
     import pkg_resources
 except ImportError:
     pkg_resources = None
 
@@ -75,49 +76,44 @@
                 break
             except (OSError, VersionException) as exc:
                 message = f"[WARNING] {exc}"
         else:
             print(message)
 
 
-def load_build(parsed):
+def load_build(parsed, skip_validation=False):
     """
     Loads Build object and returns it to the caller. Additionally, this will validate the
     installed tool versions (such as fpp and other F' utilities) against the requirements.txt
     """
 
     try:
         target = get_target(parsed)
         build_type = target.build_type
     except NoSuchTargetException:
         build_type = BuildType.BUILD_TESTING if parsed.ut else BuildType.BUILD_NORMAL
 
-    deployment = (
-        Path(parsed.deploy)
-        if parsed.deploy is not None
-        else Build.find_nearest_deployment(Path.cwd())  # Deployments look in CWD
+    cmake_root = (
+        Path(parsed.root)
+        if parsed.root is not None
+        else Build.find_nearest_parent_project(Path.cwd())
     )
 
-    build = Build(build_type, deployment, verbose=parsed.verbose)
+    build = Build(build_type, cmake_root, verbose=parsed.verbose)
 
     # All commands need to load the build cache to setup the basic information for the build with the exception of
     # generate, which is run before the creation of the build cache and thus must invent the cache instead. This
     # call will ensure the build is in a ready state before attempting to check tool versions and run the command.
     #
     # Some commands, like purge and info, run on sets of directories and will attempt to load those sets later.
     # However, the base directory must be setup here. Errors in this load are ignored to allow the command to find
     # build caches related to that set.
     if parsed.command == "generate":
         build.invent(parsed.platform, build_dir=parsed.build_cache)
     else:
-        does_not_need_cache_directory = parsed.command in [
-            "purge",
-            "info",
-            "format",
-        ]
         build.load(
             parsed.platform,
             parsed.build_cache,
-            skip_validation=does_not_need_cache_directory,
+            skip_validation=skip_validation,
         )
     validate_tools_from_requirements(build)
     return build
```

### Comparing `fprime-tools-3.2.1/src/fprime/util/cli.py` & `fprime-tools-3.3.0/src/fprime/util/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,82 @@
 """ fprime.util.cli: CLI handling
 
 Defines main entrypoint for fprime-util and sets up parsers for general CLI targets.
 
 @author mstarch
 """
 import argparse
-import sys
-import re
 import os
-
+import re
+import sys
 from pathlib import Path
-from typing import Dict, Callable
+from typing import Callable, Dict
 
-from fprime.fbuild.target import Target
+from fprime.fbuild.builder import GenerateException, UnableToDetectProjectException
 from fprime.fbuild.cli import add_fbuild_parsers
-from fprime.fbuild.builder import GenerateException, UnableToDetectDeploymentException
-
+from fprime.fbuild.target import Target
 from fprime.fpp.cli import add_fpp_parsers
-
-from fprime.util.help_text import HelpText
 from fprime.util.build_helper import load_build
-from fprime.util.commands import run_hash_to_file, run_info, run_new, run_code_format
+from fprime.util.commands import run_code_format, run_hash_to_file, run_info, run_new
+from fprime.util.help_text import HelpText
+from fprime.fpp.visualize import add_fpp_viz_parsers
 
 
 def utility_entry(args):
     """Entrypoint for fprime-util, main interface to F' utility"""
     parsed, cmake_args, make_args, parser, runners = parse_args(args)
 
     try:
-        if skip_build_loading(parsed):
-            build = None
-        else:
-            build = load_build(parsed)
+        build = (
+            None
+            if skip_build_loading(parsed)
+            else load_build(parsed, skip_build_cache_validation(parsed))
+        )
 
         # runners is a Dict[str, Callable] of {command_name: handler_functions} pairs
         return runners[parsed.command](
             build, parsed, cmake_args, make_args, getattr(parsed, "pass_through", [])
         )
 
     except GenerateException as genex:
         print(
             f"[ERROR] {genex}. Partial build cache remains. Run purge to clean-up.",
             file=sys.stderr,
         )
-    except UnableToDetectDeploymentException:
-        print(f"[ERROR] Could not detect deployment directory for: {parsed.path}")
+    except UnableToDetectProjectException:
+        print(f"[ERROR] Could not detect project directory for: {parsed.path}")
     except Exception as exc:
         print(f"[ERROR] {exc}", file=sys.stderr)
     return 1
 
 
 def skip_build_loading(parsed):
     """Determines if the build load step should be skipped. Commands that do not require a build object
-    should manually be added here by the developer."""
-    if parsed.command == "new" and parsed.new_deployment:
-        return True
+    should manually be added here by the developer.
+    """
     if parsed.command == "new" and parsed.new_project:
         return True
     return False
 
 
+def skip_build_cache_validation(parsed):
+    """Determines if the build cache validation step should be skipped. Commands that do not require a
+    build **cache** should manually be added here by the developer.
+    """
+    if parsed.command in [
+        "purge",
+        "info",
+        "format",
+    ]:
+        return True
+    if parsed.command == "new" and parsed.new_deployment:
+        return True
+    return False
+
+
 def add_special_parsers(
     subparsers, common: argparse.ArgumentParser, help_text: "HelpText"
 ) -> Dict[str, Callable]:
     """Adds in CLI parsers for other commands
 
     Args:
         subparsers: subparsers used to create new CLI subparsers
@@ -119,21 +132,14 @@
         "--component",
         default=False,
         action="store_true",
         dest="new_component",
         help="Tells the new command to generate a component",
     )
     new_exclusive.add_argument(
-        "--port",
-        default=False,
-        action="store_true",
-        dest="new_port",
-        help="Tells the new command to generate a port",
-    )
-    new_exclusive.add_argument(
         "--deployment",
         default=False,
         action="store_true",
         dest="new_deployment",
         help="Tells the new command to generate a deployment",
     )
     new_exclusive.add_argument(
@@ -211,27 +217,27 @@
     # Check platforms for existing toolchain, unless the default is specified.
     if not hasattr(parsed, "command") or parsed.command is None:
         raise ArgValidationException("'fprime-util' not supplied sub-command argument")
     if parsed.command == "generate":
         d_args = {
             match.group(1): match.group(2)
             for match in [CMAKE_REG.match(arg) for arg in unknown]
+            if match is not None
         }
         cmake_args.update(d_args)
         unknown = [arg for arg in unknown if not CMAKE_REG.match(arg)]
     # Build type only for generate, jobs only for non-generate
     elif parsed.command in Target.get_all_targets():
         parsed.settings = None  # Force to load from cache if possible
         make_args["--jobs"] = 1 if parsed.jobs <= 0 else parsed.jobs
     # Check if any arguments are still unknown
     if unknown:
         runnable = f"{os.path.basename(sys.argv[0])} {parsed.command}"
-        raise ArgValidationException(
-            f"'{runnable}' supplied invalid arguments: {','.join(unknown)}"
-        )
+        msg = f"'{runnable}' supplied invalid arguments: {','.join(unknown)}"
+        raise ArgValidationException(msg)
     parsed.build_cache = (
         None if parsed.build_cache is None else Path(parsed.build_cache)
     )
     return cmake_args, make_args
 
 
 def parse_args(args):
@@ -247,19 +253,18 @@
     common_parser.add_argument(
         "platform",
         nargs="?",
         default="default",
         help="F prime build platform (e.g. Linux, Darwin). Default specified in settings.ini",
     )
     common_parser.add_argument(
-        "-d",
-        "--deploy",
-        dest="deploy",
+        "-r",
+        "--root",
         default=None,
-        help="F prime deployment directory to use. May contain multiple build directories.",
+        help="Root of CMake project to use. May contain multiple build directories.",
     )
     common_parser.add_argument(
         "-p",
         "--path",
         default=os.getcwd(),
         help="F prime directory to operate on. Default: cwd, %(default)s.",
     )
@@ -293,18 +298,21 @@
     runners = {}
     parsers = {}
 
     fbuild_runners, fbuild_parsers = add_fbuild_parsers(
         subparsers, common_parser, HelpText
     )
     fpp_runners, fpp_parsers = add_fpp_parsers(subparsers, common_parser)
+    viz_runners, viz_parsers = add_fpp_viz_parsers(subparsers, common_parser)
     parsers.update(fbuild_parsers)
     parsers.update(fpp_parsers)
+    parsers.update(viz_parsers)
     runners.update(fbuild_runners)
     runners.update(fpp_runners)
+    runners.update(viz_runners)
     runners.update(add_special_parsers(subparsers, common_parser, HelpText))
 
     # Parse and prepare to run
     parsed, unknown = parser.parse_known_args(args)
     try:
         cmake_args, make_args = validate(parsed, unknown)
     except ArgValidationException as exc:
```

### Comparing `fprime-tools-3.2.1/src/fprime/util/code_formatter.py` & `fprime-tools-3.3.0/src/fprime/util/code_formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """ fprime.fbuild.code_formatter
 
 Wrapper for clang-format utility.
 
 @author thomas-bc
 """
 
+import re
+import shutil
+import subprocess
+from pathlib import Path
 from typing import Dict, List, Tuple
 
 from fprime.fbuild.target import ExecutableAction, TargetScope
-from pathlib import Path
-
-import subprocess
-import shutil
-import re
-
 
 # MARKER is needed to differentiate at postprocess between access specifiers
 # that were previously an uppercase MACRO, and those that were originally lowercase.
 # MARKER must be a comment for the formatting to behave - so might as well make it
 # a meaningful warning in case it's not postprocessed correctly
 MARKER = "// WARNING: fprime-util format mishap"
 
@@ -53,15 +51,15 @@
         self.style_file = style_file
         self.backup = options.get("backup", True)
         self.verbose = options.get("verbose", False)
         self.validate_extensions = options.get("validate_extensions", True)
         self.allowed_extensions = ALLOWED_EXTENSIONS.copy()
         self._files_to_format: List[Path] = []
 
-    def is_supported(self) -> bool:
+    def is_supported(self, _=None, __=None) -> bool:
         return bool(shutil.which(self.executable))
 
     def allow_extension(self, file_ext: str) -> None:
         """Add a file extension str to the list of allowed extension"""
         self.allowed_extensions.append(file_ext)
 
     def stage_file(self, filepath: Path) -> None:
@@ -135,15 +133,15 @@
                 f"[ERROR] No .clang-format file found in {self.style_file.parent}. "
                 "Override location with --pass-through --style=file:<path>."
             )
             return 1
         # Backup files unless --no-backup is requested
         if self.backup:
             for file in self._files_to_format:
-                shutil.copy2(file, file.parent / (file.stem + ".bak" + file.suffix))
+                shutil.copy2(file, file.parent / f"{file.stem}.bak{file.suffix}")
         pass_through = args[1]
         self._preprocess_files()
         clang_args = [
             self.executable,
             "-i",
             f"--style=file:{self.style_file}",
             *(["--verbose"] if self.verbose else []),
```

### Comparing `fprime-tools-3.2.1/src/fprime/util/commands.py` & `fprime-tools-3.3.0/src/fprime/util/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 """ fprime.util.commands: General-purpose command definitions
 
 Defines general-purpose command processing. Those are commands that do not belong in fbuild or fpp.
 Current commands include:
     - info: Prints out information about the build
     - hash-to-file: Processes hash-to-file to locate file
-    - new: Creates a new component, port, or deployment
+    - new: Creates a new component, deployment, or project
     - format: Formats code using clang-format
 
 @author thomas-bc
 """
 
 import argparse
 import sys
-
 from pathlib import Path
-from typing import List, Dict
+from typing import Dict, List
 
 from fprime.fbuild.builder import Build, InvalidBuildCacheException
-
+from fprime.util.code_formatter import ClangFormatter
 from fprime.util.cookiecutter_wrapper import (
     new_component,
-    new_port,
     new_deployment,
     new_project,
 )
-from fprime.util.code_formatter import ClangFormatter
 
 
 def run_info(
     base: Build, parsed: argparse.Namespace, _: Dict[str, str], __: Dict[str, str], ___
 ):
     """Builds and prints the informational output block
 
@@ -103,40 +100,39 @@
         parsed: parsed arguments for needed for parsed.hash
         _: unused cmake arguments
         __: unused make arguments
         ___: unused pass through arguments
     """
     lines = build.find_hashed_file(parsed.hash)
     if not lines:
-        raise InvalidBuildCacheException(
+        msg = (
             f"Hash 0x{parsed.hash:x} not found. Do you need '--ut' for a unittest run?"
         )
+        raise InvalidBuildCacheException(msg)
     print("[INFO] File(s) associated with hash 0x{:x}".format(parsed.hash))
     for line in lines:
         print("   ", line, end="")
 
 
 def run_new(
     build: Build, parsed: argparse.Namespace, _: Dict[str, str], __: Dict[str, str], ___
 ):
     """Processes new command
 
     Args:
-        build: build used to inform new component and new port calls
+        build: build used to inform new_* calls
         parsed: parsed arguments
         _: unused cmake arguments
         __: unused make arguments
         ___: unused pass through arguments
     """
     if parsed.new_component:
         return new_component(build)
-    if parsed.new_port:
-        return new_port(build)
     if parsed.new_deployment:
-        return new_deployment(parsed)
+        return new_deployment(build, parsed)
     if parsed.new_project:
         return new_project(parsed)
     raise NotImplementedError(
         "`fprime-util new` target is missing or not implemented. See usage (--help)."
     )
```

### Comparing `fprime-tools-3.2.1/src/fprime/util/cookiecutter_wrapper.py` & `fprime-tools-3.3.0/src/fprime/util/cookiecutter_wrapper.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """ Cookie cutter wrapper used to template out components
 """
-import os
 import glob
+import os
+import shutil
 import sys
-from pathlib import Path
-import re
 from contextlib import contextmanager
-import shutil
+from pathlib import Path
 
-from cookiecutter.main import cookiecutter
 from cookiecutter.exceptions import OutputDirExistsException
-from jinja2 import Environment, FileSystemLoader
+from cookiecutter.main import cookiecutter
 
 from fprime.common.utils import confirm
 from fprime.fbuild.builder import Build
-from fprime.fbuild.target import Target
 from fprime.fbuild.cmake import CMakeExecutionException
+from fprime.fbuild.target import Target
 from fprime.util.code_formatter import ClangFormatter
 
 
 def run_impl(build: Build, source_path: Path):
     """Run implementation of files in source_path"""
     target = Target.get_target("impl", set())
 
@@ -34,15 +32,15 @@
         )
         return False
 
     common = [name for name in cpp_files if "Common" in name] + []
     hpp_dest = hpp_files[0]
     cpp_dest = common[0] if common else cpp_files[0]
 
-    if not confirm(f"Generate implementation files (yes/no)? "):
+    if not confirm("Generate implementation files (yes/no)? "):
         return False
     print(
         "Refreshing cache and generating implementation files (ignore 'Stop' CMake warning)..."
     )
     with suppress_stdout():
         target.execute(build, source_path, ({}, [], {}))
 
@@ -75,15 +73,15 @@
     else:
         print("[WARNING] clang-format not found in PATH. Skipping formatting.")
 
     return True
 
 
 def add_to_cmake(list_file: Path, comp_path: Path, project_root: Path = None):
-    """Adds new component or port to CMakeLists.txt. If project_root is supplied,
+    """Adds comp_path directory to CMakeLists.txt. If project_root is supplied,
     the logged path will be relative to the project root instead of absolute"""
     short_display_path = (
         list_file
         if project_root is None
         else project_root.name / list_file.relative_to(project_root)
     )
     print(f"[INFO] Found CMake file at '{short_display_path}'")
@@ -115,45 +113,15 @@
         sys.stdout = devnull
         try:
             yield
         finally:
             sys.stdout = old_stdout
 
 
-def regenerate(build: Build):
-    print("Refreshing cache to include new addition...")
-    with suppress_stdout():
-        try:
-            build.cmake.cmake_refresh_cache(build.get_build_cache())
-        except CMakeExecutionException:
-            build.cmake.cmake_refresh_cache(build.get_build_cache(), True)
-
-
-def add_port_to_cmake(list_file: Path, comp_path: Path):
-    """Adds new port to CMakeLists.txt in port directory"""
-    print(f"[INFO] Found CMakeLists.txt at '{list_file}'")
-    with open(list_file, "r") as file_handle:
-        lines = file_handle.readlines()
-    index = 0
-    while re.search("set\(\s*SOURCE_FILES", lines[index]) is None:
-        index += 1
-    index += 1
-    while "CMAKE_CURRENT_LIST_DIR" in lines[index]:
-        index += 1
-    if not confirm(f"Add port {comp_path} to {list_file} ports in CMakeLists.txt?"):
-        return False
-
-    addition = '    "${{CMAKE_CURRENT_LIST_DIR}}/{}"\n'.format(comp_path)
-    lines.insert(index, addition)
-    with open(list_file, "w") as file_handle:
-        file_handle.write("".join(lines))
-    return True
-
-
-def find_nearest_cmake_file(component_dir: Path, deployment: Path, proj_root: Path):
+def find_nearest_cmake_file(component_dir: Path, cmake_root: Path, proj_root: Path):
     """Find the nearest CMake file, i.e. CMakeLists.txt or project.cmake
 
     The "nearest" file is defined as the closest parent that is not the project root CMakeLists.txt.
     If none is found, the same procedure is run from the deployment directory and includes the project
     root this time. If nothing is found, None is returned.
 
     In short the following in order of preference:
@@ -168,62 +136,29 @@
         proj_root: project root directory
 
     Returns:
         path to CMakeLists.txt or None
     """
     test_path = component_dir.parent
     # First iterate from where we are, then from the deployment to find the nearest CMakeList.txt nearby
-    for test_path, end_path in [(test_path, proj_root), (deployment, proj_root.parent)]:
+    for test_path, end_path in [(test_path, proj_root), (cmake_root, proj_root.parent)]:
         while proj_root is not None and test_path != proj_root.parent:
             project_file = test_path / "project.cmake"
             if project_file.is_file():
                 return project_file
             cmake_list_file = test_path / "CMakeLists.txt"
             if cmake_list_file.is_file():
                 return cmake_list_file
             test_path = test_path.parent
     return None
 
 
-def find_nearest_cmake_lists(component_dir: Path, deployment: Path, proj_root: Path):
-    """Find the nearest CMakeLists.txt file
-
-    The "nearest" file is defined as the closes parent that is not the "project root" that contains a CMakeLists.txt. If
-    none is found, the same procedure is run from the deployment directory and includes the project root this time. If
-    nothing is found, None is returned.
-
-    In short the following in order of preference:
-     - Any Component Parent
-     - Any Deployment Parent
-     - Project Root
-     - None
-
-    Args:
-        component_dir: directory of new component
-        deployment: deployment directory
-        proj_root: project root directory
-
-    Returns:
-        path to CMakeLists.txt or None
-    """
-    test_path = component_dir.parent
-    # First iterate from where we are, then from the deployment to find the nearest CMakeList.txt nearby
-    for test_path, end_path in [(test_path, proj_root), (deployment, proj_root.parent)]:
-        while proj_root is not None and test_path != proj_root.parent:
-            cmake_list_file = test_path / "CMakeLists.txt"
-            if cmake_list_file.is_file():
-                return cmake_list_file
-            test_path = test_path.parent
-    return None
-
-
 def new_component(build: Build):
     """Uses cookiecutter for making new components"""
     try:
-        deployment = build.deployment
         proj_root = build.get_settings("project_root", None)
 
         # Checks if component_cookiecutter is set in settings.ini file, else uses local component_cookiecutter template as default
         if (
             build.get_settings("component_cookiecutter", None) is not None
             and build.get_settings("component_cookiecutter", None) != "default"
         ):
@@ -232,32 +167,34 @@
         else:
             source = (
                 os.path.dirname(__file__)
                 + "/../cookiecutter_templates/cookiecutter-fprime-component"
             )
             print("[INFO] Cookiecutter source: using builtin")
 
-        # Use deployment name as default namespace if a deployment was found
+        # Use current working directory name as default namespace, unless at project root
         extra_context = {}
-        if not proj_root.samefile(deployment):
-            extra_context["component_namespace"] = deployment.name
+        if not proj_root.samefile(Path.cwd()):
+            extra_context["component_namespace"] = Path.cwd().name
 
         final_component_dir = Path(
             cookiecutter(source, extra_context=extra_context)
         ).resolve()
 
         if proj_root is None:
             print(
                 f"[INFO] Created component directory without adding to build system nor generating implementation {final_component_dir}"
             )
             return 0
 
         # Attempt to register to CMakeLists.txt
         proj_root = Path(proj_root)
-        cmake_file = find_nearest_cmake_file(final_component_dir, deployment, proj_root)
+        cmake_file = find_nearest_cmake_file(
+            final_component_dir, build.cmake_root, proj_root
+        )
         if cmake_file is None or not add_to_cmake(
             cmake_file,
             final_component_dir.relative_to(cmake_file.parent),
             proj_root,
         ):
             print(
                 f"[INFO] Could not register {final_component_dir} with build system. Please add it and generate implementations manually."
@@ -272,214 +209,71 @@
 
         print("[INFO] Created new component and generated initial implementations.")
         return 0
     except OutputDirExistsException as out_directory_error:
         print(f"{out_directory_error}", file=sys.stderr)
     except CMakeExecutionException as exc:
         print(f"[ERROR] Failed to create component. {exc}", file=sys.stderr)
+    except FileNotFoundError as e:
+        print(
+            f"{e}. Permission denied to write to the directory.",
+            file=sys.stderr,
+        )
+        return 1
     except OSError as ose:
         print(f"[ERROR] {ose}")
     return 1
 
 
-def is_valid_name(word: str):
-    invalid_characters = [
-        "#",
-        "%",
-        "&",
-        "{",
-        "}",
-        "/",
-        "\\",
-        "<",
-        ">",
-        "*",
-        "?",
-        " ",
-        "$",
-        "!",
-        "'",
-        '"',
-        ":",
-        "@",
-        "+",
-        "`",
-        "|",
-        "=",
-    ]
-    for char in invalid_characters:
-        if isinstance(word, str) and char in word:
-            return char
-        if not isinstance(word, str):
-            raise ValueError("Incorrect usage of is_valid_name")
-    return "valid"
-
-
-def get_valid_input(prompt):
-    valid_name = False
-    while not valid_name:
-        name = input(prompt)
-        char = is_valid_name(name)
-        if char != "valid":
-            print("'" + char + "' is not a valid character")
-        else:
-            valid_name = True
-    return name
-
-
-def get_port_input(namespace):
-    # Gather inputs to use as context for the port template
-    defaults = {
-        "port_name": "ExamplePort",
-        "short_description": "Example usage of port",
-        "dir_name": ".",
-        "namespace": namespace,
-        "arg_list": [],
-    }
-    args_done = False
-    arg_list = []
-    port_name = get_valid_input(f'Port Name [{defaults["port_name"]}]: ')
-    short_description = input(f'Short Description [{defaults["short_description"]}]: ')
-    dir_name = get_valid_input(f'Directory Name [{defaults["dir_name"]}]: ')
-    namespace = get_valid_input(f'Port Namespace [{defaults["namespace"]}]: ')
-    while not args_done:
-        add_arg = (
-            confirm("Would you like to add another argument?: ")
-            if arg_list
-            else confirm("Would you like to add an argument?: ")
-        )
-        if add_arg:
-            arg_name = get_valid_input("Argument name: ")
-            arg_type = get_valid_input(
-                "Argument type (Valid primitive types are: I8, I16, "
-                + "I32, U8, U16, U32, F32, F64, NATIVE_INT_TYPE, NATIVE_UNIT_TYPE, and POINTER_CAST. "
-                + "You may also use your own user-defined types): "
-            )
-            arg_description = input("Short description of argument: ")
-            arg_list.append((arg_name, arg_type, arg_description))
-        else:
-            args_done = True
-    values = {
-        "port_name": port_name,
-        "short_description": short_description,
-        "dir_name": dir_name,
-        "namespace": namespace,
-        "arg_list": arg_list,
-    }
-
-    # Fill in blank values with defaults
-    for key in values:
-        if values[key] == "":
-            values[key] = defaults[key]
-    return values
-
-
-def new_port(build: Build):
-    """Uses cookiecutter for making new ports"""
-    try:
-        deployment = build.deployment
-        proj_root = build.get_settings("project_root", None)
-        if proj_root is not None:
-            proj_root = Path(proj_root)
-            proj_root_found = True
-        else:
-            proj_root_found = False
-
-        PATH = os.path.dirname(os.path.abspath(__file__))
-        TEMPLATE_ENVIRONMENT = Environment(
-            autoescape=False,
-            loader=FileSystemLoader(os.path.join(PATH, "../cookiecutter_templates")),
-            trim_blocks=False,
+def new_deployment(build: Build, parsed_args):
+    """Creates a new deployment using cookiecutter"""
+    # Checks if deployment_cookiecutter is set in settings.ini file, else uses local install template as default
+    if (
+        build.get_settings("deployment_cookiecutter", None) is not None
+        and build.get_settings("deployment_cookiecutter", None) != "default"
+    ):
+        source = build.get_settings("deployment_cookiecutter", None)
+        print(f"[INFO] Cookiecutter source: {source}")
+    else:
+        source = (
+            os.path.dirname(__file__)
+            + "/../cookiecutter_templates/cookiecutter-fprime-deployment"
         )
-        context = get_port_input(deployment.name)
-
-        if Path(context["dir_name"]).resolve() == deployment.resolve():
-            print("[ERROR] cannot create port in deployment directory")
-            return 0
-        fname = context["port_name"] + "Port" + "Ai.xml"
-        if os.path.isfile(Path(context["dir_name"], fname)):
-            print(
-                "[ERROR] Port",
-                context["port_name"],
-                "already exists in directory",
-                context["dir_name"],
-            )
-            return 0
-        with open(fname, "w") as f:
-            xml_file = TEMPLATE_ENVIRONMENT.get_template("port_template.xml").render(
-                context
-            )
-            f.write(xml_file)
-        if not os.path.isdir(context["dir_name"]):
-            os.mkdir(context["dir_name"])
-
-        os.rename(fname, str(Path(context["dir_name"], fname)))
-        path_to_cmakelists = Path(context["dir_name"], "CMakeLists.txt")
-        if not os.path.isfile(str(path_to_cmakelists)):
-            with open(str(path_to_cmakelists), "w") as f:
-                CMake_file = TEMPLATE_ENVIRONMENT.get_template(
-                    "CMakeLists_template.txt"
-                ).render(context)
-                f.write(CMake_file)
-        else:
-            add_port_to_cmake(str(path_to_cmakelists), fname)
+        print("[INFO] Cookiecutter: using builtin template for new deployment")
+    try:
+        gen_path = Path(
+            cookiecutter(source, overwrite_if_exists=parsed_args.overwrite)
+        ).resolve()
 
-        if not proj_root_found:
-            print(
-                "[INFO] No project root found. Created port without adding to build system nor generating implementation."
-            )
-            return 0
-        cmake_lists_file = find_nearest_cmake_lists(
-            Path(context["dir_name"]).resolve(), deployment, proj_root
-        )
-        if cmake_lists_file is None or not add_to_cmake(
-            cmake_lists_file,
-            (Path(context["dir_name"]).resolve()).relative_to(cmake_lists_file.parent),
+        proj_root = build.get_settings("project_root", None)
+        # Attempt to register to CMakeLists.txt or project.cmake
+        proj_root = Path(proj_root)
+        cmake_file = find_nearest_cmake_file(gen_path, build.cmake_root, proj_root)
+        if cmake_file is None or not add_to_cmake(
+            cmake_file,
+            gen_path.relative_to(cmake_file.parent),
+            proj_root,
         ):
             print(
-                f'[INFO] Could not register {Path(context["dir_name"]).resolve()} with build system. Please add it and generate implementations manually.'
+                f"[INFO] Could not register {gen_path} with build system. Please add it manually."
             )
             return 0
-        regenerate(build)
-        print("")
-        print("#" * 80)
-        print("")
-        print(
-            "You have successfully created the port "
-            + context["port_name"]
-            + " located in "
-            + context["dir_name"]
-        )
-        print("")
-        print("#" * 80)
-        return 0
-    except OutputDirExistsException as out_directory_error:
-        print(f"{out_directory_error}", file=sys.stderr)
-    except CMakeExecutionException as exc:
-        print(f"[ERROR] Failed to create port. {exc}", file=sys.stderr)
-    except OSError as ose:
-        print(f"[ERROR] {ose}")
-    return 1
 
-
-def new_deployment(parsed_args):
-    """Creates a new deployment using cookiecutter"""
-    source = (
-        os.path.dirname(__file__)
-        + "/../cookiecutter_templates/cookiecutter-fprime-deployment"
-    )
-    print(f"[INFO] Cookiecutter: using builtin template for new deployment")
-    try:
-        gen_path = cookiecutter(source, overwrite_if_exists=parsed_args.overwrite)
     except OutputDirExistsException as out_directory_error:
         print(
             f"{out_directory_error}. Use --overwrite to overwrite (will not delete non-generated files).",
             file=sys.stderr,
         )
         return 1
+    except FileNotFoundError as e:
+        print(
+            f"{e}. Permission denied to write to the directory.",
+            file=sys.stderr,
+        )
+        return 1
     print(f"[INFO] New deployment successfully created: {gen_path}")
     return 0
 
 
 def new_project(parsed_args):
     """Creates a new F' project"""
 
@@ -503,9 +297,48 @@
         )
     except OutputDirExistsException as out_directory_error:
         print(
             f"{out_directory_error}. Use --overwrite to overwrite (will not delete non-generated files).",
             file=sys.stderr,
         )
         return 1
+    except FileNotFoundError as e:
+        print(
+            f"{e}. Permission denied to write to the directory.",
+            file=sys.stderr,
+        )
+        return 1
     print(f"[INFO] New project successfully created: {gen_path}")
     return 0
+
+
+def is_valid_name(word: str):
+    invalid_characters = [
+        "#",
+        "%",
+        "&",
+        "{",
+        "}",
+        "/",
+        "\\",
+        "<",
+        ">",
+        "*",
+        "?",
+        " ",
+        "$",
+        "!",
+        "'",
+        '"',
+        ":",
+        "@",
+        "+",
+        "`",
+        "|",
+        "=",
+    ]
+    for char in invalid_characters:
+        if isinstance(word, str) and char in word:
+            return char
+        if not isinstance(word, str):
+            raise ValueError("Incorrect usage of is_valid_name")
+    return "valid"
```

### Comparing `fprime-tools-3.2.1/src/fprime/util/help_text.py` & `fprime-tools-3.3.0/src/fprime/util/help_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 `
 
 @author lestarch
 """
 import os
 import sys
 
-
 # Attempt to get pkg_resources from "setuptools"
 try:
     import pkg_resources
 
     VERSION = pkg_resources.get_distribution("fprime-tools").version
 except ImportError:
     VERSION = "(unknown version)"
@@ -34,15 +33,15 @@
 
 '{EXECUTABLE}' wraps the fprime build system enabling developers to follow standard patterns when developing fprime
 applications. Specifically it translates between the developer's context (working directory and supplied flags) to the
 build system targets defined for that context. i.e. a developer can change directory into a component directory and run
 commands restricted to that component.
 
 Almost all {EXECUTABLE} commands require a valid build cache to run. Thus users should start by running '{EXECUTABLE}
-generate' in their desired deployment before running command. Once a build cache has been generated other commands can
+generate' in their desired project before running command. Once a build cache has been generated other commands can
 be run. The '--ut' flag sets up a testing build cache and enables unit test commands to be run. An explanation of how
 {EXECUTABLE} determines the build cache is included below. More information on creating build caches can be found with:
 '{EXECUTABLE} generate --help'.
 
 Examples:
 
   -- Setup and Build Ref On Default Platform  --
@@ -62,18 +61,18 @@
   {EXECUTABLE} build
 
 {EXECUTABLE} uses the working directory and supplied flags as context for all the commands it runs. This context is used
 to determine two build properties: build cache (created by 'fprime-util generate') to be used and build target to
 execute. The build cache is chosen by recurring upward from the current working directory looking for the first build
 cache matching the specified platform. If '--ut' is specified, only UT caches will be selected. The platform is read
 from the optional positional argument 'platform'. If not specified on the command line, the 'default_toolchain' setting
-in the deployment's settings.ini file is read. In not specified there, the default toolchain "native" is used.
+in the project's settings.ini file is read. If not specified there, the default toolchain "native" is used.
 
-If a different deployment is desired, the recursive search behavior can be altered with the '-d/--deployment'. When
-'-d/--deployment' is specified, a matching build cache will be selected from within the supplied deployment directory.
+If a different CMake root is desired, the recursive search behavior can be altered with the '-r/--root'. When
+'-r/--root' is specified, a matching build cache will be selected from within the supplied root directory.
 '--build-cache' may be supplied to force '{EXECUTABLE}' to use the supplied build cache regardless of other conditions.
 
 Once the build cache has been selected, the build target is chosen. {EXECUTABLE} will run the supplied command for
 a chosen directory.  This directory is can be set using the '-p/--path' argument and defaults to the user's current
 working directory. This command and directory are translated into the build target to be executed.
 e.g. 'cd Ref/SignalGen; {EXECUTABLE} impl' will run the build target 'Ref_SignalGen_impl'. Most users need not care
 about the specific build target being run and should think "command run in chosen directory".
@@ -89,15 +88,15 @@
 
   -- Build SignalGen Component --
   cd Ref/SignalGen
   {EXECUTABLE} build
 
   -- Build Command Dispatcher UTs for Ref Deployment --
   cd Svc/CmdDispatcher
-  {EXECUTABLE} build --ut -d ../../Ref/
+  {EXECUTABLE} build --ut -r ../../Ref/
 
   -- Build Command Dispatcher UTs for Ref Deployment (Alternate) --
   cd Ref
   {EXECUTABLE} build --ut -p ../../Svc/CmdDispatcher
 
   -- Build Everything --
   {EXECUTABLE} build --all
@@ -186,17 +185,17 @@
   -- Run Ref/SignalGen Unit Tests With Detailed HTML Coverage --
   cd Ref/SignalGen
   {EXECUTABLE} check --coverage
 """,
     "generate": f"""{EXECUTABLE} generate ({VERSION}): Generate build caches for the specified deployment
 
 '{EXECUTABLE} generate' is used to setup a build cache to support other commands run by {EXECUTABLE}. Without additional
-arguments a build cache will be created for the deployment in the specified directory ('-p/--path', or current working
-directory). It will use the default settings specified in the deployment's settings.ini file for the target platform,
-fprime libraries, etc. Specifying '-d/--deployment' generates the deployment at the supplied directory overriding the
+arguments a build cache will be created for the project in the specified directory ('-p/--path', or current working
+directory). It will use the default settings specified in the project's settings.ini file for the target platform,
+fprime libraries, etc. Specifying '-r/--root' generates the project at the supplied directory overriding the
 directory specified with '-p/--path' and the current working directory. '--ut' should be specified to generate testing
 build caches for running unit tests.
 
 Basic Examples:
   -- Generate Ref Build Cache With Default Settings --
   cd Ref
   {EXECUTABLE} generate
@@ -233,29 +232,29 @@
   {EXECUTABLE} generate --ut -DFPRIME_ENABLE_AUTOCODER_UTS=OFF
 
   -- Generate Ref With Baremetal Scheduler Into Specific Cache --
   cd Ref
   {EXECUTABLE} generate --build-cache `pwd`/build-ref-with-baremetal -DFPRIME_USE_BAREMETAL_SCHEDULER=ON
 
 """,
-    "purge": f"""{EXECUTABLE} purge ({VERSION}): Removes build caches for specified deployment
+    "purge": f"""{EXECUTABLE} purge ({VERSION}): Removes build caches for specified project
     
-'{EXECUTABLE} purge' removes build caches for the specified deployment. It also removes the build_artifacts directory
-in that deployment as well. Caches are searched in pairs: normal build cache, paired unit testing build cache. The
+'{EXECUTABLE} purge' removes build caches for the specified project. It also removes the build_artifacts directory
+in that project as well. Caches are searched in pairs: normal build cache, paired unit testing build cache. The
 user will be asked to confirm when a build cache is being removed unless the '--force' flag is specified. The platform
 will use the settings specified in 'settings.ini' or as specified with the optional positional argument. The
 '--build-cache' flag can be used to remove an exact build cache without looking at other build caches.
 
 '{EXECUTABLE} purge' will not remove build caches that do not look like valid build caches unless the '--force' flag is
 supplied. In this case, the build cache will be removed with reckless abandon.
     """,
     "info": f"""Print contextual target and build cache information before exiting
 
 '{EXECUTABLE} info' is used to print contextual information to the user before exiting. It will print the available]
-commands within the current context (working directory, '-p/--path', '-d/--deployment', etc.) and then exit. Users may
+commands within the current context (working directory, '-p/--path', '-r/--root', etc.) and then exit. Users may
 use the info command as a way to test and understand how {EXECUTABLE} is mapping to the context and targets used. info
 may also be used to locate the artifact output folders within the build cache in order to see generated files, compiler
 outputs, etc.
 
 '{EXECUTABLE} info' will print information for both normal and unit testing builds when possible. If '--build-cache' is
 specified then only the information for that build cache will be printed.
 """,
@@ -290,16 +289,14 @@
   Generate a new F' deployment within a F' project. The new deployment command is expected to be ran at the root of
   the project and will create a new deployment in the current directory. Using --overwrite will overwrite only the
   files that are generated by the new deployment.
   -- New Component --
   Generate a new F' component within a F' project. This command prompts for what type of component and what it should
   include. At the end of the generation, the user can chose to automatically add the component to the build system and
   run the implementation generator.
-  -- New Port --
-  WARNING: prototype code generating XML only. Not recommended for inexperienced users. Please check back later.
 """,
     "format": f"""{EXECUTABLE} format ({VERSION}): Formats C/C++ files using clang-format
 
 '{EXECUTABLE} format' uses 'clang-format' to format C/C++ files. It uses the style specified in the .clang-format file
 found at the root of the F' framework used by the project (i.e. the 'framework_path' specified in settings.ini).
 Files are specified through stdin or by using the '--files [<path/to/file>]*' flag. When reading from stdin, file paths
 should be separated by whitespace characters.
```

### Comparing `fprime-tools-3.2.1/src/fprime/util/string_util.py` & `fprime-tools-3.3.0/src/fprime/util/string_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 Utility functions to process strings to be used in FPrime GDS
 @Created March 18, 2021
 @`janamian`
 
 Note: This function has an identical copy in fprime-gds
 """
 
-import re
 import logging
+import re
 
 LOGGER = logging.getLogger("string_util_logger")
 
 
 def format_string_template(format_str, given_values):
     """
     Function to convert C-string style to python format
@@ -88,15 +88,15 @@
 
     # First try to include all types
     try:
         formatted_str = re.sub(match, convert_include_all, format_str)
         result = formatted_str.format(*values)
         result = result.replace("%%", "%")
         return result
-    except ValueError as e:
+    except ValueError:
         msg = "Value and format string do not match. "
         msg += " Will ignore integer flags `d` in string template. "
         msg += f"values: {values}. "
         msg += f"format_str: {format_str}. "
         LOGGER.warning(msg)
 
     # Second try by not including %d.
```

### Comparing `fprime-tools-3.2.1/src/fprime/util/versioning.py` & `fprime-tools-3.3.0/src/fprime/util/versioning.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,27 +20,26 @@
         requirements: path to requirements file to parse
     """
     with open(requirements, "r") as file_handle:
         matching_lines = [
             line.strip() for line in file_handle.readlines() if package in line
         ]
     if not matching_lines:
-        raise VersionException(f"Could not find {package} in requirements file")
+        msg = f"Could not find {package} in requirements file"
+        raise VersionException(msg)
     valid_lines = [line for line in matching_lines if "==" in line or "@" in line]
     if not valid_lines:
-        raise VersionException(
-            f"{package} has inexact version, use '==' or '@' format. Found: {matching_lines}"
-        )
+        msg = f"{package} has inexact version, use '==' or '@' format. Found: {matching_lines}"
+        raise VersionException(msg)
 
     # Collapse versions that match
     versions = list({line.split("==")[-1].split("@")[-1] for line in valid_lines})
     if len(versions) != 1:
-        raise VersionException(
-            f"Conflicting versions specified for {package}: {versions}"
-        )
+        msg = f"Conflicting versions specified for {package}: {versions}"
+        raise VersionException(msg)
     return versions[0]
 
 
 def main():
     """Parses arguments and acts as entry point for the tool"""
     parser = argparse.ArgumentParser(
         description="Detects the required package using a requirements file"
```

### Comparing `fprime-tools-3.2.1/src/fprime_tools.egg-info/PKG-INFO` & `fprime-tools-3.3.0/src/fprime_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fprime-tools
-Version: 3.2.1
+Version: 3.3.0
 Summary: F Prime Flight Software core data types
 Home-page: https://github.com/nasa/fprime
 Author: Michael Starch
 Author-email: Michael.D.Starch@jpl.nasa.gov
 License: Apache 2.0 License
 Project-URL: Issue Tracker, https://github.com/nasa/fprime/issues
 Keywords: fprime,embedded,nasa
```

### Comparing `fprime-tools-3.2.1/src/fprime_tools.egg-info/SOURCES.txt` & `fprime-tools-3.3.0/src/fprime_tools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,53 +35,53 @@
 src/fprime/common/models/serialize/enum_type.py
 src/fprime/common/models/serialize/numerical_types.py
 src/fprime/common/models/serialize/serializable_type.py
 src/fprime/common/models/serialize/string_type.py
 src/fprime/common/models/serialize/time_type.py
 src/fprime/common/models/serialize/type_base.py
 src/fprime/common/models/serialize/type_exceptions.py
-src/fprime/cookiecutter_templates/CMakeLists_template.txt
-src/fprime/cookiecutter_templates/port_template.xml
 src/fprime/cookiecutter_templates/cookiecutter-fprime-component/cookiecutter.json
 src/fprime/cookiecutter_templates/cookiecutter-fprime-component/hooks/pre_gen_project.py
 src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/CMakeLists.txt
 src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.cpp
 src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.fpp
 src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/{{cookiecutter.component_name}}.hpp
 src/fprime/cookiecutter_templates/cookiecutter-fprime-component/{{cookiecutter.component_name}}/docs/sdd.md
 src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/cookiecutter.json
 src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/CMakeLists.txt
 src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Main.cpp
 src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/README.md
-src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/settings.ini
 src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/CMakeLists.txt
 src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/instances.fpp
 src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/topology.fpp
 src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Packets.xml
 src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Topology.cpp
 src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}Topology.hpp
 src/fprime/cookiecutter_templates/cookiecutter-fprime-deployment/{{cookiecutter.deployment_name}}/Top/{{cookiecutter.deployment_name}}TopologyDefs.hpp
 src/fprime/cookiecutter_templates/cookiecutter-fprime-project/cookiecutter.json
 src/fprime/cookiecutter_templates/cookiecutter-fprime-project/hooks/post_gen_project.py
+src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/.gitignore
 src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/CMakeLists.txt
 src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/README.md
 src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/project.cmake
 src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/settings.ini
+src/fprime/cookiecutter_templates/cookiecutter-fprime-project/{{cookiecutter.project_name}}/Components/CMakeLists.txt
 src/fprime/fbuild/__init__.py
 src/fprime/fbuild/builder.py
 src/fprime/fbuild/cli.py
 src/fprime/fbuild/cmake.py
 src/fprime/fbuild/gcovr.py
 src/fprime/fbuild/settings.py
 src/fprime/fbuild/target.py
 src/fprime/fbuild/target_definitions.py
 src/fprime/fbuild/types.py
 src/fprime/fpp/__init__.py
 src/fprime/fpp/cli.py
 src/fprime/fpp/common.py
+src/fprime/fpp/visualize.py
 src/fprime/util/__init__.py
 src/fprime/util/__main__.py
 src/fprime/util/build_helper.py
 src/fprime/util/cli.py
 src/fprime/util/code_formatter.py
 src/fprime/util/commands.py
 src/fprime/util/cookiecutter_wrapper.py
```

### Comparing `fprime-tools-3.2.1/test/fprime/common/models/serialize/test_types.py` & `fprime-tools-3.3.0/test/fprime/common/models/serialize/test_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 Created on Jun 25, 2020
 @author: hpaulson, mstarch
 """
 import json
 from collections.abc import Iterable
 
 import pytest
-
 from fprime.common.models.serialize.array_type import ArrayType
 from fprime.common.models.serialize.bool_type import BoolType
 from fprime.common.models.serialize.enum_type import EnumType
 from fprime.common.models.serialize.numerical_types import (
     F32Type,
     F64Type,
     I8Type,
@@ -24,29 +23,27 @@
     U32Type,
     U64Type,
 )
 from fprime.common.models.serialize.serializable_type import SerializableType
 from fprime.common.models.serialize.string_type import StringType
 from fprime.common.models.serialize.time_type import TimeBase, TimeType
 from fprime.common.models.serialize.type_base import BaseType, DictionaryType, ValueType
-
 from fprime.common.models.serialize.type_exceptions import (
     AbstractMethodException,
     ArrayLengthException,
     DeserializeException,
     EnumMismatchException,
     IncorrectMembersException,
     MissingMemberException,
     NotInitializedException,
     StringSizeException,
     TypeMismatchException,
     TypeRangeException,
 )
 
-
 PYTHON_TESTABLE_TYPES = [
     True,
     False,
     -1,
     0,
     300,
     "abc",
@@ -467,18 +464,18 @@
     ]
 
     val = TimeType()
     size = val.getSize()
     assert size == TIME_SIZE
     assert val.getMaxSize() == TIME_SIZE
 
-    for (t_base, t_context, secs, usecs) in in_no_err_list:
+    for t_base, t_context, secs, usecs in in_no_err_list:
         ser_deser_time_test(t_base, t_context, secs, usecs)
 
-    for (t_base, t_context, secs, usecs) in in_err_list:
+    for t_base, t_context, secs, usecs in in_err_list:
         with pytest.raises(TypeRangeException):
             ser_deser_time_test(t_base, t_context, secs, usecs)
 
 
 class Dummy(BaseType):
     def serialize(self):
         return "serialized"
```

### Comparing `fprime-tools-3.2.1/test/fprime/common/models/serialize/time_type_unit_test.py` & `fprime-tools-3.3.0/test/fprime/common/models/serialize/time_type_unit_test.py`

 * *Files identical despite different names*

### Comparing `fprime-tools-3.2.1/test/fprime/fbuild/test_build.py` & `fprime-tools-3.3.0/test/fprime/fbuild/test_build.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 that they function as expected.
 
 @author mstarch
 """
 import os
 import pathlib
 
-import pytest
-
-import fprime.fbuild.cmake
 import fprime.fbuild.builder
+import fprime.fbuild.cmake
+import pytest
 
 
 def get_cmake_builder():
     """Gets a CMake builder for these tests
 
     Returns:
         CMakeBuilder for testing
@@ -29,17 +28,16 @@
     Gets directory containing test-data specific to the builder being tested. This will enable new implementers, should
     there be any, to implement their own build-directory structure.
 
     :return:
     """
     if type(get_cmake_builder()) is fprime.fbuild.cmake.CMakeHandler:
         return os.path.join(os.path.dirname(__file__), "cmake-data")
-    raise Exception(
-        f"Test data directory not setup for {type(get_cmake_builder())} builder class"
-    )
+    msg = f"Test data directory not setup for {type(get_cmake_builder())} builder class"
+    raise Exception(msg)
 
 
 def test_hash_finder():
     """
     Tests that the hash finder works given a known builds.
     """
     local = pathlib.Path(os.path.dirname(__file__))
@@ -170,15 +168,15 @@
                 with pytest.raises(fprime.fbuild.cmake.CMakeOrphanException):
                     value = get_cmake_builder().get_include_info(path, build_dir)
             else:
                 value = get_cmake_builder().get_include_info(path, build_dir)
                 assert value == truth
 
 
-def test_find_nearest_deployment():
+def test_find_nearest_parent_project():
     """
     This will test the ability for the system to detect valid deployment directories
     """
 
     test_dir = pathlib.Path(get_data_dir())
     test_data = [
         ("testbuild/subdir1/subdir2/subdir3", "testbuild/subdir1/"),
@@ -186,12 +184,12 @@
         ("testbuild/", "testbuild/"),
         ("/nonexistent/dirone/someotherpath", None),
     ]
     for path, truth in test_data:
         path = test_dir / path
         if truth is not None:
             truth = test_dir / truth
-            value = fprime.fbuild.builder.Build.find_nearest_deployment(path)
+            value = fprime.fbuild.builder.Build.find_nearest_parent_project(path)
             assert value == truth
         else:
-            with pytest.raises(fprime.fbuild.builder.UnableToDetectDeploymentException):
-                fprime.fbuild.builder.Build.find_nearest_deployment(path)
+            with pytest.raises(fprime.fbuild.builder.UnableToDetectProjectException):
+                fprime.fbuild.builder.Build.find_nearest_parent_project(path)
```

### Comparing `fprime-tools-3.2.1/test/fprime/fbuild/test_settings.py` & `fprime-tools-3.3.0/test/fprime/fbuild/test_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """
 (test) fprime.fbuild.settings:
 
 Tests the F prime settings module.
 @author joshuaa
 """
 
-import pytest
-import os
 from pathlib import Path
 
 from fprime.fbuild.settings import IniSettings
 
 LOCAL_PATH = Path(__file__).parent
 
 
@@ -32,14 +30,15 @@
                 "default_ut_toolchain": "native",
                 "framework_path": full_path(".."),
                 "install_destination": full_path("settings-data/build-artifacts"),
                 "library_locations": [],
                 "environment_file": full_path("settings-data/settings-empty.ini"),
                 "environment": {},
                 "component_cookiecutter": "default",
+                "deployment_cookiecutter": "default",
                 "ac_constants": full_path("..") / "config" / "AcConstants.ini",
                 "project_root": full_path(".."),
                 "config_directory": full_path("..") / "config",
                 "default_cmake_options": "",
             },
         },
         {
@@ -52,14 +51,15 @@
                 "install_destination": full_path("test"),
                 "library_locations": [],
                 "environment_file": full_path(
                     "settings-data/settings-custom-install.ini"
                 ),
                 "environment": {},
                 "component_cookiecutter": "default",
+                "deployment_cookiecutter": "default",
                 "ac_constants": full_path("..") / "config" / "AcConstants.ini",
                 "project_root": full_path(".."),
                 "config_directory": full_path("..") / "config",
                 "default_cmake_options": "",
             },
         },
         {
@@ -74,14 +74,15 @@
                 "install_destination": full_path("settings-data/build-artifacts"),
                 "library_locations": [],
                 "environment_file": full_path(
                     "settings-data/settings-custom-toolchain.ini"
                 ),
                 "environment": {},
                 "component_cookiecutter": "default",
+                "deployment_cookiecutter": "default",
                 "ac_constants": full_path("..") / "config" / "AcConstants.ini",
                 "project_root": full_path(".."),
                 "config_directory": full_path("..") / "config",
                 "default_cmake_options": "",
             },
         },
         {
@@ -96,14 +97,15 @@
                 "install_destination": full_path("settings-data/build-artifacts"),
                 "library_locations": [],
                 "environment_file": full_path(
                     "settings-data/settings-outside-cookiecutter.ini"
                 ),
                 "environment": {},
                 "component_cookiecutter": "gh:SterlingPeet/cookiecutter-fprime-deployment",
+                "deployment_cookiecutter": "https://github.com/thomas-bc/fprime-deployment-cookiecutter.git",
                 "ac_constants": full_path("..") / "config" / "AcConstants.ini",
                 "project_root": full_path(".."),
                 "config_directory": full_path("..") / "config",
                 "default_cmake_options": "",
             },
         },
         {
@@ -118,14 +120,15 @@
                 "install_destination": full_path("settings-data/build-artifacts"),
                 "library_locations": [],
                 "environment_file": full_path(
                     "settings-data/settings-multi-line-default-options.ini"
                 ),
                 "environment": {},
                 "component_cookiecutter": "default",
+                "deployment_cookiecutter": "default",
                 "ac_constants": full_path("..") / "config" / "AcConstants.ini",
                 "project_root": full_path(".."),
                 "config_directory": full_path("..") / "config",
                 "default_cmake_options": "OPTION1=ABC\nOPTION2=123\nOPTION3=Something",
             },
         },
     ]
```

