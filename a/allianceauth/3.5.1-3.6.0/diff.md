# Comparing `tmp/allianceauth-3.5.1.tar.gz` & `tmp/allianceauth-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-3.5.1.tar", last modified: Tue Jul 11 12:50:25 2023, max compression
+gzip compressed data, was "allianceauth-3.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `allianceauth-3.5.1.tar` & `allianceauth-3.6.0.tar`

### file list

```diff
@@ -1,904 +1,727 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.851134 allianceauth-3.5.1/
--rw-rw-rw-   0 root         (0) root         (0)    18026 2023-07-11 12:50:09.000000 allianceauth-3.5.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      125 2023-07-11 12:50:09.000000 allianceauth-3.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6285 2023-07-11 12:50:25.851134 allianceauth-3.5.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     4978 2023-07-11 12:50:09.000000 allianceauth-3.5.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.718134 allianceauth-3.5.1/allianceauth/
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.721134 allianceauth-3.5.1/allianceauth/analytics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.721134 allianceauth-3.5.1/allianceauth/analytics/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/fixtures/disable_analytics.json
--rw-rw-rw-   0 root         (0) root         (0)     2100 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.722134 allianceauth-3.5.1/allianceauth/analytics/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1664 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py
--rw-rw-rw-   0 root         (0) root         (0)      907 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/migrations/0003_Generate_Identifier.py
--rw-rw-rw-   0 root         (0) root         (0)     1650 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/migrations/0004_auto_20211015_0502.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/migrations/0005_alter_analyticspath_ignore_path.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/migrations/0006_more_ignore_paths.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/signals.py
--rw-rw-rw-   0 root         (0) root         (0)     6605 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.723134 allianceauth-3.5.1/allianceauth/analytics/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4313 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)      783 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/tests/test_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)    10228 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/analytics/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.726134 allianceauth-3.5.1/allianceauth/authentication/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21206 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     5638 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/backends.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/checks.py
--rw-rw-rw-   0 root         (0) root         (0)     2486 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2480 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/hmac_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.726134 allianceauth-3.5.1/allianceauth/authentication/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.726134 allianceauth-3.5.1/allianceauth/authentication/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/management/commands/checkmains.py
--rwxrwxrwx   0 root         (0) root         (0)     2709 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/managers.py
--rw-rw-rw-   0 root         (0) root         (0)     1999 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.731134 allianceauth-3.5.1/allianceauth/authentication/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     3147 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0002_auto_20160907_1914.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0003_authservicesinfo_state.py
--rw-rw-rw-   0 root         (0) root         (0)     2543 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0004_create_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1144 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0005_delete_perms.py
--rw-rw-rw-   0 root         (0) root         (0)     1324 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0006_auto_20160910_0542.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0007_remove_authservicesinfo_is_blue.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0008_set_state.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0009_auto_20161021_0228.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0013_service_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0014_fleetup_permission.py
--rw-rw-rw-   0 root         (0) root         (0)    13077 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0015_user_profiles.py
--rw-rw-rw-   0 root         (0) root         (0)     1637 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0016_ownershiprecord.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0018_alter_state_name_length.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0018_state_member_factions.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0019_merge_20211026_0919.py
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/0021_alter_userprofile_language.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/migrations/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5810 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/models.py
--rw-rw-rw-   0 root         (0) root         (0)     7806 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.694134 allianceauth-3.5.1/allianceauth/authentication/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.694134 allianceauth-3.5.1/allianceauth/authentication/static/allianceauth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.695134 allianceauth-3.5.1/allianceauth/authentication/static/allianceauth/authentication/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.731134 allianceauth-3.5.1/allianceauth/authentication/static/allianceauth/authentication/css/
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/static/allianceauth/authentication/css/admin.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.731134 allianceauth-3.5.1/allianceauth/authentication/static/allianceauth/authentication/img/
--rw-rw-rw-   0 root         (0) root         (0)   161344 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.731134 allianceauth-3.5.1/allianceauth/authentication/static/allianceauth/authentication/img/sso/
--rw-rw-rw-   0 root         (0) root         (0)     2308 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png
--rw-rw-rw-   0 root         (0) root         (0)     2248 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.732134 allianceauth-3.5.1/allianceauth/authentication/task_statistics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/task_statistics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1465 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/task_statistics/counters.py
--rw-rw-rw-   0 root         (0) root         (0)     4042 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/task_statistics/event_series.py
--rw-rw-rw-   0 root         (0) root         (0)     1123 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/task_statistics/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.733134 allianceauth-3.5.1/allianceauth/authentication/task_statistics/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/task_statistics/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/task_statistics/tests/test_counters.py
--rw-rw-rw-   0 root         (0) root         (0)     5843 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/task_statistics/tests/test_event_series.py
--rw-rw-rw-   0 root         (0) root         (0)     2918 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/task_statistics/tests/test_signals.py
--rw-rw-rw-   0 root         (0) root         (0)     1661 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.696134 allianceauth-3.5.1/allianceauth/authentication/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.733134 allianceauth-3.5.1/allianceauth/authentication/templates/authentication/
--rw-rw-rw-   0 root         (0) root         (0)    10738 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/templates/authentication/dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     2613 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/templates/authentication/tokens.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.734134 allianceauth-3.5.1/allianceauth/authentication/templates/public/
--rw-rw-rw-   0 root         (0) root         (0)     1944 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/templates/public/base.html
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/templates/public/lang_select.html
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/templates/public/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1433 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/templates/public/middle_box.html
--rw-rw-rw-   0 root         (0) root         (0)      846 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/templates/public/register.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.735134 allianceauth-3.5.1/allianceauth/authentication/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/templates/registration/activate.html
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/templates/registration/activation_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/templates/registration/activation_email_html.txt
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/templates/registration/activation_email_subject.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.737134 allianceauth-3.5.1/allianceauth/authentication/tests/
--rw-rw-rw-   0 root         (0) root         (0)      833 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    29475 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     3456 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/tests/test_app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     7427 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/tests/test_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     1517 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/tests/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     2452 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/tests/test_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6316 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/tests/test_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)    11478 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     3154 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/tests/test_signals.py
--rw-rw-rw-   0 root         (0) root         (0)    10983 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/tests/test_templatetags.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    11597 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/authentication/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.737134 allianceauth-3.5.1/allianceauth/bin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/bin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3555 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/bin/allianceauth.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/context_processors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.740134 allianceauth-3.5.1/allianceauth/corputils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1970 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.741134 allianceauth-3.5.1/allianceauth/corputils/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1417 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     5358 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/migrations/0002_migrate_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/migrations/0003_granular_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2029 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/migrations/0004_member_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/migrations/0005_cleanup_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7223 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/models.py
--rw-rw-rw-   0 root         (0) root         (0)   947431 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/swagger.json
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.696134 allianceauth-3.5.1/allianceauth/corputils/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.742134 allianceauth-3.5.1/allianceauth/corputils/templates/corputils/
--rw-rw-rw-   0 root         (0) root         (0)     2100 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/templates/corputils/base.html
--rw-rw-rw-   0 root         (0) root         (0)    14915 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/templates/corputils/corpstats.html
--rw-rw-rw-   0 root         (0) root         (0)     2540 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/templates/corputils/search.html
--rw-rw-rw-   0 root         (0) root         (0)    16016 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     6999 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/corputils/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.743134 allianceauth-3.5.1/allianceauth/eveonline/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7277 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.744134 allianceauth-3.5.1/allianceauth/eveonline/autogroups/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/autogroups/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/autogroups/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/autogroups/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.744134 allianceauth-3.5.1/allianceauth/eveonline/autogroups/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     4024 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/autogroups/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/autogroups/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10691 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/autogroups/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2625 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/autogroups/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.745134 allianceauth-3.5.1/allianceauth/eveonline/autogroups/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1403 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/autogroups/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3221 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/autogroups/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)    12356 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/autogroups/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     7961 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/autogroups/tests/test_signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.746134 allianceauth-3.5.1/allianceauth/eveonline/evelinks/
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/evelinks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/evelinks/dotlan.py
--rw-rw-rw-   0 root         (0) root         (0)     3730 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/evelinks/eveimageserver.py
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/evelinks/evewho.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.747134 allianceauth-3.5.1/allianceauth/eveonline/evelinks/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/evelinks/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7329 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/evelinks/tests/test_evelinks.py
--rw-rw-rw-   0 root         (0) root         (0)    11505 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/evelinks/tests/test_templatetags.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/evelinks/zkillboard.py
--rw-rw-rw-   0 root         (0) root         (0)     3350 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.750134 allianceauth-3.5.1/allianceauth/eveonline/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     3133 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0002_remove_eveapikeypair_error_count.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0004_eveapikeypair_sso_verified.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0005_remove_eveallianceinfo_member_count.py
--rw-rw-rw-   0 root         (0) root         (0)      655 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py
--rw-rw-rw-   0 root         (0) root         (0)     4599 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0007_unique_id_name.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0008_remove_apikeys.py
--rw-rw-rw-   0 root         (0) root         (0)      519 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0009_on_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0010_alliance_ticker.py
--rw-rw-rw-   0 root         (0) root         (0)     1297 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0011_ids_to_integers.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0012_index_additions.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0013_evecorporationinfo_ceo_id.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0014_auto_20210105_1413.py
--rw-rw-rw-   0 root         (0) root         (0)     1201 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0015_factions.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0016_character_names_are_not_unique.py
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14052 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/models.py
--rw-rw-rw-   0 root         (0) root         (0)     9958 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/providers.py
--rw-rw-rw-   0 root         (0) root         (0)    41989 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/swagger.json
--rw-rw-rw-   0 root         (0) root         (0)     3808 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.750134 allianceauth-3.5.1/allianceauth/eveonline/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8354 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/templatetags/evelinks.py
--rw-rw-rw-   0 root         (0) root         (0)     4166 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/templatetags/examples.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.752134 allianceauth-3.5.1/allianceauth/eveonline/tests/
--rw-rw-rw-   0 root         (0) root         (0)      739 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6043 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/tests/esi_client_stub.py
--rw-rw-rw-   0 root         (0) root         (0)   297070 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/tests/swagger_old.json
--rw-rw-rw-   0 root         (0) root         (0)    10079 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)    23361 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)    23834 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/tests/test_providers.py
--rw-rw-rw-   0 root         (0) root         (0)    10117 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/tests/test_tasks.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/eveonline/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.754134 allianceauth-3.5.1/allianceauth/fleetactivitytracking/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.756134 allianceauth-3.5.1/allianceauth/fleetactivitytracking/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/migrations/0002_auto_20160905_2220.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/migrations/0003_auto_20160906_2354.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/migrations/0004_make_strings_more_stringy.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/migrations/0005_remove_fat_name.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/migrations/0006_auto_20180803_0430.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/models.py
--rw-rw-rw-   0 root         (0) root         (0)   947431 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/swagger.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.698134 allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.757134 allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html
--rw-rw-rw-   0 root         (0) root         (0)     1208 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkformatter.html
--rw-rw-rw-   0 root         (0) root         (0)     2680 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html
--rw-rw-rw-   0 root         (0) root         (0)     3200 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html
--rw-rw-rw-   0 root         (0) root         (0)     1485 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html
--rw-rw-rw-   0 root         (0) root         (0)     2227 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html
--rw-rw-rw-   0 root         (0) root         (0)     2415 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html
--rw-rw-rw-   0 root         (0) root         (0)     4384 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html
--rw-rw-rw-   0 root         (0) root         (0)     1386 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    16667 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/fleetactivitytracking/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.759134 allianceauth-3.5.1/allianceauth/groupmanagement/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8978 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1370 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     4341 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.763134 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2243 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0003_default_groups.py
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0004_authgroup.py
--rw-rw-rw-   0 root         (0) root         (0)      631 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0005_authgroup_public.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py
--rw-rw-rw-   0 root         (0) root         (0)      877 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0007_on_delete.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1100 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0009_requestlog.py
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0010_authgroup_states.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0011_requestlog_date.py
--rw-rw-rw-   0 root         (0) root         (0)      672 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0012_group_leads.py
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0013_fix_requestlog_date_field.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0014_auto_20200918_1412.py
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0016_remove_grouprequest_status_field.py
--rw-rw-rw-   0 root         (0) root         (0)     2296 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py
--rw-rw-rw-   0 root         (0) root         (0)      520 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1465 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/signals.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.698134 allianceauth-3.5.1/allianceauth/groupmanagement/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.764134 allianceauth-3.5.1/allianceauth/groupmanagement/templates/groupmanagement/
--rw-rw-rw-   0 root         (0) root         (0)     4886 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/templates/groupmanagement/audit.html
--rw-rw-rw-   0 root         (0) root         (0)     4784 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html
--rw-rw-rw-   0 root         (0) root         (0)     4195 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html
--rw-rw-rw-   0 root         (0) root         (0)     2948 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/templates/groupmanagement/groups.html
--rw-rw-rw-   0 root         (0) root         (0)     9513 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/templates/groupmanagement/index.html
--rw-rw-rw-   0 root         (0) root         (0)     1301 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/templates/groupmanagement/menu.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.765134 allianceauth-3.5.1/allianceauth/groupmanagement/tests/
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24713 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)    17375 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)    11668 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     4950 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/tests/test_signals.py
--rw-rw-rw-   0 root         (0) root         (0)     3073 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)     1651 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/urls.py
--rwxrwxrwx   0 root         (0) root         (0)    19860 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/groupmanagement/views.py
--rw-rw-rw-   0 root         (0) root         (0)     4127 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.767134 allianceauth-3.5.1/allianceauth/hrapplications/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      717 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      987 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/auth_hooks.py
--rwxrwxrwx   0 root         (0) root         (0)      353 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.768134 allianceauth-3.5.1/allianceauth/hrapplications/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     6662 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1036 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/migrations/0002_choices_for_questions.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/migrations/0003_applicationquestion_multi_select.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/migrations/0005_sorted_questions.py
--rw-rw-rw-   0 root         (0) root         (0)     1946 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/migrations/0007_auto_20200918_1412.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/migrations/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3237 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.699134 allianceauth-3.5.1/allianceauth/hrapplications/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.769134 allianceauth-3.5.1/allianceauth/hrapplications/templates/hrapplications/
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/templates/hrapplications/corpchoice.html
--rw-rw-rw-   0 root         (0) root         (0)     1915 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/templates/hrapplications/create.html
--rw-rw-rw-   0 root         (0) root         (0)    11885 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/templates/hrapplications/management.html
--rw-rw-rw-   0 root         (0) root         (0)     4107 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/templates/hrapplications/searchview.html
--rw-rw-rw-   0 root         (0) root         (0)     9294 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/templates/hrapplications/view.html
--rw-rw-rw-   0 root         (0) root         (0)     4165 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/tests.py
--rw-rw-rw-   0 root         (0) root         (0)     1113 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/urls.py
--rwxrwxrwx   0 root         (0) root         (0)    12011 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/hrapplications/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.701134 allianceauth-3.5.1/allianceauth/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.699134 allianceauth-3.5.1/allianceauth/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.769134 allianceauth-3.5.1/allianceauth/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    37872 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    84839 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.699134 allianceauth-3.5.1/allianceauth/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.770134 allianceauth-3.5.1/allianceauth/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    70502 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.700134 allianceauth-3.5.1/allianceauth/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.770134 allianceauth-3.5.1/allianceauth/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    37814 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/es/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    84835 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.700134 allianceauth-3.5.1/allianceauth/locale/fr_FR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.771134 allianceauth-3.5.1/allianceauth/locale/fr_FR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    37724 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    85375 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.700134 allianceauth-3.5.1/allianceauth/locale/it_IT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.771134 allianceauth-3.5.1/allianceauth/locale/it_IT/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    17209 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/it_IT/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    77100 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.700134 allianceauth-3.5.1/allianceauth/locale/ja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.772134 allianceauth-3.5.1/allianceauth/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    41641 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/ja/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    88417 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.701134 allianceauth-3.5.1/allianceauth/locale/ko_KR/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.773134 allianceauth-3.5.1/allianceauth/locale/ko_KR/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    36909 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    84828 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.701134 allianceauth-3.5.1/allianceauth/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.773134 allianceauth-3.5.1/allianceauth/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    47123 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/ru/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    94195 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.701134 allianceauth-3.5.1/allianceauth/locale/uk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.774134 allianceauth-3.5.1/allianceauth/locale/uk/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    48143 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/uk/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    95082 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.701134 allianceauth-3.5.1/allianceauth/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.774134 allianceauth-3.5.1/allianceauth/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    27229 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)    79576 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.776134 allianceauth-3.5.1/allianceauth/notifications/
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1113 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1320 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/core.py
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     3907 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.777134 allianceauth-3.5.1/allianceauth/notifications/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1117 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/migrations/0002_auto_20160910_1649.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/migrations/0004_performance_tuning.py
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/migrations/0005_fix_level_choices.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2772 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.702134 allianceauth-3.5.1/allianceauth/notifications/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.777134 allianceauth-3.5.1/allianceauth/notifications/templates/notifications/
--rw-rw-rw-   0 root         (0) root         (0)     1478 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/templates/notifications/list.html
--rw-rw-rw-   0 root         (0) root         (0)     1325 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/templates/notifications/list_partial.html
--rw-rw-rw-   0 root         (0) root         (0)      812 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/templates/notifications/view.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.778134 allianceauth-3.5.1/allianceauth/notifications/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/templatetags/auth_notifications.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.779134 allianceauth-3.5.1/allianceauth/notifications/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3073 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)     2392 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/tests/test_handlers.py
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/tests/test_init.py
--rw-rw-rw-   0 root         (0) root         (0)     9437 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)     2398 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     2975 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/tests/test_templatetags.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     3522 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/notifications/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.781134 allianceauth-3.5.1/allianceauth/optimer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/form.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/form_widgets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.782134 allianceauth-3.5.1/allianceauth/optimer/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1452 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/migrations/0002_auto_20170413_0442.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/migrations/0004_on_delete.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/migrations/0005_add_type_and_description.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1247 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.703134 allianceauth-3.5.1/allianceauth/optimer/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.783134 allianceauth-3.5.1/allianceauth/optimer/templates/optimer/
--rw-rw-rw-   0 root         (0) root         (0)     1486 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/templates/optimer/add.html
--rw-rw-rw-   0 root         (0) root         (0)     2630 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/templates/optimer/fleetoptable.html
--rw-rw-rw-   0 root         (0) root         (0)     3707 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/templates/optimer/management.html
--rw-rw-rw-   0 root         (0) root         (0)     1718 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/templates/optimer/update.html
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5765 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/optimer/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.784134 allianceauth-3.5.1/allianceauth/permissions_tool/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/permissions_tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/permissions_tool/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/permissions_tool/auth_hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.784134 allianceauth-3.5.1/allianceauth/permissions_tool/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      589 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/permissions_tool/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/permissions_tool/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/permissions_tool/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.703134 allianceauth-3.5.1/allianceauth/permissions_tool/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.785134 allianceauth-3.5.1/allianceauth/permissions_tool/templates/permissions_tool/
--rw-rw-rw-   0 root         (0) root         (0)     3414 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/permissions_tool/templates/permissions_tool/audit.html
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html
--rw-rw-rw-   0 root         (0) root         (0)     4891 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/permissions_tool/templates/permissions_tool/overview.html
--rw-rw-rw-   0 root         (0) root         (0)     4968 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/permissions_tool/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/permissions_tool/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2610 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/permissions_tool/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.786134 allianceauth-3.5.1/allianceauth/project_template/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/project_template/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.786134 allianceauth-3.5.1/allianceauth/project_template/log/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/project_template/log/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      821 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/project_template/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.786134 allianceauth-3.5.1/allianceauth/project_template/project_name/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/project_template/project_name/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/project_template/project_name/celery.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.787134 allianceauth-3.5.1/allianceauth/project_template/project_name/settings/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/project_template/project_name/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8741 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/project_template/project_name/settings/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/project_template/project_name/settings/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.787134 allianceauth-3.5.1/allianceauth/project_template/project_name/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/project_template/project_name/static/.gitkeep
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.787134 allianceauth-3.5.1/allianceauth/project_template/project_name/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/project_template/project_name/templates/.gitkeep
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/project_template/project_name/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/project_template/project_name/wsgi.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/project_template/supervisor.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.789134 allianceauth-3.5.1/allianceauth/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3954 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      656 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2117 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     8308 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.790134 allianceauth-3.5.1/allianceauth/services/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.790134 allianceauth-3.5.1/allianceauth/services/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/management/commands/verify_service_accounts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.791134 allianceauth-3.5.1/allianceauth/services/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      483 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/migrations/0001_squashed_0003_delete_groupcache.py
--rw-rw-rw-   0 root         (0) root         (0)     1220 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/migrations/0002_nameformatter.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/migrations/0003_remove_broken_link.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.791134 allianceauth-3.5.1/allianceauth/services/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.793134 allianceauth-3.5.1/allianceauth/services/modules/discord/
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/api.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     4957 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     4446 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.794134 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    28936 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4590 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     3853 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.796134 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5027 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/example_objects.json
--rw-rw-rw-   0 root         (0) root         (0)     3013 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     2784 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py
--rw-rw-rw-   0 root         (0) root         (0)     4477 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py
--rw-rw-rw-   0 root         (0) root         (0)      904 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md
--rw-rw-rw-   0 root         (0) root         (0)    56104 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/test_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1045 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9724 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4966 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     6281 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.797134 allianceauth-3.5.1/allianceauth/services/modules/discord/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      680 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2067 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1538 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7138 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/models.py
--rw-rw-rw-   0 root         (0) root         (0)     9517 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.705134 allianceauth-3.5.1/allianceauth/services/modules/discord/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.705134 allianceauth-3.5.1/allianceauth/services/modules/discord/templates/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.797134 allianceauth-3.5.1/allianceauth/services/modules/discord/templates/services/discord/
--rw-rw-rw-   0 root         (0) root         (0)     1428 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.800134 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/factories.py
--rwxrwxrwx   0 root         (0) root         (0)     2639 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/piloting_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)    10400 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     6287 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     8456 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)    29543 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)    19956 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_managers.py
--rw-rw-rw-   0 root         (0) root         (0)    11474 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)    17995 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6783 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)      566 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     2561 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3635 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discord/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.802134 allianceauth-3.5.1/allianceauth/services/modules/discourse/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      154 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1878 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     7039 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.802134 allianceauth-3.5.1/allianceauth/services/modules/discourse/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2096 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/models.py
--rw-rw-rw-   0 root         (0) root         (0)      533 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/providers.py
--rw-rw-rw-   0 root         (0) root         (0)     2276 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.706134 allianceauth-3.5.1/allianceauth/services/modules/discourse/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.706134 allianceauth-3.5.1/allianceauth/services/modules/discourse/templates/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.803134 allianceauth-3.5.1/allianceauth/services/modules/discourse/templates/services/discourse/
--rw-rw-rw-   0 root         (0) root         (0)      397 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/templates/services/discourse/discourse_service_ctrl.html
--rw-rw-rw-   0 root         (0) root         (0)     5209 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     3486 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/discourse/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.804134 allianceauth-3.5.1/allianceauth/services/modules/example/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/example/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/example/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1336 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/example/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/example/models.py
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/example/urls.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/example/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.805134 allianceauth-3.5.1/allianceauth/services/modules/ips4/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/ips4/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      260 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/ips4/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/ips4/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1554 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/ips4/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     4199 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/ips4/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.806134 allianceauth-3.5.1/allianceauth/services/modules/ips4/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/ips4/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/ips4/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/ips4/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/ips4/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     6035 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/ips4/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/ips4/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     4789 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/ips4/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.808134 allianceauth-3.5.1/allianceauth/services/modules/mumble/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     2958 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/auth_hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.810134 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2868 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0002_auto_20161212_0100.py
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py
--rw-rw-rw-   0 root         (0) root         (0)     2063 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0008_mumbleuser_display_name.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0011_auto_20201011_1009.py
--rw-rw-rw-   0 root         (0) root         (0)     1508 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5630 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.707134 allianceauth-3.5.1/allianceauth/services/modules/mumble/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.707134 allianceauth-3.5.1/allianceauth/services/modules/mumble/templates/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.810134 allianceauth-3.5.1/allianceauth/services/modules/mumble/templates/services/mumble/
--rw-rw-rw-   0 root         (0) root         (0)     1336 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html
--rw-rw-rw-   0 root         (0) root         (0)     8632 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      588 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/mumble/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.812134 allianceauth-3.5.1/allianceauth/services/modules/openfire/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     3615 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/forms.py
--rwxrwxrwx   0 root         (0) root         (0)     8321 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.813134 allianceauth-3.5.1/allianceauth/services/modules/openfire/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2073 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2620 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.708134 allianceauth-3.5.1/allianceauth/services/modules/openfire/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.708134 allianceauth-3.5.1/allianceauth/services/modules/openfire/templates/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.813134 allianceauth-3.5.1/allianceauth/services/modules/openfire/templates/services/openfire/
--rwxrwxrwx   0 root         (0) root         (0)     1183 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html
--rw-rw-rw-   0 root         (0) root         (0)     9478 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     7688 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/openfire/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.815134 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/auth_hooks.py
--rwxrwxrwx   0 root         (0) root         (0)    13459 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.816134 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      683 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2049 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/models.py
--rw-rw-rw-   0 root         (0) root         (0)     2478 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     8189 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5139 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/phpbb3/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.817134 allianceauth-3.5.1/allianceauth/services/modules/smf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)    14780 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.818134 allianceauth-3.5.1/allianceauth/services/modules/smf/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      694 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3740 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     8057 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     5143 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/smf/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.820134 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1860 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     2128 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/forms.py
--rwxrwxrwx   0 root         (0) root         (0)    12601 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.821134 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1995 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py
--rw-rw-rw-   0 root         (0) root         (0)      781 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py
--rw-rw-rw-   0 root         (0) root         (0)     2116 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      784 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1723 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/signals.py
--rw-rw-rw-   0 root         (0) root         (0)     3780 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.709134 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.709134 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/templates/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.709134 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.822134 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/authts/
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/authts/change_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.710134 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/templates/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.822134 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/
--rw-rw-rw-   0 root         (0) root         (0)     1330 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html
--rw-rw-rw-   0 root         (0) root         (0)    21468 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.822134 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/util/
--rwxrwxrwx   0 root         (0) root         (0)       23 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/util/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    15106 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/util/ts3.py
--rw-rw-rw-   0 root         (0) root         (0)     5061 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.824134 allianceauth-3.5.1/allianceauth/services/modules/xenforo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/xenforo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/xenforo/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/xenforo/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1779 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/xenforo/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     3685 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/xenforo/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.825134 allianceauth-3.5.1/allianceauth/services/modules/xenforo/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/xenforo/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2067 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/xenforo/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/xenforo/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/xenforo/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     7153 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/xenforo/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/xenforo/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     4821 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/modules/xenforo/views.py
--rw-rw-rw-   0 root         (0) root         (0)    10087 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.710134 allianceauth-3.5.1/allianceauth/services/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.710134 allianceauth-3.5.1/allianceauth/services/static/allianceauth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.825134 allianceauth-3.5.1/allianceauth/services/static/allianceauth/services/
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/static/allianceauth/services/admin.css
--rw-rw-rw-   0 root         (0) root         (0)     1937 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.711134 allianceauth-3.5.1/allianceauth/services/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.825134 allianceauth-3.5.1/allianceauth/services/templates/public/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/templates/public/menublock.html
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/templates/public/menuitem.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.826134 allianceauth-3.5.1/allianceauth/services/templates/services/
--rw-rw-rw-   0 root         (0) root         (0)     1152 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/templates/services/fleetformattertool.html
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/templates/services/service_confirm_delete.html
--rw-rw-rw-   0 root         (0) root         (0)     1176 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/templates/services/service_credentials.html
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/templates/services/service_password.html
--rwxrwxrwx   0 root         (0) root         (0)     1058 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/templates/services/services.html
--rw-rw-rw-   0 root         (0) root         (0)     1309 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/templates/services/services_ctrl.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.827134 allianceauth-3.5.1/allianceauth/services/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/templatetags/menu_items.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.828134 allianceauth-3.5.1/allianceauth/services/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      514 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     4316 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/tests/test_nameformatter.py
--rw-rw-rw-   0 root         (0) root         (0)    12299 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/tests/test_signals.py
--rw-rw-rw-   0 root         (0) root         (0)     3248 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/urls.py
--rwxrwxrwx   0 root         (0) root         (0)     2450 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/services/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.830134 allianceauth-3.5.1/allianceauth/srp/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      205 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      926 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/auth_hooks.py
--rwxrwxrwx   0 root         (0) root         (0)     1724 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/form.py
--rw-rw-rw-   0 root         (0) root         (0)     1961 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.831134 allianceauth-3.5.1/allianceauth/srp/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2265 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/migrations/0002_srpuserrequest_srp_status_choices.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/migrations/0003_make_strings_more_stringy.py
--rw-rw-rw-   0 root         (0) root         (0)      746 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/migrations/0004_on_delete.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/migrations/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1991 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/models.py
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/providers.py
--rw-rw-rw-   0 root         (0) root         (0)    24877 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/swagger.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.711134 allianceauth-3.5.1/allianceauth/srp/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.832134 allianceauth-3.5.1/allianceauth/srp/templates/srp/
--rw-rw-rw-   0 root         (0) root         (0)     2091 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/templates/srp/add.html
--rw-rw-rw-   0 root         (0) root         (0)    13508 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/templates/srp/data.html
--rw-rw-rw-   0 root         (0) root         (0)     7269 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/templates/srp/management.html
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/templates/srp/request.html
--rw-rw-rw-   0 root         (0) root         (0)     1139 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/templates/srp/update.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.832134 allianceauth-3.5.1/allianceauth/srp/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3623 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/tests/test_managers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.832134 allianceauth-3.5.1/allianceauth/srp/tests/testdata/
--rw-rw-rw-   0 root         (0) root         (0)    28605 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/tests/testdata/zkillboard_killmail_api_81973979.json
--rw-rw-rw-   0 root         (0) root         (0)     1342 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/urls.py
--rwxrwxrwx   0 root         (0) root         (0)    17762 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/srp/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.833134 allianceauth-3.5.1/allianceauth/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.713134 allianceauth-3.5.1/allianceauth/static/allianceauth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.833134 allianceauth-3.5.1/allianceauth/static/allianceauth/css/
--rw-rw-rw-   0 root         (0) root         (0)     4636 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/css/auth-base.css
--rw-rw-rw-   0 root         (0) root         (0)     1173 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/css/checkbox.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.833134 allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/
--rw-rw-rw-   0 root         (0) root         (0)      865 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.834134 allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/darkly/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/darkly/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      624 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/darkly/darkly.less
--rw-rw-rw-   0 root         (0) root         (0)   122466 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.834134 allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/flatly/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/flatly/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/flatly/flatly.less
--rw-rw-rw-   0 root         (0) root         (0)   123138 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/flatly-shared.less
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.836134 allianceauth-3.5.1/allianceauth/static/allianceauth/icons/
--rwxrwxrwx   0 root         (0) root         (0)    21465 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/icons/allianceauth.png
--rwxrwxrwx   0 root         (0) root         (0)     3508 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/icons/apple-touch-icon.png
--rwxrwxrwx   0 root         (0) root         (0)      483 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/icons/favicon-16x16.png
--rwxrwxrwx   0 root         (0) root         (0)      868 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/icons/favicon-32x32.png
--rwxrwxrwx   0 root         (0) root         (0)     2180 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/icons/favicon-96x96.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.836134 allianceauth-3.5.1/allianceauth/static/allianceauth/js/
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/js/eve-time.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.837134 allianceauth-3.5.1/allianceauth/static/allianceauth/js/filterDropDown/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/js/filterDropDown/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     8874 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js
--rw-rw-rw-   0 root         (0) root         (0)     2529 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.713134 allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.713134 allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.837134 allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.838134 allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/
--rw-rw-rw-   0 root         (0) root         (0)     7090 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     7074 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     7111 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4618 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     6487 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)    15830 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css
--rw-rw-rw-   0 root         (0) root         (0)     2482 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/js/refresh_notifications.js
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/allianceauth/js/timers.js
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/static/robots.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.714134 allianceauth-3.5.1/allianceauth/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.838134 allianceauth-3.5.1/allianceauth/templates/admin/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/admin/base_site.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.840134 allianceauth-3.5.1/allianceauth/templates/allianceauth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.840134 allianceauth-3.5.1/allianceauth/templates/allianceauth/admin-status/
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/allianceauth/admin-status/celery_bar_partial.html
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/allianceauth/admin-status/include.html
--rw-rw-rw-   0 root         (0) root         (0)     6109 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/allianceauth/admin-status/overview.html
--rw-rw-rw-   0 root         (0) root         (0)     2299 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/allianceauth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/allianceauth/icons.html
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/allianceauth/messages.html
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/allianceauth/night-toggle.html
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/allianceauth/notifications_menu_item.html
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/allianceauth/side-menu.html
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/allianceauth/top-menu-admin.html
--rw-rw-rw-   0 root         (0) root         (0)     2872 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/allianceauth/top-menu-user-dropdown.html
--rw-rw-rw-   0 root         (0) root         (0)     1489 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/allianceauth/top-menu.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.844134 allianceauth-3.5.1/allianceauth/templates/bundles/
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/auth-base-css.html
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/bootstrap-css.html
--rw-rw-rw-   0 root         (0) root         (0)      613 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/bootstrap-js.html
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/checkbox-css.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/clipboard-js.html
--rw-rw-rw-   0 root         (0) root         (0)      363 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/datatables-css.html
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/datatables-js.html
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/evetime-js.html
--rw-rw-rw-   0 root         (0) root         (0)      111 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/filterdropdown-js.html
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/fontawesome.html
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/jquery-datetimepicker-css.html
--rw-rw-rw-   0 root         (0) root         (0)      387 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/jquery-datetimepicker-js.html
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/jquery-ui-css.html
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/jquery-ui-js.html
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/jquery-visibility-js.html
--rw-rw-rw-   0 root         (0) root         (0)      527 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/moment-js.html
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/refresh-notifications-js.html
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/timers-js.html
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/x-editable-js.html
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templates/bundles/x-editable.css.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.844134 allianceauth-3.5.1/allianceauth/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6405 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/templatetags/admin_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.845134 allianceauth-3.5.1/allianceauth/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11465 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/tests/auth_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2061 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/tests/test_auth_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.845134 allianceauth-3.5.1/allianceauth/thirdparty/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/thirdparty/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.845134 allianceauth-3.5.1/allianceauth/thirdparty/navhelper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/thirdparty/navhelper/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.846134 allianceauth-3.5.1/allianceauth/thirdparty/navhelper/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/thirdparty/navhelper/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2672 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/thirdparty/navhelper/templatetags/navactive.py
--rw-rw-rw-   0 root         (0) root         (0)     3407 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/thirdparty/navhelper/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.847134 allianceauth-3.5.1/allianceauth/timerboard/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      111 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/auth_hooks.py
--rwxrwxrwx   0 root         (0) root         (0)     4708 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/form.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.848134 allianceauth-3.5.1/allianceauth/timerboard/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1629 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1063 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py
--rw-rw-rw-   0 root         (0) root         (0)      763 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/migrations/0003_on_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      811 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/migrations/0004_timer_type.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/migrations/0005_alter_timer_planet_moon.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/migrations/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1593 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.715134 allianceauth-3.5.1/allianceauth/timerboard/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.850134 allianceauth-3.5.1/allianceauth/timerboard/templates/timerboard/
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/templates/timerboard/form.html
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/templates/timerboard/index_button.html
--rw-rw-rw-   0 root         (0) root         (0)      887 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/templates/timerboard/timer_create_form.html
--rw-rw-rw-   0 root         (0) root         (0)      325 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/templates/timerboard/timer_update_form.html
--rw-rw-rw-   0 root         (0) root         (0)    30990 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/templates/timerboard/view.html
--rw-rw-rw-   0 root         (0) root         (0)     8745 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/urls.py
--rwxrwxrwx   0 root         (0) root         (0)     2897 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/timerboard/views.py
--rwxrwxrwx   0 root         (0) root         (0)     1750 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.850134 allianceauth-3.5.1/allianceauth/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/utils/cache.py
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/utils/django.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/utils/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.851134 allianceauth-3.5.1/allianceauth/utils/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/utils/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1194 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/utils/tests/test_cache.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/utils/tests/test_django.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/utils/tests/test_testing.py
--rw-rw-rw-   0 root         (0) root         (0)     2204 2023-07-11 12:50:09.000000 allianceauth-3.5.1/allianceauth/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 12:50:25.719134 allianceauth-3.5.1/allianceauth.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6285 2023-07-11 12:50:25.000000 allianceauth-3.5.1/allianceauth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    38222 2023-07-11 12:50:25.000000 allianceauth-3.5.1/allianceauth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 12:50:25.000000 allianceauth-3.5.1/allianceauth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-07-11 12:50:25.000000 allianceauth-3.5.1/allianceauth.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 12:50:25.000000 allianceauth-3.5.1/allianceauth.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      446 2023-07-11 12:50:25.000000 allianceauth-3.5.1/allianceauth.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 12:50:25.000000 allianceauth-3.5.1/allianceauth.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-07-11 12:50:09.000000 allianceauth-3.5.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2015 2023-07-11 12:50:25.852134 allianceauth-3.5.1/setup.cfg
+-rw-r--r--   0        0        0    18026 2023-08-01 12:21:38.081352 allianceauth-3.6.0/LICENSE
+-rw-r--r--   0        0        0     4978 2023-08-01 12:21:38.081352 allianceauth-3.6.0/README.md
+-rw-r--r--   0        0        0      352 2023-08-01 12:21:38.081352 allianceauth-3.6.0/allianceauth/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.185350 allianceauth-3.6.0/allianceauth/analytics/__init__.py
+-rw-r--r--   0        0        0      567 2023-08-01 12:21:38.081352 allianceauth-3.6.0/allianceauth/analytics/admin.py
+-rw-r--r--   0        0        0      198 2023-08-01 12:21:38.081352 allianceauth-3.6.0/allianceauth/analytics/apps.py
+-rw-r--r--   0        0        0      495 2023-08-01 12:21:38.081352 allianceauth-3.6.0/allianceauth/analytics/fixtures/disable_analytics.json
+-rw-r--r--   0        0        0     2100 2023-08-01 12:21:38.081352 allianceauth-3.6.0/allianceauth/analytics/middleware.py
+-rw-r--r--   0        0        0     1664 2023-08-01 12:21:38.081352 allianceauth-3.6.0/allianceauth/analytics/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1072 2023-08-01 12:21:38.081352 allianceauth-3.6.0/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py
+-rw-r--r--   0        0        0      907 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/analytics/migrations/0003_Generate_Identifier.py
+-rw-r--r--   0        0        0     1650 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/analytics/migrations/0004_auto_20211015_0502.py
+-rw-r--r--   0        0        0      495 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/analytics/migrations/0005_alter_analyticspath_ignore_path.py
+-rw-r--r--   0        0        0     1413 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/analytics/migrations/0006_more_ignore_paths.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.186350 allianceauth-3.6.0/allianceauth/analytics/migrations/__init__.py
+-rw-r--r--   0        0        0     1496 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/analytics/models.py
+-rw-r--r--   0        0        0     1596 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/analytics/signals.py
+-rw-r--r--   0        0        0     6605 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/analytics/tasks.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.186350 allianceauth-3.6.0/allianceauth/analytics/tests/__init__.py
+-rw-r--r--   0        0        0     4313 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/analytics/tests/test_integration.py
+-rw-r--r--   0        0        0      783 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/analytics/tests/test_middleware.py
+-rw-r--r--   0        0        0      938 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/analytics/tests/test_models.py
+-rw-r--r--   0        0        0    10228 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/analytics/tests/test_tasks.py
+-rw-r--r--   0        0        0     1529 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/analytics/tests/test_utils.py
+-rw-r--r--   0        0        0      777 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/analytics/utils.py
+-rw-r--r--   0        0        0       99 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/apps.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.194350 allianceauth-3.6.0/allianceauth/authentication/__init__.py
+-rw-r--r--   0        0        0    21206 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/authentication/admin.py
+-rw-r--r--   0        0        0     1345 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/authentication/app_settings.py
+-rw-r--r--   0        0        0      514 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/authentication/apps.py
+-rw-r--r--   0        0        0     5638 2023-08-01 12:21:38.082352 allianceauth-3.6.0/allianceauth/authentication/backends.py
+-rw-r--r--   0        0        0      434 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/checks.py
+-rw-r--r--   0        0        0     2919 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/decorators.py
+-rw-r--r--   0        0        0     2480 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/forms.py
+-rw-r--r--   0        0        0      776 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/hmac_urls.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.195350 allianceauth-3.6.0/allianceauth/authentication/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.195350 allianceauth-3.6.0/allianceauth/authentication/management/commands/__init__.py
+-rw-r--r--   0        0        0     1026 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/management/commands/checkmains.py
+-rw-r--r--   0        0        0     2709 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/managers.py
+-rw-r--r--   0        0        0     1999 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/middleware.py
+-rw-r--r--   0        0        0     3147 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/migrations/0001_initial.py
+-rw-r--r--   0        0        0      474 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/migrations/0002_auto_20160907_1914.py
+-rw-r--r--   0        0        0      509 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/migrations/0003_authservicesinfo_state.py
+-rw-r--r--   0        0        0     2543 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/migrations/0004_create_permissions.py
+-rw-r--r--   0        0        0     1144 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/migrations/0005_delete_perms.py
+-rw-r--r--   0        0        0     1324 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/migrations/0006_auto_20160910_0542.py
+-rw-r--r--   0        0        0      347 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/migrations/0007_remove_authservicesinfo_is_blue.py
+-rw-r--r--   0        0        0      319 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/migrations/0008_set_state.py
+-rw-r--r--   0        0        0      532 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/migrations/0009_auto_20161021_0228.py
+-rw-r--r--   0        0        0     1235 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py
+-rw-r--r--   0        0        0      538 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py
+-rw-r--r--   0        0        0     1567 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py
+-rw-r--r--   0        0        0     1914 2023-08-01 12:21:38.083352 allianceauth-3.6.0/allianceauth/authentication/migrations/0013_service_modules.py
+-rw-r--r--   0        0        0      660 2023-08-01 12:21:38.084352 allianceauth-3.6.0/allianceauth/authentication/migrations/0014_fleetup_permission.py
+-rw-r--r--   0        0        0    13077 2023-08-01 12:21:38.084352 allianceauth-3.6.0/allianceauth/authentication/migrations/0015_user_profiles.py
+-rw-r--r--   0        0        0     1637 2023-08-01 12:21:38.084352 allianceauth-3.6.0/allianceauth/authentication/migrations/0016_ownershiprecord.py
+-rw-r--r--   0        0        0      612 2023-08-01 12:21:38.084352 allianceauth-3.6.0/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py
+-rw-r--r--   0        0        0      410 2023-08-01 12:21:38.084352 allianceauth-3.6.0/allianceauth/authentication/migrations/0018_alter_state_name_length.py
+-rw-r--r--   0        0        0      545 2023-08-01 12:21:38.084352 allianceauth-3.6.0/allianceauth/authentication/migrations/0018_state_member_factions.py
+-rw-r--r--   0        0        0      295 2023-08-01 12:21:38.084352 allianceauth-3.6.0/allianceauth/authentication/migrations/0019_merge_20211026_0919.py
+-rw-r--r--   0        0        0      841 2023-08-01 12:21:38.084352 allianceauth-3.6.0/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py
+-rw-r--r--   0        0        0     1004 2023-08-01 12:21:38.084352 allianceauth-3.6.0/allianceauth/authentication/migrations/0021_alter_userprofile_language.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.197350 allianceauth-3.6.0/allianceauth/authentication/migrations/__init__.py
+-rw-r--r--   0        0        0     5810 2023-08-01 12:21:38.084352 allianceauth-3.6.0/allianceauth/authentication/models.py
+-rw-r--r--   0        0        0     7806 2023-08-01 12:21:38.084352 allianceauth-3.6.0/allianceauth/authentication/signals.py
+-rw-r--r--   0        0        0      506 2023-08-01 12:21:38.084352 allianceauth-3.6.0/allianceauth/authentication/static/allianceauth/authentication/css/admin.css
+-rw-r--r--   0        0        0   161344 2023-08-01 12:21:38.085352 allianceauth-3.6.0/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg
+-rw-r--r--   0        0        0     2308 2023-08-01 12:21:38.085352 allianceauth-3.6.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png
+-rw-r--r--   0        0        0     2248 2023-08-01 12:21:38.085352 allianceauth-3.6.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.197350 allianceauth-3.6.0/allianceauth/authentication/task_statistics/__init__.py
+-rw-r--r--   0        0        0     1704 2023-08-01 12:21:38.085352 allianceauth-3.6.0/allianceauth/authentication/task_statistics/counters.py
+-rw-r--r--   0        0        0     4113 2023-08-01 12:21:38.085352 allianceauth-3.6.0/allianceauth/authentication/task_statistics/event_series.py
+-rw-r--r--   0        0        0     1176 2023-08-01 12:21:38.085352 allianceauth-3.6.0/allianceauth/authentication/task_statistics/helpers.py
+-rw-r--r--   0        0        0     1528 2023-08-01 12:21:38.085352 allianceauth-3.6.0/allianceauth/authentication/task_statistics/signals.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.197350 allianceauth-3.6.0/allianceauth/authentication/task_statistics/tests/__init__.py
+-rw-r--r--   0        0        0     1886 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/task_statistics/tests/test_counters.py
+-rw-r--r--   0        0        0     5843 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/task_statistics/tests/test_event_series.py
+-rw-r--r--   0        0        0     1963 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/task_statistics/tests/test_item_counter.py
+-rw-r--r--   0        0        0     2719 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/task_statistics/tests/test_signals.py
+-rw-r--r--   0        0        0     1661 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/tasks.py
+-rw-r--r--   0        0        0    10738 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/templates/authentication/dashboard.html
+-rw-r--r--   0        0        0     2613 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/templates/authentication/tokens.html
+-rw-r--r--   0        0        0     1944 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/templates/public/base.html
+-rw-r--r--   0        0        0      624 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/templates/public/lang_select.html
+-rw-r--r--   0        0        0      493 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/templates/public/login.html
+-rw-r--r--   0        0        0     1433 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/templates/public/middle_box.html
+-rw-r--r--   0        0        0      846 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/templates/public/register.html
+-rw-r--r--   0        0        0      197 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/templates/registration/activate.html
+-rw-r--r--   0        0        0      346 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/templates/registration/activation_email.txt
+-rw-r--r--   0        0        0      446 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/templates/registration/activation_email_html.txt
+-rw-r--r--   0        0        0       49 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/templates/registration/activation_email_subject.txt
+-rw-r--r--   0        0        0      833 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/tests/__init__.py
+-rw-r--r--   0        0        0    29475 2023-08-01 12:21:38.086352 allianceauth-3.6.0/allianceauth/authentication/tests/test_admin.py
+-rw-r--r--   0        0        0     3456 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/authentication/tests/test_app_settings.py
+-rw-r--r--   0        0        0     7427 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/authentication/tests/test_backend.py
+-rw-r--r--   0        0        0     1517 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/authentication/tests/test_commands.py
+-rw-r--r--   0        0        0     3538 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/authentication/tests/test_decorators.py
+-rw-r--r--   0        0        0     6316 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/authentication/tests/test_middleware.py
+-rw-r--r--   0        0        0    11478 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/authentication/tests/test_models.py
+-rw-r--r--   0        0        0     3154 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/authentication/tests/test_signals.py
+-rw-r--r--   0        0        0    10983 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/authentication/tests/test_templatetags.py
+-rw-r--r--   0        0        0      975 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/authentication/urls.py
+-rw-r--r--   0        0        0    11597 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/authentication/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.204350 allianceauth-3.6.0/allianceauth/bin/__init__.py
+-rw-r--r--   0        0        0     3555 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/bin/allianceauth.py
+-rw-r--r--   0        0        0      274 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/context_processors.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.205350 allianceauth-3.6.0/allianceauth/corputils/__init__.py
+-rw-r--r--   0        0        0      140 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/corputils/admin.py
+-rw-r--r--   0        0        0      130 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/corputils/apps.py
+-rw-r--r--   0        0        0     1007 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/corputils/auth_hooks.py
+-rw-r--r--   0        0        0     1970 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/corputils/managers.py
+-rw-r--r--   0        0        0     1417 2023-08-01 12:21:38.087352 allianceauth-3.6.0/allianceauth/corputils/migrations/0001_initial.py
+-rw-r--r--   0        0        0     5358 2023-08-01 12:21:38.088352 allianceauth-3.6.0/allianceauth/corputils/migrations/0002_migrate_permissions.py
+-rw-r--r--   0        0        0      844 2023-08-01 12:21:38.088352 allianceauth-3.6.0/allianceauth/corputils/migrations/0003_granular_permissions.py
+-rw-r--r--   0        0        0     2029 2023-08-01 12:21:38.088352 allianceauth-3.6.0/allianceauth/corputils/migrations/0004_member_models.py
+-rw-r--r--   0        0        0     1516 2023-08-01 12:21:38.088352 allianceauth-3.6.0/allianceauth/corputils/migrations/0005_cleanup_permissions.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.205350 allianceauth-3.6.0/allianceauth/corputils/migrations/__init__.py
+-rw-r--r--   0        0        0     7223 2023-08-01 12:21:38.088352 allianceauth-3.6.0/allianceauth/corputils/models.py
+-rw-r--r--   0        0        0   947431 2023-08-01 12:21:38.090352 allianceauth-3.6.0/allianceauth/corputils/swagger.json
+-rw-r--r--   0        0        0      298 2023-08-01 12:21:38.091352 allianceauth-3.6.0/allianceauth/corputils/tasks.py
+-rw-r--r--   0        0        0     2100 2023-08-01 12:21:38.091352 allianceauth-3.6.0/allianceauth/corputils/templates/corputils/base.html
+-rw-r--r--   0        0        0    14915 2023-08-01 12:21:38.091352 allianceauth-3.6.0/allianceauth/corputils/templates/corputils/corpstats.html
+-rw-r--r--   0        0        0     2540 2023-08-01 12:21:38.091352 allianceauth-3.6.0/allianceauth/corputils/templates/corputils/search.html
+-rw-r--r--   0        0        0    16016 2023-08-01 12:21:38.091352 allianceauth-3.6.0/allianceauth/corputils/tests.py
+-rw-r--r--   0        0        0      393 2023-08-01 12:21:38.091352 allianceauth-3.6.0/allianceauth/corputils/urls.py
+-rw-r--r--   0        0        0     6999 2023-08-01 12:21:38.091352 allianceauth-3.6.0/allianceauth/corputils/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.206349 allianceauth-3.6.0/allianceauth/eveonline/__init__.py
+-rw-r--r--   0        0        0     7277 2023-08-01 12:21:38.091352 allianceauth-3.6.0/allianceauth/eveonline/admin.py
+-rw-r--r--   0        0        0      130 2023-08-01 12:21:38.091352 allianceauth-3.6.0/allianceauth/eveonline/apps.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.207350 allianceauth-3.6.0/allianceauth/eveonline/autogroups/__init__.py
+-rw-r--r--   0        0        0     1320 2023-08-01 12:21:38.091352 allianceauth-3.6.0/allianceauth/eveonline/autogroups/admin.py
+-rw-r--r--   0        0        0      229 2023-08-01 12:21:38.091352 allianceauth-3.6.0/allianceauth/eveonline/autogroups/apps.py
+-rw-r--r--   0        0        0     4024 2023-08-01 12:21:38.092352 allianceauth-3.6.0/allianceauth/eveonline/autogroups/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.207350 allianceauth-3.6.0/allianceauth/eveonline/autogroups/migrations/__init__.py
+-rw-r--r--   0        0        0    10691 2023-08-01 12:21:38.092352 allianceauth-3.6.0/allianceauth/eveonline/autogroups/models.py
+-rw-r--r--   0        0        0     2625 2023-08-01 12:21:38.092352 allianceauth-3.6.0/allianceauth/eveonline/autogroups/signals.py
+-rw-r--r--   0        0        0     1403 2023-08-01 12:21:38.092352 allianceauth-3.6.0/allianceauth/eveonline/autogroups/tests/__init__.py
+-rw-r--r--   0        0        0     3221 2023-08-01 12:21:38.092352 allianceauth-3.6.0/allianceauth/eveonline/autogroups/tests/test_managers.py
+-rw-r--r--   0        0        0    12356 2023-08-01 12:21:38.092352 allianceauth-3.6.0/allianceauth/eveonline/autogroups/tests/test_models.py
+-rw-r--r--   0        0        0     7961 2023-08-01 12:21:38.092352 allianceauth-3.6.0/allianceauth/eveonline/autogroups/tests/test_signals.py
+-rw-r--r--   0        0        0      646 2023-08-01 12:21:38.092352 allianceauth-3.6.0/allianceauth/eveonline/evelinks/__init__.py
+-rw-r--r--   0        0        0     1496 2023-08-01 12:21:38.092352 allianceauth-3.6.0/allianceauth/eveonline/evelinks/dotlan.py
+-rw-r--r--   0        0        0     3730 2023-08-01 12:21:38.092352 allianceauth-3.6.0/allianceauth/eveonline/evelinks/eveimageserver.py
+-rw-r--r--   0        0        0     1229 2023-08-01 12:21:38.092352 allianceauth-3.6.0/allianceauth/eveonline/evelinks/evewho.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.207350 allianceauth-3.6.0/allianceauth/eveonline/evelinks/tests/__init__.py
+-rw-r--r--   0        0        0     7329 2023-08-01 12:21:38.092352 allianceauth-3.6.0/allianceauth/eveonline/evelinks/tests/test_evelinks.py
+-rw-r--r--   0        0        0    11505 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/evelinks/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1700 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/evelinks/zkillboard.py
+-rw-r--r--   0        0        0     3350 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/managers.py
+-rw-r--r--   0        0        0     3133 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0001_initial.py
+-rw-r--r--   0        0        0      332 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0002_remove_eveapikeypair_error_count.py
+-rw-r--r--   0        0        0      797 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py
+-rw-r--r--   0        0        0      403 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0004_eveapikeypair_sso_verified.py
+-rw-r--r--   0        0        0      354 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0005_remove_eveallianceinfo_member_count.py
+-rw-r--r--   0        0        0      655 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py
+-rw-r--r--   0        0        0     4599 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0007_unique_id_name.py
+-rw-r--r--   0        0        0      854 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0008_remove_apikeys.py
+-rw-r--r--   0        0        0      519 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0009_on_delete.py
+-rw-r--r--   0        0        0      596 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0010_alliance_ticker.py
+-rw-r--r--   0        0        0     1297 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0011_ids_to_integers.py
+-rw-r--r--   0        0        0     1121 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0012_index_additions.py
+-rw-r--r--   0        0        0      428 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0013_evecorporationinfo_ceo_id.py
+-rw-r--r--   0        0        0      416 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0014_auto_20210105_1413.py
+-rw-r--r--   0        0        0     1201 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0015_factions.py
+-rw-r--r--   0        0        0      409 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0016_character_names_are_not_unique.py
+-rw-r--r--   0        0        0      623 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.210349 allianceauth-3.6.0/allianceauth/eveonline/migrations/__init__.py
+-rw-r--r--   0        0        0    14052 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/models.py
+-rw-r--r--   0        0        0     9958 2023-08-01 12:21:38.093351 allianceauth-3.6.0/allianceauth/eveonline/providers.py
+-rw-r--r--   0        0        0    41989 2023-08-01 12:21:38.095352 allianceauth-3.6.0/allianceauth/eveonline/swagger.json
+-rw-r--r--   0        0        0     3808 2023-08-01 12:21:38.095352 allianceauth-3.6.0/allianceauth/eveonline/tasks.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.210349 allianceauth-3.6.0/allianceauth/eveonline/templatetags/__init__.py
+-rw-r--r--   0        0        0     8354 2023-08-01 12:21:38.095352 allianceauth-3.6.0/allianceauth/eveonline/templatetags/evelinks.py
+-rw-r--r--   0        0        0     4166 2023-08-01 12:21:38.095352 allianceauth-3.6.0/allianceauth/eveonline/templatetags/examples.html
+-rw-r--r--   0        0        0      739 2023-08-01 12:21:38.095352 allianceauth-3.6.0/allianceauth/eveonline/tests/__init__.py
+-rw-r--r--   0        0        0     6043 2023-08-01 12:21:38.095352 allianceauth-3.6.0/allianceauth/eveonline/tests/esi_client_stub.py
+-rw-r--r--   0        0        0   297070 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/eveonline/tests/swagger_old.json
+-rw-r--r--   0        0        0    10079 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/eveonline/tests/test_managers.py
+-rw-r--r--   0        0        0    23361 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/eveonline/tests/test_models.py
+-rw-r--r--   0        0        0    23834 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/eveonline/tests/test_providers.py
+-rw-r--r--   0        0        0    10117 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/eveonline/tests/test_tasks.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.211350 allianceauth-3.6.0/allianceauth/eveonline/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.211350 allianceauth-3.6.0/allianceauth/fleetactivitytracking/__init__.py
+-rw-r--r--   0        0        0      156 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/fleetactivitytracking/admin.py
+-rw-r--r--   0        0        0      148 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/fleetactivitytracking/apps.py
+-rw-r--r--   0        0        0      460 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/fleetactivitytracking/auth_hooks.py
+-rw-r--r--   0        0        0      332 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/fleetactivitytracking/forms.py
+-rw-r--r--   0        0        0     2291 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/fleetactivitytracking/migrations/0001_initial.py
+-rw-r--r--   0        0        0      509 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/fleetactivitytracking/migrations/0002_auto_20160905_2220.py
+-rw-r--r--   0        0        0      460 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/fleetactivitytracking/migrations/0003_auto_20160906_2354.py
+-rw-r--r--   0        0        0      414 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/fleetactivitytracking/migrations/0004_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      510 2023-08-01 12:21:38.096351 allianceauth-3.6.0/allianceauth/fleetactivitytracking/migrations/0005_remove_fat_name.py
+-rw-r--r--   0        0        0      397 2023-08-01 12:21:38.097351 allianceauth-3.6.0/allianceauth/fleetactivitytracking/migrations/0006_auto_20180803_0430.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.213349 allianceauth-3.6.0/allianceauth/fleetactivitytracking/migrations/__init__.py
+-rw-r--r--   0        0        0     1148 2023-08-01 12:21:38.097351 allianceauth-3.6.0/allianceauth/fleetactivitytracking/models.py
+-rw-r--r--   0        0        0   947431 2023-08-01 12:21:38.099352 allianceauth-3.6.0/allianceauth/fleetactivitytracking/swagger.json
+-rw-r--r--   0        0        0     1340 2023-08-01 12:21:38.099352 allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html
+-rw-r--r--   0        0        0     1208 2023-08-01 12:21:38.099352 allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkformatter.html
+-rw-r--r--   0        0        0     2680 2023-08-01 12:21:38.099352 allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html
+-rw-r--r--   0        0        0     3200 2023-08-01 12:21:38.099352 allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html
+-rw-r--r--   0        0        0     1485 2023-08-01 12:21:38.099352 allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html
+-rw-r--r--   0        0        0     2227 2023-08-01 12:21:38.099352 allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html
+-rw-r--r--   0        0        0     2415 2023-08-01 12:21:38.099352 allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html
+-rw-r--r--   0        0        0     4384 2023-08-01 12:21:38.099352 allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html
+-rw-r--r--   0        0        0     1386 2023-08-01 12:21:38.099352 allianceauth-3.6.0/allianceauth/fleetactivitytracking/urls.py
+-rw-r--r--   0        0        0    16667 2023-08-01 12:21:38.099352 allianceauth-3.6.0/allianceauth/fleetactivitytracking/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.213349 allianceauth-3.6.0/allianceauth/groupmanagement/__init__.py
+-rw-r--r--   0        0        0     8978 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/admin.py
+-rw-r--r--   0        0        0      252 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/apps.py
+-rw-r--r--   0        0        0     1370 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/auth_hooks.py
+-rw-r--r--   0        0        0     1349 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/forms.py
+-rw-r--r--   0        0        0     4341 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/managers.py
+-rw-r--r--   0        0        0     2243 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0001_initial.py
+-rw-r--r--   0        0        0      685 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py
+-rw-r--r--   0        0        0      261 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0003_default_groups.py
+-rw-r--r--   0        0        0     4324 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0004_authgroup.py
+-rw-r--r--   0        0        0      631 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0005_authgroup_public.py
+-rw-r--r--   0        0        0      607 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py
+-rw-r--r--   0        0        0      877 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0007_on_delete.py
+-rw-r--r--   0        0        0     1430 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py
+-rw-r--r--   0        0        0     1100 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0009_requestlog.py
+-rw-r--r--   0        0        0      614 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0010_authgroup_states.py
+-rw-r--r--   0        0        0      456 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0011_requestlog_date.py
+-rw-r--r--   0        0        0      672 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0012_group_leads.py
+-rw-r--r--   0        0        0      397 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0013_fix_requestlog_date_field.py
+-rw-r--r--   0        0        0      410 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0014_auto_20200918_1412.py
+-rw-r--r--   0        0        0      567 2023-08-01 12:21:38.100351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py
+-rw-r--r--   0        0        0      353 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0016_remove_grouprequest_status_field.py
+-rw-r--r--   0        0        0     2296 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py
+-rw-r--r--   0        0        0     1082 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py
+-rw-r--r--   0        0        0      520 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.216349 allianceauth-3.6.0/allianceauth/groupmanagement/migrations/__init__.py
+-rw-r--r--   0        0        0     8162 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/models.py
+-rw-r--r--   0        0        0     1465 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/signals.py
+-rw-r--r--   0        0        0      333 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/tasks.py
+-rw-r--r--   0        0        0     4886 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/templates/groupmanagement/audit.html
+-rw-r--r--   0        0        0     4784 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html
+-rw-r--r--   0        0        0     4195 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html
+-rw-r--r--   0        0        0     2948 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/templates/groupmanagement/groups.html
+-rw-r--r--   0        0        0     9513 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/templates/groupmanagement/index.html
+-rw-r--r--   0        0        0     1301 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/templates/groupmanagement/menu.html
+-rw-r--r--   0        0        0      254 2023-08-01 12:21:38.101351 allianceauth-3.6.0/allianceauth/groupmanagement/tests/__init__.py
+-rw-r--r--   0        0        0    24713 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/groupmanagement/tests/test_admin.py
+-rw-r--r--   0        0        0    17375 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/groupmanagement/tests/test_managers.py
+-rw-r--r--   0        0        0    11668 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/groupmanagement/tests/test_models.py
+-rw-r--r--   0        0        0     4950 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/groupmanagement/tests/test_signals.py
+-rw-r--r--   0        0        0     3073 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/groupmanagement/tests/test_views.py
+-rw-r--r--   0        0        0     1651 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/groupmanagement/urls.py
+-rw-r--r--   0        0        0    19860 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/groupmanagement/views.py
+-rw-r--r--   0        0        0     4127 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/hooks.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.216349 allianceauth-3.6.0/allianceauth/hrapplications/__init__.py
+-rw-r--r--   0        0        0      698 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/hrapplications/admin.py
+-rw-r--r--   0        0        0      145 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/hrapplications/apps.py
+-rw-r--r--   0        0        0      987 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/hrapplications/auth_hooks.py
+-rw-r--r--   0        0        0      353 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/hrapplications/forms.py
+-rw-r--r--   0        0        0      900 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/hrapplications/managers.py
+-rw-r--r--   0        0        0     6662 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/hrapplications/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1036 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/hrapplications/migrations/0002_choices_for_questions.py
+-rw-r--r--   0        0        0      415 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/hrapplications/migrations/0003_applicationquestion_multi_select.py
+-rw-r--r--   0        0        0     1461 2023-08-01 12:21:38.102351 allianceauth-3.6.0/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      558 2023-08-01 12:21:38.103351 allianceauth-3.6.0/allianceauth/hrapplications/migrations/0005_sorted_questions.py
+-rw-r--r--   0        0        0     1946 2023-08-01 12:21:38.103351 allianceauth-3.6.0/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py
+-rw-r--r--   0        0        0      427 2023-08-01 12:21:38.103351 allianceauth-3.6.0/allianceauth/hrapplications/migrations/0007_auto_20200918_1412.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.221349 allianceauth-3.6.0/allianceauth/hrapplications/migrations/__init__.py
+-rw-r--r--   0        0        0     3237 2023-08-01 12:21:38.103351 allianceauth-3.6.0/allianceauth/hrapplications/models.py
+-rw-r--r--   0        0        0     1082 2023-08-01 12:21:38.103351 allianceauth-3.6.0/allianceauth/hrapplications/templates/hrapplications/corpchoice.html
+-rw-r--r--   0        0        0     1915 2023-08-01 12:21:38.103351 allianceauth-3.6.0/allianceauth/hrapplications/templates/hrapplications/create.html
+-rw-r--r--   0        0        0    11885 2023-08-01 12:21:38.103351 allianceauth-3.6.0/allianceauth/hrapplications/templates/hrapplications/management.html
+-rw-r--r--   0        0        0     4107 2023-08-01 12:21:38.103351 allianceauth-3.6.0/allianceauth/hrapplications/templates/hrapplications/searchview.html
+-rw-r--r--   0        0        0     9294 2023-08-01 12:21:38.103351 allianceauth-3.6.0/allianceauth/hrapplications/templates/hrapplications/view.html
+-rw-r--r--   0        0        0     4165 2023-08-01 12:21:38.103351 allianceauth-3.6.0/allianceauth/hrapplications/tests.py
+-rw-r--r--   0        0        0     1113 2023-08-01 12:21:38.103351 allianceauth-3.6.0/allianceauth/hrapplications/urls.py
+-rw-r--r--   0        0        0    12011 2023-08-01 12:21:38.103351 allianceauth-3.6.0/allianceauth/hrapplications/views.py
+-rw-r--r--   0        0        0    37872 2023-08-01 12:21:38.103351 allianceauth-3.6.0/allianceauth/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    84839 2023-08-01 12:21:38.104351 allianceauth-3.6.0/allianceauth/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2023-08-01 12:21:38.104351 allianceauth-3.6.0/allianceauth/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    70502 2023-08-01 12:21:38.105351 allianceauth-3.6.0/allianceauth/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    37814 2023-08-01 12:21:38.105351 allianceauth-3.6.0/allianceauth/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    84835 2023-08-01 12:21:38.106351 allianceauth-3.6.0/allianceauth/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    37724 2023-08-01 12:21:38.106351 allianceauth-3.6.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    85375 2023-08-01 12:21:38.106351 allianceauth-3.6.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    17209 2023-08-01 12:21:38.106351 allianceauth-3.6.0/allianceauth/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    77100 2023-08-01 12:21:38.106351 allianceauth-3.6.0/allianceauth/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    41641 2023-08-01 12:21:38.107351 allianceauth-3.6.0/allianceauth/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    88417 2023-08-01 12:21:38.107351 allianceauth-3.6.0/allianceauth/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    36909 2023-08-01 12:21:38.107351 allianceauth-3.6.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    84828 2023-08-01 12:21:38.107351 allianceauth-3.6.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    47123 2023-08-01 12:21:38.108351 allianceauth-3.6.0/allianceauth/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    94195 2023-08-01 12:21:38.108351 allianceauth-3.6.0/allianceauth/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    48143 2023-08-01 12:21:38.108351 allianceauth-3.6.0/allianceauth/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    95082 2023-08-01 12:21:38.108351 allianceauth-3.6.0/allianceauth/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    27229 2023-08-01 12:21:38.108351 allianceauth-3.6.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    79576 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.221349 allianceauth-3.6.0/allianceauth/models.py
+-rw-r--r--   0        0        0       39 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/__init__.py
+-rw-r--r--   0        0        0     1138 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/admin.py
+-rw-r--r--   0        0        0      142 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/apps.py
+-rw-r--r--   0        0        0     1320 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/core.py
+-rw-r--r--   0        0        0      998 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/handlers.py
+-rw-r--r--   0        0        0     3907 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/managers.py
+-rw-r--r--   0        0        0     1117 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/migrations/0001_initial.py
+-rw-r--r--   0        0        0      353 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/migrations/0002_auto_20160910_1649.py
+-rw-r--r--   0        0        0      514 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      714 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/migrations/0004_performance_tuning.py
+-rw-r--r--   0        0        0      512 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/migrations/0005_fix_level_choices.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.222349 allianceauth-3.6.0/allianceauth/notifications/migrations/__init__.py
+-rw-r--r--   0        0        0     2772 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/models.py
+-rw-r--r--   0        0        0     1478 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/templates/notifications/list.html
+-rw-r--r--   0        0        0     1325 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/templates/notifications/list_partial.html
+-rw-r--r--   0        0        0      812 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/templates/notifications/view.html
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.222349 allianceauth-3.6.0/allianceauth/notifications/templatetags/__init__.py
+-rw-r--r--   0        0        0     1156 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/templatetags/auth_notifications.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.227349 allianceauth-3.6.0/allianceauth/notifications/tests/__init__.py
+-rw-r--r--   0        0        0     3073 2023-08-01 12:21:38.109351 allianceauth-3.6.0/allianceauth/notifications/tests/test_core.py
+-rw-r--r--   0        0        0     2392 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/notifications/tests/test_handlers.py
+-rw-r--r--   0        0        0     1120 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/notifications/tests/test_init.py
+-rw-r--r--   0        0        0     9437 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/notifications/tests/test_managers.py
+-rw-r--r--   0        0        0     2398 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/notifications/tests/test_models.py
+-rw-r--r--   0        0        0     2975 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/notifications/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1463 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/notifications/tests/test_views.py
+-rw-r--r--   0        0        0      674 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/notifications/urls.py
+-rw-r--r--   0        0        0     3522 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/notifications/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.227349 allianceauth-3.6.0/allianceauth/optimer/__init__.py
+-rw-r--r--   0        0        0      158 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/optimer/admin.py
+-rw-r--r--   0        0        0      124 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/optimer/apps.py
+-rw-r--r--   0        0        0      763 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/optimer/auth_hooks.py
+-rw-r--r--   0        0        0     1368 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/optimer/form.py
+-rw-r--r--   0        0        0      990 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/optimer/form_widgets.py
+-rw-r--r--   0        0        0     1452 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/optimer/migrations/0001_initial.py
+-rw-r--r--   0        0        0      424 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/optimer/migrations/0002_auto_20170413_0442.py
+-rw-r--r--   0        0        0     1076 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      507 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/optimer/migrations/0004_on_delete.py
+-rw-r--r--   0        0        0     1447 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/optimer/migrations/0005_add_type_and_description.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.227349 allianceauth-3.6.0/allianceauth/optimer/migrations/__init__.py
+-rw-r--r--   0        0        0     1247 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/optimer/models.py
+-rw-r--r--   0        0        0     1486 2023-08-01 12:21:38.110351 allianceauth-3.6.0/allianceauth/optimer/templates/optimer/add.html
+-rw-r--r--   0        0        0     2630 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/optimer/templates/optimer/fleetoptable.html
+-rw-r--r--   0        0        0     3707 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/optimer/templates/optimer/management.html
+-rw-r--r--   0        0        0     1718 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/optimer/templates/optimer/update.html
+-rw-r--r--   0        0        0       26 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/optimer/tests.py
+-rw-r--r--   0        0        0      336 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/optimer/urls.py
+-rw-r--r--   0        0        0     5765 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/optimer/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.227349 allianceauth-3.6.0/allianceauth/permissions_tool/__init__.py
+-rw-r--r--   0        0        0      150 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/permissions_tool/apps.py
+-rw-r--r--   0        0        0      787 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/permissions_tool/auth_hooks.py
+-rw-r--r--   0        0        0      589 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/permissions_tool/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.230349 allianceauth-3.6.0/allianceauth/permissions_tool/migrations/__init__.py
+-rw-r--r--   0        0        0      258 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/permissions_tool/models.py
+-rw-r--r--   0        0        0     3414 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/permissions_tool/templates/permissions_tool/audit.html
+-rw-r--r--   0        0        0      797 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html
+-rw-r--r--   0        0        0     4891 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/permissions_tool/templates/permissions_tool/overview.html
+-rw-r--r--   0        0        0     4968 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/permissions_tool/tests.py
+-rw-r--r--   0        0        0      340 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/permissions_tool/urls.py
+-rw-r--r--   0        0        0     2610 2023-08-01 12:21:38.111351 allianceauth-3.6.0/allianceauth/permissions_tool/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.230349 allianceauth-3.6.0/allianceauth/project_template/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.230349 allianceauth-3.6.0/allianceauth/project_template/log/.gitkeep
+-rw-r--r--   0        0        0      821 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/project_template/manage.py
+-rw-r--r--   0        0        0       38 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/project_template/project_name/__init__.py
+-rw-r--r--   0        0        0     1256 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/project_template/project_name/celery.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.230349 allianceauth-3.6.0/allianceauth/project_template/project_name/settings/__init__.py
+-rw-r--r--   0        0        0     8755 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/project_template/project_name/settings/base.py
+-rw-r--r--   0        0        0     3132 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/project_template/project_name/settings/local.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.230349 allianceauth-3.6.0/allianceauth/project_template/project_name/static/.gitkeep
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.230349 allianceauth-3.6.0/allianceauth/project_template/project_name/templates/.gitkeep
+-rw-r--r--   0        0        0      329 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/project_template/project_name/urls.py
+-rw-r--r--   0        0        0      432 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/project_template/project_name/wsgi.py
+-rw-r--r--   0        0        0     1051 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/project_template/supervisor.conf
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.230349 allianceauth-3.6.0/allianceauth/services/__init__.py
+-rw-r--r--   0        0        0     3954 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/services/abstract.py
+-rw-r--r--   0        0        0     2162 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/services/admin.py
+-rw-r--r--   0        0        0      179 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/services/apps.py
+-rw-r--r--   0        0        0      656 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/services/auth_hooks.py
+-rw-r--r--   0        0        0     2117 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/services/forms.py
+-rw-r--r--   0        0        0     9400 2023-08-01 12:21:38.112351 allianceauth-3.6.0/allianceauth/services/hooks.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.230349 allianceauth-3.6.0/allianceauth/services/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.230349 allianceauth-3.6.0/allianceauth/services/management/commands/__init__.py
+-rw-r--r--   0        0        0      469 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/management/commands/verify_service_accounts.py
+-rw-r--r--   0        0        0      483 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/migrations/0001_squashed_0003_delete_groupcache.py
+-rw-r--r--   0        0        0     1220 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/migrations/0002_nameformatter.py
+-rw-r--r--   0        0        0      522 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/migrations/0003_remove_broken_link.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.230349 allianceauth-3.6.0/allianceauth/services/migrations/__init__.py
+-rw-r--r--   0        0        0     1000 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/models.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.231349 allianceauth-3.6.0/allianceauth/services/modules/__init__.py
+-rw-r--r--   0        0        0       30 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/modules/discord/__init__.py
+-rw-r--r--   0        0        0     1024 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/modules/discord/admin.py
+-rw-r--r--   0        0        0     1290 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/modules/discord/api.py
+-rw-r--r--   0        0        0     1062 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/modules/discord/app_settings.py
+-rw-r--r--   0        0        0      148 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/modules/discord/apps.py
+-rw-r--r--   0        0        0     4957 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/modules/discord/auth_hooks.py
+-rw-r--r--   0        0        0     4446 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/modules/discord/core.py
+-rw-r--r--   0        0        0      372 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/__init__.py
+-rw-r--r--   0        0        0     1681 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/app_settings.py
+-rw-r--r--   0        0        0    28997 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/client.py
+-rw-r--r--   0        0        0     1009 2023-08-01 12:21:38.113351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/exceptions.py
+-rw-r--r--   0        0        0     4590 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/helpers.py
+-rw-r--r--   0        0        0     3853 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/models.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.231349 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/__init__.py
+-rw-r--r--   0        0        0     5027 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/example_objects.json
+-rw-r--r--   0        0        0     3013 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/factories.py
+-rw-r--r--   0        0        0     2784 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py
+-rw-r--r--   0        0        0     4477 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py
+-rw-r--r--   0        0        0      904 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md
+-rw-r--r--   0        0        0    56114 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/test_client.py
+-rw-r--r--   0        0        0     1045 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py
+-rw-r--r--   0        0        0     9724 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py
+-rw-r--r--   0        0        0     4966 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/test_models.py
+-rw-r--r--   0        0        0     6281 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/managers.py
+-rw-r--r--   0        0        0      680 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2067 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0     1538 2023-08-01 12:21:38.114351 allianceauth-3.6.0/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.234349 allianceauth-3.6.0/allianceauth/services/modules/discord/migrations/__init__.py
+-rw-r--r--   0        0        0     7138 2023-08-01 12:21:38.115351 allianceauth-3.6.0/allianceauth/services/modules/discord/models.py
+-rw-r--r--   0        0        0     9517 2023-08-01 12:21:38.115351 allianceauth-3.6.0/allianceauth/services/modules/discord/tasks.py
+-rw-r--r--   0        0        0     1428 2023-08-01 12:21:38.115351 allianceauth-3.6.0/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html
+-rw-r--r--   0        0        0      480 2023-08-01 12:21:38.115351 allianceauth-3.6.0/allianceauth/services/modules/discord/tests/__init__.py
+-rw-r--r--   0        0        0      917 2023-08-01 12:21:38.115351 allianceauth-3.6.0/allianceauth/services/modules/discord/tests/factories.py
+-rw-r--r--   0        0        0     2639 2023-08-01 12:21:38.115351 allianceauth-3.6.0/allianceauth/services/modules/discord/tests/piloting_tasks.py
+-rw-r--r--   0        0        0    10400 2023-08-01 12:21:38.115351 allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_admin.py
+-rw-r--r--   0        0        0      525 2023-08-01 12:21:38.115351 allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_api.py
+-rw-r--r--   0        0        0     6287 2023-08-01 12:21:38.115351 allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     8456 2023-08-01 12:21:38.115351 allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_core.py
+-rw-r--r--   0        0        0    29543 2023-08-01 12:21:38.115351 allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_integration.py
+-rw-r--r--   0        0        0    19956 2023-08-01 12:21:38.116351 allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_managers.py
+-rw-r--r--   0        0        0    11474 2023-08-01 12:21:38.116351 allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_models.py
+-rw-r--r--   0        0        0    17995 2023-08-01 12:21:38.116351 allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_tasks.py
+-rw-r--r--   0        0        0     3201 2023-08-01 12:21:38.116351 allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_utils.py
+-rw-r--r--   0        0        0     6783 2023-08-01 12:21:38.116351 allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_views.py
+-rw-r--r--   0        0        0      538 2023-08-01 12:21:38.116351 allianceauth-3.6.0/allianceauth/services/modules/discord/urls.py
+-rw-r--r--   0        0        0     2561 2023-08-01 12:21:38.116351 allianceauth-3.6.0/allianceauth/services/modules/discord/utils.py
+-rw-r--r--   0        0        0     3635 2023-08-01 12:21:38.116351 allianceauth-3.6.0/allianceauth/services/modules/discord/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.234349 allianceauth-3.6.0/allianceauth/services/modules/discourse/__init__.py
+-rw-r--r--   0        0        0      264 2023-08-01 12:21:38.116351 allianceauth-3.6.0/allianceauth/services/modules/discourse/admin.py
+-rw-r--r--   0        0        0      154 2023-08-01 12:21:38.116351 allianceauth-3.6.0/allianceauth/services/modules/discourse/apps.py
+-rw-r--r--   0        0        0     1878 2023-08-01 12:21:38.116351 allianceauth-3.6.0/allianceauth/services/modules/discourse/auth_hooks.py
+-rw-r--r--   0        0        0     7039 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/discourse/manager.py
+-rw-r--r--   0        0        0      677 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/discourse/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2096 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.234349 allianceauth-3.6.0/allianceauth/services/modules/discourse/migrations/__init__.py
+-rw-r--r--   0        0        0      529 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/discourse/models.py
+-rw-r--r--   0        0        0      533 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/discourse/providers.py
+-rw-r--r--   0        0        0     2276 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/discourse/tasks.py
+-rw-r--r--   0        0        0      397 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/discourse/templates/services/discourse/discourse_service_ctrl.html
+-rw-r--r--   0        0        0     5209 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/discourse/tests.py
+-rw-r--r--   0        0        0      176 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/discourse/urls.py
+-rw-r--r--   0        0        0     3486 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/discourse/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.235349 allianceauth-3.6.0/allianceauth/services/modules/example/__init__.py
+-rw-r--r--   0        0        0      156 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/example/apps.py
+-rw-r--r--   0        0        0     1336 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/example/auth_hooks.py
+-rw-r--r--   0        0        0      411 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/example/models.py
+-rw-r--r--   0        0        0      206 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/example/urls.py
+-rw-r--r--   0        0        0       22 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/example/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.236349 allianceauth-3.6.0/allianceauth/services/modules/ips4/__init__.py
+-rw-r--r--   0        0        0      240 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/ips4/admin.py
+-rw-r--r--   0        0        0      139 2023-08-01 12:21:38.117351 allianceauth-3.6.0/allianceauth/services/modules/ips4/apps.py
+-rw-r--r--   0        0        0     1554 2023-08-01 12:21:38.118351 allianceauth-3.6.0/allianceauth/services/modules/ips4/auth_hooks.py
+-rw-r--r--   0        0        0     4199 2023-08-01 12:21:38.118351 allianceauth-3.6.0/allianceauth/services/modules/ips4/manager.py
+-rw-r--r--   0        0        0      737 2023-08-01 12:21:38.118351 allianceauth-3.6.0/allianceauth/services/modules/ips4/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2025 2023-08-01 12:21:38.118351 allianceauth-3.6.0/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.236349 allianceauth-3.6.0/allianceauth/services/modules/ips4/migrations/__init__.py
+-rw-r--r--   0        0        0      558 2023-08-01 12:21:38.118351 allianceauth-3.6.0/allianceauth/services/modules/ips4/models.py
+-rw-r--r--   0        0        0     1104 2023-08-01 12:21:38.118351 allianceauth-3.6.0/allianceauth/services/modules/ips4/tasks.py
+-rw-r--r--   0        0        0     6035 2023-08-01 12:21:38.118351 allianceauth-3.6.0/allianceauth/services/modules/ips4/tests.py
+-rw-r--r--   0        0        0      495 2023-08-01 12:21:38.118351 allianceauth-3.6.0/allianceauth/services/modules/ips4/urls.py
+-rw-r--r--   0        0        0     4789 2023-08-01 12:21:38.118351 allianceauth-3.6.0/allianceauth/services/modules/ips4/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.236349 allianceauth-3.6.0/allianceauth/services/modules/mumble/__init__.py
+-rw-r--r--   0        0        0      455 2023-08-01 12:21:38.118351 allianceauth-3.6.0/allianceauth/services/modules/mumble/admin.py
+-rw-r--r--   0        0        0      145 2023-08-01 12:21:38.118351 allianceauth-3.6.0/allianceauth/services/modules/mumble/apps.py
+-rw-r--r--   0        0        0     2958 2023-08-01 12:21:38.118351 allianceauth-3.6.0/allianceauth/services/modules/mumble/auth_hooks.py
+-rw-r--r--   0        0        0      726 2023-08-01 12:21:38.118351 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2868 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py
+-rw-r--r--   0        0        0      316 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0002_auto_20161212_0100.py
+-rw-r--r--   0        0        0      613 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py
+-rw-r--r--   0        0        0      548 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py
+-rw-r--r--   0        0        0      561 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py
+-rw-r--r--   0        0        0     2063 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py
+-rw-r--r--   0        0        0      679 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py
+-rw-r--r--   0        0        0      398 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0008_mumbleuser_display_name.py
+-rw-r--r--   0        0        0     1181 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py
+-rw-r--r--   0        0        0      554 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py
+-rw-r--r--   0        0        0      390 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0011_auto_20201011_1009.py
+-rw-r--r--   0        0        0     1508 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.238349 allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/__init__.py
+-rw-r--r--   0        0        0     5630 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/models.py
+-rw-r--r--   0        0        0     3142 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/tasks.py
+-rw-r--r--   0        0        0     1336 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html
+-rw-r--r--   0        0        0     8632 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/tests.py
+-rw-r--r--   0        0        0      560 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/urls.py
+-rw-r--r--   0        0        0      994 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/mumble/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.238349 allianceauth-3.6.0/allianceauth/services/modules/openfire/__init__.py
+-rw-r--r--   0        0        0      317 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/openfire/admin.py
+-rw-r--r--   0        0        0      151 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/openfire/apps.py
+-rw-r--r--   0        0        0     3615 2023-08-01 12:21:38.119351 allianceauth-3.6.0/allianceauth/services/modules/openfire/auth_hooks.py
+-rw-r--r--   0        0        0      263 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/openfire/forms.py
+-rw-r--r--   0        0        0     8321 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/openfire/manager.py
+-rw-r--r--   0        0        0      687 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/openfire/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2073 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.245349 allianceauth-3.6.0/allianceauth/services/modules/openfire/migrations/__init__.py
+-rw-r--r--   0        0        0      495 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/openfire/models.py
+-rw-r--r--   0        0        0     2620 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/openfire/tasks.py
+-rw-r--r--   0        0        0     1183 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html
+-rw-r--r--   0        0        0     9478 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/openfire/tests.py
+-rw-r--r--   0        0        0      585 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/openfire/urls.py
+-rw-r--r--   0        0        0     7688 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/openfire/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.245349 allianceauth-3.6.0/allianceauth/services/modules/phpbb3/__init__.py
+-rw-r--r--   0        0        0      310 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/phpbb3/admin.py
+-rw-r--r--   0        0        0      145 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/phpbb3/apps.py
+-rw-r--r--   0        0        0     2196 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/phpbb3/auth_hooks.py
+-rw-r--r--   0        0        0    13459 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/phpbb3/manager.py
+-rw-r--r--   0        0        0      683 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/phpbb3/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2049 2023-08-01 12:21:38.120351 allianceauth-3.6.0/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.245349 allianceauth-3.6.0/allianceauth/services/modules/phpbb3/migrations/__init__.py
+-rw-r--r--   0        0        0      487 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/phpbb3/models.py
+-rw-r--r--   0        0        0     2478 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/phpbb3/tasks.py
+-rw-r--r--   0        0        0     8189 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/phpbb3/tests.py
+-rw-r--r--   0        0        0      504 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/phpbb3/urls.py
+-rw-r--r--   0        0        0     5139 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/phpbb3/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.245349 allianceauth-3.6.0/allianceauth/services/modules/smf/__init__.py
+-rw-r--r--   0        0        0      302 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/smf/admin.py
+-rw-r--r--   0        0        0      136 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/smf/apps.py
+-rw-r--r--   0        0        0     2408 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/smf/auth_hooks.py
+-rw-r--r--   0        0        0    14780 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/smf/manager.py
+-rw-r--r--   0        0        0      677 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/smf/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2011 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/smf/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0      694 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.246349 allianceauth-3.6.0/allianceauth/services/modules/smf/migrations/__init__.py
+-rw-r--r--   0        0        0      475 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/smf/models.py
+-rw-r--r--   0        0        0     3740 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/smf/tasks.py
+-rw-r--r--   0        0        0     8057 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/smf/tests.py
+-rw-r--r--   0        0        0      489 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/smf/urls.py
+-rw-r--r--   0        0        0     5143 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/smf/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.246349 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/__init__.py
+-rw-r--r--   0        0        0     1872 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/admin.py
+-rw-r--r--   0        0        0      209 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/apps.py
+-rw-r--r--   0        0        0     2128 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/auth_hooks.py
+-rw-r--r--   0        0        0      500 2023-08-01 12:21:38.121351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/forms.py
+-rw-r--r--   0        0        0    12601 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/manager.py
+-rw-r--r--   0        0        0     1995 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py
+-rw-r--r--   0        0        0      538 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py
+-rw-r--r--   0        0        0      781 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py
+-rw-r--r--   0        0        0     2116 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py
+-rw-r--r--   0        0        0      784 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.247349 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/migrations/__init__.py
+-rw-r--r--   0        0        0     1567 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/models.py
+-rw-r--r--   0        0        0     1723 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/signals.py
+-rw-r--r--   0        0        0     3780 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/tasks.py
+-rw-r--r--   0        0        0      267 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/templates/admin/teamspeak3/authts/change_list.html
+-rw-r--r--   0        0        0     1330 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html
+-rw-r--r--   0        0        0     1098 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html
+-rw-r--r--   0        0        0    21468 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/tests.py
+-rw-r--r--   0        0        0      661 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/urls.py
+-rw-r--r--   0        0        0       23 2023-08-01 12:21:38.122351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/util/__init__.py
+-rw-r--r--   0        0        0    15106 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/util/ts3.py
+-rw-r--r--   0        0        0     5061 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.248349 allianceauth-3.6.0/allianceauth/services/modules/xenforo/__init__.py
+-rw-r--r--   0        0        0      314 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/modules/xenforo/admin.py
+-rw-r--r--   0        0        0      148 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/modules/xenforo/apps.py
+-rw-r--r--   0        0        0     1779 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/modules/xenforo/auth_hooks.py
+-rw-r--r--   0        0        0     3685 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/modules/xenforo/manager.py
+-rw-r--r--   0        0        0      685 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/modules/xenforo/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2067 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.248349 allianceauth-3.6.0/allianceauth/services/modules/xenforo/migrations/__init__.py
+-rw-r--r--   0        0        0      491 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/modules/xenforo/models.py
+-rw-r--r--   0        0        0     1268 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/modules/xenforo/tasks.py
+-rw-r--r--   0        0        0     7153 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/modules/xenforo/tests.py
+-rw-r--r--   0        0        0      529 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/modules/xenforo/urls.py
+-rw-r--r--   0        0        0     4821 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/modules/xenforo/views.py
+-rw-r--r--   0        0        0    10087 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/signals.py
+-rw-r--r--   0        0        0      126 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/static/allianceauth/services/admin.css
+-rw-r--r--   0        0        0     1937 2023-08-01 12:21:38.123351 allianceauth-3.6.0/allianceauth/services/tasks.py
+-rw-r--r--   0        0        0       57 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/templates/public/menublock.html
+-rw-r--r--   0        0        0      334 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/templates/public/menuitem.html
+-rw-r--r--   0        0        0     1152 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/templates/services/fleetformattertool.html
+-rw-r--r--   0        0        0     1213 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/templates/services/service_confirm_delete.html
+-rw-r--r--   0        0        0     1176 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/templates/services/service_credentials.html
+-rw-r--r--   0        0        0     1099 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/templates/services/service_password.html
+-rw-r--r--   0        0        0     1058 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/templates/services/services.html
+-rw-r--r--   0        0        0     1309 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/templates/services/services_ctrl.html
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.249349 allianceauth-3.6.0/allianceauth/services/templatetags/__init__.py
+-rw-r--r--   0        0        0      565 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/templatetags/menu_items.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.249349 allianceauth-3.6.0/allianceauth/services/tests/__init__.py
+-rw-r--r--   0        0        0     1048 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/tests/test_hooks.py
+-rw-r--r--   0        0        0      514 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/tests/test_models.py
+-rw-r--r--   0        0        0     4316 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/tests/test_nameformatter.py
+-rw-r--r--   0        0        0    12299 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/tests/test_signals.py
+-rw-r--r--   0        0        0     3248 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/tests/test_tasks.py
+-rw-r--r--   0        0        0      530 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/urls.py
+-rw-r--r--   0        0        0     2450 2023-08-01 12:21:38.124351 allianceauth-3.6.0/allianceauth/services/views.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.249349 allianceauth-3.6.0/allianceauth/srp/__init__.py
+-rw-r--r--   0        0        0      205 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/admin.py
+-rw-r--r--   0        0        0      112 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/apps.py
+-rw-r--r--   0        0        0      926 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/auth_hooks.py
+-rw-r--r--   0        0        0     1724 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/form.py
+-rw-r--r--   0        0        0     1961 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/managers.py
+-rw-r--r--   0        0        0     2265 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/migrations/0001_initial.py
+-rw-r--r--   0        0        0      488 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/migrations/0002_srpuserrequest_srp_status_choices.py
+-rw-r--r--   0        0        0     2048 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/migrations/0003_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      746 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/migrations/0004_on_delete.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.250349 allianceauth-3.6.0/allianceauth/srp/migrations/__init__.py
+-rw-r--r--   0        0        0     1991 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/models.py
+-rw-r--r--   0        0        0      388 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/providers.py
+-rw-r--r--   0        0        0    24877 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/swagger.json
+-rw-r--r--   0        0        0     2091 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/templates/srp/add.html
+-rw-r--r--   0        0        0    13508 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/templates/srp/data.html
+-rw-r--r--   0        0        0     7269 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/templates/srp/management.html
+-rw-r--r--   0        0        0      891 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/templates/srp/request.html
+-rw-r--r--   0        0        0     1139 2023-08-01 12:21:38.125351 allianceauth-3.6.0/allianceauth/srp/templates/srp/update.html
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.250349 allianceauth-3.6.0/allianceauth/srp/tests/__init__.py
+-rw-r--r--   0        0        0     3623 2023-08-01 12:21:38.126351 allianceauth-3.6.0/allianceauth/srp/tests/test_managers.py
+-rw-r--r--   0        0        0    28605 2023-08-01 12:21:38.126351 allianceauth-3.6.0/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json
+-rw-r--r--   0        0        0      363 2023-08-01 12:21:38.126351 allianceauth-3.6.0/allianceauth/srp/tests/testdata/zkillboard_killmail_api_81973979.json
+-rw-r--r--   0        0        0     1342 2023-08-01 12:21:38.126351 allianceauth-3.6.0/allianceauth/srp/urls.py
+-rw-r--r--   0        0        0    17762 2023-08-01 12:21:38.126351 allianceauth-3.6.0/allianceauth/srp/views.py
+-rw-r--r--   0        0        0     4636 2023-08-01 12:21:38.126351 allianceauth-3.6.0/allianceauth/static/allianceauth/css/auth-base.css
+-rw-r--r--   0        0        0     1173 2023-08-01 12:21:38.126351 allianceauth-3.6.0/allianceauth/static/allianceauth/css/checkbox.css
+-rw-r--r--   0        0        0      865 2023-08-01 12:21:38.126351 allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less
+-rw-r--r--   0        0        0     1078 2023-08-01 12:21:38.126351 allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/darkly/LICENSE
+-rw-r--r--   0        0        0      624 2023-08-01 12:21:38.126351 allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.less
+-rw-r--r--   0        0        0   122466 2023-08-01 12:21:38.127351 allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css
+-rw-r--r--   0        0        0      979 2023-08-01 12:21:38.127351 allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/flatly-shared.less
+-rw-r--r--   0        0        0     1078 2023-08-01 12:21:38.127351 allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/flatly/LICENSE
+-rw-r--r--   0        0        0      985 2023-08-01 12:21:38.127351 allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.less
+-rw-r--r--   0        0        0   123138 2023-08-01 12:21:38.127351 allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css
+-rwxr-xr-x   0        0        0    21465 2023-08-01 12:21:38.127351 allianceauth-3.6.0/allianceauth/static/allianceauth/icons/allianceauth.png
+-rw-r--r--   0        0        0     7686 2023-08-01 12:21:38.127351 allianceauth-3.6.0/allianceauth/static/allianceauth/icons/android-chrome-192x192.png
+-rw-r--r--   0        0        0    26346 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/icons/android-chrome-512x512.png
+-rw-r--r--   0        0        0     7160 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/icons/apple-touch-icon.png
+-rw-r--r--   0        0        0      272 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/icons/browserconfig.xml
+-rw-r--r--   0        0        0      941 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/icons/favicon-16x16.png
+-rw-r--r--   0        0        0     1565 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/icons/favicon-32x32.png
+-rwxr-xr-x   0        0        0     2180 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/icons/favicon-96x96.png
+-rw-r--r--   0        0        0    15086 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/icons/favicon.ico
+-rw-r--r--   0        0        0     4681 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/icons/mstile-150x150.png
+-rw-r--r--   0        0        0     2590 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/icons/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      478 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/icons/site.webmanifest
+-rw-r--r--   0        0        0      558 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/eve-time.js
+-rw-r--r--   0        0        0     1070 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/filterDropDown/LICENSE
+-rw-r--r--   0        0        0     8874 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js
+-rw-r--r--   0        0        0     2529 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js
+-rw-r--r--   0        0        0     7090 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     7074 2023-08-01 12:21:38.128351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     4618 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     7111 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     4618 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     6487 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    15830 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css
+-rw-r--r--   0        0        0     2482 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/refresh_notifications.js
+-rw-r--r--   0        0        0     1198 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/timerboard.js
+-rw-r--r--   0        0        0      999 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/static/allianceauth/js/timers.js
+-rw-r--r--   0        0        0       26 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/static/robots.txt
+-rw-r--r--   0        0        0      119 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/templates/admin/base_site.html
+-rw-r--r--   0        0        0      413 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/templates/allianceauth/admin-status/celery_bar_partial.html
+-rw-r--r--   0        0        0       47 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/templates/allianceauth/admin-status/include.html
+-rw-r--r--   0        0        0     6320 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/templates/allianceauth/admin-status/overview.html
+-rw-r--r--   0        0        0     2299 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/templates/allianceauth/base.html
+-rw-r--r--   0        0        0      927 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/templates/allianceauth/icons.html
+-rw-r--r--   0        0        0     1069 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/templates/allianceauth/messages.html
+-rw-r--r--   0        0        0      258 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/templates/allianceauth/night-toggle.html
+-rw-r--r--   0        0        0      445 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/templates/allianceauth/notifications_menu_item.html
+-rw-r--r--   0        0        0      873 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/templates/allianceauth/side-menu.html
+-rw-r--r--   0        0        0      882 2023-08-01 12:21:38.129351 allianceauth-3.6.0/allianceauth/templates/allianceauth/top-menu-admin.html
+-rw-r--r--   0        0        0     2872 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/allianceauth/top-menu-user-dropdown.html
+-rw-r--r--   0        0        0     1489 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/allianceauth/top-menu.html
+-rw-r--r--   0        0        0       96 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/auth-base-css.html
+-rw-r--r--   0        0        0     1268 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/bootstrap-css.html
+-rw-r--r--   0        0        0      613 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/bootstrap-js.html
+-rw-r--r--   0        0        0       95 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/checkbox-css.html
+-rw-r--r--   0        0        0      313 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/clipboard-js.html
+-rw-r--r--   0        0        0      363 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/datatables-css.html
+-rw-r--r--   0        0        0      623 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/datatables-js.html
+-rw-r--r--   0        0        0       86 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/evetime-js.html
+-rw-r--r--   0        0        0      111 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/filterdropdown-js.html
+-rw-r--r--   0        0        0      349 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/fontawesome.html
+-rw-r--r--   0        0        0      392 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/jquery-datetimepicker-css.html
+-rw-r--r--   0        0        0      387 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/jquery-datetimepicker-js.html
+-rw-r--r--   0        0        0      507 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/jquery-ui-css.html
+-rw-r--r--   0        0        0      333 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/jquery-ui-js.html
+-rw-r--r--   0        0        0      344 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/jquery-visibility-js.html
+-rw-r--r--   0        0        0      527 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/moment-js.html
+-rw-r--r--   0        0        0       99 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/refresh-notifications-js.html
+-rw-r--r--   0        0        0       88 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/timerboard-js.html
+-rw-r--r--   0        0        0       84 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/timers-js.html
+-rw-r--r--   0        0        0      368 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/x-editable-js.html
+-rw-r--r--   0        0        0      375 2023-08-01 12:21:38.130351 allianceauth-3.6.0/allianceauth/templates/bundles/x-editable.css.html
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.255349 allianceauth-3.6.0/allianceauth/templatetags/__init__.py
+-rw-r--r--   0        0        0     6478 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/templatetags/admin_status.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.255349 allianceauth-3.6.0/allianceauth/tests/__init__.py
+-rw-r--r--   0        0        0    11465 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/tests/auth_utils.py
+-rw-r--r--   0        0        0     2061 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/tests/test_auth_utils.py
+-rw-r--r--   0        0        0     2897 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/tests/test_urls.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.255349 allianceauth-3.6.0/allianceauth/thirdparty/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.255349 allianceauth-3.6.0/allianceauth/thirdparty/navhelper/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.255349 allianceauth-3.6.0/allianceauth/thirdparty/navhelper/templatetags/__init__.py
+-rw-r--r--   0        0        0     2672 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/thirdparty/navhelper/templatetags/navactive.py
+-rw-r--r--   0        0        0     3407 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/thirdparty/navhelper/tests.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.255349 allianceauth-3.6.0/allianceauth/timerboard/__init__.py
+-rw-r--r--   0        0        0      111 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/timerboard/admin.py
+-rw-r--r--   0        0        0      133 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/timerboard/apps.py
+-rw-r--r--   0        0        0      701 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/timerboard/auth_hooks.py
+-rw-r--r--   0        0        0     5267 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/timerboard/form.py
+-rw-r--r--   0        0        0     1629 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/timerboard/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1063 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py
+-rw-r--r--   0        0        0      763 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/timerboard/migrations/0003_on_delete.py
+-rw-r--r--   0        0        0      811 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/timerboard/migrations/0004_timer_type.py
+-rw-r--r--   0        0        0      410 2023-08-01 12:21:38.131351 allianceauth-3.6.0/allianceauth/timerboard/migrations/0005_alter_timer_planet_moon.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.256349 allianceauth-3.6.0/allianceauth/timerboard/migrations/__init__.py
+-rw-r--r--   0        0        0     1593 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/timerboard/models.py
+-rw-r--r--   0        0        0     1382 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/timerboard/templates/timerboard/form.html
+-rw-r--r--   0        0        0      141 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/timerboard/templates/timerboard/index_button.html
+-rw-r--r--   0        0        0      887 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html
+-rw-r--r--   0        0        0      774 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/timerboard/templates/timerboard/timer_create_form.html
+-rw-r--r--   0        0        0      830 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/timerboard/templates/timerboard/timer_update_form.html
+-rw-r--r--   0        0        0    30990 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/timerboard/templates/timerboard/view.html
+-rw-r--r--   0        0        0     8745 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/timerboard/tests.py
+-rw-r--r--   0        0        0      358 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/timerboard/urls.py
+-rw-r--r--   0        0        0     2897 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/timerboard/views.py
+-rw-r--r--   0        0        0     2567 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/urls.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.256349 allianceauth-3.6.0/allianceauth/utils/__init__.py
+-rw-r--r--   0        0        0      568 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/utils/cache.py
+-rw-r--r--   0        0        0      615 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/utils/django.py
+-rw-r--r--   0        0        0      844 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/utils/testing.py
+-rw-r--r--   0        0        0        0 2023-08-01 12:21:38.257349 allianceauth-3.6.0/allianceauth/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1194 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/utils/tests/test_cache.py
+-rw-r--r--   0        0        0      777 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/utils/tests/test_django.py
+-rw-r--r--   0        0        0      310 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/utils/tests/test_testing.py
+-rw-r--r--   0        0        0     2204 2023-08-01 12:21:38.132351 allianceauth-3.6.0/allianceauth/views.py
+-rw-r--r--   0        0        0     2212 2023-08-01 12:21:38.149351 allianceauth-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7057 1970-01-01 00:00:00.000000 allianceauth-3.6.0/PKG-INFO
```

