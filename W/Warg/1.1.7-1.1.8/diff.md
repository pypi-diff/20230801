# Comparing `tmp/Warg-1.1.7.tar.gz` & `tmp/Warg-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Warg-1.1.7.tar", last modified: Wed Jul 26 11:18:12 2023, max compression
+gzip compressed data, was "Warg-1.1.8.tar", last modified: Tue Aug  1 06:11:34 2023, max compression
```

## Comparing `Warg-1.1.7.tar` & `Warg-1.1.8.tar`

### file list

```diff
@@ -1,130 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.149507 Warg-1.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.133507 Warg-1.1.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-26 11:18:05.000000 Warg-1.1.7/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:05.000000 Warg-1.1.7/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 11:18:05.000000 Warg-1.1.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 11:18:05.000000 Warg-1.1.7/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-07-26 11:18:05.000000 Warg-1.1.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-26 11:18:05.000000 Warg-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-26 11:18:12.149507 Warg-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-26 11:18:05.000000 Warg-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-26 11:18:05.000000 Warg-1.1.7/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.133507 Warg-1.1.7/Warg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-07-26 11:18:12.000000 Warg-1.1.7/Warg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-07-26 11:18:12.000000 Warg-1.1.7/Warg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:18:12.000000 Warg-1.1.7/Warg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-26 11:18:12.000000 Warg-1.1.7/Warg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 11:18:12.000000 Warg-1.1.7/Warg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.137507 Warg-1.1.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 11:18:05.000000 Warg-1.1.7/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-26 11:18:05.000000 Warg-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-26 11:18:05.000000 Warg-1.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-26 11:18:12.149507 Warg-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-07-26 11:18:05.000000 Warg-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.137507 Warg-1.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_ast_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_auto_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_collective.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_gdkc.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_nod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_post_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-26 11:18:05.000000 Warg-1.1.7/tests/test_singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.141507 Warg-1.1.7/warg/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.141507 Warg-1.1.7/warg/ast_ops/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/ast_ops/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/ast_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/ast_ops/arg_indentifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/ast_ops/first_arg_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.141507 Warg-1.1.7/warg/bases/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/bases/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/bases/property_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/boolean_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/business.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.141507 Warg-1.1.7/warg/colors/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/colors/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/colors/color_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/colors/css_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/colors/label_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/config_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/context_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/contexts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.141507 Warg-1.1.7/warg/data_structures/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/auto_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16665 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/named_ordered_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/ordered_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/data_structures/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/datetimes.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.145507 Warg-1.1.7/warg/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.145507 Warg-1.1.7/warg/decorators/caching/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/caching/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/caching/look_up_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/caching/property_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/exporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/kw_passing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/decorators/wrapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/gdkc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.145507 Warg-1.1.7/warg/generators/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/cyclic_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/mapping_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/generators/zipping_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/map_itertools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.145507 Warg-1.1.7/warg/math_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/math_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/math_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/math_utilities/multiples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/math_utilities/ordinals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/math_utilities/powers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.145507 Warg-1.1.7/warg/metas/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/metas/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/metas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/metas/post_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/metas/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.149507 Warg-1.1.7/warg/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/mixins/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/mixins/dict_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/mixins/ordinal_index_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/mixins/private.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/ode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:18:12.149507 Warg-1.1.7/warg/os_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/os_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/path_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/path_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/os_utilities/platform_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/replication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/styling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-26 11:18:05.000000 Warg-1.1.7/warg/typing_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.234342 Warg-1.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.218341 Warg-1.1.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-08-01 06:11:28.000000 Warg-1.1.8/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:28.000000 Warg-1.1.8/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 06:11:28.000000 Warg-1.1.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 06:11:28.000000 Warg-1.1.8/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-08-01 06:11:28.000000 Warg-1.1.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-01 06:11:28.000000 Warg-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-08-01 06:11:34.234342 Warg-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-08-01 06:11:28.000000 Warg-1.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-01 06:11:28.000000 Warg-1.1.8/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.218341 Warg-1.1.8/Warg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-08-01 06:11:34.000000 Warg-1.1.8/Warg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-08-01 06:11:34.000000 Warg-1.1.8/Warg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 06:11:34.000000 Warg-1.1.8/Warg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-01 06:11:34.000000 Warg-1.1.8/Warg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-01 06:11:34.000000 Warg-1.1.8/Warg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.218341 Warg-1.1.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-01 06:11:28.000000 Warg-1.1.8/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-08-01 06:11:28.000000 Warg-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-01 06:11:28.000000 Warg-1.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-01 06:11:34.234342 Warg-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-08-01 06:11:28.000000 Warg-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.222341 Warg-1.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_ast_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_auto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_gdkc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11725 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_nod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_post_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-01 06:11:28.000000 Warg-1.1.8/tests/test_singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.222341 Warg-1.1.8/warg/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.226342 Warg-1.1.8/warg/ast_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/ast_ops/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/ast_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/ast_ops/arg_indentifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/ast_ops/first_arg_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.226342 Warg-1.1.8/warg/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/bases/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/bases/property_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/boolean_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/business.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.226342 Warg-1.1.8/warg/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/colors/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/colors/color_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/colors/css_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/colors/label_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/config_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/context_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/contexts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.226342 Warg-1.1.8/warg/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/auto_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16665 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/named_ordered_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28783 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/ordered_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/data_structures/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/datetimes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.226342 Warg-1.1.8/warg/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.230342 Warg-1.1.8/warg/decorators/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/caching/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/caching/look_up_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/caching/property_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/exporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/kw_passing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/decorators/wrapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/gdkc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.230342 Warg-1.1.8/warg/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/cyclic_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/mapping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/generators/zipping_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/map_itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.230342 Warg-1.1.8/warg/math_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/math_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/math_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/math_utilities/multiples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/math_utilities/ordinals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/math_utilities/powers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.230342 Warg-1.1.8/warg/metas/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/metas/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/metas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/metas/post_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/metas/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.230342 Warg-1.1.8/warg/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/mixins/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/mixins/dict_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/mixins/ordinal_index_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/mixins/private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/ode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.234342 Warg-1.1.8/warg/os_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/os_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/path_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/path_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/os_utilities/platform_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 06:11:34.234342 Warg-1.1.8/warg/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/packages/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/packages/editable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/packages/pip_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10270 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/packages/reloading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-01 06:11:28.000000 Warg-1.1.8/warg/typing_extension.py
```

### Comparing `Warg-1.1.7/.github/CODE_OF_CONDUCT.md` & `Warg-1.1.8/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/LICENSE.md` & `Warg-1.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/PKG-INFO` & `Warg-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.1.7
+Version: 1.1.8
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
```

### Comparing `Warg-1.1.7/README.md` & `Warg-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/SECURITY.md` & `Warg-1.1.8/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/Warg.egg-info/PKG-INFO` & `Warg-1.1.8/Warg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Warg
-Version: 1.1.7
+Version: 1.1.8
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/warg
 Download-URL: https://github.com/pything/warg/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
