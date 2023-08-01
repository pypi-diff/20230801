# Comparing `tmp/htmltools-0.2.1.tar.gz` & `tmp/htmltools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htmltools-0.2.1.tar", last modified: Mon Apr  3 20:15:46 2023, max compression
+gzip compressed data, was "htmltools-0.3.0.tar", last modified: Tue Aug  1 21:34:35 2023, max compression
```

## Comparing `htmltools-0.2.1.tar` & `htmltools-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:15:46.396905 htmltools-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-03 20:15:37.000000 htmltools-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-03 20:15:37.000000 htmltools-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-03 20:15:46.396905 htmltools-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-03 20:15:37.000000 htmltools-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:15:46.396905 htmltools-0.2.1/htmltools/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-03 20:15:37.000000 htmltools-0.2.1/htmltools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44123 2023-04-03 20:15:37.000000 htmltools-0.2.1/htmltools/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-04-03 20:15:37.000000 htmltools-0.2.1/htmltools/_jsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-03 20:15:37.000000 htmltools-0.2.1/htmltools/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-03 20:15:37.000000 htmltools-0.2.1/htmltools/_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:15:46.392905 htmltools-0.2.1/htmltools/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:15:46.396905 htmltools-0.2.1/htmltools/lib/react/
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-04-03 20:15:37.000000 htmltools-0.2.1/htmltools/lib/react/react.production.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:15:46.396905 htmltools-0.2.1/htmltools/lib/react-dom/
--rw-r--r--   0 runner    (1001) docker     (123)   120585 2023-04-03 20:15:37.000000 htmltools-0.2.1/htmltools/lib/react-dom/react-dom.production.min.js
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 20:15:37.000000 htmltools-0.2.1/htmltools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39743 2023-04-03 20:15:37.000000 htmltools-0.2.1/htmltools/svg.py
--rw-r--r--   0 runner    (1001) docker     (123)    84483 2023-04-03 20:15:37.000000 htmltools-0.2.1/htmltools/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:15:46.396905 htmltools-0.2.1/htmltools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-03 20:15:46.000000 htmltools-0.2.1/htmltools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-03 20:15:46.000000 htmltools-0.2.1/htmltools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 20:15:46.000000 htmltools-0.2.1/htmltools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 20:15:46.000000 htmltools-0.2.1/htmltools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-03 20:15:46.000000 htmltools-0.2.1/htmltools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-03 20:15:46.000000 htmltools-0.2.1/htmltools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-03 20:15:46.396905 htmltools-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 20:15:37.000000 htmltools-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:34:35.023670 htmltools-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-01 21:34:23.000000 htmltools-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-01 21:34:23.000000 htmltools-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-01 21:34:35.023670 htmltools-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-01 21:34:23.000000 htmltools-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:34:35.023670 htmltools-0.3.0/htmltools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-01 21:34:23.000000 htmltools-0.3.0/htmltools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46628 2023-08-01 21:34:23.000000 htmltools-0.3.0/htmltools/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12121 2023-08-01 21:34:23.000000 htmltools-0.3.0/htmltools/_jsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-08-01 21:34:23.000000 htmltools-0.3.0/htmltools/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-01 21:34:23.000000 htmltools-0.3.0/htmltools/_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:34:35.023670 htmltools-0.3.0/htmltools/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:34:35.023670 htmltools-0.3.0/htmltools/lib/react/
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-08-01 21:34:23.000000 htmltools-0.3.0/htmltools/lib/react/react.production.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:34:35.023670 htmltools-0.3.0/htmltools/lib/react-dom/
+-rw-r--r--   0 runner    (1001) docker     (123)   120585 2023-08-01 21:34:23.000000 htmltools-0.3.0/htmltools/lib/react-dom/react-dom.production.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 21:34:23.000000 htmltools-0.3.0/htmltools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42317 2023-08-01 21:34:23.000000 htmltools-0.3.0/htmltools/svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88890 2023-08-01 21:34:23.000000 htmltools-0.3.0/htmltools/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 21:34:35.023670 htmltools-0.3.0/htmltools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-08-01 21:34:34.000000 htmltools-0.3.0/htmltools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-01 21:34:35.000000 htmltools-0.3.0/htmltools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:34:34.000000 htmltools-0.3.0/htmltools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 21:34:34.000000 htmltools-0.3.0/htmltools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-01 21:34:34.000000 htmltools-0.3.0/htmltools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 21:34:34.000000 htmltools-0.3.0/htmltools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-01 21:34:35.023670 htmltools-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 21:34:23.000000 htmltools-0.3.0/setup.py
```

### Comparing `htmltools-0.2.1/LICENSE` & `htmltools-0.3.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 RStudio, PBC
+Copyright (c) 2023 Posit Software, PBC
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `htmltools-0.2.1/PKG-INFO` & `htmltools-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: htmltools
-Version: 0.2.1
+Version: 0.3.0
 Summary: Tools for HTML generation and output.
 Home-page: https://github.com/rstudio/py-htmltools
 Author: Carson Sievert
 Author-email: carson@rstudio.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rstudio/py-htmltools/issues
 Project-URL: Source Code, https://github.com/rstudio/py-htmltools
 Keywords: html
 Platform: any
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # htmltools
```

