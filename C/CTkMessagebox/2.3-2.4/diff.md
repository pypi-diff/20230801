# Comparing `tmp/CTkMessagebox-2.3.tar.gz` & `tmp/CTkMessagebox-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkMessagebox-2.3.tar", last modified: Wed Jul 12 14:39:38 2023, max compression
+gzip compressed data, was "CTkMessagebox-2.4.tar", last modified: Tue Aug  1 14:11:47 2023, max compression
```

## Comparing `CTkMessagebox-2.3.tar` & `CTkMessagebox-2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 14:39:38.700017 CTkMessagebox-2.3/
-drwxrwxrwx   0        0        0        0 2023-07-12 14:39:38.653143 CTkMessagebox-2.3/CTkMessagebox/
--rw-rw-rw-   0        0        0      232 2023-07-12 14:33:56.000000 CTkMessagebox-2.3/CTkMessagebox/__init__.py
--rw-rw-rw-   0        0        0    17006 2023-07-12 14:33:23.000000 CTkMessagebox-2.3/CTkMessagebox/ctkmessagebox.py
-drwxrwxrwx   0        0        0        0 2023-07-12 14:39:38.700017 CTkMessagebox-2.3/CTkMessagebox/icons/
--rw-rw-rw-   0        0        0    38437 2023-02-24 17:58:14.000000 CTkMessagebox-2.3/CTkMessagebox/icons/cancel.png
--rw-rw-rw-   0        0        0    31308 2023-02-24 17:40:20.000000 CTkMessagebox-2.3/CTkMessagebox/icons/check.png
--rw-rw-rw-   0        0        0    14921 2023-02-24 18:08:36.000000 CTkMessagebox-2.3/CTkMessagebox/icons/info.png
--rw-rw-rw-   0        0        0    15030 2023-04-14 12:27:30.000000 CTkMessagebox-2.3/CTkMessagebox/icons/question.png
--rw-rw-rw-   0        0        0    17104 2023-02-24 18:03:33.000000 CTkMessagebox-2.3/CTkMessagebox/icons/warning.png
-drwxrwxrwx   0        0        0        0 2023-07-12 14:39:38.668769 CTkMessagebox-2.3/CTkMessagebox.egg-info/
--rw-rw-rw-   0        0        0     7184 2023-07-12 14:39:38.000000 CTkMessagebox-2.3/CTkMessagebox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-07-12 14:39:38.000000 CTkMessagebox-2.3/CTkMessagebox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       73 2023-07-12 14:39:38.000000 CTkMessagebox-2.3/CTkMessagebox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-12 14:39:38.000000 CTkMessagebox-2.3/CTkMessagebox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-12 14:39:38.000000 CTkMessagebox-2.3/CTkMessagebox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkMessagebox-2.3/LICENSE
--rw-rw-rw-   0        0        0     7184 2023-07-12 14:39:38.700017 CTkMessagebox-2.3/PKG-INFO
--rw-rw-rw-   0        0        0     6486 2023-07-12 14:35:39.000000 CTkMessagebox-2.3/README.md
--rw-rw-rw-   0        0        0      625 2023-07-12 14:39:38.700017 CTkMessagebox-2.3/setup.cfg
--rw-rw-rw-   0        0        0     1361 2023-07-12 14:38:12.000000 CTkMessagebox-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:47.710416 CTkMessagebox-2.4/
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:47.645875 CTkMessagebox-2.4/CTkMessagebox/
+-rw-rw-rw-   0        0        0      232 2023-08-01 13:43:37.000000 CTkMessagebox-2.4/CTkMessagebox/__init__.py
+-rw-rw-rw-   0        0        0    19179 2023-08-01 14:07:54.000000 CTkMessagebox-2.4/CTkMessagebox/ctkmessagebox.py
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:47.707740 CTkMessagebox-2.4/CTkMessagebox/icons/
+-rw-rw-rw-   0        0        0    38437 2023-02-24 17:58:14.000000 CTkMessagebox-2.4/CTkMessagebox/icons/cancel.png
+-rw-rw-rw-   0        0        0    31308 2023-02-24 17:40:20.000000 CTkMessagebox-2.4/CTkMessagebox/icons/check.png
+-rw-rw-rw-   0        0        0    14921 2023-02-24 18:08:36.000000 CTkMessagebox-2.4/CTkMessagebox/icons/info.png
+-rw-rw-rw-   0        0        0    15030 2023-04-14 12:27:30.000000 CTkMessagebox-2.4/CTkMessagebox/icons/question.png
+-rw-rw-rw-   0        0        0    17104 2023-02-24 18:03:33.000000 CTkMessagebox-2.4/CTkMessagebox/icons/warning.png
+drwxrwxrwx   0        0        0        0 2023-08-01 14:11:47.677135 CTkMessagebox-2.4/CTkMessagebox.egg-info/
+-rw-rw-rw-   0        0        0     7249 2023-08-01 14:11:47.000000 CTkMessagebox-2.4/CTkMessagebox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-08-01 14:11:47.000000 CTkMessagebox-2.4/CTkMessagebox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       73 2023-08-01 14:11:47.000000 CTkMessagebox-2.4/CTkMessagebox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-08-01 14:11:47.000000 CTkMessagebox-2.4/CTkMessagebox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-01 14:11:47.000000 CTkMessagebox-2.4/CTkMessagebox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkMessagebox-2.4/LICENSE
+-rw-rw-rw-   0        0        0     7249 2023-08-01 14:11:47.710416 CTkMessagebox-2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6551 2023-08-01 14:10:45.000000 CTkMessagebox-2.4/README.md
+-rw-rw-rw-   0        0        0      625 2023-08-01 14:11:47.711032 CTkMessagebox-2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1361 2023-08-01 14:10:59.000000 CTkMessagebox-2.4/setup.py
```

### Comparing `CTkMessagebox-2.3/CTkMessagebox/ctkmessagebox.py` & `CTkMessagebox-2.4/CTkMessagebox/ctkmessagebox.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 CustomTkinter Messagebox
 Author: Akash Bora
