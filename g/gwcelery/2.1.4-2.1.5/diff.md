# Comparing `tmp/gwcelery-2.1.4.tar.gz` & `tmp/gwcelery-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwcelery-2.1.4.tar", max compression
+gzip compressed data, was "gwcelery-2.1.5.tar", max compression
```

## Comparing `gwcelery-2.1.4.tar` & `gwcelery-2.1.5.tar`

### file list

```diff
@@ -1,240 +1,240 @@
--rw-r--r--   0        0        0    99257 2023-07-26 22:43:30.913941 gwcelery-2.1.4/CHANGES.rst
--rw-r--r--   0        0        0       64 2023-07-26 22:43:30.913941 gwcelery-2.1.4/CONTRIBUTING.rst
--rw-r--r--   0        0        0    19716 2023-07-26 22:43:30.914941 gwcelery-2.1.4/LICENSE.rst
--rw-r--r--   0        0        0     1351 2023-07-26 22:43:30.914941 gwcelery-2.1.4/README.rst
--rw-r--r--   0        0        0      634 2023-07-26 22:43:30.915942 gwcelery-2.1.4/doc/Makefile
--rw-r--r--   0        0        0   191486 2023-07-26 22:43:30.918942 gwcelery-2.1.4/doc/_static/acceptance-tests-checklist.png
--rw-r--r--   0        0        0   241593 2023-07-26 22:43:30.921942 gwcelery-2.1.4/doc/_static/celeryevent-screenshot.png
--rw-r--r--   0        0        0   206465 2023-07-26 22:43:30.924941 gwcelery-2.1.4/doc/_static/deployment-screenshot.png
--rw-r--r--   0        0        0   161306 2023-07-26 22:43:30.927941 gwcelery-2.1.4/doc/_static/flask-screenshot.png
--rw-r--r--   0        0        0   328056 2023-07-26 22:43:30.933941 gwcelery-2.1.4/doc/_static/flower-screenshot.png
--rw-r--r--   0        0        0   114719 2023-07-26 22:43:30.935942 gwcelery-2.1.4/doc/_static/logo-0.5x.png
--rw-r--r--   0        0        0   351955 2023-07-26 22:43:30.941942 gwcelery-2.1.4/doc/_static/logo.png
--rw-r--r--   0        0        0   230777 2023-07-26 22:43:30.945942 gwcelery-2.1.4/doc/_static/sentry-screenshot.png
--rwxr-xr-x   0        0        0     7356 2023-07-26 22:43:30.945942 gwcelery-2.1.4/doc/conf.py
--rw-r--r--   0        0        0     4346 2023-07-26 22:43:30.946942 gwcelery-2.1.4/doc/configuration.rst
--rw-r--r--   0        0        0     5698 2023-07-26 22:43:30.946942 gwcelery-2.1.4/doc/contributing.rst
--rw-r--r--   0        0        0     7202 2023-07-26 22:43:30.947942 gwcelery-2.1.4/doc/deployment.rst
--rw-r--r--   0        0        0    10176 2023-07-26 22:43:30.947942 gwcelery-2.1.4/doc/design.rst
--rw-r--r--   0        0        0      486 2023-07-26 22:43:30.947942 gwcelery-2.1.4/doc/gwcelery.conf.rst
--rw-r--r--   0        0        0      284 2023-07-26 22:43:30.947942 gwcelery-2.1.4/doc/gwcelery.email.rst
--rw-r--r--   0        0        0      329 2023-07-26 22:43:30.948942 gwcelery-2.1.4/doc/gwcelery.igwn_alert.rst
--rw-r--r--   0        0        0      227 2023-07-26 22:43:30.948942 gwcelery-2.1.4/doc/gwcelery.rst
--rw-r--r--   0        0        0       79 2023-07-26 22:43:30.948942 gwcelery-2.1.4/doc/gwcelery.sentry.rst
--rw-r--r--   0        0        0       97 2023-07-26 22:43:30.948942 gwcelery-2.1.4/doc/gwcelery.tasks.alerts.rst
--rw-r--r--   0        0        0      103 2023-07-26 22:43:30.948942 gwcelery-2.1.4/doc/gwcelery.tasks.bayestar.rst
--rw-r--r--   0        0        0      107 2023-07-26 22:43:30.949941 gwcelery-2.1.4/doc/gwcelery.tasks.circulars.rst
--rw-r--r--   0        0        0       98 2023-07-26 22:43:30.949941 gwcelery-2.1.4/doc/gwcelery.tasks.condor.rst
--rw-r--r--   0        0        0     2404 2023-07-26 22:43:30.949941 gwcelery-2.1.4/doc/gwcelery.tasks.detchar.rst
--rw-r--r--   0        0        0     1110 2023-07-26 22:43:30.949941 gwcelery-2.1.4/doc/gwcelery.tasks.em_bright.rst
--rw-r--r--   0        0        0      129 2023-07-26 22:43:30.949941 gwcelery-2.1.4/doc/gwcelery.tasks.external_skymaps.rst
--rw-r--r--   0        0        0     6738 2023-07-26 22:43:30.950942 gwcelery-2.1.4/doc/gwcelery.tasks.external_triggers.rst
--rw-r--r--   0        0        0      112 2023-07-26 22:43:30.950942 gwcelery-2.1.4/doc/gwcelery.tasks.first2years.rst
--rw-r--r--   0        0        0       88 2023-07-26 22:43:30.950942 gwcelery-2.1.4/doc/gwcelery.tasks.gcn.rst
--rw-r--r--   0        0        0      100 2023-07-26 22:43:30.950942 gwcelery-2.1.4/doc/gwcelery.tasks.gracedb.rst
--rw-r--r--   0        0        0      109 2023-07-26 22:43:30.950942 gwcelery-2.1.4/doc/gwcelery.tasks.igwn_alert.rst
--rw-r--r--   0        0        0      109 2023-07-26 22:43:30.950942 gwcelery-2.1.4/doc/gwcelery.tasks.inference.rst
--rw-r--r--   0        0        0     8111 2023-07-26 22:43:30.951942 gwcelery-2.1.4/doc/gwcelery.tasks.orchestrator.rst
--rw-r--r--   0        0        0      100 2023-07-26 22:43:30.951942 gwcelery-2.1.4/doc/gwcelery.tasks.p_astro.rst
--rw-r--r--   0        0        0       94 2023-07-26 22:43:30.951942 gwcelery-2.1.4/doc/gwcelery.tasks.raven.rst
--rw-r--r--   0        0        0      628 2023-07-26 22:43:30.951942 gwcelery-2.1.4/doc/gwcelery.tasks.rst
--rw-r--r--   0        0        0      100 2023-07-26 22:43:30.952942 gwcelery-2.1.4/doc/gwcelery.tasks.skymaps.rst
--rw-r--r--   0        0        0     7161 2023-07-26 22:43:30.952942 gwcelery-2.1.4/doc/gwcelery.tasks.superevents.rst
--rw-r--r--   0        0        0       97 2023-07-26 22:43:30.952942 gwcelery-2.1.4/doc/gwcelery.tools.condor.rst
--rw-r--r--   0        0        0       94 2023-07-26 22:43:30.952942 gwcelery-2.1.4/doc/gwcelery.tools.flask.rst
--rw-r--r--   0        0        0       97 2023-07-26 22:43:30.952942 gwcelery-2.1.4/doc/gwcelery.tools.nagios.rst
--rw-r--r--   0        0        0      185 2023-07-26 22:43:30.953942 gwcelery-2.1.4/doc/gwcelery.tools.rst
--rw-r--r--   0        0        0       73 2023-07-26 22:43:30.953942 gwcelery-2.1.4/doc/gwcelery.util.rst
--rw-r--r--   0        0        0      507 2023-07-26 22:43:30.953942 gwcelery-2.1.4/doc/gwcelery.voevent.rst
--rw-r--r--   0        0        0     3564 2023-07-26 22:43:30.953942 gwcelery-2.1.4/doc/htcondor.rst
--rw-r--r--   0        0        0     1576 2023-07-26 22:43:30.953942 gwcelery-2.1.4/doc/index.rst
--rw-r--r--   0        0        0      800 2023-07-26 22:43:30.954942 gwcelery-2.1.4/doc/make.bat
--rw-r--r--   0        0        0     4416 2023-07-26 22:43:30.954942 gwcelery-2.1.4/doc/monitoring.rst
--rw-r--r--   0        0        0     5312 2023-07-26 22:43:30.954942 gwcelery-2.1.4/doc/quickstart.rst
--rw-r--r--   0        0        0     1149 2023-07-26 22:43:30.955942 gwcelery-2.1.4/gwcelery/__init__.py
--rw-r--r--   0        0        0    18447 2023-07-26 22:43:30.955942 gwcelery-2.1.4/gwcelery/_version.py
--rw-r--r--   0        0        0    16852 2023-07-26 22:43:30.956942 gwcelery-2.1.4/gwcelery/conf/__init__.py
--rw-r--r--   0        0        0     1014 2023-07-26 22:43:30.956942 gwcelery-2.1.4/gwcelery/conf/dev.py
--rw-r--r--   0        0        0      403 2023-07-26 22:43:30.956942 gwcelery-2.1.4/gwcelery/conf/development.py
--rw-r--r--   0        0        0     1289 2023-07-26 22:43:30.957942 gwcelery-2.1.4/gwcelery/conf/minikube.py
--rw-r--r--   0        0        0     1865 2023-07-26 22:43:30.957942 gwcelery-2.1.4/gwcelery/conf/playground.py
--rw-r--r--   0        0        0     3507 2023-07-26 22:43:30.957942 gwcelery-2.1.4/gwcelery/conf/production.py
--rw-r--r--   0        0        0     2040 2023-07-26 22:43:30.957942 gwcelery-2.1.4/gwcelery/conf/test.py
--rw-r--r--   0        0        0        0 2023-07-26 22:43:31.249943 gwcelery-2.1.4/gwcelery/data/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 22:43:31.250943 gwcelery-2.1.4/gwcelery/data/first2years/__init__.py
--rw-r--r--   0        0        0   731421 2023-07-26 22:43:30.964942 gwcelery-2.1.4/gwcelery/data/first2years/gstlal.xml.gz
--rwxr-xr-x   0        0        0     2999 2023-07-26 22:43:30.965942 gwcelery-2.1.4/gwcelery/data/gwcelery.sub
--rw-r--r--   0        0        0      505 2023-07-26 22:43:30.965942 gwcelery-2.1.4/gwcelery/email/__init__.py
--rw-r--r--   0        0        0     3317 2023-07-26 22:43:30.965942 gwcelery-2.1.4/gwcelery/email/bootsteps.py
--rw-r--r--   0        0        0      995 2023-07-26 22:43:30.966942 gwcelery-2.1.4/gwcelery/email/signals.py
--rw-r--r--   0        0        0     1457 2023-07-26 22:43:30.966942 gwcelery-2.1.4/gwcelery/flask.py
--rw-r--r--   0        0        0      529 2023-07-26 22:43:30.966942 gwcelery-2.1.4/gwcelery/igwn_alert/__init__.py
--rw-r--r--   0        0        0     4484 2023-07-26 22:43:30.967942 gwcelery-2.1.4/gwcelery/igwn_alert/bootsteps.py
--rw-r--r--   0        0        0      608 2023-07-26 22:43:30.967942 gwcelery-2.1.4/gwcelery/igwn_alert/signals.py
--rw-r--r--   0        0        0      275 2023-07-26 22:43:30.967942 gwcelery-2.1.4/gwcelery/jinja.py
--rw-r--r--   0        0        0      305 2023-07-26 22:43:30.967942 gwcelery-2.1.4/gwcelery/kafka/__init__.py
--rw-r--r--   0        0        0    10758 2023-07-26 22:43:30.968942 gwcelery-2.1.4/gwcelery/kafka/bootsteps.py
--rw-r--r--   0        0        0      522 2023-07-26 22:43:30.968942 gwcelery-2.1.4/gwcelery/kafka/signals.py
--rw-r--r--   0        0        0     2567 2023-07-26 22:43:30.968942 gwcelery-2.1.4/gwcelery/sentry/__init__.py
--rw-r--r--   0        0        0       34 2023-07-26 22:43:30.968942 gwcelery-2.1.4/gwcelery/sentry/integrations/__init__.py
--rw-r--r--   0        0        0      832 2023-07-26 22:43:30.969942 gwcelery-2.1.4/gwcelery/sentry/integrations/condor.py
--rw-r--r--   0        0        0      836 2023-07-26 22:43:30.969942 gwcelery-2.1.4/gwcelery/sentry/integrations/requests.py
--rw-r--r--   0        0        0      939 2023-07-26 22:43:30.969942 gwcelery-2.1.4/gwcelery/sentry/integrations/subprocess.py
--rw-r--r--   0        0        0     1302 2023-07-26 22:43:30.969942 gwcelery-2.1.4/gwcelery/static/typeahead.css
--rw-r--r--   0        0        0     4124 2023-07-26 22:43:30.970942 gwcelery-2.1.4/gwcelery/static/vega/index.html
--rw-r--r--   0        0        0      515 2023-07-26 22:43:30.970942 gwcelery-2.1.4/gwcelery/tasks/__init__.py
--rw-r--r--   0        0        0    13633 2023-07-26 22:43:30.970942 gwcelery-2.1.4/gwcelery/tasks/alerts.py
--rw-r--r--   0        0        0     2672 2023-07-26 22:43:30.971942 gwcelery-2.1.4/gwcelery/tasks/bayestar.py
--rw-r--r--   0        0        0     1535 2023-07-26 22:43:30.971942 gwcelery-2.1.4/gwcelery/tasks/circulars.py
--rw-r--r--   0        0        0     7502 2023-07-26 22:43:30.971942 gwcelery-2.1.4/gwcelery/tasks/condor.py
--rw-r--r--   0        0        0     2692 2023-07-26 22:43:30.971942 gwcelery-2.1.4/gwcelery/tasks/core.py
--rw-r--r--   0        0        0    22989 2023-07-26 22:43:30.972942 gwcelery-2.1.4/gwcelery/tasks/detchar.py
--rw-r--r--   0        0        0     4865 2023-07-26 22:43:30.972942 gwcelery-2.1.4/gwcelery/tasks/em_bright.py
--rw-r--r--   0        0        0    23428 2023-07-26 22:43:30.973942 gwcelery-2.1.4/gwcelery/tasks/external_skymaps.py
--rw-r--r--   0        0        0    29099 2023-07-26 22:43:30.974942 gwcelery-2.1.4/gwcelery/tasks/external_triggers.py
--rw-r--r--   0        0        0     6832 2023-07-26 22:43:30.974942 gwcelery-2.1.4/gwcelery/tasks/first2years.py
--rw-r--r--   0        0        0     6320 2023-07-26 22:43:30.974942 gwcelery-2.1.4/gwcelery/tasks/first2years_external.py
--rw-r--r--   0        0        0     4831 2023-07-26 22:43:30.975942 gwcelery-2.1.4/gwcelery/tasks/gcn.py
--rw-r--r--   0        0        0    11079 2023-07-26 22:43:30.975942 gwcelery-2.1.4/gwcelery/tasks/gracedb.py
--rw-r--r--   0        0        0     6105 2023-07-26 22:43:30.975942 gwcelery-2.1.4/gwcelery/tasks/gwskynet.py
--rw-r--r--   0        0        0     2453 2023-07-26 22:43:30.976942 gwcelery-2.1.4/gwcelery/tasks/igwn_alert.py
--rw-r--r--   0        0        0    34172 2023-07-26 22:43:30.977942 gwcelery-2.1.4/gwcelery/tasks/inference.py
--rw-r--r--   0        0        0     1406 2023-07-26 22:43:30.977942 gwcelery-2.1.4/gwcelery/tasks/legacy_gracedb.py
--rw-r--r--   0        0        0     7772 2023-07-26 22:43:30.977942 gwcelery-2.1.4/gwcelery/tasks/notice_text.py
--rw-r--r--   0        0        0    48026 2023-07-26 22:43:30.978942 gwcelery-2.1.4/gwcelery/tasks/orchestrator.py
--rw-r--r--   0        0        0     5796 2023-07-26 22:43:30.978942 gwcelery-2.1.4/gwcelery/tasks/p_astro.py
--rw-r--r--   0        0        0    21540 2023-07-26 22:43:30.979942 gwcelery-2.1.4/gwcelery/tasks/raven.py
--rw-r--r--   0        0        0     2242 2023-07-26 22:43:30.979942 gwcelery-2.1.4/gwcelery/tasks/rrt_utils.py
--rw-r--r--   0        0        0    12528 2023-07-26 22:43:30.980942 gwcelery-2.1.4/gwcelery/tasks/skymaps.py
--rw-r--r--   0        0        0    23631 2023-07-26 22:43:30.981942 gwcelery-2.1.4/gwcelery/tasks/superevents.py
--rw-r--r--   0        0        0     1084 2023-07-26 22:43:30.981942 gwcelery-2.1.4/gwcelery/templates/fits_header.jinja2
--rw-r--r--   0        0        0    35556 2023-07-26 22:43:30.982942 gwcelery-2.1.4/gwcelery/templates/index.jinja2
--rw-r--r--   0        0        0     8505 2023-07-26 22:43:30.983942 gwcelery-2.1.4/gwcelery/templates/lalinference.jinja2
--rw-r--r--   0        0        0     9442 2023-07-26 22:43:30.983942 gwcelery-2.1.4/gwcelery/templates/rapidpe.jinja2
--rw-r--r--   0        0        0      472 2023-07-26 22:43:30.983942 gwcelery-2.1.4/gwcelery/templates/vector_table.jinja2
--rw-r--r--   0        0        0        0 2023-07-26 22:43:31.256943 gwcelery-2.1.4/gwcelery/tests/__init__.py
--rw-r--r--   0        0        0     4388 2023-07-26 22:43:30.984942 gwcelery-2.1.4/gwcelery/tests/conftest.py
--rw-r--r--   0        0        0      976 2023-07-26 22:43:30.984942 gwcelery-2.1.4/gwcelery/tests/data/G000012_S0040_preferred.json
--rw-r--r--   0        0        0     6258 2023-07-26 22:43:30.985942 gwcelery-2.1.4/gwcelery/tests/data/G298048-1-Initial.xml
--rw-r--r--   0        0        0      599 2023-07-26 22:43:30.985942 gwcelery-2.1.4/gwcelery/tests/data/G298048_log.json
--rw-r--r--   0        0        0      150 2023-07-26 22:43:30.985942 gwcelery-2.1.4/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
--rw-r--r--   0        0        0      974 2023-07-26 22:43:30.985942 gwcelery-2.1.4/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
--rw-r--r--   0        0        0    17572 2023-07-26 22:43:30.986942 gwcelery-2.1.4/gwcelery/tests/data/MS220722v.xml
--rw-r--r--   0        0        0   777600 2023-07-26 22:43:31.000942 gwcelery-2.1.4/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
--rw-r--r--   0        0        0     8220 2023-07-26 22:43:31.001942 gwcelery-2.1.4/gwcelery/tests/data/S230413b.json
--rw-r--r--   0        0        0     7255 2023-07-26 22:43:31.001942 gwcelery-2.1.4/gwcelery/tests/data/S230413g.json
--rw-r--r--   0        0        0     7721 2023-07-26 22:43:31.001942 gwcelery-2.1.4/gwcelery/tests/data/S230413h.json
--rw-r--r--   0        0        0     3387 2023-07-26 22:43:31.002942 gwcelery-2.1.4/gwcelery/tests/data/T0212_S0039_preferred.json
--rw-r--r--   0        0        0     3384 2023-07-26 22:43:31.002942 gwcelery-2.1.4/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
--rw-r--r--   0        0        0     5210 2023-07-26 22:43:31.002942 gwcelery-2.1.4/gwcelery/tests/data/T0219_S0041_nopreferred.json
--rw-r--r--   0        0        0        0 2023-07-26 22:43:31.257943 gwcelery-2.1.4/gwcelery/tests/data/__init__.py
--rw-r--r--   0        0        0     2290 2023-07-26 22:43:31.003942 gwcelery-2.1.4/gwcelery/tests/data/agile_grb_gcn.xml
--rw-r--r--   0        0        0   854036 2023-07-26 22:43:31.015942 gwcelery-2.1.4/gwcelery/tests/data/coinc.xml
--rw-r--r--   0        0        0     6175 2023-07-26 22:43:31.015942 gwcelery-2.1.4/gwcelery/tests/data/externaltrigger_original_data.xml
--rw-r--r--   0        0        0     5482 2023-07-26 22:43:31.016942 gwcelery-2.1.4/gwcelery/tests/data/fermi_grb_gcn.xml
--rw-r--r--   0        0        0     5469 2023-07-26 22:43:31.016942 gwcelery-2.1.4/gwcelery/tests/data/fermi_initial_grb_gcn.xml
--rw-r--r--   0        0        0     5865 2023-07-26 22:43:31.016942 gwcelery-2.1.4/gwcelery/tests/data/fermi_noise_gcn.xml
--rw-r--r--   0        0        0     5864 2023-07-26 22:43:31.016942 gwcelery-2.1.4/gwcelery/tests/data/fermi_noise_gcn_2.xml
--rw-r--r--   0        0        0     1914 2023-07-26 22:43:31.017942 gwcelery-2.1.4/gwcelery/tests/data/fermi_subgrbtargeted_template.xml
--rw-r--r--   0        0        0     4914 2023-07-26 22:43:31.017942 gwcelery-2.1.4/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
--rw-r--r--   0        0        0     4914 2023-07-26 22:43:31.017942 gwcelery-2.1.4/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
--rw-r--r--   0        0        0     3407 2023-07-26 22:43:31.017942 gwcelery-2.1.4/gwcelery/tests/data/fits_header_result.html
--rw-r--r--   0        0        0      882 2023-07-26 22:43:31.018942 gwcelery-2.1.4/gwcelery/tests/data/gracedb_externaltrigger_log.json
--rw-r--r--   0        0        0      446 2023-07-26 22:43:31.018942 gwcelery-2.1.4/gwcelery/tests/data/gracedb_setrigger_log.json
--rw-r--r--   0        0        0      870 2023-07-26 22:43:31.018942 gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_detchar.json
--rw-r--r--   0        0        0     2025 2023-07-26 22:43:31.019942 gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_exttrig_creation.json
--rw-r--r--   0        0        0     2007 2023-07-26 22:43:31.019942 gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
--rw-r--r--   0        0        0      166 2023-07-26 22:43:31.019942 gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_fits.json
--rw-r--r--   0        0        0      101 2023-07-26 22:43:31.019942 gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_label_dqv.json
--rw-r--r--   0        0        0      743 2023-07-26 22:43:31.019942 gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_psd.json
--rw-r--r--   0        0        0     2020 2023-07-26 22:43:31.020942 gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_snews_creation.json
--rw-r--r--   0        0        0     2012 2023-07-26 22:43:31.020942 gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_snews_test_creation.json
--rw-r--r--   0        0        0     2028 2023-07-26 22:43:31.020942 gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_subgrb_creation.json
--rw-r--r--   0        0        0     1235 2023-07-26 22:43:31.020942 gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_superevent_creation.json
--rw-r--r--   0        0        0      107 2023-07-26 22:43:31.021942 gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_superevent_label.json
--rw-r--r--   0        0        0     5021 2023-07-26 22:43:31.021942 gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_voevent.json
--rw-r--r--   0        0        0     4429 2023-07-26 22:43:31.021942 gwcelery-2.1.4/gwcelery/tests/data/integral_grb_gcn.xml
--rw-r--r--   0        0        0     4295 2023-07-26 22:43:31.022942 gwcelery-2.1.4/gwcelery/tests/data/integral_mdc_gcn.xml
--rw-r--r--   0        0        0  1038044 2023-07-26 22:43:31.038942 gwcelery-2.1.4/gwcelery/tests/data/kafka_alert_fermi.json
--rw-r--r--   0        0        0  1038042 2023-07-26 22:43:31.060942 gwcelery-2.1.4/gwcelery/tests/data/kafka_alert_fermi_ignore.json
--rw-r--r--   0        0        0      806 2023-07-26 22:43:31.060942 gwcelery-2.1.4/gwcelery/tests/data/kafka_alert_swift.json
--rw-r--r--   0        0        0      743 2023-07-26 22:43:31.061942 gwcelery-2.1.4/gwcelery/tests/data/kafka_alert_swift_noloc.json
--rw-r--r--   0        0        0  1037630 2023-07-26 22:43:31.079942 gwcelery-2.1.4/gwcelery/tests/data/kafka_alert_swift_wskymap.json
--rw-r--r--   0        0        0        0 2023-07-26 22:43:31.260943 gwcelery-2.1.4/gwcelery/tests/data/llhoft/__init__.py
--rw-r--r--   0        0        0     8267 2023-07-26 22:43:31.082942 gwcelery-2.1.4/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-07-26 22:43:31.261943 gwcelery-2.1.4/gwcelery/tests/data/llhoft/fail/L1/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 22:43:31.261943 gwcelery-2.1.4/gwcelery/tests/data/llhoft/fail/__init__.py
--rw-r--r--   0        0        0    14942 2023-07-26 22:43:31.083942 gwcelery-2.1.4/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-07-26 22:43:31.261943 gwcelery-2.1.4/gwcelery/tests/data/llhoft/omegascan/__init__.py
--rw-r--r--   0        0        0   516419 2023-07-26 22:43:31.086942 gwcelery-2.1.4/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
--rw-r--r--   0        0        0    14950 2023-07-26 22:43:31.086942 gwcelery-2.1.4/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-07-26 22:43:31.261943 gwcelery-2.1.4/gwcelery/tests/data/llhoft/pass/H1/__init__.py
--rw-r--r--   0        0        0        0 2023-07-26 22:43:31.261943 gwcelery-2.1.4/gwcelery/tests/data/llhoft/pass/__init__.py
--rw-r--r--   0        0        0    13099 2023-07-26 22:43:31.087942 gwcelery-2.1.4/gwcelery/tests/data/lvalert_event_creation.json
--rw-r--r--   0        0        0     9060 2023-07-26 22:43:31.087942 gwcelery-2.1.4/gwcelery/tests/data/lvalert_xmpp.xml
--rw-r--r--   0        0        0      864 2023-07-26 22:43:31.087942 gwcelery-2.1.4/gwcelery/tests/data/mock_superevent_object.json
--rw-r--r--   0        0        0   445440 2023-07-26 22:43:31.091942 gwcelery-2.1.4/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
--rw-r--r--   0        0        0   294426 2023-07-26 22:43:31.094942 gwcelery-2.1.4/gwcelery/tests/data/psd.xml.gz
--rw-r--r--   0        0        0    11520 2023-07-26 22:43:31.095942 gwcelery-2.1.4/gwcelery/tests/data/rrt_small_area.fits
--rw-r--r--   0        0        0     2964 2023-07-26 22:43:31.095942 gwcelery-2.1.4/gwcelery/tests/data/sample_events.json
--rw-r--r--   0        0        0     3648 2023-07-26 22:43:31.095942 gwcelery-2.1.4/gwcelery/tests/data/samples.hdf5
--rw-r--r--   0        0        0      616 2023-07-26 22:43:31.095942 gwcelery-2.1.4/gwcelery/tests/data/scaler_set_all.pickle
--rw-r--r--   0        0        0     6169 2023-07-26 22:43:31.095942 gwcelery-2.1.4/gwcelery/tests/data/snews_gcn.xml
--rw-r--r--   0        0        0     6161 2023-07-26 22:43:31.096942 gwcelery-2.1.4/gwcelery/tests/data/snews_gcn_test.xml
--rw-r--r--   0        0        0     9583 2023-07-26 22:43:31.096942 gwcelery-2.1.4/gwcelery/tests/data/superevents.json
--rw-r--r--   0        0        0     7713 2023-07-26 22:43:31.096942 gwcelery-2.1.4/gwcelery/tests/data/swift_grb_gcn.xml
--rw-r--r--   0        0        0     1962 2023-07-26 22:43:31.096942 gwcelery-2.1.4/gwcelery/tests/data/swift_subgrbtargeted_template.xml
--rw-r--r--   0        0        0   581918 2023-07-26 22:43:31.102942 gwcelery-2.1.4/gwcelery/tests/data/test_classifier.pickle
--rw-r--r--   0        0        0     4042 2023-07-26 22:43:31.103942 gwcelery-2.1.4/gwcelery/tests/process.py
--rw-r--r--   0        0        0     2307 2023-07-26 22:43:31.103942 gwcelery-2.1.4/gwcelery/tests/test_sentry.py
--rw-r--r--   0        0        0     1705 2023-07-26 22:43:31.103942 gwcelery-2.1.4/gwcelery/tests/test_tasks_alerts.py
--rw-r--r--   0        0        0     4916 2023-07-26 22:43:31.103942 gwcelery-2.1.4/gwcelery/tests/test_tasks_alerts_validate.py
--rw-r--r--   0        0        0     1439 2023-07-26 22:43:31.104942 gwcelery-2.1.4/gwcelery/tests/test_tasks_bayestar.py
--rw-r--r--   0        0        0     3007 2023-07-26 22:43:31.104942 gwcelery-2.1.4/gwcelery/tests/test_tasks_circulars.py
--rw-r--r--   0        0        0     4550 2023-07-26 22:43:31.104942 gwcelery-2.1.4/gwcelery/tests/test_tasks_condor.py
--rw-r--r--   0        0        0    16937 2023-07-26 22:43:31.105942 gwcelery-2.1.4/gwcelery/tests/test_tasks_detchar.py
--rw-r--r--   0        0        0     2317 2023-07-26 22:43:31.105942 gwcelery-2.1.4/gwcelery/tests/test_tasks_em_bright.py
--rw-r--r--   0        0        0    13802 2023-07-26 22:43:31.106942 gwcelery-2.1.4/gwcelery/tests/test_tasks_external_skymaps.py
--rw-r--r--   0        0        0    40706 2023-07-26 22:43:31.106942 gwcelery-2.1.4/gwcelery/tests/test_tasks_external_triggers.py
--rw-r--r--   0        0        0     1816 2023-07-26 22:43:31.107942 gwcelery-2.1.4/gwcelery/tests/test_tasks_first2years.py
--rw-r--r--   0        0        0     4584 2023-07-26 22:43:31.107942 gwcelery-2.1.4/gwcelery/tests/test_tasks_first2years_external.py
--rw-r--r--   0        0        0     1826 2023-07-26 22:43:31.107942 gwcelery-2.1.4/gwcelery/tests/test_tasks_gcn.py
--rw-r--r--   0        0        0     1655 2023-07-26 22:43:31.107942 gwcelery-2.1.4/gwcelery/tests/test_tasks_gcn_validate.py
--rw-r--r--   0        0        0     5739 2023-07-26 22:43:31.108942 gwcelery-2.1.4/gwcelery/tests/test_tasks_gracedb.py
--rw-r--r--   0        0        0     9591 2023-07-26 22:43:31.108942 gwcelery-2.1.4/gwcelery/tests/test_tasks_gwskynet.py
--rw-r--r--   0        0        0     3662 2023-07-26 22:43:31.109942 gwcelery-2.1.4/gwcelery/tests/test_tasks_igwn_alert.py
--rw-r--r--   0        0        0    26701 2023-07-26 22:43:31.110942 gwcelery-2.1.4/gwcelery/tests/test_tasks_inference.py
--rw-r--r--   0        0        0    36838 2023-07-26 22:43:31.110942 gwcelery-2.1.4/gwcelery/tests/test_tasks_orchestrator.py
--rw-r--r--   0        0        0     1647 2023-07-26 22:43:31.110942 gwcelery-2.1.4/gwcelery/tests/test_tasks_p_astro.py
--rw-r--r--   0        0        0    26081 2023-07-26 22:43:31.111942 gwcelery-2.1.4/gwcelery/tests/test_tasks_raven.py
--rw-r--r--   0        0        0     4724 2023-07-26 22:43:31.111942 gwcelery-2.1.4/gwcelery/tests/test_tasks_rrt_utils.py
--rw-r--r--   0        0        0     5035 2023-07-26 22:43:31.112942 gwcelery-2.1.4/gwcelery/tests/test_tasks_skymaps.py
--rw-r--r--   0        0        0    40274 2023-07-26 22:43:31.112942 gwcelery-2.1.4/gwcelery/tests/test_tasks_superevents.py
--rw-r--r--   0        0        0      637 2023-07-26 22:43:31.112942 gwcelery-2.1.4/gwcelery/tests/test_tempfile.py
--rw-r--r--   0        0        0     3520 2023-07-26 22:43:31.113942 gwcelery-2.1.4/gwcelery/tests/test_tools_condor.py
--rw-r--r--   0        0        0     1098 2023-07-26 22:43:31.113942 gwcelery-2.1.4/gwcelery/tests/test_tools_condor_submit_helper.py
--rw-r--r--   0        0        0      633 2023-07-26 22:43:31.113942 gwcelery-2.1.4/gwcelery/tests/test_tools_flask.py
--rw-r--r--   0        0        0    10579 2023-07-26 22:43:31.114942 gwcelery-2.1.4/gwcelery/tests/test_tools_nagios.py
--rw-r--r--   0        0        0      269 2023-07-26 22:43:31.114942 gwcelery-2.1.4/gwcelery/tests/test_util.py
--rw-r--r--   0        0        0    22656 2023-07-26 22:43:31.115942 gwcelery-2.1.4/gwcelery/tests/test_views.py
--rw-r--r--   0        0        0      216 2023-07-26 22:43:31.115942 gwcelery-2.1.4/gwcelery/tools/__init__.py
--rw-r--r--   0        0        0     2948 2023-07-26 22:43:31.116942 gwcelery-2.1.4/gwcelery/tools/condor.py
--rw-r--r--   0        0        0     1120 2023-07-26 22:43:31.116942 gwcelery-2.1.4/gwcelery/tools/condor_submit_helper.py
--rw-r--r--   0        0        0     1938 2023-07-26 22:43:31.116942 gwcelery-2.1.4/gwcelery/tools/flask.py
--rw-r--r--   0        0        0     7898 2023-07-26 22:43:31.117942 gwcelery-2.1.4/gwcelery/tools/nagios.py
--rw-r--r--   0        0        0      413 2023-07-26 22:43:31.117942 gwcelery-2.1.4/gwcelery/util/__init__.py
--rw-r--r--   0        0        0     1007 2023-07-26 22:43:31.117942 gwcelery-2.1.4/gwcelery/util/cmdline.py
--rw-r--r--   0        0        0      453 2023-07-26 22:43:31.118942 gwcelery-2.1.4/gwcelery/util/matplotlib.py
--rw-r--r--   0        0        0      390 2023-07-26 22:43:31.118942 gwcelery-2.1.4/gwcelery/util/proxy.py
--rw-r--r--   0        0        0      514 2023-07-26 22:43:31.118942 gwcelery-2.1.4/gwcelery/util/resources.py
--rw-r--r--   0        0        0      253 2023-07-26 22:43:31.118942 gwcelery-2.1.4/gwcelery/util/sphinx.py
--rw-r--r--   0        0        0      941 2023-07-26 22:43:31.118942 gwcelery-2.1.4/gwcelery/util/tempfile.py
--rw-r--r--   0        0        0    19407 2023-07-26 22:43:31.119942 gwcelery-2.1.4/gwcelery/views.py
--rw-r--r--   0        0        0      365 2023-07-26 22:43:31.120942 gwcelery-2.1.4/gwcelery/voevent/__init__.py
--rw-r--r--   0        0        0     6387 2023-07-26 22:43:31.120942 gwcelery-2.1.4/gwcelery/voevent/bootsteps.py
--rw-r--r--   0        0        0     1063 2023-07-26 22:43:31.120942 gwcelery-2.1.4/gwcelery/voevent/logging.py
--rw-r--r--   0        0        0      779 2023-07-26 22:43:31.120942 gwcelery-2.1.4/gwcelery/voevent/signals.py
--rw-r--r--   0        0        0      852 2023-07-26 22:43:31.121942 gwcelery-2.1.4/gwcelery/voevent/subscriber.py
--rw-r--r--   0        0        0     1454 2023-07-26 22:43:31.121942 gwcelery-2.1.4/gwcelery/voevent/util.py
--rw-r--r--   0        0        0     6099 2023-07-26 22:43:58.200040 gwcelery-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     4530 1970-01-01 00:00:00.000000 gwcelery-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0    99692 2023-08-01 20:37:01.547901 gwcelery-2.1.5/CHANGES.rst
+-rw-r--r--   0        0        0       64 2023-08-01 20:37:01.547901 gwcelery-2.1.5/CONTRIBUTING.rst
+-rw-r--r--   0        0        0    19716 2023-08-01 20:37:01.548901 gwcelery-2.1.5/LICENSE.rst
+-rw-r--r--   0        0        0     1351 2023-08-01 20:37:01.549901 gwcelery-2.1.5/README.rst
+-rw-r--r--   0        0        0      634 2023-08-01 20:37:01.549901 gwcelery-2.1.5/doc/Makefile
+-rw-r--r--   0        0        0   191486 2023-08-01 20:37:01.553901 gwcelery-2.1.5/doc/_static/acceptance-tests-checklist.png
+-rw-r--r--   0        0        0   241593 2023-08-01 20:37:01.557901 gwcelery-2.1.5/doc/_static/celeryevent-screenshot.png
+-rw-r--r--   0        0        0   206465 2023-08-01 20:37:01.562901 gwcelery-2.1.5/doc/_static/deployment-screenshot.png
+-rw-r--r--   0        0        0   161306 2023-08-01 20:37:01.566901 gwcelery-2.1.5/doc/_static/flask-screenshot.png
+-rw-r--r--   0        0        0   328056 2023-08-01 20:37:01.573901 gwcelery-2.1.5/doc/_static/flower-screenshot.png
+-rw-r--r--   0        0        0   114719 2023-08-01 20:37:01.576901 gwcelery-2.1.5/doc/_static/logo-0.5x.png
+-rw-r--r--   0        0        0   351955 2023-08-01 20:37:01.583901 gwcelery-2.1.5/doc/_static/logo.png
+-rw-r--r--   0        0        0   230777 2023-08-01 20:37:01.589901 gwcelery-2.1.5/doc/_static/sentry-screenshot.png
+-rwxr-xr-x   0        0        0     7356 2023-08-01 20:37:01.589901 gwcelery-2.1.5/doc/conf.py
+-rw-r--r--   0        0        0     4346 2023-08-01 20:37:01.590901 gwcelery-2.1.5/doc/configuration.rst
+-rw-r--r--   0        0        0     5698 2023-08-01 20:37:01.590901 gwcelery-2.1.5/doc/contributing.rst
+-rw-r--r--   0        0        0     7202 2023-08-01 20:37:01.591901 gwcelery-2.1.5/doc/deployment.rst
+-rw-r--r--   0        0        0    10176 2023-08-01 20:37:01.591901 gwcelery-2.1.5/doc/design.rst
+-rw-r--r--   0        0        0      486 2023-08-01 20:37:01.592901 gwcelery-2.1.5/doc/gwcelery.conf.rst
+-rw-r--r--   0        0        0      284 2023-08-01 20:37:01.592901 gwcelery-2.1.5/doc/gwcelery.email.rst
+-rw-r--r--   0        0        0      329 2023-08-01 20:37:01.592901 gwcelery-2.1.5/doc/gwcelery.igwn_alert.rst
+-rw-r--r--   0        0        0      227 2023-08-01 20:37:01.592901 gwcelery-2.1.5/doc/gwcelery.rst
+-rw-r--r--   0        0        0       79 2023-08-01 20:37:01.592901 gwcelery-2.1.5/doc/gwcelery.sentry.rst
+-rw-r--r--   0        0        0       97 2023-08-01 20:37:01.593901 gwcelery-2.1.5/doc/gwcelery.tasks.alerts.rst
+-rw-r--r--   0        0        0      103 2023-08-01 20:37:01.593901 gwcelery-2.1.5/doc/gwcelery.tasks.bayestar.rst
+-rw-r--r--   0        0        0      107 2023-08-01 20:37:01.593901 gwcelery-2.1.5/doc/gwcelery.tasks.circulars.rst
+-rw-r--r--   0        0        0       98 2023-08-01 20:37:01.593901 gwcelery-2.1.5/doc/gwcelery.tasks.condor.rst
+-rw-r--r--   0        0        0     2404 2023-08-01 20:37:01.593901 gwcelery-2.1.5/doc/gwcelery.tasks.detchar.rst
+-rw-r--r--   0        0        0     1110 2023-08-01 20:37:01.594901 gwcelery-2.1.5/doc/gwcelery.tasks.em_bright.rst
+-rw-r--r--   0        0        0      129 2023-08-01 20:37:01.594901 gwcelery-2.1.5/doc/gwcelery.tasks.external_skymaps.rst
+-rw-r--r--   0        0        0     6738 2023-08-01 20:37:01.594901 gwcelery-2.1.5/doc/gwcelery.tasks.external_triggers.rst
+-rw-r--r--   0        0        0      112 2023-08-01 20:37:01.594901 gwcelery-2.1.5/doc/gwcelery.tasks.first2years.rst
+-rw-r--r--   0        0        0       88 2023-08-01 20:37:01.595901 gwcelery-2.1.5/doc/gwcelery.tasks.gcn.rst
+-rw-r--r--   0        0        0      100 2023-08-01 20:37:01.595901 gwcelery-2.1.5/doc/gwcelery.tasks.gracedb.rst
+-rw-r--r--   0        0        0      109 2023-08-01 20:37:01.595901 gwcelery-2.1.5/doc/gwcelery.tasks.igwn_alert.rst
+-rw-r--r--   0        0        0      109 2023-08-01 20:37:01.595901 gwcelery-2.1.5/doc/gwcelery.tasks.inference.rst
+-rw-r--r--   0        0        0     8111 2023-08-01 20:37:01.596901 gwcelery-2.1.5/doc/gwcelery.tasks.orchestrator.rst
+-rw-r--r--   0        0        0      100 2023-08-01 20:37:01.596901 gwcelery-2.1.5/doc/gwcelery.tasks.p_astro.rst
+-rw-r--r--   0        0        0       94 2023-08-01 20:37:01.596901 gwcelery-2.1.5/doc/gwcelery.tasks.raven.rst
+-rw-r--r--   0        0        0      628 2023-08-01 20:37:01.596901 gwcelery-2.1.5/doc/gwcelery.tasks.rst
+-rw-r--r--   0        0        0      100 2023-08-01 20:37:01.596901 gwcelery-2.1.5/doc/gwcelery.tasks.skymaps.rst
+-rw-r--r--   0        0        0     7161 2023-08-01 20:37:01.597901 gwcelery-2.1.5/doc/gwcelery.tasks.superevents.rst
+-rw-r--r--   0        0        0       97 2023-08-01 20:37:01.597901 gwcelery-2.1.5/doc/gwcelery.tools.condor.rst
+-rw-r--r--   0        0        0       94 2023-08-01 20:37:01.597901 gwcelery-2.1.5/doc/gwcelery.tools.flask.rst
+-rw-r--r--   0        0        0       97 2023-08-01 20:37:01.597901 gwcelery-2.1.5/doc/gwcelery.tools.nagios.rst
+-rw-r--r--   0        0        0      185 2023-08-01 20:37:01.597901 gwcelery-2.1.5/doc/gwcelery.tools.rst
+-rw-r--r--   0        0        0       73 2023-08-01 20:37:01.598901 gwcelery-2.1.5/doc/gwcelery.util.rst
+-rw-r--r--   0        0        0      507 2023-08-01 20:37:01.598901 gwcelery-2.1.5/doc/gwcelery.voevent.rst
+-rw-r--r--   0        0        0     3564 2023-08-01 20:37:01.598901 gwcelery-2.1.5/doc/htcondor.rst
+-rw-r--r--   0        0        0     1576 2023-08-01 20:37:01.598901 gwcelery-2.1.5/doc/index.rst
+-rw-r--r--   0        0        0      800 2023-08-01 20:37:01.599901 gwcelery-2.1.5/doc/make.bat
+-rw-r--r--   0        0        0     4416 2023-08-01 20:37:01.599901 gwcelery-2.1.5/doc/monitoring.rst
+-rw-r--r--   0        0        0     5312 2023-08-01 20:37:01.599901 gwcelery-2.1.5/doc/quickstart.rst
+-rw-r--r--   0        0        0     1149 2023-08-01 20:37:01.600901 gwcelery-2.1.5/gwcelery/__init__.py
+-rw-r--r--   0        0        0    18447 2023-08-01 20:37:01.600901 gwcelery-2.1.5/gwcelery/_version.py
+-rw-r--r--   0        0        0    16852 2023-08-01 20:37:01.601901 gwcelery-2.1.5/gwcelery/conf/__init__.py
+-rw-r--r--   0        0        0     1014 2023-08-01 20:37:01.601901 gwcelery-2.1.5/gwcelery/conf/dev.py
+-rw-r--r--   0        0        0      403 2023-08-01 20:37:01.602901 gwcelery-2.1.5/gwcelery/conf/development.py
+-rw-r--r--   0        0        0     1289 2023-08-01 20:37:01.602901 gwcelery-2.1.5/gwcelery/conf/minikube.py
+-rw-r--r--   0        0        0     1865 2023-08-01 20:37:01.602901 gwcelery-2.1.5/gwcelery/conf/playground.py
+-rw-r--r--   0        0        0     3507 2023-08-01 20:37:01.602901 gwcelery-2.1.5/gwcelery/conf/production.py
+-rw-r--r--   0        0        0     2040 2023-08-01 20:37:01.603901 gwcelery-2.1.5/gwcelery/conf/test.py
+-rw-r--r--   0        0        0        0 2023-08-01 20:37:01.936901 gwcelery-2.1.5/gwcelery/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 20:37:01.939901 gwcelery-2.1.5/gwcelery/data/first2years/__init__.py
+-rw-r--r--   0        0        0   731421 2023-08-01 20:37:01.611901 gwcelery-2.1.5/gwcelery/data/first2years/gstlal.xml.gz
+-rwxr-xr-x   0        0        0     2999 2023-08-01 20:37:01.612901 gwcelery-2.1.5/gwcelery/data/gwcelery.sub
+-rw-r--r--   0        0        0      505 2023-08-01 20:37:01.612901 gwcelery-2.1.5/gwcelery/email/__init__.py
+-rw-r--r--   0        0        0     3317 2023-08-01 20:37:01.613901 gwcelery-2.1.5/gwcelery/email/bootsteps.py
+-rw-r--r--   0        0        0      995 2023-08-01 20:37:01.613901 gwcelery-2.1.5/gwcelery/email/signals.py
+-rw-r--r--   0        0        0     1457 2023-08-01 20:37:01.613901 gwcelery-2.1.5/gwcelery/flask.py
+-rw-r--r--   0        0        0      529 2023-08-01 20:37:01.614901 gwcelery-2.1.5/gwcelery/igwn_alert/__init__.py
+-rw-r--r--   0        0        0     4484 2023-08-01 20:37:01.614901 gwcelery-2.1.5/gwcelery/igwn_alert/bootsteps.py
+-rw-r--r--   0        0        0      608 2023-08-01 20:37:01.614901 gwcelery-2.1.5/gwcelery/igwn_alert/signals.py
+-rw-r--r--   0        0        0      275 2023-08-01 20:37:01.615901 gwcelery-2.1.5/gwcelery/jinja.py
+-rw-r--r--   0        0        0      305 2023-08-01 20:37:01.615901 gwcelery-2.1.5/gwcelery/kafka/__init__.py
+-rw-r--r--   0        0        0    11838 2023-08-01 20:37:01.615901 gwcelery-2.1.5/gwcelery/kafka/bootsteps.py
+-rw-r--r--   0        0        0      522 2023-08-01 20:37:01.616901 gwcelery-2.1.5/gwcelery/kafka/signals.py
+-rw-r--r--   0        0        0     2567 2023-08-01 20:37:01.616901 gwcelery-2.1.5/gwcelery/sentry/__init__.py
+-rw-r--r--   0        0        0       34 2023-08-01 20:37:01.617901 gwcelery-2.1.5/gwcelery/sentry/integrations/__init__.py
+-rw-r--r--   0        0        0      832 2023-08-01 20:37:01.617901 gwcelery-2.1.5/gwcelery/sentry/integrations/condor.py
+-rw-r--r--   0        0        0      836 2023-08-01 20:37:01.617901 gwcelery-2.1.5/gwcelery/sentry/integrations/requests.py
+-rw-r--r--   0        0        0      939 2023-08-01 20:37:01.617901 gwcelery-2.1.5/gwcelery/sentry/integrations/subprocess.py
+-rw-r--r--   0        0        0     1302 2023-08-01 20:37:01.617901 gwcelery-2.1.5/gwcelery/static/typeahead.css
+-rw-r--r--   0        0        0     4124 2023-08-01 20:37:01.618901 gwcelery-2.1.5/gwcelery/static/vega/index.html
+-rw-r--r--   0        0        0      515 2023-08-01 20:37:01.618901 gwcelery-2.1.5/gwcelery/tasks/__init__.py
+-rw-r--r--   0        0        0    13633 2023-08-01 20:37:01.619901 gwcelery-2.1.5/gwcelery/tasks/alerts.py
+-rw-r--r--   0        0        0     2672 2023-08-01 20:37:01.619901 gwcelery-2.1.5/gwcelery/tasks/bayestar.py
+-rw-r--r--   0        0        0     1535 2023-08-01 20:37:01.619901 gwcelery-2.1.5/gwcelery/tasks/circulars.py
+-rw-r--r--   0        0        0     7502 2023-08-01 20:37:01.620901 gwcelery-2.1.5/gwcelery/tasks/condor.py
+-rw-r--r--   0        0        0     2692 2023-08-01 20:37:01.620901 gwcelery-2.1.5/gwcelery/tasks/core.py
+-rw-r--r--   0        0        0    22989 2023-08-01 20:37:01.621901 gwcelery-2.1.5/gwcelery/tasks/detchar.py
+-rw-r--r--   0        0        0     4865 2023-08-01 20:37:01.621901 gwcelery-2.1.5/gwcelery/tasks/em_bright.py
+-rw-r--r--   0        0        0    23428 2023-08-01 20:37:01.622901 gwcelery-2.1.5/gwcelery/tasks/external_skymaps.py
+-rw-r--r--   0        0        0    29099 2023-08-01 20:37:01.623901 gwcelery-2.1.5/gwcelery/tasks/external_triggers.py
+-rw-r--r--   0        0        0     6832 2023-08-01 20:37:01.623901 gwcelery-2.1.5/gwcelery/tasks/first2years.py
+-rw-r--r--   0        0        0     6320 2023-08-01 20:37:01.623901 gwcelery-2.1.5/gwcelery/tasks/first2years_external.py
+-rw-r--r--   0        0        0     4831 2023-08-01 20:37:01.624901 gwcelery-2.1.5/gwcelery/tasks/gcn.py
+-rw-r--r--   0        0        0    11079 2023-08-01 20:37:01.624901 gwcelery-2.1.5/gwcelery/tasks/gracedb.py
+-rw-r--r--   0        0        0     6105 2023-08-01 20:37:01.625901 gwcelery-2.1.5/gwcelery/tasks/gwskynet.py
+-rw-r--r--   0        0        0     2453 2023-08-01 20:37:01.625901 gwcelery-2.1.5/gwcelery/tasks/igwn_alert.py
+-rw-r--r--   0        0        0    34213 2023-08-01 20:37:01.626901 gwcelery-2.1.5/gwcelery/tasks/inference.py
+-rw-r--r--   0        0        0     1406 2023-08-01 20:37:01.626901 gwcelery-2.1.5/gwcelery/tasks/legacy_gracedb.py
+-rw-r--r--   0        0        0     7772 2023-08-01 20:37:01.627901 gwcelery-2.1.5/gwcelery/tasks/notice_text.py
+-rw-r--r--   0        0        0    48026 2023-08-01 20:37:01.628901 gwcelery-2.1.5/gwcelery/tasks/orchestrator.py
+-rw-r--r--   0        0        0     5796 2023-08-01 20:37:01.628901 gwcelery-2.1.5/gwcelery/tasks/p_astro.py
+-rw-r--r--   0        0        0    21540 2023-08-01 20:37:01.629901 gwcelery-2.1.5/gwcelery/tasks/raven.py
+-rw-r--r--   0        0        0     2242 2023-08-01 20:37:01.629901 gwcelery-2.1.5/gwcelery/tasks/rrt_utils.py
+-rw-r--r--   0        0        0    12528 2023-08-01 20:37:01.630901 gwcelery-2.1.5/gwcelery/tasks/skymaps.py
+-rw-r--r--   0        0        0    23631 2023-08-01 20:37:01.631901 gwcelery-2.1.5/gwcelery/tasks/superevents.py
+-rw-r--r--   0        0        0     1084 2023-08-01 20:37:01.632901 gwcelery-2.1.5/gwcelery/templates/fits_header.jinja2
+-rw-r--r--   0        0        0    35556 2023-08-01 20:37:01.633901 gwcelery-2.1.5/gwcelery/templates/index.jinja2
+-rw-r--r--   0        0        0     8505 2023-08-01 20:37:01.633901 gwcelery-2.1.5/gwcelery/templates/lalinference.jinja2
+-rw-r--r--   0        0        0     9442 2023-08-01 20:37:01.634901 gwcelery-2.1.5/gwcelery/templates/rapidpe.jinja2
+-rw-r--r--   0        0        0      472 2023-08-01 20:37:01.634901 gwcelery-2.1.5/gwcelery/templates/vector_table.jinja2
+-rw-r--r--   0        0        0        0 2023-08-01 20:37:01.944901 gwcelery-2.1.5/gwcelery/tests/__init__.py
+-rw-r--r--   0        0        0     4388 2023-08-01 20:37:01.634901 gwcelery-2.1.5/gwcelery/tests/conftest.py
+-rw-r--r--   0        0        0      976 2023-08-01 20:37:01.635901 gwcelery-2.1.5/gwcelery/tests/data/G000012_S0040_preferred.json
+-rw-r--r--   0        0        0     6258 2023-08-01 20:37:01.635901 gwcelery-2.1.5/gwcelery/tests/data/G298048-1-Initial.xml
+-rw-r--r--   0        0        0      599 2023-08-01 20:37:01.636901 gwcelery-2.1.5/gwcelery/tests/data/G298048_log.json
+-rw-r--r--   0        0        0      150 2023-08-01 20:37:01.636901 gwcelery-2.1.5/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
+-rw-r--r--   0        0        0      974 2023-08-01 20:37:01.636901 gwcelery-2.1.5/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
+-rw-r--r--   0        0        0    17572 2023-08-01 20:37:01.636901 gwcelery-2.1.5/gwcelery/tests/data/MS220722v.xml
+-rw-r--r--   0        0        0   777600 2023-08-01 20:37:01.654901 gwcelery-2.1.5/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
+-rw-r--r--   0        0        0     8220 2023-08-01 20:37:01.655901 gwcelery-2.1.5/gwcelery/tests/data/S230413b.json
+-rw-r--r--   0        0        0     7255 2023-08-01 20:37:01.655901 gwcelery-2.1.5/gwcelery/tests/data/S230413g.json
+-rw-r--r--   0        0        0     7721 2023-08-01 20:37:01.655901 gwcelery-2.1.5/gwcelery/tests/data/S230413h.json
+-rw-r--r--   0        0        0     3387 2023-08-01 20:37:01.656901 gwcelery-2.1.5/gwcelery/tests/data/T0212_S0039_preferred.json
+-rw-r--r--   0        0        0     3384 2023-08-01 20:37:01.656901 gwcelery-2.1.5/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
+-rw-r--r--   0        0        0     5210 2023-08-01 20:37:01.656901 gwcelery-2.1.5/gwcelery/tests/data/T0219_S0041_nopreferred.json
+-rw-r--r--   0        0        0        0 2023-08-01 20:37:01.945901 gwcelery-2.1.5/gwcelery/tests/data/__init__.py
+-rw-r--r--   0        0        0     2290 2023-08-01 20:37:01.657901 gwcelery-2.1.5/gwcelery/tests/data/agile_grb_gcn.xml
+-rw-r--r--   0        0        0   854036 2023-08-01 20:37:01.674901 gwcelery-2.1.5/gwcelery/tests/data/coinc.xml
+-rw-r--r--   0        0        0     6175 2023-08-01 20:37:01.674901 gwcelery-2.1.5/gwcelery/tests/data/externaltrigger_original_data.xml
+-rw-r--r--   0        0        0     5482 2023-08-01 20:37:01.675901 gwcelery-2.1.5/gwcelery/tests/data/fermi_grb_gcn.xml
+-rw-r--r--   0        0        0     5469 2023-08-01 20:37:01.675901 gwcelery-2.1.5/gwcelery/tests/data/fermi_initial_grb_gcn.xml
+-rw-r--r--   0        0        0     5865 2023-08-01 20:37:01.675901 gwcelery-2.1.5/gwcelery/tests/data/fermi_noise_gcn.xml
+-rw-r--r--   0        0        0     5864 2023-08-01 20:37:01.676901 gwcelery-2.1.5/gwcelery/tests/data/fermi_noise_gcn_2.xml
+-rw-r--r--   0        0        0     1914 2023-08-01 20:37:01.676901 gwcelery-2.1.5/gwcelery/tests/data/fermi_subgrbtargeted_template.xml
+-rw-r--r--   0        0        0     4914 2023-08-01 20:37:01.676901 gwcelery-2.1.5/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
+-rw-r--r--   0        0        0     4914 2023-08-01 20:37:01.677901 gwcelery-2.1.5/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
+-rw-r--r--   0        0        0     3407 2023-08-01 20:37:01.677901 gwcelery-2.1.5/gwcelery/tests/data/fits_header_result.html
+-rw-r--r--   0        0        0      882 2023-08-01 20:37:01.677901 gwcelery-2.1.5/gwcelery/tests/data/gracedb_externaltrigger_log.json
+-rw-r--r--   0        0        0      446 2023-08-01 20:37:01.677901 gwcelery-2.1.5/gwcelery/tests/data/gracedb_setrigger_log.json
+-rw-r--r--   0        0        0      870 2023-08-01 20:37:01.678901 gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_detchar.json
+-rw-r--r--   0        0        0     2025 2023-08-01 20:37:01.678901 gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_exttrig_creation.json
+-rw-r--r--   0        0        0     2007 2023-08-01 20:37:01.678901 gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
+-rw-r--r--   0        0        0      166 2023-08-01 20:37:01.679901 gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_fits.json
+-rw-r--r--   0        0        0      101 2023-08-01 20:37:01.679901 gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_label_dqv.json
+-rw-r--r--   0        0        0      743 2023-08-01 20:37:01.679901 gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_psd.json
+-rw-r--r--   0        0        0     2020 2023-08-01 20:37:01.679901 gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_snews_creation.json
+-rw-r--r--   0        0        0     2012 2023-08-01 20:37:01.680901 gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_snews_test_creation.json
+-rw-r--r--   0        0        0     2028 2023-08-01 20:37:01.680901 gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_subgrb_creation.json
+-rw-r--r--   0        0        0     1235 2023-08-01 20:37:01.680901 gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_superevent_creation.json
+-rw-r--r--   0        0        0      107 2023-08-01 20:37:01.680901 gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_superevent_label.json
+-rw-r--r--   0        0        0     5021 2023-08-01 20:37:01.681901 gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_voevent.json
+-rw-r--r--   0        0        0     4429 2023-08-01 20:37:01.681901 gwcelery-2.1.5/gwcelery/tests/data/integral_grb_gcn.xml
+-rw-r--r--   0        0        0     4295 2023-08-01 20:37:01.682901 gwcelery-2.1.5/gwcelery/tests/data/integral_mdc_gcn.xml
+-rw-r--r--   0        0        0  1038044 2023-08-01 20:37:01.705901 gwcelery-2.1.5/gwcelery/tests/data/kafka_alert_fermi.json
+-rw-r--r--   0        0        0  1038042 2023-08-01 20:37:01.732901 gwcelery-2.1.5/gwcelery/tests/data/kafka_alert_fermi_ignore.json
+-rw-r--r--   0        0        0      806 2023-08-01 20:37:01.733901 gwcelery-2.1.5/gwcelery/tests/data/kafka_alert_swift.json
+-rw-r--r--   0        0        0      743 2023-08-01 20:37:01.733901 gwcelery-2.1.5/gwcelery/tests/data/kafka_alert_swift_noloc.json
+-rw-r--r--   0        0        0  1037630 2023-08-01 20:37:01.757901 gwcelery-2.1.5/gwcelery/tests/data/kafka_alert_swift_wskymap.json
+-rw-r--r--   0        0        0        0 2023-08-01 20:37:01.951901 gwcelery-2.1.5/gwcelery/tests/data/llhoft/__init__.py
+-rw-r--r--   0        0        0     8267 2023-08-01 20:37:01.760901 gwcelery-2.1.5/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-08-01 20:37:01.951901 gwcelery-2.1.5/gwcelery/tests/data/llhoft/fail/L1/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 20:37:01.951901 gwcelery-2.1.5/gwcelery/tests/data/llhoft/fail/__init__.py
+-rw-r--r--   0        0        0    14942 2023-08-01 20:37:01.761901 gwcelery-2.1.5/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-08-01 20:37:01.952901 gwcelery-2.1.5/gwcelery/tests/data/llhoft/omegascan/__init__.py
+-rw-r--r--   0        0        0   516419 2023-08-01 20:37:01.765901 gwcelery-2.1.5/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
+-rw-r--r--   0        0        0    14950 2023-08-01 20:37:01.766901 gwcelery-2.1.5/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-08-01 20:37:01.952901 gwcelery-2.1.5/gwcelery/tests/data/llhoft/pass/H1/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 20:37:01.952901 gwcelery-2.1.5/gwcelery/tests/data/llhoft/pass/__init__.py
+-rw-r--r--   0        0        0    13099 2023-08-01 20:37:01.766901 gwcelery-2.1.5/gwcelery/tests/data/lvalert_event_creation.json
+-rw-r--r--   0        0        0     9060 2023-08-01 20:37:01.767901 gwcelery-2.1.5/gwcelery/tests/data/lvalert_xmpp.xml
+-rw-r--r--   0        0        0      864 2023-08-01 20:37:01.767901 gwcelery-2.1.5/gwcelery/tests/data/mock_superevent_object.json
+-rw-r--r--   0        0        0   445440 2023-08-01 20:37:01.772901 gwcelery-2.1.5/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
+-rw-r--r--   0        0        0   294426 2023-08-01 20:37:01.776901 gwcelery-2.1.5/gwcelery/tests/data/psd.xml.gz
+-rw-r--r--   0        0        0    11520 2023-08-01 20:37:01.777901 gwcelery-2.1.5/gwcelery/tests/data/rrt_small_area.fits
+-rw-r--r--   0        0        0     2964 2023-08-01 20:37:01.777901 gwcelery-2.1.5/gwcelery/tests/data/sample_events.json
+-rw-r--r--   0        0        0     3648 2023-08-01 20:37:01.777901 gwcelery-2.1.5/gwcelery/tests/data/samples.hdf5
+-rw-r--r--   0        0        0      616 2023-08-01 20:37:01.778901 gwcelery-2.1.5/gwcelery/tests/data/scaler_set_all.pickle
+-rw-r--r--   0        0        0     6169 2023-08-01 20:37:01.778901 gwcelery-2.1.5/gwcelery/tests/data/snews_gcn.xml
+-rw-r--r--   0        0        0     6161 2023-08-01 20:37:01.778901 gwcelery-2.1.5/gwcelery/tests/data/snews_gcn_test.xml
+-rw-r--r--   0        0        0     9583 2023-08-01 20:37:01.778901 gwcelery-2.1.5/gwcelery/tests/data/superevents.json
+-rw-r--r--   0        0        0     7713 2023-08-01 20:37:01.779901 gwcelery-2.1.5/gwcelery/tests/data/swift_grb_gcn.xml
+-rw-r--r--   0        0        0     1962 2023-08-01 20:37:01.779901 gwcelery-2.1.5/gwcelery/tests/data/swift_subgrbtargeted_template.xml
+-rw-r--r--   0        0        0   581918 2023-08-01 20:37:01.787901 gwcelery-2.1.5/gwcelery/tests/data/test_classifier.pickle
+-rw-r--r--   0        0        0     4042 2023-08-01 20:37:01.788901 gwcelery-2.1.5/gwcelery/tests/process.py
+-rw-r--r--   0        0        0     2307 2023-08-01 20:37:01.788901 gwcelery-2.1.5/gwcelery/tests/test_sentry.py
+-rw-r--r--   0        0        0     1705 2023-08-01 20:37:01.788901 gwcelery-2.1.5/gwcelery/tests/test_tasks_alerts.py
+-rw-r--r--   0        0        0     4916 2023-08-01 20:37:01.789901 gwcelery-2.1.5/gwcelery/tests/test_tasks_alerts_validate.py
+-rw-r--r--   0        0        0     1439 2023-08-01 20:37:01.789901 gwcelery-2.1.5/gwcelery/tests/test_tasks_bayestar.py
+-rw-r--r--   0        0        0     3007 2023-08-01 20:37:01.789901 gwcelery-2.1.5/gwcelery/tests/test_tasks_circulars.py
+-rw-r--r--   0        0        0     4550 2023-08-01 20:37:01.790901 gwcelery-2.1.5/gwcelery/tests/test_tasks_condor.py
+-rw-r--r--   0        0        0    16937 2023-08-01 20:37:01.791901 gwcelery-2.1.5/gwcelery/tests/test_tasks_detchar.py
+-rw-r--r--   0        0        0     2317 2023-08-01 20:37:01.791901 gwcelery-2.1.5/gwcelery/tests/test_tasks_em_bright.py
+-rw-r--r--   0        0        0    13802 2023-08-01 20:37:01.792901 gwcelery-2.1.5/gwcelery/tests/test_tasks_external_skymaps.py
+-rw-r--r--   0        0        0    40706 2023-08-01 20:37:01.793901 gwcelery-2.1.5/gwcelery/tests/test_tasks_external_triggers.py
+-rw-r--r--   0        0        0     1816 2023-08-01 20:37:01.793901 gwcelery-2.1.5/gwcelery/tests/test_tasks_first2years.py
+-rw-r--r--   0        0        0     4584 2023-08-01 20:37:01.793901 gwcelery-2.1.5/gwcelery/tests/test_tasks_first2years_external.py
+-rw-r--r--   0        0        0     1826 2023-08-01 20:37:01.794901 gwcelery-2.1.5/gwcelery/tests/test_tasks_gcn.py
+-rw-r--r--   0        0        0     1655 2023-08-01 20:37:01.794901 gwcelery-2.1.5/gwcelery/tests/test_tasks_gcn_validate.py
+-rw-r--r--   0        0        0     5739 2023-08-01 20:37:01.794901 gwcelery-2.1.5/gwcelery/tests/test_tasks_gracedb.py
+-rw-r--r--   0        0        0     9591 2023-08-01 20:37:01.795901 gwcelery-2.1.5/gwcelery/tests/test_tasks_gwskynet.py
+-rw-r--r--   0        0        0     3662 2023-08-01 20:37:01.795901 gwcelery-2.1.5/gwcelery/tests/test_tasks_igwn_alert.py
+-rw-r--r--   0        0        0    26722 2023-08-01 20:37:01.796901 gwcelery-2.1.5/gwcelery/tests/test_tasks_inference.py
+-rw-r--r--   0        0        0    36838 2023-08-01 20:37:01.796901 gwcelery-2.1.5/gwcelery/tests/test_tasks_orchestrator.py
+-rw-r--r--   0        0        0     1647 2023-08-01 20:37:01.797901 gwcelery-2.1.5/gwcelery/tests/test_tasks_p_astro.py
+-rw-r--r--   0        0        0    26081 2023-08-01 20:37:01.797901 gwcelery-2.1.5/gwcelery/tests/test_tasks_raven.py
+-rw-r--r--   0        0        0     4734 2023-08-01 20:37:01.798901 gwcelery-2.1.5/gwcelery/tests/test_tasks_rrt_utils.py
+-rw-r--r--   0        0        0     5035 2023-08-01 20:37:01.798901 gwcelery-2.1.5/gwcelery/tests/test_tasks_skymaps.py
+-rw-r--r--   0        0        0    40274 2023-08-01 20:37:01.799901 gwcelery-2.1.5/gwcelery/tests/test_tasks_superevents.py
+-rw-r--r--   0        0        0      637 2023-08-01 20:37:01.799901 gwcelery-2.1.5/gwcelery/tests/test_tempfile.py
+-rw-r--r--   0        0        0     3520 2023-08-01 20:37:01.799901 gwcelery-2.1.5/gwcelery/tests/test_tools_condor.py
+-rw-r--r--   0        0        0     1098 2023-08-01 20:37:01.800901 gwcelery-2.1.5/gwcelery/tests/test_tools_condor_submit_helper.py
+-rw-r--r--   0        0        0      633 2023-08-01 20:37:01.800901 gwcelery-2.1.5/gwcelery/tests/test_tools_flask.py
+-rw-r--r--   0        0        0    10579 2023-08-01 20:37:01.800901 gwcelery-2.1.5/gwcelery/tests/test_tools_nagios.py
+-rw-r--r--   0        0        0      269 2023-08-01 20:37:01.800901 gwcelery-2.1.5/gwcelery/tests/test_util.py
+-rw-r--r--   0        0        0    22656 2023-08-01 20:37:01.801901 gwcelery-2.1.5/gwcelery/tests/test_views.py
+-rw-r--r--   0        0        0      216 2023-08-01 20:37:01.801901 gwcelery-2.1.5/gwcelery/tools/__init__.py
+-rw-r--r--   0        0        0     2948 2023-08-01 20:37:01.802901 gwcelery-2.1.5/gwcelery/tools/condor.py
+-rw-r--r--   0        0        0     1120 2023-08-01 20:37:01.802901 gwcelery-2.1.5/gwcelery/tools/condor_submit_helper.py
+-rw-r--r--   0        0        0     1938 2023-08-01 20:37:01.802901 gwcelery-2.1.5/gwcelery/tools/flask.py
+-rw-r--r--   0        0        0     7899 2023-08-01 20:37:01.803901 gwcelery-2.1.5/gwcelery/tools/nagios.py
+-rw-r--r--   0        0        0      413 2023-08-01 20:37:01.803901 gwcelery-2.1.5/gwcelery/util/__init__.py
+-rw-r--r--   0        0        0     1007 2023-08-01 20:37:01.803901 gwcelery-2.1.5/gwcelery/util/cmdline.py
+-rw-r--r--   0        0        0      453 2023-08-01 20:37:01.803901 gwcelery-2.1.5/gwcelery/util/matplotlib.py
+-rw-r--r--   0        0        0      390 2023-08-01 20:37:01.804901 gwcelery-2.1.5/gwcelery/util/proxy.py
+-rw-r--r--   0        0        0      514 2023-08-01 20:37:01.804901 gwcelery-2.1.5/gwcelery/util/resources.py
+-rw-r--r--   0        0        0      253 2023-08-01 20:37:01.804901 gwcelery-2.1.5/gwcelery/util/sphinx.py
+-rw-r--r--   0        0        0      941 2023-08-01 20:37:01.804901 gwcelery-2.1.5/gwcelery/util/tempfile.py
+-rw-r--r--   0        0        0    19524 2023-08-01 20:37:01.805901 gwcelery-2.1.5/gwcelery/views.py
+-rw-r--r--   0        0        0      365 2023-08-01 20:37:01.805901 gwcelery-2.1.5/gwcelery/voevent/__init__.py
+-rw-r--r--   0        0        0     6387 2023-08-01 20:37:01.805901 gwcelery-2.1.5/gwcelery/voevent/bootsteps.py
+-rw-r--r--   0        0        0     1063 2023-08-01 20:37:01.806901 gwcelery-2.1.5/gwcelery/voevent/logging.py
+-rw-r--r--   0        0        0      779 2023-08-01 20:37:01.806901 gwcelery-2.1.5/gwcelery/voevent/signals.py
+-rw-r--r--   0        0        0      852 2023-08-01 20:37:01.806901 gwcelery-2.1.5/gwcelery/voevent/subscriber.py
+-rw-r--r--   0        0        0     1454 2023-08-01 20:37:01.806901 gwcelery-2.1.5/gwcelery/voevent/util.py
+-rw-r--r--   0        0        0     6099 2023-08-01 20:37:33.533915 gwcelery-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4530 1970-01-01 00:00:00.000000 gwcelery-2.1.5/PKG-INFO
```

### Comparing `gwcelery-2.1.4/CHANGES.rst` & `gwcelery-2.1.5/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 Changelog
 =========
 