```

### Comparing `Warg-1.1.7/Warg.egg-info/SOURCES.txt` & `Warg-1.1.8/Warg.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -37,19 +37,17 @@
 warg/context_wrapper.py
 warg/contexts.py
 warg/datetimes.py
 warg/debug.py
 warg/exceptions.py
 warg/functions.py
 warg/gdkc.py
-warg/importing.py
 warg/manipulation.py
 warg/map_itertools.py
 warg/ode.py
-warg/packages.py
 warg/plugin.py
 warg/replication.py
 warg/strings.py
 warg/styling.py
 warg/text.py
 warg/typing_extension.py
 warg/ast_ops/README.md
@@ -105,8 +103,13 @@
 warg/mixins/private.py
 warg/os_utilities/README.md
 warg/os_utilities/__init__.py
 warg/os_utilities/filtering.py
 warg/os_utilities/os_platform.py
 warg/os_utilities/path_functions.py
 warg/os_utilities/path_utilities.py
-warg/os_utilities/platform_selection.py
+warg/os_utilities/platform_selection.py
+warg/packages/README.md
+warg/packages/__init__.py
+warg/packages/editable.py
+warg/packages/pip_parsing.py
+warg/packages/reloading.py
```

### Comparing `Warg-1.1.7/Warg.egg-info/requires.txt` & `Warg-1.1.8/Warg.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 setuptools>=60.9.3
 
 [all]
