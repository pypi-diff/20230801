# Comparing `tmp/nessai-0.9.0.tar.gz` & `tmp/nessai-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nessai-0.9.0.tar", last modified: Sun Jul  2 09:21:34 2023, max compression
+gzip compressed data, was "nessai-0.9.1.tar", last modified: Tue Aug  1 11:55:06 2023, max compression
```

## Comparing `nessai-0.9.0.tar` & `nessai-0.9.1.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.174573 nessai-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.090571 nessai-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.102571 nessai-0.9.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.102571 nessai-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/workflows/compatibility-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/workflows/integration-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-02 09:21:24.000000 nessai-0.9.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-02 09:21:24.000000 nessai-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-02 09:21:24.000000 nessai-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-02 09:21:24.000000 nessai-0.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    39295 2023-07-02 09:21:24.000000 nessai-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-02 09:21:24.000000 nessai-0.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-02 09:21:24.000000 nessai-0.9.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-02 09:21:34.174573 nessai-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-02 09:21:24.000000 nessai-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-02 09:21:24.000000 nessai-0.9.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-02 09:21:24.000000 nessai-0.9.0/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.106571 nessai-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.110571 nessai-0.9.0/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    40373 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/assets/insertion_indices.png
--rw-r--r--   0 runner    (1001) docker     (123)    25386 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/assets/logXlogL.png
--rw-r--r--   0 runner    (1001) docker     (123)    70482 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/assets/posterior_distribution.png
--rw-r--r--   0 runner    (1001) docker     (123)   159636 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/assets/state.png
--rw-r--r--   0 runner    (1001) docker     (123)    20221 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/assets/trace.png
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/bilby-example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/further-details.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/gaussian-example.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/gravitational-wave-inference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/importance-nested-sampling.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/normalising-flows-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/parallelisation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/reparameterisations.rst
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/running-the-sampler.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-02 09:21:24.000000 nessai-0.9.0/docs/sampler-configuration.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.114571 nessai-0.9.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/2d_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/augmented_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/bilby_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/bilby_unbounded_priors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/corner_plot_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/eggbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.114571 nessai-0.9.0/examples/gw/
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/gw/basic_gw_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/gw/calibration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/gw/full_gw_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/half_gaussian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.114571 nessai-0.9.0/examples/importance_nested_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/importance_nested_sampler/basic_ins_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/importance_nested_sampler/nsf_unit_hypercube.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/parallelisation_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/reparameterisations_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-02 09:21:24.000000 nessai-0.9.0/examples/unbounded_prior.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.118572 nessai-0.9.0/nessai/
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/evidence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.122572 nessai-0.9.0/nessai/flowmodel/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flowmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flowmodel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flowmodel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flowmodel/importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flowmodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.126572 nessai-0.9.0/nessai/flows/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/maf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/nets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/nsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/realnvp.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flows/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19668 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/flowsampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.126572 nessai-0.9.0/nessai/gw/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/gw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/gw/proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/gw/reparameterisations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/gw/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/livepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/nestedsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/priors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.130572 nessai-0.9.0/nessai/proposal/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/augmented.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    58980 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/flowproposal.py
--rw-r--r--   0 runner    (1001) docker     (123)    27273 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/proposal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.130572 nessai-0.9.0/nessai/reparameterisations/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/combined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/null.py
--rw-r--r--   0 runner    (1001) docker     (123)    24042 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/reparameterisations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.134572 nessai-0.9.0/nessai/samplers/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/samplers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/samplers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    67237 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/samplers/importancesampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    47766 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/samplers/nestedsampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.138572 nessai-0.9.0/nessai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/bilbyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/hist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/indices.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/information.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/optimise.py
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/sorting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-02 09:21:24.000000 nessai-0.9.0/nessai/utils/torchutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.118572 nessai-0.9.0/nessai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-02 09:21:34.000000 nessai-0.9.0/nessai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-07-02 09:21:34.000000 nessai-0.9.0/nessai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 09:21:34.000000 nessai-0.9.0/nessai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-02 09:21:34.000000 nessai-0.9.0/nessai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-02 09:21:34.000000 nessai-0.9.0/nessai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-02 09:21:24.000000 nessai-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-02 09:21:24.000000 nessai-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-02 09:21:34.174573 nessai-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-02 09:21:24.000000 nessai-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.142572 nessai-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_bilby_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_deprecation_warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.142572 nessai-0.9.0/tests/test_evidence/
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_evidence/test_ins_evidence.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_evidence/test_standard_evidence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.142572 nessai-0.9.0/tests/test_flowmodel/
--rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flowmodel/test_flowmodel_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flowmodel/test_flowmodel_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flowmodel/test_flowmodel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.146572 nessai-0.9.0/tests/test_flows/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_base_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.146572 nessai-0.9.0/tests/test_flows/test_distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_distributions/test_multivariate_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_distributions/test_resampled.py
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_flow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_included_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flows/test_specific_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_flowsampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.146572 nessai-0.9.0/tests/test_gw/
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_gw/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_gw/test_distance_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_gw/test_gw_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_gw/test_gw_reparameterisations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_gw/test_reparameterisation_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_livepoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    38907 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    18382 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_priors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.150572 nessai-0.9.0/tests/test_proposal/
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_analytic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_augmented.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_base_proposal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.154572 nessai-0.9.0/tests/test_proposal/test_flowproposal/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_add_reparam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_init_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_population.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    24357 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_rescaling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.154572 nessai-0.9.0/tests/test_proposal/test_importance/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_prob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_rescaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_importance/test_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_proposal/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.158572 nessai-0.9.0/tests/test_reparameterisations/
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_angle_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_base_reparameterisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_combined.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_get_reparameterisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_null.py
--rw-r--r--   0 runner    (1001) docker     (123)    36520 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_rescale_to_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_scale_and_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_reparameterisations/test_to_cartesian.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.158572 nessai-0.9.0/tests/test_samplers/
--rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_base_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.162572 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.166573 nessai-0.9.0/tests/test_samplers/test_nested_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_core_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_flow_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_general_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_live_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_manage_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_ns_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_proposal_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_yield_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.166573 nessai-0.9.0/tests/test_sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_sampling/test_ins_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    17194 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_sampling/test_standard_sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 09:21:34.174573 nessai-0.9.0/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_bilbyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_distance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_distribution_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_hist_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_indices_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_information_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_optimise_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_rescaling_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_sampling_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_sorting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_stats_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_structures_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_threading_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_utils/test_torchtutils_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-02 09:21:24.000000 nessai-0.9.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.186017 nessai-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.158017 nessai-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.162017 nessai-0.9.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-08-01 11:54:56.000000 nessai-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-01 11:54:56.000000 nessai-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.162017 nessai-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-08-01 11:54:56.000000 nessai-0.9.1/.github/workflows/compatibility-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-08-01 11:54:56.000000 nessai-0.9.1/.github/workflows/integration-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-01 11:54:56.000000 nessai-0.9.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-01 11:54:56.000000 nessai-0.9.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-01 11:54:56.000000 nessai-0.9.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-01 11:54:56.000000 nessai-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-01 11:54:56.000000 nessai-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-01 11:54:56.000000 nessai-0.9.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    39569 2023-08-01 11:54:56.000000 nessai-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-08-01 11:54:56.000000 nessai-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-01 11:54:56.000000 nessai-0.9.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-08-01 11:55:06.186017 nessai-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-08-01 11:54:56.000000 nessai-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 11:54:56.000000 nessai-0.9.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-01 11:54:56.000000 nessai-0.9.1/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.162017 nessai-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.162017 nessai-0.9.1/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    40373 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/assets/insertion_indices.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25386 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/assets/logXlogL.png
+-rw-r--r--   0 runner    (1001) docker     (123)    70482 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/assets/posterior_distribution.png
+-rw-r--r--   0 runner    (1001) docker     (123)   159636 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/assets/state.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20221 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/assets/trace.png
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/bilby-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/further-details.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/gaussian-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/gravitational-wave-inference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/importance-nested-sampling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/normalising-flows-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/parallelisation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6621 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/reparameterisations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/running-the-sampler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-08-01 11:54:56.000000 nessai-0.9.1/docs/sampler-configuration.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.166017 nessai-0.9.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/2d_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/augmented_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/bilby_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/bilby_unbounded_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/corner_plot_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/eggbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.166017 nessai-0.9.1/examples/gw/
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/gw/basic_gw_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/gw/calibration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/gw/full_gw_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/half_gaussian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.166017 nessai-0.9.1/examples/importance_nested_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/importance_nested_sampler/basic_ins_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/importance_nested_sampler/nsf_unit_hypercube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/parallelisation_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/reparameterisations_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-08-01 11:54:56.000000 nessai-0.9.1/examples/unbounded_prior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.166017 nessai-0.9.1/nessai/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/evidence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.166017 nessai-0.9.1/nessai/flowmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flowmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flowmodel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flowmodel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flowmodel/importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flowmodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.170017 nessai-0.9.1/nessai/flows/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flows/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flows/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flows/maf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flows/nets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flows/nsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flows/realnvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flows/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19668 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/flowsampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.170017 nessai-0.9.1/nessai/gw/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/gw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/gw/proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/gw/reparameterisations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/gw/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12247 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/livepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22917 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/nestedsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/priors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.170017 nessai-0.9.1/nessai/proposal/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/proposal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/proposal/analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/proposal/augmented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/proposal/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59046 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/proposal/flowproposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27273 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/proposal/importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/proposal/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/proposal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.170017 nessai-0.9.1/nessai/reparameterisations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/reparameterisations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18348 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/reparameterisations/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/reparameterisations/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/reparameterisations/combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/reparameterisations/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24042 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/reparameterisations/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/reparameterisations/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.170017 nessai-0.9.1/nessai/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/samplers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67237 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/samplers/importancesampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47766 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/samplers/nestedsampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.174017 nessai-0.9.1/nessai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/bilbyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/optimise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-08-01 11:54:56.000000 nessai-0.9.1/nessai/utils/torchutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.166017 nessai-0.9.1/nessai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-08-01 11:55:06.000000 nessai-0.9.1/nessai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-08-01 11:55:06.000000 nessai-0.9.1/nessai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:55:06.000000 nessai-0.9.1/nessai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-08-01 11:55:06.000000 nessai-0.9.1/nessai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 11:55:06.000000 nessai-0.9.1/nessai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-08-01 11:54:56.000000 nessai-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-01 11:54:56.000000 nessai-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-01 11:55:06.186017 nessai-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-01 11:54:56.000000 nessai-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.174017 nessai-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_bilby_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_deprecation_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.174017 nessai-0.9.1/tests/test_evidence/
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_evidence/test_ins_evidence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_evidence/test_standard_evidence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.174017 nessai-0.9.1/tests/test_flowmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)    17582 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_flowmodel/test_flowmodel_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_flowmodel/test_flowmodel_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_flowmodel/test_flowmodel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.178017 nessai-0.9.1/tests/test_flows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_flows/test_base_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.178017 nessai-0.9.1/tests/test_flows/test_distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_flows/test_distributions/test_multivariate_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_flows/test_distributions/test_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_flows/test_flow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_flows/test_included_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_flows/test_nets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_flows/test_specific_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26252 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_flowsampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.178017 nessai-0.9.1/tests/test_gw/
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_gw/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_gw/test_distance_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_gw/test_gw_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_gw/test_gw_reparameterisations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_gw/test_reparameterisation_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_livepoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38907 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18382 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_priors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.178017 nessai-0.9.1/tests/test_proposal/
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_analytic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_augmented.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_base_proposal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.178017 nessai-0.9.1/tests/test_proposal/test_flowproposal/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_flowproposal/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_add_reparam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_init_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15832 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24357 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_rescaling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.178017 nessai-0.9.1/tests/test_proposal/test_importance/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_importance/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_importance/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_importance/test_prob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_importance/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_importance/test_rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_importance/test_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_importance/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_importance/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_proposal/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.182017 nessai-0.9.1/tests/test_reparameterisations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_reparameterisations/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_reparameterisations/test_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_reparameterisations/test_angle_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_reparameterisations/test_base_reparameterisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_reparameterisations/test_combined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_reparameterisations/test_get_reparameterisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_reparameterisations/test_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36520 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_reparameterisations/test_rescale_to_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_reparameterisations/test_scale_and_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_reparameterisations/test_to_cartesian.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.182017 nessai-0.9.1/tests/test_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_base_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.182017 nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/test_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/test_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.182017 nessai-0.9.1/tests/test_samplers/test_nested_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_nested_sampler/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_core_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_flow_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_general_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_live_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_manage_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_ns_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_proposal_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_yield_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.182017 nessai-0.9.1/tests/test_sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_sampling/test_ins_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17194 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_sampling/test_standard_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:55:06.186017 nessai-0.9.1/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_bilbyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_distance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_distribution_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_hist_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_indices_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_information_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_optimise_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_rescaling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_sampling_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_sorting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_stats_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_structures_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_threading_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_utils/test_torchtutils_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-01 11:54:56.000000 nessai-0.9.1/tests/test_version.py
```

### Comparing `nessai-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md` & `nessai-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/.github/workflows/compatibility-tests.yml` & `nessai-0.9.1/.github/workflows/compatibility-tests.yml`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/.github/workflows/integration-tests.yml` & `nessai-0.9.1/.github/workflows/integration-tests.yml`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/.github/workflows/lint.yml` & `nessai-0.9.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/.github/workflows/publish-to-pypi.yml` & `nessai-0.9.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/.github/workflows/tests.yml` & `nessai-0.9.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/.gitignore` & `nessai-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/.pre-commit-config.yaml` & `nessai-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/CHANGELOG.md` & `nessai-0.9.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.9.1]
+
+### Fixed
+
+- Fix duplicate parameters when adding reparameterisations (see [#320](https://github.com/mj-will/nessai/issues/320) for details) ([#321](https://github.com/mj-will/nessai/pull/321))
+
 ## [0.9.0]
 
 ### Added
 
 - Add importance nested sampler ([#285](https://github.com/mj-will/nessai/pull/285))
 - Add support for using regex for specifying parameters in the reparametersations dictionary ([#312](https://github.com/mj-will/nessai/pull/312))
 
@@ -513,15 +519,16 @@
 
 - Fix a bug where `maximum_uninformed` did not have the expected behaviour.
 
 ### Deprecated
 
 - Original `GWFlowProposal` method renamed to `LegacyGWFlowProposal`. Will be removed in the next release.
 
-[Unreleased]: https://github.com/mj-will/nessai/compare/v0.9.0...HEAD
+[Unreleased]: https://github.com/mj-will/nessai/compare/v0.9.1...HEAD
+[0.9.1]: https://github.com/mj-will/nessai/compare/v0.9.0...v0.9.1
 [0.9.0]: https://github.com/mj-will/nessai/compare/v0.8.1...v0.9.0
 [0.8.1]: https://github.com/mj-will/nessai/compare/v0.8.0...v0.8.1
 [0.8.0]: https://github.com/mj-will/nessai/compare/v0.7.1...v0.8.0
 [0.7.1]: https://github.com/mj-will/nessai/compare/v0.7.0...v0.7.1
 [0.7.0]: https://github.com/mj-will/nessai/compare/v0.6.0...v0.7.0
 [0.6.0]: https://github.com/mj-will/nessai/compare/v0.5.1...v0.6.0
 [0.5.1]: https://github.com/mj-will/nessai/compare/v0.5.0...v0.5.1
```

### Comparing `nessai-0.9.0/CONTRIBUTING.md` & `nessai-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/LICENSE.md` & `nessai-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/PKG-INFO` & `nessai-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nessai
-Version: 0.9.0
+Version: 0.9.1
 Summary: Nessai: Nested Sampling with Artificial Intelligence
 Home-page: https://github.com/mj-will/nessai
 Author: Michael J. Williams
 Author-email: m.williams.4@research.gla.ac.uk
 Project-URL: Documentation, https://nessai.readthedocs.io/
 Keywords: nested sampling,normalising flows,machine learning
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `nessai-0.9.0/README.md` & `nessai-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/Makefile` & `nessai-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/assets/insertion_indices.png` & `nessai-0.9.1/docs/assets/insertion_indices.png`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/assets/logXlogL.png` & `nessai-0.9.1/docs/assets/logXlogL.png`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/assets/posterior_distribution.png` & `nessai-0.9.1/docs/assets/posterior_distribution.png`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/assets/state.png` & `nessai-0.9.1/docs/assets/state.png`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/assets/trace.png` & `nessai-0.9.1/docs/assets/trace.png`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/conf.py` & `nessai-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/further-details.rst` & `nessai-0.9.1/docs/further-details.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/gaussian-example.rst` & `nessai-0.9.1/docs/gaussian-example.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/gravitational-wave-inference.rst` & `nessai-0.9.1/docs/gravitational-wave-inference.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/importance-nested-sampling.rst` & `nessai-0.9.1/docs/importance-nested-sampling.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/index.rst` & `nessai-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/installation.rst` & `nessai-0.9.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/normalising-flows-configuration.rst` & `nessai-0.9.1/docs/normalising-flows-configuration.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/parallelisation.rst` & `nessai-0.9.1/docs/parallelisation.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/reparameterisations.rst` & `nessai-0.9.1/docs/reparameterisations.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/running-the-sampler.rst` & `nessai-0.9.1/docs/running-the-sampler.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/docs/sampler-configuration.rst` & `nessai-0.9.1/docs/sampler-configuration.rst`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/2d_gaussian.py` & `nessai-0.9.1/examples/2d_gaussian.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/augmented_example.py` & `nessai-0.9.1/examples/augmented_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/bilby_example.py` & `nessai-0.9.1/examples/bilby_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/bilby_unbounded_priors.py` & `nessai-0.9.1/examples/bilby_unbounded_priors.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/corner_plot_example.py` & `nessai-0.9.1/examples/corner_plot_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/eggbox.py` & `nessai-0.9.1/examples/eggbox.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/gw/basic_gw_example.py` & `nessai-0.9.1/examples/gw/basic_gw_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/gw/calibration_example.py` & `nessai-0.9.1/examples/gw/calibration_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/gw/full_gw_example.py` & `nessai-0.9.1/examples/gw/full_gw_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/half_gaussian.py` & `nessai-0.9.1/examples/half_gaussian.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/importance_nested_sampler/basic_ins_example.py` & `nessai-0.9.1/examples/importance_nested_sampler/basic_ins_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/importance_nested_sampler/nsf_unit_hypercube.py` & `nessai-0.9.1/examples/importance_nested_sampler/nsf_unit_hypercube.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/parallelisation_example.py` & `nessai-0.9.1/examples/parallelisation_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/reparameterisations_example.py` & `nessai-0.9.1/examples/reparameterisations_example.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/rosenbrock.py` & `nessai-0.9.1/examples/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/examples/unbounded_prior.py` & `nessai-0.9.1/examples/unbounded_prior.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/__init__.py` & `nessai-0.9.1/nessai/__init__.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/config.py` & `nessai-0.9.1/nessai/config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/evidence.py` & `nessai-0.9.1/nessai/evidence.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/flowmodel/base.py` & `nessai-0.9.1/nessai/flowmodel/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/flowmodel/config.py` & `nessai-0.9.1/nessai/flowmodel/config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/flowmodel/importance.py` & `nessai-0.9.1/nessai/flowmodel/importance.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/flowmodel/utils.py` & `nessai-0.9.1/nessai/flowmodel/utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/flows/base.py` & `nessai-0.9.1/nessai/flows/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/flows/distributions.py` & `nessai-0.9.1/nessai/flows/distributions.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/flows/maf.py` & `nessai-0.9.1/nessai/flows/maf.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/flows/nets.py` & `nessai-0.9.1/nessai/flows/nets.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/flows/nsf.py` & `nessai-0.9.1/nessai/flows/nsf.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/flows/realnvp.py` & `nessai-0.9.1/nessai/flows/realnvp.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/flows/transforms.py` & `nessai-0.9.1/nessai/flows/transforms.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/flows/utils.py` & `nessai-0.9.1/nessai/flows/utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/flowsampler.py` & `nessai-0.9.1/nessai/flowsampler.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/gw/proposal.py` & `nessai-0.9.1/nessai/gw/proposal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/gw/reparameterisations.py` & `nessai-0.9.1/nessai/gw/reparameterisations.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/gw/utils.py` & `nessai-0.9.1/nessai/gw/utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/livepoint.py` & `nessai-0.9.1/nessai/livepoint.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/model.py` & `nessai-0.9.1/nessai/model.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/plot.py` & `nessai-0.9.1/nessai/plot.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/posterior.py` & `nessai-0.9.1/nessai/posterior.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/priors.py` & `nessai-0.9.1/nessai/priors.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/proposal/analytic.py` & `nessai-0.9.1/nessai/proposal/analytic.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/proposal/augmented.py` & `nessai-0.9.1/nessai/proposal/augmented.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/proposal/base.py` & `nessai-0.9.1/nessai/proposal/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/proposal/flowproposal.py` & `nessai-0.9.1/nessai/proposal/flowproposal.py`

 * *Files 0% similar despite different names*

```diff
@@ -640,15 +640,17 @@
                             else:
                                 patterns = list(parameters)
                         else:
                             patterns = parameters.copy()
                         matches = []
                         for pattern in patterns:
                             r = re.compile(pattern)
-                            matches += list(filter(r.match, self.model.names))
+                            matches += list(
+                                filter(r.fullmatch, self.model.names)
+                            )
                         default_config["parameters"] = matches
                     else:
                         logger.warning(
                             "Reparameterisation might be missing parameters!"
                         )
 
                 except ValueError:
```

### Comparing `nessai-0.9.0/nessai/proposal/importance.py` & `nessai-0.9.1/nessai/proposal/importance.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/proposal/rejection.py` & `nessai-0.9.1/nessai/proposal/rejection.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/proposal/utils.py` & `nessai-0.9.1/nessai/proposal/utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/reparameterisations/__init__.py` & `nessai-0.9.1/nessai/reparameterisations/__init__.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/reparameterisations/angle.py` & `nessai-0.9.1/nessai/reparameterisations/angle.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/reparameterisations/base.py` & `nessai-0.9.1/nessai/reparameterisations/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/reparameterisations/combined.py` & `nessai-0.9.1/nessai/reparameterisations/combined.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/reparameterisations/null.py` & `nessai-0.9.1/nessai/reparameterisations/null.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/reparameterisations/rescale.py` & `nessai-0.9.1/nessai/reparameterisations/rescale.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/reparameterisations/utils.py` & `nessai-0.9.1/nessai/reparameterisations/utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/samplers/base.py` & `nessai-0.9.1/nessai/samplers/base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/samplers/importancesampler.py` & `nessai-0.9.1/nessai/samplers/importancesampler.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/samplers/nestedsampler.py` & `nessai-0.9.1/nessai/samplers/nestedsampler.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/__init__.py` & `nessai-0.9.1/nessai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/bilbyutils.py` & `nessai-0.9.1/nessai/utils/bilbyutils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/distance.py` & `nessai-0.9.1/nessai/utils/distance.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/distributions.py` & `nessai-0.9.1/nessai/utils/distributions.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/hist.py` & `nessai-0.9.1/nessai/utils/hist.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/indices.py` & `nessai-0.9.1/nessai/utils/indices.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/information.py` & `nessai-0.9.1/nessai/utils/information.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/io.py` & `nessai-0.9.1/nessai/utils/io.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/logging.py` & `nessai-0.9.1/nessai/utils/logging.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/multiprocessing.py` & `nessai-0.9.1/nessai/utils/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/optimise.py` & `nessai-0.9.1/nessai/utils/optimise.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/rescaling.py` & `nessai-0.9.1/nessai/utils/rescaling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/sampling.py` & `nessai-0.9.1/nessai/utils/sampling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/sorting.py` & `nessai-0.9.1/nessai/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/stats.py` & `nessai-0.9.1/nessai/utils/stats.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/structures.py` & `nessai-0.9.1/nessai/utils/structures.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/testing.py` & `nessai-0.9.1/nessai/utils/testing.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/threading.py` & `nessai-0.9.1/nessai/utils/threading.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai/utils/torchutils.py` & `nessai-0.9.1/nessai/utils/torchutils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/nessai.egg-info/PKG-INFO` & `nessai-0.9.1/nessai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nessai
-Version: 0.9.0
+Version: 0.9.1
 Summary: Nessai: Nested Sampling with Artificial Intelligence
 Home-page: https://github.com/mj-will/nessai
 Author: Michael J. Williams
 Author-email: m.williams.4@research.gla.ac.uk
 Project-URL: Documentation, https://nessai.readthedocs.io/
 Keywords: nested sampling,normalising flows,machine learning
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `nessai-0.9.0/nessai.egg-info/SOURCES.txt` & `nessai-0.9.1/nessai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/pyproject.toml` & `nessai-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/setup.cfg` & `nessai-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/conftest.py` & `nessai-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_bilby_compatibility.py` & `nessai-0.9.1/tests/test_bilby_compatibility.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_config.py` & `nessai-0.9.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_deprecation_warnings.py` & `nessai-0.9.1/tests/test_deprecation_warnings.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_evidence/test_ins_evidence.py` & `nessai-0.9.1/tests/test_evidence/test_ins_evidence.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_evidence/test_standard_evidence.py` & `nessai-0.9.1/tests/test_evidence/test_standard_evidence.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_flowmodel/test_flowmodel_base.py` & `nessai-0.9.1/tests/test_flowmodel/test_flowmodel_base.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_flowmodel/test_flowmodel_importance.py` & `nessai-0.9.1/tests/test_flowmodel/test_flowmodel_importance.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_flowmodel/test_flowmodel_utils.py` & `nessai-0.9.1/tests/test_flowmodel/test_flowmodel_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_flows/test_base_flow.py` & `nessai-0.9.1/tests/test_flows/test_base_flow.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_flows/test_distributions/test_multivariate_normal.py` & `nessai-0.9.1/tests/test_flows/test_distributions/test_multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_flows/test_flow_utils.py` & `nessai-0.9.1/tests/test_flows/test_flow_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_flows/test_included_flows.py` & `nessai-0.9.1/tests/test_flows/test_included_flows.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_flows/test_nets.py` & `nessai-0.9.1/tests/test_flows/test_nets.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_flows/test_specific_flows.py` & `nessai-0.9.1/tests/test_flows/test_specific_flows.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_flowsampler.py` & `nessai-0.9.1/tests/test_flowsampler.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_gw/conftest.py` & `nessai-0.9.1/tests/test_gw/conftest.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_gw/test_distance_converters.py` & `nessai-0.9.1/tests/test_gw/test_distance_converters.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_gw/test_gw_proposal.py` & `nessai-0.9.1/tests/test_gw/test_gw_proposal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_gw/test_gw_reparameterisations.py` & `nessai-0.9.1/tests/test_gw/test_gw_reparameterisations.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_gw/test_reparameterisation_integration.py` & `nessai-0.9.1/tests/test_gw/test_reparameterisation_integration.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_livepoint.py` & `nessai-0.9.1/tests/test_livepoint.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_model.py` & `nessai-0.9.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_plot.py` & `nessai-0.9.1/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_posterior.py` & `nessai-0.9.1/tests/test_posterior.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_priors.py` & `nessai-0.9.1/tests/test_priors.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_analytic.py` & `nessai-0.9.1/tests/test_proposal/test_analytic.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_augmented.py` & `nessai-0.9.1/tests/test_proposal/test_augmented.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_base_proposal.py` & `nessai-0.9.1/tests/test_proposal/test_base_proposal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_add_reparam.py` & `nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_add_reparam.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,19 +82,20 @@
 
 
 @pytest.mark.integration_test
 def test_default_reparameterisations(caplog, tmpdir):
     """Assert that by default the reparameterisation is RescaleToBounds"""
     caplog.set_level("INFO")
     model = MagicMock()
-    model.names = ["x", "y"]
+    model.names = ["x1", "x10", "x11"]
     model.bounds = {p: [-1, 1] for p in model.names}
     model.reparameterisations = None
     proposal = FlowProposal(
         model, poolsize=100, output=str(tmpdir.mkdir("test"))
     )
     # Mocked model so can't verify rescaling
     proposal.verify_rescaling = MagicMock()
     proposal.initialise()
     reparams = list(proposal._reparameterisation.values())
     assert len(reparams) == 1
-    assert reparams[0].parameters == ["x", "y"]
+    assert reparams[0].parameters == ["x1", "x10", "x11"]
+    assert proposal.rescale_parameters == ["x1", "x10", "x11"]
```

### Comparing `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_configuration.py` & `nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_configuration.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_draw.py` & `nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_draw.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_flow.py` & `nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_flow.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_init_resume.py` & `nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_init_resume.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_integration.py` & `nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_integration.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_plots.py` & `nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_plots.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_population.py` & `nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_population.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_properties.py` & `nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_properties.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_flowproposal/test_flowproposal_rescaling.py` & `nessai-0.9.1/tests/test_proposal/test_flowproposal/test_flowproposal_rescaling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_importance/conftest.py` & `nessai-0.9.1/tests/test_proposal/test_importance/conftest.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_importance/test_config.py` & `nessai-0.9.1/tests/test_proposal/test_importance/test_config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_importance/test_prob.py` & `nessai-0.9.1/tests/test_proposal/test_importance/test_prob.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_importance/test_properties.py` & `nessai-0.9.1/tests/test_proposal/test_importance/test_properties.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_importance/test_rescaling.py` & `nessai-0.9.1/tests/test_proposal/test_importance/test_rescaling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_importance/test_resume.py` & `nessai-0.9.1/tests/test_proposal/test_importance/test_resume.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_importance/test_sampling.py` & `nessai-0.9.1/tests/test_proposal/test_importance/test_sampling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_importance/test_training.py` & `nessai-0.9.1/tests/test_proposal/test_importance/test_training.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_rejection.py` & `nessai-0.9.1/tests/test_proposal/test_rejection.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_proposal/test_utils.py` & `nessai-0.9.1/tests/test_proposal/test_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_reparameterisations/conftest.py` & `nessai-0.9.1/tests/test_reparameterisations/conftest.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_reparameterisations/test_angle.py` & `nessai-0.9.1/tests/test_reparameterisations/test_angle.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_reparameterisations/test_angle_pair.py` & `nessai-0.9.1/tests/test_reparameterisations/test_angle_pair.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_reparameterisations/test_base_reparameterisation.py` & `nessai-0.9.1/tests/test_reparameterisations/test_base_reparameterisation.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_reparameterisations/test_combined.py` & `nessai-0.9.1/tests/test_reparameterisations/test_combined.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_reparameterisations/test_get_reparameterisation.py` & `nessai-0.9.1/tests/test_reparameterisations/test_get_reparameterisation.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_reparameterisations/test_null.py` & `nessai-0.9.1/tests/test_reparameterisations/test_null.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_reparameterisations/test_rescale_to_bounds.py` & `nessai-0.9.1/tests/test_reparameterisations/test_rescale_to_bounds.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_reparameterisations/test_scale_and_shift.py` & `nessai-0.9.1/tests/test_reparameterisations/test_scale_and_shift.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_reparameterisations/test_to_cartesian.py` & `nessai-0.9.1/tests/test_reparameterisations/test_to_cartesian.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_base_sampler.py` & `nessai-0.9.1/tests/test_samplers/test_base_sampler.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/conftest.py` & `nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/conftest.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_config.py` & `nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/test_config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_plots.py` & `nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/test_plots.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_proposal.py` & `nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/test_proposal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_result.py` & `nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/test_result.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_samples.py` & `nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/test_samples.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_importance_nested_sampler/test_threshold.py` & `nessai-0.9.1/tests/test_samplers/test_importance_nested_sampler/test_threshold.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_core_sampling.py` & `nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_core_sampling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_flow_proposal.py` & `nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_flow_proposal.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_general_config.py` & `nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_general_config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_live_points.py` & `nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_live_points.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_manage_state.py` & `nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_manage_state.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_ns_plotting.py` & `nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_ns_plotting.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_properties.py` & `nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_properties.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_proposal_config.py` & `nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_proposal_config.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_resume.py` & `nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_resume.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_samplers/test_nested_sampler/test_yield_sample.py` & `nessai-0.9.1/tests/test_samplers/test_nested_sampler/test_yield_sample.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_sampling/test_ins_sampling.py` & `nessai-0.9.1/tests/test_sampling/test_ins_sampling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_sampling/test_standard_sampling.py` & `nessai-0.9.1/tests/test_sampling/test_standard_sampling.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_bilbyutils.py` & `nessai-0.9.1/tests/test_utils/test_bilbyutils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_distance_utils.py` & `nessai-0.9.1/tests/test_utils/test_distance_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_distribution_utils.py` & `nessai-0.9.1/tests/test_utils/test_distribution_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_hist_utils.py` & `nessai-0.9.1/tests/test_utils/test_hist_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_indices_utils.py` & `nessai-0.9.1/tests/test_utils/test_indices_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_io_utils.py` & `nessai-0.9.1/tests/test_utils/test_io_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_logging_utils.py` & `nessai-0.9.1/tests/test_utils/test_logging_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_multiprocessing_utils.py` & `nessai-0.9.1/tests/test_utils/test_multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_optimise_utils.py` & `nessai-0.9.1/tests/test_utils/test_optimise_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_rescaling_utils.py` & `nessai-0.9.1/tests/test_utils/test_rescaling_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_sampling_utils.py` & `nessai-0.9.1/tests/test_utils/test_sampling_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_sorting_utils.py` & `nessai-0.9.1/tests/test_utils/test_sorting_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_stats_utils.py` & `nessai-0.9.1/tests/test_utils/test_stats_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_structures_utils.py` & `nessai-0.9.1/tests/test_utils/test_structures_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_testing_utils.py` & `nessai-0.9.1/tests/test_utils/test_testing_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_threading_utils.py` & `nessai-0.9.1/tests/test_utils/test_threading_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_utils/test_torchtutils_utils.py` & `nessai-0.9.1/tests/test_utils/test_torchtutils_utils.py`

 * *Files identical despite different names*

### Comparing `nessai-0.9.0/tests/test_version.py` & `nessai-0.9.1/tests/test_version.py`

 * *Files identical despite different names*