+2.1.5 "Ningen" (08-01-2023)
+---------------------------
+
+-   Add "online" label to PESummary result page from online Bilby.
+
+-   Increase tolerance duration for superevent existence nagios check in
+    the last hour from 1 min to 10 mins.
+
+-   Add error handling to hop-client consumers, and restart the consumer
+    on non-fatal errors.
+
+-   Ensure that the content of ``coincidence_far.json`` is in JSON format
+    in ``views.py``.
+
 2.1.4 "Mokele-Mbembe" (07-26-2023)
 ----------------------------------
 
 -   Use upload instead of create_log and update t_0 in update_if_dqok.
 
 -   Add nagios check for presence of recent MDC superevents.
```

### Comparing `gwcelery-2.1.4/LICENSE.rst` & `gwcelery-2.1.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/README.rst` & `gwcelery-2.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/Makefile` & `gwcelery-2.1.5/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/_static/acceptance-tests-checklist.png` & `gwcelery-2.1.5/doc/_static/acceptance-tests-checklist.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/_static/celeryevent-screenshot.png` & `gwcelery-2.1.5/doc/_static/celeryevent-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/_static/deployment-screenshot.png` & `gwcelery-2.1.5/doc/_static/deployment-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/_static/flask-screenshot.png` & `gwcelery-2.1.5/doc/_static/flask-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/_static/flower-screenshot.png` & `gwcelery-2.1.5/doc/_static/flower-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/_static/logo-0.5x.png` & `gwcelery-2.1.5/doc/_static/logo-0.5x.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/_static/logo.png` & `gwcelery-2.1.5/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/_static/sentry-screenshot.png` & `gwcelery-2.1.5/doc/_static/sentry-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/conf.py` & `gwcelery-2.1.5/doc/conf.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/configuration.rst` & `gwcelery-2.1.5/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/contributing.rst` & `gwcelery-2.1.5/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/deployment.rst` & `gwcelery-2.1.5/doc/deployment.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/design.rst` & `gwcelery-2.1.5/doc/design.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/gwcelery.tasks.detchar.rst` & `gwcelery-2.1.5/doc/gwcelery.tasks.detchar.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/gwcelery.tasks.em_bright.rst` & `gwcelery-2.1.5/doc/gwcelery.tasks.em_bright.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/gwcelery.tasks.external_triggers.rst` & `gwcelery-2.1.5/doc/gwcelery.tasks.external_triggers.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/gwcelery.tasks.orchestrator.rst` & `gwcelery-2.1.5/doc/gwcelery.tasks.orchestrator.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/gwcelery.tasks.rst` & `gwcelery-2.1.5/doc/gwcelery.tasks.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/gwcelery.tasks.superevents.rst` & `gwcelery-2.1.5/doc/gwcelery.tasks.superevents.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/htcondor.rst` & `gwcelery-2.1.5/doc/htcondor.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/index.rst` & `gwcelery-2.1.5/doc/index.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/make.bat` & `gwcelery-2.1.5/doc/make.bat`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/monitoring.rst` & `gwcelery-2.1.5/doc/monitoring.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/doc/quickstart.rst` & `gwcelery-2.1.5/doc/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/__init__.py` & `gwcelery-2.1.5/gwcelery/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/_version.py` & `gwcelery-2.1.5/gwcelery/_version.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/conf/__init__.py` & `gwcelery-2.1.5/gwcelery/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/conf/dev.py` & `gwcelery-2.1.5/gwcelery/conf/dev.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/conf/minikube.py` & `gwcelery-2.1.5/gwcelery/conf/minikube.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/conf/playground.py` & `gwcelery-2.1.5/gwcelery/conf/playground.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/conf/production.py` & `gwcelery-2.1.5/gwcelery/conf/production.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/conf/test.py` & `gwcelery-2.1.5/gwcelery/conf/test.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/data/first2years/gstlal.xml.gz` & `gwcelery-2.1.5/gwcelery/data/first2years/gstlal.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/data/gwcelery.sub` & `gwcelery-2.1.5/gwcelery/data/gwcelery.sub`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/email/bootsteps.py` & `gwcelery-2.1.5/gwcelery/email/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/email/signals.py` & `gwcelery-2.1.5/gwcelery/email/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/flask.py` & `gwcelery-2.1.5/gwcelery/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/igwn_alert/__init__.py` & `gwcelery-2.1.5/gwcelery/igwn_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/igwn_alert/bootsteps.py` & `gwcelery-2.1.5/gwcelery/igwn_alert/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/igwn_alert/signals.py` & `gwcelery-2.1.5/gwcelery/igwn_alert/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/kafka/bootsteps.py` & `gwcelery-2.1.5/gwcelery/kafka/bootsteps.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,32 +111,54 @@
 
 
 class KafkaListener(KafkaBase):
 
     def __init__(self, name, config):
         super().__init__(name, config, 'consumer')
         self._open_hop_stream = None
