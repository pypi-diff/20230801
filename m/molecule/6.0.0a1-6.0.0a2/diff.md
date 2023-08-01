# Comparing `tmp/molecule-6.0.0a1.tar.gz` & `tmp/molecule-6.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule-6.0.0a1.tar", last modified: Tue Jul 25 14:58:37 2023, max compression
+gzip compressed data, was "molecule-6.0.0a2.tar", last modified: Tue Aug  1 12:47:47 2023, max compression
```

## Comparing `molecule-6.0.0a1.tar` & `molecule-6.0.0a2.tar`

### file list

```diff
@@ -1,416 +1,434 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.854848 molecule-6.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.codespellrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.766845 molecule-6.0.0a1/.config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.766845 molecule-6.0.0a1/.config/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/molecule/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/molecule.spec
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/requirements-lock.txt
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.config/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.770846 molecule-6.0.0a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.770846 molecule-6.0.0a1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/patchback.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.774845 molecule-6.0.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/workflows/redirects.yml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.npmrc
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.packit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.774845 molecule-6.0.0a1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-25 14:58:16.000000 molecule-6.0.0a1/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-25 14:58:16.000000 molecule-6.0.0a1/DCO_1_1.md
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-25 14:58:16.000000 molecule-6.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 14:58:16.000000 molecule-6.0.0a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-25 14:58:37.854848 molecule-6.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-25 14:58:16.000000 molecule-6.0.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-25 14:58:16.000000 molecule-6.0.0a1/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-25 14:58:16.000000 molecule-6.0.0a1/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-25 14:58:16.000000 molecule-6.0.0a1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.702844 molecule-6.0.0a1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/_static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/_static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   143898 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/_static/images/logo_big.png
--rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/ci.md
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/google04e29a42ae6e6cbc.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/next.md
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/podman.md
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/redirects.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-25 14:58:16.000000 molecule-6.0.0a1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 14:58:16.000000 molecule-6.0.0a1/linkcheckerrc
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-25 14:58:16.000000 molecule-6.0.0a1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.702844 molecule-6.0.0a1/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/molecule/podman/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/podman/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/podman/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/podman/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/podman/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/podman/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/molecule/podman/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-25 14:58:16.000000 molecule-6.0.0a1/molecule/podman/tasks/create-fail.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-25 14:58:16.000000 molecule-6.0.0a1/playbooks/snap-pre-run.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-07-25 14:58:16.000000 molecule-6.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-25 14:58:16.000000 molecule-6.0.0a1/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:58:37.854848 molecule-6.0.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.782846 molecule-6.0.0a1/snap/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-25 14:58:16.000000 molecule-6.0.0a1/snap/snapcraft.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.706844 molecule-6.0.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.794846 molecule-6.0.0a1/src/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.806846 molecule-6.0.0a1/src/molecule/command/
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/converge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/idempotence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.806846 molecule-6.0.0a1/src/molecule/command/init/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/init/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/init/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/init/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/side_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/command/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.810846 molecule-6.0.0a1/src/molecule/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/driver.json
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/init-scenario.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14472 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/molecule.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.710844 molecule-6.0.0a1/src/molecule/data/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.810846 molecule-6.0.0a1/src/molecule/data/templates/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/templates/scenario/converge.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/templates/scenario/create.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/templates/scenario/destroy.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/data/templates/scenario/molecule.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.814847 molecule-6.0.0a1/src/molecule/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.814847 molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/dependency/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.818847 molecule-6.0.0a1/src/molecule/driver/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/driver/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/driver/delegated.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.818847 molecule-6.0.0a1/src/molecule/model/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/model/schema_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/platforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.818847 molecule-6.0.0a1/src/molecule/provisioner/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/provisioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33606 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/provisioner/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/provisioner/ansible_playbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/provisioner/ansible_playbooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/provisioner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.818847 molecule-6.0.0a1/src/molecule/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.822847 molecule-6.0.0a1/src/molecule/test/a_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/command/init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/init/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_converge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_idempotence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_side_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_syntax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/command/test_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/cookiecutter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/cookiecutter/test_molecule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/ansible_galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/ansible_galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/ansible_galaxy/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/ansible_galaxy/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/dependency/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/driver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/driver/test_delegated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/lint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/lint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.826847 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_dependency_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_driver_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_platforms_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_provisioner_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_scenario_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_verifier_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/test_ansible_playbook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/test_ansible_playbooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_scenarios.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_scenarios_ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/a_unit/verifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/verifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/verifier/test_ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/a_unit/verifier/test_testinfra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/b_functional/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/b_functional/.ansible-lint
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/b_functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/b_functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/b_functional/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/.yamllint
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/invalid_role_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/invalid_role_template/bad_format/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/invalid_role_template/bad_format/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/invalid_role_template/cookiecutter.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/playbooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/roles/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/roles/molecule/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/roles/molecule/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/roles/molecule/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/roles/molecule/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.722844 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/roles/get_rich/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.726844 molecule-6.0.0a1/src/molecule/test/resources/schema_instance_files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/schema_instance_files/invalid/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.830847 molecule-6.0.0a1/src/molecule/test/resources/schema_instance_files/valid/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/resources/schema_instance_files/valid/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.834847 molecule-6.0.0a1/src/molecule/test/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.726844 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.726844 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.834847 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/cleanup.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.834847 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/cleanup/molecule/default/tests/test_cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.726844 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.730844 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.834847 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.834847 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/shell/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/shell/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/dependency/molecule/shell/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.730844 molecule-6.0.0a1/src/molecule/test/scenarios/driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.730844 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.838847 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.730844 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.838847 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.730844 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.838847 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.734845 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.838847 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/destroy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.838847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.734845 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/group_vars/example/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/group_vars/example/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/extra-host
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/instance/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/host_vars/instance/all.yml
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/hosts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.738845 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.734845 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/all.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.738845 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/all.yml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/links/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/links/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/links/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.738845 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.738845 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/molecule/raises/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/molecule/raises/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/molecule/raises/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.842847 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/idempotence/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.742845 molecule-6.0.0a1/src/molecule/test/scenarios/interpolation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.742845 molecule-6.0.0a1/src/molecule/test/scenarios/interpolation/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/interpolation/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/interpolation/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/interpolation/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.742845 molecule-6.0.0a1/src/molecule/test/scenarios/overrride_driver/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.742845 molecule-6.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/overrride_driver/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.742845 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.742845 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/molecule.yml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/side_effect.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/side_effect/molecule/default/tests/test_side_effect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.746845 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.746845 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.846847 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.750845 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.850847 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.850847 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/test_shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.850847 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/test_testinfra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.850847 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.850847 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/test_testinfra_pre_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.850847 molecule-6.0.0a1/src/molecule/verifier/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/verifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/verifier/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/verifier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-25 14:58:16.000000 molecule-6.0.0a1/src/molecule/verifier/testinfra.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.798846 molecule-6.0.0a1/src/molecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 14:58:37.000000 molecule-6.0.0a1/src/molecule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:58:37.854848 molecule-6.0.0a1/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-07-25 14:58:16.000000 molecule-6.0.0a1/tools/get-version.sh
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 14:58:16.000000 molecule-6.0.0a1/tools/opts.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-07-25 14:58:16.000000 molecule-6.0.0a1/tools/smoketest.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-07-25 14:58:16.000000 molecule-6.0.0a1/tools/test-setup.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-07-25 14:58:16.000000 molecule-6.0.0a1/tools/update-version.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-25 14:58:16.000000 molecule-6.0.0a1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.645762 molecule-6.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.codespellrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.557760 molecule-6.0.0a2/.config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.557760 molecule-6.0.0a2/.config/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.config/molecule/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.config/molecule.spec
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.config/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.config/requirements-testinfra.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.557760 molecule-6.0.0a2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.557760 molecule-6.0.0a2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.github/patchback.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.557760 molecule-6.0.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.github/workflows/redirects.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.packit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.557760 molecule-6.0.0a2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-08-01 12:47:31.000000 molecule-6.0.0a2/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-01 12:47:31.000000 molecule-6.0.0a2/DCO_1_1.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-01 12:47:31.000000 molecule-6.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-01 12:47:31.000000 molecule-6.0.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-08-01 12:47:47.641762 molecule-6.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-08-01 12:47:31.000000 molecule-6.0.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-01 12:47:31.000000 molecule-6.0.0a2/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-01 12:47:31.000000 molecule-6.0.0a2/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-08-01 12:47:31.000000 molecule-6.0.0a2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.561761 molecule-6.0.0a2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.525760 molecule-6.0.0a2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.561761 molecule-6.0.0a2/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/_static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/_static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   143898 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/_static/images/logo_big.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10447 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/ci.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/docker.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/google04e29a42ae6e6cbc.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.561761 molecule-6.0.0a2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/kubevirt.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/next.md
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/podman.md
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/redirects.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 12:47:31.000000 molecule-6.0.0a2/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-01 12:47:31.000000 molecule-6.0.0a2/linkcheckerrc
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-08-01 12:47:31.000000 molecule-6.0.0a2/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.525760 molecule-6.0.0a2/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.561761 molecule-6.0.0a2/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.561761 molecule-6.0.0a2/molecule/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/docker/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/docker/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/docker/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/docker/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/docker/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.561761 molecule-6.0.0a2/molecule/docker/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/docker/tasks/create-fail.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.561761 molecule-6.0.0a2/molecule/kubevirt/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/kubevirt/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/kubevirt/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/kubevirt/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/kubevirt/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/kubevirt/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.565760 molecule-6.0.0a2/molecule/kubevirt/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/kubevirt/tasks/create_vm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/kubevirt/tasks/create_vm_dictionary.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.565760 molecule-6.0.0a2/molecule/podman/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/podman/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/podman/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/podman/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/podman/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/podman/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.565760 molecule-6.0.0a2/molecule/podman/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-01 12:47:31.000000 molecule-6.0.0a2/molecule/podman/tasks/create-fail.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.565760 molecule-6.0.0a2/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-08-01 12:47:31.000000 molecule-6.0.0a2/playbooks/snap-pre-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-08-01 12:47:31.000000 molecule-6.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-01 12:47:31.000000 molecule-6.0.0a2/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 12:47:47.645762 molecule-6.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.565760 molecule-6.0.0a2/snap/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-08-01 12:47:31.000000 molecule-6.0.0a2/snap/snapcraft.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.529760 molecule-6.0.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.569761 molecule-6.0.0a2/src/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-01 12:47:47.000000 molecule-6.0.0a2/src/molecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.577761 molecule-6.0.0a2/src/molecule/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/converge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/idempotence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.581761 molecule-6.0.0a2/src/molecule/command/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/init/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/init/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/init/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/side_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/command/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17449 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.581761 molecule-6.0.0a2/src/molecule/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/data/driver.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/data/init-scenario.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14472 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/data/molecule.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.529760 molecule-6.0.0a2/src/molecule/data/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.585761 molecule-6.0.0a2/src/molecule/data/templates/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/data/templates/scenario/converge.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/data/templates/scenario/create.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/data/templates/scenario/destroy.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/data/templates/scenario/molecule.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.585761 molecule-6.0.0a2/src/molecule/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.585761 molecule-6.0.0a2/src/molecule/dependency/ansible_galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/dependency/ansible_galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/dependency/ansible_galaxy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/dependency/ansible_galaxy/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/dependency/ansible_galaxy/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/dependency/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/dependency/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.585761 molecule-6.0.0a2/src/molecule/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/driver/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/driver/delegated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.589761 molecule-6.0.0a2/src/molecule/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/model/schema_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/platforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.589761 molecule-6.0.0a2/src/molecule/provisioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/provisioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33606 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/provisioner/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/provisioner/ansible_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/provisioner/ansible_playbooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/provisioner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.589761 molecule-6.0.0a2/src/molecule/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.597761 molecule-6.0.0a2/src/molecule/test/a_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.601761 molecule-6.0.0a2/src/molecule/test/a_unit/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.601761 molecule-6.0.0a2/src/molecule/test/a_unit/command/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/init/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_converge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_destroy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_idempotence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_side_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/command/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.601761 molecule-6.0.0a2/src/molecule/test/a_unit/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/cookiecutter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/cookiecutter/test_molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.601761 molecule-6.0.0a2/src/molecule/test/a_unit/dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/dependency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.601761 molecule-6.0.0a2/src/molecule/test/a_unit/dependency/ansible_galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/dependency/ansible_galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/dependency/ansible_galaxy/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/dependency/ansible_galaxy/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/dependency/test_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.601761 molecule-6.0.0a2/src/molecule/test/a_unit/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/driver/test_delegated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.601761 molecule-6.0.0a2/src/molecule/test/a_unit/lint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/lint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.601761 molecule-6.0.0a2/src/molecule/test/a_unit/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.605761 molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_dependency_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_driver_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_platforms_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_provisioner_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_scenario_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_verifier_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.609761 molecule-6.0.0a2/src/molecule/test/a_unit/provisioner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/provisioner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/provisioner/test_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/provisioner/test_ansible_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/provisioner/test_ansible_playbooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/test_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/test_platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/test_scenarios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/test_scenarios_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.609761 molecule-6.0.0a2/src/molecule/test/a_unit/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/verifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/verifier/test_ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/a_unit/verifier/test_testinfra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.613761 molecule-6.0.0a2/src/molecule/test/b_functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/b_functional/.ansible-lint
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/b_functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/b_functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10245 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/b_functional/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.613761 molecule-6.0.0a2/src/molecule/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/.yamllint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.613761 molecule-6.0.0a2/src/molecule/test/resources/invalid_role_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.613761 molecule-6.0.0a2/src/molecule/test/resources/invalid_role_template/bad_format/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/invalid_role_template/bad_format/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/invalid_role_template/cookiecutter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.537760 molecule-6.0.0a2/src/molecule/test/resources/playbooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.613761 molecule-6.0.0a2/src/molecule/test/resources/playbooks/delegated/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/playbooks/delegated/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/playbooks/delegated/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.537760 molecule-6.0.0a2/src/molecule/test/resources/playbooks/delegated/inventory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.537760 molecule-6.0.0a2/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.613761 molecule-6.0.0a2/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/playbooks/delegated/inventory/group_vars/all/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.537760 molecule-6.0.0a2/src/molecule/test/resources/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.537760 molecule-6.0.0a2/src/molecule/test/resources/roles/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.613761 molecule-6.0.0a2/src/molecule/test/resources/roles/molecule/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/roles/molecule/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.613761 molecule-6.0.0a2/src/molecule/test/resources/roles/molecule/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/roles/molecule/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.617761 molecule-6.0.0a2/src/molecule/test/resources/sample-collection/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/sample-collection/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.537760 molecule-6.0.0a2/src/molecule/test/resources/sample-collection/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.617761 molecule-6.0.0a2/src/molecule/test/resources/sample-collection/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/sample-collection/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/sample-collection/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.537760 molecule-6.0.0a2/src/molecule/test/resources/sample-collection/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.541760 molecule-6.0.0a2/src/molecule/test/resources/sample-collection/roles/get_rich/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.617761 molecule-6.0.0a2/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/sample-collection/roles/get_rich/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.541760 molecule-6.0.0a2/src/molecule/test/resources/schema_instance_files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.617761 molecule-6.0.0a2/src/molecule/test/resources/schema_instance_files/invalid/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/schema_instance_files/invalid/molecule_delegated.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.617761 molecule-6.0.0a2/src/molecule/test/resources/schema_instance_files/valid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/resources/schema_instance_files/valid/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.617761 molecule-6.0.0a2/src/molecule/test/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.541760 molecule-6.0.0a2/src/molecule/test/scenarios/cleanup/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.541760 molecule-6.0.0a2/src/molecule/test/scenarios/cleanup/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.621761 molecule-6.0.0a2/src/molecule/test/scenarios/cleanup/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/cleanup/molecule/default/cleanup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/cleanup/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/cleanup/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.621761 molecule-6.0.0a2/src/molecule/test/scenarios/cleanup/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/cleanup/molecule/default/tests/test_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.541760 molecule-6.0.0a2/src/molecule/test/scenarios/dependency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.541760 molecule-6.0.0a2/src/molecule/test/scenarios/dependency/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.621761 molecule-6.0.0a2/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/dependency/molecule/ansible-galaxy/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.621761 molecule-6.0.0a2/src/molecule/test/scenarios/dependency/molecule/shell/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/dependency/molecule/shell/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/dependency/molecule/shell/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.545760 molecule-6.0.0a2/src/molecule/test/scenarios/driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.545760 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.621761 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.545760 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.625761 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.545760 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.625761 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.545760 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.625761 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/destroy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/driver/delegated_invalid_role_name_with_role_name_check_equals_to_1/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.625761 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.545760 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.625761 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/group_vars/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/group_vars/example/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.629762 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/host_vars/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/host_vars/extra-host
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.629762 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/host_vars/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/host_vars/instance/all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/hosts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.545760 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.629762 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.545760 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.629762 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/default/group_vars/example/all.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.545760 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.629762 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/default/host_vars/instance/all.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.629762 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/links/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/links/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/links/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.545760 molecule-6.0.0a2/src/molecule/test/scenarios/idempotence/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.545760 molecule-6.0.0a2/src/molecule/test/scenarios/idempotence/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.629762 molecule-6.0.0a2/src/molecule/test/scenarios/idempotence/molecule/raises/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/idempotence/molecule/raises/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/idempotence/molecule/raises/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.633762 molecule-6.0.0a2/src/molecule/test/scenarios/idempotence/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/idempotence/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.549760 molecule-6.0.0a2/src/molecule/test/scenarios/interpolation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.549760 molecule-6.0.0a2/src/molecule/test/scenarios/interpolation/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.633762 molecule-6.0.0a2/src/molecule/test/scenarios/interpolation/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/interpolation/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/interpolation/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.549760 molecule-6.0.0a2/src/molecule/test/scenarios/overrride_driver/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.549760 molecule-6.0.0a2/src/molecule/test/scenarios/overrride_driver/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.633762 molecule-6.0.0a2/src/molecule/test/scenarios/overrride_driver/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/overrride_driver/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/overrride_driver/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.549760 molecule-6.0.0a2/src/molecule/test/scenarios/side_effect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.549760 molecule-6.0.0a2/src/molecule/test/scenarios/side_effect/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.633762 molecule-6.0.0a2/src/molecule/test/scenarios/side_effect/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/side_effect/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/side_effect/molecule/default/molecule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/side_effect/molecule/default/side_effect.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.633762 molecule-6.0.0a2/src/molecule/test/scenarios/side_effect/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/side_effect/molecule/default/tests/test_side_effect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.549760 molecule-6.0.0a2/src/molecule/test/scenarios/test_destroy_strategy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.549760 molecule-6.0.0a2/src/molecule/test/scenarios/test_destroy_strategy/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.637762 molecule-6.0.0a2/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.637762 molecule-6.0.0a2/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.637762 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.549760 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.637762 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/molecule/testinfra/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/molecule/testinfra/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/molecule/testinfra/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.637762 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/molecule/testinfra/shared/test_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.641762 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/molecule/testinfra/tests/test_testinfra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.637762 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.637762 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/test/scenarios/verifier/molecule/testinfra-pre-commit/tests/test_testinfra_pre_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.641762 molecule-6.0.0a2/src/molecule/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/verifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/verifier/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/verifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-08-01 12:47:31.000000 molecule-6.0.0a2/src/molecule/verifier/testinfra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.573761 molecule-6.0.0a2/src/molecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-08-01 12:47:47.000000 molecule-6.0.0a2/src/molecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12979 2023-08-01 12:47:47.000000 molecule-6.0.0a2/src/molecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 12:47:47.000000 molecule-6.0.0a2/src/molecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-01 12:47:47.000000 molecule-6.0.0a2/src/molecule.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-08-01 12:47:47.000000 molecule-6.0.0a2/src/molecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-01 12:47:47.000000 molecule-6.0.0a2/src/molecule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 12:47:47.641762 molecule-6.0.0a2/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-08-01 12:47:31.000000 molecule-6.0.0a2/tools/get-version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 12:47:31.000000 molecule-6.0.0a2/tools/opts.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-08-01 12:47:31.000000 molecule-6.0.0a2/tools/smoketest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-08-01 12:47:31.000000 molecule-6.0.0a2/tools/test-setup.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      214 2023-08-01 12:47:31.000000 molecule-6.0.0a2/tools/update-version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-08-01 12:47:31.000000 molecule-6.0.0a2/tox.ini
```

### Comparing `molecule-6.0.0a1/.config/molecule.spec` & `molecule-6.0.0a2/.config/molecule.spec`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/.gitattributes` & `molecule-6.0.0a2/.gitattributes`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/.github/ISSUE_TEMPLATE/bug_report.md` & `molecule-6.0.0a2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/.github/ISSUE_TEMPLATE/config.yml` & `molecule-6.0.0a2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/.github/workflows/redirects.yml` & `molecule-6.0.0a2/.github/workflows/redirects.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/.github/workflows/release.yml` & `molecule-6.0.0a2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/.github/workflows/tox.yml` & `molecule-6.0.0a2/.github/workflows/tox.yml`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     # limit potential endless looks like we had with build-containers
     timeout-minutes: 20
     strategy:
       fail-fast: false
       matrix: ${{ fromJson(needs.pre.outputs.matrix) }}
 
     env:
-      PYTEST_REQPASS: 445
+      PYTEST_REQPASS: 446
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0 # needed by setuptools-scm
           submodules: true
 
       - name: Set pre-commit cache
```

