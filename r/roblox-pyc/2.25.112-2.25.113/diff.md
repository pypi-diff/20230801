# Comparing `tmp/roblox-pyc-2.25.112.tar.gz` & `tmp/roblox-pyc-2.25.113.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roblox-pyc-2.25.112.tar", last modified: Mon Jul 31 22:33:52 2023, max compression
+gzip compressed data, was "roblox-pyc-2.25.113.tar", last modified: Tue Aug  1 01:28:44 2023, max compression
```

## Comparing `roblox-pyc-2.25.112.tar` & `roblox-pyc-2.25.113.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.824151 roblox-pyc-2.25.112/
--rw-r--r--   0 runner    (1001) docker     (123)    34525 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-31 22:33:52.824151 roblox-pyc-2.25.112/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.812151 roblox-pyc-2.25.112/roblox_pyc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-31 22:33:52.000000 roblox-pyc-2.25.112/roblox_pyc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-07-31 22:33:52.000000 roblox-pyc-2.25.112/roblox_pyc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 22:33:52.000000 roblox-pyc-2.25.112/roblox_pyc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-31 22:33:52.000000 roblox-pyc-2.25.112/roblox_pyc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-31 22:33:52.000000 roblox-pyc-2.25.112/roblox_pyc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 22:33:52.000000 roblox-pyc-2.25.112/roblox_pyc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.816151 roblox-pyc-2.25.112/robloxpyc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.816151 roblox-pyc-2.25.112/robloxpyc/LuauAST/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/bundle.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.816151 roblox-pyc-2.25.112/robloxpyc/LuauAST/impl/
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/impl/List.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/impl/create.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/impl/enums.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/impl/globals.ts
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/impl/strings.ts
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/impl/typeGuards.ts
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.816151 roblox-pyc-2.25.112/robloxpyc/LuauAST/types/
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/types/mapping.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/types/nodes.ts
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/types/operators.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.820151 roblox-pyc-2.25.112/robloxpyc/LuauAST/util/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/util/assert.ts
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/util/getKindName.ts
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/util/isMetamethod.ts
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/util/isReservedClassField.ts
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/util/isReservedIdentifier.ts
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/util/isValidIdentifier.ts
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauAST/util/isValidNumberLiteral.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.820151 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/RenderState.ts
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.812151 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.820151 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.820151 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/indexable/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderCallExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderComputedIndexExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderIdentifier.ts
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderMethodCallExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderParenthesizedExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderPropertyAccessExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderTemporaryIdentifier.ts
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderArray.ts
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderBinaryExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderFunctionExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderIfExpression.ts
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderMap.ts
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderMixedTable.ts
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderNumberLiteral.ts
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderSet.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderStringLiteral.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderUnaryExpression.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.820151 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/fields/renderMapField.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.824151 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderAssignment.ts
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderBreakStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderCallStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderComment.ts
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderContinueStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderDoStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderForStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderFunctionDeclaration.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderIfStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderMethodDeclaration.ts
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderNumericForStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderRepeatStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderReturnStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderVariableDeclaration.ts
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderWhileStatement.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/render.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/solveTempIds.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.824151 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/getEnding.ts
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/getOrSetDefault.ts
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/getSafeBracketEquals.ts
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/identity.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/needsParentheses.ts
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/renderArguments.ts
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/renderParameters.ts
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/renderStatements.ts
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/visit.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:52.824151 roblox-pyc-2.25.112/robloxpyc/__communication__/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/__communication__/cfg.pkl
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/basecompilers.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/binopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/boolopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8562 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/climaker.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/cmpopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/cnodevisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/colortext.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/configmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/cpAST.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/ctranslator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/errormanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/installationmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/loopcounter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/luainit.py
--rw-r--r--   0 runner    (1001) docker     (123)    28487 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/luainitlua.lua
--rw-r--r--   0 runner    (1001) docker     (123)    49380 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/nameconstdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/nodevisitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    62675 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/pytranslator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    50619 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/robloxpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/symbolsstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/textcompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/tokenendmode.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/unaryopdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/wally.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/robloxpyc/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-31 22:33:52.824151 roblox-pyc-2.25.112/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-31 22:33:43.000000 roblox-pyc-2.25.112/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.237825 roblox-pyc-2.25.113/
+-rw-r--r--   0 runner    (1001) docker     (123)    34525 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-08-01 01:28:44.237825 roblox-pyc-2.25.113/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.225825 roblox-pyc-2.25.113/roblox_pyc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-08-01 01:28:44.000000 roblox-pyc-2.25.113/roblox_pyc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-08-01 01:28:44.000000 roblox-pyc-2.25.113/roblox_pyc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 01:28:44.000000 roblox-pyc-2.25.113/roblox_pyc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-01 01:28:44.000000 roblox-pyc-2.25.113/roblox_pyc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-08-01 01:28:44.000000 roblox-pyc-2.25.113/roblox_pyc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 01:28:44.000000 roblox-pyc-2.25.113/roblox_pyc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.229825 roblox-pyc-2.25.113/robloxpyc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.229825 roblox-pyc-2.25.113/robloxpyc/LuauAST/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/bundle.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/List.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/create.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/enums.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/globals.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/strings.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/typeGuards.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauAST/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/types/mapping.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/types/nodes.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/types/operators.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/assert.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/getKindName.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/isMetamethod.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/isReservedClassField.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/isReservedIdentifier.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/isValidIdentifier.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauAST/util/isValidNumberLiteral.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/RenderState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.225825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderCallExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderComputedIndexExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderIdentifier.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderMethodCallExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderParenthesizedExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderPropertyAccessExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/indexable/renderTemporaryIdentifier.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderArray.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderBinaryExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderFunctionExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderIfExpression.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderMap.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderMixedTable.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderNumberLiteral.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderSet.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderStringLiteral.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderUnaryExpression.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.233825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/fields/renderMapField.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.237825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderAssignment.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderBreakStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderCallStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderComment.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderContinueStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderDoStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderForStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderFunctionDeclaration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderIfStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderMethodDeclaration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderNumericForStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderRepeatStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderReturnStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderVariableDeclaration.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderWhileStatement.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7263 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/render.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/solveTempIds.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.237825 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/getEnding.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/getOrSetDefault.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/getSafeBracketEquals.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/identity.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/needsParentheses.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/renderArguments.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/renderParameters.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/renderStatements.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/visit.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:44.237825 roblox-pyc-2.25.113/robloxpyc/__communication__/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/__communication__/cfg.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/basecompilers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/binopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/boolopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/climaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/cmpopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/cnodevisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/colortext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/configmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/cpAST.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/ctranslator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/errormanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/installationmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/loopcounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/luainit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28487 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/luainitlua.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    49380 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/nameconstdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/nodevisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62675 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/pytranslator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50521 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/robloxpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/symbolsstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/textcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/tokenendmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/unaryopdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/wally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/robloxpyc/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-01 01:28:44.237825 roblox-pyc-2.25.113/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-01 01:28:34.000000 roblox-pyc-2.25.113/setup.py
```

### Comparing `roblox-pyc-2.25.112/LICENSE` & `roblox-pyc-2.25.113/LICENSE`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/PKG-INFO` & `roblox-pyc-2.25.113/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: roblox-pyc
-Version: 2.25.112
+Version: 2.25.113
 Summary: The Python, Lunar, C, C++ to Roblox Lua compiler
 Home-page: https://github.com/AsynchronousAI/roblox.pyc
 Author: roblox-pyc team
 Author-email: roblox.pyc@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Introduction
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 <div align="center">
 
 <figure><img src=".gitbook/assets/Screenshot 2023-07-10 at 12.06.03 AM.png" alt="" width="375"><figcaption></figcaption></figure>
 
 ## Sponsors
@@ -28,14 +28,15 @@
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/AsynchronousAI"><img src="https://avatars.githubusercontent.com/u/72946059?v=4?s=100" width="100px;" alt="aqzp"/><br /><sub><b>aqzp</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/commits?author=AsynchronousAI" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/tututuana"><img src="https://avatars.githubusercontent.com/u/51187395?v=4?s=100" width="100px;" alt="tututuana"/><br /><sub><b>tututuana</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/commits?author=tututuana" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/BazirGames"><img src="https://avatars.githubusercontent.com/u/49544193?v=4?s=100" width="100px;" alt="BazirGames"/><br /><sub><b>BazirGames</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/issues?q=author%3ABazirGames" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://lawmixerscpf.tk/group"><img src="https://avatars.githubusercontent.com/u/53837083?v=4?s=100" width="100px;" alt="LawMixer"/><br /><sub><b>LawMixer</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/issues?q=author%3ALawMixer" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/cataclysmic-dev"><img src="https://avatars.githubusercontent.com/u/141081747?v=4?s=100" width="100px;" alt="cataclysmic-dev"/><br /><sub><b>cataclysmic-dev</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/commits?author=cataclysmic-dev" title="Code">🔨</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: roblox-pyc Version: 2.25.112 Summary: The Python,
+Metadata-Version: 2.1 Name: roblox-pyc Version: 2.25.113 Summary: The Python,
 Lunar, C, C++ to Roblox Lua compiler Home-page: https://github.com/
 AsynchronousAI/roblox.pyc Author: roblox-pyc team Author-email:
 roblox.pyc@gmail.com License: GNU AFFERO GENERAL PUBLIC LICENSE Description-
 Content-Type: text/markdown License-File: LICENSE # Introduction  [![All
-Contributors](https://img.shields.io/badge/all_contributors-4-
+Contributors](https://img.shields.io/badge/all_contributors-5-
 orange.svg?style=flat-square)](#contributors-)
                     ## Sponsors  0 sadly ## Contributors
-                  [aqzp]  [tututuana] [BazirGames] [LawMixer]
-                   aqzp    tututuana   BazirGames   LawMixer
-                   ð�   ð»     ð    ð
+         [aqzp]  [tututuana] [BazirGames] [LawMixer] [cataclysmic-dev]
+          aqzp    tututuana   BazirGames   LawMixer   cataclysmic-dev
+          ð�   ð»     ð    ð      ð¨
 
 ## roblox-pyc [**Docs**](https://robloxpyc.gitbook.io/roblox-pyc) **|**
 [**Devforum**](https://devforum.roblox.com/t/roblox-py-python-luau/
 2457105?u=dev98799) **|** [**Github**](https://github.com/AsynchronousAI/
 roblox.pyc) **|** [**Tests/Examples**](https://github.com/AsynchronousAI/
 roblox.py/tree/main/test) *** ``` pip install roblox-pyc ``` Python, Lunar, C,
 C++ Compiler for Roblox. Python 3.13 (dev), C (all versions), C++ (all
```

