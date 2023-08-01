# Comparing `tmp/drf-serializer-prefetch-1.1.0b0.tar.gz` & `tmp/drf-serializer-prefetch-1.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-serializer-prefetch-1.1.0b0.tar", last modified: Thu Jul  6 13:17:34 2023, max compression
+gzip compressed data, was "drf-serializer-prefetch-1.1.0b1.tar", last modified: Tue Aug  1 20:49:04 2023, max compression
```

## Comparing `drf-serializer-prefetch-1.1.0b0.tar` & `drf-serializer-prefetch-1.1.0b1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-07-06 13:17:34.251536 drf-serializer-prefetch-1.1.0b0/
--rw-rw-r--   0 max       (1000) max       (1000)     1073 2023-06-20 13:02:29.000000 drf-serializer-prefetch-1.1.0b0/LICENSE
--rw-rw-r--   0 max       (1000) max       (1000)     9307 2023-07-06 13:17:34.247536 drf-serializer-prefetch-1.1.0b0/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     8990 2023-06-21 19:04:46.000000 drf-serializer-prefetch-1.1.0b0/README.md
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-07-06 13:17:34.247536 drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)     9307 2023-07-06 13:17:34.000000 drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)      465 2023-07-06 13:17:34.000000 drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2023-07-06 13:17:34.000000 drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)       40 2023-07-06 13:17:34.000000 drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)       26 2023-07-06 13:17:34.000000 drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/top_level.txt
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-07-06 13:17:34.247536 drf-serializer-prefetch-1.1.0b0/serializer_prefetch/
--rw-rw-r--   0 max       (1000) max       (1000)      139 2023-06-20 14:41:43.000000 drf-serializer-prefetch-1.1.0b0/serializer_prefetch/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)    14025 2023-07-06 13:14:30.000000 drf-serializer-prefetch-1.1.0b0/serializer_prefetch/base.py
--rw-rw-r--   0 max       (1000) max       (1000)       38 2023-07-06 13:17:34.251536 drf-serializer-prefetch-1.1.0b0/setup.cfg
--rw-rw-r--   0 max       (1000) max       (1000)      680 2023-07-06 13:17:25.000000 drf-serializer-prefetch-1.1.0b0/setup.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-07-06 13:17:34.247536 drf-serializer-prefetch-1.1.0b0/tests/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-20 15:59:03.000000 drf-serializer-prefetch-1.1.0b0/tests/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)      674 2023-07-06 13:14:30.000000 drf-serializer-prefetch-1.1.0b0/tests/models.py
--rw-rw-r--   0 max       (1000) max       (1000)      708 2023-06-21 14:24:52.000000 drf-serializer-prefetch-1.1.0b0/tests/serializers.py
--rw-rw-r--   0 max       (1000) max       (1000)      381 2023-06-20 18:58:38.000000 drf-serializer-prefetch-1.1.0b0/tests/settings.py
--rw-rw-r--   0 max       (1000) max       (1000)     4003 2023-07-06 13:14:30.000000 drf-serializer-prefetch-1.1.0b0/tests/test_conditions.py
--rw-rw-r--   0 max       (1000) max       (1000)     2404 2023-06-21 15:24:05.000000 drf-serializer-prefetch-1.1.0b0/tests/test_errors.py
--rw-rw-r--   0 max       (1000) max       (1000)    25671 2023-07-06 13:14:35.000000 drf-serializer-prefetch-1.1.0b0/tests/test_serializers.py
+drwxrwxrwx   0        0        0        0 2023-08-01 20:49:04.996529 drf-serializer-prefetch-1.1.0b1/
+-rw-rw-rw-   0        0        0     1094 2023-08-01 20:31:22.000000 drf-serializer-prefetch-1.1.0b1/LICENSE
+-rw-rw-rw-   0        0        0     9517 2023-08-01 20:49:04.996529 drf-serializer-prefetch-1.1.0b1/PKG-INFO
+-rw-rw-rw-   0        0        0     9190 2023-08-01 20:31:22.000000 drf-serializer-prefetch-1.1.0b1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 20:49:04.988144 drf-serializer-prefetch-1.1.0b1/drf_serializer_prefetch.egg-info/
+-rw-rw-rw-   0        0        0     9517 2023-08-01 20:49:04.000000 drf-serializer-prefetch-1.1.0b1/drf_serializer_prefetch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-08-01 20:49:04.000000 drf-serializer-prefetch-1.1.0b1/drf_serializer_prefetch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 20:49:04.000000 drf-serializer-prefetch-1.1.0b1/drf_serializer_prefetch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-01 20:49:04.000000 drf-serializer-prefetch-1.1.0b1/drf_serializer_prefetch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-08-01 20:49:04.000000 drf-serializer-prefetch-1.1.0b1/drf_serializer_prefetch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 20:49:04.989119 drf-serializer-prefetch-1.1.0b1/serializer_prefetch/
+-rw-rw-rw-   0        0        0      142 2023-08-01 20:31:22.000000 drf-serializer-prefetch-1.1.0b1/serializer_prefetch/__init__.py
+-rw-rw-rw-   0        0        0    14937 2023-08-01 20:40:19.000000 drf-serializer-prefetch-1.1.0b1/serializer_prefetch/base.py
+-rw-rw-rw-   0        0        0       42 2023-08-01 20:49:04.996529 drf-serializer-prefetch-1.1.0b1/setup.cfg
+-rw-rw-rw-   0        0        0      702 2023-08-01 20:42:41.000000 drf-serializer-prefetch-1.1.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 20:49:04.995547 drf-serializer-prefetch-1.1.0b1/tests/
+-rw-rw-rw-   0        0        0        0 2023-08-01 20:31:22.000000 drf-serializer-prefetch-1.1.0b1/tests/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-08-01 20:33:06.000000 drf-serializer-prefetch-1.1.0b1/tests/models.py
+-rw-rw-rw-   0        0        0      734 2023-08-01 20:31:22.000000 drf-serializer-prefetch-1.1.0b1/tests/serializers.py
+-rw-rw-rw-   0        0        0      402 2023-08-01 20:31:22.000000 drf-serializer-prefetch-1.1.0b1/tests/settings.py
+-rw-rw-rw-   0        0        0     4131 2023-08-01 20:33:06.000000 drf-serializer-prefetch-1.1.0b1/tests/test_conditions.py
+-rw-rw-rw-   0        0        0     2473 2023-08-01 20:31:22.000000 drf-serializer-prefetch-1.1.0b1/tests/test_errors.py
+-rw-rw-rw-   0        0        0    26491 2023-08-01 20:33:06.000000 drf-serializer-prefetch-1.1.0b1/tests/test_serializers.py
```

### Comparing `drf-serializer-prefetch-1.1.0b0/PKG-INFO` & `drf-serializer-prefetch-1.1.0b1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,210 +1,210 @@
-Metadata-Version: 2.1
-Name: drf-serializer-prefetch
-Version: 1.1.0b0
-Summary: An automatic prefetcher for django-rest-framework.
-Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
-Author: Maxime Toussaint
-Author-email: m.toussaint@mail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![codecov](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch/branch/main/graph/badge.svg?token=MFI4E7L7SU)](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch)
-
-# drf-serializer-prefetch
-
-An automatic prefetcher that looks at the serializer fields and determines what needs to be prefetched accordingly.
-
-## Installation
-
-To install, call `pip install drf-serializer-prefetch`.
-
-## Usage
-
-In its most simple form, the serializer prefetch can be used by simply adding `PrefetchingSerializerMixin` to the class definition of the model serializer you want to allow automatic prefetching for like so:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-Using it like this, the Prefetching Serializer will be able to see what fields will be returned and prefetch them accordingly.
-
-However, SerializerMethodFields are an issue for the Prefetching Serializer, as those can make calls that are only done at run time. The Prefetching Serializer does not make any kind of file analysis, and as such cannot know what will happen in those methods. If you are calling a related model in that function, you can define either `select_related` or `prefetch_related` on the model. The fields defined here will also be taken into account. As for usual with Django, you can go as deep as you need here. For example, you could add `user`, or you could add `user__pizza_set`, if you were to loop over the user's pizzas.
-
-For example:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    select_related = ('other_model',)
-
-    other_field = serializers.SerializerMethodField()
-
-    def get_other_field(self, obj):
-        return obj.other_model.other_field
-
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-If you need to add some logic to when the prefetching should happen, you can also define `get_select_related` or `get_prefetch_related`:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    def get_select_related(self):
-        return ('other_model',)
-
-    other_field = serializers.SerializerMethodField()
-
-    def get_other_field(self, obj):
-        return obj.other_model.other_field
-
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-Note that because this is run before the queryset has been split into individual models, we cannot use object logic here. If you need a field for some models only, you can either fetch it for all of them, or fetch it for none of them.
-
-Sometimes, other serializers can be called in a `SerializerMethodField`. For this, you can either define `additional_serializers` like so:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    additional_serializers = (
-        {
-            'relation_and_field': 'other_model',
-            'serializer': OtherModelSerializer(),
-        },
-    )
-
-    other_field = serializers.SerializerMethodField()
-
-    def get_other_field(self, obj):
-        return OtherModelSerializer(obj.other_model, auto_prefetch=False)
-
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-Notice the part `auto_prefetch=False` in the `OtherModelSerializer` call. This is because drf-auto-prefetch uses parents to know if the serializer is at the higher-most level, so that the fetching is only done once. In this case however, the serializer has no parent, but the prefetching is already done by SomeSerializer, so we do not want to do it again. We can tell it to not prefetch by setting `auto_prefetch` to `False`.
-
-As for `select_related` and `prefetch_related`, you can define `get_additional_serializers` instead:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    def get_additional_serializers:
-        return (
-            {
-                'relation_and_field': 'other_model',
-                'serializer': OtherModelSerializer(),
-            },
-        )
-
-    other_field = serializers.SerializerMethodField()
-
-    def get_other_field(self, obj):
-        return OtherModelSerializer(obj.other_model, auto_prefetch=False)
-
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-This can be useful to avoid circular dependencies or to add some logic to the prefetching.
-
-## Special cases
-
-There are a few situations where you might want to be able to customize the behaviour more. Here are some of the ways you can tweak the Prefetching Serializer to fit the needs of your project.
-
-### Adding logic to the PrefetchingListSerializer
-
-If you had a ListSerializer for you Serializer, you will most likely want to keep its logic. This can be done by simply inheriting from `PrefetchingListSerializer` in that ListSerializer rather than inheriting from `serializers.ListSerializer`. Note that if you do not do this, but add the `PrefetchingSerializerMixin` to the main Serializer, you will get an error saying that the list_serializer_class must inherit from `PrefetchingListSerializer` to be used with the `PrefetchingSerializerMixin`. This is because the behaviour of the prefetching depends on it.
-
-### Adding compatibility with django-zen-queries or other libraries
-
-The goal of this library is to make it easy to not have to think about prefetching. However, this comes with the potential danger of not thinking enough about prefetching. To avoid discovering issues only once in production, you can add django-zen-queries in the mix. To do so, simply extend the `PrefetchingListSerializer` and `PrefetchingSerializerMixin` by defining a new mixin that will be inherited by both. In this mixin, you can override the `queryset_after_prefetch` and `call_to_representation` methods to add some behaviour right after the prefetching has been done on the queryset and right before or after calling `super().to_representation(instance)` on the serializer respectively. For django-zen-queries, it looks something like this:
-
-``` python
-from contextlib import nullcontext
-from django.conf import settings
-import serializer_prefetch
-from zen_queries import fetch, queries_disabled
-
-
-class ZenQueriesPrefetchingMixin:
-    def queryset_after_prefetch(self, queryset):
-        fetch(queryset)
-        return queryset
-
-    def call_to_representation(self, instance):
-        with queries_disabled() if settings.DEBUG else nullcontext():
-            return super().to_representation(instance)
-
-
-class PrefetchingListSerializer(
-    ZenQueriesPrefetchingMixin, 
-    serializer_prefetch.PrefetchingListSerializer
-):
-    pass
-
-
-class PrefetchingSerializerMixin(
-    ZenQueriesPrefetchingMixin,
-    serializer_prefetch.PrefetchingSerializerMixin
-):
-    default_list_serializer_class = PrefetchingListSerializer
-```
-
-The same logic can be applied to other libraries that could need to interact with the queryset between the time it is prefetched and the time it is split into models. Note that `queryset_after_prefetch` is only ever called if the instance passed to the ListSerializer is a Queryset, so you do not need to worry about checking for the type. Similarly, `call_to_representation` is only called if some prefetching was done. If none was done, either because it was not the furthermost parent or because auto_prefetch has been set to `False`, then this method will not be called. If you need a method to always be called, you can define a `to_representation` method in the new `PrefetchingListSerializer` you defined. Do not forget to call the super method!
-
-## Important note
-
-While the Prefetching Serializer does work on regular django-rest-framework serializers, it is really intended to be used with their `ModelSerializer`. If you do use it with a regular Serializer, you will need to define `select_related` and `prefetch_related` for all the fields used. Note that this is still better than having the logic in `get_queryset` in the viewset, as it is kept with its own serializer and will be used properly if the serializer is nested.
+Metadata-Version: 2.1
+Name: drf-serializer-prefetch
+Version: 1.1.0b1
+Summary: An automatic prefetcher for django-rest-framework.
+Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
+Author: Maxime Toussaint
+Author-email: m.toussaint@mail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![codecov](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch/branch/main/graph/badge.svg?token=MFI4E7L7SU)](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch)
+
+# drf-serializer-prefetch
+
+An automatic prefetcher that looks at the serializer fields and determines what needs to be prefetched accordingly.
+
+## Installation
+
+To install, call `pip install drf-serializer-prefetch`.
+
+## Usage
+
+In its most simple form, the serializer prefetch can be used by simply adding `PrefetchingSerializerMixin` to the class definition of the model serializer you want to allow automatic prefetching for like so:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+Using it like this, the Prefetching Serializer will be able to see what fields will be returned and prefetch them accordingly.
+
+However, SerializerMethodFields are an issue for the Prefetching Serializer, as those can make calls that are only done at run time. The Prefetching Serializer does not make any kind of file analysis, and as such cannot know what will happen in those methods. If you are calling a related model in that function, you can define either `select_related` or `prefetch_related` on the model. The fields defined here will also be taken into account. As for usual with Django, you can go as deep as you need here. For example, you could add `user`, or you could add `user__pizza_set`, if you were to loop over the user's pizzas.
+
+For example:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    select_related = ('other_model',)
+
+    other_field = serializers.SerializerMethodField()
+
+    def get_other_field(self, obj):
+        return obj.other_model.other_field
+
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+If you need to add some logic to when the prefetching should happen, you can also define `get_select_related` or `get_prefetch_related`:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    def get_select_related(self):
+        return ('other_model',)
+
+    other_field = serializers.SerializerMethodField()
+
+    def get_other_field(self, obj):
+        return obj.other_model.other_field
+
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+Note that because this is run before the queryset has been split into individual models, we cannot use object logic here. If you need a field for some models only, you can either fetch it for all of them, or fetch it for none of them.
+
+Sometimes, other serializers can be called in a `SerializerMethodField`. For this, you can either define `additional_serializers` like so:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    additional_serializers = (
+        {
+            'relation_and_field': 'other_model',
+            'serializer': OtherModelSerializer(),
+        },
+    )
+
+    other_field = serializers.SerializerMethodField()
+
+    def get_other_field(self, obj):
+        return OtherModelSerializer(obj.other_model, auto_prefetch=False)
+
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+Notice the part `auto_prefetch=False` in the `OtherModelSerializer` call. This is because drf-auto-prefetch uses parents to know if the serializer is at the higher-most level, so that the fetching is only done once. In this case however, the serializer has no parent, but the prefetching is already done by SomeSerializer, so we do not want to do it again. We can tell it to not prefetch by setting `auto_prefetch` to `False`.
+
+As for `select_related` and `prefetch_related`, you can define `get_additional_serializers` instead:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    def get_additional_serializers:
+        return (
+            {
+                'relation_and_field': 'other_model',
+                'serializer': OtherModelSerializer(),
+            },
+        )
+
+    other_field = serializers.SerializerMethodField()
+
+    def get_other_field(self, obj):
+        return OtherModelSerializer(obj.other_model, auto_prefetch=False)
+
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+This can be useful to avoid circular dependencies or to add some logic to the prefetching.
+
+## Special cases
+
+There are a few situations where you might want to be able to customize the behaviour more. Here are some of the ways you can tweak the Prefetching Serializer to fit the needs of your project.
+
+### Adding logic to the PrefetchingListSerializer
+
+If you had a ListSerializer for you Serializer, you will most likely want to keep its logic. This can be done by simply inheriting from `PrefetchingListSerializer` in that ListSerializer rather than inheriting from `serializers.ListSerializer`. Note that if you do not do this, but add the `PrefetchingSerializerMixin` to the main Serializer, you will get an error saying that the list_serializer_class must inherit from `PrefetchingListSerializer` to be used with the `PrefetchingSerializerMixin`. This is because the behaviour of the prefetching depends on it.
+
+### Adding compatibility with django-zen-queries or other libraries
+
+The goal of this library is to make it easy to not have to think about prefetching. However, this comes with the potential danger of not thinking enough about prefetching. To avoid discovering issues only once in production, you can add django-zen-queries in the mix. To do so, simply extend the `PrefetchingListSerializer` and `PrefetchingSerializerMixin` by defining a new mixin that will be inherited by both. In this mixin, you can override the `queryset_after_prefetch` and `call_to_representation` methods to add some behaviour right after the prefetching has been done on the queryset and right before or after calling `super().to_representation(instance)` on the serializer respectively. For django-zen-queries, it looks something like this:
+
+``` python
+from contextlib import nullcontext
+from django.conf import settings
+import serializer_prefetch
+from zen_queries import fetch, queries_disabled
+
+
+class ZenQueriesPrefetchingMixin:
+    def queryset_after_prefetch(self, queryset):
+        fetch(queryset)
+        return queryset
+
+    def call_to_representation(self, instance):
+        with queries_disabled() if settings.DEBUG else nullcontext():
+            return super().to_representation(instance)
+
+
+class PrefetchingListSerializer(
+    ZenQueriesPrefetchingMixin, 
+    serializer_prefetch.PrefetchingListSerializer
+):
+    pass
+
+
+class PrefetchingSerializerMixin(
+    ZenQueriesPrefetchingMixin,
+    serializer_prefetch.PrefetchingSerializerMixin
+):
+    default_list_serializer_class = PrefetchingListSerializer
+```
+
+The same logic can be applied to other libraries that could need to interact with the queryset between the time it is prefetched and the time it is split into models. Note that `queryset_after_prefetch` is only ever called if the instance passed to the ListSerializer is a Queryset, so you do not need to worry about checking for the type. Similarly, `call_to_representation` is only called if some prefetching was done. If none was done, either because it was not the furthermost parent or because auto_prefetch has been set to `False`, then this method will not be called. If you need a method to always be called, you can define a `to_representation` method in the new `PrefetchingListSerializer` you defined. Do not forget to call the super method!
+
+## Important note
+
+While the Prefetching Serializer does work on regular django-rest-framework serializers, it is really intended to be used with their `ModelSerializer`. If you do use it with a regular Serializer, you will need to define `select_related` and `prefetch_related` for all the fields used. Note that this is still better than having the logic in `get_queryset` in the viewset, as it is kept with its own serializer and will be used properly if the serializer is nested.
```

### Comparing `drf-serializer-prefetch-1.1.0b0/README.md` & `drf-serializer-prefetch-1.1.0b1/drf_serializer_prefetch.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,200 +1,210 @@
-[![codecov](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch/branch/main/graph/badge.svg?token=MFI4E7L7SU)](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch)
-
-# drf-serializer-prefetch
-
-An automatic prefetcher that looks at the serializer fields and determines what needs to be prefetched accordingly.
-
-## Installation
-
-To install, call `pip install drf-serializer-prefetch`.
-
-## Usage
-
-In its most simple form, the serializer prefetch can be used by simply adding `PrefetchingSerializerMixin` to the class definition of the model serializer you want to allow automatic prefetching for like so:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-Using it like this, the Prefetching Serializer will be able to see what fields will be returned and prefetch them accordingly.
-
-However, SerializerMethodFields are an issue for the Prefetching Serializer, as those can make calls that are only done at run time. The Prefetching Serializer does not make any kind of file analysis, and as such cannot know what will happen in those methods. If you are calling a related model in that function, you can define either `select_related` or `prefetch_related` on the model. The fields defined here will also be taken into account. As for usual with Django, you can go as deep as you need here. For example, you could add `user`, or you could add `user__pizza_set`, if you were to loop over the user's pizzas.
-
-For example:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    select_related = ('other_model',)
-
-    other_field = serializers.SerializerMethodField()
-
-    def get_other_field(self, obj):
-        return obj.other_model.other_field
-
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-If you need to add some logic to when the prefetching should happen, you can also define `get_select_related` or `get_prefetch_related`:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    def get_select_related(self):
-        return ('other_model',)
-
-    other_field = serializers.SerializerMethodField()
-
-    def get_other_field(self, obj):
-        return obj.other_model.other_field
-
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-Note that because this is run before the queryset has been split into individual models, we cannot use object logic here. If you need a field for some models only, you can either fetch it for all of them, or fetch it for none of them.
-
-Sometimes, other serializers can be called in a `SerializerMethodField`. For this, you can either define `additional_serializers` like so:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    additional_serializers = (
-        {
-            'relation_and_field': 'other_model',
-            'serializer': OtherModelSerializer(),
-        },
-    )
-
-    other_field = serializers.SerializerMethodField()
-
-    def get_other_field(self, obj):
-        return OtherModelSerializer(obj.other_model, auto_prefetch=False)
-
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-Notice the part `auto_prefetch=False` in the `OtherModelSerializer` call. This is because drf-auto-prefetch uses parents to know if the serializer is at the higher-most level, so that the fetching is only done once. In this case however, the serializer has no parent, but the prefetching is already done by SomeSerializer, so we do not want to do it again. We can tell it to not prefetch by setting `auto_prefetch` to `False`.
-
-As for `select_related` and `prefetch_related`, you can define `get_additional_serializers` instead:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    def get_additional_serializers:
-        return (
-            {
-                'relation_and_field': 'other_model',
-                'serializer': OtherModelSerializer(),
-            },
-        )
-
-    other_field = serializers.SerializerMethodField()
-
-    def get_other_field(self, obj):
-        return OtherModelSerializer(obj.other_model, auto_prefetch=False)
-
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-This can be useful to avoid circular dependencies or to add some logic to the prefetching.
-
-## Special cases
-
-There are a few situations where you might want to be able to customize the behaviour more. Here are some of the ways you can tweak the Prefetching Serializer to fit the needs of your project.
-
-### Adding logic to the PrefetchingListSerializer
-
-If you had a ListSerializer for you Serializer, you will most likely want to keep its logic. This can be done by simply inheriting from `PrefetchingListSerializer` in that ListSerializer rather than inheriting from `serializers.ListSerializer`. Note that if you do not do this, but add the `PrefetchingSerializerMixin` to the main Serializer, you will get an error saying that the list_serializer_class must inherit from `PrefetchingListSerializer` to be used with the `PrefetchingSerializerMixin`. This is because the behaviour of the prefetching depends on it.
-
-### Adding compatibility with django-zen-queries or other libraries
-
-The goal of this library is to make it easy to not have to think about prefetching. However, this comes with the potential danger of not thinking enough about prefetching. To avoid discovering issues only once in production, you can add django-zen-queries in the mix. To do so, simply extend the `PrefetchingListSerializer` and `PrefetchingSerializerMixin` by defining a new mixin that will be inherited by both. In this mixin, you can override the `queryset_after_prefetch` and `call_to_representation` methods to add some behaviour right after the prefetching has been done on the queryset and right before or after calling `super().to_representation(instance)` on the serializer respectively. For django-zen-queries, it looks something like this:
-
-``` python
-from contextlib import nullcontext
-from django.conf import settings
-import serializer_prefetch
-from zen_queries import fetch, queries_disabled
-
-
-class ZenQueriesPrefetchingMixin:
-    def queryset_after_prefetch(self, queryset):
-        fetch(queryset)
-        return queryset
-
-    def call_to_representation(self, instance):
-        with queries_disabled() if settings.DEBUG else nullcontext():
-            return super().to_representation(instance)
-
-
-class PrefetchingListSerializer(
-    ZenQueriesPrefetchingMixin, 
-    serializer_prefetch.PrefetchingListSerializer
-):
-    pass
-
-
-class PrefetchingSerializerMixin(
-    ZenQueriesPrefetchingMixin,
-    serializer_prefetch.PrefetchingSerializerMixin
-):
-    default_list_serializer_class = PrefetchingListSerializer
-```
-
-The same logic can be applied to other libraries that could need to interact with the queryset between the time it is prefetched and the time it is split into models. Note that `queryset_after_prefetch` is only ever called if the instance passed to the ListSerializer is a Queryset, so you do not need to worry about checking for the type. Similarly, `call_to_representation` is only called if some prefetching was done. If none was done, either because it was not the furthermost parent or because auto_prefetch has been set to `False`, then this method will not be called. If you need a method to always be called, you can define a `to_representation` method in the new `PrefetchingListSerializer` you defined. Do not forget to call the super method!
-
-## Important note
-
-While the Prefetching Serializer does work on regular django-rest-framework serializers, it is really intended to be used with their `ModelSerializer`. If you do use it with a regular Serializer, you will need to define `select_related` and `prefetch_related` for all the fields used. Note that this is still better than having the logic in `get_queryset` in the viewset, as it is kept with its own serializer and will be used properly if the serializer is nested.
+Metadata-Version: 2.1
+Name: drf-serializer-prefetch
+Version: 1.1.0b1
+Summary: An automatic prefetcher for django-rest-framework.
+Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
+Author: Maxime Toussaint
+Author-email: m.toussaint@mail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![codecov](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch/branch/main/graph/badge.svg?token=MFI4E7L7SU)](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch)
+
+# drf-serializer-prefetch
+
+An automatic prefetcher that looks at the serializer fields and determines what needs to be prefetched accordingly.
+
+## Installation
+
+To install, call `pip install drf-serializer-prefetch`.
+
+## Usage
+
+In its most simple form, the serializer prefetch can be used by simply adding `PrefetchingSerializerMixin` to the class definition of the model serializer you want to allow automatic prefetching for like so:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+Using it like this, the Prefetching Serializer will be able to see what fields will be returned and prefetch them accordingly.
+
+However, SerializerMethodFields are an issue for the Prefetching Serializer, as those can make calls that are only done at run time. The Prefetching Serializer does not make any kind of file analysis, and as such cannot know what will happen in those methods. If you are calling a related model in that function, you can define either `select_related` or `prefetch_related` on the model. The fields defined here will also be taken into account. As for usual with Django, you can go as deep as you need here. For example, you could add `user`, or you could add `user__pizza_set`, if you were to loop over the user's pizzas.
+
+For example:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    select_related = ('other_model',)
+
+    other_field = serializers.SerializerMethodField()
+
+    def get_other_field(self, obj):
+        return obj.other_model.other_field
+
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+If you need to add some logic to when the prefetching should happen, you can also define `get_select_related` or `get_prefetch_related`:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    def get_select_related(self):
+        return ('other_model',)
+
+    other_field = serializers.SerializerMethodField()
+
+    def get_other_field(self, obj):
+        return obj.other_model.other_field
+
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+Note that because this is run before the queryset has been split into individual models, we cannot use object logic here. If you need a field for some models only, you can either fetch it for all of them, or fetch it for none of them.
+
+Sometimes, other serializers can be called in a `SerializerMethodField`. For this, you can either define `additional_serializers` like so:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    additional_serializers = (
+        {
+            'relation_and_field': 'other_model',
+            'serializer': OtherModelSerializer(),
+        },
+    )
+
+    other_field = serializers.SerializerMethodField()
+
+    def get_other_field(self, obj):
+        return OtherModelSerializer(obj.other_model, auto_prefetch=False)
+
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+Notice the part `auto_prefetch=False` in the `OtherModelSerializer` call. This is because drf-auto-prefetch uses parents to know if the serializer is at the higher-most level, so that the fetching is only done once. In this case however, the serializer has no parent, but the prefetching is already done by SomeSerializer, so we do not want to do it again. We can tell it to not prefetch by setting `auto_prefetch` to `False`.
+
+As for `select_related` and `prefetch_related`, you can define `get_additional_serializers` instead:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    def get_additional_serializers:
+        return (
+            {
+                'relation_and_field': 'other_model',
+                'serializer': OtherModelSerializer(),
+            },
+        )
+
+    other_field = serializers.SerializerMethodField()
+
+    def get_other_field(self, obj):
+        return OtherModelSerializer(obj.other_model, auto_prefetch=False)
+
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+This can be useful to avoid circular dependencies or to add some logic to the prefetching.
+
+## Special cases
+
+There are a few situations where you might want to be able to customize the behaviour more. Here are some of the ways you can tweak the Prefetching Serializer to fit the needs of your project.
+
+### Adding logic to the PrefetchingListSerializer
+
+If you had a ListSerializer for you Serializer, you will most likely want to keep its logic. This can be done by simply inheriting from `PrefetchingListSerializer` in that ListSerializer rather than inheriting from `serializers.ListSerializer`. Note that if you do not do this, but add the `PrefetchingSerializerMixin` to the main Serializer, you will get an error saying that the list_serializer_class must inherit from `PrefetchingListSerializer` to be used with the `PrefetchingSerializerMixin`. This is because the behaviour of the prefetching depends on it.
+
+### Adding compatibility with django-zen-queries or other libraries
+
+The goal of this library is to make it easy to not have to think about prefetching. However, this comes with the potential danger of not thinking enough about prefetching. To avoid discovering issues only once in production, you can add django-zen-queries in the mix. To do so, simply extend the `PrefetchingListSerializer` and `PrefetchingSerializerMixin` by defining a new mixin that will be inherited by both. In this mixin, you can override the `queryset_after_prefetch` and `call_to_representation` methods to add some behaviour right after the prefetching has been done on the queryset and right before or after calling `super().to_representation(instance)` on the serializer respectively. For django-zen-queries, it looks something like this:
+
+``` python
+from contextlib import nullcontext
+from django.conf import settings
+import serializer_prefetch
+from zen_queries import fetch, queries_disabled
+
+
+class ZenQueriesPrefetchingMixin:
+    def queryset_after_prefetch(self, queryset):
+        fetch(queryset)
+        return queryset
+
+    def call_to_representation(self, instance):
+        with queries_disabled() if settings.DEBUG else nullcontext():
+            return super().to_representation(instance)
+
+
+class PrefetchingListSerializer(
+    ZenQueriesPrefetchingMixin, 
+    serializer_prefetch.PrefetchingListSerializer
+):
+    pass
+
+
+class PrefetchingSerializerMixin(
+    ZenQueriesPrefetchingMixin,
+    serializer_prefetch.PrefetchingSerializerMixin
+):
+    default_list_serializer_class = PrefetchingListSerializer
+```
+
+The same logic can be applied to other libraries that could need to interact with the queryset between the time it is prefetched and the time it is split into models. Note that `queryset_after_prefetch` is only ever called if the instance passed to the ListSerializer is a Queryset, so you do not need to worry about checking for the type. Similarly, `call_to_representation` is only called if some prefetching was done. If none was done, either because it was not the furthermost parent or because auto_prefetch has been set to `False`, then this method will not be called. If you need a method to always be called, you can define a `to_representation` method in the new `PrefetchingListSerializer` you defined. Do not forget to call the super method!
+
+## Important note
+
+While the Prefetching Serializer does work on regular django-rest-framework serializers, it is really intended to be used with their `ModelSerializer`. If you do use it with a regular Serializer, you will need to define `select_related` and `prefetch_related` for all the fields used. Note that this is still better than having the logic in `get_queryset` in the viewset, as it is kept with its own serializer and will be used properly if the serializer is nested.
```

### Comparing `drf-serializer-prefetch-1.1.0b0/drf_serializer_prefetch.egg-info/PKG-INFO` & `drf-serializer-prefetch-1.1.0b1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,210 +1,200 @@
-Metadata-Version: 2.1
-Name: drf-serializer-prefetch
-Version: 1.1.0b0
-Summary: An automatic prefetcher for django-rest-framework.
-Home-page: https://github.com/MaxDude132/drf-serializer-prefetch
-Author: Maxime Toussaint
-Author-email: m.toussaint@mail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![codecov](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch/branch/main/graph/badge.svg?token=MFI4E7L7SU)](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch)
-
-# drf-serializer-prefetch
-
-An automatic prefetcher that looks at the serializer fields and determines what needs to be prefetched accordingly.
-
-## Installation
-
-To install, call `pip install drf-serializer-prefetch`.
-
-## Usage
-
-In its most simple form, the serializer prefetch can be used by simply adding `PrefetchingSerializerMixin` to the class definition of the model serializer you want to allow automatic prefetching for like so:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-Using it like this, the Prefetching Serializer will be able to see what fields will be returned and prefetch them accordingly.
-
-However, SerializerMethodFields are an issue for the Prefetching Serializer, as those can make calls that are only done at run time. The Prefetching Serializer does not make any kind of file analysis, and as such cannot know what will happen in those methods. If you are calling a related model in that function, you can define either `select_related` or `prefetch_related` on the model. The fields defined here will also be taken into account. As for usual with Django, you can go as deep as you need here. For example, you could add `user`, or you could add `user__pizza_set`, if you were to loop over the user's pizzas.
-
-For example:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    select_related = ('other_model',)
-
-    other_field = serializers.SerializerMethodField()
-
-    def get_other_field(self, obj):
-        return obj.other_model.other_field
-
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-If you need to add some logic to when the prefetching should happen, you can also define `get_select_related` or `get_prefetch_related`:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    def get_select_related(self):
-        return ('other_model',)
-
-    other_field = serializers.SerializerMethodField()
-
-    def get_other_field(self, obj):
-        return obj.other_model.other_field
-
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-Note that because this is run before the queryset has been split into individual models, we cannot use object logic here. If you need a field for some models only, you can either fetch it for all of them, or fetch it for none of them.
-
-Sometimes, other serializers can be called in a `SerializerMethodField`. For this, you can either define `additional_serializers` like so:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    additional_serializers = (
-        {
-            'relation_and_field': 'other_model',
-            'serializer': OtherModelSerializer(),
-        },
-    )
-
-    other_field = serializers.SerializerMethodField()
-
-    def get_other_field(self, obj):
-        return OtherModelSerializer(obj.other_model, auto_prefetch=False)
-
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-Notice the part `auto_prefetch=False` in the `OtherModelSerializer` call. This is because drf-auto-prefetch uses parents to know if the serializer is at the higher-most level, so that the fetching is only done once. In this case however, the serializer has no parent, but the prefetching is already done by SomeSerializer, so we do not want to do it again. We can tell it to not prefetch by setting `auto_prefetch` to `False`.
-
-As for `select_related` and `prefetch_related`, you can define `get_additional_serializers` instead:
-
-``` python
-from rest_framework import serializers
-from serializer_prefetch import PrefetchingSerializerMixin
-
-
-class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
-    def get_additional_serializers:
-        return (
-            {
-                'relation_and_field': 'other_model',
-                'serializer': OtherModelSerializer(),
-            },
-        )
-
-    other_field = serializers.SerializerMethodField()
-
-    def get_other_field(self, obj):
-        return OtherModelSerializer(obj.other_model, auto_prefetch=False)
-
-    class Meta:
-        model = SomeModel
-        fields = (
-            'some',
-            'fields',
-            'are',
-            'defined',
-        )
-```
-
-This can be useful to avoid circular dependencies or to add some logic to the prefetching.
-
-## Special cases
-
-There are a few situations where you might want to be able to customize the behaviour more. Here are some of the ways you can tweak the Prefetching Serializer to fit the needs of your project.
-
-### Adding logic to the PrefetchingListSerializer
-
-If you had a ListSerializer for you Serializer, you will most likely want to keep its logic. This can be done by simply inheriting from `PrefetchingListSerializer` in that ListSerializer rather than inheriting from `serializers.ListSerializer`. Note that if you do not do this, but add the `PrefetchingSerializerMixin` to the main Serializer, you will get an error saying that the list_serializer_class must inherit from `PrefetchingListSerializer` to be used with the `PrefetchingSerializerMixin`. This is because the behaviour of the prefetching depends on it.
-
-### Adding compatibility with django-zen-queries or other libraries
-
-The goal of this library is to make it easy to not have to think about prefetching. However, this comes with the potential danger of not thinking enough about prefetching. To avoid discovering issues only once in production, you can add django-zen-queries in the mix. To do so, simply extend the `PrefetchingListSerializer` and `PrefetchingSerializerMixin` by defining a new mixin that will be inherited by both. In this mixin, you can override the `queryset_after_prefetch` and `call_to_representation` methods to add some behaviour right after the prefetching has been done on the queryset and right before or after calling `super().to_representation(instance)` on the serializer respectively. For django-zen-queries, it looks something like this:
-
-``` python
-from contextlib import nullcontext
-from django.conf import settings
-import serializer_prefetch
-from zen_queries import fetch, queries_disabled
-
-
-class ZenQueriesPrefetchingMixin:
-    def queryset_after_prefetch(self, queryset):
-        fetch(queryset)
-        return queryset
-
-    def call_to_representation(self, instance):
-        with queries_disabled() if settings.DEBUG else nullcontext():
-            return super().to_representation(instance)
-
-
-class PrefetchingListSerializer(
-    ZenQueriesPrefetchingMixin, 
-    serializer_prefetch.PrefetchingListSerializer
-):
-    pass
-
-
-class PrefetchingSerializerMixin(
-    ZenQueriesPrefetchingMixin,
-    serializer_prefetch.PrefetchingSerializerMixin
-):
-    default_list_serializer_class = PrefetchingListSerializer
-```
-
-The same logic can be applied to other libraries that could need to interact with the queryset between the time it is prefetched and the time it is split into models. Note that `queryset_after_prefetch` is only ever called if the instance passed to the ListSerializer is a Queryset, so you do not need to worry about checking for the type. Similarly, `call_to_representation` is only called if some prefetching was done. If none was done, either because it was not the furthermost parent or because auto_prefetch has been set to `False`, then this method will not be called. If you need a method to always be called, you can define a `to_representation` method in the new `PrefetchingListSerializer` you defined. Do not forget to call the super method!
-
-## Important note
-
-While the Prefetching Serializer does work on regular django-rest-framework serializers, it is really intended to be used with their `ModelSerializer`. If you do use it with a regular Serializer, you will need to define `select_related` and `prefetch_related` for all the fields used. Note that this is still better than having the logic in `get_queryset` in the viewset, as it is kept with its own serializer and will be used properly if the serializer is nested.
+[![codecov](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch/branch/main/graph/badge.svg?token=MFI4E7L7SU)](https://codecov.io/gh/MaxDude132/drf-serializer-prefetch)
+
+# drf-serializer-prefetch
+
+An automatic prefetcher that looks at the serializer fields and determines what needs to be prefetched accordingly.
+
+## Installation
+
+To install, call `pip install drf-serializer-prefetch`.
+
+## Usage
+
+In its most simple form, the serializer prefetch can be used by simply adding `PrefetchingSerializerMixin` to the class definition of the model serializer you want to allow automatic prefetching for like so:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+Using it like this, the Prefetching Serializer will be able to see what fields will be returned and prefetch them accordingly.
+
+However, SerializerMethodFields are an issue for the Prefetching Serializer, as those can make calls that are only done at run time. The Prefetching Serializer does not make any kind of file analysis, and as such cannot know what will happen in those methods. If you are calling a related model in that function, you can define either `select_related` or `prefetch_related` on the model. The fields defined here will also be taken into account. As for usual with Django, you can go as deep as you need here. For example, you could add `user`, or you could add `user__pizza_set`, if you were to loop over the user's pizzas.
+
+For example:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    select_related = ('other_model',)
+
+    other_field = serializers.SerializerMethodField()
+
+    def get_other_field(self, obj):
+        return obj.other_model.other_field
+
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+If you need to add some logic to when the prefetching should happen, you can also define `get_select_related` or `get_prefetch_related`:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    def get_select_related(self):
+        return ('other_model',)
+
+    other_field = serializers.SerializerMethodField()
+
+    def get_other_field(self, obj):
+        return obj.other_model.other_field
+
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+Note that because this is run before the queryset has been split into individual models, we cannot use object logic here. If you need a field for some models only, you can either fetch it for all of them, or fetch it for none of them.
+
+Sometimes, other serializers can be called in a `SerializerMethodField`. For this, you can either define `additional_serializers` like so:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    additional_serializers = (
+        {
+            'relation_and_field': 'other_model',
+            'serializer': OtherModelSerializer(),
+        },
+    )
+
+    other_field = serializers.SerializerMethodField()
+
+    def get_other_field(self, obj):
+        return OtherModelSerializer(obj.other_model, auto_prefetch=False)
+
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+Notice the part `auto_prefetch=False` in the `OtherModelSerializer` call. This is because drf-auto-prefetch uses parents to know if the serializer is at the higher-most level, so that the fetching is only done once. In this case however, the serializer has no parent, but the prefetching is already done by SomeSerializer, so we do not want to do it again. We can tell it to not prefetch by setting `auto_prefetch` to `False`.
+
+As for `select_related` and `prefetch_related`, you can define `get_additional_serializers` instead:
+
+``` python
+from rest_framework import serializers
+from serializer_prefetch import PrefetchingSerializerMixin
+
+
+class SomeSerializer(PrefetchingSerializerMixin, serializer.ModelSerializer):
+    def get_additional_serializers:
+        return (
+            {
+                'relation_and_field': 'other_model',
+                'serializer': OtherModelSerializer(),
+            },
+        )
+
+    other_field = serializers.SerializerMethodField()
+
+    def get_other_field(self, obj):
+        return OtherModelSerializer(obj.other_model, auto_prefetch=False)
+
+    class Meta:
+        model = SomeModel
+        fields = (
+            'some',
+            'fields',
+            'are',
+            'defined',
+        )
+```
+
+This can be useful to avoid circular dependencies or to add some logic to the prefetching.
+
+## Special cases
+
+There are a few situations where you might want to be able to customize the behaviour more. Here are some of the ways you can tweak the Prefetching Serializer to fit the needs of your project.
+
+### Adding logic to the PrefetchingListSerializer
+
+If you had a ListSerializer for you Serializer, you will most likely want to keep its logic. This can be done by simply inheriting from `PrefetchingListSerializer` in that ListSerializer rather than inheriting from `serializers.ListSerializer`. Note that if you do not do this, but add the `PrefetchingSerializerMixin` to the main Serializer, you will get an error saying that the list_serializer_class must inherit from `PrefetchingListSerializer` to be used with the `PrefetchingSerializerMixin`. This is because the behaviour of the prefetching depends on it.
+
+### Adding compatibility with django-zen-queries or other libraries
+
+The goal of this library is to make it easy to not have to think about prefetching. However, this comes with the potential danger of not thinking enough about prefetching. To avoid discovering issues only once in production, you can add django-zen-queries in the mix. To do so, simply extend the `PrefetchingListSerializer` and `PrefetchingSerializerMixin` by defining a new mixin that will be inherited by both. In this mixin, you can override the `queryset_after_prefetch` and `call_to_representation` methods to add some behaviour right after the prefetching has been done on the queryset and right before or after calling `super().to_representation(instance)` on the serializer respectively. For django-zen-queries, it looks something like this:
+
+``` python
+from contextlib import nullcontext
+from django.conf import settings
+import serializer_prefetch
+from zen_queries import fetch, queries_disabled
+
+
+class ZenQueriesPrefetchingMixin:
+    def queryset_after_prefetch(self, queryset):
+        fetch(queryset)
+        return queryset
+
+    def call_to_representation(self, instance):
+        with queries_disabled() if settings.DEBUG else nullcontext():
+            return super().to_representation(instance)
+
+
+class PrefetchingListSerializer(
+    ZenQueriesPrefetchingMixin, 
+    serializer_prefetch.PrefetchingListSerializer
+):
+    pass
+
+
+class PrefetchingSerializerMixin(
+    ZenQueriesPrefetchingMixin,
+    serializer_prefetch.PrefetchingSerializerMixin
+):
+    default_list_serializer_class = PrefetchingListSerializer
+```
+
+The same logic can be applied to other libraries that could need to interact with the queryset between the time it is prefetched and the time it is split into models. Note that `queryset_after_prefetch` is only ever called if the instance passed to the ListSerializer is a Queryset, so you do not need to worry about checking for the type. Similarly, `call_to_representation` is only called if some prefetching was done. If none was done, either because it was not the furthermost parent or because auto_prefetch has been set to `False`, then this method will not be called. If you need a method to always be called, you can define a `to_representation` method in the new `PrefetchingListSerializer` you defined. Do not forget to call the super method!
+
+## Important note
+
+While the Prefetching Serializer does work on regular django-rest-framework serializers, it is really intended to be used with their `ModelSerializer`. If you do use it with a regular Serializer, you will need to define `select_related` and `prefetch_related` for all the fields used. Note that this is still better than having the logic in `get_queryset` in the viewset, as it is kept with its own serializer and will be used properly if the serializer is nested.
```

### Comparing `drf-serializer-prefetch-1.1.0b0/setup.py` & `drf-serializer-prefetch-1.1.0b1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from pathlib import Path
-from setuptools import setup, find_packages
-
-
-VERSION = "1.1.0b"
-DESCRIPTION = "An automatic prefetcher for django-rest-framework."
-this_directory = Path(__file__).parent
-LONG_DESCRIPTION = (this_directory / "README.md").read_text()
-
-setup(
-    name="drf-serializer-prefetch",
-    version=VERSION,
-    author="Maxime Toussaint",
-    author_email="m.toussaint@mail.com",
-    description=DESCRIPTION,
-    long_description=LONG_DESCRIPTION,
-    long_description_content_type="text/markdown",
-    packages=find_packages(),
-    install_requires=("django>=3.2.0", "djangorestframework>=3.12"),
-    url="https://github.com/MaxDude132/drf-serializer-prefetch",
-)
+from pathlib import Path
+from setuptools import setup, find_packages
+
+
+VERSION = "1.1.0b1"
+DESCRIPTION = "An automatic prefetcher for django-rest-framework."
+this_directory = Path(__file__).parent
+LONG_DESCRIPTION = (this_directory / "README.md").read_text()
+
+setup(
+    name="drf-serializer-prefetch",
+    version=VERSION,
+    author="Maxime Toussaint",
+    author_email="m.toussaint@mail.com",
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    long_description_content_type="text/markdown",
+    packages=find_packages(),
+    install_requires=("django>=3.2.0", "djangorestframework>=3.12"),
+    url="https://github.com/MaxDude132/drf-serializer-prefetch",
+)
```

### Comparing `drf-serializer-prefetch-1.1.0b0/tests/models.py` & `drf-serializer-prefetch-1.1.0b1/tests/models.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from django.db import models
-
-
-class Continent(models.Model):
-    label = models.CharField(max_length=50)
-
-
-class Country(models.Model):
-    label = models.CharField(max_length=50)
-    continent = models.ForeignKey(Continent, on_delete=models.CASCADE, null=True)
-
-
-class Pizza(models.Model):
-    label = models.CharField(max_length=50)
-    provenance = models.ForeignKey(Country, on_delete=models.CASCADE)
-
-
-class Topping(models.Model):
-    pizza = models.ForeignKey(Pizza, on_delete=models.CASCADE, related_name="toppings")
-    label = models.CharField(max_length=50)
-    origin = models.ForeignKey(
-        Country, on_delete=models.CASCADE, related_name="toppings"
-    )
+from django.db import models
+
+
+class Continent(models.Model):
+    label = models.CharField(max_length=50)
+
+
+class Country(models.Model):
+    label = models.CharField(max_length=50)
+    continent = models.ForeignKey(Continent, on_delete=models.CASCADE, null=True)
+
+
+class Pizza(models.Model):
+    label = models.CharField(max_length=50)
+    provenance = models.ForeignKey(Country, on_delete=models.CASCADE)
+
+
+class Topping(models.Model):
+    pizza = models.ForeignKey(Pizza, on_delete=models.CASCADE, related_name="toppings")
+    label = models.CharField(max_length=50)
+    origin = models.ForeignKey(
+        Country, on_delete=models.CASCADE, related_name="toppings"
+    )
```

### Comparing `drf-serializer-prefetch-1.1.0b0/tests/serializers.py` & `drf-serializer-prefetch-1.1.0b1/tests/serializers.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from rest_framework import serializers
-
-from serializer_prefetch import PrefetchingSerializerMixin
-
-from tests.models import Pizza, Topping, Country
-
-
-class ToppingSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-    class Meta:
-        model = Topping
-        fields = ("label",)
-
-
-class CountrySerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-    class Meta:
-        model = Country
-        fields = ("label",)
-
-
-class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-    toppings = ToppingSerializer(many=True)
-    provenance = CountrySerializer()
-
-    class Meta:
-        model = Pizza
-        fields = ("label", "toppings", "provenance")
+from rest_framework import serializers
+
+from serializer_prefetch import PrefetchingSerializerMixin
+
+from tests.models import Pizza, Topping, Country
+
+
+class ToppingSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+    class Meta:
+        model = Topping
+        fields = ("label",)
+
+
+class CountrySerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+    class Meta:
+        model = Country
+        fields = ("label",)
+
+
+class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+    toppings = ToppingSerializer(many=True)
+    provenance = CountrySerializer()
+
+    class Meta:
+        model = Pizza
+        fields = ("label", "toppings", "provenance")
```

### Comparing `drf-serializer-prefetch-1.1.0b0/tests/test_conditions.py` & `drf-serializer-prefetch-1.1.0b1/tests/test_conditions.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-from django.test import TestCase
-
-from rest_framework import serializers
-
-from serializer_prefetch import PrefetchingSerializerMixin
-
-from tests.models import Pizza, Topping, Country
-from tests.serializers import PizzaSerializer, ToppingSerializer
-
-
-class ConditionsTestCase(TestCase):
-    @classmethod
-    def setUpTestData(cls) -> None:
-        cls.canada = Country.objects.create(label="Canada")
-        cls.usa = Country.objects.create(label="USA")
-        cls.china = Country.objects.create(label="China")
-        cls.argentina = Country.objects.create(label="Argentina")
-
-        cls.hawaian_pizza = Pizza.objects.create(
-            label="Hawaiian", provenance=cls.canada
-        )
-        cls.ham_topping = Topping.objects.create(
-            pizza=cls.hawaian_pizza, label="Ham", origin=cls.china
-        )
-        cls.pineapple_topping = Topping.objects.create(
-            pizza=cls.hawaian_pizza, label="Pineapple", origin=cls.argentina
-        )
-
-        cls.pepperoni_pizza = Pizza.objects.create(
-            label="Pepperoni", provenance=cls.usa
-        )
-        cls.pepperoni_topping = Topping.objects.create(
-            pizza=cls.pepperoni_pizza, label="Pepperoni", origin=cls.usa
-        )
-
-    def test_with_write_only_field(self):
-        global PizzaSerializer
-
-        class PizzaSerializer(PizzaSerializer):
-            toppings = ToppingSerializer(many=True, write_only=True)
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(1):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "provenance": {"label": "Canada"},
-                },
-                {
-                    "label": "Pepperoni",
-                    "provenance": {"label": "USA"},
-                },
-            ],
-        )
-
-    def test_list_is_passed(self):
-        pizzas = list(Pizza.objects.all())
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(2):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [{"label": "Ham"}, {"label": "Pineapple"}],
-                    "provenance": {"label": "Canada"},
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [{"label": "Pepperoni"}],
-                    "provenance": {"label": "USA"},
-                },
-            ],
-        )
-
-    def test_dict_is_passed(self):
-        pizza = Pizza.objects.first()
-        pizza = {
-            "label": pizza.label,
-            "toppings": [],
-            "provenance": {"label": pizza.provenance.label},
-        }
-        serializer = PizzaSerializer(pizza)
-
-        with self.assertNumQueries(0):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            {
-                "label": "Hawaiian",
-                "toppings": [],
-                "provenance": {"label": "Canada"},
-            },
-        )
-
-    def test_non_model_serializer(self):
-        class PizzaSerializer(PrefetchingSerializerMixin, serializers.Serializer):
-            toppings = ToppingSerializer(many=True)
-            label = serializers.CharField()
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        # Note: the regular Serializer cannot handle auto prefetching,
-        # it has to be done manually
-        with self.assertNumQueries(3):
-            serializer.data
-
-        class PizzaSerializer(PizzaSerializer):
-            additional_serializers = (
-                {"relation_and_field": "toppings", "serializer": ToppingSerializer()},
-            )
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(2):
-            serializer.data
+from django.test import TestCase
+
+from rest_framework import serializers
+
+from serializer_prefetch import PrefetchingSerializerMixin
+
+from tests.models import Pizza, Topping, Country
+from tests.serializers import PizzaSerializer, ToppingSerializer
+
+
+class ConditionsTestCase(TestCase):
+    @classmethod
+    def setUpTestData(cls) -> None:
+        cls.canada = Country.objects.create(label="Canada")
+        cls.usa = Country.objects.create(label="USA")
+        cls.china = Country.objects.create(label="China")
+        cls.argentina = Country.objects.create(label="Argentina")
+
+        cls.hawaian_pizza = Pizza.objects.create(
+            label="Hawaiian", provenance=cls.canada
+        )
+        cls.ham_topping = Topping.objects.create(
+            pizza=cls.hawaian_pizza, label="Ham", origin=cls.china
+        )
+        cls.pineapple_topping = Topping.objects.create(
+            pizza=cls.hawaian_pizza, label="Pineapple", origin=cls.argentina
+        )
+
+        cls.pepperoni_pizza = Pizza.objects.create(
+            label="Pepperoni", provenance=cls.usa
+        )
+        cls.pepperoni_topping = Topping.objects.create(
+            pizza=cls.pepperoni_pizza, label="Pepperoni", origin=cls.usa
+        )
+
+    def test_with_write_only_field(self):
+        global PizzaSerializer
+
+        class PizzaSerializer(PizzaSerializer):
+            toppings = ToppingSerializer(many=True, write_only=True)
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(1):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "provenance": {"label": "Canada"},
+                },
+                {
+                    "label": "Pepperoni",
+                    "provenance": {"label": "USA"},
+                },
+            ],
+        )
+
+    def test_list_is_passed(self):
+        pizzas = list(Pizza.objects.all())
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(2):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [{"label": "Ham"}, {"label": "Pineapple"}],
+                    "provenance": {"label": "Canada"},
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [{"label": "Pepperoni"}],
+                    "provenance": {"label": "USA"},
+                },
+            ],
+        )
+
+    def test_dict_is_passed(self):
+        pizza = Pizza.objects.first()
+        pizza = {
+            "label": pizza.label,
+            "toppings": [],
+            "provenance": {"label": pizza.provenance.label},
+        }
+        serializer = PizzaSerializer(pizza)
+
+        with self.assertNumQueries(0):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            {
+                "label": "Hawaiian",
+                "toppings": [],
+                "provenance": {"label": "Canada"},
+            },
+        )
+
+    def test_non_model_serializer(self):
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.Serializer):
+            toppings = ToppingSerializer(many=True)
+            label = serializers.CharField()
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        # Note: the regular Serializer cannot handle auto prefetching,
+        # it has to be done manually
+        with self.assertNumQueries(3):
+            serializer.data
+
+        class PizzaSerializer(PizzaSerializer):
+            additional_serializers = (
+                {"relation_and_field": "toppings", "serializer": ToppingSerializer()},
+            )
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(2):
+            serializer.data
```

### Comparing `drf-serializer-prefetch-1.1.0b0/tests/test_errors.py` & `drf-serializer-prefetch-1.1.0b1/tests/test_errors.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from django.test import TestCase
-
-from rest_framework import serializers
-
-from tests.models import Pizza, Topping, Country
-from tests.serializers import PizzaSerializer
-
-
-class ErrorsTestCase(TestCase):
-    @classmethod
-    def setUpTestData(cls) -> None:
-        cls.canada = Country.objects.create(label="Canada")
-        cls.usa = Country.objects.create(label="USA")
-        cls.china = Country.objects.create(label="China")
-        cls.argentina = Country.objects.create(label="Argentina")
-
-        cls.hawaian_pizza = Pizza.objects.create(
-            label="Hawaiian", provenance=cls.canada
-        )
-        cls.ham_topping = Topping.objects.create(
-            pizza=cls.hawaian_pizza, label="Ham", origin=cls.china
-        )
-        cls.pineapple_topping = Topping.objects.create(
-            pizza=cls.hawaian_pizza, label="Pineapple", origin=cls.argentina
-        )
-
-        cls.pepperoni_pizza = Pizza.objects.create(
-            label="Pepperoni", provenance=cls.usa
-        )
-        cls.pepperoni_topping = Topping.objects.create(
-            pizza=cls.pepperoni_pizza, label="Pepperoni", origin=cls.usa
-        )
-
-    def test_value_error_if_serializer_not_in_additional_serializer_data(self):
-        class LocalPizzaSerializer(PizzaSerializer):
-            additional_serializers = ({"relation_and_field": "toppings"},)
-
-        serializer = LocalPizzaSerializer(Pizza.objects.all(), many=True)
-
-        with self.assertRaises(ValueError):
-            serializer.data
-
-    def test_list_serializer_does_not_subclass(self):
-        class PizzaListSerializer(serializers.ListSerializer):
-            pass
-
-        class LocalPizzaSerializer(PizzaSerializer):
-            class Meta:
-                model = Pizza
-                fields = ("label", "toppings", "provenance")
-                list_serializer_class = PizzaListSerializer
-
-        pizzas = Pizza.objects.all()
-        with self.assertRaises(ValueError):
-            LocalPizzaSerializer(pizzas, many=True)
-
-    def test_many_true_wrongly_passed(self):
-        pizza = Pizza.objects.first()
-        serializer = PizzaSerializer(pizza, many=True)
-
-        with self.assertRaises(ValueError):
-            serializer.data
-
-    def test_many_true_not_passed_but_should(self):
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas)
-
-        with self.assertRaises(ValueError):
-            serializer.data
+from django.test import TestCase
+
+from rest_framework import serializers
+
+from tests.models import Pizza, Topping, Country
+from tests.serializers import PizzaSerializer
+
+
+class ErrorsTestCase(TestCase):
+    @classmethod
+    def setUpTestData(cls) -> None:
+        cls.canada = Country.objects.create(label="Canada")
+        cls.usa = Country.objects.create(label="USA")
+        cls.china = Country.objects.create(label="China")
+        cls.argentina = Country.objects.create(label="Argentina")
+
+        cls.hawaian_pizza = Pizza.objects.create(
+            label="Hawaiian", provenance=cls.canada
+        )
+        cls.ham_topping = Topping.objects.create(
+            pizza=cls.hawaian_pizza, label="Ham", origin=cls.china
+        )
+        cls.pineapple_topping = Topping.objects.create(
+            pizza=cls.hawaian_pizza, label="Pineapple", origin=cls.argentina
+        )
+
+        cls.pepperoni_pizza = Pizza.objects.create(
+            label="Pepperoni", provenance=cls.usa
+        )
+        cls.pepperoni_topping = Topping.objects.create(
+            pizza=cls.pepperoni_pizza, label="Pepperoni", origin=cls.usa
+        )
+
+    def test_value_error_if_serializer_not_in_additional_serializer_data(self):
+        class LocalPizzaSerializer(PizzaSerializer):
+            additional_serializers = ({"relation_and_field": "toppings"},)
+
+        serializer = LocalPizzaSerializer(Pizza.objects.all(), many=True)
+
+        with self.assertRaises(ValueError):
+            serializer.data
+
+    def test_list_serializer_does_not_subclass(self):
+        class PizzaListSerializer(serializers.ListSerializer):
+            pass
+
+        class LocalPizzaSerializer(PizzaSerializer):
+            class Meta:
+                model = Pizza
+                fields = ("label", "toppings", "provenance")
+                list_serializer_class = PizzaListSerializer
+
+        pizzas = Pizza.objects.all()
+        with self.assertRaises(ValueError):
+            LocalPizzaSerializer(pizzas, many=True)
+
+    def test_many_true_wrongly_passed(self):
+        pizza = Pizza.objects.first()
+        serializer = PizzaSerializer(pizza, many=True)
+
+        with self.assertRaises(ValueError):
+            serializer.data
+
+    def test_many_true_not_passed_but_should(self):
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas)
+
+        with self.assertRaises(ValueError):
+            serializer.data
```

### Comparing `drf-serializer-prefetch-1.1.0b0/tests/test_serializers.py` & `drf-serializer-prefetch-1.1.0b1/tests/test_serializers.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,820 +1,820 @@
-from django.db.models import Prefetch
-from django.test import TestCase
-
-from rest_framework import serializers
-
-from serializer_prefetch import PrefetchingSerializerMixin
-
-from tests.models import Pizza, Topping, Country, Continent
-from tests.serializers import PizzaSerializer, ToppingSerializer, CountrySerializer
-
-
-class SerializersTestCase(TestCase):
-    @classmethod
-    def setUpTestData(cls) -> None:
-        cls.america = Continent.objects.create(label="America")
-        cls.asia = Continent.objects.create(label="Asia")
-
-        cls.canada = Country.objects.create(label="Canada", continent=cls.america)
-        cls.usa = Country.objects.create(label="USA", continent=cls.america)
-        cls.china = Country.objects.create(label="China", continent=cls.asia)
-        cls.argentina = Country.objects.create(label="Argentina", continent=cls.america)
-
-        cls.hawaian_pizza = Pizza.objects.create(
-            label="Hawaiian", provenance=cls.canada
-        )
-        cls.ham_topping = Topping.objects.create(
-            pizza=cls.hawaian_pizza, label="Ham", origin=cls.china
-        )
-        cls.pineapple_topping = Topping.objects.create(
-            pizza=cls.hawaian_pizza, label="Pineapple", origin=cls.argentina
-        )
-
-        cls.pepperoni_pizza = Pizza.objects.create(
-            label="Pepperoni", provenance=cls.usa
-        )
-        cls.pepperoni_topping = Topping.objects.create(
-            pizza=cls.pepperoni_pizza, label="Pepperoni", origin=cls.usa
-        )
-
-    def test_default_behaviour(self):
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(2):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [{"label": "Ham"}, {"label": "Pineapple"}],
-                    "provenance": {"label": "Canada"},
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [{"label": "Pepperoni"}],
-                    "provenance": {"label": "USA"},
-                },
-            ],
-        )
-
-    def test_related_fields(self):
-        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-            toppings = serializers.SerializerMethodField()
-
-            def get_toppings(self, obj):
-                return [topping.label for topping in obj.toppings.all()]
-
-            provenance = serializers.SerializerMethodField()
-
-            def get_provenance(self, obj):
-                return obj.provenance.label
-
-            class Meta:
-                model = Pizza
-                fields = ("label", "toppings", "provenance")
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(3):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": ["Ham", "Pineapple"],
-                    "provenance": "Canada",
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": ["Pepperoni"],
-                    "provenance": "USA",
-                },
-            ],
-        )
-
-        PizzaSerializer.select_related = ("provenance",)
-        PizzaSerializer.prefetch_related = ("toppings",)
-
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(2):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": ["Ham", "Pineapple"],
-                    "provenance": "Canada",
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": ["Pepperoni"],
-                    "provenance": "USA",
-                },
-            ],
-        )
-
-        class PizzaSerializer(PizzaSerializer):
-            def get_select_related(self):
-                return ("provenance",)
-
-            def get_prefetch_related(self):
-                return ("toppings",)
-
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(2):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": ["Ham", "Pineapple"],
-                    "provenance": "Canada",
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": ["Pepperoni"],
-                    "provenance": "USA",
-                },
-            ],
-        )
-
-    def test_get_additional_serializers(self):
-        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-            toppings = serializers.SerializerMethodField()
-
-            def get_toppings(self, obj):
-                return [
-                    ToppingSerializer(topping).data for topping in obj.toppings.all()
-                ]
-
-            class Meta:
-                model = Pizza
-                fields = ("label", "toppings")
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(3):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [{"label": "Ham"}, {"label": "Pineapple"}],
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [{"label": "Pepperoni"}],
-                },
-            ],
-        )
-
-        class PizzaSerializer(PizzaSerializer):
-            additional_serializers = (
-                {
-                    "relation_and_field": "toppings",
-                    "serializer": ToppingSerializer(),
-                },
-            )
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(2):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [{"label": "Ham"}, {"label": "Pineapple"}],
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [{"label": "Pepperoni"}],
-                },
-            ],
-        )
-
-        class PizzaSerializer(PizzaSerializer):
-            def get_additional_serializers(self):
-                return (
-                    {
-                        "relation_and_field": "toppings",
-                        "serializer": ToppingSerializer(),
-                    },
-                )
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(2):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [{"label": "Ham"}, {"label": "Pineapple"}],
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [{"label": "Pepperoni"}],
-                },
-            ],
-        )
-
-    def test_default_behaviour_with_depth(self):
-        class ToppingSerializer(
-            PrefetchingSerializerMixin, serializers.ModelSerializer
-        ):
-            origin = CountrySerializer()
-
-            class Meta:
-                model = Topping
-                fields = ("label", "origin")
-
-        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-            toppings = ToppingSerializer(many=True)
-            provenance = CountrySerializer()
-
-            class Meta:
-                model = Pizza
-                fields = ("label", "toppings", "provenance")
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(3):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [
-                        {"label": "Ham", "origin": {"label": "China"}},
-                        {"label": "Pineapple", "origin": {"label": "Argentina"}},
-                    ],
-                    "provenance": {"label": "Canada"},
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [{"label": "Pepperoni", "origin": {"label": "USA"}}],
-                    "provenance": {"label": "USA"},
-                },
-            ],
-        )
-
-    def test_select_related_with_depth(self):
-        class CountrySerializer(
-            PrefetchingSerializerMixin, serializers.ModelSerializer
-        ):
-            continent = serializers.SerializerMethodField()
-
-            def get_continent(self, obj):
-                return obj.continent.label
-
-            class Meta:
-                model = Country
-                fields = ("label", "continent")
-
-        class ToppingSerializer(
-            PrefetchingSerializerMixin, serializers.ModelSerializer
-        ):
-            origin = CountrySerializer()
-
-            class Meta:
-                model = Topping
-                fields = ("label", "origin")
-
-        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-            toppings = ToppingSerializer(many=True)
-            provenance = CountrySerializer()
-
-            class Meta:
-                model = Pizza
-                fields = ("label", "toppings", "provenance")
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(8):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [
-                        {
-                            "label": "Ham",
-                            "origin": {"label": "China", "continent": "Asia"},
-                        },
-                        {
-                            "label": "Pineapple",
-                            "origin": {"label": "Argentina", "continent": "America"},
-                        },
-                    ],
-                    "provenance": {"label": "Canada", "continent": "America"},
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [
-                        {
-                            "label": "Pepperoni",
-                            "origin": {"label": "USA", "continent": "America"},
-                        }
-                    ],
-                    "provenance": {"label": "USA", "continent": "America"},
-                },
-            ],
-        )
-
-        class CountrySerializer(
-            PrefetchingSerializerMixin, serializers.ModelSerializer
-        ):
-            select_related = ("continent",)
-
-            continent = serializers.SerializerMethodField()
-
-            def get_continent(self, obj):
-                return obj.continent.label
-
-            class Meta:
-                model = Country
-                fields = ("label", "continent")
-
-        class ToppingSerializer(
-            PrefetchingSerializerMixin, serializers.ModelSerializer
-        ):
-            origin = CountrySerializer()
-
-            class Meta:
-                model = Topping
-                fields = ("label", "origin")
-
-        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-            toppings = ToppingSerializer(many=True)
-            provenance = CountrySerializer()
-
-            class Meta:
-                model = Pizza
-                fields = ("label", "toppings", "provenance")
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(4):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [
-                        {
-                            "label": "Ham",
-                            "origin": {"label": "China", "continent": "Asia"},
-                        },
-                        {
-                            "label": "Pineapple",
-                            "origin": {"label": "Argentina", "continent": "America"},
-                        },
-                    ],
-                    "provenance": {"label": "Canada", "continent": "America"},
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [
-                        {
-                            "label": "Pepperoni",
-                            "origin": {"label": "USA", "continent": "America"},
-                        }
-                    ],
-                    "provenance": {"label": "USA", "continent": "America"},
-                },
-            ],
-        )
-
-    def test_get_additional_serializers_with_depth(self):
-        class ToppingSerializer(
-            PrefetchingSerializerMixin, serializers.ModelSerializer
-        ):
-            origin = CountrySerializer()
-
-            class Meta:
-                model = Topping
-                fields = ("label", "origin")
-
-        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-            toppings = serializers.SerializerMethodField()
-
-            def get_toppings(self, obj):
-                return [
-                    ToppingSerializer(topping).data for topping in obj.toppings.all()
-                ]
-
-            class Meta:
-                model = Pizza
-                fields = ("label", "toppings")
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(6):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [
-                        {"label": "Ham", "origin": {"label": "China"}},
-                        {"label": "Pineapple", "origin": {"label": "Argentina"}},
-                    ],
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [{"label": "Pepperoni", "origin": {"label": "USA"}}],
-                },
-            ],
-        )
-
-        class PizzaSerializer(PizzaSerializer):
-            additional_serializers = (
-                {
-                    "relation_and_field": "toppings",
-                    "serializer": ToppingSerializer(),
-                },
-            )
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(3):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [
-                        {"label": "Ham", "origin": {"label": "China"}},
-                        {"label": "Pineapple", "origin": {"label": "Argentina"}},
-                    ],
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [{"label": "Pepperoni", "origin": {"label": "USA"}}],
-                },
-            ],
-        )
-
-        class PizzaSerializer(PizzaSerializer):
-            def get_additional_serializers(self):
-                return (
-                    {
-                        "relation_and_field": "toppings",
-                        "serializer": ToppingSerializer(),
-                    },
-                )
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(3):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [
-                        {"label": "Ham", "origin": {"label": "China"}},
-                        {"label": "Pineapple", "origin": {"label": "Argentina"}},
-                    ],
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [{"label": "Pepperoni", "origin": {"label": "USA"}}],
-                },
-            ],
-        )
-
-    def test_additional_serializers_with_depth_relation_and_field(self):
-        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-            topping_countries = serializers.SerializerMethodField()
-
-            def get_topping_countries(self, obj):
-                return [
-                    CountrySerializer(topping.origin).data
-                    for topping in obj.toppings.all()
-                ]
-
-            class Meta:
-                model = Pizza
-                fields = ("label", "topping_countries")
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(6):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "topping_countries": [
-                        {"label": "China"},
-                        {"label": "Argentina"},
-                    ],
-                },
-                {
-                    "label": "Pepperoni",
-                    "topping_countries": [{"label": "USA"}],
-                },
-            ],
-        )
-
-        class PizzaSerializer(PizzaSerializer):
-            additional_serializers = (
-                {
-                    "relation_and_field": "toppings__origin",
-                    "serializer": CountrySerializer(),
-                },
-            )
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(3):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "topping_countries": [
-                        {"label": "China"},
-                        {"label": "Argentina"},
-                    ],
-                },
-                {
-                    "label": "Pepperoni",
-                    "topping_countries": [{"label": "USA"}],
-                },
-            ],
-        )
-
-    def test_get_additional_serializer_set_on_child_serializer(self):
-        class ToppingSerializer(
-            PrefetchingSerializerMixin, serializers.ModelSerializer
-        ):
-            origin = serializers.SerializerMethodField()
-
-            def get_origin(self, obj):
-                return obj.origin.label
-
-            class Meta:
-                model = Topping
-                fields = ("label", "origin")
-
-        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-            toppings = ToppingSerializer(many=True)
-
-            class Meta:
-                model = Pizza
-                fields = ("label", "toppings")
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(5):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [
-                        {"label": "Ham", "origin": "China"},
-                        {"label": "Pineapple", "origin": "Argentina"},
-                    ],
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [
-                        {"label": "Pepperoni", "origin": "USA"},
-                    ],
-                },
-            ],
-        )
-
-        class ToppingSerializer(ToppingSerializer):
-            additional_serializers = (
-                {
-                    "relation_and_field": "origin",
-                    "serializer": CountrySerializer(),
-                },
-            )
-
-        class PizzaSerializer(PizzaSerializer):
-            toppings = ToppingSerializer(many=True)
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(3):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [
-                        {"label": "Ham", "origin": "China"},
-                        {"label": "Pineapple", "origin": "Argentina"},
-                    ],
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [
-                        {"label": "Pepperoni", "origin": "USA"},
-                    ],
-                },
-            ],
-        )
-
-    def test_allow_passing_prefetch_object(self):
-        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-            american_toppings = serializers.SerializerMethodField()
-
-            def get_american_toppings(self, obj):
-                return [
-                    topping.label
-                    for topping in obj.toppings.filter(
-                        origin__continent__label="America"
-                    )
-                ]
-
-            class Meta:
-                model = Pizza
-                fields = ("label", "american_toppings")
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(3):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "american_toppings": ["Pineapple"],
-                },
-                {
-                    "label": "Pepperoni",
-                    "american_toppings": ["Pepperoni"],
-                },
-            ],
-        )
-
-        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-            prefetch_related = (
-                Prefetch(
-                    "toppings",
-                    queryset=Topping.objects.filter(origin__continent__label="America"),
-                    to_attr="american_toppings",
-                ),
-            )
-
-            american_toppings = serializers.SerializerMethodField()
-
-            def get_american_toppings(self, obj):
-                return [topping.label for topping in obj.american_toppings]
-
-            class Meta:
-                model = Pizza
-                fields = ("label", "american_toppings")
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(2):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "american_toppings": ["Pineapple"],
-                },
-                {
-                    "label": "Pepperoni",
-                    "american_toppings": ["Pepperoni"],
-                },
-            ],
-        )
-
-    def test_allow_passing_prefetch_object_with_depth(self):
-        class ToppingSerializer(
-            PrefetchingSerializerMixin, serializers.ModelSerializer
-        ):
-            origin = serializers.SerializerMethodField()
-
-            def get_origin(self, obj):
-                return obj.origin.label
-
-            class Meta:
-                model = Topping
-                fields = ("label", "origin")
-
-        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
-            toppings = ToppingSerializer(many=True)
-
-            class Meta:
-                model = Pizza
-                fields = ("label", "toppings")
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(5):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [
-                        {"label": "Ham", "origin": "China"},
-                        {"label": "Pineapple", "origin": "Argentina"},
-                    ],
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [{"label": "Pepperoni", "origin": "USA"}],
-                },
-            ],
-        )
-
-        class ToppingSerializer(ToppingSerializer):
-            prefetch_related = (Prefetch("origin"),)
-
-        class PizzaSerializer(PizzaSerializer):
-            toppings = ToppingSerializer(many=True)
-
-        pizzas = Pizza.objects.all()
-        serializer = PizzaSerializer(pizzas, many=True)
-
-        with self.assertNumQueries(3):
-            data = serializer.data
-
-        self.assertEqual(
-            data,
-            [
-                {
-                    "label": "Hawaiian",
-                    "toppings": [
-                        {"label": "Ham", "origin": "China"},
-                        {"label": "Pineapple", "origin": "Argentina"},
-                    ],
-                },
-                {
-                    "label": "Pepperoni",
-                    "toppings": [{"label": "Pepperoni", "origin": "USA"}],
-                },
-            ],
-        )
+from django.db.models import Prefetch
+from django.test import TestCase
+
+from rest_framework import serializers
+
+from serializer_prefetch import PrefetchingSerializerMixin
+
+from tests.models import Pizza, Topping, Country, Continent
+from tests.serializers import PizzaSerializer, ToppingSerializer, CountrySerializer
+
+
+class SerializersTestCase(TestCase):
+    @classmethod
+    def setUpTestData(cls) -> None:
+        cls.america = Continent.objects.create(label="America")
+        cls.asia = Continent.objects.create(label="Asia")
+
+        cls.canada = Country.objects.create(label="Canada", continent=cls.america)
+        cls.usa = Country.objects.create(label="USA", continent=cls.america)
+        cls.china = Country.objects.create(label="China", continent=cls.asia)
+        cls.argentina = Country.objects.create(label="Argentina", continent=cls.america)
+
+        cls.hawaian_pizza = Pizza.objects.create(
+            label="Hawaiian", provenance=cls.canada
+        )
+        cls.ham_topping = Topping.objects.create(
+            pizza=cls.hawaian_pizza, label="Ham", origin=cls.china
+        )
+        cls.pineapple_topping = Topping.objects.create(
+            pizza=cls.hawaian_pizza, label="Pineapple", origin=cls.argentina
+        )
+
+        cls.pepperoni_pizza = Pizza.objects.create(
+            label="Pepperoni", provenance=cls.usa
+        )
+        cls.pepperoni_topping = Topping.objects.create(
+            pizza=cls.pepperoni_pizza, label="Pepperoni", origin=cls.usa
+        )
+
+    def test_default_behaviour(self):
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(2):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [{"label": "Ham"}, {"label": "Pineapple"}],
+                    "provenance": {"label": "Canada"},
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [{"label": "Pepperoni"}],
+                    "provenance": {"label": "USA"},
+                },
+            ],
+        )
+
+    def test_related_fields(self):
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            toppings = serializers.SerializerMethodField()
+
+            def get_toppings(self, obj):
+                return [topping.label for topping in obj.toppings.all()]
+
+            provenance = serializers.SerializerMethodField()
+
+            def get_provenance(self, obj):
+                return obj.provenance.label
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "toppings", "provenance")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(3):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": ["Ham", "Pineapple"],
+                    "provenance": "Canada",
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": ["Pepperoni"],
+                    "provenance": "USA",
+                },
+            ],
+        )
+
+        PizzaSerializer.select_related = ("provenance",)
+        PizzaSerializer.prefetch_related = ("toppings",)
+
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(2):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": ["Ham", "Pineapple"],
+                    "provenance": "Canada",
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": ["Pepperoni"],
+                    "provenance": "USA",
+                },
+            ],
+        )
+
+        class PizzaSerializer(PizzaSerializer):
+            def get_select_related(self):
+                return ("provenance",)
+
+            def get_prefetch_related(self):
+                return ("toppings",)
+
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(2):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": ["Ham", "Pineapple"],
+                    "provenance": "Canada",
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": ["Pepperoni"],
+                    "provenance": "USA",
+                },
+            ],
+        )
+
+    def test_get_additional_serializers(self):
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            toppings = serializers.SerializerMethodField()
+
+            def get_toppings(self, obj):
+                return [
+                    ToppingSerializer(topping).data for topping in obj.toppings.all()
+                ]
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "toppings")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(3):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [{"label": "Ham"}, {"label": "Pineapple"}],
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [{"label": "Pepperoni"}],
+                },
+            ],
+        )
+
+        class PizzaSerializer(PizzaSerializer):
+            additional_serializers = (
+                {
+                    "relation_and_field": "toppings",
+                    "serializer": ToppingSerializer(),
+                },
+            )
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(2):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [{"label": "Ham"}, {"label": "Pineapple"}],
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [{"label": "Pepperoni"}],
+                },
+            ],
+        )
+
+        class PizzaSerializer(PizzaSerializer):
+            def get_additional_serializers(self):
+                return (
+                    {
+                        "relation_and_field": "toppings",
+                        "serializer": ToppingSerializer(),
+                    },
+                )
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(2):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [{"label": "Ham"}, {"label": "Pineapple"}],
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [{"label": "Pepperoni"}],
+                },
+            ],
+        )
+
+    def test_default_behaviour_with_depth(self):
+        class ToppingSerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            origin = CountrySerializer()
+
+            class Meta:
+                model = Topping
+                fields = ("label", "origin")
+
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            toppings = ToppingSerializer(many=True)
+            provenance = CountrySerializer()
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "toppings", "provenance")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(3):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {"label": "Ham", "origin": {"label": "China"}},
+                        {"label": "Pineapple", "origin": {"label": "Argentina"}},
+                    ],
+                    "provenance": {"label": "Canada"},
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [{"label": "Pepperoni", "origin": {"label": "USA"}}],
+                    "provenance": {"label": "USA"},
+                },
+            ],
+        )
+
+    def test_select_related_with_depth(self):
+        class CountrySerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            continent = serializers.SerializerMethodField()
+
+            def get_continent(self, obj):
+                return obj.continent.label
+
+            class Meta:
+                model = Country
+                fields = ("label", "continent")
+
+        class ToppingSerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            origin = CountrySerializer()
+
+            class Meta:
+                model = Topping
+                fields = ("label", "origin")
+
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            toppings = ToppingSerializer(many=True)
+            provenance = CountrySerializer()
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "toppings", "provenance")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(8):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {
+                            "label": "Ham",
+                            "origin": {"label": "China", "continent": "Asia"},
+                        },
+                        {
+                            "label": "Pineapple",
+                            "origin": {"label": "Argentina", "continent": "America"},
+                        },
+                    ],
+                    "provenance": {"label": "Canada", "continent": "America"},
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [
+                        {
+                            "label": "Pepperoni",
+                            "origin": {"label": "USA", "continent": "America"},
+                        }
+                    ],
+                    "provenance": {"label": "USA", "continent": "America"},
+                },
+            ],
+        )
+
+        class CountrySerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            select_related = ("continent",)
+
+            continent = serializers.SerializerMethodField()
+
+            def get_continent(self, obj):
+                return obj.continent.label
+
+            class Meta:
+                model = Country
+                fields = ("label", "continent")
+
+        class ToppingSerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            origin = CountrySerializer()
+
+            class Meta:
+                model = Topping
+                fields = ("label", "origin")
+
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            toppings = ToppingSerializer(many=True)
+            provenance = CountrySerializer()
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "toppings", "provenance")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(4):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {
+                            "label": "Ham",
+                            "origin": {"label": "China", "continent": "Asia"},
+                        },
+                        {
+                            "label": "Pineapple",
+                            "origin": {"label": "Argentina", "continent": "America"},
+                        },
+                    ],
+                    "provenance": {"label": "Canada", "continent": "America"},
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [
+                        {
+                            "label": "Pepperoni",
+                            "origin": {"label": "USA", "continent": "America"},
+                        }
+                    ],
+                    "provenance": {"label": "USA", "continent": "America"},
+                },
+            ],
+        )
+
+    def test_get_additional_serializers_with_depth(self):
+        class ToppingSerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            origin = CountrySerializer()
+
+            class Meta:
+                model = Topping
+                fields = ("label", "origin")
+
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            toppings = serializers.SerializerMethodField()
+
+            def get_toppings(self, obj):
+                return [
+                    ToppingSerializer(topping).data for topping in obj.toppings.all()
+                ]
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "toppings")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(6):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {"label": "Ham", "origin": {"label": "China"}},
+                        {"label": "Pineapple", "origin": {"label": "Argentina"}},
+                    ],
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [{"label": "Pepperoni", "origin": {"label": "USA"}}],
+                },
+            ],
+        )
+
+        class PizzaSerializer(PizzaSerializer):
+            additional_serializers = (
+                {
+                    "relation_and_field": "toppings",
+                    "serializer": ToppingSerializer(),
+                },
+            )
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(3):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {"label": "Ham", "origin": {"label": "China"}},
+                        {"label": "Pineapple", "origin": {"label": "Argentina"}},
+                    ],
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [{"label": "Pepperoni", "origin": {"label": "USA"}}],
+                },
+            ],
+        )
+
+        class PizzaSerializer(PizzaSerializer):
+            def get_additional_serializers(self):
+                return (
+                    {
+                        "relation_and_field": "toppings",
+                        "serializer": ToppingSerializer(),
+                    },
+                )
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(3):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {"label": "Ham", "origin": {"label": "China"}},
+                        {"label": "Pineapple", "origin": {"label": "Argentina"}},
+                    ],
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [{"label": "Pepperoni", "origin": {"label": "USA"}}],
+                },
+            ],
+        )
+
+    def test_additional_serializers_with_depth_relation_and_field(self):
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            topping_countries = serializers.SerializerMethodField()
+
+            def get_topping_countries(self, obj):
+                return [
+                    CountrySerializer(topping.origin).data
+                    for topping in obj.toppings.all()
+                ]
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "topping_countries")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(6):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "topping_countries": [
+                        {"label": "China"},
+                        {"label": "Argentina"},
+                    ],
+                },
+                {
+                    "label": "Pepperoni",
+                    "topping_countries": [{"label": "USA"}],
+                },
+            ],
+        )
+
+        class PizzaSerializer(PizzaSerializer):
+            additional_serializers = (
+                {
+                    "relation_and_field": "toppings__origin",
+                    "serializer": CountrySerializer(),
+                },
+            )
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(3):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "topping_countries": [
+                        {"label": "China"},
+                        {"label": "Argentina"},
+                    ],
+                },
+                {
+                    "label": "Pepperoni",
+                    "topping_countries": [{"label": "USA"}],
+                },
+            ],
+        )
+
+    def test_get_additional_serializer_set_on_child_serializer(self):
+        class ToppingSerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            origin = serializers.SerializerMethodField()
+
+            def get_origin(self, obj):
+                return obj.origin.label
+
+            class Meta:
+                model = Topping
+                fields = ("label", "origin")
+
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            toppings = ToppingSerializer(many=True)
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "toppings")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(5):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {"label": "Ham", "origin": "China"},
+                        {"label": "Pineapple", "origin": "Argentina"},
+                    ],
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [
+                        {"label": "Pepperoni", "origin": "USA"},
+                    ],
+                },
+            ],
+        )
+
+        class ToppingSerializer(ToppingSerializer):
+            additional_serializers = (
+                {
+                    "relation_and_field": "origin",
+                    "serializer": CountrySerializer(),
+                },
+            )
+
+        class PizzaSerializer(PizzaSerializer):
+            toppings = ToppingSerializer(many=True)
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(3):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {"label": "Ham", "origin": "China"},
+                        {"label": "Pineapple", "origin": "Argentina"},
+                    ],
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [
+                        {"label": "Pepperoni", "origin": "USA"},
+                    ],
+                },
+            ],
+        )
+
+    def test_allow_passing_prefetch_object(self):
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            american_toppings = serializers.SerializerMethodField()
+
+            def get_american_toppings(self, obj):
+                return [
+                    topping.label
+                    for topping in obj.toppings.filter(
+                        origin__continent__label="America"
+                    )
+                ]
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "american_toppings")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(3):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "american_toppings": ["Pineapple"],
+                },
+                {
+                    "label": "Pepperoni",
+                    "american_toppings": ["Pepperoni"],
+                },
+            ],
+        )
+
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            prefetch_related = (
+                Prefetch(
+                    "toppings",
+                    queryset=Topping.objects.filter(origin__continent__label="America"),
+                    to_attr="american_toppings",
+                ),
+            )
+
+            american_toppings = serializers.SerializerMethodField()
+
+            def get_american_toppings(self, obj):
+                return [topping.label for topping in obj.american_toppings]
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "american_toppings")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(2):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "american_toppings": ["Pineapple"],
+                },
+                {
+                    "label": "Pepperoni",
+                    "american_toppings": ["Pepperoni"],
+                },
+            ],
+        )
+
+    def test_allow_passing_prefetch_object_with_depth(self):
+        class ToppingSerializer(
+            PrefetchingSerializerMixin, serializers.ModelSerializer
+        ):
+            origin = serializers.SerializerMethodField()
+
+            def get_origin(self, obj):
+                return obj.origin.label
+
+            class Meta:
+                model = Topping
+                fields = ("label", "origin")
+
+        class PizzaSerializer(PrefetchingSerializerMixin, serializers.ModelSerializer):
+            toppings = ToppingSerializer(many=True)
+
+            class Meta:
+                model = Pizza
+                fields = ("label", "toppings")
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(5):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {"label": "Ham", "origin": "China"},
+                        {"label": "Pineapple", "origin": "Argentina"},
+                    ],
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [{"label": "Pepperoni", "origin": "USA"}],
+                },
+            ],
+        )
+
+        class ToppingSerializer(ToppingSerializer):
+            prefetch_related = (Prefetch("origin"),)
+
+        class PizzaSerializer(PizzaSerializer):
+            toppings = ToppingSerializer(many=True)
+
+        pizzas = Pizza.objects.all()
+        serializer = PizzaSerializer(pizzas, many=True)
+
+        with self.assertNumQueries(3):
+            data = serializer.data
+
+        self.assertEqual(
+            data,
+            [
+                {
+                    "label": "Hawaiian",
+                    "toppings": [
+                        {"label": "Ham", "origin": "China"},
+                        {"label": "Pineapple", "origin": "Argentina"},
+                    ],
+                },
+                {
+                    "label": "Pepperoni",
+                    "toppings": [{"label": "Pepperoni", "origin": "USA"}],
+                },
+            ],
+        )
```