-apppath
-setuptools>=60.9.3
-pytest-runner
+pytest>=4.3.0
+sphinx
 tox
-black>=18.9b0
 sphinxcontrib-programoutput
-twine>=1.13.0
 pytest-cov>=2.6.1
-sphinx
-wheel>=0.33.0
-coveralls>=1.6.0
 pip>=19.0.3
+coveralls>=1.6.0
+wheel>=0.33.0
+pytest-runner
+setuptools>=60.9.3
+twine>=1.13.0
+black>=18.9b0
+apppath
 warg
-pytest>=4.3.0
 
 [dev]
+pytest>=4.3.0
+sphinx
+tox
+pip>=19.0.3
+warg
+coveralls>=1.6.0
+wheel>=0.33.0
 apppath
-setuptools>=60.9.3
 pytest-runner
-tox
+setuptools>=60.9.3
+twine>=1.13.0
 black>=18.9b0
 sphinxcontrib-programoutput
-twine>=1.13.0
 pytest-cov>=2.6.1
-sphinx
-wheel>=0.33.0
-coveralls>=1.6.0
-pip>=19.0.3
-warg
-pytest>=4.3.0
 
 [docs]
-apppath
-sphinxcontrib-programoutput
 sphinx
+sphinxcontrib-programoutput
+apppath
 warg
 
 [setup]
 pytest-runner
 
 [tests]
+pytest>=4.3.0
 tox
 pytest-cov>=2.6.1
-pytest>=4.3.0
```

### Comparing `Warg-1.1.7/pyproject.toml` & `Warg-1.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/setup.py` & `Warg-1.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/tests/test_arguments.py` & `Warg-1.1.8/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/tests/test_ast_ops.py` & `Warg-1.1.8/tests/test_ast_ops.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/tests/test_auto_dict.py` & `Warg-1.1.8/tests/test_auto_dict.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/tests/test_collective.py` & `Warg-1.1.8/tests/test_collective.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/tests/test_gdkc.py` & `Warg-1.1.8/tests/test_gdkc.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/tests/test_imports.py` & `Warg-1.1.8/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/tests/test_kw_passing.py` & `Warg-1.1.8/tests/test_kw_passing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/tests/test_nod.py` & `Warg-1.1.8/tests/test_nod.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/tests/test_post_init.py` & `Warg-1.1.8/tests/test_post_init.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/tests/test_singleton.py` & `Warg-1.1.8/tests/test_singleton.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/__init__.py` & `Warg-1.1.8/warg/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-
+from importlib import resources
+from importlib.metadata import Distribution, PackageNotFoundError
 from warnings import warn
 
-import pkg_resources
-
 __project__ = "Warg"
 
 __author__ = "Christian Heider Nielsen"
-__version__ = "1.1.7"
+__version__ = "1.1.8"
 __doc__ = r"""
 Created on 27/04/2019
 
 @author: cnheider
 
 """
 
 from pathlib import Path
 
+
 with open(Path(__file__).parent / "README.md", "r") as this_init_file:
     __doc__ += this_init_file.read()
 # del Path
 
 # with open(Path(__file__).parent.parent / "README.md", "r") as this_init_file:
 #    __doc__ += this_init_file.read()
 
@@ -40,15 +40,14 @@
     from .metas import *
     from .bases import *
     from .typing_extension import *
     from .context_wrapper import *
     from .boolean_tests import *
     from .map_itertools import *
     from .ast_ops import *
-    from .importing import *
     from .functions import *
     from .os_utilities import *
     from .generators import *
     from .text import *
     from .math_utilities import *
     from .business import *
     from .datetimes import *
@@ -78,49 +77,53 @@
 PROJECT_ORGANISATION = "pything"
 
 __url__ = f"https://github.com/{PROJECT_ORGANISATION}/{PROJECT_NAME}"
 
 # from apppath import AppPath # CAREFUL CIRCULAR DEPENDENCY WARNING!
 # PROJECT_APP_PATH = AppPath(app_name=PROJECT_NAME, app_author=PROJECT_AUTHOR) # NOT USED!
 