### Comparing `roblox-pyc-2.25.112/README.md` & `roblox-pyc-2.25.113/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Introduction
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 <div align="center">
 
 <figure><img src=".gitbook/assets/Screenshot 2023-07-10 at 12.06.03 AM.png" alt="" width="375"><figcaption></figcaption></figure>
 
 ## Sponsors
@@ -17,14 +17,15 @@
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/AsynchronousAI"><img src="https://avatars.githubusercontent.com/u/72946059?v=4?s=100" width="100px;" alt="aqzp"/><br /><sub><b>aqzp</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/commits?author=AsynchronousAI" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/tututuana"><img src="https://avatars.githubusercontent.com/u/51187395?v=4?s=100" width="100px;" alt="tututuana"/><br /><sub><b>tututuana</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/commits?author=tututuana" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/BazirGames"><img src="https://avatars.githubusercontent.com/u/49544193?v=4?s=100" width="100px;" alt="BazirGames"/><br /><sub><b>BazirGames</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/issues?q=author%3ABazirGames" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://lawmixerscpf.tk/group"><img src="https://avatars.githubusercontent.com/u/53837083?v=4?s=100" width="100px;" alt="LawMixer"/><br /><sub><b>LawMixer</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/issues?q=author%3ALawMixer" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/cataclysmic-dev"><img src="https://avatars.githubusercontent.com/u/141081747?v=4?s=100" width="100px;" alt="cataclysmic-dev"/><br /><sub><b>cataclysmic-dev</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/commits?author=cataclysmic-dev" title="Code">🔨</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # Introduction  [![All Contributors](https://img.shields.io/badge/
-all_contributors-4-orange.svg?style=flat-square)](#contributors-)
+all_contributors-5-orange.svg?style=flat-square)](#contributors-)
                     ## Sponsors  0 sadly ## Contributors
-                  [aqzp]  [tututuana] [BazirGames] [LawMixer]
-                   aqzp    tututuana   BazirGames   LawMixer
-                   ð�   ð»     ð    ð
+         [aqzp]  [tututuana] [BazirGames] [LawMixer] [cataclysmic-dev]
+          aqzp    tututuana   BazirGames   LawMixer   cataclysmic-dev
+          ð�   ð»     ð    ð      ð¨
 
 ## roblox-pyc [**Docs**](https://robloxpyc.gitbook.io/roblox-pyc) **|**
 [**Devforum**](https://devforum.roblox.com/t/roblox-py-python-luau/
 2457105?u=dev98799) **|** [**Github**](https://github.com/AsynchronousAI/
 roblox.pyc) **|** [**Tests/Examples**](https://github.com/AsynchronousAI/
 roblox.py/tree/main/test) *** ``` pip install roblox-pyc ``` Python, Lunar, C,
 C++ Compiler for Roblox. Python 3.13 (dev), C (all versions), C++ (all
```

### Comparing `roblox-pyc-2.25.112/roblox_pyc.egg-info/PKG-INFO` & `roblox-pyc-2.25.113/roblox_pyc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: roblox-pyc
-Version: 2.25.112
+Version: 2.25.113
 Summary: The Python, Lunar, C, C++ to Roblox Lua compiler
 Home-page: https://github.com/AsynchronousAI/roblox.pyc
 Author: roblox-pyc team
 Author-email: roblox.pyc@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Introduction
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-4-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-5-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 <div align="center">
 
 <figure><img src=".gitbook/assets/Screenshot 2023-07-10 at 12.06.03 AM.png" alt="" width="375"><figcaption></figcaption></figure>
 
 ## Sponsors
@@ -28,14 +28,15 @@
 <table>
   <tbody>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/AsynchronousAI"><img src="https://avatars.githubusercontent.com/u/72946059?v=4?s=100" width="100px;" alt="aqzp"/><br /><sub><b>aqzp</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/commits?author=AsynchronousAI" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/tututuana"><img src="https://avatars.githubusercontent.com/u/51187395?v=4?s=100" width="100px;" alt="tututuana"/><br /><sub><b>tututuana</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/commits?author=tututuana" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/BazirGames"><img src="https://avatars.githubusercontent.com/u/49544193?v=4?s=100" width="100px;" alt="BazirGames"/><br /><sub><b>BazirGames</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/issues?q=author%3ABazirGames" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://lawmixerscpf.tk/group"><img src="https://avatars.githubusercontent.com/u/53837083?v=4?s=100" width="100px;" alt="LawMixer"/><br /><sub><b>LawMixer</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/issues?q=author%3ALawMixer" title="Bug reports">🐛</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/cataclysmic-dev"><img src="https://avatars.githubusercontent.com/u/141081747?v=4?s=100" width="100px;" alt="cataclysmic-dev"/><br /><sub><b>cataclysmic-dev</b></sub></a><br /><a href="https://github.com/AsynchronousAI/roblox-pyc/commits?author=cataclysmic-dev" title="Code">🔨</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: roblox-pyc Version: 2.25.112 Summary: The Python,
+Metadata-Version: 2.1 Name: roblox-pyc Version: 2.25.113 Summary: The Python,
 Lunar, C, C++ to Roblox Lua compiler Home-page: https://github.com/
 AsynchronousAI/roblox.pyc Author: roblox-pyc team Author-email:
 roblox.pyc@gmail.com License: GNU AFFERO GENERAL PUBLIC LICENSE Description-
 Content-Type: text/markdown License-File: LICENSE # Introduction  [![All
-Contributors](https://img.shields.io/badge/all_contributors-4-
+Contributors](https://img.shields.io/badge/all_contributors-5-
 orange.svg?style=flat-square)](#contributors-)
                     ## Sponsors  0 sadly ## Contributors
-                  [aqzp]  [tututuana] [BazirGames] [LawMixer]
-                   aqzp    tututuana   BazirGames   LawMixer
-                   ð�   ð»     ð    ð
+         [aqzp]  [tututuana] [BazirGames] [LawMixer] [cataclysmic-dev]
+          aqzp    tututuana   BazirGames   LawMixer   cataclysmic-dev
+          ð�   ð»     ð    ð      ð¨
 
 ## roblox-pyc [**Docs**](https://robloxpyc.gitbook.io/roblox-pyc) **|**
 [**Devforum**](https://devforum.roblox.com/t/roblox-py-python-luau/
 2457105?u=dev98799) **|** [**Github**](https://github.com/AsynchronousAI/
 roblox.pyc) **|** [**Tests/Examples**](https://github.com/AsynchronousAI/
 roblox.py/tree/main/test) *** ``` pip install roblox-pyc ``` Python, Lunar, C,
 C++ Compiler for Roblox. Python 3.13 (dev), C (all versions), C++ (all
```

### Comparing `roblox-pyc-2.25.112/roblox_pyc.egg-info/SOURCES.txt` & `roblox-pyc-2.25.113/roblox_pyc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauAST/bundle.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauAST/bundle.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauAST/impl/List.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/List.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauAST/impl/create.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/create.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauAST/impl/enums.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/enums.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauAST/impl/globals.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/globals.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauAST/impl/typeGuards.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauAST/impl/typeGuards.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauAST/types/mapping.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauAST/types/mapping.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauAST/types/nodes.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauAST/types/nodes.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauAST/util/assert.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauAST/util/assert.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauAST/util/getKindName.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauAST/util/getKindName.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauAST/util/isValidIdentifier.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauAST/util/isValidIdentifier.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/RenderState.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/RenderState.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderFunctionExpression.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderFunctionExpression.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderIfExpression.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderIfExpression.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderStringLiteral.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderStringLiteral.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/expressions/renderUnaryExpression.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/expressions/renderUnaryExpression.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderAssignment.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderAssignment.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderComment.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderComment.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderForStatement.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderForStatement.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderFunctionDeclaration.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderFunctionDeclaration.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderIfStatement.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderIfStatement.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderMethodDeclaration.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderMethodDeclaration.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderNumericForStatement.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderNumericForStatement.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/nodes/statements/renderVariableDeclaration.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/nodes/statements/renderVariableDeclaration.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/render.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/render.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/solveTempIds.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/solveTempIds.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/getEnding.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/getEnding.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/getOrSetDefault.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/getOrSetDefault.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/needsParentheses.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/needsParentheses.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/renderStatements.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/renderStatements.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/LuauRenderer/util/visit.ts` & `roblox-pyc-2.25.113/robloxpyc/LuauRenderer/util/visit.ts`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/basecompilers.py` & `roblox-pyc-2.25.113/robloxpyc/basecompilers.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/binopdesc.py` & `roblox-pyc-2.25.113/robloxpyc/binopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/climaker.py` & `roblox-pyc-2.25.113/robloxpyc/climaker.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # TODO
 
 import sys
 
 import os 
+
+from platform import uname
+
 if not (os.path.dirname(os.path.abspath(__file__)).startswith(sys.path[-1])):
     from loader import loader
     from textcompiler import *
     from configmanager import *
     from util import *
     from basecompilers import *
 else:
@@ -110,14 +113,21 @@
       action = input("")
       if action == "exit":
         exit(0)
       else:
         incli2()              
   return incli2
 
+def replaceLuaFiles(r, file, basefile, commentart, luafilecontents):
+  # create new file with same name but  .py and write the lua file contents to it
+  open(os.path.join(r, file.replace(".lua", basefile)), "x").close()
+  # write the old file contents as a py comment
+  open(os.path.join(r, file.replace(".lua", basefile)), "w").write(commentart.format(luafilecontents))
+  print(colortext.green("Converted to py "+os.path.join(r, file)+" as "+file.replace(".lua", basefile)))
+
 def newLanguage(basefile, func, commentart, p=None):
     def w():
       try:
         incli = newIncli(basefile, func)
         incli2 = newIncli2(basefile, func)
         
         if sys.argv.__len__() >= 1:
@@ -140,32 +150,55 @@
                 for file in f:
                   if '.lua' in file:
                     luafilecontents = ""
                     with open(os.path.join(r, file), "r") as f:
                       luafilecontents = f.read()
                       
                     os.remove(os.path.join(r, file))
+                    replaceLuaFiles(r, file, basefile, commentart, luafilecontents)
                     
-                    # create new file with same name but  .py and write the lua file contents to it
-                    open(os.path.join(r, file.replace(".lua", basefile)), "x").close()
-                    # write the old file contents as a py comment
-                    open(os.path.join(r, file.replace(".lua", basefile)), "w").write(commentart.format(luafilecontents))
-                    print(colortext.green("Converted to py "+os.path.join(r, file)+" as "+file.replace(".lua", basefile)))
           elif sys.argv[1] == "cd":
             # Duplicate the cwd directory, the original will be renamed to -compiled and the new one will be renamed to the original. For the new one, go through every lua descendant file in the current directory and delete it and create a new file with the same name but .py
             confirm = input(warn("Are you sure? This will duplicate the current directory and compile the files in the new directory.\n\nType 'yes' to continue."))
-            if confirm == "yes":
+            if confirm == "yes" and uname().system == "Windows":
+              # check if cwd/default.project.json exists, if it does, then use that as the default project file
+              #if os.path.exists(os.getcwd()+"/default.project.json"):
+              #  formatdefaultproj(os.getcwd()+"/default.project.json")
+              # rename directory to -compiled
+              path_name = os.getcwd()
+              #os.rename(path_name, path_name+"-compiled")
+              # duplicate the directory, remove the -compiled from the end
+              shutil.copytree(path_name, path_name + "-compiled")
+              # now we have 2 identical directories, one with -compiled and one without. for the one without, go through every lua descendant file in the current directory and delete it and create a new file with the same name but .py
+              path = os.getcwd()
+
+              for r, d, f in os.walk(backwordreplace(path, "-compiled", "", 1)):
+                for file in f:
+                  if '.lua' in file:
+                    luafilecontents = ""
+                    with open(os.path.join(r, file), "r") as f:
+                      luafilecontents = f.read()
+                      
+                    os.remove(os.path.join(r, file))
+                    replaceLuaFiles(r, file, basefile, commentart, luafilecontents)
+              # create a .rpyc file in the non -compiled directory
+              open(os.path.join(backwordreplace(path, "-compiled", "", 1), ".rpyc"), "x").close()
+              # set cwd to not -compiled
+              os.chdir(backwordreplace(path, "-compiled", "", 1))
+              print(info("Completed! You may need to modify the default.package.json or any other equivalent file to make it use the -compiled directory rather than the original."))
+            elif confirm == "yes":
+              # note by CataclysmicDev -> i left this old code here just to make sure its stable on unix but you can delete it and see if the above code works on unix too
               path = os.path.join(os.getcwd(), "src")
               # check if cwd/default.project.json exists, if it does, then use that as the default project file
               #if os.path.exists(os.getcwd()+"/default.project.json"):
               #  formatdefaultproj(os.getcwd()+"/default.project.json")
               # rename directory to -compiled
-              os.rename(path, path+"-compiled")
+              os.rename(path_name, path_name+"-compiled")
               # duplicate the directory, remove the -compiled from the end
-              shutil.copytree(path+"-compiled", path)
+              shutil.copytree(path_name + "-compiled", path_name)
               # now we have 2 identical directories, one with -compiled and one without. for the one without, go through every lua descendant file in the current directory and delete it and create a new file with the same name but .py
               path = os.getcwd()
 
               for r, d, f in os.walk(backwordreplace(path, "-compiled", "", 1)):
                 for file in f:
                   if '.lua' in file:
                     luafilecontents = ""
@@ -193,8 +226,8 @@
             incli2()
           
       except IndexError:
         print(error("Invalid amount of arguments!", "roblox-py"))
       except KeyboardInterrupt:
         print(colortext.red("Aborted!"))
         sys.exit(0)
-    return w
+    return w
```

### Comparing `roblox-pyc-2.25.112/robloxpyc/cmpopdesc.py` & `roblox-pyc-2.25.113/robloxpyc/cmpopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/cnodevisitor.py` & `roblox-pyc-2.25.113/robloxpyc/cnodevisitor.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/colortext.py` & `roblox-pyc-2.25.113/robloxpyc/colortext.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/config.py` & `roblox-pyc-2.25.113/robloxpyc/config.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/configmanager.py` & `roblox-pyc-2.25.113/robloxpyc/configmanager.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/context.py` & `roblox-pyc-2.25.113/robloxpyc/context.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/errormanager.py` & `roblox-pyc-2.25.113/robloxpyc/errormanager.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/header.py` & `roblox-pyc-2.25.113/robloxpyc/header.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/installationmanager.py` & `roblox-pyc-2.25.113/robloxpyc/installationmanager.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/loader.py` & `roblox-pyc-2.25.113/robloxpyc/loader.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/luainit.py` & `roblox-pyc-2.25.113/robloxpyc/luainit.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/luainitlua.lua` & `roblox-pyc-2.25.113/robloxpyc/luainitlua.lua`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/model.py` & `roblox-pyc-2.25.113/robloxpyc/model.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/nodevisitor.py` & `roblox-pyc-2.25.113/robloxpyc/nodevisitor.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/parser.py` & `roblox-pyc-2.25.113/robloxpyc/parser.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/plugin.py` & `roblox-pyc-2.25.113/robloxpyc/plugin.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/pytranslator.py` & `roblox-pyc-2.25.113/robloxpyc/pytranslator.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/reporter.py` & `roblox-pyc-2.25.113/robloxpyc/reporter.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/robloxpy.py` & `roblox-pyc-2.25.113/robloxpyc/robloxpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 from pyflakes import api
 from packaging import version
 from tqdm import tqdm
 from time import sleep
 
 # FILES
 if __name__ == "__main__":
-  from robloxpyc import pytranslator, colortext, luainit, parser, ctranslator, header #ctranslator is old and not used
+  import colortext #ctranslator is old and not used
 
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
-  from . import pytranslator, colortext, luainit, parser, ctranslator, header #ctranslator is old and not used
+  import colortext #ctranslator is old and not used
 
   # MODULAR
   from .errormanager import *
   from .installationmanager import *
   from .configmanager import *
   from .textcompiler import *
   from .basecompilers import *
@@ -666,18 +666,18 @@
   if action == "exit":
     exit(0)
   else:
     globalincli2()
 """
 
 
-w = newLanguage("py", pycompile, '"""%s"""')
-cw = newLanguage("c", ccompile, '/*%s*/')
-cpw = newLanguage("cpp", cppcompile, '/*%s*/')
-lunar = newLanguage("moon", lunarcompile, '--[[%s]]')
+w = newLanguage(".py", pycompile, '"""%s"""')
+cw = newLanguage(".c", ccompile, '/*%s*/')
+cpw = newLanguage(".cpp", cppcompile, '/*%s*/')
+lunar = newLanguage(".moon", lunarcompile, '--[[%s]]')
 
 globalincli = newIncli(["py", "c", "cpp", "moon"], allcompile)
 globalincli2 = newIncli2(["py", "c", "cpp", "moon"], allcompile)
 
 def pyc():
   title = colortext.magenta("roblox-pyc", ["bold"])
   py = colortext.blue("roblox-py", ["bold"])
@@ -687,14 +687,15 @@
   border = colortext.white("--------------------")
   blank = colortext.blue("roblox-", ["bold"])+colortext.magenta("<lang>")
   blank2 = colortext.blue("rblx-", ["bold"])+colortext.magenta("<lang>")
   blankpath = colortext.magenta("<path>")
   selftool = colortext.blue("roblox-pyc", ["bold"])
   shortselftool = colortext.blue("rblx-pyc", ["bold"])
   shorterselftool = colortext.blue("rpyc", ["bold"])
+  print(str(sys.argv))
   try:
     if sys.argv[1] == "config":
       # Open config menu
       print(f"""
 Config menu
 {border} 
 1 - {py}
@@ -1119,8 +1120,8 @@
     cw()
   elif mode == "3":
     cpw()
   elif mode == "4":
     lunar()
   else:
     pyc()
-  
+
```

### Comparing `roblox-pyc-2.25.112/robloxpyc/symbolsstack.py` & `roblox-pyc-2.25.113/robloxpyc/symbolsstack.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/textcompiler.py` & `roblox-pyc-2.25.113/robloxpyc/textcompiler.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/unaryopdesc.py` & `roblox-pyc-2.25.113/robloxpyc/unaryopdesc.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/util.py` & `roblox-pyc-2.25.113/robloxpyc/util.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/wally.py` & `roblox-pyc-2.25.113/robloxpyc/wally.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/robloxpyc/writer.py` & `roblox-pyc-2.25.113/robloxpyc/writer.py`

 * *Files identical despite different names*

### Comparing `roblox-pyc-2.25.112/setup.cfg` & `roblox-pyc-2.25.113/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = roblox-pyc
-version = 2.25.112
+version = 2.25.113
 
 [options]
 packages = robloxpyc
 
 [options.entry_points]
 console_scripts = 
 	rblx-py = robloxpyc.robloxpy:w
```

### Comparing `roblox-pyc-2.25.112/setup.py` & `roblox-pyc-2.25.113/setup.py`

 * *Files identical despite different names*