-Version: 2.3
+Version: 2.4
 """
 
 import customtkinter
-from PIL import Image
+from PIL import Image, ImageTk
 import os
 import sys
 import time
 from typing import Literal
 
 class CTkMessagebox(customtkinter.CTkToplevel):
     ICONS = {
         "check": None,
         "cancel": None,
         "info": None,
         "question": None,
         "warning": None
     }
-
+    ICON_BITMAP = {}
     def __init__(self,
                  master: any = None,
                  width: int = 400,
                  height: int = 200,
                  title: str = "CTkMessagebox",
                  message: str = "This is a CTkMessagebox!",
                  option_1: str = "OK",
@@ -42,14 +42,15 @@
                  button_height: int = None,
                  cancel_button_color: str = None,
                  cancel_button: str = None, # types: circle, cross or none
                  button_hover_color: str = "default",
                  icon: str = "info",
                  icon_size: tuple = None,
                  corner_radius: int = 15,
+                 justify: str = "right",
                  font: tuple = None,
                  header: bool = False,
                  topmost: bool = True,
                  fade_in_duration: int = 0,
                  option_focus: Literal[1, 2, 3] = None):
         
         super().__init__()
@@ -75,15 +76,15 @@
         
         if self.fade:
             self.fade = 20 if self.fade<20 else self.fade
             self.attributes("-alpha", 0)
         
         if not header:
             self.overrideredirect(1)
-    
+            
         if topmost:
             self.attributes("-topmost", True)
         else:
             self.transient(self.master_window)
     
         if sys.platform.startswith("win"):
             self.transparent_color = self._apply_appearance_mode(self.cget("fg_color"))
@@ -105,15 +106,15 @@
         self.grid_columnconfigure(0, weight=1)
         self.grid_rowconfigure(0, weight=1)    
         self.x = self.winfo_x()
         self.y = self.winfo_y()
         self._title = title
         self.message = message
         self.font = font
-        
+        self.justify = justify
         self.cancel_button = cancel_button if cancel_button else default_cancel_button      
         self.round_corners = corner_radius if corner_radius<=30 else 30
         self.button_width = button_width if button_width else self.width/4
         self.button_height = button_height if button_height else 28
         if self.fade: self.attributes("-alpha", 0)
         
         if self.button_height>self.height/4: self.button_height = self.height/4 -20
@@ -186,14 +187,15 @@
         if icon_size:
             self.size_height = icon_size[1] if icon_size[1]<=self.height-100 else self.height-100
             self.size = (icon_size[0], self.size_height)
         else:
             self.size = (self.height/4, self.height/4)
         
         self.icon = self.load_icon(icon, icon_size) if icon else None
+        
         self.frame_top = customtkinter.CTkFrame(self, corner_radius=self.round_corners, width=self.width, border_width=self.border_width,
                                                 bg_color=self.transparent_color, fg_color=self.bg_color, border_color=self.border_color)
         self.frame_top.grid(sticky="nswe")
 
         if button_width:
             self.frame_top.grid_columnconfigure(0, weight=1)
         else:
@@ -206,62 +208,94 @@
             
         self.frame_top.bind("<B1-Motion>", self.move_window)
         self.frame_top.bind("<ButtonPress-1>", self.oldxyset)
 
         if self.cancel_button=="cross":
             self.button_close = customtkinter.CTkButton(self.frame_top, corner_radius=10, width=0, height=0, hover=False, border_width=0,
                                                         text_color=self.dot_color if self.dot_color else self.title_color,
-                                                        text="✕", fg_color="transparent", command=self.button_event)
-            self.button_close.grid(row=0, column=3, sticky="ne", padx=5+self.border_width, pady=5+self.border_width)
+                                                      text="✕", fg_color="transparent", command=self.button_event)
+            self.button_close.grid(row=0, column=5, sticky="ne", padx=5+self.border_width, pady=5+self.border_width)
         elif self.cancel_button=="circle":
             self.button_close = customtkinter.CTkButton(self.frame_top, corner_radius=10, width=10, height=10, hover=False, border_width=0,
                                                         text="", fg_color=self.dot_color if self.dot_color else "#c42b1c", command=self.button_event)     
-            self.button_close.grid(row=0, column=3, sticky="ne", padx=10, pady=10)       
+            self.button_close.grid(row=0, column=5, sticky="ne", padx=10, pady=10)       
             
         self.title_label = customtkinter.CTkLabel(self.frame_top, width=1, text=self._title, text_color=self.title_color, font=self.font)
-        self.title_label.grid(row=0, column=0, columnspan=4, sticky="nw", padx=(15,30), pady=5)
+        self.title_label.grid(row=0, column=0, columnspan=6, sticky="nw", padx=(15,30), pady=5)
         self.title_label.bind("<B1-Motion>", self.move_window)
         self.title_label.bind("<ButtonPress-1>", self.oldxyset)
         
         self.info = customtkinter.CTkButton(self.frame_top,  width=1, height=self.height/2, corner_radius=0, text=self.message, font=self.font,
                                             fg_color=self.fg_color, hover=False, text_color=self.text_color, image=self.icon)
         self.info._text_label.configure(wraplength=self.width/2, justify="left")
-        self.info.grid(row=1, column=0, columnspan=4, sticky="nwes", padx=self.border_width)
+        self.info.grid(row=1, column=0, columnspan=6, sticky="nwes", padx=self.border_width)
         
         if self.info._text_label.winfo_reqheight()>self.height/2:
             height_offset = int((self.info._text_label.winfo_reqheight())-(self.height/2) + self.height)
             self.geometry(f"{self.width}x{height_offset}")
-            
+
+
         self.option_text_1 = option_1
+        
         self.button_1 = customtkinter.CTkButton(self.frame_top, text=self.option_text_1, fg_color=self.button_color[0],
                                                 width=self.button_width, font=self.font, text_color=self.bt_text_color,
                                                 hover_color=self.bt_hv_color, height=self.button_height,
                                                 command=lambda: self.button_event(self.option_text_1))
         
-        self.button_1.grid(row=2, column=3, sticky="news", padx=(0,10), pady=10)
 
         self.option_text_2 = option_2 
         if option_2:     
             self.button_2 = customtkinter.CTkButton(self.frame_top, text=self.option_text_2, fg_color=self.button_color[1],
                                                     width=self.button_width, font=self.font, text_color=self.bt_text_color,
                                                     hover_color=self.bt_hv_color, height=self.button_height,
                                                     command=lambda: self.button_event(self.option_text_2))
-            self.button_2.grid(row=2, column=2, sticky="news", padx=10, pady=10)
 
         self.option_text_3 = option_3
         if option_3:
             self.button_3 = customtkinter.CTkButton(self.frame_top, text=self.option_text_3, fg_color=self.button_color[2],
                                                     width=self.button_width, font=self.font, text_color=self.bt_text_color,
                                                     hover_color=self.bt_hv_color, height=self.button_height,
                                                     command=lambda: self.button_event(self.option_text_3))
-            self.button_3.grid(row=2, column=1, sticky="news", padx=(10,0), pady=10)
-
+            
+        if self.justify=="center":
+            if option_3:
+                self.frame_top.columnconfigure((0,1,2,3,4,5), weight=1)
+                columns = [4,2,0]
+                self.button_1.grid(row=2, column=columns[0], columnspan=2, sticky="news", padx=(0,10), pady=10) 
+                self.button_2.grid(row=2, column=columns[1], columnspan=2, sticky="news", padx=10, pady=10)
+                self.button_3.grid(row=2, column=columns[2], columnspan=2, sticky="news", padx=(10,0), pady=10)
+            elif option_2:
+                self.frame_top.columnconfigure((0,5), weight=1)
+                columns = [2,3]
+                self.button_1.grid(row=2, column=columns[0], sticky="news", padx=(0,5), pady=10)
+                self.button_2.grid(row=2, column=columns[1], sticky="news", padx=(5,0), pady=10)
+            else:
+                self.frame_top.columnconfigure((0,2,4), weight=2)
+                self.button_1.grid(row=2, column=2, columnspan=2, sticky="news", padx=(0,10), pady=10)   
+        elif self.justify=="left":
+            self.frame_top.columnconfigure((0,1,2,3,4,5), weight=1)
+            columns = [0,2,4]
+            self.button_1.grid(row=2, column=columns[0], columnspan=2, sticky="news", padx=(10,0), pady=10)
+            if option_2:  
+                self.button_2.grid(row=2, column=columns[1], columnspan=2, sticky="news", padx=10, pady=10)
+            if option_3:
+                self.button_3.grid(row=2, column=columns[2], columnspan=2, sticky="news", padx=(0,10), pady=10)
+        else:
+            self.frame_top.columnconfigure((0,1,2,3,4,5), weight=1)
+            columns = [4,2,0]
+            self.button_1.grid(row=2, column=columns[0], columnspan=2, sticky="news", padx=(0,10), pady=10)
+            if option_2:  
+                self.button_2.grid(row=2, column=columns[1], columnspan=2, sticky="news", padx=10, pady=10)
+            if option_3:
+                self.button_3.grid(row=2, column=columns[2], columnspan=2, sticky="news", padx=(10,0), pady=10)
+                        
         if header:
-            self.title_label.grid_forget()
-            self.button_close.grid_forget()
+            self.title_label.configure(text="")
+            self.title_label.grid_configure(pady=0)
+            self.button_close.configure(text_color=self.bg_color)
             self.frame_top.configure(corner_radius=0)
 
         if self.winfo_exists():
             self.grab_set()
             
         if self.fade:
             self.fade_in()
@@ -329,14 +363,16 @@
                 image_path = icon
             if icon_size:
                 size_height = icon_size[1] if icon_size[1] <= self.height - 100 else self.height - 100
                 size = (icon_size[0], size_height)
             else:
                 size = (self.height / 4, self.height / 4)
             self.ICONS[icon] = customtkinter.CTkImage(Image.open(image_path), size=size)
+            self.ICON_BITMAP[icon] = ImageTk.PhotoImage(file=image_path)
+        self.after(200, lambda: self.iconphoto(False, self.ICON_BITMAP[icon]))
         return self.ICONS[icon]
         
     def fade_in(self):
         for i in range(0,110,10):
             if not self.winfo_exists():
                 break
             self.attributes("-alpha", i/100)
```

### Comparing `CTkMessagebox-2.3/CTkMessagebox/icons/cancel.png` & `CTkMessagebox-2.4/CTkMessagebox/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.3/CTkMessagebox/icons/check.png` & `CTkMessagebox-2.4/CTkMessagebox/icons/check.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.3/CTkMessagebox/icons/info.png` & `CTkMessagebox-2.4/CTkMessagebox/icons/info.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.3/CTkMessagebox/icons/question.png` & `CTkMessagebox-2.4/CTkMessagebox/icons/question.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.3/CTkMessagebox/icons/warning.png` & `CTkMessagebox-2.4/CTkMessagebox/icons/warning.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.3/CTkMessagebox.egg-info/PKG-INFO` & `CTkMessagebox-2.4/CTkMessagebox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMessagebox
-Version: 2.3
+Version: 2.4
 Summary: A modern messagebox for customtkinter
 Home-page: https://github.com/Akascape/CTkMessagebox
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -159,16 +159,18 @@
   | _cancel_button_color_ | color of the **close** button, **set it to 'transparent' if you want to hide it** |
   | **_icon_** | icon that will be shown in the messagebox [Default is the 'info' icon] |
   | _icon_size_ | define the size of the icon image manually (tuple) |
   | _corner_radius_ | corner roundness of the messagebox window [**not applicable in linux**] |
   | _font_ | font of the messagebox text (tuple) |
   | _header_ | add the original header back if you don't like **overrideredirect** (bool) |
   | _topmost_ | disable the topmost window outside the app (bool) |
+  | _justify_ | position the buttons to center/right/left |
   | _focus_option_ | select an option by default when `Enter` key is pressed |
   | **_fade_in_duration_** | enable a fade-in and fade-out animation (int, default is 0)  |
+  
 
 </div>
 
 <br>
 
 <h2 align="center"> Icons </h2>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CTkMessagebox Version: 2.3 Summary: A modern
+Metadata-Version: 2.1 Name: CTkMessagebox Version: 2.4 Summary: A modern
 messagebox for customtkinter Home-page: https://github.com/Akascape/
 CTkMessagebox Author: Akash Bora License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-
 messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-
 messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
@@ -79,17 +79,17 @@
 cancel button type: **circle, cross or None** | | _cancel_button_color_ | color
 of the **close** button, **set it to 'transparent' if you want to hide it** | |
  **_icon_** | icon that will be shown in the messagebox [Default is the 'info'
 icon] | | _icon_size_ | define the size of the icon image manually (tuple) | |
  _corner_radius_ | corner roundness of the messagebox window [**not applicable
 in linux**] | | _font_ | font of the messagebox text (tuple) | | _header_ | add
   the original header back if you don't like **overrideredirect** (bool) | |
-       _topmost_ | disable the topmost window outside the app (bool) | |
- _focus_option_ | select an option by default when `Enter` key is pressed | |
-**_fade_in_duration_** | enable a fade-in and fade-out animation (int, default
-                                    is 0) |
+ _topmost_ | disable the topmost window outside the app (bool) | | _justify_ |
+position the buttons to center/right/left | | _focus_option_ | select an option
+ by default when `Enter` key is pressed | | **_fade_in_duration_** | enable a
+             fade-in and fade-out animation (int, default is 0) |
 
                                ***** Icons *****
 **Default icons:** ![icons](https://user-images.githubusercontent.com/89206401/
  221258403-aafea575-856e-4f4e-b3af-f995785c9879.png) (*These icons are created
          using Paint.NET, free to use!*) **For custom images, just use
  `icon="image_path.png"`** ## That's all, hope it will help in UI development!
```

### Comparing `CTkMessagebox-2.3/LICENSE` & `CTkMessagebox-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.3/PKG-INFO` & `CTkMessagebox-2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMessagebox
-Version: 2.3
+Version: 2.4
 Summary: A modern messagebox for customtkinter
 Home-page: https://github.com/Akascape/CTkMessagebox
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -159,16 +159,18 @@
   | _cancel_button_color_ | color of the **close** button, **set it to 'transparent' if you want to hide it** |
   | **_icon_** | icon that will be shown in the messagebox [Default is the 'info' icon] |
   | _icon_size_ | define the size of the icon image manually (tuple) |
   | _corner_radius_ | corner roundness of the messagebox window [**not applicable in linux**] |
   | _font_ | font of the messagebox text (tuple) |
   | _header_ | add the original header back if you don't like **overrideredirect** (bool) |
   | _topmost_ | disable the topmost window outside the app (bool) |
+  | _justify_ | position the buttons to center/right/left |
   | _focus_option_ | select an option by default when `Enter` key is pressed |
   | **_fade_in_duration_** | enable a fade-in and fade-out animation (int, default is 0)  |
+  
 
 </div>
 
 <br>
 
 <h2 align="center"> Icons </h2>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CTkMessagebox Version: 2.3 Summary: A modern
+Metadata-Version: 2.1 Name: CTkMessagebox Version: 2.4 Summary: A modern
 messagebox for customtkinter Home-page: https://github.com/Akascape/
 CTkMessagebox Author: Akash Bora License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-
 messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-
 messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
@@ -79,17 +79,17 @@
 cancel button type: **circle, cross or None** | | _cancel_button_color_ | color
 of the **close** button, **set it to 'transparent' if you want to hide it** | |
  **_icon_** | icon that will be shown in the messagebox [Default is the 'info'
 icon] | | _icon_size_ | define the size of the icon image manually (tuple) | |
  _corner_radius_ | corner roundness of the messagebox window [**not applicable
 in linux**] | | _font_ | font of the messagebox text (tuple) | | _header_ | add
   the original header back if you don't like **overrideredirect** (bool) | |
-       _topmost_ | disable the topmost window outside the app (bool) | |
- _focus_option_ | select an option by default when `Enter` key is pressed | |
-**_fade_in_duration_** | enable a fade-in and fade-out animation (int, default
-                                    is 0) |
+ _topmost_ | disable the topmost window outside the app (bool) | | _justify_ |
+position the buttons to center/right/left | | _focus_option_ | select an option
+ by default when `Enter` key is pressed | | **_fade_in_duration_** | enable a
+             fade-in and fade-out animation (int, default is 0) |
 
                                ***** Icons *****
 **Default icons:** ![icons](https://user-images.githubusercontent.com/89206401/
  221258403-aafea575-856e-4f4e-b3af-f995785c9879.png) (*These icons are created
          using Paint.NET, free to use!*) **For custom images, just use
  `icon="image_path.png"`** ## That's all, hope it will help in UI development!
```

### Comparing `CTkMessagebox-2.3/README.md` & `CTkMessagebox-2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -144,16 +144,18 @@
   | _cancel_button_color_ | color of the **close** button, **set it to 'transparent' if you want to hide it** |
   | **_icon_** | icon that will be shown in the messagebox [Default is the 'info' icon] |
   | _icon_size_ | define the size of the icon image manually (tuple) |
   | _corner_radius_ | corner roundness of the messagebox window [**not applicable in linux**] |
   | _font_ | font of the messagebox text (tuple) |
   | _header_ | add the original header back if you don't like **overrideredirect** (bool) |
   | _topmost_ | disable the topmost window outside the app (bool) |
+  | _justify_ | position the buttons to center/right/left |
   | _focus_option_ | select an option by default when `Enter` key is pressed |
   | **_fade_in_duration_** | enable a fade-in and fade-out animation (int, default is 0)  |
+  
 
 </div>
 
 <br>
 
 <h2 align="center"> Icons </h2>
```

#### html2text {}

```diff
@@ -69,17 +69,17 @@
 cancel button type: **circle, cross or None** | | _cancel_button_color_ | color
 of the **close** button, **set it to 'transparent' if you want to hide it** | |
  **_icon_** | icon that will be shown in the messagebox [Default is the 'info'
 icon] | | _icon_size_ | define the size of the icon image manually (tuple) | |
  _corner_radius_ | corner roundness of the messagebox window [**not applicable
 in linux**] | | _font_ | font of the messagebox text (tuple) | | _header_ | add
   the original header back if you don't like **overrideredirect** (bool) | |
-       _topmost_ | disable the topmost window outside the app (bool) | |
- _focus_option_ | select an option by default when `Enter` key is pressed | |
-**_fade_in_duration_** | enable a fade-in and fade-out animation (int, default
-                                    is 0) |
+ _topmost_ | disable the topmost window outside the app (bool) | | _justify_ |
+position the buttons to center/right/left | | _focus_option_ | select an option
+ by default when `Enter` key is pressed | | **_fade_in_duration_** | enable a
+             fade-in and fade-out animation (int, default is 0) |
 
                                ***** Icons *****
 **Default icons:** ![icons](https://user-images.githubusercontent.com/89206401/
  221258403-aafea575-856e-4f4e-b3af-f995785c9879.png) (*These icons are created
          using Paint.NET, free to use!*) **For custom images, just use
  `icon="image_path.png"`** ## That's all, hope it will help in UI development!
```

### Comparing `CTkMessagebox-2.3/setup.cfg` & `CTkMessagebox-2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 4d65 7373 6167 6562 6f78   = CTkMessagebox
-00000020: 0d0a 7665 7273 696f 6e20 3d20 322e 330d  ..version = 2.3.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 322e 340d  ..version = 2.4.
 00000030: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000040: 206d 6f64 6572 6e20 6d65 7373 6167 6562   modern messageb
 00000050: 6f78 2066 6f72 2063 7573 746f 6d74 6b69  ox for customtki
 00000060: 6e74 6572 0d0a 6c6f 6e67 5f64 6573 6372  nter..long_descr
 00000070: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 00000080: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
 00000090: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
```

### Comparing `CTkMessagebox-2.3/setup.py` & `CTkMessagebox-2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkMessagebox',
-    version = '2.3',
+    version = '2.4',
     description = "A modern messagebox for customtkinter",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkMessagebox",
```