-distributions = {v.key: v for v in pkg_resources.working_set}
-if PROJECT_NAME in distributions:
-    distribution = distributions[PROJECT_NAME]
-    DEVELOP = dist_is_editable(distribution)
-else:
+PACKAGE_DATA_PATH = resources.files(PROJECT_NAME) / "data"
+
+try:
+    DEVELOP = package_is_editable(PROJECT_NAME)
+except PackageNotFoundError as e:
     DEVELOP = True
 
 
 def get_version(append_time: Any = DEVELOP) -> str:
-    """description"""
+    """
+
+    :param append_time:
+    :return:
+    """
     import datetime
     import os
 
     version = __version__
     if not version:
         version = os.getenv("VERSION", "0.0.0")
 
     if append_time:
         now = datetime.datetime.utcnow()
         date_version = now.strftime("%Y%m%d%H%M%S")
         # date_version = time.time()
 
         if version:
             # Most git tags are prefixed with 'v' (example: v1.2.3) this is
-            # never desirable for artifact repositories, so we strip the
+            # never desirable for artefact repositories, so we strip the
             # leading 'v' if it's present.
             version = version[1:] if isinstance(version, str) and version.startswith("v") else version
         else:
-            # Default version is an ISO8601 compliant datetime. PyPI doesn't allow
+            # The Default version is an ISO8601 compliant datetime. PyPI doesn't allow
             # the colon ':' character in its versions, and time is required to allow
             # for multiple publications to master in one day. This datetime string
             # uses the 'basic' ISO8601 format for both its date and time components
             # to avoid issues with the colon character (ISO requires that date and
             # time components of a date-time string must be uniformly basic or
-            # extended, which is why the date component does not have dashes.
+            # extended, which is why the date component does not have dashes.)
             #
             # Publications using datetime versions should only be made from master
             # to represent the HEAD moving forward.
             warn(f"Environment variable VERSION is not set, only using datetime: {date_version}")
 
             # warn(f'Environment variable VERSION is not set, only using timestamp: {version}')
 
@@ -129,7 +132,11 @@
     return version
 
 
 if __version__ is None:
     __version__ = get_version(append_time=True)
 
 __version_info__ = tuple(int(segment) for segment in __version__.split("."))
+
+
+if __name__ == "__main__":
+    print(__version__)
```

### Comparing `Warg-1.1.7/warg/arguments.py` & `Warg-1.1.8/warg/arguments.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/ast_ops/arg_indentifier.py` & `Warg-1.1.8/warg/ast_ops/arg_indentifier.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/ast_ops/first_arg_identifier.py` & `Warg-1.1.8/warg/ast_ops/first_arg_identifier.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/bases/property_settings.py` & `Warg-1.1.8/warg/bases/property_settings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/boolean_tests.py` & `Warg-1.1.8/warg/boolean_tests.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/business.py` & `Warg-1.1.8/warg/business.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/colors/color_conversion.py` & `Warg-1.1.8/warg/colors/color_conversion.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/colors/css_colors.py` & `Warg-1.1.8/warg/colors/css_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/colors/label_colors.py` & `Warg-1.1.8/warg/colors/label_colors.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/config_shell.py` & `Warg-1.1.8/warg/config_shell.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/context_wrapper.py` & `Warg-1.1.8/warg/context_wrapper.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/contexts.py` & `Warg-1.1.8/warg/contexts.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/data_structures/auto_dict.py` & `Warg-1.1.8/warg/data_structures/auto_dict.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/data_structures/mappings.py` & `Warg-1.1.8/warg/data_structures/mappings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/data_structures/named_ordered_dictionary.py` & `Warg-1.1.8/warg/data_structures/named_ordered_dictionary.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/data_structures/ordered_set.py` & `Warg-1.1.8/warg/data_structures/ordered_set.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/data_structures/sequences.py` & `Warg-1.1.8/warg/data_structures/sequences.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/datetimes.py` & `Warg-1.1.8/warg/datetimes.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/debug.py` & `Warg-1.1.8/warg/debug.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/decorators/caching/look_up_table.py` & `Warg-1.1.8/warg/decorators/caching/look_up_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 __doc__ = r"""
           Automatically generates a look up data
 
            Created on 06/03/2020
            """
 
 from time import sleep, time
