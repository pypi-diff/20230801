# Comparing `tmp/slac-alarm-manager-1.2.1.tar.gz` & `tmp/slac-alarm-manager-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slac-alarm-manager-1.2.1.tar", last modified: Tue May 30 16:56:34 2023, max compression
+gzip compressed data, was "slac-alarm-manager-1.2.2.tar", last modified: Tue Aug  1 20:57:22 2023, max compression
```

## Comparing `slac-alarm-manager-1.2.1.tar` & `slac-alarm-manager-1.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:34.712424 slac-alarm-manager-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-30 16:56:34.712424 slac-alarm-manager-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:34.708424 slac-alarm-manager-1.2.1/pydm_alarm_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/pydm_alarm_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/pydm_alarm_plugin/alarm_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:56:34.712424 slac-alarm-manager-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:34.708424 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-05-30 16:56:34.000000 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-30 16:56:34.000000 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:56:34.000000 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-30 16:56:34.000000 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 16:56:34.000000 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 16:56:34.000000 slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:34.708424 slac-alarm-manager-1.2.1/slam/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/alarm_configuration_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/alarm_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/alarm_table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/alarm_table_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/alarm_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/alarm_tree_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/archive_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/kafka_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    14516 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:34.712424 slac-alarm-manager-1.2.1/slam_launcher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam_launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-30 16:56:23.000000 slac-alarm-manager-1.2.1/slam_launcher/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:57:22.824214 slac-alarm-manager-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-01 20:57:22.824214 slac-alarm-manager-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:57:22.820214 slac-alarm-manager-1.2.2/pydm_alarm_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/pydm_alarm_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/pydm_alarm_plugin/alarm_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:57:22.824214 slac-alarm-manager-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:57:22.820214 slac-alarm-manager-1.2.2/slac_alarm_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-08-01 20:57:22.000000 slac-alarm-manager-1.2.2/slac_alarm_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-01 20:57:22.000000 slac-alarm-manager-1.2.2/slac_alarm_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:57:22.000000 slac-alarm-manager-1.2.2/slac_alarm_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-01 20:57:22.000000 slac-alarm-manager-1.2.2/slac_alarm_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-01 20:57:22.000000 slac-alarm-manager-1.2.2/slac_alarm_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-01 20:57:22.000000 slac-alarm-manager-1.2.2/slac_alarm_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:57:22.824214 slac-alarm-manager-1.2.2/slam/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/slam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/slam/alarm_configuration_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/slam/alarm_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/slam/alarm_table_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/slam/alarm_table_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10008 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/slam/alarm_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/slam/alarm_tree_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/slam/archive_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/slam/kafka_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/slam/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/slam/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:57:22.824214 slac-alarm-manager-1.2.2/slam_launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/slam_launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-01 20:57:07.000000 slac-alarm-manager-1.2.2/slam_launcher/main.py
```

### Comparing `slac-alarm-manager-1.2.1/LICENSE.md` & `slac-alarm-manager-1.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.1/PKG-INFO` & `slac-alarm-manager-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slac-alarm-manager
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python interface for managing alarms
 Home-page: https://github.com/slaclab/slac-alarm-manager
 Author: SLAC National Accelerator Laboratory
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `slac-alarm-manager-1.2.1/README.md` & `slac-alarm-manager-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.1/pydm_alarm_plugin/alarm_plugin.py` & `slac-alarm-manager-1.2.2/pydm_alarm_plugin/alarm_plugin.py`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.1/setup.py` & `slac-alarm-manager-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 curr_dir = Path(__file__).parent
 long_description = (curr_dir/'README.md').read_text()
 
 setup(
     name='slac-alarm-manager',
-    version='1.2.1',
+    version='1.2.2',
     description='Python interface for managing alarms',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='SLAC National Accelerator Laboratory',
     url='https://github.com/slaclab/slac-alarm-manager',
     packages=['slam', 'slam_launcher', 'pydm_alarm_plugin'],
     install_requires=['kafka-python', 'pydm', 'qtpy'],
```

### Comparing `slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/PKG-INFO` & `slac-alarm-manager-1.2.2/slac_alarm_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slac-alarm-manager
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python interface for managing alarms
 Home-page: https://github.com/slaclab/slac-alarm-manager
 Author: SLAC National Accelerator Laboratory
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `slac-alarm-manager-1.2.1/slac_alarm_manager.egg-info/SOURCES.txt` & `slac-alarm-manager-1.2.2/slac_alarm_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.1/slam/alarm_configuration_widget.py` & `slac-alarm-manager-1.2.2/slam/alarm_configuration_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,25 +44,27 @@
         self.description_box = QLineEdit(alarm_item.description or '')
 
         self.cant_edit_label = QLabel('Warning: Cannot edit - requires alarm admin privileges')
         self.cant_edit_label.setStyleSheet('background-color: orange')
 
         self.behavior_label = QLabel('Behavior:')
         self.enabled_checkbox = QCheckBox('Enabled')
+        self.enabled_checkbox.clicked.connect(self.update_enabled_checkbox_pre_disabled_value)
+
         self.latch_checkbox = QCheckBox('Latched')
         self.annunciate_checkbox = QCheckBox('Annunciate')
 
         self.disable_date_label = QLabel('Disable Until:')
         self.minimum_datetime = QDateTime.currentDateTime().addDays(-1)
         self.datetime_widget = QDateTimeEdit(self.minimum_datetime)
         self.datetime_widget.setMinimumDateTime(self.minimum_datetime)
         self.datetime_widget.setSpecialValueText(' ')
         self.datetime_widget.setCalendarPopup(True)
 
-        self.datetime_widget.dateTimeChanged.connect(self.uncheck_enabled_box)
+        self.datetime_widget.dateTimeChanged.connect(self.uncheck_enabled_box_when_date_set)
         self.enabled_checkbox.stateChanged.connect(self.clear_datetime_widget)
 
         self.delay_label = QLabel('Alarm Delay (sec)')
         self.delay_spinbox = QSpinBox()
         self.delay_spinbox.setRange(0, 1000000)
         self.delay_spinbox.setFixedWidth(100)
 
@@ -124,14 +126,15 @@
             self.layout.addLayout(self.description_layout)
             self.behavior_layout = QHBoxLayout()
             self.behavior_layout.addWidget(self.behavior_label)
             if type(self.alarm_item.enabled) is bool:
                 self.enabled_checkbox.setChecked(self.alarm_item.enabled)
             elif self.alarm_item.enabled and type(self.alarm_item.enabled) is str:
                 self.enabled_checkbox.setChecked(False)  # Any string here means a disable timeout has been set
+            self.enabled_checkbox_pre_disabled_value = self.enabled_checkbox.isChecked()
             self.behavior_layout.addWidget(self.enabled_checkbox)
             self.latch_checkbox.setChecked(self.alarm_item.latching)
             self.behavior_layout.addWidget(self.latch_checkbox)
             self.annunciate_checkbox.setChecked(self.alarm_item.annunciating)
             self.behavior_layout.addWidget(self.annunciate_checkbox)
             self.layout.addLayout(self.behavior_layout)
             self.disable_layout = QHBoxLayout()
@@ -146,14 +149,17 @@
             if self.alarm_item.delay:
                 self.delay_spinbox.setValue(self.alarm_item.delay)
             self.delay_layout.addWidget(self.delay_spinbox)
             self.layout.addLayout(self.delay_layout)
             self.filter_layout = QHBoxLayout()
             self.filter_layout.addWidget(self.filter_label)
             self.filter_layout.addWidget(self.filter_edit)
+            if self.filter_edit.text():
+                self.enabled_checkbox.setEnabled(False)
+            self.filter_edit.textChanged.connect(self.grey_out_enabled_box_when_filter_set)
             self.layout.addLayout(self.filter_layout)
         self.layout.addWidget(self.guidance_label)
         self.layout.addWidget(self.guidance_table)
         self.layout.addWidget(self.displays_label)
         self.layout.addWidget(self.displays_table)
         self.layout.addWidget(self.commands_label)
         self.layout.addWidget(self.commands_table)
@@ -227,15 +233,38 @@
             self.kafka_producer.send(self.topic,
                                      key=f'config:{self.alarm_item.path}',
                                      value={'user': username, 'host': hostname, 'guidance': guidance,
                                             'displays': displays, 'commands': commands})
 
         self.close()
 
-    def uncheck_enabled_box(self):
+    def grey_out_enabled_box_when_filter_set(self):
+        """
+        Check and grey-out "Enabled" checkbox on config-page when enabling-filter is present.
+        Avoids confusion and keep consistency in regards to if checkbox needs to be checked when adding filter.
+        Assume filter is valid if any text is present in text-edit (no easy way verify). 
+        """
+        editIsEmpty = not self.filter_edit.text()
+        self.enabled_checkbox.setEnabled(editIsEmpty)
+        
+        if editIsEmpty:
+            # reset checkbox to value before getting overridden when user enters filter
+            self.enabled_checkbox.setChecked(self.enabled_checkbox_pre_disabled_value)
+        else:
+            self.enabled_checkbox.setChecked(True)
+
+    def update_enabled_checkbox_pre_disabled_value(self):
+        """ 
+        Grabs the checked/unchecked value of the "Enabled" checkbox, so we know what it was before
+        it was overridden because filter-text was added. For example, if the user had the checkbox un-clicked,
+        then started to add a filter but decided to clear it instead, the checkbox returns to its original value.
+        """
+        self.enabled_checkbox_pre_disabled_value = self.enabled_checkbox.isChecked()
+
+    def uncheck_enabled_box_when_date_set(self):
         """ A simple slot for unchecking the enabled checkbox when the date time widget is set  """
         if self.datetime_widget.dateTime() != self.minimum_datetime:
             self.enabled_checkbox.setChecked(False)
 
     def clear_datetime_widget(self, checkbox_state: int):
         """ A simple slot for clearing out the datetime widget if the enabled checkbox is checked """
         if checkbox_state != 0:
```

### Comparing `slac-alarm-manager-1.2.1/slam/alarm_item.py` & `slac-alarm-manager-1.2.2/slam/alarm_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         Return a QBrush with the appropriate color for drawing this alarm based on severity
 
         Parameters
         ----------
         severity : AlarmSeverity
             The severity to base the display color on
         """
-        if not self.is_enabled():
+        if not self.is_enabled() and self.is_leaf():
             return QBrush(Qt.gray)
         elif severity == AlarmSeverity.OK:
             return QBrush(Qt.darkGreen)
         elif severity == AlarmSeverity.UNDEFINED:
             return QBrush(Qt.magenta)
         elif severity == AlarmSeverity.MAJOR:
             return QBrush(Qt.red)
```

### Comparing `slac-alarm-manager-1.2.1/slam/alarm_table_model.py` & `slac-alarm-manager-1.2.2/slam/alarm_table_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     parent : QObject, optional
         The parent of the table model.
     """
 
     def __init__(self, parent: Optional[QObject] = None):
         super(QAbstractTableModel, self).__init__(parent=parent)
         self.alarm_items = OrderedDict()  # Key (str) to data
-        self.column_names = ('PV', 'Latched Severity', 'Latched Status', 'Description', 'Time', 'Alarm Value',
-                             'Current Severity', 'Current Status')
-        self.column_to_attr = {0: 'name', 1: 'alarm_severity', 2: 'alarm_status', 3: 'description', 4: 'alarm_time',
-                               5: 'alarm_value', 6: 'pv_severity', 7: 'pv_status'}
+        self.column_names = ('PV', 'Latched Severity', 'Current Severity', 'Description', 'Time', 'Value',
+                             'Latched Status', 'Current Status')
+        self.column_to_attr = {0: 'name', 1: 'alarm_severity', 2: 'pv_severity', 3: 'description', 4: 'alarm_time',
+                               5: 'alarm_value', 6: 'alarm_status', 7: 'pv_status'}
 
     def rowCount(self, parent) -> int:
         """ Return the row count of the table """
         if parent is not None and parent.isValid():
             return 0
         return len(self.alarm_items)
 
@@ -65,15 +65,15 @@
             return alarm_item.alarm_severity.value
         elif column_name == 'Latched Status':
             return alarm_item.alarm_status
         elif column_name == 'Description':
             return alarm_item.description
         elif column_name == 'Time':
             return str(alarm_item.alarm_time)
-        elif column_name == 'Alarm Value':
+        elif column_name == 'Value':
             return alarm_item.alarm_value
         elif column_name == 'Current Severity':
             return alarm_item.pv_severity.value
         elif column_name == 'Current Status':
             return alarm_item.pv_status
 
     def headerData(self, section, orientation, role=Qt.DisplayRole):
```

### Comparing `slac-alarm-manager-1.2.1/slam/alarm_table_view.py` & `slac-alarm-manager-1.2.2/slam/alarm_table_view.py`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.1/slam/alarm_tree_model.py` & `slac-alarm-manager-1.2.2/slam/alarm_tree_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from operator import attrgetter
 from qtpy.QtCore import QAbstractItemModel, QModelIndex, QObject, Qt
+from qtpy.QtGui import QBrush
 from typing import List, Optional
 from .alarm_item import AlarmItem, AlarmSeverity
 import logging
 
 logger = logging.getLogger(__name__)
 
 
@@ -49,24 +50,26 @@
                 # Set an indication there is a bypassed alarm somewhere underneath this top level summary
                 all_leaf_nodes = self.get_all_leaf_nodes(alarm_item)
                 for node in all_leaf_nodes:
                     if not node.is_enabled():
                         bypass_indicator = ' *'
                         break
             if not alarm_item.is_enabled():
-                return alarm_item.name + ' (disabled)'
+                return alarm_item.name + ' * (disabled)'
             elif alarm_item.alarm_severity != AlarmSeverity.OK:
                 return alarm_item.name + f'{bypass_indicator} - {alarm_item.alarm_severity.value}/{alarm_item.alarm_status}'
             return alarm_item.name + bypass_indicator
         elif role == Qt.TextColorRole:
             if alarm_item.is_leaf():
                 return alarm_item.display_color(alarm_item.alarm_severity)
             else:
                 all_leaf_nodes = self.get_all_leaf_nodes(alarm_item)
                 highest_severity_alarm = max(all_leaf_nodes, key=attrgetter('alarm_severity'))
+                if not highest_severity_alarm.is_enabled():
+                    return QBrush(Qt.darkGreen)
                 return highest_severity_alarm.display_color(highest_severity_alarm.alarm_severity)
 
     def index(self, row: int, column: int, parent: QModelIndex) -> QModelIndex:
         """ Create an index for the input row and column based on the parent item. """
         if not self.hasIndex(row, column, parent):
             return QModelIndex()
```

### Comparing `slac-alarm-manager-1.2.1/slam/alarm_tree_view.py` & `slac-alarm-manager-1.2.2/slam/alarm_tree_view.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,15 +59,17 @@
         self.context_menu = QMenu(self)
         self.acknowledge_action = QAction('Acknowledge')
         self.unacknowledge_action = QAction('Unacknowledge')
         self.copy_action = QAction('Copy PV To Clipboard')
         self.plot_action = QAction('Draw Plot')
         self.enable_action = QAction('Enable')
         self.disable_action = QAction('Disable')
+        self.guidance_menu = QMenu('Guidance')
         self.display_actions = []
+        self.guidance_objects = []
 
         self.acknowledge_action.triggered.connect(partial(self.send_action, True, None))
         self.unacknowledge_action.triggered.connect(partial(self.send_action, False, None))
         self.plot_action.triggered.connect(self.plot_pv)
         self.copy_action.triggered.connect(self.copy_to_clipboard)
         self.enable_action.triggered.connect(partial(self.send_action, None, True))
         self.disable_action.triggered.connect(partial(self.send_action, None, False))
@@ -109,14 +111,44 @@
                 self.context_menu = QMenu(self)
                 if add_acknowledge_action:  # This always should take precedence over unacknowledge
                     self.context_menu.addAction(self.acknowledge_action)
                 elif add_unacknowledge_action:
                     self.context_menu.addAction(self.unacknowledge_action)
             self.context_menu.addAction(self.enable_action)
             self.context_menu.addAction(self.disable_action)
+            self.context_menu.addMenu(self.guidance_menu)
+    
+            # Make the entires from the config-page appear when alarm in tree is right-clicked
+            indices = self.tree_view.selectedIndexes()
+            alarm_item = self.treeModel.getItem(indices[0])
+
+            self.guidance_objects.clear()
+            has_guidance = False
+            if alarm_item.guidance is not None:
+                guidance_count = 0
+                for index, guidance_item in enumerate(alarm_item.guidance):
+                    has_guidance = True
+                    guidance_count += 1
+ 
+                    curr_title = guidance_item['title']
+                    # sometimes people don't add titles to their guidance notes
+                    if curr_title == "":
+                        curr_title = "Guidance #" + str(guidance_count)
+                    curr_details = guidance_item['details']
+
+                    title_menu = QMenu(curr_title)
+                    self.detail_action = QAction(curr_details)
+                    self.guidance_menu.addMenu(title_menu)
+                    title_menu.addAction(self.detail_action)
+
+                    self.guidance_objects.append(title_menu)
+                    self.guidance_objects.append(self.detail_action)
+
+            self.guidance_menu.menuAction().setVisible(has_guidance)
+
             self.display_actions.clear()
             if alarm_item.displays:
                 for display in alarm_item.displays:
                     display_action = QAction(display['title'])
                     display_action.triggered.connect(partial(self.launch_pydm_display, display['details']))
                     self.context_menu.addAction(display_action)
                     self.display_actions.append(display_action)
```

### Comparing `slac-alarm-manager-1.2.1/slam/archive_search.py` & `slac-alarm-manager-1.2.2/slam/archive_search.py`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.1/slam/kafka_reader.py` & `slac-alarm-manager-1.2.2/slam/kafka_reader.py`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.1/slam/main_window.py` & `slac-alarm-manager-1.2.2/slam/main_window.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,14 +78,22 @@
                                                                    self.plot_pv)
             self.acknowledged_alarm_tables[topic] = AlarmTableViewWidget(self.alarm_trees[topic].treeModel,
                                                                          self.kafka_producer,
                                                                          topic,
                                                                          AlarmTableType.ACKNOWLEDGED,
                                                                          self.plot_pv)
 
