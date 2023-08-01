# Comparing `tmp/roblox-pyc-2.25.113.tar.gz` & `tmp/roblox-pyc-2.26.113.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-pyc-2.25.113.tar", last modified: Tue Aug  1 01:28:44 2023, max compression
+gzip compressed data, was "roblox-pyc-2.26.113.tar", last modified: Tue Aug  1 01:37:07 2023, max compression
```

## Comparing `roblox-pyc-2.25.113.tar` & `roblox-pyc-2.26.113.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.237825 roblox-pyc-2.25.113/
--rw-r--r--   0 runner    (1001) docker     (123)    34525 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-08-01 01:28:44.237825 roblox-pyc-2.25.113/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.225825 roblox-pyc-2.25.113/roblox_pyc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-08-01 01:28:44.000000 roblox-pyc-2.25.113/roblox_pyc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-08-01 01:28:44.000000 roblox-pyc-2.25.113/roblox_pyc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:28:44.000000 roblox-pyc-2.25.113/roblox_pyc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-01 01:28:44.000000 roblox-pyc-2.25.113/roblox_pyc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 01:28:44.000000 roblox-pyc-2.25.113/roblox_pyc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 01:28:44.000000 roblox-pyc-2.25.113/roblox_pyc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.229825 roblox-pyc-2.25.113/robloxpyc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.229825 roblox-pyc-2.25.113/robloxpyc/LuauAST/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/bundle.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/List.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/create.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/enums.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/globals.ts
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/strings.ts
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/typeGuards.ts
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauAST/types/
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/types/mapping.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/types/nodes.ts
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/types/operators.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/assert.ts
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/getKindName.ts
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/isMetamethod.ts
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/isReservedClassField.ts
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/isReservedIdentifier.ts
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/isValidIdentifier.ts
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/isValidNumberLiteral.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/RenderState.ts
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.225825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderCallExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderComputedIndexExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderIdentifier.ts
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderMethodCallExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderParenthesizedExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderPropertyAccessExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderTemporaryIdentifier.ts
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderArray.ts
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderBinaryExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderFunctionExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderIfExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderMap.ts
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderMixedTable.ts
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderNumberLiteral.ts
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderSet.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderStringLiteral.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderUnaryExpression.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/fields/renderMapField.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.237825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderAssignment.ts
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderBreakStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderCallStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderComment.ts
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderContinueStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderDoStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderForStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderFunctionDeclaration.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderIfStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderMethodDeclaration.ts
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderNumericForStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderRepeatStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderReturnStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderVariableDeclaration.ts
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderWhileStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/render.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/solveTempIds.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.237825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/getEnding.ts
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/getOrSetDefault.ts
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/getSafeBracketEquals.ts
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/identity.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/needsParentheses.ts
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/renderArguments.ts
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/renderParameters.ts
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/renderStatements.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/visit.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.237825 roblox-pyc-2.25.113/robloxpyc/__communication__/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/__communication__/cfg.pkl
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/basecompilers.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/binopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/boolopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/climaker.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/cmpopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/cnodevisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/colortext.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/configmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/cpAST.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/ctranslator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/errormanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/installationmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/loopcounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/luainit.py
--rw-r--r--   0 runner    (1001) docker     (123)    28487 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/luainitlua.lua
--rw-r--r--   0 runner    (1001) docker     (123)    49380 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/nameconstdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/nodevisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    62675 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/pytranslator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    50521 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/robloxpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/symbolsstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/textcompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/tokenendmode.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/unaryopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/wally.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 01:28:44.237825 roblox-pyc-2.25.113/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.855219 roblox-pyc-2.26.113/
+-rw-r--r--   0 runner    (1001) docker     (123)    34525 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-08-01 01:37:07.855219 roblox-pyc-2.26.113/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.831219 roblox-pyc-2.26.113/roblox_pyc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-08-01 01:37:07.000000 roblox-pyc-2.26.113/roblox_pyc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-08-01 01:37:07.000000 roblox-pyc-2.26.113/roblox_pyc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:37:07.000000 roblox-pyc-2.26.113/roblox_pyc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-01 01:37:07.000000 roblox-pyc-2.26.113/roblox_pyc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 01:37:07.000000 roblox-pyc-2.26.113/roblox_pyc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 01:37:07.000000 roblox-pyc-2.26.113/roblox_pyc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.839219 roblox-pyc-2.26.113/robloxpyc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.839219 roblox-pyc-2.26.113/robloxpyc/LuauAST/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/bundle.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.839219 roblox-pyc-2.26.113/robloxpyc/LuauAST/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/impl/List.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/impl/create.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/impl/enums.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/impl/globals.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/impl/strings.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/impl/typeGuards.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.843219 roblox-pyc-2.26.113/robloxpyc/LuauAST/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/types/mapping.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/types/nodes.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/types/operators.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.843219 roblox-pyc-2.26.113/robloxpyc/LuauAST/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/util/assert.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/util/getKindName.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/util/isMetamethod.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/util/isReservedClassField.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/util/isReservedIdentifier.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/util/isValidIdentifier.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauAST/util/isValidNumberLiteral.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.843219 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/RenderState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.827219 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.847219 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.847219 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderCallExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderComputedIndexExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderIdentifier.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderMethodCallExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderParenthesizedExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderPropertyAccessExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderTemporaryIdentifier.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderArray.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderBinaryExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderFunctionExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderIfExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderMap.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderMixedTable.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderNumberLiteral.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderSet.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderStringLiteral.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderUnaryExpression.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.847219 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/fields/renderMapField.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.851219 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderAssignment.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderBreakStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderCallStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderComment.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderContinueStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderDoStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderForStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderFunctionDeclaration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderIfStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderMethodDeclaration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderNumericForStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderRepeatStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderReturnStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderVariableDeclaration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderWhileStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/render.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/solveTempIds.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.855219 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/getEnding.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/getOrSetDefault.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/getSafeBracketEquals.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/identity.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/needsParentheses.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/renderArguments.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/renderParameters.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/renderStatements.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/visit.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:37:07.855219 roblox-pyc-2.26.113/robloxpyc/__communication__/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/__communication__/cfg.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/basecompilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/binopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/boolopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/climaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/cmpopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/cnodevisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/colortext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/configmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/cpAST.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/ctranslator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/errormanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/installationmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/loopcounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/luainit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28487 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/luainitlua.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    49380 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/nameconstdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/nodevisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62675 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/pytranslator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50543 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/robloxpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/symbolsstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/textcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/tokenendmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/unaryopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/wally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/robloxpyc/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 01:37:07.855219 roblox-pyc-2.26.113/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-01 01:36:55.000000 roblox-pyc-2.26.113/setup.py
```

### Comparing `roblox-pyc-2.25.113/LICENSE` & `roblox-pyc-2.26.113/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/PKG-INFO` & `roblox-pyc-2.26.113/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roblox-pyc
-Version: 2.25.113
+Version: 2.26.113
 Summary: The Python, Lunar, C, C++ to Roblox Lua compiler
 Home-page: https://github.com/AsynchronousAI/roblox.pyc
 Author: roblox-pyc team
 Author-email: roblox.pyc@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roblox-pyc Version: 2.25.113 Summary: The Python,