-from typing import Iterable, Mapping, Set, Tuple, Sequence, MutableMapping, Any, Callable
+from typing import (
+    Iterable,
+    Mapping,
+    Set,
+    Tuple,
+    Sequence,
+    MutableMapping,
+    Any,
+    Callable,
+)
 
 from warg.decorators.hashing import make_hash
 
 global_table = {}
 
 __all__ = ["add_lut", "look_up", "look_up_args", "look_up_kws"]
```

### Comparing `Warg-1.1.7/warg/decorators/caching/property_caching.py` & `Warg-1.1.8/warg/decorators/caching/property_caching.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/decorators/exporting.py` & `Warg-1.1.8/warg/decorators/exporting.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/decorators/hashing.py` & `Warg-1.1.8/warg/decorators/hashing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/decorators/kw_passing.py` & `Warg-1.1.8/warg/decorators/kw_passing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/decorators/timing.py` & `Warg-1.1.8/warg/decorators/timing.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/decorators/wrapping.py` & `Warg-1.1.8/warg/decorators/wrapping.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/exceptions.py` & `Warg-1.1.8/warg/exceptions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/functions.py` & `Warg-1.1.8/warg/functions.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/gdkc.py` & `Warg-1.1.8/warg/gdkc.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/generators/cyclic_generators.py` & `Warg-1.1.8/warg/generators/cyclic_generators.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/generators/filtering.py` & `Warg-1.1.8/warg/generators/filtering.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/generators/mapping_generator.py` & `Warg-1.1.8/warg/generators/mapping_generator.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/generators/numbers.py` & `Warg-1.1.8/warg/generators/numbers.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/generators/zipping_generator.py` & `Warg-1.1.8/warg/generators/zipping_generator.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/importing.py` & `Warg-1.1.8/warg/packages/reloading.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 import sys
 from importlib import reload
 from importlib.util import find_spec
 from pathlib import Path
 from typing import Optional, Any, Union, List, Iterable, Callable
 from warnings import warn
 
-import pkg_resources
 
-from warg import passes_kws_to
+from warg.packages import get_requirements_from_file
+from warg.decorators import passes_kws_to
 
 """
 PRELOADED_MODULES = set()
 def init():
   # local imports to keep things neat
   from sys import modules
 
@@ -90,17 +90,16 @@
 def reload_requirements(requirements_path: Path, containment_test: Callable = contain) -> None:
     """
 
     :param requirements_path:
     :param containment_test:
     :return:
     """
-    with open(requirements_path) as f:
-        for r in pkg_resources.parse_requirements(f.readlines()):
-            reload_module(r.project_name, containment_test=containment_test)
+    for r in get_requirements_from_file(requirements_path):
+        reload_module(r.name, containment_test=containment_test)
 
 
 def reload_all_modules(catch_exceptions: bool = True, verbose: bool = True) -> None:
     """
 
     :param catch_exceptions:
     :param verbose:
