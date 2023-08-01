# Comparing `tmp/dearpyapp-0.1.3-py3-none-win_amd64.whl.zip` & `tmp/dearpyapp-0.1.4-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 19858 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat      460 b- defN 23-Jul-21 07:57 dearpyapp/__init__.py
--rw-rw-rw-  2.0 fat    10777 b- defN 23-Jul-21 07:57 dearpyapp/application.py
--rw-rw-rw-  2.0 fat     2328 b- defN 23-Jul-21 07:57 dearpyapp/colors.py
--rw-rw-rw-  2.0 fat     8883 b- defN 23-Jul-21 07:57 dearpyapp/themes.py
--rw-rw-rw-  2.0 fat     9102 b- defN 23-Jul-21 07:57 dearpyapp/utils.py
--rw-rw-rw-  2.0 fat      105 b- defN 23-Jul-21 07:57 dearpyapp/components/__init__.py
--rw-rw-rw-  2.0 fat    12649 b- defN 23-Jul-21 07:57 dearpyapp/components/log.py
--rw-rw-rw-  2.0 fat    12733 b- defN 23-Jul-21 07:57 dearpyapp/components/port_control.py
--rw-rw-rw-  2.0 fat     6455 b- defN 23-Jul-21 07:57 dearpyapp/components/tab.py
--rw-rw-rw-  2.0 fat     1096 b- defN 23-Jul-21 07:57 dearpyapp-0.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      864 b- defN 23-Jul-21 07:57 dearpyapp-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-Jul-21 07:57 dearpyapp-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jul-21 07:57 dearpyapp-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1132 b- defN 23-Jul-21 07:57 dearpyapp-0.1.3.dist-info/RECORD
-14 files, 66692 bytes uncompressed, 17988 bytes compressed:  73.0%
+Zip file size: 20519 bytes, number of entries: 14
+-rw-rw-rw-  2.0 fat      460 b- defN 23-Aug-01 10:34 dearpyapp/__init__.py
+-rw-rw-rw-  2.0 fat    10777 b- defN 23-Aug-01 10:34 dearpyapp/application.py
+-rw-rw-rw-  2.0 fat     2622 b- defN 23-Aug-01 10:34 dearpyapp/colors.py
+-rw-rw-rw-  2.0 fat     8883 b- defN 23-Aug-01 10:34 dearpyapp/themes.py
+-rw-rw-rw-  2.0 fat    10757 b- defN 23-Aug-01 10:34 dearpyapp/utils.py
+-rw-rw-rw-  2.0 fat      105 b- defN 23-Aug-01 10:34 dearpyapp/components/__init__.py
+-rw-rw-rw-  2.0 fat    13513 b- defN 23-Aug-01 10:34 dearpyapp/components/log.py
+-rw-rw-rw-  2.0 fat    12733 b- defN 23-Aug-01 10:34 dearpyapp/components/port_control.py
+-rw-rw-rw-  2.0 fat     6455 b- defN 23-Aug-01 10:34 dearpyapp/components/tab.py
+-rw-rw-rw-  2.0 fat     1096 b- defN 23-Aug-01 10:34 dearpyapp-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      900 b- defN 23-Aug-01 10:34 dearpyapp-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-Aug-01 10:34 dearpyapp-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Aug-01 10:34 dearpyapp-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1133 b- defN 23-Aug-01 10:34 dearpyapp-0.1.4.dist-info/RECORD
+14 files, 69542 bytes uncompressed, 18649 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: dearpyapp/components/port_control.py
 Comment: 
 
 Filename: dearpyapp/components/tab.py
 Comment: 
 
-Filename: dearpyapp-0.1.3.dist-info/LICENSE
+Filename: dearpyapp-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: dearpyapp-0.1.3.dist-info/METADATA
+Filename: dearpyapp-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: dearpyapp-0.1.3.dist-info/WHEEL
+Filename: dearpyapp-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: dearpyapp-0.1.3.dist-info/top_level.txt
+Filename: dearpyapp-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: dearpyapp-0.1.3.dist-info/RECORD
+Filename: dearpyapp-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dearpyapp/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.3'
+__version__ = '0.1.4'
 
 from . import colors as c
 from .application import DpgApp, get_running_app
 from .themes import (
     dpg_get_color_theme,
     dpg_get_default_theme
 )