### Comparing `allianceauth-3.5.1/LICENSE` & `allianceauth-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/PKG-INFO` & `allianceauth-3.6.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,59 @@
 Metadata-Version: 2.1
 Name: allianceauth
-Version: 3.5.1
-Summary: An auth system for EVE Online to help in-game organizations manage online service access.
-Home-page: https://gitlab.com/allianceauth/allianceauth
-Author: Alliance Auth
-Author-email: adarnof@gmail.com
-License: GPL-2.0
-Project-URL: Issue / Bug Reports, https://gitlab.com/allianceauth/allianceauth/-/issues
-Project-URL: Documentation, https://allianceauth.readthedocs.io/
+Version: 3.6.0
+Summary: An auth system for EVE Online to help in-game organizations
 Keywords: allianceauth,eveonline
+Author-email: Alliance Auth <adarnof@gmail.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Requires-Dist: bcrypt
+Requires-Dist: beautifulsoup4
+Requires-Dist: celery-once>=3.0.1
+Requires-Dist: celery>=5.2.0,<6
+Requires-Dist: django-bootstrap-form
+Requires-Dist: django-celery-beat>=2.3.0
+Requires-Dist: django-esi>=4.0.1
+Requires-Dist: django-redis>=5.2.0
+Requires-Dist: django-registration>=3.3,<3.4
+Requires-Dist: django-sortedm2m
+Requires-Dist: django>=4.0.9,<4.1.0
+Requires-Dist: dnspython
+Requires-Dist: mysqlclient>=2.1.0
+Requires-Dist: openfire-restapi
+Requires-Dist: packaging>=21.0
+Requires-Dist: passlib
+Requires-Dist: pydiscourse
+Requires-Dist: python-slugify>=1.2
+Requires-Dist: redis>=4.0.0
+Requires-Dist: requests-oauthlib
+Requires-Dist: requests>=2.9.1
+Requires-Dist: semantic-version
+Requires-Dist: slixmpp
+Requires-Dist: coverage>=4.3.1 ; extra == "test"
+Requires-Dist: django-webtest ; extra == "test"
+Requires-Dist: requests-mock>=1.2.0 ; extra == "test"
+Project-URL: Documentation, https://allianceauth.readthedocs.io/
+Project-URL: Homepage, https://gitlab.com/allianceauth/allianceauth
+Project-URL: Source, https://gitlab.com/allianceauth/allianceauth
+Project-URL: Tracker, https://gitlab.com/allianceauth/allianceauth/-/issues
 Provides-Extra: test