@@ -183,15 +182,15 @@
             yield from walk_down(q, max_descent=max_descent - 1 if max_descent else None)
         except:
             yield
 
 
 def find_ancestral_relatives(
     target: Union[str, Path],
-    context: Path,  # = Path.cwd(),
+    context: Path = Path.cwd(),
     *,
     from_parent_of_context: bool = True,
     ancestral_levels: int = 2,
     descendant_levels: int = 2,
     top_level: Path = None,
     return_parent_of_target: bool = True,
     no_duplicates: bool = True,
@@ -412,13 +411,13 @@
 
         s = deepcopy(sys.path)
         clean_sys_path()
         s2 = sys.path
         print(s == s2, set(s2) - set(s), set(s) - set(s2), s2)
 
     def asuhdsaud():
-        print(find_ancestral_relatives("queues"))
+        print(find_ancestral_relatives("queues", context=__file__))
 
     # _main()
     # aisjdi()
     # iajsd()
     asuhdsaud()
```

### Comparing `Warg-1.1.7/warg/manipulation.py` & `Warg-1.1.8/warg/manipulation.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/map_itertools.py` & `Warg-1.1.8/warg/map_itertools.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/math_utilities/ordinals.py` & `Warg-1.1.8/warg/math_utilities/ordinals.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/math_utilities/powers.py` & `Warg-1.1.8/warg/math_utilities/powers.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/metas/post_init.py` & `Warg-1.1.8/warg/metas/post_init.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/metas/singleton.py` & `Warg-1.1.8/warg/metas/singleton.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/mixins/dict_mixins.py` & `Warg-1.1.8/warg/mixins/dict_mixins.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/mixins/ordinal_index_mixin.py` & `Warg-1.1.8/warg/mixins/ordinal_index_mixin.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/ode.py` & `Warg-1.1.8/warg/ode.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/os_utilities/filtering.py` & `Warg-1.1.8/warg/os_utilities/filtering.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/os_utilities/os_platform.py` & `Warg-1.1.8/warg/os_utilities/os_platform.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/os_utilities/path_functions.py` & `Warg-1.1.8/warg/os_utilities/path_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
 
            Created on 08/03/2020
            """
 
-__all__ = ["ensure_existence", "path_rmtree", "sanitise_path", "path_join", "keep_last_n_modified"]
+__all__ = [
+    "ensure_existence",
+    "path_rmtree",
+    "sanitise_path",
+    "path_join",
+    "keep_last_n_modified",
+]
 
 import collections
 import os
 from itertools import cycle
 from pathlib import Path
 
 from typing import Iterable, Union, Callable
@@ -157,15 +163,19 @@
                 out.mkdir(parents=True, exist_ok=True)
 
     return out
 
 
 # @passes_kws_to(rmtree)
 def keep_last_n_modified(
-    directory: Union[Path, str], n: int, only_directories: bool = False, only_files: bool = False, **kwargs
+    directory: Union[Path, str],
+    n: int,
+    only_directories: bool = False,
+    only_files: bool = False,
+    **kwargs,
 ):
     directory = Path(directory)
     from shutil import rmtree
 
     assert not (only_files and only_directories)  # Ensure that only of them is True or both are False
 
     timeline = {}
```

### Comparing `Warg-1.1.7/warg/os_utilities/path_utilities.py` & `Warg-1.1.8/warg/os_utilities/path_utilities.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/os_utilities/platform_selection.py` & `Warg-1.1.8/warg/os_utilities/platform_selection.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/plugin.py` & `Warg-1.1.8/warg/plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 __author__ = "Christian Heider Nielsen"
 __doc__ = r"""
           Plugin
 
            Created on 13/06/2020
            """
 
-from typing import Tuple
-
-import pkg_resources
+from importlib.metadata import entry_points, EntryPoint
+from typing import Tuple, Any, Generator, Union
 
 __all__ = ["get_plugins", "get_static_plugins", "get_dynamic_plugins"]
 
 
 def get_plugins(package_name: str) -> Tuple:
     """Returns a list specifying all known plugins.
 
@@ -37,24 +36,26 @@
     """
     v = f"{package_name.upper()}_PLUGINS"
     if v in globals():
         return globals()[v][:]
     return ()
 
 
-def get_dynamic_plugins(package_name: str) -> Tuple:
-    """Returns a list specifying  dynamically loaded plugins.
+def get_dynamic_plugins(
+    package_name: str,
+) -> Generator[Union[str, EntryPoint], Any, None]:
+    """Returns a list specifying dynamically loaded plugins.
 
     Returns:
       The list of dynamic plugins.
 
     [1]: https://packaging.python.org/specifications/entry-points/
     """
 
     # .load() method to import and load that entry point (module or object).
     # from importlib import metadata # new method!
     # return [      entry_point.load()      for entry_point in metadata.entry_points()[f'{package_name}_plugins']      ]
-    return (entry_point.load() for entry_point in pkg_resources.iter_entry_points(f"{package_name}_plugins"))
+    return (entry_point for entry_point in entry_points(group="console_scripts", name=package_name))
 
 
 if __name__ == "__main__":
     print(get_plugins("warg"))
```

### Comparing `Warg-1.1.7/warg/replication.py` & `Warg-1.1.8/warg/replication.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/strings.py` & `Warg-1.1.8/warg/strings.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/styling.py` & `Warg-1.1.8/warg/styling.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/text.py` & `Warg-1.1.8/warg/text.py`

 * *Files identical despite different names*

### Comparing `Warg-1.1.7/warg/typing_extension.py` & `Warg-1.1.8/warg/typing_extension.py`

 * *Files identical despite different names*

