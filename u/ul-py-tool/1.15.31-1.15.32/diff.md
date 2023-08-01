# Comparing `tmp/ul-py-tool-1.15.31.tar.gz` & `tmp/ul-py-tool-1.15.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-py-tool-1.15.31.tar", last modified: Tue Aug  1 08:23:19 2023, max compression
+gzip compressed data, was "ul-py-tool-1.15.32.tar", last modified: Tue Aug  1 08:55:38 2023, max compression
```

## Comparing `ul-py-tool-1.15.31.tar` & `ul-py-tool-1.15.32.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:23:19.962149 ul-py-tool-1.15.31/
--rw-r--r--   0 root         (0) root         (0)     3122 2023-08-01 08:23:19.962149 ul-py-tool-1.15.31/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2468 2023-04-18 09:10:48.000000 ul-py-tool-1.15.31/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 08:23:19.962149 ul-py-tool-1.15.31/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2508 2023-08-01 08:23:18.000000 ul-py-tool-1.15.31/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:23:19.882146 ul-py-tool-1.15.31/ul_py_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-18 08:37:40.000000 ul-py-tool-1.15.31/ul_py_tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:23:19.886147 ul-py-tool-1.15.31/ul_py_tool/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-10 10:03:09.000000 ul-py-tool-1.15.31/ul_py_tool/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       54 2022-08-10 10:03:09.000000 ul-py-tool-1.15.31/ul_py_tool/__tests__/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:23:19.914147 ul-py-tool-1.15.31/ul_py_tool/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-18 08:37:40.000000 ul-py-tool-1.15.31/ul_py_tool/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2515 2022-11-05 23:50:06.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmd.py
--rw-rw-rw-   0 root         (0) root         (0)     5321 2023-06-14 12:13:10.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmd_build_images.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2022-11-05 23:50:06.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmd_cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2022-11-05 23:50:06.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmd_fix_own.py
--rw-rw-rw-   0 root         (0) root         (0)     2463 2022-08-11 15:10:30.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmd_fmt.py
--rw-rw-rw-   0 root         (0) root         (0)     2856 2022-08-10 10:03:09.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmd_install.py
--rw-rw-rw-   0 root         (0) root         (0)    33461 2023-06-14 12:13:10.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmd_lint.py
--rw-rw-rw-   0 root         (0) root         (0)    10047 2023-07-31 11:02:29.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmd_release.py
--rw-rw-rw-   0 root         (0) root         (0)     7381 2023-08-01 08:23:18.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmd_release_dcf.py
--rw-rw-rw-   0 root         (0) root         (0)     3098 2022-08-05 17:24:42.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmd_stats.py
--rw-rw-rw-   0 root         (0) root         (0)     3597 2022-11-05 23:50:06.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmd_test.py
--rw-rw-rw-   0 root         (0) root         (0)     5475 2023-04-18 09:10:48.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmd_test_secrets.py
--rw-rw-rw-   0 root         (0) root         (0)     6001 2022-10-27 16:00:56.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmd_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2022-08-10 10:03:09.000000 ul-py-tool-1.15.31/ul_py_tool/commands/cmp_outdated.py
--rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-03 15:03:17.000000 ul-py-tool-1.15.31/ul_py_tool/commands/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:23:19.942149 ul-py-tool-1.15.31/ul_py_tool/conf/
--rw-rw-rw-   0 root         (0) root         (0)      458 2022-01-18 08:37:40.000000 ul-py-tool-1.15.31/ul_py_tool/conf/editorconfig
--rw-rw-rw-   0 root         (0) root         (0)      284 2022-01-18 08:37:40.000000 ul-py-tool-1.15.31/ul_py_tool/conf/git.hook.pre-commit.sh
--rw-rw-rw-   0 root         (0) root         (0)      298 2022-01-18 08:37:40.000000 ul-py-tool-1.15.31/ul_py_tool/conf/git.hook.pre-push.sh
--rw-rw-rw-   0 root         (0) root         (0)       37 2022-01-18 08:37:40.000000 ul-py-tool-1.15.31/ul_py_tool/conf/gitattributes
--rw-rw-rw-   0 root         (0) root         (0)     1788 2022-01-18 08:37:40.000000 ul-py-tool-1.15.31/ul_py_tool/conf/gitignore
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-08-03 16:13:25.000000 ul-py-tool-1.15.31/ul_py_tool/conf/isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1036 2022-08-05 17:24:42.000000 ul-py-tool-1.15.31/ul_py_tool/conf/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-07-26 13:02:36.000000 ul-py-tool-1.15.31/ul_py_tool/conf/pytest.ini
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-08-04 17:42:28.000000 ul-py-tool-1.15.31/ul_py_tool/conf/python-version
--rw-rw-rw-   0 root         (0) root         (0)      532 2022-08-05 17:24:42.000000 ul-py-tool-1.15.31/ul_py_tool/conf/yamlint.yml
--rw-rw-rw-   0 root         (0) root         (0)     1237 2023-07-31 11:02:29.000000 ul-py-tool-1.15.31/ul_py_tool/main.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-26 13:02:36.000000 ul-py-tool-1.15.31/ul_py_tool/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:23:19.962149 ul-py-tool-1.15.31/ul_py_tool/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-18 08:37:40.000000 ul-py-tool-1.15.31/ul_py_tool/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:23:19.962149 ul-py-tool-1.15.31/ul_py_tool/utils/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-05 23:50:06.000000 ul-py-tool-1.15.31/ul_py_tool/utils/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2022-11-06 00:17:56.000000 ul-py-tool-1.15.31/ul_py_tool/utils/__tests__/pipfile.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2022-07-22 15:16:04.000000 ul-py-tool-1.15.31/ul_py_tool/utils/arg_file_exists.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2022-08-11 15:10:30.000000 ul-py-tool-1.15.31/ul_py_tool/utils/arg_files_glob.py
--rw-rw-rw-   0 root         (0) root         (0)      374 2022-08-03 16:13:25.000000 ul-py-tool-1.15.31/ul_py_tool/utils/arg_str2bool.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2022-10-27 16:00:56.000000 ul-py-tool-1.15.31/ul_py_tool/utils/arg_str2list.py
--rw-rw-rw-   0 root         (0) root         (0)      603 2022-08-03 16:13:25.000000 ul-py-tool-1.15.31/ul_py_tool/utils/arg_str2yaml.py
--rw-rw-rw-   0 root         (0) root         (0)      496 2023-04-03 15:03:17.000000 ul-py-tool-1.15.31/ul_py_tool/utils/aseembly.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2022-08-04 17:42:28.000000 ul-py-tool-1.15.31/ul_py_tool/utils/colors.py
--rw-rw-rw-   0 root         (0) root         (0)     4909 2023-08-01 08:23:18.000000 ul-py-tool-1.15.31/ul_py_tool/utils/docker_compose.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2022-10-27 16:00:56.000000 ul-py-tool-1.15.31/ul_py_tool/utils/docker_file.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2022-01-18 08:37:40.000000 ul-py-tool-1.15.31/ul_py_tool/utils/fs.py
--rw-rw-rw-   0 root         (0) root         (0)      324 2022-08-04 10:20:20.000000 ul-py-tool-1.15.31/ul_py_tool/utils/input_lines.py
--rw-rw-rw-   0 root         (0) root         (0)     9717 2022-11-06 00:17:56.000000 ul-py-tool-1.15.31/ul_py_tool/utils/pipfile.py
--rw-rw-rw-   0 root         (0) root         (0)     3671 2022-08-03 16:13:25.000000 ul-py-tool-1.15.31/ul_py_tool/utils/run_command.py
--rw-rw-rw-   0 root         (0) root         (0)     5622 2022-08-06 11:31:24.000000 ul-py-tool-1.15.31/ul_py_tool/utils/semver.py
--rw-rw-rw-   0 root         (0) root         (0)     5927 2022-11-06 00:17:56.000000 ul-py-tool-1.15.31/ul_py_tool/utils/step.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2022-01-18 08:37:40.000000 ul-py-tool-1.15.31/ul_py_tool/utils/write_stdout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:23:19.882146 ul-py-tool-1.15.31/ul_py_tool.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3122 2023-08-01 08:23:19.000000 ul-py-tool-1.15.31/ul_py_tool.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1794 2023-08-01 08:23:19.000000 ul-py-tool-1.15.31/ul_py_tool.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 08:23:19.000000 ul-py-tool-1.15.31/ul_py_tool.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-08-01 08:23:19.000000 ul-py-tool-1.15.31/ul_py_tool.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      745 2023-08-01 08:23:19.000000 ul-py-tool-1.15.31/ul_py_tool.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-08-01 08:23:19.000000 ul-py-tool-1.15.31/ul_py_tool.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:55:38.252968 ul-py-tool-1.15.32/
+-rw-r--r--   0 root         (0) root         (0)     3122 2023-08-01 08:55:38.252968 ul-py-tool-1.15.32/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2468 2023-04-18 09:10:48.000000 ul-py-tool-1.15.32/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 08:55:38.252968 ul-py-tool-1.15.32/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2023-08-01 08:55:36.000000 ul-py-tool-1.15.32/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:55:38.144964 ul-py-tool-1.15.32/ul_py_tool/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-18 08:37:40.000000 ul-py-tool-1.15.32/ul_py_tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:55:38.144964 ul-py-tool-1.15.32/ul_py_tool/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-10 10:03:09.000000 ul-py-tool-1.15.32/ul_py_tool/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       54 2022-08-10 10:03:09.000000 ul-py-tool-1.15.32/ul_py_tool/__tests__/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:55:38.188965 ul-py-tool-1.15.32/ul_py_tool/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-18 08:37:40.000000 ul-py-tool-1.15.32/ul_py_tool/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2022-11-05 23:50:06.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmd.py
+-rw-rw-rw-   0 root         (0) root         (0)     5321 2023-06-14 12:13:10.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmd_build_images.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2022-11-05 23:50:06.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmd_cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2022-11-05 23:50:06.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmd_fix_own.py
+-rw-rw-rw-   0 root         (0) root         (0)     2463 2022-08-11 15:10:30.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmd_fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2856 2022-08-10 10:03:09.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmd_install.py
+-rw-rw-rw-   0 root         (0) root         (0)    33461 2023-06-14 12:13:10.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmd_lint.py
+-rw-rw-rw-   0 root         (0) root         (0)    10047 2023-07-31 11:02:29.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmd_release.py
+-rw-rw-rw-   0 root         (0) root         (0)     7381 2023-08-01 08:23:18.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmd_release_dcf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3098 2022-08-05 17:24:42.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmd_stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     3597 2022-11-05 23:50:06.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmd_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     5475 2023-04-18 09:10:48.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmd_test_secrets.py
+-rw-rw-rw-   0 root         (0) root         (0)     6001 2022-10-27 16:00:56.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmd_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2022-08-10 10:03:09.000000 ul-py-tool-1.15.32/ul_py_tool/commands/cmp_outdated.py
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2023-04-03 15:03:17.000000 ul-py-tool-1.15.32/ul_py_tool/commands/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:55:38.220966 ul-py-tool-1.15.32/ul_py_tool/conf/
+-rw-rw-rw-   0 root         (0) root         (0)      458 2022-01-18 08:37:40.000000 ul-py-tool-1.15.32/ul_py_tool/conf/editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      284 2022-01-18 08:37:40.000000 ul-py-tool-1.15.32/ul_py_tool/conf/git.hook.pre-commit.sh
+-rw-rw-rw-   0 root         (0) root         (0)      298 2022-01-18 08:37:40.000000 ul-py-tool-1.15.32/ul_py_tool/conf/git.hook.pre-push.sh
+-rw-rw-rw-   0 root         (0) root         (0)       37 2022-01-18 08:37:40.000000 ul-py-tool-1.15.32/ul_py_tool/conf/gitattributes
+-rw-rw-rw-   0 root         (0) root         (0)     1788 2022-01-18 08:37:40.000000 ul-py-tool-1.15.32/ul_py_tool/conf/gitignore
+-rw-rw-rw-   0 root         (0) root         (0)       24 2022-08-03 16:13:25.000000 ul-py-tool-1.15.32/ul_py_tool/conf/isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1036 2022-08-05 17:24:42.000000 ul-py-tool-1.15.32/ul_py_tool/conf/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-07-26 13:02:36.000000 ul-py-tool-1.15.32/ul_py_tool/conf/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)        7 2022-08-04 17:42:28.000000 ul-py-tool-1.15.32/ul_py_tool/conf/python-version
+-rw-rw-rw-   0 root         (0) root         (0)      532 2022-08-05 17:24:42.000000 ul-py-tool-1.15.32/ul_py_tool/conf/yamlint.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2023-07-31 11:02:29.000000 ul-py-tool-1.15.32/ul_py_tool/main.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-26 13:02:36.000000 ul-py-tool-1.15.32/ul_py_tool/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:55:38.248968 ul-py-tool-1.15.32/ul_py_tool/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-18 08:37:40.000000 ul-py-tool-1.15.32/ul_py_tool/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:55:38.252968 ul-py-tool-1.15.32/ul_py_tool/utils/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-05 23:50:06.000000 ul-py-tool-1.15.32/ul_py_tool/utils/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2022-11-06 00:17:56.000000 ul-py-tool-1.15.32/ul_py_tool/utils/__tests__/pipfile.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2022-07-22 15:16:04.000000 ul-py-tool-1.15.32/ul_py_tool/utils/arg_file_exists.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2022-08-11 15:10:30.000000 ul-py-tool-1.15.32/ul_py_tool/utils/arg_files_glob.py
+-rw-rw-rw-   0 root         (0) root         (0)      374 2022-08-03 16:13:25.000000 ul-py-tool-1.15.32/ul_py_tool/utils/arg_str2bool.py
+-rw-rw-rw-   0 root         (0) root         (0)      837 2022-10-27 16:00:56.000000 ul-py-tool-1.15.32/ul_py_tool/utils/arg_str2list.py
+-rw-rw-rw-   0 root         (0) root         (0)      603 2022-08-03 16:13:25.000000 ul-py-tool-1.15.32/ul_py_tool/utils/arg_str2yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-04-03 15:03:17.000000 ul-py-tool-1.15.32/ul_py_tool/utils/aseembly.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2022-08-04 17:42:28.000000 ul-py-tool-1.15.32/ul_py_tool/utils/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4780 2023-08-01 08:55:36.000000 ul-py-tool-1.15.32/ul_py_tool/utils/docker_compose.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2022-10-27 16:00:56.000000 ul-py-tool-1.15.32/ul_py_tool/utils/docker_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2022-01-18 08:37:40.000000 ul-py-tool-1.15.32/ul_py_tool/utils/fs.py
+-rw-rw-rw-   0 root         (0) root         (0)      324 2022-08-04 10:20:20.000000 ul-py-tool-1.15.32/ul_py_tool/utils/input_lines.py
+-rw-rw-rw-   0 root         (0) root         (0)     9717 2022-11-06 00:17:56.000000 ul-py-tool-1.15.32/ul_py_tool/utils/pipfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3671 2022-08-03 16:13:25.000000 ul-py-tool-1.15.32/ul_py_tool/utils/run_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     5622 2022-08-06 11:31:24.000000 ul-py-tool-1.15.32/ul_py_tool/utils/semver.py
+-rw-rw-rw-   0 root         (0) root         (0)     5927 2022-11-06 00:17:56.000000 ul-py-tool-1.15.32/ul_py_tool/utils/step.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2022-01-18 08:37:40.000000 ul-py-tool-1.15.32/ul_py_tool/utils/write_stdout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 08:55:38.144964 ul-py-tool-1.15.32/ul_py_tool.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3122 2023-08-01 08:55:37.000000 ul-py-tool-1.15.32/ul_py_tool.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-08-01 08:55:37.000000 ul-py-tool-1.15.32/ul_py_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 08:55:37.000000 ul-py-tool-1.15.32/ul_py_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-08-01 08:55:37.000000 ul-py-tool-1.15.32/ul_py_tool.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      745 2023-08-01 08:55:37.000000 ul-py-tool-1.15.32/ul_py_tool.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-01 08:55:37.000000 ul-py-tool-1.15.32/ul_py_tool.egg-info/top_level.txt
```

### Comparing `ul-py-tool-1.15.31/PKG-INFO` & `ul-py-tool-1.15.32/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-py-tool
-Version: 1.15.31
+Version: 1.15.32
 Summary: Python ul py tool
 Home-page: https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/ul-py-tool.git
 Author: Unic-lab
 Author-email: 
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-py-tool-1.15.31/README.md` & `ul-py-tool-1.15.32/README.md`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/setup.py` & `ul-py-tool-1.15.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-py-tool',
-    version='1.15.31',
+    version='1.15.32',
     description='Python ul py tool',
     author='Unic-lab',
     author_email='',
     url='https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/ul-py-tool.git',
     packages=find_packages(include=['ul_py_tool*']),
     platforms='any',
     package_data={
```

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/cmd.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/cmd.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/cmd_build_images.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/cmd_build_images.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/cmd_cleanup.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/cmd_cleanup.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/cmd_fmt.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/cmd_fmt.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/cmd_install.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/cmd_install.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/cmd_lint.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/cmd_lint.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/cmd_release.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/cmd_release.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/cmd_release_dcf.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/cmd_release_dcf.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/cmd_stats.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/cmd_stats.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/cmd_test.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/cmd_test.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/cmd_test_secrets.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/cmd_test_secrets.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/cmd_version.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/cmd_version.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/cmp_outdated.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/cmp_outdated.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/commands/conf.py` & `ul-py-tool-1.15.32/ul_py_tool/commands/conf.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/conf/gitignore` & `ul-py-tool-1.15.32/ul_py_tool/conf/gitignore`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/conf/mypy.ini` & `ul-py-tool-1.15.32/ul_py_tool/conf/mypy.ini`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/conf/yamlint.yml` & `ul-py-tool-1.15.32/ul_py_tool/conf/yamlint.yml`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/main.py` & `ul-py-tool-1.15.32/ul_py_tool/main.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/utils/__tests__/pipfile.py` & `ul-py-tool-1.15.32/ul_py_tool/utils/__tests__/pipfile.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/utils/arg_files_glob.py` & `ul-py-tool-1.15.32/ul_py_tool/utils/arg_files_glob.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/utils/arg_str2list.py` & `ul-py-tool-1.15.32/ul_py_tool/utils/arg_str2list.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/utils/arg_str2yaml.py` & `ul-py-tool-1.15.32/ul_py_tool/utils/arg_str2yaml.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/utils/docker_compose.py` & `ul-py-tool-1.15.32/ul_py_tool/utils/docker_compose.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 class DockerComposeFile(BaseModel):
     volumes: Dict[str, None]
     common_dependencies: List[str]
     version: str
     services: List[DockerComposeService]
 
     @staticmethod
-    def from_kubernetes(file: Iterable[Dict[str, Any]]) -> 'DockerComposeFile':  # Missing type parameters for generic type "Iterable" help me
+    def from_kubernetes(file: Iterable[Dict[str, Any]]) -> 'DockerComposeFile':
         volumes_list: Dict[str, None] = {}
         services_list: List[DockerComposeService] = []
         common_dependencies: List[str] = []
         for resource in file:
             if resource['kind'] not in KUBERNETES_OBJECTS__TRANSFORM_TO_DCF__TYPE:
                 continue
             service, volumes = DockerComposeService.from_kubernetes(resource)
@@ -99,14 +99,13 @@
 
     def to_json(self) -> Dict[str, Any]:
         services_dict: Dict[str, Any] = {}
         for service in self.services:
             service_json = service.to_json(
                 common_dependencies=self.common_dependencies if service.kubernetes_type not in KUBERNETES_OBJECTS__DEPENDS_ON_OBJECT__TYPE else [],
             )
-            service_json['depends_on'] = self.common_dependencies
             services_dict.update(**service_json)
         return {
             "version": "3.8",
             "volumes": self.volumes,
             "services": services_dict,
         }
```