```

## dearpyapp/colors.py

```diff
@@ -1,10 +1,11 @@
 import typing as t
 import sys
 
+# TODO rename colors variables to background, forground, accent, error, etc...
 black_theme = True
 
 NONE = (-255, 0, 0, 255)
 TRANSPARENT = (0, 0, 0, 0)
 BLACK = (0, 0, 0, 255)
 WHITE = (255, 255, 255, 255)
 
@@ -15,66 +16,73 @@
     GRAY_3 = (240, 240, 240, 255)
     GRAY_4 = (220, 220, 220, 255)
     GRAY_5 = (210, 210, 210, 255)
     GRAY_6 = (200, 200, 200, 255)
     GRAY_8 = (155, 155, 155, 255)
     GRAY_10 = (150, 150, 150, 255)
     GRAY_12 = (130, 130, 130, 255)
+    GRAY_16 = (120, 120, 120, 255)
     GRAY_14 = (115, 115, 115, 255)
     GRAY_18 = (43, 43, 43, 255)
     GRAY_20 = (32, 32, 32, 255)
     GRAY_22 = (15, 15, 15, 255)
     GRAY_25 = (0, 0, 0, 255)
 
+    BLUE_4 = (180, 230, 255, 255)
     BLUE_9 = (175, 226, 251, 255)
     BLUE_12 = (129, 194, 247, 255)
     BLUE_15 = (100, 163, 217, 255)
     BLUE_18 = (18, 81, 153, 255)
 
     YELLOW_17 = (220, 110, 0, 255)
     YELLOW_19 = (255, 115, 0, 255)
 
     RED_9 = (236, 173, 173, 255)
     RED_20 = (200, 30, 41, 255)
     RED_23 = (160, 20, 30, 255)
 
     GREEN_6 = (170, 235, 170, 255)
+    GREEN_18 = (30, 130, 30, 255)
     GREEN_20 = (17, 110, 25, 255)
     GREEN_23 = (10, 85, 25, 255)
+
 else:
     GRAY_0 = (0, 0, 0, 255)  # not used
     GRAY_1 = (17, 17, 17, 255)  # not used
     GRAY_2 = (25, 25, 25, 255)
     GRAY_3 = (32, 32, 32, 255)
     GRAY_4 = (43, 43, 43, 255)
     GRAY_5 = (50, 50, 50, 255)
     GRAY_6 = (65, 65, 65, 255)
     GRAY_8 = (87, 87, 87, 255)
     GRAY_10 = (100, 100, 100, 255)
     GRAY_12 = (120, 120, 120, 255)
     GRAY_14 = (140, 140, 140, 255)
+    GRAY_16 = (160, 160, 160, 255)
     GRAY_18 = (180, 180, 180, 255)
     GRAY_20 = (200, 200, 200, 255)
     GRAY_22 = (220, 220, 220, 255)
     GRAY_25 = (250, 250, 250, 255)
 
+    BLUE_4 = (25, 35, 45, 255)
     BLUE_9 = (38, 70, 95, 255)
     BLUE_12 = (43, 82, 120, 255)
     BLUE_15 = (55, 110, 155, 255)
     BLUE_18 = (68, 140, 186, 255)
 
-    YELLOW_17 = (173, 173, 42, 255)
-    YELLOW_19 = (190, 190, 45, 255)
+    YELLOW_17 = (173, 173, 75, 255)
+    YELLOW_19 = (190, 190, 75, 255)
 
-    RED_9 = (90, 20, 20, 255)
-    RED_20 = (200, 50, 50, 255)
-    RED_23 = (235, 55, 65, 255)
-
-    GREEN_6 = (10, 65, 10, 255)
-    GREEN_20 = (50, 200, 50, 255)
-    GREEN_23 = (55, 230, 65, 255)
+    RED_9 = (90, 30, 20, 255)
+    RED_20 = (200, 70, 50, 255)
+    RED_23 = (235, 85, 65, 255)
+
+    GREEN_6 = (30, 65, 35, 255)
+    GREEN_18 = (95, 180, 90, 255)
+    GREEN_20 = (100, 200, 95, 255)
+    GREEN_23 = (105, 230, 100, 255)
 
 
 def to_hex_rgb(color: t.Union[list, tuple]):
     return ''.join((f'{num:02x}' for index, num in enumerate(color) if index != 3))