### Comparing `htmltools-0.2.1/htmltools/__init__.py` & `htmltools-0.3.0/htmltools/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 
 from . import svg, tags
 from ._core import TagAttrArg  # pyright: ignore[reportUnusedImport]  # noqa: F401
 from ._core import TagChildArg  # pyright: ignore[reportUnusedImport]  # noqa: F401
 from ._core import (
     HTML,
     HTMLDependency,
```

### Comparing `htmltools-0.2.1/htmltools/_core.py` & `htmltools-0.3.0/htmltools/_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,23 +28,15 @@
 # they should both come from the same typing module.
 # https://peps.python.org/pep-0655/#usage-in-python-3-11
 if sys.version_info >= (3, 11):
     from typing import Never, NotRequired, TypedDict
 else:
     from typing_extensions import Never, NotRequired, TypedDict
 
-if sys.version_info >= (3, 8):
-    from typing import Literal, Protocol, SupportsIndex, runtime_checkable
-else:
-    from typing_extensions import (
-        SupportsIndex,
-        Protocol,
-        runtime_checkable,
-        Literal,
-    )
+from typing import Literal, Protocol, SupportsIndex, runtime_checkable
 
 from packaging.version import Version
 
 from ._util import (
     ensure_http_server,
     flatten,
     hash_deterministic,
@@ -86,57 +78,70 @@
     pass
 
 
 T = TypeVar("T")
 
 TagT = TypeVar("TagT", bound="Tag")
 
-# Types that can be passed in as attributes to Tag functions. These values will be
-# converted to strings before being stored as tag attributes.
 TagAttrValue = Union[str, float, bool, None]
+"""
+Types that can be passed in as attributes to `Tag` functions. These values will be
+converted to strings before being stored as tag attributes.
+"""
 
-# For dictionaries of tag attributes (e.g., {"id": "foo"}), which can be passed as
-# unnamed arguments to Tag functions like ``div()``.
 TagAttrs = Dict[str, TagAttrValue]
+"""
+For dictionaries of tag attributes (e.g., `{"id": "foo"}`), which can be passed as
+unnamed arguments to Tag functions like `div()`.
+"""
 
-# Types of objects that can be a node in a Tag tree. Equivalently, these are the valid
-# elements of a TagList. Note that this type represents the internal structure of items
-# in a TagList; the user-facing type is TagChild.
 TagNode = Union["Tagifiable", "Tag", MetadataNode, str]
+"""
+Types of objects that can be a node in a `Tag` tree. Equivalently, these are the valid
+elements of a `TagList`. Note that this type represents the internal structure of items
+in a `TagList`; the user-facing type is `TagChild`.
+"""
 
-# Types of objects that can be passed as children to Tag functions like ``div()``. The
-# Tag functions and the TagList() constructor can accept these as unnamed arguments;
-# they will be flattened and normalized to TagNode objects.
 TagChild = Union[
     TagNode,
     "TagList",
     float,
     None,
     Sequence["TagChild"],
 ]
-
+"""
+Types of objects that can be passed as children to Tag functions like `div()`. The `Tag`
+functions and the `TagList()` constructor can accept these as unnamed arguments; they
+will be flattened and normalized to `TagNode` objects.
+"""
 
 # These two types existed in htmltools 0.14.0 and earlier. They are here so that
 # existing versions of Shiny will be able to load, but users of those existing packages
 # will see type errors, which should encourage them to upgrade Shiny.
 TagChildArg = Never
 TagAttrArg = Never
 
 
-# Objects with tagify() methods are considered Tagifiable. Note that an object returns a
-# TagList, the children of the TagList must also be tagified.
 @runtime_checkable
 class Tagifiable(Protocol):
+    """
+    Objects with `tagify()` methods are considered `Tagifiable`. Note that an object
+    returns a `TagList`, the children of the `TagList` must also be tagified.
+    """
+
     def tagify(self) -> "TagList | Tag | MetadataNode | str":
         ...
 
 
-# Tag functions, like div(), span(), etc.
 @runtime_checkable
 class TagFunction(Protocol):
+    """
+    Tag functions, like `div()`, `span()`, etc.
+    """
+
     def __call__(
         self,
         *args: TagChild | TagAttrs,
         _add_ws: bool = ...,
         **kwargs: TagAttrValue,
     ) -> "Tag":
         ...
@@ -150,16 +155,16 @@
     Create an HTML tag list (i.e., a fragment of HTML)
 
     Parameters
     ----------
     *args
         The tag children to add to the list.
 
-    Example
-    -------
+    Examples
+    --------
     >>> from htmltools import TagList, div
     >>> TagList("hello", div(id="foo", class_="bar"))
     hello
     <div id="foo" class="bar"></div>
     """
 
     def __init__(self, *args: TagChild) -> None:
@@ -197,15 +202,16 @@
         # with 0, 1, or more items (if it returns TagList).
         for i in reversed(range(len(cp))):
             child = cp[i]
 
             if isinstance(child, Tagifiable):
                 tagified_child = child.tagify()
                 if isinstance(tagified_child, TagList):
-                    # If the Tagifiable object returned a TagList, flatten it into this one.
+                    # If the Tagifiable object returned a TagList, flatten it into this
+                    # one.
                     cp[i : i + 1] = _tagchilds_to_tagnodes(tagified_child)
                 else:
                     cp[i] = tagified_child
 
             elif isinstance(child, MetadataNode):
                 cp[i] = copy(child)
         return cp
@@ -223,15 +229,16 @@
         libdir
             The directory to save the dependencies to.
         include_version
             Whether to include the version number in the dependency folder name.
 
         Returns
         -------
-        The path to the generated HTML file.
+        :
+            The path to the generated HTML file.
         """
 
         return HTMLDocument(self).save_html(
             file, libdir=libdir, include_version=include_version
         )
 
     def render(self) -> RenderedHTML:
@@ -390,15 +397,19 @@
 
     def __setitem__(self, name: str, value: TagAttrValue) -> None:
         val = self._normalize_attr_value(value)
         if val is not None:
             nm = self._normalize_attr_name(name)
             super().__setitem__(nm, val)
 
-    def update(self, *args: Mapping[str, TagAttrValue], **kwargs: TagAttrValue) -> None:
+    def update(  # type: ignore[reportIncompatibleMethodOverride] # TODO-future: fix typing
+        self,
+        *args: Mapping[str, TagAttrValue],
+        **kwargs: TagAttrValue,
+    ) -> None:
         if kwargs:
             args = args + (kwargs,)
 
         attrz: dict[str, str | HTML] = {}
         for arg in args:
             for k, v in arg.items():
                 val = self._normalize_attr_value(v)
@@ -483,18 +494,18 @@
     results in formatting that is easier to read.
 
     The only times that whitespace is not added around tags is when two sibling tags
     have `_add_ws=False`, or when a tag and its first child both have `_add_ws=False`.
     Bare strings are treated as children with `_add_ws=False`.
 
     If you need fine control over whitespace in the output HTML, you can create tags
-    with `_add_ws=False` and manually add whitespace, like `div("\n", span("a"),
+    with `_add_ws=False` and manually add whitespace, like `div("\\n", span("a"),
     _add_ws=False)`.
 
-    Example
+    Examples
     --------
     >>> from htmltools import div
     >>> x = div("hello", id="foo", class_="bar")
     >>> x
     <div id="foo" class="bar">hello</div>
     >>> x.show()
     """
@@ -546,52 +557,128 @@
     def append(self, *args: TagChild) -> None:
         """
         Append tag children to the end of the list.
         """
 
         self.children.append(*args)
 
-    def add_class(self, x: str) -> "Tag":
+    def add_class(self: TagT, class_: str, *, prepend: bool = False) -> TagT:
         """
-        Add an HTML class attribute.
+        Add a class value to the HTML class attribute.
 
         Parameters
         ----------
-        x
+        class_
             The class name to add.
+        prepend
+            Bool that determines if the `class` is added to the beginning or end of the
+            class attribute.
 
         Returns
         -------
-        The modified tag.
+        :
+            The modified tag.
         """
-        cls = self.attrs.get("class")
-        if cls:
-            x = cls + " " + x
-        self.attrs["class"] = x
+        if prepend:
+            self.attrs.update({"class": class_}, {"class": self.attrs.get("class")})
+        else:
+            self.attrs.update({"class": self.attrs.get("class")}, {"class": class_})
+        return self
+
+    def remove_class(self: TagT, class_: str) -> TagT:
+        """
+        Remove a class value from the HTML class attribute.
+
+        Parameters
+        ----------
+        class_
+            The class name to remove.
+
+        Returns
+        -------
+        :
+            The modified tag.
+        """
+        # Nothing to do if no class is specified
+        if not class_:
+            return self
+        cls = self.attrs.get("class") or ""
+
+        # If no class attribute exists, there's nothing to remove
+        if not cls:
+            return self
+
+        # Coerce and clean
+        class_ = str(class_).strip()
+
+        # Remove the class value from the ordered set of class values
+        # Note: .split() splits on any whitespace and removes empty strings
+        new_classes = [cls_val for cls_val in cls.split() if cls_val != class_]
+        if len(new_classes) > 0:
+            # Store the new class value
+            self.attrs.update({"class": " ".join(new_classes)})
+        else:
+            # If no class values remain, remove the class attribute
+            self.attrs.pop("class")
         return self
 
     def has_class(self, class_: str) -> bool:
         """
-        Check if the tag has a particular class.
+        Check if the tag has a particular class value.
 
         Parameters
         ----------
         class_
             The class name to check for.
 
         Returns
         -------
-        ``True`` if the tag has the class, ``False`` otherwise.
+        :
+            ``True`` if the tag has the class, ``False`` otherwise.
         """
         cls = self.attrs.get("class")
         if cls:
-            return class_ in cls.split(" ")
+            return class_ in cls.split()
         else:
             return False
 
+    def add_style(self: TagT, style: str, *, prepend: bool = False) -> TagT:
+        """
+        Add a style value(s) to the HTML style attribute.
+
+        Parameters
+        ----------
+        style
+            CSS properties and values already properly formatted. Each should already
+            contain trailing semicolons.
+        prepend
+            Bool that determines if the `style` is added to the beginning or end of the
+            style attribute.
+
+        See Also
+        --------
+        ~htmltools.css
+
+        Returns
+        -------
+        :
+            The modified tag.
+        """
+
+        if isinstance(  # type: ignore[reportUnnecessaryIsInstance]
+            style, str
+        ) and not style.endswith(";"):
+            raise ValueError("`Tag.add_style(style=)` must end with a semicolon")
+
+        if prepend:
+            self.attrs.update({"style": style}, {"style": self.attrs.get("style")})
+        else:
+            self.attrs.update({"style": self.attrs.get("style")}, {"style": style})
+        return self
+
     def tagify(self: TagT) -> TagT:
         """
         Convert any tagifiable children to Tag/TagList objects.
         """
 
         cp = copy(self)
         cp.children = cp.children.tagify()
@@ -749,16 +836,16 @@
     Parameters
     ----------
     *args
         Children to add to the document.
     **kwargs
         Attributes to set on the document (i.e., the root <html> tag).
 
-    Example
-    -------
+    Examples
+    --------
     >>> from htmltools import HTMLDocument, h1, tags
     >>> HTMLDocument(h1("Hello"), tags.meta(name="description", content="test"), lang = "en")
     """
 
     def __init__(
         self,
         *args: TagChild,
@@ -865,15 +952,15 @@
         ):
             body = cast(Tag, content[0])
         else:
             body = Tag("body", content)
 
         body = body.tagify()
 
-        html = Tag("html", Tag("head"), body, **self._html_attr_args)
+        html = Tag("html", Tag("head"), body, _add_ws=True, **self._html_attr_args)
         html = HTMLDocument._hoist_head_content(html, lib_prefix, include_version)
         return html
 
     # Given an <html> tag object, copies the top node, then extracts dependencies from
     # the tree, and inserts the content from those dependencies into the <head>, such as
     # <link> and <script> tags.
     @staticmethod
@@ -929,16 +1016,16 @@
 # HTML strings
 # =============================================================================
 class HTML(str):
     """
     Mark a string as raw HTML. This will prevent the string from being escaped when
     rendered inside an HTML tag.
 
-    Example
-    -------
+    Examples
+    --------
     >>> from htmltools import HTML, div
     >>> div("<p>Hello</p>")
     <div>&lt;p&gt;Hello&lt;/p&gt;</div>
     >>> div(HTML("<p>Hello</p>"))
     <div><p>Hello</p></div>
     """
 
@@ -1078,16 +1165,16 @@
         ``False``, only the files specified in script and stylesheet are treated as
         dependency files.
     meta
         ``<meta>`` tags to include in the document's ``<head>``.
     head
         Tags to include in the document's ``<head>``.
 
-    Example
-    -------
+    Examples
+    --------
     >>> dep = HTMLDependency(
             name="mypackage",
             version="1.0",
             source={
                 "package": "mypackage",
                 "subdir": "lib/",
             },
@@ -1179,15 +1266,14 @@
         """
 
         src = self.source
         if src is None:
             return {"source": "", "href": ""}
 
         if "href" in src:
-            src = cast(HTMLDependencyUrl, src)
             return {"source": "", "href": src["href"]}
 
         pkg = src.get("package", None)
         if pkg is None:
             source = os.path.realpath(src["subdir"])
         else:
             source = os.path.join(package_dir(pkg), src["subdir"])
@@ -1348,16 +1434,16 @@
     ----
     If the same content, ``x``, is included in a document multiple times via
     ``head_content(x)``, ``x`` will only appear once in the final HTML document's
     ``<head>``. More often than not, this is desirable behavior, but if you need the
     same content included multiple times, you can add some irrelevant/empty tags (e.g.,
     ``TagList(x, Tag("meta"))``) to make sure ``x`` is included multiple times.
 
-    Example
-    -------
+    Examples
+    --------
     >>> from htmltools import *
     >>> x = div(head_content(title("My Title")))
     >>> print(HTMLDocument(x).render()["html"])
     <!DOCTYPE html>
     <html>
       <head>
         <meta charset="utf-8"/>
```

### Comparing `htmltools-0.2.1/htmltools/_jsx.py` & `htmltools-0.3.0/htmltools/_jsx.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,18 @@
         super().__init__()
         self.update(**kwargs)
 
     def __setitem__(self, name: str, value: JSXTagAttrValue) -> None:
         nm = self._normalize_attr_name(name)
         super().__setitem__(nm, value)
 
-    def update(
-        self, *args: Mapping[str, JSXTagAttrValue], **kwargs: JSXTagAttrValue
+    def update(  # type: ignore[reportIncompatibleMethodOverride] # TODO-future: fix typing
+        self,
+        *args: Mapping[str, JSXTagAttrValue],
+        **kwargs: JSXTagAttrValue,
     ) -> None:
         for arg in args:
             self._update(arg)
         self._update(kwargs)
 
     def _update(self, __m: Mapping[str, JSXTagAttrValue]) -> None:
         attrs: dict[str, JSXTagAttrValue] = {}
@@ -296,15 +298,16 @@
         The name of the JSX tag (should be camelCase and start with a capital letter).
     allowedProps
         A list of allowed properties for the tag. If ``None``, all properties are
         allowed.
 
     Returns
     -------
-    JSXTag
+    :
+        JSXTag
 
     Examples
     --------
     >>> from htmltools import jsx_tag_create
     >>> MyTag = jsx_tag_create("MyTag")
     >>> MyTag(id="foo", class_="bar")
     <script type="text/javascript">
@@ -360,15 +363,14 @@
 
     # jsx() + jsx() should return jsx()
     def __add__(self, other: "str | jsx") -> str:
         res = str.__add__(self, other)
         return jsx(res) if isinstance(other, jsx) else res
 
 
-def _lib_dependency(pkg: str, script: ScriptItem, **kwargs: object) -> HTMLDependency:
+def _lib_dependency(pkg: str, script: ScriptItem) -> HTMLDependency:
     return HTMLDependency(
         name=pkg,
         version=versions[pkg],
         source={"package": "htmltools", "subdir": "lib/" + pkg},
         script=script,
-        **kwargs,
     )
```

### Comparing `htmltools-0.2.1/htmltools/_util.py` & `htmltools-0.3.0/htmltools/_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         default) for style attributes, and either "\n" or None for style blocks.
     **kwargs
         Named style properties, where the name is the property name and the argument is
         the property value.
 
     Returns
     -------
-    A string of CSS style declarations, or ``None`` if no properties were given.
+    :
+        A string of CSS style declarations, or ``None`` if no properties were given.
 
     Example
     -------
     >>> from htmltools import css
     >>> css(font_size = "12px", backgroundColor = "red")
     'font-size:12px;background-color:red;'
```

### Comparing `htmltools-0.2.1/htmltools/lib/react/react.production.min.js` & `htmltools-0.3.0/htmltools/lib/react/react.production.min.js`

 * *Files identical despite different names*

### Comparing `htmltools-0.2.1/htmltools/lib/react-dom/react-dom.production.min.js` & `htmltools-0.3.0/htmltools/lib/react-dom/react-dom.production.min.js`

 * *Files identical despite different names*

### Comparing `htmltools-0.2.1/htmltools/svg.py` & `htmltools-0.3.0/htmltools/svg.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("a", *args, _add_ws=_add_ws, **kwargs)
@@ -50,15 +51,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("animate", *args, _add_ws=_add_ws, **kwargs)
@@ -77,15 +79,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("animateMotion", *args, _add_ws=_add_ws, **kwargs)
@@ -104,15 +107,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("animateTransform", *args, _add_ws=_add_ws, **kwargs)
@@ -131,15 +135,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("circle", *args, _add_ws=_add_ws, **kwargs)
@@ -158,15 +163,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("clipPath", *args, _add_ws=_add_ws, **kwargs)
@@ -185,15 +191,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("defs", *args, _add_ws=_add_ws, **kwargs)
@@ -212,15 +219,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("desc", *args, _add_ws=_add_ws, **kwargs)
@@ -239,15 +247,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("discard", *args, _add_ws=_add_ws, **kwargs)
@@ -266,15 +275,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("ellipse", *args, _add_ws=_add_ws, **kwargs)
@@ -293,15 +303,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feBlend", *args, _add_ws=_add_ws, **kwargs)
@@ -320,15 +331,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feColorMatrix", *args, _add_ws=_add_ws, **kwargs)
@@ -347,15 +359,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feComponentTransfer", *args, _add_ws=_add_ws, **kwargs)
@@ -374,15 +387,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feComposite", *args, _add_ws=_add_ws, **kwargs)
@@ -401,15 +415,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feConvolveMatrix", *args, _add_ws=_add_ws, **kwargs)
@@ -428,15 +443,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feDiffuseLighting", *args, _add_ws=_add_ws, **kwargs)
@@ -455,15 +471,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feDisplacementMap", *args, _add_ws=_add_ws, **kwargs)
@@ -482,15 +499,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feDistantLight", *args, _add_ws=_add_ws, **kwargs)
@@ -509,15 +527,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feDropShadow", *args, _add_ws=_add_ws, **kwargs)
@@ -536,15 +555,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feFlood", *args, _add_ws=_add_ws, **kwargs)
@@ -563,15 +583,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feFuncA", *args, _add_ws=_add_ws, **kwargs)
@@ -590,15 +611,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feFuncB", *args, _add_ws=_add_ws, **kwargs)
@@ -617,15 +639,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feFuncG", *args, _add_ws=_add_ws, **kwargs)
@@ -644,15 +667,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feFuncR", *args, _add_ws=_add_ws, **kwargs)
@@ -671,15 +695,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feGaussianBlur", *args, _add_ws=_add_ws, **kwargs)
@@ -698,15 +723,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feImage", *args, _add_ws=_add_ws, **kwargs)
@@ -725,15 +751,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feMerge", *args, _add_ws=_add_ws, **kwargs)
@@ -752,15 +779,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feMergeNode", *args, _add_ws=_add_ws, **kwargs)
@@ -779,15 +807,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feMorphology", *args, _add_ws=_add_ws, **kwargs)
@@ -806,15 +835,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feOffset", *args, _add_ws=_add_ws, **kwargs)
@@ -833,15 +863,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("fePointLight", *args, _add_ws=_add_ws, **kwargs)
@@ -860,15 +891,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feSpecularLighting", *args, _add_ws=_add_ws, **kwargs)
@@ -887,15 +919,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feSpotLight", *args, _add_ws=_add_ws, **kwargs)
@@ -914,15 +947,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feTile", *args, _add_ws=_add_ws, **kwargs)
@@ -941,15 +975,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("feTurbulence", *args, _add_ws=_add_ws, **kwargs)
@@ -968,15 +1003,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("filter", *args, _add_ws=_add_ws, **kwargs)
@@ -995,15 +1031,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("foreignObject", *args, _add_ws=_add_ws, **kwargs)
@@ -1022,15 +1059,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("g", *args, _add_ws=_add_ws, **kwargs)
@@ -1049,15 +1087,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("hatch", *args, _add_ws=_add_ws, **kwargs)
@@ -1076,15 +1115,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("hatchpath", *args, _add_ws=_add_ws, **kwargs)
@@ -1103,15 +1143,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("image", *args, _add_ws=_add_ws, **kwargs)
@@ -1130,15 +1171,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("line", *args, _add_ws=_add_ws, **kwargs)
@@ -1157,15 +1199,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("linearGradient", *args, _add_ws=_add_ws, **kwargs)
@@ -1184,15 +1227,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("marker", *args, _add_ws=_add_ws, **kwargs)
@@ -1211,15 +1255,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("mask", *args, _add_ws=_add_ws, **kwargs)
@@ -1238,15 +1283,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("metadata", *args, _add_ws=_add_ws, **kwargs)
@@ -1265,15 +1311,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("mpath", *args, _add_ws=_add_ws, **kwargs)
@@ -1292,15 +1339,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("path", *args, _add_ws=_add_ws, **kwargs)
@@ -1319,15 +1367,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("pattern", *args, _add_ws=_add_ws, **kwargs)
@@ -1346,15 +1395,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("polygon", *args, _add_ws=_add_ws, **kwargs)
@@ -1373,15 +1423,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("polyline", *args, _add_ws=_add_ws, **kwargs)
@@ -1400,15 +1451,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("radialGradient", *args, _add_ws=_add_ws, **kwargs)
@@ -1427,15 +1479,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("rect", *args, _add_ws=_add_ws, **kwargs)
@@ -1454,15 +1507,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("script", *args, _add_ws=_add_ws, **kwargs)
@@ -1481,15 +1535,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("set", *args, _add_ws=_add_ws, **kwargs)
@@ -1508,15 +1563,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("stop", *args, _add_ws=_add_ws, **kwargs)
@@ -1535,15 +1591,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("style", *args, _add_ws=_add_ws, **kwargs)
@@ -1562,15 +1619,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("svg", *args, _add_ws=_add_ws, **kwargs)
@@ -1589,15 +1647,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("switch", *args, _add_ws=_add_ws, **kwargs)
@@ -1616,15 +1675,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("symbol", *args, _add_ws=_add_ws, **kwargs)
@@ -1643,15 +1703,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("text", *args, _add_ws=_add_ws, **kwargs)
@@ -1670,15 +1731,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("textPath", *args, _add_ws=_add_ws, **kwargs)
@@ -1697,15 +1759,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("title", *args, _add_ws=_add_ws, **kwargs)
@@ -1724,15 +1787,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("tspan", *args, _add_ws=_add_ws, **kwargs)
@@ -1751,15 +1815,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("use", *args, _add_ws=_add_ws, **kwargs)
@@ -1778,15 +1843,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("view", *args, _add_ws=_add_ws, **kwargs)
```

### Comparing `htmltools-0.2.1/htmltools/tags.py` & `htmltools-0.3.0/htmltools/tags.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("html", *args, _add_ws=_add_ws, **kwargs)
@@ -70,15 +71,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("base", *args, _add_ws=_add_ws, **kwargs)
@@ -97,15 +99,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("head", *args, _add_ws=_add_ws, **kwargs)
@@ -125,15 +128,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("link", *args, _add_ws=_add_ws, **kwargs)
@@ -152,15 +156,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("meta", *args, _add_ws=_add_ws, **kwargs)
@@ -179,15 +184,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("style", *args, _add_ws=_add_ws, **kwargs)
@@ -206,15 +212,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("title", *args, _add_ws=_add_ws, **kwargs)
@@ -233,15 +240,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("body", *args, _add_ws=_add_ws, **kwargs)
@@ -260,15 +268,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("address", *args, _add_ws=_add_ws, **kwargs)
@@ -287,15 +296,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("article", *args, _add_ws=_add_ws, **kwargs)
@@ -314,15 +324,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("aside", *args, _add_ws=_add_ws, **kwargs)
@@ -341,15 +352,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("footer", *args, _add_ws=_add_ws, **kwargs)
@@ -368,15 +380,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("header", *args, _add_ws=_add_ws, **kwargs)
@@ -395,15 +408,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("h1", *args, _add_ws=_add_ws, **kwargs)
@@ -422,15 +436,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("h2", *args, _add_ws=_add_ws, **kwargs)
@@ -449,15 +464,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("h3", *args, _add_ws=_add_ws, **kwargs)
@@ -476,15 +492,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("h4", *args, _add_ws=_add_ws, **kwargs)
@@ -503,15 +520,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("h5", *args, _add_ws=_add_ws, **kwargs)
@@ -530,15 +548,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("h6", *args, _add_ws=_add_ws, **kwargs)
@@ -557,15 +576,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("main", *args, _add_ws=_add_ws, **kwargs)
@@ -584,15 +604,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("nav", *args, _add_ws=_add_ws, **kwargs)
@@ -611,15 +632,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("section", *args, _add_ws=_add_ws, **kwargs)
@@ -638,15 +660,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("blockquote", *args, _add_ws=_add_ws, **kwargs)
@@ -665,15 +688,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("dd", *args, _add_ws=_add_ws, **kwargs)
@@ -692,15 +716,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("div", *args, _add_ws=_add_ws, **kwargs)
@@ -719,15 +744,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("dl", *args, _add_ws=_add_ws, **kwargs)
@@ -746,15 +772,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("dt", *args, _add_ws=_add_ws, **kwargs)
@@ -773,15 +800,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("figcaption", *args, _add_ws=_add_ws, **kwargs)
@@ -800,15 +828,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("figure", *args, _add_ws=_add_ws, **kwargs)
@@ -827,15 +856,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("hr", *args, _add_ws=_add_ws, **kwargs)
@@ -854,15 +884,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("li", *args, _add_ws=_add_ws, **kwargs)
@@ -881,15 +912,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("menu", *args, _add_ws=_add_ws, **kwargs)
@@ -908,15 +940,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("ol", *args, _add_ws=_add_ws, **kwargs)
@@ -935,15 +968,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("p", *args, _add_ws=_add_ws, **kwargs)
@@ -962,15 +996,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("pre", *args, _add_ws=_add_ws, **kwargs)
@@ -989,15 +1024,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("ul", *args, _add_ws=_add_ws, **kwargs)
@@ -1016,15 +1052,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("a", *args, _add_ws=_add_ws, **kwargs)
@@ -1043,15 +1080,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("abbr", *args, _add_ws=_add_ws, **kwargs)
@@ -1070,15 +1108,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("b", *args, _add_ws=_add_ws, **kwargs)
@@ -1097,15 +1136,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("bdi", *args, _add_ws=_add_ws, **kwargs)
@@ -1124,15 +1164,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("bdo", *args, _add_ws=_add_ws, **kwargs)
@@ -1151,15 +1192,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("br", *args, _add_ws=_add_ws, **kwargs)
@@ -1178,15 +1220,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("cite", *args, _add_ws=_add_ws, **kwargs)
@@ -1205,15 +1248,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("code", *args, _add_ws=_add_ws, **kwargs)
@@ -1232,15 +1276,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("data", *args, _add_ws=_add_ws, **kwargs)
@@ -1259,15 +1304,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("dfn", *args, _add_ws=_add_ws, **kwargs)
@@ -1286,15 +1332,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("em", *args, _add_ws=_add_ws, **kwargs)
@@ -1313,15 +1360,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("i", *args, _add_ws=_add_ws, **kwargs)
@@ -1340,15 +1388,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("kbd", *args, _add_ws=_add_ws, **kwargs)
@@ -1367,15 +1416,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("mark", *args, _add_ws=_add_ws, **kwargs)
@@ -1394,15 +1444,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("q", *args, _add_ws=_add_ws, **kwargs)
@@ -1421,15 +1472,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("rp", *args, _add_ws=_add_ws, **kwargs)
@@ -1448,15 +1500,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("rt", *args, _add_ws=_add_ws, **kwargs)
@@ -1475,15 +1528,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("ruby", *args, _add_ws=_add_ws, **kwargs)
@@ -1502,15 +1556,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("s", *args, _add_ws=_add_ws, **kwargs)
@@ -1529,15 +1584,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("samp", *args, _add_ws=_add_ws, **kwargs)
@@ -1556,15 +1612,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("small", *args, _add_ws=_add_ws, **kwargs)
@@ -1583,15 +1640,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("span", *args, _add_ws=_add_ws, **kwargs)
@@ -1610,15 +1668,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("strong", *args, _add_ws=_add_ws, **kwargs)
@@ -1637,15 +1696,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("sub", *args, _add_ws=_add_ws, **kwargs)
@@ -1664,15 +1724,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("sup", *args, _add_ws=_add_ws, **kwargs)
@@ -1691,15 +1752,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("time", *args, _add_ws=_add_ws, **kwargs)
@@ -1718,15 +1780,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("u", *args, _add_ws=_add_ws, **kwargs)
@@ -1745,15 +1808,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("var", *args, _add_ws=_add_ws, **kwargs)
@@ -1772,15 +1836,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("wbr", *args, _add_ws=_add_ws, **kwargs)
@@ -1799,15 +1864,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("area", *args, _add_ws=_add_ws, **kwargs)
@@ -1826,15 +1892,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("audio", *args, _add_ws=_add_ws, **kwargs)
@@ -1853,15 +1920,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("img", *args, _add_ws=_add_ws, **kwargs)
@@ -1880,15 +1948,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("map", *args, _add_ws=_add_ws, **kwargs)
@@ -1907,15 +1976,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("track", *args, _add_ws=_add_ws, **kwargs)
@@ -1934,15 +2004,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("video", *args, _add_ws=_add_ws, **kwargs)
@@ -1961,15 +2032,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("embed", *args, _add_ws=_add_ws, **kwargs)
@@ -1988,15 +2060,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("iframe", *args, _add_ws=_add_ws, **kwargs)
@@ -2015,15 +2088,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("object", *args, _add_ws=_add_ws, **kwargs)
@@ -2042,15 +2116,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("param", *args, _add_ws=_add_ws, **kwargs)
@@ -2069,15 +2144,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("picture", *args, _add_ws=_add_ws, **kwargs)
@@ -2096,15 +2172,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("portal", *args, _add_ws=_add_ws, **kwargs)
@@ -2123,15 +2200,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("source", *args, _add_ws=_add_ws, **kwargs)
@@ -2154,15 +2232,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("svg", *args, _add_ws=_add_ws, **kwargs)
@@ -2185,15 +2264,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("math", *args, _add_ws=_add_ws, **kwargs)
@@ -2212,15 +2292,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("canvas", *args, _add_ws=_add_ws, **kwargs)
@@ -2239,15 +2320,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("noscript", *args, _add_ws=_add_ws, **kwargs)
@@ -2266,15 +2348,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("script", *args, _add_ws=_add_ws, **kwargs)
@@ -2293,15 +2376,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("ins", *args, _add_ws=_add_ws, **kwargs)
@@ -2320,15 +2404,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("caption", *args, _add_ws=_add_ws, **kwargs)
@@ -2347,15 +2432,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("col", *args, _add_ws=_add_ws, **kwargs)
@@ -2374,15 +2460,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("colgroup", *args, _add_ws=_add_ws, **kwargs)
@@ -2401,15 +2488,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("table", *args, _add_ws=_add_ws, **kwargs)
@@ -2428,15 +2516,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("tbody", *args, _add_ws=_add_ws, **kwargs)
@@ -2455,15 +2544,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("td", *args, _add_ws=_add_ws, **kwargs)
@@ -2482,15 +2572,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("tfoot", *args, _add_ws=_add_ws, **kwargs)
@@ -2509,15 +2600,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("th", *args, _add_ws=_add_ws, **kwargs)
@@ -2536,15 +2628,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("thead", *args, _add_ws=_add_ws, **kwargs)
@@ -2563,15 +2656,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("tr", *args, _add_ws=_add_ws, **kwargs)
@@ -2590,15 +2684,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("button", *args, _add_ws=_add_ws, **kwargs)
@@ -2617,15 +2712,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("datalist", *args, _add_ws=_add_ws, **kwargs)
@@ -2644,15 +2740,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("fieldset", *args, _add_ws=_add_ws, **kwargs)
@@ -2671,15 +2768,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("form", *args, _add_ws=_add_ws, **kwargs)
@@ -2698,15 +2796,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("input", *args, _add_ws=_add_ws, **kwargs)
@@ -2725,15 +2824,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("label", *args, _add_ws=_add_ws, **kwargs)
@@ -2752,15 +2852,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("legend", *args, _add_ws=_add_ws, **kwargs)
@@ -2779,15 +2880,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("meter", *args, _add_ws=_add_ws, **kwargs)
@@ -2806,15 +2908,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("optgroup", *args, _add_ws=_add_ws, **kwargs)
@@ -2833,15 +2936,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("option", *args, _add_ws=_add_ws, **kwargs)
@@ -2860,15 +2964,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("output", *args, _add_ws=_add_ws, **kwargs)
@@ -2887,15 +2992,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("progress", *args, _add_ws=_add_ws, **kwargs)
@@ -2914,15 +3020,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("select", *args, _add_ws=_add_ws, **kwargs)
@@ -2941,15 +3048,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("textarea", *args, _add_ws=_add_ws, **kwargs)
@@ -2968,15 +3076,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("details", *args, _add_ws=_add_ws, **kwargs)
@@ -2995,15 +3104,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("dialog", *args, _add_ws=_add_ws, **kwargs)
@@ -3022,15 +3132,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("summary", *args, _add_ws=_add_ws, **kwargs)
@@ -3049,15 +3160,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("slot", *args, _add_ws=_add_ws, **kwargs)
@@ -3076,15 +3188,16 @@
     _add_ws
         Whether whitespace should be added around this tag.
     **kwargs
         Attributes to this tag.
 
     Returns
     -------
-    Tag
+    :
+        A :func:`~htmltools.Tag` object.
 
     See Also
     --------
     ~htmltools.Tag
     """
 
     return Tag("template", *args, _add_ws=_add_ws, **kwargs)
```

### Comparing `htmltools-0.2.1/htmltools.egg-info/PKG-INFO` & `htmltools-0.3.0/htmltools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: htmltools
-Version: 0.2.1
+Version: 0.3.0
 Summary: Tools for HTML generation and output.
 Home-page: https://github.com/rstudio/py-htmltools
 Author: Carson Sievert
 Author-email: carson@rstudio.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rstudio/py-htmltools/issues
 Project-URL: Source Code, https://github.com/rstudio/py-htmltools
 Keywords: html
 Platform: any
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: HTML
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # htmltools
```

### Comparing `htmltools-0.2.1/setup.cfg` & `htmltools-0.3.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -8,33 +8,32 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = html
 license = MIT
 license_file = LICENSE
 platforms = any
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Text Processing :: Markup :: HTML
 project_urls = 
 	Bug Tracker = https://github.com/rstudio/py-htmltools/issues
 	Source Code = https://github.com/rstudio/py-htmltools
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 packages = find:
 test_suite = tests
 include_package_data = True
 setup_requires = 
 	setuptools
 install_requires = 
 	typing-extensions>=3.10.0.0
@@ -44,16 +43,15 @@
 zip_safe = False
 
 [options.extras_require]
 test = 
 	pytest>=6.2.4
 dev = 
 	black>=23.1.0
-	flake8==5.0.4;python_version<="3.7"
-	flake8>=6.0.0;python_version>"3.7"
+	flake8>=6.0.0
 	isort>=5.11.2
 	pyright>=1.1.284
 	pre-commit>=2.15.0
 	snapshottest>=0.6.0
 	wheel
 
 [options.packages.find]
```