+            # Sync the column widths in the active and acknowledged tables, resizing a column will effect both tables.
+            # Managing the width of tables is done with their headers (QHeaderViews). 
+            self.acknowledged_alarm_tables[topic].alarmView.horizontalHeader().sectionResized.connect(\
+                lambda logicalIndex, oldSize, newSize: self.active_alarm_tables[topic].alarmView.horizontalHeader().resizeSection(logicalIndex, newSize))
+
+            self.active_alarm_tables[topic].alarmView.horizontalHeader().sectionResized.connect(\
+                lambda logicalIndex, oldSize, newSize: self.acknowledged_alarm_tables[topic].alarmView.horizontalHeader().resizeSection(logicalIndex, newSize))
+        
         self.alarm_update_signal.connect(self.update_tree)
         self.alarm_update_signal.connect(self.update_table)
 
         self.server_status_timer = QTimer()  # Periodically checks to ensure connection to the alarm server is active
         self.server_status_timer.timeout.connect(self.check_server_status)
         self.server_status_timer.start(3000)
         self.alarm_server_connected = True
```

### Comparing `slac-alarm-manager-1.2.1/slam/permissions.py` & `slac-alarm-manager-1.2.2/slam/permissions.py`

 * *Files identical despite different names*

### Comparing `slac-alarm-manager-1.2.1/slam_launcher/main.py` & `slac-alarm-manager-1.2.2/slam_launcher/main.py`

 * *Files identical despite different names*