+Metadata-Version: 2.1 Name: roblox-pyc Version: 2.26.113 Summary: The Python,
 Lunar, C, C++ to Roblox Lua compiler Home-page: https://github.com/
 AsynchronousAI/roblox.pyc Author: roblox-pyc team Author-email:
 roblox.pyc@gmail.com License: GNU AFFERO GENERAL PUBLIC LICENSE Description-
 Content-Type: text/markdown License-File: LICENSE # Introduction  [![All
 Contributors](https://img.shields.io/badge/all_contributors-5-
 orange.svg?style=flat-square)](#contributors-)
                     ## Sponsors  0 sadly ## Contributors
```

### Comparing `roblox-pyc-2.25.113/README.md` & `roblox-pyc-2.26.113/README.md`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/roblox_pyc.egg-info/PKG-INFO` & `roblox-pyc-2.26.113/roblox_pyc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roblox-pyc
-Version: 2.25.113
+Version: 2.26.113
 Summary: The Python, Lunar, C, C++ to Roblox Lua compiler
 Home-page: https://github.com/AsynchronousAI/roblox.pyc
 Author: roblox-pyc team
 Author-email: roblox.pyc@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roblox-pyc Version: 2.25.113 Summary: The Python,
+Metadata-Version: 2.1 Name: roblox-pyc Version: 2.26.113 Summary: The Python,
 Lunar, C, C++ to Roblox Lua compiler Home-page: https://github.com/
 AsynchronousAI/roblox.pyc Author: roblox-pyc team Author-email:
 roblox.pyc@gmail.com License: GNU AFFERO GENERAL PUBLIC LICENSE Description-
 Content-Type: text/markdown License-File: LICENSE # Introduction  [![All
 Contributors](https://img.shields.io/badge/all_contributors-5-
 orange.svg?style=flat-square)](#contributors-)
                     ## Sponsors  0 sadly ## Contributors
```

### Comparing `roblox-pyc-2.25.113/roblox_pyc.egg-info/SOURCES.txt` & `roblox-pyc-2.26.113/roblox_pyc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauAST/bundle.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauAST/bundle.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/List.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauAST/impl/List.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/create.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauAST/impl/create.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/enums.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauAST/impl/enums.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/globals.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauAST/impl/globals.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/typeGuards.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauAST/impl/typeGuards.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauAST/types/mapping.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauAST/types/mapping.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauAST/types/nodes.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauAST/types/nodes.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauAST/util/assert.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauAST/util/assert.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauAST/util/getKindName.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauAST/util/getKindName.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauAST/util/isValidIdentifier.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauAST/util/isValidIdentifier.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/RenderState.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/RenderState.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderFunctionExpression.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderFunctionExpression.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderIfExpression.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderIfExpression.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderStringLiteral.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderStringLiteral.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderUnaryExpression.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/expressions/renderUnaryExpression.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderAssignment.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderAssignment.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderComment.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderComment.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderForStatement.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderForStatement.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderFunctionDeclaration.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderFunctionDeclaration.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderIfStatement.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderIfStatement.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderMethodDeclaration.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderMethodDeclaration.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderNumericForStatement.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderNumericForStatement.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderVariableDeclaration.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/nodes/statements/renderVariableDeclaration.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/render.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/render.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/solveTempIds.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/solveTempIds.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/getEnding.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/getEnding.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/getOrSetDefault.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/getOrSetDefault.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/needsParentheses.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/needsParentheses.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/renderStatements.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/renderStatements.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/visit.ts` & `roblox-pyc-2.26.113/robloxpyc/LuauRenderer/util/visit.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/basecompilers.py` & `roblox-pyc-2.26.113/robloxpyc/basecompilers.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/binopdesc.py` & `roblox-pyc-2.26.113/robloxpyc/binopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/climaker.py` & `roblox-pyc-2.26.113/robloxpyc/climaker.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/cmpopdesc.py` & `roblox-pyc-2.26.113/robloxpyc/cmpopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/cnodevisitor.py` & `roblox-pyc-2.26.113/robloxpyc/cnodevisitor.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/colortext.py` & `roblox-pyc-2.26.113/robloxpyc/colortext.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/config.py` & `roblox-pyc-2.26.113/robloxpyc/config.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/configmanager.py` & `roblox-pyc-2.26.113/robloxpyc/configmanager.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/context.py` & `roblox-pyc-2.26.113/robloxpyc/context.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/errormanager.py` & `roblox-pyc-2.26.113/robloxpyc/errormanager.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/header.py` & `roblox-pyc-2.26.113/robloxpyc/header.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/installationmanager.py` & `roblox-pyc-2.26.113/robloxpyc/installationmanager.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/loader.py` & `roblox-pyc-2.26.113/robloxpyc/loader.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/luainit.py` & `roblox-pyc-2.26.113/robloxpyc/luainit.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/luainitlua.lua` & `roblox-pyc-2.26.113/robloxpyc/luainitlua.lua`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/model.py` & `roblox-pyc-2.26.113/robloxpyc/model.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/nodevisitor.py` & `roblox-pyc-2.26.113/robloxpyc/nodevisitor.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/parser.py` & `roblox-pyc-2.26.113/robloxpyc/parser.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/plugin.py` & `roblox-pyc-2.26.113/robloxpyc/plugin.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/pytranslator.py` & `roblox-pyc-2.26.113/robloxpyc/pytranslator.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/reporter.py` & `roblox-pyc-2.26.113/robloxpyc/reporter.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/robloxpy.py` & `roblox-pyc-2.26.113/robloxpyc/robloxpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 from pyflakes import api
 from packaging import version
 from tqdm import tqdm
 from time import sleep
 
 # FILES
 if __name__ == "__main__":
-  import colortext #ctranslator is old and not used
+  from robloxpyc import colortext #ctranslator is old and not used
 
   # MODULAR
   from errormanager import *
   from installationmanager import *
   from configmanager import *
   from textcompiler import *
   from basecompilers import *
   from util import *
   from plugin import *
   from loader import loader
   from climaker import newIncli, newIncli2, newLanguage
   from wally import wallyget
 else:
-  import colortext #ctranslator is old and not used
+  from . import colortext #ctranslator is old and not used
 
   # MODULAR
   from .errormanager import *
   from .installationmanager import *
   from .configmanager import *
   from .textcompiler import *
   from .basecompilers import *
```

### Comparing `roblox-pyc-2.25.113/robloxpyc/symbolsstack.py` & `roblox-pyc-2.26.113/robloxpyc/symbolsstack.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/textcompiler.py` & `roblox-pyc-2.26.113/robloxpyc/textcompiler.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/unaryopdesc.py` & `roblox-pyc-2.26.113/robloxpyc/unaryopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/util.py` & `roblox-pyc-2.26.113/robloxpyc/util.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/wally.py` & `roblox-pyc-2.26.113/robloxpyc/wally.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/robloxpyc/writer.py` & `roblox-pyc-2.26.113/robloxpyc/writer.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.113/setup.cfg` & `roblox-pyc-2.26.113/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = roblox-pyc
-version = 2.25.113
+version = 2.26.113
 
 [options]
 packages = robloxpyc
 
 [options.entry_points]
 console_scripts = 
 	rblx-py = robloxpyc.robloxpy:w
```

### Comparing `roblox-pyc-2.25.113/setup.py` & `roblox-pyc-2.26.113/setup.py`

 * *Files identical despite different names*