+        self.running = False
         # Don't kill worker if listener can't connect
         try:
             self._open_hop_stream = self._hop_stream.open(config['url'], 'r')
         except KafkaException:
             log.exception('Connection to %s failed', self._config["url"])
         except ValueError:
             # Hop client will return a ValueError if the topic doesn't exist on
             # the broker
             log.exception('Connection to %s failed', self._config["url"])
 
     def listen(self):
-        for message in self._open_hop_stream:
-            # Send signal
-            kafka_record_consumed.send(
-                None,
-                name=self.name,
-                record=self.get_payload_output(message)
-            )
+        self.running = True
+        # Restart the consumer when non-fatal errors come up, similar to
+        # gwcelery.igwn_alert.IGWNAlertClient
+        while self.running:
+            try:
+                for message in self._open_hop_stream:
+                    # Send signal
+                    kafka_record_consumed.send(
+                        None,
+                        name=self.name,
+                        record=self.get_payload_output(message)
+                    )
+            except KafkaException as exception:
+                err = exception.args[0]
+                if self.running is False:
+                    # The close attempt in the KafkaListener stop method throws
+                    # a KafkaException that's caught by this try except, so we
+                    # just have to catch this case for the worker to shut down
+                    # gracefully
+                    pass
+                elif err.fatal():
+                    # stop running and close before raising error
+                    self.running = False
+                    self._open_hop_stream.close()
+                    raise
+                else:
+                    log.warning(
+                        "non-fatal error from kafka: {}".format(err.name))
 
 
 class KafkaWriter(KafkaBase):
     """Write Kafka topics and monitor health."""
 
     def __init__(self, name, config):
         super().__init__(name, config, 'producer')