-License-File: LICENSE
 
 # Alliance Auth
 
 [![license](https://img.shields.io/badge/license-GPLv2-green)](https://pypi.org/project/allianceauth/)
 [![python](https://img.shields.io/pypi/pyversions/allianceauth)](https://pypi.org/project/allianceauth/)
 [![django](https://img.shields.io/pypi/djversions/allianceauth?label=django)](https://pypi.org/project/allianceauth/)
 [![version](https://img.shields.io/pypi/v/allianceauth?label=release)](https://pypi.org/project/allianceauth/)
@@ -113,7 +135,8 @@
 Alliance Auth is maintained and developed by the community and we welcome every contribution!
 
 To see what needs to be worked on please review our issue list or chat with our active developers on Discord.
 
 Also, please make sure you have signed the [License Agreement](https://developers.eveonline.com/resource/license-agreement) by logging in at [https://developers.eveonline.com](https://developers.eveonline.com) before submitting any pull requests.
 
 In addition to the core AA system we also very much welcome contributions to our growing list of 3rd party services and plugin apps. Please see [AA Community Creations](https://gitlab.com/allianceauth/community-creations) for details.
+
```

### Comparing `allianceauth-3.5.1/README.md` & `allianceauth-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/admin.py` & `allianceauth-3.6.0/allianceauth/analytics/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/middleware.py` & `allianceauth-3.6.0/allianceauth/analytics/middleware.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/analytics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py` & `allianceauth-3.6.0/allianceauth/analytics/migrations/0002_add_AA_Team_Token.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/migrations/0003_Generate_Identifier.py` & `allianceauth-3.6.0/allianceauth/analytics/migrations/0003_Generate_Identifier.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/migrations/0004_auto_20211015_0502.py` & `allianceauth-3.6.0/allianceauth/analytics/migrations/0004_auto_20211015_0502.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/migrations/0006_more_ignore_paths.py` & `allianceauth-3.6.0/allianceauth/analytics/migrations/0006_more_ignore_paths.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/models.py` & `allianceauth-3.6.0/allianceauth/analytics/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/signals.py` & `allianceauth-3.6.0/allianceauth/analytics/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/tasks.py` & `allianceauth-3.6.0/allianceauth/analytics/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/tests/test_integration.py` & `allianceauth-3.6.0/allianceauth/analytics/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/tests/test_middleware.py` & `allianceauth-3.6.0/allianceauth/analytics/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/tests/test_models.py` & `allianceauth-3.6.0/allianceauth/analytics/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/tests/test_tasks.py` & `allianceauth-3.6.0/allianceauth/analytics/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/tests/test_utils.py` & `allianceauth-3.6.0/allianceauth/analytics/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/analytics/utils.py` & `allianceauth-3.6.0/allianceauth/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/admin.py` & `allianceauth-3.6.0/allianceauth/authentication/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/app_settings.py` & `allianceauth-3.6.0/allianceauth/authentication/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/apps.py` & `allianceauth-3.6.0/allianceauth/authentication/apps.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/backends.py` & `allianceauth-3.6.0/allianceauth/authentication/backends.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/decorators.py` & `allianceauth-3.6.0/allianceauth/authentication/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,43 @@
-from django.conf.urls import include
-from django.contrib.auth.decorators import user_passes_test
-from django.core.exceptions import PermissionDenied
 from functools import wraps
-from django.shortcuts import redirect
+from typing import Callable, Iterable, Optional
+
+from django.urls import include
 from django.contrib import messages
+from django.contrib.auth.decorators import login_required, user_passes_test
+from django.core.exceptions import PermissionDenied
+from django.shortcuts import redirect
 from django.utils.translation import gettext_lazy as _
-from django.contrib.auth.decorators import login_required
 
 
 def user_has_main_character(user):
     return bool(user.profile.main_character)
 
 
-def decorate_url_patterns(urls, decorator):
+def decorate_url_patterns(
+    urls, decorator: Callable, excluded_views: Optional[Iterable] = None
+):
+    """Decorate views given in url patterns except when they are explicitly excluded.
+
+    Args:
+        - urls: Django URL patterns
+        - decorator: Decorator to be added to each view
+        - exclude_views: Optional iterable of view names to be excluded
+    """
     url_list, app_name, namespace = include(urls)
 
     def process_patterns(url_patterns):
         for pattern in url_patterns:
             if hasattr(pattern, 'url_patterns'):
                 # this is an include - apply to all nested patterns
                 process_patterns(pattern.url_patterns)
             else:
                 # this is a pattern
+                if excluded_views and pattern.lookup_str in excluded_views:
+                    return
                 pattern.callback = decorator(pattern.callback)
 
     process_patterns(url_list)
     return url_list, app_name, namespace
 
 
 def main_character_required(view_func):
```

### Comparing `allianceauth-3.5.1/allianceauth/authentication/forms.py` & `allianceauth-3.6.0/allianceauth/authentication/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/hmac_urls.py` & `allianceauth-3.6.0/allianceauth/authentication/hmac_urls.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from django.conf.urls import include
-
 from allianceauth.authentication import views
-from django.urls import re_path
-from django.urls import path
+from django.urls import include, re_path, path
 
 urlpatterns = [
     path('activate/complete/', views.activation_complete, name='registration_activation_complete'),
     # The activation key can make use of any character from the
     # URL-safe base64 alphabet, plus the colon as a separator.
     re_path(r'^activate/(?P<activation_key>[-:\w]+)/$', views.ActivationView.as_view(), name='registration_activate'),
     path('register/', views.RegistrationView.as_view(), name='registration_register'),
```

### Comparing `allianceauth-3.5.1/allianceauth/authentication/management/commands/checkmains.py` & `allianceauth-3.6.0/allianceauth/authentication/management/commands/checkmains.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/managers.py` & `allianceauth-3.6.0/allianceauth/authentication/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/middleware.py` & `allianceauth-3.6.0/allianceauth/authentication/middleware.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0004_create_permissions.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0004_create_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0005_delete_perms.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0005_delete_perms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0006_auto_20160910_0542.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0006_auto_20160910_0542.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0009_auto_20161021_0228.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0009_auto_20161021_0228.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0010_only_one_authservicesinfo.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0011_authservicesinfo_user_onetoonefield.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0012_remove_add_delete_authservicesinfo_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0013_service_modules.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0013_service_modules.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0014_fleetup_permission.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0014_fleetup_permission.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0015_user_profiles.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0015_user_profiles.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0016_ownershiprecord.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0016_ownershiprecord.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0017_remove_fleetup_permission.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0018_state_member_factions.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0018_state_member_factions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0020_userprofile_language_userprofile_night_mode.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/migrations/0021_alter_userprofile_language.py` & `allianceauth-3.6.0/allianceauth/authentication/migrations/0021_alter_userprofile_language.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/models.py` & `allianceauth-3.6.0/allianceauth/authentication/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/signals.py` & `allianceauth-3.6.0/allianceauth/authentication/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg` & `allianceauth-3.6.0/allianceauth/authentication/static/allianceauth/authentication/img/background.jpg`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png` & `allianceauth-3.6.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_Black.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png` & `allianceauth-3.6.0/allianceauth/authentication/static/allianceauth/authentication/img/sso/EVE_SSO_Login_Buttons_Large_White.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/task_statistics/event_series.py` & `allianceauth-3.6.0/allianceauth/authentication/task_statistics/event_series.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Event series for Task Statistics."""
+
 import datetime as dt
 import logging
 from typing import List, Optional
 
 from pytz import utc
 from redis import Redis, RedisError
 
@@ -69,16 +71,16 @@
         """Add event.
 
         Args:
         - event_time: timestamp of event. Will use current time if not specified.
         """
         if not event_time:
             event_time = dt.datetime.utcnow()
-        id = self._redis.incr(self._key_counter)
-        self._redis.zadd(self._key_sorted_set, {id: event_time.timestamp()})
+        my_id = self._redis.incr(self._key_counter)
+        self._redis.zadd(self._key_sorted_set, {my_id: event_time.timestamp()})
 
     def all(self) -> List[dt.datetime]:
         """List of all known events."""
         return [
             event[1]
             for event in self._redis.zrangebyscore(
                 self._key_sorted_set,
@@ -97,28 +99,28 @@
     def count(self, earliest: dt.datetime = None, latest: dt.datetime = None) -> int:
         """Count of events, can be restricted to given timeframe.
 
         Args:
         - earliest: Date of first events to count(inclusive), or -infinite if not specified
         - latest: Date of last events to count(inclusive), or +infinite if not specified
         """
-        min = "-inf" if not earliest else earliest.timestamp()
-        max = "+inf" if not latest else latest.timestamp()
-        return self._redis.zcount(self._key_sorted_set, min=min, max=max)
+        minimum = "-inf" if not earliest else earliest.timestamp()
+        maximum = "+inf" if not latest else latest.timestamp()
+        return self._redis.zcount(self._key_sorted_set, min=minimum, max=maximum)
 
     def first_event(self, earliest: dt.datetime = None) -> Optional[dt.datetime]:
         """Date/Time of first event. Returns `None` if series has no events.
 
         Args:
         - earliest: Date of first events to count(inclusive), or any if not specified
         """
-        min = "-inf" if not earliest else earliest.timestamp()
+        minimum = "-inf" if not earliest else earliest.timestamp()
         event = self._redis.zrangebyscore(
             self._key_sorted_set,
-            min,
+            minimum,
             "+inf",
             withscores=True,
             start=0,
             num=1,
             score_cast_func=self._cast_scores_to_dt,
         )
         if not event:
```

### Comparing `allianceauth-3.5.1/allianceauth/authentication/task_statistics/signals.py` & `allianceauth-3.6.0/allianceauth/authentication/task_statistics/signals.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+"""Signals for Task Statistics."""
+
 from celery.signals import (
-    task_failure,
-    task_internal_error,
-    task_retry,
-    task_success,
-    worker_ready
+    task_failure, task_internal_error, task_postrun, task_prerun, task_retry,
+    task_success, worker_ready,
 )
 
 from django.conf import settings
 
-from .counters import failed_tasks, retried_tasks, succeeded_tasks
+from .counters import (
+    failed_tasks, retried_tasks, running_tasks, succeeded_tasks,
+)
 
 
 def reset_counters():
     """Reset all counters for the celery status."""
     succeeded_tasks.clear()
     failed_tasks.clear()
     retried_tasks.clear()
+    running_tasks.reset()
 
 
 def is_enabled() -> bool:
+    """Return True if task statistics are enabled, else return False."""
     return not bool(
         getattr(settings, "ALLIANCEAUTH_DASHBOARD_TASK_STATISTICS_DISABLED", False)
     )
 
 
 @worker_ready.connect
 def reset_counters_when_celery_restarted(*args, **kwargs):
@@ -48,7 +51,19 @@
         failed_tasks.add()
 
 
 @task_internal_error.connect
 def record_task_internal_error(*args, **kwargs):
     if is_enabled():
         failed_tasks.add()
+
+
+@task_prerun.connect
+def record_task_prerun(*args, **kwargs):
+    if is_enabled():
+        running_tasks.incr()
+
+
+@task_postrun.connect
+def record_task_postrun(*args, **kwargs):
+    if is_enabled():
+        running_tasks.decr()
```

### Comparing `allianceauth-3.5.1/allianceauth/authentication/task_statistics/tests/test_counters.py` & `allianceauth-3.6.0/allianceauth/authentication/task_statistics/tests/test_counters.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,48 +4,57 @@
 from django.utils.timezone import now
 
 from allianceauth.authentication.task_statistics.counters import (
     dashboard_results,
     succeeded_tasks,
     retried_tasks,
     failed_tasks,
+    running_tasks,
 )
 
 
 class TestDashboardResults(TestCase):
-    def test_should_return_counts_for_given_timeframe_only(self):
+    def test_should_return_counts_for_given_time_frame_only(self):
         # given
         earliest_task = now() - dt.timedelta(minutes=15)
+
         succeeded_tasks.clear()
         succeeded_tasks.add(now() - dt.timedelta(hours=1, seconds=1))
         succeeded_tasks.add(earliest_task)
         succeeded_tasks.add()
         succeeded_tasks.add()
+
         retried_tasks.clear()
         retried_tasks.add(now() - dt.timedelta(hours=1, seconds=1))
         retried_tasks.add(now() - dt.timedelta(seconds=30))
         retried_tasks.add()
+
         failed_tasks.clear()
         failed_tasks.add(now() - dt.timedelta(hours=1, seconds=1))
         failed_tasks.add()
+
+        running_tasks.reset(8)
         # when
         results = dashboard_results(hours=1)
         # then
         self.assertEqual(results.succeeded, 3)
         self.assertEqual(results.retried, 2)
         self.assertEqual(results.failed, 1)
         self.assertEqual(results.total, 6)
         self.assertEqual(results.earliest_task, earliest_task)
+        self.assertEqual(results.running, 8)
 
     def test_should_work_with_no_data(self):
         # given
         succeeded_tasks.clear()
         retried_tasks.clear()
         failed_tasks.clear()
+        running_tasks.reset()
         # when
         results = dashboard_results(hours=1)
         # then
         self.assertEqual(results.succeeded, 0)
         self.assertEqual(results.retried, 0)
         self.assertEqual(results.failed, 0)
         self.assertEqual(results.total, 0)
         self.assertIsNone(results.earliest_task)
+        self.assertEqual(results.running, 0)
```

### Comparing `allianceauth-3.5.1/allianceauth/authentication/task_statistics/tests/test_event_series.py` & `allianceauth-3.6.0/allianceauth/authentication/task_statistics/tests/test_event_series.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/task_statistics/tests/test_signals.py` & `allianceauth-3.6.0/allianceauth/authentication/task_statistics/tests/test_signals.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,56 +13,49 @@
     reset_counters,
     is_enabled,
 )
 from allianceauth.eveonline.tasks import update_character
 
 
 @override_settings(
-    CELERY_ALWAYS_EAGER=True,ALLIANCEAUTH_DASHBOARD_TASK_STATISTICS_DISABLED=False
+    CELERY_ALWAYS_EAGER=True, ALLIANCEAUTH_DASHBOARD_TASK_STATISTICS_DISABLED=False
 )
 class TestTaskSignals(TestCase):
     fixtures = ["disable_analytics"]
 
-    def test_should_record_successful_task(self):
-        # given
+    def setUp(self) -> None:
         succeeded_tasks.clear()
         retried_tasks.clear()
         failed_tasks.clear()
+
+    def test_should_record_successful_task(self):
         # when
         with patch(
             "allianceauth.eveonline.tasks.EveCharacter.objects.update_character"
         ) as mock_update:
             mock_update.return_value = None
             update_character.delay(1)
         # then
         self.assertEqual(succeeded_tasks.count(), 1)
         self.assertEqual(retried_tasks.count(), 0)
         self.assertEqual(failed_tasks.count(), 0)
 
     def test_should_record_retried_task(self):
-        # given
-        succeeded_tasks.clear()
-        retried_tasks.clear()
-        failed_tasks.clear()
         # when
         with patch(
             "allianceauth.eveonline.tasks.EveCharacter.objects.update_character"
         ) as mock_update:
             mock_update.side_effect = Retry
             update_character.delay(1)
         # then
         self.assertEqual(succeeded_tasks.count(), 0)
         self.assertEqual(failed_tasks.count(), 0)
         self.assertEqual(retried_tasks.count(), 1)
 
     def test_should_record_failed_task(self):
-        # given
-        succeeded_tasks.clear()
-        retried_tasks.clear()
-        failed_tasks.clear()
         # when
         with patch(
             "allianceauth.eveonline.tasks.EveCharacter.objects.update_character"
         ) as mock_update:
             mock_update.side_effect = RuntimeError
             update_character.delay(1)
         # then
```

### Comparing `allianceauth-3.5.1/allianceauth/authentication/tasks.py` & `allianceauth-3.6.0/allianceauth/authentication/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/templates/authentication/dashboard.html` & `allianceauth-3.6.0/allianceauth/authentication/templates/authentication/dashboard.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/templates/authentication/tokens.html` & `allianceauth-3.6.0/allianceauth/authentication/templates/authentication/tokens.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/templates/public/base.html` & `allianceauth-3.6.0/allianceauth/authentication/templates/public/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/templates/public/lang_select.html` & `allianceauth-3.6.0/allianceauth/authentication/templates/public/lang_select.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/templates/public/middle_box.html` & `allianceauth-3.6.0/allianceauth/authentication/templates/public/middle_box.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/templates/public/register.html` & `allianceauth-3.6.0/allianceauth/authentication/templates/public/register.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/tests/__init__.py` & `allianceauth-3.6.0/allianceauth/authentication/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/tests/test_admin.py` & `allianceauth-3.6.0/allianceauth/authentication/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/tests/test_app_settings.py` & `allianceauth-3.6.0/allianceauth/authentication/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/tests/test_backend.py` & `allianceauth-3.6.0/allianceauth/authentication/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/tests/test_commands.py` & `allianceauth-3.6.0/allianceauth/authentication/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/tests/test_decorators.py` & `allianceauth-3.6.0/allianceauth/tests/test_urls.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,72 @@
-from unittest import mock
-from urllib import parse
-
-from django.conf import settings
-from django.contrib.auth.models import AnonymousUser
-from django.http.response import HttpResponse
-from django.shortcuts import reverse
-from django.test import TestCase
-from django.test.client import RequestFactory
-
-from allianceauth.eveonline.models import EveCharacter
-from allianceauth.tests.auth_utils import AuthUtils
-
-from ..decorators import main_character_required
-from ..models import CharacterOwnership
-
-
-MODULE_PATH = 'allianceauth.authentication'
-
-
-class DecoratorTestCase(TestCase):
-    @staticmethod
-    @main_character_required
-    def dummy_view(*args, **kwargs):
-        return HttpResponse(status=200)
-
-    @classmethod
-    def setUpTestData(cls):
-        cls.main_user = AuthUtils.create_user('main_user', disconnect_signals=True)
-        cls.no_main_user = AuthUtils.create_user(
-            'no_main_user', disconnect_signals=True
-        )
-        main_character = EveCharacter.objects.create(
-            character_id=1,
-            character_name='Main Character',
-            corporation_id=1,
-            corporation_name='Corp',
-            corporation_ticker='CORP',
-        )
-        CharacterOwnership.objects.create(
-            user=cls.main_user, character=main_character, owner_hash='1'
-        )
-        cls.main_user.profile.main_character = main_character
-
-    def setUp(self):
-        self.request = RequestFactory().get('/test/')
-
-    @mock.patch(MODULE_PATH + '.decorators.messages')
-    def test_login_redirect(self, m):
-        setattr(self.request, 'user', AnonymousUser())
-        response = self.dummy_view(self.request)
-        self.assertEqual(response.status_code, 302)
-        url = getattr(response, 'url', None)
-        self.assertEqual(parse.urlparse(url).path, reverse(settings.LOGIN_URL))
-
-    @mock.patch(MODULE_PATH + '.decorators.messages')
-    def test_main_character_redirect(self, m):
-        setattr(self.request, 'user', self.no_main_user)
-        response = self.dummy_view(self.request)
-        self.assertEqual(response.status_code, 302)
-        url = getattr(response, 'url', None)
-        self.assertEqual(url, reverse('authentication:dashboard'))
-
-    @mock.patch(MODULE_PATH + '.decorators.messages')
-    def test_successful_request(self, m):
-        setattr(self.request, 'user', self.main_user)
-        response = self.dummy_view(self.request)
-        self.assertEqual(response.status_code, 200)
+from unittest import TestCase
+from unittest.mock import patch, MagicMock
+from django.urls import URLPattern
+
+from allianceauth.services.hooks import UrlHook
+from allianceauth.urls import urls_from_apps
+
+MODULE_PATH = "allianceauth.urls"
+
+
+@patch(MODULE_PATH + ".main_character_required")
+@patch(MODULE_PATH + ".decorate_url_patterns")
+class TestUrlsFromApps(TestCase):
+    def test_should_decorate_url_by_default(self, mock_decorate_url_patterns, mock_main_character_required):
+        # given
+        def hook_function():
+            return UrlHook(urlconf_module, "my_namespace", r"^my_app/")
+
+        view = MagicMock(name="view")
+        path = MagicMock(spec=URLPattern, name="path")
+        path.callback = view
+        urlconf_module = [patch], "my_app"
+        # when
+        result = urls_from_apps([hook_function], [])
+        # then
+        self.assertIsInstance(result[0], URLPattern)
+        self.assertTrue(mock_decorate_url_patterns.called)
+        args, _ = mock_decorate_url_patterns.call_args
+        decorator = args[1]
+        self.assertEqual(decorator, mock_main_character_required)
+        excluded_views = args[2]
+        self.assertIsNone(excluded_views)
+
+    def test_should_not_decorate_when_excluded(self, mock_decorate_url_patterns, mock_main_character_required):
+        # given
+        def hook_function():
+            return UrlHook(urlconf_module, "my_namespace", r"^my_app/", ["excluded_view"])
+
+        view = MagicMock(name="view")
+        path = MagicMock(spec=URLPattern, name="path")
+        path.callback = view
+        urlconf_module = [patch], "my_app"
+        # when
+        result = urls_from_apps([hook_function], ["my_app"])
+        # then
+        self.assertIsInstance(result[0], URLPattern)
+        self.assertTrue(mock_decorate_url_patterns.called)
+        args, _ = mock_decorate_url_patterns.call_args
+        decorator = args[1]
+        self.assertEqual(decorator, mock_main_character_required)
+        excluded_views = args[2]
+        self.assertSetEqual(excluded_views, {"excluded_view"})
+
+    def test_should_decorate_when_app_has_no_permission(self, mock_decorate_url_patterns, mock_main_character_required):
+        # given
+        def hook_function():
+            return UrlHook(urlconf_module, "my_namespace", r"^my_app/", ["excluded_view"])
+
+        view = MagicMock(name="view")
+        path = MagicMock(spec=URLPattern, name="path")
+        path.callback = view
+        urlconf_module = [patch], "my_app"
+        # when
+        result = urls_from_apps([hook_function], ["other_app"])
+        # then
+        self.assertIsInstance(result[0], URLPattern)
+        self.assertTrue(mock_decorate_url_patterns.called)
+        args, _ = mock_decorate_url_patterns.call_args
+        decorator = args[1]
+        self.assertEqual(decorator, mock_main_character_required)
+        excluded_views = args[2]
+        self.assertIsNone(excluded_views)
```

### Comparing `allianceauth-3.5.1/allianceauth/authentication/tests/test_middleware.py` & `allianceauth-3.6.0/allianceauth/authentication/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/tests/test_models.py` & `allianceauth-3.6.0/allianceauth/authentication/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/tests/test_signals.py` & `allianceauth-3.6.0/allianceauth/authentication/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/tests/test_templatetags.py` & `allianceauth-3.6.0/allianceauth/authentication/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/urls.py` & `allianceauth-3.6.0/allianceauth/authentication/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/authentication/views.py` & `allianceauth-3.6.0/allianceauth/authentication/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/bin/allianceauth.py` & `allianceauth-3.6.0/allianceauth/bin/allianceauth.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/corputils/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/managers.py` & `allianceauth-3.6.0/allianceauth/corputils/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/corputils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/migrations/0002_migrate_permissions.py` & `allianceauth-3.6.0/allianceauth/corputils/migrations/0002_migrate_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/migrations/0003_granular_permissions.py` & `allianceauth-3.6.0/allianceauth/corputils/migrations/0003_granular_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/migrations/0004_member_models.py` & `allianceauth-3.6.0/allianceauth/corputils/migrations/0004_member_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/migrations/0005_cleanup_permissions.py` & `allianceauth-3.6.0/allianceauth/corputils/migrations/0005_cleanup_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/models.py` & `allianceauth-3.6.0/allianceauth/corputils/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/swagger.json` & `allianceauth-3.6.0/allianceauth/corputils/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/templates/corputils/base.html` & `allianceauth-3.6.0/allianceauth/corputils/templates/corputils/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/templates/corputils/corpstats.html` & `allianceauth-3.6.0/allianceauth/corputils/templates/corputils/corpstats.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/templates/corputils/search.html` & `allianceauth-3.6.0/allianceauth/corputils/templates/corputils/search.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/tests.py` & `allianceauth-3.6.0/allianceauth/corputils/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/corputils/views.py` & `allianceauth-3.6.0/allianceauth/corputils/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/admin.py` & `allianceauth-3.6.0/allianceauth/eveonline/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/autogroups/admin.py` & `allianceauth-3.6.0/allianceauth/eveonline/autogroups/admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 def sync_user_groups(modeladmin, request, queryset):
     for agc in queryset:
         logger.debug(f"update_all_states_group_membership for {agc}")
         agc.update_all_states_group_membership()
 
 
+@admin.register(AutogroupsConfig)
 class AutogroupsConfigAdmin(admin.ModelAdmin):
     formfield_overrides = {
         models.CharField: {'strip': False}
     }
 
     def get_readonly_fields(self, request, obj=None):
         if obj:  # This is the case when obj is already created i.e. it's an edit
@@ -32,10 +33,9 @@
         actions = super().get_actions(request)
         actions['sync_user_groups'] = (sync_user_groups,
                                         'sync_user_groups',
                                         'Sync all users groups for this Autogroup Config')
         return actions
 
 
-admin.site.register(AutogroupsConfig, AutogroupsConfigAdmin)
 admin.site.register(ManagedCorpGroup)
 admin.site.register(ManagedAllianceGroup)
```

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/autogroups/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/eveonline/autogroups/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/autogroups/models.py` & `allianceauth-3.6.0/allianceauth/eveonline/autogroups/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/autogroups/signals.py` & `allianceauth-3.6.0/allianceauth/eveonline/autogroups/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/autogroups/tests/__init__.py` & `allianceauth-3.6.0/allianceauth/eveonline/autogroups/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/autogroups/tests/test_managers.py` & `allianceauth-3.6.0/allianceauth/eveonline/autogroups/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/autogroups/tests/test_models.py` & `allianceauth-3.6.0/allianceauth/eveonline/autogroups/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/autogroups/tests/test_signals.py` & `allianceauth-3.6.0/allianceauth/eveonline/autogroups/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/evelinks/__init__.py` & `allianceauth-3.6.0/allianceauth/eveonline/evelinks/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/evelinks/dotlan.py` & `allianceauth-3.6.0/allianceauth/eveonline/evelinks/dotlan.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/evelinks/eveimageserver.py` & `allianceauth-3.6.0/allianceauth/eveonline/evelinks/eveimageserver.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/evelinks/evewho.py` & `allianceauth-3.6.0/allianceauth/eveonline/evelinks/evewho.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/evelinks/tests/test_evelinks.py` & `allianceauth-3.6.0/allianceauth/eveonline/evelinks/tests/test_evelinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/evelinks/tests/test_templatetags.py` & `allianceauth-3.6.0/allianceauth/eveonline/evelinks/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/evelinks/zkillboard.py` & `allianceauth-3.6.0/allianceauth/eveonline/evelinks/zkillboard.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/managers.py` & `allianceauth-3.6.0/allianceauth/eveonline/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/eveonline/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py` & `allianceauth-3.6.0/allianceauth/eveonline/migrations/0003_auto_20161026_0149.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py` & `allianceauth-3.6.0/allianceauth/eveonline/migrations/0006_allow_null_evecharacter_alliance.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/migrations/0007_unique_id_name.py` & `allianceauth-3.6.0/allianceauth/eveonline/migrations/0007_unique_id_name.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/migrations/0008_remove_apikeys.py` & `allianceauth-3.6.0/allianceauth/eveonline/migrations/0008_remove_apikeys.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/migrations/0009_on_delete.py` & `allianceauth-3.6.0/allianceauth/eveonline/migrations/0009_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/migrations/0010_alliance_ticker.py` & `allianceauth-3.6.0/allianceauth/eveonline/migrations/0010_alliance_ticker.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/migrations/0011_ids_to_integers.py` & `allianceauth-3.6.0/allianceauth/eveonline/migrations/0011_ids_to_integers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/migrations/0012_index_additions.py` & `allianceauth-3.6.0/allianceauth/eveonline/migrations/0012_index_additions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/migrations/0015_factions.py` & `allianceauth-3.6.0/allianceauth/eveonline/migrations/0015_factions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py` & `allianceauth-3.6.0/allianceauth/eveonline/migrations/0017_alliance_and_corp_names_are_not_unique.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/models.py` & `allianceauth-3.6.0/allianceauth/eveonline/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/providers.py` & `allianceauth-3.6.0/allianceauth/eveonline/providers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/swagger.json` & `allianceauth-3.6.0/allianceauth/eveonline/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/tasks.py` & `allianceauth-3.6.0/allianceauth/eveonline/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/templatetags/evelinks.py` & `allianceauth-3.6.0/allianceauth/eveonline/templatetags/evelinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/templatetags/examples.html` & `allianceauth-3.6.0/allianceauth/eveonline/templatetags/examples.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/tests/__init__.py` & `allianceauth-3.6.0/allianceauth/eveonline/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/tests/esi_client_stub.py` & `allianceauth-3.6.0/allianceauth/eveonline/tests/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/tests/swagger_old.json` & `allianceauth-3.6.0/allianceauth/eveonline/tests/swagger_old.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/tests/test_managers.py` & `allianceauth-3.6.0/allianceauth/eveonline/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/tests/test_models.py` & `allianceauth-3.6.0/allianceauth/eveonline/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/tests/test_providers.py` & `allianceauth-3.6.0/allianceauth/eveonline/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/eveonline/tests/test_tasks.py` & `allianceauth-3.6.0/allianceauth/eveonline/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/fleetactivitytracking/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/fleetactivitytracking/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/fleetactivitytracking/models.py` & `allianceauth-3.6.0/allianceauth/fleetactivitytracking/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/fleetactivitytracking/swagger.json` & `allianceauth-3.6.0/allianceauth/fleetactivitytracking/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html` & `allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/characternotexisting.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkformatter.html` & `allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkformatter.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html` & `allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkmodify.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html` & `allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalmonthlystatisticsview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html` & `allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkpersonalstatisticsview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html` & `allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticscorpview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html` & `allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkstatisticsview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html` & `allianceauth-3.6.0/allianceauth/fleetactivitytracking/templates/fleetactivitytracking/fatlinkview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/fleetactivitytracking/urls.py` & `allianceauth-3.6.0/allianceauth/fleetactivitytracking/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/fleetactivitytracking/views.py` & `allianceauth-3.6.0/allianceauth/fleetactivitytracking/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/admin.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/forms.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/managers.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0002_auto_20160906_2354.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0004_authgroup.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0004_authgroup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0005_authgroup_public.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0005_authgroup_public.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0006_request_groups_perm.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0007_on_delete.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0007_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0008_remove_authgroup_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0009_requestlog.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0009_requestlog.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0010_authgroup_states.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0010_authgroup_states.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0012_group_leads.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0012_group_leads.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0015_make_descriptions_great_again.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0017_improve_groups_documentation.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0018_reservedgroupname.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/migrations/0019_adding_restricted_to_groups.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/models.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/signals.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/templates/groupmanagement/audit.html` & `allianceauth-3.6.0/allianceauth/groupmanagement/templates/groupmanagement/audit.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html` & `allianceauth-3.6.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembers.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html` & `allianceauth-3.6.0/allianceauth/groupmanagement/templates/groupmanagement/groupmembership.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/templates/groupmanagement/groups.html` & `allianceauth-3.6.0/allianceauth/groupmanagement/templates/groupmanagement/groups.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/templates/groupmanagement/index.html` & `allianceauth-3.6.0/allianceauth/groupmanagement/templates/groupmanagement/index.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/templates/groupmanagement/menu.html` & `allianceauth-3.6.0/allianceauth/groupmanagement/templates/groupmanagement/menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/tests/test_admin.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/tests/test_managers.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/tests/test_models.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/tests/test_signals.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/tests/test_views.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/urls.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/groupmanagement/views.py` & `allianceauth-3.6.0/allianceauth/groupmanagement/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hooks.py` & `allianceauth-3.6.0/allianceauth/hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/admin.py` & `allianceauth-3.6.0/allianceauth/hrapplications/admin.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 class ChoiceInline(admin.TabularInline):
     model = ApplicationChoice
     extra = 0
     verbose_name_plural = 'Choices (optional)'
     verbose_name= 'Choice'
 
+@admin.register(ApplicationQuestion)
 class QuestionAdmin(admin.ModelAdmin):
     fieldsets = [
             (None,      {'fields': ['title', 'help_text', 'multi_select']}),
             ]
     inlines = [ChoiceInline]
 
 admin.site.register(Application)
 admin.site.register(ApplicationComment)
-admin.site.register(ApplicationQuestion, QuestionAdmin)
 admin.site.register(ApplicationForm)
 admin.site.register(ApplicationResponse)
```

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/hrapplications/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/managers.py` & `allianceauth-3.6.0/allianceauth/hrapplications/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/hrapplications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/migrations/0002_choices_for_questions.py` & `allianceauth-3.6.0/allianceauth/hrapplications/migrations/0002_choices_for_questions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py` & `allianceauth-3.6.0/allianceauth/hrapplications/migrations/0004_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/migrations/0005_sorted_questions.py` & `allianceauth-3.6.0/allianceauth/hrapplications/migrations/0005_sorted_questions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py` & `allianceauth-3.6.0/allianceauth/hrapplications/migrations/0006_remove_legacy_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/models.py` & `allianceauth-3.6.0/allianceauth/hrapplications/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/templates/hrapplications/corpchoice.html` & `allianceauth-3.6.0/allianceauth/hrapplications/templates/hrapplications/corpchoice.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/templates/hrapplications/create.html` & `allianceauth-3.6.0/allianceauth/hrapplications/templates/hrapplications/create.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/templates/hrapplications/management.html` & `allianceauth-3.6.0/allianceauth/hrapplications/templates/hrapplications/management.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/templates/hrapplications/searchview.html` & `allianceauth-3.6.0/allianceauth/hrapplications/templates/hrapplications/searchview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/templates/hrapplications/view.html` & `allianceauth-3.6.0/allianceauth/hrapplications/templates/hrapplications/view.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/tests.py` & `allianceauth-3.6.0/allianceauth/hrapplications/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/urls.py` & `allianceauth-3.6.0/allianceauth/hrapplications/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/hrapplications/views.py` & `allianceauth-3.6.0/allianceauth/hrapplications/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/de/LC_MESSAGES/django.mo` & `allianceauth-3.6.0/allianceauth/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/de/LC_MESSAGES/django.po` & `allianceauth-3.6.0/allianceauth/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/en/LC_MESSAGES/django.po` & `allianceauth-3.6.0/allianceauth/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/es/LC_MESSAGES/django.mo` & `allianceauth-3.6.0/allianceauth/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/es/LC_MESSAGES/django.po` & `allianceauth-3.6.0/allianceauth/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo` & `allianceauth-3.6.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/fr_FR/LC_MESSAGES/django.po` & `allianceauth-3.6.0/allianceauth/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/it_IT/LC_MESSAGES/django.mo` & `allianceauth-3.6.0/allianceauth/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/it_IT/LC_MESSAGES/django.po` & `allianceauth-3.6.0/allianceauth/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/ja/LC_MESSAGES/django.mo` & `allianceauth-3.6.0/allianceauth/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/ja/LC_MESSAGES/django.po` & `allianceauth-3.6.0/allianceauth/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo` & `allianceauth-3.6.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/ko_KR/LC_MESSAGES/django.po` & `allianceauth-3.6.0/allianceauth/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/ru/LC_MESSAGES/django.mo` & `allianceauth-3.6.0/allianceauth/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/ru/LC_MESSAGES/django.po` & `allianceauth-3.6.0/allianceauth/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/uk/LC_MESSAGES/django.mo` & `allianceauth-3.6.0/allianceauth/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/uk/LC_MESSAGES/django.po` & `allianceauth-3.6.0/allianceauth/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo` & `allianceauth-3.6.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po` & `allianceauth-3.6.0/allianceauth/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/admin.py` & `allianceauth-3.6.0/allianceauth/notifications/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,25 +11,29 @@
         "timestamp",
         "user__profile__state",
         ('user__profile__main_character', admin.RelatedOnlyFieldListFilter),
     )
     ordering = ("-timestamp", )
     search_fields = ["user__username", "user__profile__main_character__character_name"]
 
+    @admin.display(
+        ordering="user__profile__main_character__character_name"
+    )
     def _main(self, obj):
         try:
             return obj.user.profile.main_character
         except AttributeError:
             return obj.user
 
-    _main.admin_order_field = "user__profile__main_character__character_name"
 
+    @admin.display(
+        ordering="user__profile__state__name"
+    )
     def _state(self, obj):
         return obj.user.profile.state
 
-    _state.admin_order_field = "user__profile__state__name"
 
     def has_change_permission(self, request, obj=None):
         return False
 
     def has_add_permission(self, request) -> bool:
         return False
```

### Comparing `allianceauth-3.5.1/allianceauth/notifications/core.py` & `allianceauth-3.6.0/allianceauth/notifications/core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/handlers.py` & `allianceauth-3.6.0/allianceauth/notifications/handlers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/managers.py` & `allianceauth-3.6.0/allianceauth/notifications/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py` & `allianceauth-3.6.0/allianceauth/notifications/migrations/0003_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/migrations/0004_performance_tuning.py` & `allianceauth-3.6.0/allianceauth/notifications/migrations/0004_performance_tuning.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/migrations/0005_fix_level_choices.py` & `allianceauth-3.6.0/allianceauth/notifications/migrations/0005_fix_level_choices.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/models.py` & `allianceauth-3.6.0/allianceauth/notifications/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/templates/notifications/list.html` & `allianceauth-3.6.0/allianceauth/notifications/templates/notifications/list.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/templates/notifications/list_partial.html` & `allianceauth-3.6.0/allianceauth/notifications/templates/notifications/list_partial.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/templates/notifications/view.html` & `allianceauth-3.6.0/allianceauth/notifications/templates/notifications/view.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/templatetags/auth_notifications.py` & `allianceauth-3.6.0/allianceauth/notifications/templatetags/auth_notifications.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/tests/test_core.py` & `allianceauth-3.6.0/allianceauth/notifications/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/tests/test_handlers.py` & `allianceauth-3.6.0/allianceauth/notifications/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/tests/test_init.py` & `allianceauth-3.6.0/allianceauth/notifications/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/tests/test_managers.py` & `allianceauth-3.6.0/allianceauth/notifications/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/tests/test_models.py` & `allianceauth-3.6.0/allianceauth/notifications/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/tests/test_templatetags.py` & `allianceauth-3.6.0/allianceauth/notifications/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/tests/test_views.py` & `allianceauth-3.6.0/allianceauth/notifications/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/urls.py` & `allianceauth-3.6.0/allianceauth/notifications/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/notifications/views.py` & `allianceauth-3.6.0/allianceauth/notifications/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/optimer/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/optimer/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/optimer/form.py` & `allianceauth-3.6.0/allianceauth/optimer/form.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/optimer/form_widgets.py` & `allianceauth-3.6.0/allianceauth/optimer/form_widgets.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/optimer/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/optimer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py` & `allianceauth-3.6.0/allianceauth/optimer/migrations/0003_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/optimer/migrations/0005_add_type_and_description.py` & `allianceauth-3.6.0/allianceauth/optimer/migrations/0005_add_type_and_description.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/optimer/models.py` & `allianceauth-3.6.0/allianceauth/optimer/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/optimer/templates/optimer/add.html` & `allianceauth-3.6.0/allianceauth/optimer/templates/optimer/add.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/optimer/templates/optimer/fleetoptable.html` & `allianceauth-3.6.0/allianceauth/optimer/templates/optimer/fleetoptable.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/optimer/templates/optimer/management.html` & `allianceauth-3.6.0/allianceauth/optimer/templates/optimer/management.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/optimer/templates/optimer/update.html` & `allianceauth-3.6.0/allianceauth/optimer/templates/optimer/update.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/optimer/views.py` & `allianceauth-3.6.0/allianceauth/optimer/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/permissions_tool/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/permissions_tool/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/permissions_tool/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/permissions_tool/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/permissions_tool/templates/permissions_tool/audit.html` & `allianceauth-3.6.0/allianceauth/permissions_tool/templates/permissions_tool/audit.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html` & `allianceauth-3.6.0/allianceauth/permissions_tool/templates/permissions_tool/audit_row.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/permissions_tool/templates/permissions_tool/overview.html` & `allianceauth-3.6.0/allianceauth/permissions_tool/templates/permissions_tool/overview.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/permissions_tool/tests.py` & `allianceauth-3.6.0/allianceauth/permissions_tool/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/permissions_tool/views.py` & `allianceauth-3.6.0/allianceauth/permissions_tool/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/project_template/manage.py` & `allianceauth-3.6.0/allianceauth/project_template/manage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/project_template/project_name/celery.py` & `allianceauth-3.6.0/allianceauth/project_template/project_name/celery.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/project_template/project_name/settings/base.py` & `allianceauth-3.6.0/allianceauth/project_template/project_name/settings/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,31 +37,31 @@
 
 # Celery configuration
 BROKER_URL = 'redis://localhost:6379/0'
 CELERYBEAT_SCHEDULER = "django_celery_beat.schedulers.DatabaseScheduler"
 CELERYBEAT_SCHEDULE = {
     'esi_cleanup_callbackredirect': {
         'task': 'esi.tasks.cleanup_callbackredirect',
-        'schedule': crontab(minute=0, hour='*/4'),
+        'schedule': crontab(minute='0', hour='*/4'),
     },
     'esi_cleanup_token': {
         'task': 'esi.tasks.cleanup_token',
-        'schedule': crontab(minute=0, hour=0),
+        'schedule': crontab(minute='0', hour='0'),
     },
     'run_model_update': {
         'task': 'allianceauth.eveonline.tasks.run_model_update',
-        'schedule': crontab(minute=0, hour="*/6"),
+        'schedule': crontab(minute='0', hour="*/6"),
     },
     'check_all_character_ownership': {
         'task': 'allianceauth.authentication.tasks.check_all_character_ownership',
-        'schedule': crontab(minute=0, hour='*/4'),
+        'schedule': crontab(minute='0', hour='*/4'),
     },
     'analytics_daily_stats': {
         'task': 'allianceauth.analytics.tasks.analytics_daily_stats',
-        'schedule': crontab(minute=0, hour=2),
+        'schedule': crontab(minute='0', hour='2'),
     }
 }
 
 # Build paths inside the project like this: os.path.join(BASE_DIR, ...)
 PROJECT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 BASE_DIR = os.path.dirname(PROJECT_DIR)
```

### Comparing `allianceauth-3.5.1/allianceauth/project_template/project_name/settings/local.py` & `allianceauth-3.6.0/allianceauth/project_template/project_name/settings/local.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,18 @@
 INSTALLED_APPS += [
 
 ]
 
 # To change the logging level for extensions, uncomment the following line.
 # LOGGING['handlers']['extension_file']['level'] = 'DEBUG'
 
+# By default apps are prevented from having public views for security reasons.
+# If you want to allow specific apps to have public views
+# you can put there names here (same name as in INSTALLED_APPS):
+APPS_WITH_PUBLIC_VIEWS = []
 
 # Enter credentials to use MySQL/MariaDB. Comment out to use sqlite3
 DATABASES['default'] = {
     'ENGINE': 'django.db.backends.mysql',
     'NAME': 'alliance_auth',
     'USER': '',
     'PASSWORD': '',
```

### Comparing `allianceauth-3.5.1/allianceauth/project_template/supervisor.conf` & `allianceauth-3.6.0/allianceauth/project_template/supervisor.conf`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/abstract.py` & `allianceauth-3.6.0/allianceauth/services/abstract.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/admin.py` & `allianceauth-3.6.0/allianceauth/services/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -62,10 +62,12 @@
 
 
 @admin.register(NameFormatConfig)
 class NameFormatConfigAdmin(admin.ModelAdmin):
     form = NameFormatConfigForm
     list_display = ('service_name', 'get_state_display_string')
 
+    @admin.display(
+        description='States'
+    )
     def get_state_display_string(self, obj):
         return ', '.join([state.name for state in obj.states.all()])
-    get_state_display_string.short_description = 'States'
```

### Comparing `allianceauth-3.5.1/allianceauth/services/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/services/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/forms.py` & `allianceauth-3.6.0/allianceauth/services/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/hooks.py` & `allianceauth-3.6.0/allianceauth/services/hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from django.conf.urls import include
-from django.urls import re_path
+from string import Formatter
+from typing import Iterable, Optional
+
+from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from django.template.loader import render_to_string
+from django.urls import include, re_path
 from django.utils.functional import cached_property
-from django.conf import settings
-from string import Formatter
 
 from allianceauth.hooks import get_hooks
 
 from .models import NameFormatConfig
 
+
 def get_extension_logger(name):
     """
     Takes the name of a plugin/extension and generates a child logger of the extensions logger
     to be used by the extension to log events to the extensions logger.
 
     The logging level is determined by the level defined for the parent logger.
 
@@ -152,16 +154,40 @@
     def render(self, request):
         return render_to_string(self.template,
                                 {'item': self},
                                 request=request)
 
 
 class UrlHook:
-    def __init__(self, urls, namespace, base_url):
+    """A hook for registering the URLs of a Django app.
+
+    Args:
+        - urls: The urls module to include
+        - namespace: The URL namespace to apply. This is usually just the app name.
+        - base_url: The URL prefix to match against in regex form.
+            Example ``r'^app_name/'``.
+            This prefix will be applied in front of all URL patterns included.
+            It is possible to use the same prefix as existing apps (or no prefix at all),
+            but standard URL resolution ordering applies
+            (hook URLs are the last ones registered).
+        - excluded_views: Optional list of views to be excluded
+            from auto-decorating them with the
+            default ``main_character_required`` decorator, e.g. to make them public.
+            Views must be specified by their qualified name,
+            e.g. ``["example.views.my_public_view"]``
+    """
+    def __init__(
+            self,
+            urls,
+            namespace: str,
+            base_url: str,
+            excluded_views : Optional[Iterable[str]] = None
+    ):
         self.include_pattern = re_path(base_url, include(urls, namespace=namespace))
+        self.excluded_views = set(excluded_views or [])
 
 
 class NameFormatter:
     DEFAULT_FORMAT = getattr(settings, "DEFAULT_SERVICE_NAME_FORMAT", '[{corp_ticker}] {character_name}')
 
     def __init__(self, service, user):
         """
```

### Comparing `allianceauth-3.5.1/allianceauth/services/migrations/0002_nameformatter.py` & `allianceauth-3.6.0/allianceauth/services/migrations/0002_nameformatter.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/migrations/0003_remove_broken_link.py` & `allianceauth-3.6.0/allianceauth/services/migrations/0003_remove_broken_link.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/models.py` & `allianceauth-3.6.0/allianceauth/services/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/admin.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/api.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/api.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/app_settings.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/core.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/app_settings.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/client.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -584,24 +584,25 @@
         - None if user is not a member of the guild
         """
         member_info = self.guild_member(guild_id=guild_id, user_id=user_id)
         if member_info is None:
             return None  # User is no longer a member
         guild_roles = RolesSet(self.guild_roles(guild_id=guild_id))
         logger.debug('Current guild roles: %s', guild_roles.ids())
+        _roles = set(member_info.roles)
         if not guild_roles.has_roles(member_info.roles):
             guild_roles = RolesSet(
                 self.guild_roles(guild_id=guild_id, use_cache=False)
             )
             if not guild_roles.has_roles(member_info.roles):
                 role_ids = set(member_info.roles).difference(guild_roles.ids())
-                raise RuntimeError(
-                    f'Discord user {user_id} has unknown roles: {role_ids}'
-                )
-        return guild_roles.subset(member_info.roles)
+                logger.warning(f'Discord user {user_id} has unknown roles: {role_ids}')
+                for _r in role_ids:
+                    _roles.remove(_r)
+        return guild_roles.subset(_roles)
 
     @classmethod
     def _is_member_unknown_error(cls, r: requests.Response) -> bool:
         try:
             result = (
                 r.status_code == HTTPStatus.NOT_FOUND
                 and r.json()['code'] == DiscordApiStatusCode.UNKNOWN_MEMBER
```

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/exceptions.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/helpers.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/models.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/example_objects.json` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/example_objects.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/factories.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/factories.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/piloting_concurrency.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/piloting_functionality.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/rate_limits.md`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/test_client.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -895,16 +895,16 @@
         # given
         role_a = create_role(id=1)
         role_b = create_role(id=2)
         mock_guild_member.return_value = create_guild_member(roles=[1, 99])
         mock_guild_roles.return_value = {role_a, role_b}
         client = DiscordClientStub(TEST_BOT_TOKEN, mock_redis)
         # when/then
-        with self.assertRaises(RuntimeError):
-            client.guild_member_roles(TEST_GUILD_ID, TEST_USER_ID)
+        roles = client.guild_member_roles(TEST_GUILD_ID, TEST_USER_ID)
+        self.assertEqual(roles, RolesSet([role_a]))
 
     # TODO: Re-enable after adding Discord general error handling
     # def test_should_raise_exception_if_member_info_is_invalid(
     #     self, mock_guild_member, mock_guild_roles
     # ):
     #     # given
     #     member_info = create_guild_member(roles=[1])
```

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/discord_client/tests/test_models.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/discord_client/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/managers.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/migrations/0002_service_permissions.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/migrations/0003_big_overhaul.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/models.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/tasks.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html` & `allianceauth-3.6.0/allianceauth/services/modules/discord/templates/services/discord/discord_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/tests/factories.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/tests/factories.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/tests/piloting_tasks.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/tests/piloting_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_admin.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_api.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_auth_hooks.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_core.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_integration.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_managers.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_models.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_tasks.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_utils.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/tests/test_views.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/urls.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/urls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from django.conf.urls import include
-from django.urls import path
+from django.urls import include, path
 
 from . import views
 
 app_name = 'discord'
 
 module_urls = [
     # Discord Service Control
```

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/utils.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discord/views.py` & `allianceauth-3.6.0/allianceauth/services/modules/discord/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discourse/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/services/modules/discourse/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discourse/manager.py` & `allianceauth-3.6.0/allianceauth/services/modules/discourse/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discourse/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/services/modules/discourse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py` & `allianceauth-3.6.0/allianceauth/services/modules/discourse/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discourse/models.py` & `allianceauth-3.6.0/allianceauth/services/modules/discourse/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discourse/providers.py` & `allianceauth-3.6.0/allianceauth/services/modules/discourse/providers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discourse/tasks.py` & `allianceauth-3.6.0/allianceauth/services/modules/discourse/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discourse/tests.py` & `allianceauth-3.6.0/allianceauth/services/modules/discourse/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/discourse/views.py` & `allianceauth-3.6.0/allianceauth/services/modules/discourse/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/example/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/services/modules/example/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/ips4/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/services/modules/ips4/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/ips4/manager.py` & `allianceauth-3.6.0/allianceauth/services/modules/ips4/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/ips4/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/services/modules/ips4/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py` & `allianceauth-3.6.0/allianceauth/services/modules/ips4/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/ips4/models.py` & `allianceauth-3.6.0/allianceauth/services/modules/ips4/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/ips4/tasks.py` & `allianceauth-3.6.0/allianceauth/services/modules/ips4/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/ips4/tests.py` & `allianceauth-3.6.0/allianceauth/services/modules/ips4/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/ips4/views.py` & `allianceauth-3.6.0/allianceauth/services/modules/ips4/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0001_squashed_0011_auto_20201011_1009.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0003_mumbleuser_user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0004_auto_20161214_1024.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0005_mumbleuser_hashfn.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0006_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0007_not_null_user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0009_set_mumble_dissplay_names.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0010_mumbleuser_certhash.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/migrations/0012_mumble_client_info.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/models.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/tasks.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/templates/services/mumble/mumble_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/tests.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/urls.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/urls.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from django.conf.urls import include
-from django.urls import path
+from django.urls import include, path
 
 from . import views
 
 app_name = 'mumble'
 
 module_urls = [
     # Mumble service control
```

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/mumble/views.py` & `allianceauth-3.6.0/allianceauth/services/modules/mumble/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/openfire/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/services/modules/openfire/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/openfire/manager.py` & `allianceauth-3.6.0/allianceauth/services/modules/openfire/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/openfire/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/services/modules/openfire/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py` & `allianceauth-3.6.0/allianceauth/services/modules/openfire/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/openfire/tasks.py` & `allianceauth-3.6.0/allianceauth/services/modules/openfire/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html` & `allianceauth-3.6.0/allianceauth/services/modules/openfire/templates/services/openfire/broadcast.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/openfire/tests.py` & `allianceauth-3.6.0/allianceauth/services/modules/openfire/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/openfire/urls.py` & `allianceauth-3.6.0/allianceauth/services/modules/openfire/urls.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from django.conf.urls import include
-from django.urls import path
+from django.urls import include, path
 
 from . import views
 
 app_name = 'openfire'
 
 module_urls = [
     # Jabber Service Control
```

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/openfire/views.py` & `allianceauth-3.6.0/allianceauth/services/modules/openfire/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/phpbb3/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/services/modules/phpbb3/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/phpbb3/manager.py` & `allianceauth-3.6.0/allianceauth/services/modules/phpbb3/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/phpbb3/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/services/modules/phpbb3/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py` & `allianceauth-3.6.0/allianceauth/services/modules/phpbb3/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/phpbb3/tasks.py` & `allianceauth-3.6.0/allianceauth/services/modules/phpbb3/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/phpbb3/tests.py` & `allianceauth-3.6.0/allianceauth/services/modules/phpbb3/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/phpbb3/urls.py` & `allianceauth-3.6.0/allianceauth/services/modules/xenforo/urls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-from django.conf.urls import include
-from django.urls import path
+from django.urls import include, path
 
 from . import views
 
-app_name = 'phpbb3'
+app_name = 'xenforo'
 
 module_urls = [
-    # Forum Service Control
-    path('activate/', views.activate_forum, name='activate'),
-    path('deactivate/', views.deactivate_forum, name='deactivate'),
-    path('reset_password/', views.reset_forum_password, name='reset_password'),
-    path('set_password/', views.set_forum_password, name='set_password'),
+    # XenForo service control
+    path('activate/', views.activate_xenforo_forum, name='activate'),
+    path('deactivate/', views.deactivate_xenforo_forum, name='deactivate'),
+    path('reset_password/', views.reset_xenforo_password, name='reset_password'),
+    path('set_password/', views.set_xenforo_password, name='set_password'),
 ]
 
 urlpatterns = [
-    path('phpbb3/', include((module_urls, app_name), namespace=app_name))
+    path('xenforo/', include((module_urls, app_name), namespace=app_name)),
 ]
```

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/phpbb3/views.py` & `allianceauth-3.6.0/allianceauth/services/modules/phpbb3/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/smf/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/services/modules/smf/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/smf/manager.py` & `allianceauth-3.6.0/allianceauth/services/modules/smf/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/smf/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/services/modules/smf/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/smf/migrations/0002_service_permissions.py` & `allianceauth-3.6.0/allianceauth/services/modules/smf/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py` & `allianceauth-3.6.0/allianceauth/services/modules/smf/migrations/0003_set_smf_displayed_names.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/smf/tasks.py` & `allianceauth-3.6.0/allianceauth/services/modules/smf/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/smf/tests.py` & `allianceauth-3.6.0/allianceauth/services/modules/smf/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/smf/urls.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/urls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-from django.conf.urls import include
-from django.urls import path
+from django.urls import include, path
 
 from . import views
 
-app_name = 'smf'
+app_name = 'teamspeak3'
 
 module_urls = [
-    # SMF Service Control
-    path('activate/', views.activate_smf, name='activate'),
-    path('deactivate/', views.deactivate_smf, name='deactivate'),
-    path('reset_password/', views.reset_smf_password, name='reset_password'),
-    path('set_password/', views.set_smf_password, name='set_password'),
+    # Teamspeak3 service control
+    path('activate/', views.activate_teamspeak3, name='activate'),
+    path('deactivate/', views.deactivate_teamspeak3, name='deactivate'),
+    path('reset_perm/', views.reset_teamspeak3_perm, name='reset_perm'),
+    path(
+        'admin_update_ts3_groups/',
+        views.admin_update_ts3_groups,
+        name='admin_update_ts3_groups'
+    ),
+
+    # Teamspeak Urls
+    path('verify/', views.verify_teamspeak3, name='verify'),
 ]
 
 urlpatterns = [
-    path('smf/', include((module_urls, app_name), namespace=app_name)),
+    path('teamspeak3/', include((module_urls, app_name), namespace=app_name)),
 ]
```

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/smf/views.py` & `allianceauth-3.6.0/allianceauth/services/modules/smf/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/admin.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,18 +32,20 @@
         return super().formfield_for_foreignkey(db_field, request, **kwargs)
 
     def formfield_for_manytomany(self, db_field, request, **kwargs):
         if db_field.name == 'ts_group':
             kwargs['queryset'] = TSgroup.objects.exclude(ts_group_name__in=ReservedGroupName.objects.values_list('name', flat=True))
         return super().formfield_for_manytomany(db_field, request, **kwargs)
 
+    @admin.display(
+        description='ts groups'
+    )
     def _ts_group(self, obj):
         return [x for x in obj.ts_group.all().order_by('ts_group_id')]
 
-    _ts_group.short_description = 'ts groups'
     # _ts_group.admin_order_field = 'profile__state'
 
 
 @admin.register(StateGroup)
 class StateGroupAdmin(admin.ModelAdmin):
     list_display = ('state', 'ts_group')
     search_fields = ('state__name', 'ts_group__ts_group_name')
```

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/manager.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/migrations/0002_auto_20161212_0133.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/migrations/0003_teamspeak3user.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/migrations/0004_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/migrations/0005_stategroup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/models.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/signals.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/tasks.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeak3_service_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/templates/services/teamspeak3/teamspeakjoin.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/tests.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/util/ts3.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/util/ts3.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/teamspeak3/views.py` & `allianceauth-3.6.0/allianceauth/services/modules/teamspeak3/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/xenforo/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/services/modules/xenforo/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/xenforo/manager.py` & `allianceauth-3.6.0/allianceauth/services/modules/xenforo/manager.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/xenforo/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/services/modules/xenforo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py` & `allianceauth-3.6.0/allianceauth/services/modules/xenforo/migrations/0002_service_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/xenforo/tasks.py` & `allianceauth-3.6.0/allianceauth/services/modules/xenforo/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/xenforo/tests.py` & `allianceauth-3.6.0/allianceauth/services/modules/xenforo/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/modules/xenforo/views.py` & `allianceauth-3.6.0/allianceauth/services/modules/xenforo/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/signals.py` & `allianceauth-3.6.0/allianceauth/services/signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/tasks.py` & `allianceauth-3.6.0/allianceauth/services/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/templates/services/fleetformattertool.html` & `allianceauth-3.6.0/allianceauth/services/templates/services/fleetformattertool.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/templates/services/service_confirm_delete.html` & `allianceauth-3.6.0/allianceauth/services/templates/services/service_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/templates/services/service_credentials.html` & `allianceauth-3.6.0/allianceauth/services/templates/services/service_credentials.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/templates/services/service_password.html` & `allianceauth-3.6.0/allianceauth/services/templates/services/service_password.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/templates/services/services.html` & `allianceauth-3.6.0/allianceauth/services/templates/services/services.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/templates/services/services_ctrl.html` & `allianceauth-3.6.0/allianceauth/services/templates/services/services_ctrl.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/templatetags/menu_items.py` & `allianceauth-3.6.0/allianceauth/services/templatetags/menu_items.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/tests/test_models.py` & `allianceauth-3.6.0/allianceauth/services/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/tests/test_nameformatter.py` & `allianceauth-3.6.0/allianceauth/services/tests/test_nameformatter.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/tests/test_signals.py` & `allianceauth-3.6.0/allianceauth/services/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/tests/test_tasks.py` & `allianceauth-3.6.0/allianceauth/services/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/services/urls.py` & `allianceauth-3.6.0/allianceauth/services/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.conf.urls import include
+from django.urls import include
 from allianceauth.hooks import get_hooks
 from django.urls import path
 
 from . import views
 
 urlpatterns = [
     # Services
```

### Comparing `allianceauth-3.5.1/allianceauth/services/views.py` & `allianceauth-3.6.0/allianceauth/services/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/srp/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/form.py` & `allianceauth-3.6.0/allianceauth/srp/form.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/managers.py` & `allianceauth-3.6.0/allianceauth/srp/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/srp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/migrations/0003_make_strings_more_stringy.py` & `allianceauth-3.6.0/allianceauth/srp/migrations/0003_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/migrations/0004_on_delete.py` & `allianceauth-3.6.0/allianceauth/srp/migrations/0004_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/models.py` & `allianceauth-3.6.0/allianceauth/srp/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/swagger.json` & `allianceauth-3.6.0/allianceauth/srp/swagger.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/templates/srp/add.html` & `allianceauth-3.6.0/allianceauth/srp/templates/srp/add.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/templates/srp/data.html` & `allianceauth-3.6.0/allianceauth/srp/templates/srp/data.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/templates/srp/management.html` & `allianceauth-3.6.0/allianceauth/srp/templates/srp/management.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/templates/srp/request.html` & `allianceauth-3.6.0/allianceauth/srp/templates/srp/request.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/templates/srp/update.html` & `allianceauth-3.6.0/allianceauth/srp/templates/srp/update.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/tests/test_managers.py` & `allianceauth-3.6.0/allianceauth/srp/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json` & `allianceauth-3.6.0/allianceauth/srp/tests/testdata/get_killmails_killmail_id_killmail_hash_81973979.json`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/urls.py` & `allianceauth-3.6.0/allianceauth/srp/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/srp/views.py` & `allianceauth-3.6.0/allianceauth/srp/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/css/auth-base.css` & `allianceauth-3.6.0/allianceauth/static/allianceauth/css/auth-base.css`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/css/checkbox.css` & `allianceauth-3.6.0/allianceauth/static/allianceauth/css/checkbox.css`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less` & `allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/bootstrap-locals.less`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/darkly/LICENSE` & `allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/darkly/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/darkly/darkly.less` & `allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.less`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css` & `allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/darkly/darkly.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/flatly/LICENSE` & `allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/flatly/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/flatly/flatly.less` & `allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.less`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css` & `allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/flatly/flatly.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/css/themes/flatly-shared.less` & `allianceauth-3.6.0/allianceauth/static/allianceauth/css/themes/flatly-shared.less`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/icons/allianceauth.png` & `allianceauth-3.6.0/allianceauth/static/allianceauth/icons/allianceauth.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/icons/favicon-96x96.png` & `allianceauth-3.6.0/allianceauth/static/allianceauth/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/js/eve-time.js` & `allianceauth-3.6.0/allianceauth/static/allianceauth/js/eve-time.js`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/js/filterDropDown/LICENSE` & `allianceauth-3.6.0/allianceauth/static/allianceauth/js/filterDropDown/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js` & `allianceauth-3.6.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.js`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js` & `allianceauth-3.6.0/allianceauth/static/allianceauth/js/filterDropDown/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png` & `allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png` & `allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png` & `allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png` & `allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png` & `allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png` & `allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css` & `allianceauth-3.6.0/allianceauth/static/allianceauth/js/jquery-ui/1.12.1/css/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/js/refresh_notifications.js` & `allianceauth-3.6.0/allianceauth/static/allianceauth/js/refresh_notifications.js`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/static/allianceauth/js/timers.js` & `allianceauth-3.6.0/allianceauth/static/allianceauth/js/timers.js`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/templates/allianceauth/admin-status/overview.html` & `allianceauth-3.6.0/allianceauth/templates/allianceauth/admin-status/overview.html`

 * *Files 6% similar despite different names*

```diff
@@ -88,16 +88,19 @@
                         title="{{ tasks_succeeded|intcomma }} succeeded, {{ tasks_retried|intcomma }} retried, {{ tasks_failed|intcomma }} failed"
                     >
                         {% include "allianceauth/admin-status/celery_bar_partial.html" with label="suceeded" level="success" tasks_count=tasks_succeeded %}
                         {% include "allianceauth/admin-status/celery_bar_partial.html" with label="retried" level="info" tasks_count=tasks_retried %}
                         {% include "allianceauth/admin-status/celery_bar_partial.html" with label="failed" level="danger" tasks_count=tasks_failed %}
                     </div>
                     <p>
+                        {% blocktranslate with running_count=tasks_running|default_if_none:"?"|intcomma %}
+                            {{ running_count }} running |
+                        {% endblocktranslate %}
                         {% blocktranslate with queue_length=task_queue_length|default_if_none:"?"|intcomma %}
-                        {{ queue_length }} queued tasks
+                            {{ queue_length }} queued
                         {% endblocktranslate %}
                     </p>
                 </div>
             </div>
         </div>
     </div>
     <div class="clearfix"></div>
```

#### html2text {}

```diff
@@ -26,9 +26,11 @@
 tasks â¢ last {{ latest }} {% endblocktranslate %}
 {% include "allianceauth/admin-status/celery_bar_partial.html" with
 label="suceeded" level="success" tasks_count=tasks_succeeded %} {% include
 "allianceauth/admin-status/celery_bar_partial.html" with label="retried"
 level="info" tasks_count=tasks_retried %} {% include "allianceauth/admin-
 status/celery_bar_partial.html" with label="failed" level="danger"
 tasks_count=tasks_failed %}
-{% blocktranslate with queue_length=task_queue_length|default_if_none:
-"?"|intcomma %} {{ queue_length }} queued tasks {% endblocktranslate %}
+{% blocktranslate with running_count=tasks_running|default_if_none:"?"|intcomma
+%} {{ running_count }} running | {% endblocktranslate %} {% blocktranslate with
+queue_length=task_queue_length|default_if_none:"?"|intcomma %} {{ queue_length
+}} queued {% endblocktranslate %}
```

### Comparing `allianceauth-3.5.1/allianceauth/templates/allianceauth/base.html` & `allianceauth-3.6.0/allianceauth/templates/allianceauth/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/templates/allianceauth/messages.html` & `allianceauth-3.6.0/allianceauth/templates/allianceauth/messages.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/templates/allianceauth/side-menu.html` & `allianceauth-3.6.0/allianceauth/templates/allianceauth/side-menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/templates/allianceauth/top-menu-admin.html` & `allianceauth-3.6.0/allianceauth/templates/allianceauth/top-menu-admin.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/templates/allianceauth/top-menu-user-dropdown.html` & `allianceauth-3.6.0/allianceauth/templates/allianceauth/top-menu-user-dropdown.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/templates/allianceauth/top-menu.html` & `allianceauth-3.6.0/allianceauth/templates/allianceauth/top-menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/templates/bundles/bootstrap-css.html` & `allianceauth-3.6.0/allianceauth/templates/bundles/bootstrap-css.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/templates/bundles/bootstrap-js.html` & `allianceauth-3.6.0/allianceauth/templates/bundles/bootstrap-js.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/templates/bundles/datatables-js.html` & `allianceauth-3.6.0/allianceauth/templates/bundles/datatables-js.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/templates/bundles/moment-js.html` & `allianceauth-3.6.0/allianceauth/templates/bundles/moment-js.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/templatetags/admin_status.py` & `allianceauth-3.6.0/allianceauth/templatetags/admin_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,29 +36,30 @@
 
 
 @register.simple_tag()
 def decimal_widthratio(this_value, max_value, max_width) -> str:
     if max_value == 0:
         return str(0)
 
-    return str(round(this_value/max_value * max_width, 2))
+    return str(round(this_value / max_value * max_width, 2))
 
 
 @register.inclusion_tag('allianceauth/admin-status/overview.html')
 def status_overview() -> dict:
     response = {
         "notifications": list(),
         "current_version": __version__,
         "task_queue_length": None,
         "tasks_succeeded": 0,
         "tasks_retried": 0,
         "tasks_failed": 0,
         "tasks_total": 0,
         "tasks_hours": 0,
-        "earliest_task": None
+        "earliest_task": None,
+        "tasks_running": 0
     }
     response.update(_current_notifications())
     response.update(_current_version_summary())
     response.update({'task_queue_length': _fetch_celery_queue_length()})
     response.update(_celery_stats())
     return response
 
@@ -68,15 +69,16 @@
     results = dashboard_results(hours=hours)
     return {
         "tasks_succeeded": results.succeeded,
         "tasks_retried": results.retried,
         "tasks_failed": results.failed,
         "tasks_total": results.total,
         "tasks_hours": results.hours,
-        "earliest_task": results.earliest_task
+        "earliest_task": results.earliest_task,
+        "tasks_running": results.running,
     }
 
 
 def _fetch_celery_queue_length() -> Optional[int]:
     try:
         app = app_or_default(None)
         with app.connection_or_acquire() as conn:
```

### Comparing `allianceauth-3.5.1/allianceauth/tests/auth_utils.py` & `allianceauth-3.6.0/allianceauth/tests/auth_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/tests/test_auth_utils.py` & `allianceauth-3.6.0/allianceauth/tests/test_auth_utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/thirdparty/navhelper/templatetags/navactive.py` & `allianceauth-3.6.0/allianceauth/thirdparty/navhelper/templatetags/navactive.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/thirdparty/navhelper/tests.py` & `allianceauth-3.6.0/allianceauth/thirdparty/navhelper/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/timerboard/auth_hooks.py` & `allianceauth-3.6.0/allianceauth/timerboard/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/timerboard/form.py` & `allianceauth-3.6.0/allianceauth/timerboard/form.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,38 +57,53 @@
 
     details = forms.CharField(max_length=254, required=True, label=_('Details'))
     system = forms.CharField(max_length=254, required=True, label=_("System"))
     planet_moon = forms.CharField(max_length=254, label=_("Planet/Moon"), required=False, initial="")
     structure = forms.ChoiceField(choices=structure_choices, required=True, label=_("Structure Type"))
     timer_type = forms.ChoiceField(choices=TimerType.choices, label=_("Timer Type"))
     objective = forms.ChoiceField(choices=objective_choices, required=True, label=_("Objective"))
-    days_left = forms.IntegerField(required=True, label=_("Days Remaining"), validators=[MinValueValidator(0)])
-    hours_left = forms.IntegerField(required=True, label=_("Hours Remaining"),
+    absolute_checkbox = forms.BooleanField(label=_("Absolute Timer"), required=False, initial=False)
+    absolute_time = forms.CharField(required=False,label=_("Date and Time"))
+    days_left = forms.IntegerField(required=False, label=_("Days Remaining"), validators=[MinValueValidator(0)])
+    hours_left = forms.IntegerField(required=False, label=_("Hours Remaining"),
                                     validators=[MinValueValidator(0), MaxValueValidator(23)])
-    minutes_left = forms.IntegerField(required=True, label=_("Minutes Remaining"),
+    minutes_left = forms.IntegerField(required=False, label=_("Minutes Remaining"),
                                         validators=[MinValueValidator(0), MaxValueValidator(59)])
     important = forms.BooleanField(label=_("Important"), required=False)
     corp_timer = forms.BooleanField(label=_("Corp-Restricted"), required=False)
 
+
     def save(self, commit=True):
         timer = super().save(commit=False)
 
         # Get character
         character = self.user.profile.main_character
         corporation = character.corporation
         logger.debug("Determined timer save request on behalf "
                     "of character {} corporation {}".format(character, corporation))
-        # calculate future time
-        future_time = datetime.timedelta(days=self.cleaned_data['days_left'], hours=self.cleaned_data['hours_left'],
-                                        minutes=self.cleaned_data['minutes_left'])
-        current_time = timezone.now()
-        eve_time = current_time + future_time
-        logger.debug(
-            f"Determined timer eve time is {eve_time} - current time {current_time}, adding {future_time}")
+
+        days_left = self.cleaned_data['days_left']
+        hours_left = self.cleaned_data['hours_left']
+        minutes_left = self.cleaned_data['minutes_left']
+        absolute_time = self.cleaned_data['absolute_time']
+
+        if days_left or hours_left or minutes_left:
+            # Calculate future time
+            future_time = datetime.timedelta(days=days_left, hours=hours_left, minutes=minutes_left)
+            current_time = timezone.now()
+            eve_time = current_time + future_time
+            logger.debug(f"Determined timer eve time is {eve_time} - current time {current_time}, adding {future_time}")
+        elif absolute_time:
+            # Use absolute time
+            eve_time = absolute_time
+        else:
+            raise ValueError("Either future time or absolute time must be provided.")
 
         timer.eve_time = eve_time
         timer.eve_character = character
         timer.eve_corp = corporation
         timer.user = self.user
+
         if commit:
             timer.save()
+
         return timer
```

### Comparing `allianceauth-3.5.1/allianceauth/timerboard/migrations/0001_initial.py` & `allianceauth-3.6.0/allianceauth/timerboard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py` & `allianceauth-3.6.0/allianceauth/timerboard/migrations/0002_make_strings_more_stringy.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/timerboard/migrations/0003_on_delete.py` & `allianceauth-3.6.0/allianceauth/timerboard/migrations/0003_on_delete.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/timerboard/migrations/0004_timer_type.py` & `allianceauth-3.6.0/allianceauth/timerboard/migrations/0004_timer_type.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/timerboard/models.py` & `allianceauth-3.6.0/allianceauth/timerboard/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html` & `allianceauth-3.6.0/allianceauth/timerboard/templates/timerboard/timer_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/timerboard/templates/timerboard/view.html` & `allianceauth-3.6.0/allianceauth/timerboard/templates/timerboard/view.html`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/timerboard/tests.py` & `allianceauth-3.6.0/allianceauth/timerboard/tests.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/timerboard/views.py` & `allianceauth-3.6.0/allianceauth/timerboard/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/utils/cache.py` & `allianceauth-3.6.0/allianceauth/utils/cache.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/utils/django.py` & `allianceauth-3.6.0/allianceauth/utils/django.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/utils/testing.py` & `allianceauth-3.6.0/allianceauth/utils/testing.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/utils/tests/test_cache.py` & `allianceauth-3.6.0/allianceauth/utils/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/utils/tests/test_django.py` & `allianceauth-3.6.0/allianceauth/utils/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `allianceauth-3.5.1/allianceauth/views.py` & `allianceauth-3.6.0/allianceauth/views.py`

 * *Files identical despite different names*

