# Comparing `tmp/edx-submissions-3.5.6.tar.gz` & `tmp/edx-submissions-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-submissions-3.5.6.tar", last modified: Fri Jun 16 07:43:03 2023, max compression
+gzip compressed data, was "edx-submissions-3.6.0.tar", last modified: Tue Aug  1 18:23:34 2023, max compression
```

## Comparing `edx-submissions-3.5.6.tar` & `edx-submissions-3.6.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/
--rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.503181 edx-submissions-3.5.6/edx_submissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-06-16 07:43:03.000000 edx-submissions-3.5.6/edx_submissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-06-16 07:43:03.000000 edx-submissions-3.5.6/edx_submissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 07:43:03.000000 edx-submissions-3.5.6/edx_submissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       75 2023-06-16 07:43:03.000000 edx-submissions-3.5.6/edx_submissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-16 07:43:03.000000 edx-submissions-3.5.6/edx_submissions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.503181 edx-submissions-3.5.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/submissions/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5181 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    39479 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/submissions/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/submissions/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/management/commands/analyze_uploaded_file_sizes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/management/commands/update_submissions_uuids.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 07:43:03.507181 edx-submissions-3.5.6/submissions/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     6745 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0001_squashed_0005_CreateTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (122)      910 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0002_auto_20151119_0913.py
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0002_team_submission_optional.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0003_ensure_ascii.py
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0003_submission_status.py
--rw-r--r--   0 runner    (1001) docker     (122)      375 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0004_remove_django_extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/0005_CreateTeamModel.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20313 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     7303 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)    18543 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/team_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-06-16 07:42:58.000000 edx-submissions-3.5.6/submissions/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1793 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.086647 edx-submissions-3.6.0/edx_submissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-08-01 18:23:34.000000 edx-submissions-3.6.0/edx_submissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-08-01 18:23:34.000000 edx-submissions-3.6.0/edx_submissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-01 18:23:34.000000 edx-submissions-3.6.0/edx_submissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-08-01 18:23:34.000000 edx-submissions-3.6.0/edx_submissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-08-01 18:23:34.000000 edx-submissions-3.6.0/edx_submissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.086647 edx-submissions-3.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/submissions/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5170 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39479 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2454 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/submissions/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/submissions/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6344 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/management/commands/analyze_uploaded_file_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/management/commands/update_submissions_uuids.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:34.090648 edx-submissions-3.6.0/submissions/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3489 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6745 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0001_squashed_0005_CreateTeamModel.py
+-rw-r--r--   0 runner    (1001) docker     (122)      910 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0002_auto_20151119_0913.py
+-rw-r--r--   0 runner    (1001) docker     (122)      658 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0002_team_submission_optional.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0003_ensure_ascii.py
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0003_submission_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0004_remove_django_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2379 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/0005_CreateTeamModel.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20313 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7303 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18543 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/team_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1469 2023-08-01 18:23:25.000000 edx-submissions-3.6.0/submissions/views.py
```

### Comparing `edx-submissions-3.5.6/LICENSE` & `edx-submissions-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/PKG-INFO` & `edx-submissions-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-submissions
-Version: 3.5.6
+Version: 3.6.0
 Summary: An API for creating submissions and scores.
 Home-page: http://github.com/openedx/edx-submissions.git
 Author: edX
 License: AGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `edx-submissions-3.5.6/README.rst` & `edx-submissions-3.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/edx_submissions.egg-info/PKG-INFO` & `edx-submissions-3.6.0/edx_submissions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-submissions
-Version: 3.5.6
+Version: 3.6.0
 Summary: An API for creating submissions and scores.
 Home-page: http://github.com/openedx/edx-submissions.git
 Author: edX
 License: AGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
```

### Comparing `edx-submissions-3.5.6/edx_submissions.egg-info/SOURCES.txt` & `edx-submissions-3.6.0/edx_submissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/setup.py` & `edx-submissions-3.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/submissions/admin.py` & `edx-submissions-3.6.0/submissions/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,45 +12,54 @@
     search_fields = (
         'student_item__course_id',
         'student_item__student_id',
         'student_item__item_id',
         'student_item__id'
     )
 
+    @admin.display(
+        ordering='student_item__course_id'
+    )
     def course_id(self, obj):
         return obj.student_item.course_id
-    course_id.admin_order_field = 'student_item__course_id'
 
+    @admin.display(
+        ordering='student_item__item_id'
+    )
     def item_id(self, obj):
         return obj.student_item.item_id
-    item_id.admin_order_field = 'student_item__item_id'
 
+    @admin.display(
+        ordering='student_item__student_id'
+    )
     def student_id(self, obj):
         return obj.student_item.student_id
-    student_id.admin_order_field = 'student_item__student_id'
 
+    @admin.display(
+        description='S.I. ID',
+        ordering='student_item__id',
+    )
     def student_item_id(self, obj):
         """ Formated student item id. """
         url = reverse(
             'admin:submissions_studentitem_change',
             args=[obj.student_item.id]
         )
         return format_html(f'<a href="{url}">{obj.student_item.id}</a>')
 
-    student_item_id.admin_order_field = 'student_item__id'
-    student_item_id.short_description = 'S.I. ID'
-
 