### Comparing `molecule-6.0.0a1/.packit.yaml` & `molecule-6.0.0a2/.packit.yaml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/.vscode/settings.json` & `molecule-6.0.0a2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/.yamllint` & `molecule-6.0.0a2/.yamllint`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/DCO_1_1.md` & `molecule-6.0.0a2/DCO_1_1.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/LICENSE` & `molecule-6.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/PKG-INFO` & `molecule-6.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule
-Version: 6.0.0a1
+Version: 6.0.0a2
 Summary: Molecule aids in the development and testing of Ansible roles
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule
@@ -28,15 +28,15 @@
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
-Provides-Extra: lock
+Provides-Extra: testinfra
 License-File: LICENSE
 
 # About Ansible Molecule
 
 [![PyPI Package](https://img.shields.io/pypi/v/molecule)](https://pypi.org/project/molecule/)
 [![Documentation Status](https://readthedocs.org/projects/molecule/badge/?version=latest)](https://ansible.readthedocs.io/projects/molecule)
 [![image](https://github.com/ansible-community/molecule/workflows/tox/badge.svg)](https://github.com/ansible-community/molecule/actions)
```

### Comparing `molecule-6.0.0a1/README.md` & `molecule-6.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/bindep.txt` & `molecule-6.0.0a2/bindep.txt`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/conftest.py` & `molecule-6.0.0a2/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/_static/images/favicon.ico` & `molecule-6.0.0a2/docs/_static/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/_static/images/logo.png` & `molecule-6.0.0a2/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/_static/images/logo_big.png` & `molecule-6.0.0a2/docs/_static/images/logo_big.png`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/ci.md` & `molecule-6.0.0a2/docs/ci.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/configuration.md` & `molecule-6.0.0a2/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/contributing.md` & `molecule-6.0.0a2/docs/contributing.md`

 * *Files 6% similar despite different names*

```diff
@@ -117,19 +117,14 @@
 ### Updating Dependencies
 
 Dependencies need to be updated by hand in:
 
 - `.config/requirements.in`
 - `.pre-commit-config.yaml` (2 places)
 
-Afterwards, you will need to generate changes to `requirements.lock.txt`
-and `requirement.txt`, by running the commands listed at the top of those files.
-
-Please note that CI will attempt to regenerate those changes, and if there is any diff, CI will fail.
-
 ## Credits
 
 Based on the good work of John Dewey
 ([\@retr0h](https://github.com/retr0h)) and other
 [contributors](https://github.com/ansible-community/molecule/graphs/contributors).
 Active member list can be seen at [Molecule working
 group](https://github.com/ansible/community/wiki/Molecule).
```

### Comparing `molecule-6.0.0a1/docs/examples.md` & `molecule-6.0.0a2/docs/examples.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/faq.md` & `molecule-6.0.0a2/docs/faq.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/getting-started.md` & `molecule-6.0.0a2/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/images/favicon.ico` & `molecule-6.0.0a2/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/images/logo.png` & `molecule-6.0.0a2/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/images/logo.svg` & `molecule-6.0.0a2/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/index.md` & `molecule-6.0.0a2/docs/index.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/installation.md` & `molecule-6.0.0a2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/next.md` & `molecule-6.0.0a2/docs/next.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/podman.md` & `molecule-6.0.0a2/docs/podman.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/docs/usage.md` & `molecule-6.0.0a2/docs/usage.md`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/mkdocs.yml` & `molecule-6.0.0a2/mkdocs.yml`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,17 @@
   - Using:
       - getting-started.md
       - usage.md
       - next.md
       - configuration.md
       - ci.md
   - Examples:
+      - docker.md
       - podman.md
+      - kubevirt.md
   - examples.md
   - faq.md
   - contributing.md
 
 plugins:
   - autorefs
   - search
```

### Comparing `molecule-6.0.0a1/molecule/default/create.yml` & `molecule-6.0.0a2/molecule/default/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/molecule/default/destroy.yml` & `molecule-6.0.0a2/molecule/default/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/molecule/podman/converge.yml` & `molecule-6.0.0a2/molecule/docker/converge.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/molecule/podman/create.yml` & `molecule-6.0.0a2/molecule/podman/create.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/molecule/podman/destroy.yml` & `molecule-6.0.0a2/molecule/podman/destroy.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/playbooks/snap-pre-run.yaml` & `molecule-6.0.0a2/playbooks/snap-pre-run.yaml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/pyproject.toml` & `molecule-6.0.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -217,13 +217,15 @@
 [tool.ruff.per-file-ignores]
 "src/molecule/test/**.py" = ["S"]
 "src/molecule/*/\\{\\{*/**.py" = ["S"]
 
 [tool.setuptools.dynamic]
 optional-dependencies.docs = { file = [".config/requirements-docs.txt"] }
 optional-dependencies.test = { file = [".config/requirements-test.txt"] }
-optional-dependencies.lock = { file = [".config/requirements-lock.txt"] }
+optional-dependencies.testinfra = { file = [
+  ".config/requirements-testinfra.txt",
+] }
 dependencies = { file = [".config/requirements.in"] }
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
 write_to = "src/molecule/_version.py"
```

### Comparing `molecule-6.0.0a1/snap/snapcraft.yaml` & `molecule-6.0.0a2/snap/snapcraft.yaml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/__init__.py` & `molecule-6.0.0a2/src/molecule/__init__.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/__main__.py` & `molecule-6.0.0a2/src/molecule/__main__.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/api.py` & `molecule-6.0.0a2/src/molecule/api.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/__init__.py` & `molecule-6.0.0a2/src/molecule/command/__init__.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/base.py` & `molecule-6.0.0a2/src/molecule/command/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/check.py` & `molecule-6.0.0a2/src/molecule/command/check.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/cleanup.py` & `molecule-6.0.0a2/src/molecule/command/cleanup.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/converge.py` & `molecule-6.0.0a2/src/molecule/command/converge.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/create.py` & `molecule-6.0.0a2/src/molecule/command/create.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/dependency.py` & `molecule-6.0.0a2/src/molecule/command/dependency.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/destroy.py` & `molecule-6.0.0a2/src/molecule/command/destroy.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/drivers.py` & `molecule-6.0.0a2/src/molecule/command/drivers.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/idempotence.py` & `molecule-6.0.0a2/src/molecule/command/idempotence.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/init/base.py` & `molecule-6.0.0a2/src/molecule/command/init/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/init/init.py` & `molecule-6.0.0a2/src/molecule/command/init/init.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/init/scenario.py` & `molecule-6.0.0a2/src/molecule/command/init/scenario.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/list.py` & `molecule-6.0.0a2/src/molecule/command/list.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/login.py` & `molecule-6.0.0a2/src/molecule/command/login.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/matrix.py` & `molecule-6.0.0a2/src/molecule/command/matrix.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/prepare.py` & `molecule-6.0.0a2/src/molecule/command/prepare.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/reset.py` & `molecule-6.0.0a2/src/molecule/command/reset.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/side_effect.py` & `molecule-6.0.0a2/src/molecule/command/side_effect.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/syntax.py` & `molecule-6.0.0a2/src/molecule/command/syntax.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/test.py` & `molecule-6.0.0a2/src/molecule/command/test.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/command/verify.py` & `molecule-6.0.0a2/src/molecule/command/verify.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/config.py` & `molecule-6.0.0a2/src/molecule/config.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/console.py` & `molecule-6.0.0a2/src/molecule/console.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/data/driver.json` & `molecule-6.0.0a2/src/molecule/data/driver.json`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/data/init-scenario.yml` & `molecule-6.0.0a2/src/molecule/data/init-scenario.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/data/molecule.json` & `molecule-6.0.0a2/src/molecule/data/molecule.json`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/data/templates/scenario/create.yml.j2` & `molecule-6.0.0a2/src/molecule/data/templates/scenario/create.yml.j2`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/data/templates/scenario/destroy.yml.j2` & `molecule-6.0.0a2/src/molecule/data/templates/scenario/destroy.yml.j2`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/__init__.py` & `molecule-6.0.0a2/src/molecule/dependency/ansible_galaxy/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 from molecule.dependency.ansible_galaxy.roles import Roles
 from molecule.dependency.base import Base
 
 
 class AnsibleGalaxy(Base):
     """Galaxy is the default dependency manager.
 
+    From v6.0.0, the dependencies are installed in the directory that defined
+    in ansible configuration. The default installation directory is
+    [DEFAULT_ROLES_PATH][]([ANSIBLE_HOME][]). If two versions of the same
+    dependency is required, there is a conflict if the default installation
+    directory is used because both are tried to be installed in one directory.
+
     Additional options can be passed to ``ansible-galaxy install`` through the
     options dict.  Any option set in this section will override the defaults.
 
     The `role-file` and `requirements-file` search path is `<role-name>`
     directory. The default value for `role-file` is `requirements.yml`, and the
     default value for `requirements-file` is `collections.yml`.
 
@@ -70,14 +76,17 @@
 
     ``` yaml
         dependency:
           name: galaxy
           env:
             FOO: bar
     ```
+
+    [DEFAULT_ROLES_PATH]: https://docs.ansible.com/ansible/latest/cli/ansible-galaxy.html#cmdoption-ansible-galaxy-role-remove-p
+    [ANSIBLE_HOME]: https://docs.ansible.com/ansible/latest/reference_appendices/config.html#ansible-home
     """
 
     def __init__(self, config) -> None:
         """Construct AnsibleGalaxy."""
         super().__init__(config)
         self.invocations = [Roles(config), Collections(config)]
```

### Comparing `molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/base.py` & `molecule-6.0.0a2/src/molecule/dependency/ansible_galaxy/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     @abc.abstractmethod
     def requirements_file(self):  # cover
         pass
 
     @property
     def default_options(self):
         d = {
-            "force": True,
+            "force": False,
         }
         if self._config.debug:
             d["vvv"] = True
 
         return d
 
     def filter_options(self, opts, keys):
```

### Comparing `molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/collections.py` & `molecule-6.0.0a2/src/molecule/dependency/ansible_galaxy/collections.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/dependency/ansible_galaxy/roles.py` & `molecule-6.0.0a2/src/molecule/dependency/ansible_galaxy/roles.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/dependency/base.py` & `molecule-6.0.0a2/src/molecule/dependency/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/dependency/shell.py` & `molecule-6.0.0a2/src/molecule/dependency/shell.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/driver/base.py` & `molecule-6.0.0a2/src/molecule/driver/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/driver/delegated.py` & `molecule-6.0.0a2/src/molecule/driver/delegated.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/interpolation.py` & `molecule-6.0.0a2/src/molecule/interpolation.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/logger.py` & `molecule-6.0.0a2/src/molecule/logger.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/model/schema_v3.py` & `molecule-6.0.0a2/src/molecule/model/schema_v3.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/platforms.py` & `molecule-6.0.0a2/src/molecule/platforms.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/provisioner/ansible.py` & `molecule-6.0.0a2/src/molecule/provisioner/ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/provisioner/ansible_playbook.py` & `molecule-6.0.0a2/src/molecule/provisioner/ansible_playbook.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/provisioner/ansible_playbooks.py` & `molecule-6.0.0a2/src/molecule/provisioner/ansible_playbooks.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/provisioner/base.py` & `molecule-6.0.0a2/src/molecule/provisioner/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/scenario.py` & `molecule-6.0.0a2/src/molecule/scenario.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/scenarios.py` & `molecule-6.0.0a2/src/molecule/scenarios.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/shell.py` & `molecule-6.0.0a2/src/molecule/shell.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/state.py` & `molecule-6.0.0a2/src/molecule/state.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/status.py` & `molecule-6.0.0a2/src/molecule/status.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/conftest.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/init/test_scenario.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/init/test_scenario.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_base.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_check.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_check.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_cleanup.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_converge.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_converge.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_create.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_create.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_dependency.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_dependency.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_destroy.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_destroy.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_idempotence.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_idempotence.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_list.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_list.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_login.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_login.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_matrix.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_matrix.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_prepare.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_prepare.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_side_effect.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_side_effect.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_syntax.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_syntax.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_test.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_test.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/command/test_verify.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/command/test_verify.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/conftest.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/cookiecutter/test_molecule.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/cookiecutter/test_molecule.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/dependency/ansible_galaxy/test_collections.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/dependency/ansible_galaxy/test_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
 def test_default_options_property(_instance, role_file):
-    x = {"requirements-file": role_file, "force": True}
+    x = {"requirements-file": role_file, "force": False}
 
     assert x == _instance.default_options
 
 
 def test_default_env_property(_instance):
     env = _instance.default_env
 
@@ -91,28 +91,28 @@
 def test_enabled_property(_instance):
     assert _instance.enabled
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_options_property(_instance, role_file):
     x = {
-        "force": True,
+        "force": False,
         "requirements-file": role_file,
         "foo": "bar",
         "v": True,
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_options_property_handles_cli_args(role_file, _instance):
     _instance._config.args = {"debug": True}
     x = {
-        "force": True,
+        "force": False,
         "requirements-file": role_file,
         "foo": "bar",
         "vvv": True,
     }
 
     assert x == _instance.options
 
@@ -127,15 +127,14 @@
     _instance.bake()
     args = [
         "ansible-galaxy",
         "collection",
         "install",
         "--foo",
         "bar",
-        "--force",
         "--requirements-file",
         role_file,
         "-v",
     ]
     assert _instance._sh_command == args
```

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/dependency/ansible_galaxy/test_roles.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/dependency/ansible_galaxy/test_roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 
 def test_config_private_member(_instance):
     assert isinstance(_instance._config, config.Config)
 
 
 def test_default_options_property(_instance, role_file):
-    x = {"role-file": role_file, "force": True}
+    x = {"role-file": role_file, "force": False}
 
     assert x == _instance.default_options
 
 
 def test_default_env_property(_instance):
     env = _instance.default_env
 
@@ -90,28 +90,28 @@
 def test_enabled_property(_instance):
     assert _instance.enabled
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_options_property(_instance, role_file):
     x = {
-        "force": True,
+        "force": False,
         "role-file": role_file,
         "foo": "bar",
         "v": True,
     }
 
     assert x == _instance.options
 
 
 @pytest.mark.parametrize("config_instance", ["_dependency_section_data"], indirect=True)
 def test_options_property_handles_cli_args(role_file, _instance):
     _instance._config.args = {"debug": True}
     x = {
-        "force": True,
+        "force": False,
         "role-file": role_file,
         "foo": "bar",
         "vvv": True,
     }
 
     assert x == _instance.options
 
@@ -125,15 +125,14 @@
 def test_galaxy_bake(_instance, role_file):
     _instance.bake()
     args = [
         "ansible-galaxy",
         "install",
         "--foo",
         "bar",
-        "--force",
         "--role-file",
         role_file,
         "-v",
     ]
     assert _instance._sh_command == args
```

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/dependency/test_shell.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/dependency/test_shell.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/driver/test_delegated.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/driver/test_delegated.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/conftest.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_dependency_section.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_dependency_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_driver_section.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_driver_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_platforms_section.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_platforms_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_provisioner_section.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_provisioner_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_scenario_section.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_scenario_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_schema.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_schema.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/model/v2/test_verifier_section.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/model/v2/test_verifier_section.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/test_ansible.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/provisioner/test_ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/test_ansible_playbook.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/provisioner/test_ansible_playbook.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/provisioner/test_ansible_playbooks.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/provisioner/test_ansible_playbooks.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/test_api.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/test_api.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/test_config.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/test_config.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/test_interpolation.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/test_logger.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/test_platforms.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/test_platforms.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/test_scenario.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/test_scenario.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/test_scenarios.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/test_scenarios.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/test_scenarios_ordered.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/test_scenarios_ordered.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/test_shell.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/test_state.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/test_state.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/test_status.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/test_status.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/test_text.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/test_text.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/test_util.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/test_util.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/verifier/test_ansible.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/verifier/test_ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/a_unit/verifier/test_testinfra.py` & `molecule-6.0.0a2/src/molecule/test/a_unit/verifier/test_testinfra.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/b_functional/conftest.py` & `molecule-6.0.0a2/src/molecule/test/b_functional/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/b_functional/test_command.py` & `molecule-6.0.0a2/src/molecule/test/b_functional/test_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,7 +339,16 @@
 def test_podman() -> None:
     assert (
         run_command(
             ["molecule", "test", "--scenario-name", "podman"],
         ).returncode
         == 0
     )
+
+
+def test_docker() -> None:
+    assert (
+        run_command(
+            ["molecule", "test", "--scenario-name", "docker"],
+        ).returncode
+        == 0
+    )
```

### Comparing `molecule-6.0.0a1/src/molecule/test/conftest.py` & `molecule-6.0.0a2/src/molecule/test/conftest.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/resources/schema_instance_files/valid/molecule.yml` & `molecule-6.0.0a2/src/molecule/test/resources/schema_instance_files/valid/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml` & `molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/default/converge.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml` & `molecule-6.0.0a2/src/molecule/test/scenarios/host_group_vars/molecule/default/molecule.yml`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py` & `molecule-6.0.0a2/src/molecule/test/scenarios/test_destroy_strategy/molecule/default/tests/test_destroy_strategy.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/text.py` & `molecule-6.0.0a2/src/molecule/text.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/util.py` & `molecule-6.0.0a2/src/molecule/util.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/verifier/ansible.py` & `molecule-6.0.0a2/src/molecule/verifier/ansible.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/verifier/base.py` & `molecule-6.0.0a2/src/molecule/verifier/base.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule/verifier/testinfra.py` & `molecule-6.0.0a2/src/molecule/verifier/testinfra.py`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/src/molecule.egg-info/PKG-INFO` & `molecule-6.0.0a2/src/molecule.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecule
-Version: 6.0.0a1
+Version: 6.0.0a2
 Summary: Molecule aids in the development and testing of Ansible roles
 Author-email: Ansible by Red Hat <info@ansible.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible-community/molecule
 Project-URL: documentation, https://molecule.readthedocs.io/
 Project-URL: repository, https://github.com/ansible-community/molecule
@@ -28,15 +28,15 @@
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
-Provides-Extra: lock
+Provides-Extra: testinfra
 License-File: LICENSE
 
 # About Ansible Molecule
 
 [![PyPI Package](https://img.shields.io/pypi/v/molecule)](https://pypi.org/project/molecule/)
 [![Documentation Status](https://readthedocs.org/projects/molecule/badge/?version=latest)](https://ansible.readthedocs.io/projects/molecule)
 [![image](https://github.com/ansible-community/molecule/workflows/tox/badge.svg)](https://github.com/ansible-community/molecule/actions)
```

### Comparing `molecule-6.0.0a1/src/molecule.egg-info/SOURCES.txt` & `molecule-6.0.0a2/src/molecule.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,17 @@
 linkcheckerrc
 mkdocs.yml
 pyproject.toml
 runtime.txt
 tox.ini
 .config/molecule.spec
 .config/requirements-docs.txt
-.config/requirements-lock.txt
 .config/requirements-test.txt
+.config/requirements-testinfra.txt
 .config/requirements.in
-.config/requirements.txt
 .config/molecule/config.yml
 .github/CODEOWNERS
 .github/CODE_OF_CONDUCT.md
 .github/dependabot.yml
 .github/patchback.yml
 .github/release-drafter.yml
 .github/ISSUE_TEMPLATE/bug_report.md
@@ -41,34 +40,49 @@
 .github/workflows/release.yml
 .github/workflows/tox.yml
 .vscode/extensions.json
 .vscode/settings.json
 docs/ci.md
 docs/configuration.md
 docs/contributing.md
+docs/docker.md
 docs/examples.md
 docs/faq.md
 docs/getting-started.md
 docs/google04e29a42ae6e6cbc.html
 docs/index.md
 docs/installation.md
+docs/kubevirt.md
 docs/next.md
 docs/podman.md
 docs/redirects.yml
 docs/usage.md
 docs/_static/images/favicon.ico
 docs/_static/images/logo.png
 docs/_static/images/logo_big.png
 docs/images/favicon.ico
 docs/images/logo.png
 docs/images/logo.svg
 molecule/default/converge.yml
 molecule/default/create.yml
 molecule/default/destroy.yml
 molecule/default/molecule.yml
+molecule/docker/converge.yml
+molecule/docker/create.yml
+molecule/docker/destroy.yml
+molecule/docker/molecule.yml
+molecule/docker/requirements.yml
+molecule/docker/tasks/create-fail.yml
+molecule/kubevirt/converge.yml
+molecule/kubevirt/create.yml
+molecule/kubevirt/destroy.yml
+molecule/kubevirt/molecule.yml
+molecule/kubevirt/requirements.yml
+molecule/kubevirt/tasks/create_vm.yml
+molecule/kubevirt/tasks/create_vm_dictionary.yml
 molecule/podman/converge.yml
 molecule/podman/create.yml
 molecule/podman/destroy.yml
 molecule/podman/molecule.yml
 molecule/podman/requirements.yml
 molecule/podman/tasks/create-fail.yml
 playbooks/snap-pre-run.yaml
```

### Comparing `molecule-6.0.0a1/tools/test-setup.sh` & `molecule-6.0.0a2/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `molecule-6.0.0a1/tox.ini` & `molecule-6.0.0a2/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,14 @@
     ANSIBLE_CONFIG={toxinidir}/.ansible.cfg
     ANSIBLE_DISPLAY_FAILED_STDERR=1
     ANSIBLE_NOCOWS=1
     ANSIBLE_VERBOSITY=1
     COVERAGE_FILE={env:COVERAGE_FILE:{toxworkdir}/.coverage.{envname}}
     COVERAGE_PROCESS_START={toxinidir}/pyproject.toml
     MOLECULE_NO_LOG=0
-    PIP_CONSTRAINT = {toxinidir}/.config/requirements.txt
-    devel: PIP_CONSTRAINT=/dev/null
     PIP_DISABLE_PIP_VERSION_CHECK=1
     PYTHONDONTWRITEBYTECODE=1
     PYTHONUNBUFFERED=1
     # Temporare remove "-n auto" as it seems to break coverage on this project.
     _EXTRAS=-l
 deps =
     devel: git+https://github.com/ansible/ansible#egg=ansible-core
@@ -76,34 +74,17 @@
     python -m pre_commit run {posargs:--all --show-diff-on-failure}
 deps =
     pre-commit>=2.21.0
     check-jsonschema>=0.20.0
     jsonschema>=4.17.3
 setenv =
   {[testenv]setenv}
-  # without his upgrade would likely not do anything
-  PIP_CONSTRAINT = /dev/null
 skip_install = true
 usedevelop = false
 
-[testenv:deps]
-description = Bump all test dependencies
-skip_install = true
-deps = {[testenv:lint]deps}
-setenv = {[testenv:lint]setenv}
-commands =
-  # manual hook calls the optional pip-compile-upgrade hook after pip-compile
-  {[testenv:lint]commands} --hook-stage manual pip-compile
-  # Update pre-commit hooks
-  -pre-commit autoupdate
-  # We fail if files are modified at the end
-  git diff --exit-code
-allowlist_externals =
-    git
-
 [testenv:docs]
 description = Build documentation
 passenv = *
 usedevelop = true
 commands =
     mkdocs build --strict
     linkchecker -f linkcheckerrc site
```