```

## dearpyapp/utils.py

```diff
@@ -196,28 +196,73 @@
                     dpg.set_value(getattr(gui_obj_, tag_), getattr(val_obj_, tag_))
             else:
                 dpg.set_value(gui_obj_, val_obj_)
         else:
             dpg_set_values(gui_obj_, val_obj_)
 
 
-def _get_wrapped_text(text, wrap, font):
-    text_size = start_index = 0
+def _process_split_indexes(split_indexes: list) -> list:
+    index = len(split_indexes)
+    expected_index = None
+    for _, split_index, _ in reversed(split_indexes):
+        if expected_index is not None and split_index != expected_index:
+            break
+        expected_index = split_index - 1
+        index -= 1
+    if index != len(split_indexes) - 1:
+        for i in range(index + 1, len(split_indexes)):
+            is_whitespace_char, *_ = split_indexes[i]
+            if not is_whitespace_char:
+                break
+            index += 1
+    return split_indexes[index:]
+
+
+def _get_wrapped_text(text: str, wrap: int, font: int):
+    delimeters = {',', ';', '.', '?', '!', '\"'}
+    whitespaces = (' ', '\t')
+    split_indexes = []
+    start_index = 0
+    text_size = 0
     wrapped_text = []
     for char_index, char in enumerate(text):
+        previous_text_size = text_size
         text_size += dpg.get_text_size(char, font=font)[0]
-        if char == '\n' or (wrap and text_size > wrap):
-            wrapped_text.append(text[start_index: char_index])
-            start_index = char_index + 1 if char == '\n' else char_index
+        is_whitespace_char = char in whitespaces
+        is_split_char = is_whitespace_char or (char in delimeters)
+
+        if char == '\n':
+            split_indexes.clear()
             text_size = 0
+        elif not is_whitespace_char and wrap and text_size > wrap:
+            while True:
+                if split_indexes:
+                    split_indexes = _process_split_indexes(split_indexes)
+                    _, stop_index, split_chunk_size = split_indexes.pop(0)
+                    for index in range(len(split_indexes)):
+                        split_indexes[index][2] -= split_chunk_size
+                else:
+                    stop_index = char_index
+                    split_chunk_size = previous_text_size
+
+                wrapped_text.append(text[start_index: stop_index])
+                start_index = stop_index
+                text_size -= split_chunk_size
+                if text_size <= wrap:
+                    break
+
+        if is_split_char:
+            split_indexes.append([is_whitespace_char, char_index + 1, text_size])
+
     wrapped_text.append(text[start_index:])
-    return '\n'.join(wrapped_text)
+
+    return '\r\n'.join(wrapped_text)
 
 
-def dpg_get_text_from_cell(cell, wrap=-1, font=0):
+def dpg_get_text_from_cell(cell: int, wrap: int = -1, font: int = 0):
     if (item_type := dpg_get_item_type(cell)) == dpg.mvText:
         text = dpg.get_value(cell)
         width, height = dpg.get_text_size(text, font=font, wrap_width=wrap)
     elif item_type != dpg.mvGroup:
         return None, 0, 0
     else:
         width, height = dpg.get_item_rect_size(cell)
```

## dearpyapp/components/log.py

```diff
@@ -1,43 +1,41 @@
 import asyncio
+import typing as t
 
 import dearpygui.dearpygui as dpg
 from dearpyapp import *
-import typing as t
+import pyperclip
 
 
 class TableLog:
+    # TODO callumns_info in dataclass, wrap parameter
     # TODO для скрытия колнки dpg.configure_item(col, show=True, enabled=False)
     # TODO передавать теги стиля текста, как в html
-    # TODO сделать враппер текста общий для dpg.text и dpg.input_text врапить через '\r\n' и
-    #  эти символы удалять при копировании через ctrl-c и при dpg.get_value
     # TODO не обновлять лог, если таблица не отрисовывалась (get_available_content_region(table_window) == [0, 0])
     # TODO не обновлять лог, если таблица не видна
     # TODO если строк в таблице больше ~900 и ее видно, то ctrl-c на любом input_text приводит к
     #  зависанию(коллбэки не обрабатываются, буфер обмена в других приложениях не работает), если установить в
     #  таблице clipper=True, то все ок, сейчас при больше 900, включается клиппер
