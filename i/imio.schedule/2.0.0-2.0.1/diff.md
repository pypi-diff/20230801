# Comparing `tmp/imio.schedule-2.0.0.tar.gz` & `tmp/imio.schedule-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imio.schedule-2.0.0.tar", last modified: Mon Jul  3 10:26:18 2023, max compression
+gzip compressed data, was "dist/imio.schedule-2.0.1.tar", last modified: Tue Aug  1 07:54:13 2023, max compression
```

## Comparing `imio.schedule-2.0.0.tar` & `imio.schedule-2.0.1.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/
--rw-r--r--   0 mpeeters   (501) staff       (20)     1443 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/CHANGES.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)       41 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/CONTRIBUTORS.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)       91 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/MANIFEST.in
--rw-r--r--   0 mpeeters   (501) staff       (20)      703 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/Makefile
--rw-r--r--   0 mpeeters   (501) staff       (20)     5036 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/PKG-INFO
--rw-r--r--   0 mpeeters   (501) staff       (20)     1543 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/README.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)     7458 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/bootstrap.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/docs/
--rw-r--r--   0 mpeeters   (501) staff       (20)    18092 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/docs/LICENSE.GPL
--rw-r--r--   0 mpeeters   (501) staff       (20)      658 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/docs/LICENSE.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)       76 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/docs/index.rst
--rw-r--r--   0 mpeeters   (501) staff       (20)      140 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/setup.cfg
--rw-r--r--   0 mpeeters   (501) staff       (20)     1810 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/setup.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/
--rw-r--r--   0 mpeeters   (501) staff       (20)       80 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/__init__.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/
--rw-r--r--   0 mpeeters   (501) staff       (20)      130 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/__init__.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/browser/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/browser/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1071 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/browser/close_task.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1806 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/browser/configure.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/browser/overrides/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/browser/overrides/.gitkeep
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/browser/static/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/browser/static/.gitkeep
--rw-r--r--   0 mpeeters   (501) staff       (20)      175 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/browser/static/overlay.js
--rw-r--r--   0 mpeeters   (501) staff       (20)     1016 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/browser/static/schedule.css
--rw-r--r--   0 mpeeters   (501) staff       (20)     3696 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/browser/task_completion.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1324 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/browser/task_owner.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/browser/templates/
--rw-r--r--   0 mpeeters   (501) staff       (20)      566 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/browser/templates/close_task.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)      577 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/browser/templates/task_change_owner.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)     3167 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/browser/templates/task_completion.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)     5112 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/browser/templates/taskmacros.pt
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/collectionwidget/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/collectionwidget/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      638 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/collectionwidget/configure.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/collectionwidget/templates/
--rw-r--r--   0 mpeeters   (501) staff       (20)     1569 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/collectionwidget/templates/term.pt
--rw-r--r--   0 mpeeters   (501) staff       (20)      439 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/collectionwidget/views.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1266 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/collectionwidget/vocabulary.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      661 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/config.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1316 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/configure.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/content/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     5091 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/condition.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2177 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/conditions.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      362 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2273 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/delay.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      592 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/delay.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     4054 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/logic.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1276 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/logic.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     6337 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/object_factories.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3432 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/object_factories.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2764 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/schedule_config.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1641 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/subform_context_choice.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     8001 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/task.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    46099 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/task_config.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      460 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/view.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      304 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/view.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)    16202 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/vocabulary.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     5614 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/vocabulary.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      616 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/content/widget.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/dashboard/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/dashboard/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     7306 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/dashboard/columns.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2640 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/dashboard/columns.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      178 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/dashboard/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      624 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/dashboard/interfaces.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1386 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/dashboard/vocabulary.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      534 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/dashboard/vocabulary.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/events/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/events/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     5177 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/events/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1810 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/events/create_task.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2864 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/events/dashboard_collection.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2174 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/events/task_config.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     7941 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/events/update_tasks.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     8333 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/events/zope_registration.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      611 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/indexes.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      378 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/indexes.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     4626 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/interfaces.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/locales/
--rw-r--r--   0 mpeeters   (501) staff       (20)      767 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/locales/collective.eeafaceted.z3ctable.pot
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/locales/fr/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/locales/fr/LC_MESSAGES/
--rw-r--r--   0 mpeeters   (501) staff       (20)      666 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.mo
--rw-r--r--   0 mpeeters   (501) staff       (20)      701 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po
--rw-r--r--   0 mpeeters   (501) staff       (20)     8147 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.mo
--rw-r--r--   0 mpeeters   (501) staff       (20)    12139 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.po
--rw-r--r--   0 mpeeters   (501) staff       (20)     9239 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/locales/imio.schedule.pot
--rw-r--r--   0 mpeeters   (501) staff       (20)     1575 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/locales/manual_translations.pot
--rwxr-xr-x   0 mpeeters   (501) staff       (20)      686 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/locales/update.sh
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/migration/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/migration/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      244 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/migration/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      561 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/migration/migrate_to_18.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1047 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/migration/upgrades.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      764 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/migration/upgrades.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/
--rw-r--r--   0 mpeeters   (501) staff       (20)      148 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/browserlayer.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      554 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/catalog.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      490 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/cssregistry.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/imioschedule_default.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)      655 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/jsregistry.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      367 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/metadata.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      231 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/propertiestool.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1595 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/registry.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/types/
--rw-r--r--   0 mpeeters   (501) staff       (20)     2134 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/types/AutomatedMacroTask.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1955 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/types/AutomatedTask.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2193 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/types/MacroTaskConfig.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2193 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/types/ScheduleConfig.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)     2087 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/types/TaskConfig.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      488 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/types.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      369 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/default/workflows.xml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/testing/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/testing/imioschedule_testing.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)      164 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/profiles/testing/metadata.xml
--rw-r--r--   0 mpeeters   (501) staff       (20)      222 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/setuphandlers.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     7829 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/testing.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      782 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/testing.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/tests/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1774 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/condition.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3056 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/conditions.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      396 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      279 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/due_date.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      391 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/due_date.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)      318 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/holidays.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      426 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/logic.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      455 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/logic.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/tests/robot/
--rw-r--r--   0 mpeeters   (501) staff       (20)     1542 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/robot/test_example.robot
--rw-r--r--   0 mpeeters   (501) staff       (20)     9742 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/setup.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1003 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/test_dashboardcollection.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2292 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/test_delay.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     1197 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/test_indexes.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     2792 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/test_logic.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     6586 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/test_registration_events.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     4809 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/test_scheduleconfig.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3294 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/test_setup.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    10523 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/test_task.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    17095 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/test_task_events.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    57639 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/test_taskconfig.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     3361 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/test_utils.py
--rw-r--r--   0 mpeeters   (501) staff       (20)    13257 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/tests/test_vocabulary.py
--rw-r--r--   0 mpeeters   (501) staff       (20)     7360 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/utils.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      847 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/vocabularies.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      461 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/vocabularies.zcml
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio/schedule/workflow/
--rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/workflow/__init__.py
--rw-r--r--   0 mpeeters   (501) staff       (20)      404 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/workflow/configure.zcml
--rw-r--r--   0 mpeeters   (501) staff       (20)     1286 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio/schedule/workflow/freeze_task.py
-drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio.schedule.egg-info/
--rw-r--r--   0 mpeeters   (501) staff       (20)     5036 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio.schedule.egg-info/PKG-INFO
--rw-r--r--   0 mpeeters   (501) staff       (20)     5679 2023-07-03 10:26:18.000000 imio.schedule-2.0.0/src/imio.schedule.egg-info/SOURCES.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        1 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio.schedule.egg-info/dependency_links.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)       53 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio.schedule.egg-info/entry_points.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        5 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio.schedule.egg-info/namespace_packages.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        1 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio.schedule.egg-info/not-zip-safe
--rw-r--r--   0 mpeeters   (501) staff       (20)      240 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio.schedule.egg-info/requires.txt
--rw-r--r--   0 mpeeters   (501) staff       (20)        5 2023-07-03 10:26:17.000000 imio.schedule-2.0.0/src/imio.schedule.egg-info/top_level.txt
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1537 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/CHANGES.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)       41 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/CONTRIBUTORS.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)       91 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/MANIFEST.in
+-rw-r--r--   0 mpeeters   (501) staff       (20)      703 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/Makefile
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3755 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/PKG-INFO
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1543 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/README.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7458 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/bootstrap.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:12.000000 imio.schedule-2.0.1/docs/
+-rw-r--r--   0 mpeeters   (501) staff       (20)    18092 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/docs/LICENSE.GPL
+-rw-r--r--   0 mpeeters   (501) staff       (20)      658 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/docs/LICENSE.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)       76 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/docs/index.rst
+-rw-r--r--   0 mpeeters   (501) staff       (20)      140 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/setup.cfg
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1810 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/setup.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:12.000000 imio.schedule-2.0.1/src/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:12.000000 imio.schedule-2.0.1/src/imio/
+-rw-r--r--   0 mpeeters   (501) staff       (20)       80 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/__init__.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      130 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/__init__.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/browser/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/browser/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1071 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/browser/close_task.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1806 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/browser/configure.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/browser/overrides/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/browser/overrides/.gitkeep
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/browser/static/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/browser/static/.gitkeep
+-rw-r--r--   0 mpeeters   (501) staff       (20)      175 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/browser/static/overlay.js
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1016 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/browser/static/schedule.css
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3696 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/browser/task_completion.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1324 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/browser/task_owner.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/browser/templates/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      566 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/browser/templates/close_task.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      577 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/browser/templates/task_change_owner.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3167 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/browser/templates/task_completion.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5112 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/browser/templates/taskmacros.pt
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/collectionwidget/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/collectionwidget/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      638 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/collectionwidget/configure.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/collectionwidget/templates/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1569 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/collectionwidget/templates/term.pt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      439 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/collectionwidget/views.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1266 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/collectionwidget/vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      661 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1316 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/configure.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/content/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5091 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/condition.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2177 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/conditions.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      362 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2273 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/delay.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      592 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/delay.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4054 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/logic.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1276 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/logic.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     6337 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/object_factories.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3432 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/object_factories.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2764 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/schedule_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1641 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/subform_context_choice.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     8001 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/task.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    46099 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/task_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      460 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/view.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      304 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/view.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)    16202 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5614 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/vocabulary.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      616 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/content/widget.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/dashboard/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/dashboard/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7306 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/dashboard/columns.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2640 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/dashboard/columns.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      178 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/dashboard/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      624 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/dashboard/interfaces.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1386 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/dashboard/vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      534 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/dashboard/vocabulary.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/events/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/events/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5177 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/events/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1810 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/events/create_task.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2864 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/events/dashboard_collection.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2174 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/events/task_config.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7941 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/events/update_tasks.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     8333 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/events/zope_registration.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      611 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/indexes.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      378 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/indexes.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4626 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/interfaces.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/locales/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      767 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/locales/collective.eeafaceted.z3ctable.pot
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:12.000000 imio.schedule-2.0.1/src/imio/schedule/locales/fr/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      666 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.mo
+-rw-r--r--   0 mpeeters   (501) staff       (20)      701 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po
+-rw-r--r--   0 mpeeters   (501) staff       (20)     8147 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.mo
+-rw-r--r--   0 mpeeters   (501) staff       (20)    12139 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.po
+-rw-r--r--   0 mpeeters   (501) staff       (20)     9239 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/locales/imio.schedule.pot
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1575 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/locales/manual_translations.pot
+-rwxr-xr-x   0 mpeeters   (501) staff       (20)      686 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/locales/update.sh
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/migration/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/migration/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      244 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/migration/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      561 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/migration/migrate_to_18.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1047 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/migration/upgrades.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      766 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/migration/upgrades.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:12.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/
+-rw-r--r--   0 mpeeters   (501) staff       (20)      148 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/browserlayer.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      554 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/catalog.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      490 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/cssregistry.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/imioschedule_default.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      655 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/jsregistry.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      367 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/metadata.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      231 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/propertiestool.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1595 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/registry.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/types/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2134 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/types/AutomatedMacroTask.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1955 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/types/AutomatedTask.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2193 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/types/MacroTaskConfig.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2193 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/types/ScheduleConfig.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2087 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/types/TaskConfig.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      488 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/types.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      369 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/default/workflows.xml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/testing/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/testing/imioschedule_testing.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)      164 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/profiles/testing/metadata.xml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      222 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/setuphandlers.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7829 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/testing.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      782 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/testing.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/tests/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1774 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/condition.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3056 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/conditions.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      396 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      279 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/due_date.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      391 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/due_date.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)      318 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/holidays.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      426 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/logic.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      455 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/logic.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/tests/robot/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1542 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/robot/test_example.robot
+-rw-r--r--   0 mpeeters   (501) staff       (20)     9742 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/setup.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1003 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/test_dashboardcollection.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2292 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/test_delay.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1197 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/test_indexes.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     2792 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/test_logic.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     6586 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/test_registration_events.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     4809 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/test_scheduleconfig.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3294 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/test_setup.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    10523 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/test_task.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    17095 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/test_task_events.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    57639 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/test_taskconfig.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3361 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/test_utils.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)    13257 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/tests/test_vocabulary.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)     7360 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/utils.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      847 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/vocabularies.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      461 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/vocabularies.zcml
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio/schedule/workflow/
+-rw-r--r--   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/workflow/__init__.py
+-rw-r--r--   0 mpeeters   (501) staff       (20)      404 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/workflow/configure.zcml
+-rw-r--r--   0 mpeeters   (501) staff       (20)     1286 2023-08-01 07:54:11.000000 imio.schedule-2.0.1/src/imio/schedule/workflow/freeze_task.py
+drwxr-xr-x   0 mpeeters   (501) staff       (20)        0 2023-08-01 07:54:13.000000 imio.schedule-2.0.1/src/imio.schedule.egg-info/
+-rw-r--r--   0 mpeeters   (501) staff       (20)     3755 2023-08-01 07:54:12.000000 imio.schedule-2.0.1/src/imio.schedule.egg-info/PKG-INFO
+-rw-r--r--   0 mpeeters   (501) staff       (20)     5679 2023-08-01 07:54:12.000000 imio.schedule-2.0.1/src/imio.schedule.egg-info/SOURCES.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        1 2023-08-01 07:54:12.000000 imio.schedule-2.0.1/src/imio.schedule.egg-info/dependency_links.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)       40 2023-08-01 07:54:12.000000 imio.schedule-2.0.1/src/imio.schedule.egg-info/entry_points.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        5 2023-08-01 07:54:12.000000 imio.schedule-2.0.1/src/imio.schedule.egg-info/namespace_packages.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        1 2023-08-01 07:54:12.000000 imio.schedule-2.0.1/src/imio.schedule.egg-info/not-zip-safe
+-rw-r--r--   0 mpeeters   (501) staff       (20)      240 2023-08-01 07:54:12.000000 imio.schedule-2.0.1/src/imio.schedule.egg-info/requires.txt
+-rw-r--r--   0 mpeeters   (501) staff       (20)        5 2023-08-01 07:54:12.000000 imio.schedule-2.0.1/src/imio.schedule.egg-info/top_level.txt
```

### Comparing `imio.schedule-2.0.0/CHANGES.rst` & `imio.schedule-2.0.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+2.0.1 (2023-08-01)
+------------------
+
+- Fix order of upgrade steps [URB-2627]
+  [mpeeters]
+
+
 2.0.0 (2023-07-03)
 ------------------
 
 - Migrate to use `collective.eeafaceted.collectionwidget` [URB-2627]
   [mpeeters]