+@admin.register(StudentItem)
 class StudentItemAdmin(admin.ModelAdmin):
     list_display = ('id', 'course_id', 'item_type', 'item_id', 'student_id')
     list_filter = ('item_type',)
     search_fields = ('id', 'course_id', 'item_type', 'item_id', 'student_id')
     readonly_fields = ('course_id', 'item_type', 'item_id', 'student_id')
 
 
+@admin.register(Submission)
 class SubmissionAdmin(admin.ModelAdmin, StudentItemAdminMixin):
     """ Student Submission Admin View. """
     list_display = (
         'id', 'uuid',
         'course_id', 'item_id', 'student_id', 'student_item_id',
         'attempt_number', 'submitted_at',
     )
@@ -79,23 +88,25 @@
     """ Inline admin for TeamSubmissions to view individual Submissions """
     model = Submission
     readonly_fields = ('uuid', 'student_id', 'status')
     exclude = ('student_item', 'attempt_number', 'submitted_at', 'answer')
     extra = 0
 
 
+@admin.register(TeamSubmission)
 class TeamSubmissionAdmin(admin.ModelAdmin):
     """ Student Submission Admin View. """
 
     list_display = ('id', 'uuid', 'course_id', 'item_id', 'team_id', 'status')
     search_fields = ('uuid', 'course_id', 'item_id', 'team_id')
     fields = ('uuid', 'attempt_number', 'submitted_at', 'course_id', 'item_id', 'team_id', 'submitted_by', 'status')
     inlines = (SubmissionInlineAdmin,)
 
 
+@admin.register(Score)
 class ScoreAdmin(admin.ModelAdmin, StudentItemAdminMixin):
     """ Student Score Admin View. """
     list_display = (
         'id',
         'course_id', 'item_id', 'student_id', 'student_item_id',
         'points', 'created_at'
     )
@@ -110,42 +121,40 @@
     )
     search_fields = ('id', ) + StudentItemAdminMixin.search_fields
 
     def points(self, score):
         return f"{score.points_earned}/{score.points_possible}"
 
 
+@admin.register(ScoreSummary)
 class ScoreSummaryAdmin(admin.ModelAdmin, StudentItemAdminMixin):
     """ Student Score Summary Admin View. """
     list_display = (
         'id',
         'course_id', 'item_id', 'student_id', 'student_item_id',
         'latest', 'highest',
     )
     search_fields = ('id', ) + StudentItemAdminMixin.search_fields
     readonly_fields = (
         'student_item_id', 'student_item', 'highest_link', 'latest_link'
     )
     exclude = ('highest', 'latest')
 
+    @admin.display(
+        description='Highest'
+    )
     def highest_link(self, score_summary):
+        """Returns highest link"""
         url = reverse(
             'admin:submissions_score_change', args=[score_summary.highest.id]
         )
         return format_html(f'<a href="{url}">{score_summary.highest}</a>')
 
-    highest_link.short_description = 'Highest'
-
+    @admin.display(
+        description='Latest'
+    )
     def latest_link(self, score_summary):
+        """Returns latest link"""
         url = reverse(
             'admin:submissions_score_change', args=[score_summary.latest.id]
         )
         return format_html(f'<a href="{url}">{score_summary.latest}</a>')
-
-    latest_link.short_description = 'Latest'
-
-
-admin.site.register(Score, ScoreAdmin)
-admin.site.register(StudentItem, StudentItemAdmin)
-admin.site.register(Submission, SubmissionAdmin)
-admin.site.register(TeamSubmission, TeamSubmissionAdmin)
-admin.site.register(ScoreSummary, ScoreSummaryAdmin)
```

### Comparing `edx-submissions-3.5.6/submissions/api.py` & `edx-submissions-3.6.0/submissions/api.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/submissions/errors.py` & `edx-submissions-3.6.0/submissions/errors.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/submissions/management/commands/analyze_uploaded_file_sizes.py` & `edx-submissions-3.6.0/submissions/management/commands/analyze_uploaded_file_sizes.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/submissions/management/commands/update_submissions_uuids.py` & `edx-submissions-3.6.0/submissions/management/commands/update_submissions_uuids.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/submissions/migrations/0001_initial.py` & `edx-submissions-3.6.0/submissions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/submissions/migrations/0001_squashed_0005_CreateTeamModel.py` & `edx-submissions-3.6.0/submissions/migrations/0001_squashed_0005_CreateTeamModel.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/submissions/migrations/0002_auto_20151119_0913.py` & `edx-submissions-3.6.0/submissions/migrations/0002_auto_20151119_0913.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/submissions/migrations/0002_team_submission_optional.py` & `edx-submissions-3.6.0/submissions/migrations/0002_team_submission_optional.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/submissions/migrations/0005_CreateTeamModel.py` & `edx-submissions-3.6.0/submissions/migrations/0005_CreateTeamModel.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/submissions/models.py` & `edx-submissions-3.6.0/submissions/models.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/submissions/serializers.py` & `edx-submissions-3.6.0/submissions/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/submissions/team_api.py` & `edx-submissions-3.6.0/submissions/team_api.py`

 * *Files identical despite different names*

### Comparing `edx-submissions-3.5.6/submissions/views.py` & `edx-submissions-3.6.0/submissions/views.py`

 * *Files identical despite different names*