-    # TODO callumns_info in dataclass
     # TODO dpg.clipper для таблиц, так как если таблица видна, то на обновление тратится много ресурсов
-    # TODO сделать кнопку вниз))
     # TODO horizontal scroll + autofit all
     # TODO сделать скрываемые колонки, попробовать использовать нативные хедеры
-    # TODO переделать ресайз, не по каждому релизу кнопки, а по релизу, если нажимали на хедер
-    #  или менялся размер окна/внешней таблицы
-    # TODO scrollsize запрашивать
+
     columns = []
     scroll_size = 20
 
     def __init__(self, *, log_size=100):
         self.gui = self._Gui()
         self.log_size = log_size
         self.column_widths = [0] * len(self.columns)
         self.wrap_text = True
         self.rows: dict[int, list[int]] = {}
-        self.input_text_row = None
-        self.input_text_cell = None
+        self.show_scroll_to_end_btn = False
+        self._selected_row_index = -1
+        self._input_text_row = None
+        self._input_text_cell = None
 
     # TODO сделать по-нормальному
     async def _task(self):
         while True:
             try:
                 self._width_changed()
             except SystemError:
@@ -49,40 +47,46 @@
         gui = self.gui
         if not dpg.is_item_visible(gui.group):
             return
 
         dpg.configure_item(gui.table_group,
                            width=dpg.get_available_content_region(gui.table_window)[0])
         len_columns = len(self.columns)
+        group = 0
         for group, column, index in zip(dpg.get_item_children(dpg.get_item_children(gui.header, 1)[0], 1),
                                         dpg.get_item_children(gui.table, 0), range(len_columns)):
             actual_width = dpg.get_available_content_region(group)[0] - 4
             actual_width = actual_width if index != len_columns - 1 else \
-                    actual_width - self.scroll_size
+                actual_width - self.scroll_size
             if self.column_widths[index] != actual_width:
                 self._input_text_cleanup()
                 self.column_widths[index] = actual_width
                 dpg.configure_item(column, init_width_or_weight=actual_width + 4,)
                 # TODO нормально сделать колонки, где нужно wrap делать
                 if self.wrap_text:
                     for row in dpg.get_item_children(gui.table, 1):
                         fields = dpg.get_item_children(row, 1)
                         if len(fields) - 1 < index or dpg_get_item_type(fields[index]) != dpg.mvText:
                             continue
                         dpg.configure_item(fields[index], wrap=actual_width)
-                # dpg.set_y_scroll(gui.table_window, -1)
+
+        if group != 0 and self.show_scroll_to_end_btn:
+            x, y = dpg.get_item_pos(group)
+            dpg.configure_item(
+                gui.scroll_to_end_btn,
+                pos=(x + dpg.get_item_rect_size(group)[0] - 20, y),
+                show=dpg.get_y_scroll_max(gui.table_window) != dpg.get_y_scroll(gui.table_window))
 
     def append(self, data):
         self.extend((data, ))
 
     def extend(self, iterable: t.Iterable):
         if not dpg.does_item_exist(self.gui.group):
             return
 
-        last_index = len(self.columns) - 1
         with dpg.mutex():
             with dpg_container(self.gui.table):
                 for data in iterable:
                     if not (data := self._process_data(data)):
                         continue
                     with dpg.table_row() as row:
                         fields = []
@@ -93,82 +97,105 @@
 
                             color = c.NONE
                             if not isinstance(field, str):
                                 field, color = field
                             fields.append(dpg.add_text(field, color=color,
                                                        wrap=self.column_widths[index] if self.wrap_text else -1))
                     self.rows.update({row: fields})
-            self.set_y_scroll()
+            self._delete_rows()
 
     def _process_data(self, data) -> t.Iterable:
         ...
 
     def clear(self):
         gui = self.gui
-        self.input_text_row and self._input_text_cleanup()
+        self._input_text_row and self._input_text_cleanup()
         dpg.delete_item(gui.table, slot=1, children_only=True)
         dpg.set_y_scroll(gui.table_window, -1)
+        self._selected_row_index = -1
         self.rows.clear()
 