```

### Comparing `imio.schedule-2.0.0/Makefile` & `imio.schedule-2.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/README.rst` & `imio.schedule-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/bootstrap.py` & `imio.schedule-2.0.1/bootstrap.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/docs/LICENSE.GPL` & `imio.schedule-2.0.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/docs/LICENSE.rst` & `imio.schedule-2.0.1/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/setup.py` & `imio.schedule-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     '\n' +
     open('CHANGES.rst').read() +
     '\n')
 
 
 setup(
     name='imio.schedule',
-    version='2.0.0',
+    version='2.0.1',
     description="Schedule for imio products",
     long_description=long_description,
     # Get more from https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: 4.3",
```

### Comparing `imio.schedule-2.0.0/src/imio/schedule/browser/close_task.py` & `imio.schedule-2.0.1/src/imio/schedule/browser/close_task.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/browser/configure.zcml` & `imio.schedule-2.0.1/src/imio/schedule/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/browser/static/schedule.css` & `imio.schedule-2.0.1/src/imio/schedule/browser/static/schedule.css`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/browser/task_completion.py` & `imio.schedule-2.0.1/src/imio/schedule/browser/task_completion.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/browser/task_owner.py` & `imio.schedule-2.0.1/src/imio/schedule/browser/task_owner.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/browser/templates/close_task.pt` & `imio.schedule-2.0.1/src/imio/schedule/browser/templates/close_task.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/browser/templates/task_change_owner.pt` & `imio.schedule-2.0.1/src/imio/schedule/browser/templates/task_change_owner.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/browser/templates/task_completion.pt` & `imio.schedule-2.0.1/src/imio/schedule/browser/templates/task_completion.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/browser/templates/taskmacros.pt` & `imio.schedule-2.0.1/src/imio/schedule/browser/templates/taskmacros.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/collectionwidget/configure.zcml` & `imio.schedule-2.0.1/src/imio/schedule/collectionwidget/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/collectionwidget/templates/term.pt` & `imio.schedule-2.0.1/src/imio/schedule/collectionwidget/templates/term.pt`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/collectionwidget/vocabulary.py` & `imio.schedule-2.0.1/src/imio/schedule/collectionwidget/vocabulary.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/config.py` & `imio.schedule-2.0.1/src/imio/schedule/config.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/configure.zcml` & `imio.schedule-2.0.1/src/imio/schedule/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/condition.py` & `imio.schedule-2.0.1/src/imio/schedule/content/condition.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/conditions.zcml` & `imio.schedule-2.0.1/src/imio/schedule/content/conditions.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/delay.py` & `imio.schedule-2.0.1/src/imio/schedule/content/delay.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/delay.zcml` & `imio.schedule-2.0.1/src/imio/schedule/content/delay.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/logic.py` & `imio.schedule-2.0.1/src/imio/schedule/content/logic.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/logic.zcml` & `imio.schedule-2.0.1/src/imio/schedule/content/logic.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/object_factories.py` & `imio.schedule-2.0.1/src/imio/schedule/content/object_factories.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/object_factories.zcml` & `imio.schedule-2.0.1/src/imio/schedule/content/object_factories.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/schedule_config.py` & `imio.schedule-2.0.1/src/imio/schedule/content/schedule_config.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/subform_context_choice.py` & `imio.schedule-2.0.1/src/imio/schedule/content/subform_context_choice.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/task.py` & `imio.schedule-2.0.1/src/imio/schedule/content/task.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/task_config.py` & `imio.schedule-2.0.1/src/imio/schedule/content/task_config.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/vocabulary.py` & `imio.schedule-2.0.1/src/imio/schedule/content/vocabulary.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/vocabulary.zcml` & `imio.schedule-2.0.1/src/imio/schedule/content/vocabulary.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/content/widget.zcml` & `imio.schedule-2.0.1/src/imio/schedule/content/widget.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/dashboard/columns.py` & `imio.schedule-2.0.1/src/imio/schedule/dashboard/columns.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/dashboard/columns.zcml` & `imio.schedule-2.0.1/src/imio/schedule/dashboard/columns.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/dashboard/interfaces.py` & `imio.schedule-2.0.1/src/imio/schedule/dashboard/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/dashboard/vocabulary.py` & `imio.schedule-2.0.1/src/imio/schedule/dashboard/vocabulary.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/dashboard/vocabulary.zcml` & `imio.schedule-2.0.1/src/imio/schedule/dashboard/vocabulary.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/events/configure.zcml` & `imio.schedule-2.0.1/src/imio/schedule/events/configure.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/events/create_task.py` & `imio.schedule-2.0.1/src/imio/schedule/events/create_task.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/events/dashboard_collection.py` & `imio.schedule-2.0.1/src/imio/schedule/events/dashboard_collection.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/events/task_config.py` & `imio.schedule-2.0.1/src/imio/schedule/events/task_config.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/events/update_tasks.py` & `imio.schedule-2.0.1/src/imio/schedule/events/update_tasks.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/events/zope_registration.py` & `imio.schedule-2.0.1/src/imio/schedule/events/zope_registration.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/indexes.py` & `imio.schedule-2.0.1/src/imio/schedule/indexes.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/interfaces.py` & `imio.schedule-2.0.1/src/imio/schedule/interfaces.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/locales/collective.eeafaceted.z3ctable.pot` & `imio.schedule-2.0.1/src/imio/schedule/locales/collective.eeafaceted.z3ctable.pot`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.mo` & `imio.schedule-2.0.1/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.mo`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po` & `imio.schedule-2.0.1/src/imio/schedule/locales/fr/LC_MESSAGES/collective.eeafaceted.z3ctable.po`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.mo` & `imio.schedule-2.0.1/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.mo`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.po` & `imio.schedule-2.0.1/src/imio/schedule/locales/fr/LC_MESSAGES/imio.schedule.po`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/locales/imio.schedule.pot` & `imio.schedule-2.0.1/src/imio/schedule/locales/imio.schedule.pot`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/locales/manual_translations.pot` & `imio.schedule-2.0.1/src/imio/schedule/locales/manual_translations.pot`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/locales/update.sh` & `imio.schedule-2.0.1/src/imio/schedule/locales/update.sh`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/migration/migrate_to_18.py` & `imio.schedule-2.0.1/src/imio/schedule/migration/migrate_to_18.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/migration/upgrades.py` & `imio.schedule-2.0.1/src/imio/schedule/migration/upgrades.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/migration/upgrades.zcml` & `imio.schedule-2.0.1/src/imio/schedule/migration/upgrades.zcml`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     source="1.7"
     destination="1.8"
     handler=".migrate_to_18.migrate_to_18"
     profile="imio.schedule:default" />
 
   <gs:upgradeStep
     title="Fix marker interface on schedule collections"
-    source="*"
+    source="1.8"
     destination="2"
     handler=".upgrades.upgrade_2_fix_schedule_collection"
     profile="imio.schedule:default" />
 
   <gs:upgradeStep
     title="Set showNumberOfItems value"
     source="2"
```

### Comparing `imio.schedule-2.0.0/src/imio/schedule/profiles/default/catalog.xml` & `imio.schedule-2.0.1/src/imio/schedule/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/profiles/default/jsregistry.xml` & `imio.schedule-2.0.1/src/imio/schedule/profiles/default/jsregistry.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/profiles/default/registry.xml` & `imio.schedule-2.0.1/src/imio/schedule/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/profiles/default/types/AutomatedMacroTask.xml` & `imio.schedule-2.0.1/src/imio/schedule/profiles/default/types/AutomatedMacroTask.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/profiles/default/types/AutomatedTask.xml` & `imio.schedule-2.0.1/src/imio/schedule/profiles/default/types/AutomatedTask.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/profiles/default/types/MacroTaskConfig.xml` & `imio.schedule-2.0.1/src/imio/schedule/profiles/default/types/MacroTaskConfig.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/profiles/default/types/ScheduleConfig.xml` & `imio.schedule-2.0.1/src/imio/schedule/profiles/default/types/ScheduleConfig.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/profiles/default/types/TaskConfig.xml` & `imio.schedule-2.0.1/src/imio/schedule/profiles/default/types/TaskConfig.xml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/testing.py` & `imio.schedule-2.0.1/src/imio/schedule/testing.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/testing.zcml` & `imio.schedule-2.0.1/src/imio/schedule/testing.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/condition.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/condition.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/conditions.zcml` & `imio.schedule-2.0.1/src/imio/schedule/tests/conditions.zcml`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/robot/test_example.robot` & `imio.schedule-2.0.1/src/imio/schedule/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/setup.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/setup.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/test_dashboardcollection.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/test_dashboardcollection.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/test_delay.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/test_delay.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/test_indexes.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/test_indexes.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/test_logic.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/test_logic.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/test_registration_events.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/test_registration_events.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/test_scheduleconfig.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/test_scheduleconfig.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/test_setup.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/test_task.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/test_task_events.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/test_task_events.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/test_taskconfig.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/test_taskconfig.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/test_utils.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/tests/test_vocabulary.py` & `imio.schedule-2.0.1/src/imio/schedule/tests/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/utils.py` & `imio.schedule-2.0.1/src/imio/schedule/utils.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/vocabularies.py` & `imio.schedule-2.0.1/src/imio/schedule/vocabularies.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio/schedule/workflow/freeze_task.py` & `imio.schedule-2.0.1/src/imio/schedule/workflow/freeze_task.py`

 * *Files identical despite different names*

### Comparing `imio.schedule-2.0.0/src/imio.schedule.egg-info/SOURCES.txt` & `imio.schedule-2.0.1/src/imio.schedule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