@@ -228,14 +250,15 @@
 
     def stop(self, consumer):
         log.info('Closing connection to topics: ' +
                  ' '.join(listener._config['url'] for listener in
                           self._listeners.values() if listener._open_hop_stream
                           is not None))
         for s in self._listeners.values():
+            s.running = False
             if s._open_hop_stream is not None:
                 s._open_hop_stream.close()
 
         for thread in self.threads:
             thread.join()
 
     def info(self, consumer):
```

### Comparing `gwcelery-2.1.4/gwcelery/kafka/signals.py` & `gwcelery-2.1.5/gwcelery/kafka/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/sentry/__init__.py` & `gwcelery-2.1.5/gwcelery/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/sentry/integrations/condor.py` & `gwcelery-2.1.5/gwcelery/sentry/integrations/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/sentry/integrations/requests.py` & `gwcelery-2.1.5/gwcelery/sentry/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/sentry/integrations/subprocess.py` & `gwcelery-2.1.5/gwcelery/sentry/integrations/subprocess.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/static/typeahead.css` & `gwcelery-2.1.5/gwcelery/static/typeahead.css`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/static/vega/index.html` & `gwcelery-2.1.5/gwcelery/static/vega/index.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/__init__.py` & `gwcelery-2.1.5/gwcelery/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/alerts.py` & `gwcelery-2.1.5/gwcelery/tasks/alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/bayestar.py` & `gwcelery-2.1.5/gwcelery/tasks/bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/circulars.py` & `gwcelery-2.1.5/gwcelery/tasks/circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/condor.py` & `gwcelery-2.1.5/gwcelery/tasks/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/core.py` & `gwcelery-2.1.5/gwcelery/tasks/core.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/detchar.py` & `gwcelery-2.1.5/gwcelery/tasks/detchar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/em_bright.py` & `gwcelery-2.1.5/gwcelery/tasks/em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/external_skymaps.py` & `gwcelery-2.1.5/gwcelery/tasks/external_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/external_triggers.py` & `gwcelery-2.1.5/gwcelery/tasks/external_triggers.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/first2years.py` & `gwcelery-2.1.5/gwcelery/tasks/first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/first2years_external.py` & `gwcelery-2.1.5/gwcelery/tasks/first2years_external.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/gcn.py` & `gwcelery-2.1.5/gwcelery/tasks/gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/gracedb.py` & `gwcelery-2.1.5/gwcelery/tasks/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/gwskynet.py` & `gwcelery-2.1.5/gwcelery/tasks/gwskynet.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/igwn_alert.py` & `gwcelery-2.1.5/gwcelery/tasks/igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/inference.py` & `gwcelery-2.1.5/gwcelery/tasks/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -712,14 +712,15 @@
     )
     pesummary_kwargs["calibration"] = convert_string_to_dict(
         config_content["spline-calibration-envelope-dict"]
     )
     pesummary_kwargs["approximant"] = config_content["waveform-approximant"]
     pesummary_kwargs["f_low"] = config_content["minimum-frequency"]
     pesummary_kwargs["f_ref"] = config_content["reference-frequency"]
+    pesummary_kwargs["label"] = "online"
 
     webdir = os.path.join(config_content["webdir"], 'pesummary')
     url = urllib.parse.urljoin(
         app.conf['pe_results_url'],
         os.path.relpath(
             os.path.join(webdir, 'home.html'),
             app.conf['pe_results_path']
```