-    def set_y_scroll(self):
+    def set_y_scroll_to_end(self):
+        dpg.set_y_scroll(self.gui.table_window, -1)
+
+    def _delete_rows(self):
         gui = self.gui
         scroll_max = dpg.get_y_scroll_max(gui.table_window)
         scroll_pos = dpg.get_y_scroll(gui.table_window)
         rows = dpg.get_item_children(self.gui.table, slot=1)
         len_rows = len(rows)
         if (scroll_pos == scroll_max or scroll_pos < 0 or len_rows > self.log_size * 2) and\
                 (rows_to_delete := len_rows - self.log_size) > 0:
             for row_index in range(rows_to_delete):
                 row = rows[row_index]
                 (row in self.rows) and self.rows.pop(row)
-                (row == self.input_text_row) and self._input_text_cleanup()
+                (row == self._input_text_row) and self._input_text_cleanup()
                 dpg.delete_item(row)
+            self.select_row(self._selected_row_index - rows_to_delete)
 
         if scroll_pos == scroll_max:
-            dpg.set_y_scroll(gui.table_window, -1)
+            self.set_y_scroll_to_end()
+
+    def _clipboard_copy(self):
+        if dpg.is_key_down(dpg.mvKey_Control) and dpg.is_item_focused(self.gui.input_text):
+            pyperclip.copy(str.replace(pyperclip.paste(), '\r\n', ''))
 
     def _input_text_cleanup(self):
         gui = self.gui
-        self.input_text_cell and dpg.move_item(self.input_text_cell, before=gui.input_text)
+        self._input_text_cell and dpg.move_item(self._input_text_cell, before=gui.input_text)
         dpg.move_item(gui.input_text, parent=gui.input_text_stage)
-        self.input_text_row = None
-        self.input_text_cell = None
+        self._input_text_row = None
+        self._input_text_cell = None
 
-
-    def cell_clicked(self):
+    def _cell_clicked(self):
         gui = self.gui
         if not self.rows or dpg.is_item_hovered(gui.input_text):
             return
 
         # TODO to function
         container = gui.table_window
         width_offset = height_offset = 0
         while container:
             width, height = dpg.get_item_pos(container)
             width_offset += width
             height_offset += height
             container = dpg_get_item_container(container, dpg.mvChildWindow) or \
-                        dpg_get_item_container(container)
+                dpg_get_item_container(container)
 
         mouse_pos = dpg.get_mouse_pos(local=False)
         mouse_pos = (dpg.get_x_scroll(gui.table_window) + mouse_pos[0] - width_offset,
                      dpg.get_y_scroll(gui.table_window) + mouse_pos[1] - height_offset)  # + 15
 
         row, row_index = dpg_get_item_by_pos(tuple(self.rows.values()), mouse_pos, return_index=True)
         cell, cell_index = dpg_get_item_by_pos(row, mouse_pos, horizontal=True, return_index=True)
         text, width, height = dpg_get_text_from_cell(cell, wrap=self.column_widths[cell_index])
-        if text:
-            self.input_text_cell and dpg.move_item(self.input_text_cell, before=gui.input_text)
-            self.input_text_row = tuple(self.rows)[row_index]
-            self.input_text_cell = cell
+        if text is None:
+            self._input_text_cleanup()
+        else:
+            self._input_text_cell and dpg.move_item(self._input_text_cell, before=gui.input_text)
+            self._input_text_row = tuple(self.rows)[row_index]
+            self._input_text_cell = cell
             dpg.configure_item(gui.input_text, default_value=text,
-                               width=width + 2, height=height)  # width + 1 prevent input_text to scrolling
+                               width=width + 2, height=height)  # width + 2 prevent input_text to scrolling
             dpg.move_item(gui.input_text, before=cell)
             dpg.move_item(cell, parent=gui.input_text_stage)
 
+        self.select_row(row_index)
+
+    def select_row(self, index: int = None):
+        try:
+            if self._selected_row_index >= 0:
+                dpg.unset_table_row_color(self.gui.table, self._selected_row_index)
+            if index is not None:
+                self._selected_row_index = index
+            if self._selected_row_index >= 0:
+                dpg.set_table_row_color(self.gui.table, self._selected_row_index, c.BLUE_4)
+        except SystemError:
+            self._selected_row_index = -1
+
     # TODO implement delete method
     # def close(self):
     #     # get_running_app().size_subscribers.remove(self._width_changed)
     #     # dpg.delete_item(self.gui.handler_reg)
     #     dpg.delete_item(self.gui.group)
 
     def create_gui(self):