### Comparing `ul-py-tool-1.15.31/ul_py_tool/utils/docker_file.py` & `ul-py-tool-1.15.32/ul_py_tool/utils/docker_file.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/utils/pipfile.py` & `ul-py-tool-1.15.32/ul_py_tool/utils/pipfile.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/utils/run_command.py` & `ul-py-tool-1.15.32/ul_py_tool/utils/run_command.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/utils/semver.py` & `ul-py-tool-1.15.32/ul_py_tool/utils/semver.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool/utils/step.py` & `ul-py-tool-1.15.32/ul_py_tool/utils/step.py`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool.egg-info/PKG-INFO` & `ul-py-tool-1.15.32/ul_py_tool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-py-tool
-Version: 1.15.31
+Version: 1.15.32
 Summary: Python ul py tool
 Home-page: https://gitlab.neroelectronics.by/unic-lab/libraries/common-python-utils/ul-py-tool.git
 Author: Unic-lab
 Author-email: 
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-py-tool-1.15.31/ul_py_tool.egg-info/SOURCES.txt` & `ul-py-tool-1.15.32/ul_py_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ul-py-tool-1.15.31/ul_py_tool.egg-info/requires.txt` & `ul-py-tool-1.15.32/ul_py_tool.egg-info/requires.txt`

 * *Files identical despite different names*