### Comparing `gwcelery-2.1.4/gwcelery/tasks/legacy_gracedb.py` & `gwcelery-2.1.5/gwcelery/tasks/legacy_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/notice_text.py` & `gwcelery-2.1.5/gwcelery/tasks/notice_text.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/orchestrator.py` & `gwcelery-2.1.5/gwcelery/tasks/orchestrator.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/p_astro.py` & `gwcelery-2.1.5/gwcelery/tasks/p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/raven.py` & `gwcelery-2.1.5/gwcelery/tasks/raven.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/rrt_utils.py` & `gwcelery-2.1.5/gwcelery/tasks/rrt_utils.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/skymaps.py` & `gwcelery-2.1.5/gwcelery/tasks/skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tasks/superevents.py` & `gwcelery-2.1.5/gwcelery/tasks/superevents.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/templates/fits_header.jinja2` & `gwcelery-2.1.5/gwcelery/templates/fits_header.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/templates/index.jinja2` & `gwcelery-2.1.5/gwcelery/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/templates/lalinference.jinja2` & `gwcelery-2.1.5/gwcelery/templates/lalinference.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/templates/rapidpe.jinja2` & `gwcelery-2.1.5/gwcelery/templates/rapidpe.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/conftest.py` & `gwcelery-2.1.5/gwcelery/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/G000012_S0040_preferred.json` & `gwcelery-2.1.5/gwcelery/tests/data/G000012_S0040_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/G298048-1-Initial.xml` & `gwcelery-2.1.5/gwcelery/tests/data/G298048-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/G298048_log.json` & `gwcelery-2.1.5/gwcelery/tests/data/G298048_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json` & `gwcelery-2.1.5/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/MS220722v.xml` & `gwcelery-2.1.5/gwcelery/tests/data/MS220722v.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits` & `gwcelery-2.1.5/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/S230413b.json` & `gwcelery-2.1.5/gwcelery/tests/data/S230413b.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/S230413g.json` & `gwcelery-2.1.5/gwcelery/tests/data/S230413g.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/S230413h.json` & `gwcelery-2.1.5/gwcelery/tests/data/S230413h.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/T0212_S0039_preferred.json` & `gwcelery-2.1.5/gwcelery/tests/data/T0212_S0039_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json` & `gwcelery-2.1.5/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/T0219_S0041_nopreferred.json` & `gwcelery-2.1.5/gwcelery/tests/data/T0219_S0041_nopreferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/agile_grb_gcn.xml` & `gwcelery-2.1.5/gwcelery/tests/data/agile_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/coinc.xml` & `gwcelery-2.1.5/gwcelery/tests/data/coinc.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/externaltrigger_original_data.xml` & `gwcelery-2.1.5/gwcelery/tests/data/externaltrigger_original_data.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/fermi_grb_gcn.xml` & `gwcelery-2.1.5/gwcelery/tests/data/fermi_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/fermi_initial_grb_gcn.xml` & `gwcelery-2.1.5/gwcelery/tests/data/fermi_initial_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/fermi_noise_gcn.xml` & `gwcelery-2.1.5/gwcelery/tests/data/fermi_noise_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/fermi_noise_gcn_2.xml` & `gwcelery-2.1.5/gwcelery/tests/data/fermi_noise_gcn_2.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/fermi_subgrbtargeted_template.xml` & `gwcelery-2.1.5/gwcelery/tests/data/fermi_subgrbtargeted_template.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml` & `gwcelery-2.1.5/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml` & `gwcelery-2.1.5/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/fits_header_result.html` & `gwcelery-2.1.5/gwcelery/tests/data/fits_header_result.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/gracedb_externaltrigger_log.json` & `gwcelery-2.1.5/gwcelery/tests/data/gracedb_externaltrigger_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_detchar.json` & `gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_detchar.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_exttrig_creation.json` & `gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_exttrig_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json` & `gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_psd.json` & `gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_psd.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_snews_creation.json` & `gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_snews_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_snews_test_creation.json` & `gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_snews_test_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_subgrb_creation.json` & `gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_subgrb_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_superevent_creation.json` & `gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_superevent_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/igwn_alert_voevent.json` & `gwcelery-2.1.5/gwcelery/tests/data/igwn_alert_voevent.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/integral_grb_gcn.xml` & `gwcelery-2.1.5/gwcelery/tests/data/integral_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/integral_mdc_gcn.xml` & `gwcelery-2.1.5/gwcelery/tests/data/integral_mdc_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/kafka_alert_fermi.json` & `gwcelery-2.1.5/gwcelery/tests/data/kafka_alert_fermi.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/kafka_alert_fermi_ignore.json` & `gwcelery-2.1.5/gwcelery/tests/data/kafka_alert_fermi_ignore.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/kafka_alert_swift.json` & `gwcelery-2.1.5/gwcelery/tests/data/kafka_alert_swift.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/kafka_alert_swift_noloc.json` & `gwcelery-2.1.5/gwcelery/tests/data/kafka_alert_swift_noloc.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/kafka_alert_swift_wskymap.json` & `gwcelery-2.1.5/gwcelery/tests/data/kafka_alert_swift_wskymap.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.1.5/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.1.5/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/llhoft/omegascan/scanme.gwf` & `gwcelery-2.1.5/gwcelery/tests/data/llhoft/omegascan/scanme.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.1.5/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/lvalert_event_creation.json` & `gwcelery-2.1.5/gwcelery/tests/data/lvalert_event_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/lvalert_xmpp.xml` & `gwcelery-2.1.5/gwcelery/tests/data/lvalert_xmpp.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/mock_superevent_object.json` & `gwcelery-2.1.5/gwcelery/tests/data/mock_superevent_object.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite` & `gwcelery-2.1.5/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/psd.xml.gz` & `gwcelery-2.1.5/gwcelery/tests/data/psd.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/rrt_small_area.fits` & `gwcelery-2.1.5/gwcelery/tests/data/rrt_small_area.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/sample_events.json` & `gwcelery-2.1.5/gwcelery/tests/data/sample_events.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/samples.hdf5` & `gwcelery-2.1.5/gwcelery/tests/data/samples.hdf5`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/scaler_set_all.pickle` & `gwcelery-2.1.5/gwcelery/tests/data/scaler_set_all.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/snews_gcn.xml` & `gwcelery-2.1.5/gwcelery/tests/data/snews_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/snews_gcn_test.xml` & `gwcelery-2.1.5/gwcelery/tests/data/snews_gcn_test.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/superevents.json` & `gwcelery-2.1.5/gwcelery/tests/data/superevents.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/swift_grb_gcn.xml` & `gwcelery-2.1.5/gwcelery/tests/data/swift_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/swift_subgrbtargeted_template.xml` & `gwcelery-2.1.5/gwcelery/tests/data/swift_subgrbtargeted_template.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/data/test_classifier.pickle` & `gwcelery-2.1.5/gwcelery/tests/data/test_classifier.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/process.py` & `gwcelery-2.1.5/gwcelery/tests/process.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_sentry.py` & `gwcelery-2.1.5/gwcelery/tests/test_sentry.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_alerts.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_alerts_validate.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_alerts_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_bayestar.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_circulars.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_condor.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_detchar.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_detchar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_em_bright.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_external_skymaps.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_external_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_external_triggers.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_external_triggers.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_first2years.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_first2years_external.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_first2years_external.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_gcn.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_gcn_validate.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_gcn_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_gracedb.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_gwskynet.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_gwskynet.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_igwn_alert.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_inference.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,15 +493,15 @@
                 ans = [
                     "summarypages", "--webdir", "webdir/pesummary",
                     "--samples", os.path.join(sampledir, 'test_result.hdf5'),
                     "--gw", "--no_ligo_skymap", "--multi_process", "6",
                     "--config", path_to_bilby_config, "--psd", "H1:H1_psd.txt",
                     "L1:L1_psd.txt", "--calibration", "H1:H1_cal.txt",
                     "L1:L1_cal.txt", "--approximant", "IMRPhenomPv2",
-                    "--f_low", "20", "--f_ref", "100"
+                    "--f_low", "20", "--f_ref", "100", "--label", "online"
                 ]
                 if host != 'gracedb.ligo.org':
                     ans += ["--disable_interactive", "--disable_expert"]
                 else:
                     ans += [
                         "--redshift_method", "exact", "--evolve_spins_forwards"
                     ]