@@ -192,29 +219,31 @@
                 dpg.add_theme_color(dpg.mvThemeCol_TableBorderLight, c.GRAY_4)
                 dpg.add_theme_color(dpg.mvThemeCol_TableBorderStrong, c.GRAY_4)
 
                 dpg.add_theme_color(dpg.mvThemeCol_Text, c.GRAY_22)
 
             with dpg.theme_component(dpg.mvInputText):
                 dpg.add_theme_color(dpg.mvThemeCol_Text, c.GRAY_25)
-                dpg.add_theme_color(dpg.mvThemeCol_FrameBg, c.GRAY_2)
-                dpg.add_theme_color(dpg.mvThemeCol_FrameBgHovered, c.GRAY_2)
-                # dpg.add_theme_style(dpg.mvStyleVar_FrameBorderSize, 1, 1)
-                # dpg.add_theme_color(dpg.mvThemeCol_Border, c.BLUE_18)
-                # dpg.add_theme_color(dpg.mvThemeCol_BorderShadow, c.BLUE_18)
-
-        # with dpg.handler_registry(tag=gui.handler_reg):
-        #     dpg.add_mouse_release_handler(0, callback=lambda s, a, u: self._width_changed())
-        # get_running_app().size_subscribers.add(self._width_changed)
+                dpg.add_theme_color(dpg.mvThemeCol_FrameBg, c.BLUE_4)
+                dpg.add_theme_color(dpg.mvThemeCol_FrameBgHovered, c.BLUE_4)
+
+        with dpg.handler_registry():
+            dpg.add_key_press_handler(dpg.mvKey_C, callback=lambda *_: self._clipboard_copy())
 
         with dpg.item_handler_registry() as table_handler_reg:
-            dpg.add_item_clicked_handler(dpg.mvMouseButton_Left, callback=lambda: self.cell_clicked())
+            dpg.add_item_clicked_handler(dpg.mvMouseButton_Left, callback=lambda *_: self._cell_clicked())
 
         with dpg.group(tag=gui.group):
             dpg.bind_item_theme(dpg.last_container(), table_theme)
+            dpg.bind_item_theme(
+                dpg.add_button(tag=gui.scroll_to_end_btn, label='\u25BC', height=20, width=20, pos=(0, 0), show=False,
+                               callback=lambda *_: self.set_y_scroll_to_end()),
+                dpg_get_color_theme(colors=(c.TRANSPARENT, c.GRAY_5, c.TRANSPARENT),
+                                    text_color=c.YELLOW_19))
+
             # TODO cleanup_stage after close in delete method
             with dpg.stage(tag=gui.input_text_stage):
                 dpg.add_input_text(readonly=True, multiline=True, tag=gui.input_text)
             with dpg.table(header_row=False, borders_innerH=False, borders_outerH=False,
                            borders_innerV=True, borders_outerV=False, tag=gui.header,
                            resizable=True, reorderable=True):
                 for name, width, fixed in self.columns:
@@ -222,15 +251,14 @@
                 with dpg.table_row():
                     for name, width, fixed in self.columns:
                         btn = dpg.add_button(label=name, width=-1)
                         dpg.bind_item_theme(btn, header_buttons_theme)
             with dpg.child_window(border=False, tag=gui.table_window, height=-2):
                 with dpg.group(tag=gui.table_group):
                     dpg.bind_item_handler_registry(gui.table_group, table_handler_reg)
-
                     with dpg.table(policy=dpg.mvTable_SizingFixedFit, borders_innerH=True, borders_outerH=False,
                                    borders_innerV=True, borders_outerV=False, tag=gui.table, header_row=False,
                                    resizable=False, reorderable=True, freeze_rows=1, hideable=True,
                                    clipper=self.log_size > 900):
                         for name, width, fixed in self.columns:
                             dpg.add_table_column(width_fixed=True, init_width_or_weight=width)
 
@@ -242,9 +270,10 @@
         group: int
         header: int
         input_text: int
         input_text_stage: int
         table_window: int
         table_group: int
         table: int
+        scroll_to_end_btn: int
         # handler_reg: int