```

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_orchestrator.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_orchestrator.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_p_astro.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_raven.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_raven.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_rrt_utils.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_rrt_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,51 +61,51 @@
             'gpstime': 1234,
         }
     return event
 
 
 @pytest.mark.parametrize(
         'superevent,embright,pastro,skymap,result',
-        [[{'labels': [], 'gw_events':['G123', 'G456']},
+        [[{'labels': [], 'gw_events': ['G123', 'G456']},
           {'HasNS': 0.0, 'HasRemnant': 0.0, 'HasMassGap': 0.0},
           {"BNS": 0.0, "NSBH": 0.0, "BBH": 0.7, "Terrestrial": 0.3},
           skymap_large, True],
-         [{'labels': [], 'gw_events':['G123']},
+         [{'labels': [], 'gw_events': ['G123']},
           {'HasNS': 0.8, 'HasRemnant': 0.2, 'HasMassGap': 0.0},
           {"BNS": 0.0, "NSBH": 0.0, "BBH": 0.7, "Terrestrial": 0.3},
           skymap_large, True],
-         [{'labels': [], 'gw_events':['G123']},
+         [{'labels': [], 'gw_events': ['G123']},
           {'HasNS': 0.9, 'HasRemnant': 0.0, 'HasMassGap': 0.0},
           {"BNS": 0.8, "NSBH": 0.2, "BBH": 0.0, "Terrestrial": 0.0},
           skymap_large, True],
-         [{'labels': [], 'gw_events':['G123']},
+         [{'labels': [], 'gw_events': ['G123']},
           {'HasNS': 0.9, 'HasRemnant': 0.2, 'HasMassGap': 0.0},
           {"BNS": 0.0, "NSBH": 0.9, "BBH": 0.0, "Terrestrial": 0.1},
           skymap_large, True],
-         [{'labels': [], 'gw_events':['G123']},
+         [{'labels': [], 'gw_events': ['G123']},
           {'HasNS': 0.0, 'HasRemnant': 0.0, 'HasMassGap': 0.0},
           {"BNS": 0.0, "NSBH": 0.0, "BBH": 0.9, "Terrestrial": 0.1},
           skymap_small, True],
-         [{'labels': [], 'gw_events':['G123']},
+         [{'labels': [], 'gw_events': ['G123']},
           {'HasNS': 0.0, 'HasRemnant': 0.0, 'HasMassGap': 0.0},
           {"BNS": 0.0, "NSBH": 0.0, "BBH": 1.0, "Terrestrial": 0.0},
           skymap_large, False],
-         [{'labels': [], 'gw_events':['G123', 'G789']},
+         [{'labels': [], 'gw_events': ['G123', 'G789']},
           {'HasNS': 0.0, 'HasRemnant': 0.0, 'HasMassGap': 0.0},
           {"BNS": 0.0, "NSBH": 0.0, "BBH": 1.0, "Terrestrial": 0.0},
           skymap_large, False],
-         [{'labels': [], 'gw_events':['G123']},
+         [{'labels': [], 'gw_events': ['G123']},
           {'HasNS': 1.0, 'HasRemnant': 1.0, 'HasMassGap': 0.0},
           {"BNS": 0.2, "NSBH": 0.2, "BBH": 0.0, "Terrestrial": 0.6},
           skymap_large, False],
-         [{'labels': [], 'gw_events':['G123', 'G246']},
+         [{'labels': [], 'gw_events': ['G123', 'G246']},
           {'HasNS': 0.0, 'HasRemnant': 0.0, 'HasMassGap': 0.0},
           {"BNS": 0.0, "NSBH": 0.0, "BBH": 0.7, "Terrestrial": 0.3},
           skymap_large, False],
-         [{'labels': ['HIGH_PROFILE'], 'gw_events':['G123', 'G246']},
+         [{'labels': ['HIGH_PROFILE'], 'gw_events': ['G123', 'G246']},
           {'HasNS': 1.0, 'HasRemnant': 1.0, 'HasMassGap': 0.0},
           {"BNS": 1.0, "NSBH": 0.0, "BBH": 0.0, "Terrestrial": 0.0},
           skymap_small, False]
          ])
 def test_high_profile(monkeypatch, superevent, embright,
                       pastro, skymap, result):
     embright = json.dumps(embright)
```

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_skymaps.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tasks_superevents.py` & `gwcelery-2.1.5/gwcelery/tests/test_tasks_superevents.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tempfile.py` & `gwcelery-2.1.5/gwcelery/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tools_condor.py` & `gwcelery-2.1.5/gwcelery/tests/test_tools_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tools_condor_submit_helper.py` & `gwcelery-2.1.5/gwcelery/tests/test_tools_condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tools_flask.py` & `gwcelery-2.1.5/gwcelery/tests/test_tools_flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_tools_nagios.py` & `gwcelery-2.1.5/gwcelery/tests/test_tools_nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tests/test_views.py` & `gwcelery-2.1.5/gwcelery/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tools/condor.py` & `gwcelery-2.1.5/gwcelery/tools/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tools/condor_submit_helper.py` & `gwcelery-2.1.5/gwcelery/tools/condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tools/flask.py` & `gwcelery-2.1.5/gwcelery/tools/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/tools/nagios.py` & `gwcelery-2.1.5/gwcelery/tools/nagios.py`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         raise NagiosCriticalError(
                 'No MDC superevents found in past six hours') \
             from AssertionError(
                 f'Last entry earlier than GPSTime {t_lower} = '
                 f'{to_utc(t_lower)} UTC')
     last_superevent = recent_mdc_superevents[0]
     # check presence in last hour with a tolerance
-    none_in_last_hour = (t_now - last_superevent['t_0']) > (3600 + 60)
+    none_in_last_hour = (t_now - last_superevent['t_0']) > (3600 + 600)
     if none_in_last_hour:
         raise NagiosCriticalError(
                 'No MDC superevents found in last one hour') \
             from AssertionError(
                 f"Last entry is at GPSTime {last_superevent['superevent_id']}"
                 f" = {to_utc(last_superevent['t_0'])} UTC")
```

### Comparing `gwcelery-2.1.4/gwcelery/util/cmdline.py` & `gwcelery-2.1.5/gwcelery/util/cmdline.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/util/resources.py` & `gwcelery-2.1.5/gwcelery/util/resources.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/util/tempfile.py` & `gwcelery-2.1.5/gwcelery/util/tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/views.py` & `gwcelery-2.1.5/gwcelery/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Flask web application views."""
 import datetime
 from importlib import metadata
+import json
 import platform
 import re
 import socket
 import sys
 
 from astropy.time import Time
 from celery import group
@@ -442,14 +443,16 @@
 def _update_preferred_external_event(ext_event, superevent_id):
     """Update preferred external event to given external event."""
     # FIXME: Consider consolidating with raven.update_coinc_far by using
     # a single function in superevents.py
     if ext_event['search'] in {'GRB', 'SubGRB', 'SubGRBTargeted'}:
         coinc_far_dict = gracedb.download(
             'coincidence_far.json', ext_event['graceid'])
+        if not isinstance(coinc_far_dict, dict):
+            coinc_far_dict = json.loads(coinc_far_dict)
         time_coinc_far = coinc_far_dict['temporal_coinc_far']
         space_coinc_far = coinc_far_dict['spatiotemporal_coinc_far']
     else:
         time_coinc_far = None
         space_coinc_far = None
     gracedb.update_superevent(superevent_id, em_type=ext_event['graceid'],
                               time_coinc_far=time_coinc_far,
```

### Comparing `gwcelery-2.1.4/gwcelery/voevent/bootsteps.py` & `gwcelery-2.1.5/gwcelery/voevent/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/voevent/logging.py` & `gwcelery-2.1.5/gwcelery/voevent/logging.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/voevent/signals.py` & `gwcelery-2.1.5/gwcelery/voevent/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/voevent/subscriber.py` & `gwcelery-2.1.5/gwcelery/voevent/subscriber.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/gwcelery/voevent/util.py` & `gwcelery-2.1.5/gwcelery/voevent/util.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.4/pyproject.toml` & `gwcelery-2.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwcelery"
-version = "2.1.4"
+version = "2.1.5"
 description = "Low-latency pipeline for annotating IGWN events"
 readme = "README.rst"
 authors = [
     "Deep Chatterjee <deep.chatterjee@ligo.org>",
     "Cody Messick <cody.messick@ligo.org>",
     "Geoffrey Mo <geoffrey.mo@ligo.org>",
     "Leo Singer <leo.singer@ligo.org>"
```

### Comparing `gwcelery-2.1.4/PKG-INFO` & `gwcelery-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwcelery
-Version: 2.1.4
+Version: 2.1.5
 Summary: Low-latency pipeline for annotating IGWN events
 Home-page: https://git.ligo.org/emfollow/gwcelery
 License: GPL-2.0+
 Author: Deep Chatterjee
 Author-email: deep.chatterjee@ligo.org
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
```