```

## Comparing `dearpyapp-0.1.3.dist-info/LICENSE` & `dearpyapp-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dearpyapp-0.1.3.dist-info/METADATA` & `dearpyapp-0.1.4.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearpyapp
-Version: 0.1.3
+Version: 0.1.4
 Summary: Wrapper for DearPyGui
 Home-page: https://github.com/means0nothing/DearPyApp
 Author: Pavel Shevcov
 Author-email: means0nothing@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,9 +15,10 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dearpygui (==1.8.0)
 Requires-Dist: recordclass (==0.17.2)
 Requires-Dist: pywin32 (==304)
+Requires-Dist: pyperclip (==1.8.2)
 
 Wrapper for DearPyGui with async support and more features.
```

## Comparing `dearpyapp-0.1.3.dist-info/RECORD` & `dearpyapp-0.1.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-dearpyapp/__init__.py,sha256=-dGIQnU8MIMVQasr6iSKrYdr-qDPIbJChqg9DTLSckA,460
+dearpyapp/__init__.py,sha256=kHnkjwdH2lHBTjxK-efWyk7Pc8znBr0GMkwl7sprv00,460
 dearpyapp/application.py,sha256=Nma4VawA6GPQaeAihsjy_2M_NzVgUAaeQosN-w7NqXo,10777
-dearpyapp/colors.py,sha256=MIeFfAmC3Gwjyaf6EcjzO1Byxte_g_QBi5q8X-AgOmA,2328
+dearpyapp/colors.py,sha256=WyocMrodma5892tcjdCwzlZlHFXJ817WradZpZu9YjM,2622
 dearpyapp/themes.py,sha256=sEPZcvwAVxbqBqci87Q0v57IFJxaZSNVFD6YVs0XSgw,8883
-dearpyapp/utils.py,sha256=SDPunxOee-INsQavMk6wvIN76CYBPv6RgDHGULOnzq8,9102
+dearpyapp/utils.py,sha256=1GckeHYxRPk2bqoHcB_oAbFDakBCuOSdx54nekvK2EI,10757
 dearpyapp/components/__init__.py,sha256=DH-92pXUHLPgxHSIJlc06FsA_WzMvooPck47pkvssGg,105
-dearpyapp/components/log.py,sha256=nigCQlPxlIoLJL5MeSE0oldTUd4Fu_dUqgYdvhoWXzU,12649
+dearpyapp/components/log.py,sha256=c3aEf9EkxhBOYWc59ELwWYIk3mFzaXQmwxCmUotVD2U,13513
 dearpyapp/components/port_control.py,sha256=Jo1Q5d8-xmFRo_p5zutt7iBjN0KepiuNgQCcSMw9rJQ,12733
 dearpyapp/components/tab.py,sha256=4yhD6xGGI4jKZpYlDoyM8bN700ZrEf5LT4YELA6MumU,6455
-dearpyapp-0.1.3.dist-info/LICENSE,sha256=KOI2v5c_M5MQQkVqxM4BBqmkZnNAh6PYV-3Q9pTInWE,1096
-dearpyapp-0.1.3.dist-info/METADATA,sha256=RcLcprhabDmVOW_zLP0TFJXgI6Njko-X5tA21iZTjh4,864
-dearpyapp-0.1.3.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-dearpyapp-0.1.3.dist-info/top_level.txt,sha256=XwOBbr99GukN8XkQi7CxxSmYO32SNAfcDnXtKuKRT_k,10
-dearpyapp-0.1.3.dist-info/RECORD,,
+dearpyapp-0.1.4.dist-info/LICENSE,sha256=KOI2v5c_M5MQQkVqxM4BBqmkZnNAh6PYV-3Q9pTInWE,1096
+dearpyapp-0.1.4.dist-info/METADATA,sha256=cj740hnzcgAaPxM_Qr9Jm6drLAMf9uf0lYnaoXyXUqE,900
+dearpyapp-0.1.4.dist-info/WHEEL,sha256=mrWOx6J2F1tE6ZQ2IHrEElXwJlXc4qGHu6mNTK_VE4U,98
+dearpyapp-0.1.4.dist-info/top_level.txt,sha256=XwOBbr99GukN8XkQi7CxxSmYO32SNAfcDnXtKuKRT_k,10
+dearpyapp-0.1.4.dist-info/RECORD,,
```

