# Comparing `tmp/pyrfu-2.4.4.tar.gz` & `tmp/pyrfu-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfu-2.4.4.tar", last modified: Thu Jul 27 14:08:27 2023, max compression
+gzip compressed data, was "pyrfu-2.4.5.tar", last modified: Tue Aug  1 09:02:49 2023, max compression
```

## Comparing `pyrfu-2.4.4.tar` & `pyrfu-2.4.5.tar`

### file list

```diff
@@ -1,314 +1,288 @@
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.539250 pyrfu-2.4.4/
--rw-r--r--   0 louisr     (501) staff       (20)       69 2023-04-21 10:39:09.000000 pyrfu-2.4.4/.flake8
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.627836 pyrfu-2.4.4/.github/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.667641 pyrfu-2.4.4/.github/workflows/
--rw-r--r--   0 louisr     (501) staff       (20)      625 2023-07-21 11:39:19.000000 pyrfu-2.4.4/.github/workflows/flake8.yml
--rw-r--r--   0 louisr     (501) staff       (20)      823 2023-05-14 19:49:15.000000 pyrfu-2.4.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 louisr     (501) staff       (20)      643 2023-07-21 11:38:43.000000 pyrfu-2.4.4/.github/workflows/pylint.yml
--rw-r--r--   0 louisr     (501) staff       (20)      289 2023-06-09 14:44:34.000000 pyrfu-2.4.4/.gitignore
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.672539 pyrfu-2.4.4/.idea/
--rw-r--r--   0 louisr     (501) staff       (20)      294 2023-07-27 10:47:39.000000 pyrfu-2.4.4/.idea/aws.xml
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.673963 pyrfu-2.4.4/.idea/codeStyles/
--rw-r--r--   0 louisr     (501) staff       (20)      153 2023-04-20 14:38:38.000000 pyrfu-2.4.4/.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.676057 pyrfu-2.4.4/.idea/inspectionProfiles/
--rw-r--r--   0 louisr     (501) staff       (20)      803 2023-04-20 14:38:38.000000 pyrfu-2.4.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 louisr     (501) staff       (20)      174 2023-04-20 14:38:38.000000 pyrfu-2.4.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.4/.idea/vcs (LAPTOP-E2ISLACJ's conflicted copy 2022-09-29).xml
--rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.4/.idea/vcs.xml
--rw-r--r--   0 louisr     (501) staff       (20)    17383 2023-04-20 14:38:38.000000 pyrfu-2.4.4/.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml
--rw-r--r--   0 louisr     (501) staff       (20)     1499 2023-07-21 10:56:15.000000 pyrfu-2.4.4/.pre-commit-config.yaml
--rw-r--r--   0 louisr     (501) staff       (20)     2237 2023-07-21 11:09:58.000000 pyrfu-2.4.4/CONTRIBUTING.rst
--rw-r--r--   0 louisr     (501) staff       (20)     1067 2023-04-20 14:38:38.000000 pyrfu-2.4.4/LICENSE.txt
--rw-r--r--   0 louisr     (501) staff       (20)      438 2023-04-20 14:38:38.000000 pyrfu-2.4.4/MANIFEST.in
--rw-r--r--   0 louisr     (501) staff       (20)     8802 2023-07-27 14:08:27.538152 pyrfu-2.4.4/PKG-INFO
--rw-r--r--   0 louisr     (501) staff       (20)     6429 2023-07-21 11:27:45.000000 pyrfu-2.4.4/README.rst
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.678747 pyrfu-2.4.4/docs/
--rw-r--r--   0 louisr     (501) staff       (20)      658 2023-07-21 12:01:16.000000 pyrfu-2.4.4/docs/Makefile
--rw-r--r--   0 louisr     (501) staff       (20)     7075 2023-07-21 11:17:04.000000 pyrfu-2.4.4/docs/conf.py
--rw-r--r--   0 louisr     (501) staff       (20)     3034 2023-07-27 14:06:50.000000 pyrfu-2.4.4/pyproject.toml
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.680045 pyrfu-2.4.4/pyrfu/
--rw-r--r--   0 louisr     (501) staff       (20)      334 2023-07-27 14:06:50.000000 pyrfu-2.4.4/pyrfu/__init__.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.685728 pyrfu-2.4.4/pyrfu/__pycache__/
--rw-r--r--   0 louisr     (501) staff       (20)      521 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.689203 pyrfu-2.4.4/pyrfu/dispersion/
--rw-r--r--   0 louisr     (501) staff       (20)      381 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/dispersion/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)    10001 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/dispersion/disp_surf_calc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3487 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/dispersion/one_fluid_dispersion.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.693595 pyrfu-2.4.4/pyrfu/lp/
--rw-r--r--   0 louisr     (501) staff       (20)     5325 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/lp/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     3604 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/lp/photo_current.py
--rw-r--r--   0 louisr     (501) staff       (20)     3295 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/lp/thermal_current.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.108832 pyrfu-2.4.4/pyrfu/mms/
--rw-r--r--   0 louisr     (501) staff       (20)     6045 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)      726 2023-05-15 20:42:04.000000 pyrfu-2.4.4/pyrfu/mms/ancillary.json
--rw-r--r--   0 louisr     (501) staff       (20)     4954 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/calculate_epsilon.py
--rw-r--r--   0 louisr     (501) staff       (20)       35 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/config.json
--rw-r--r--   0 louisr     (501) staff       (20)     2280 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/copy_files.py
--rw-r--r--   0 louisr     (501) staff       (20)     2195 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/copy_files_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     2914 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/correct_edp_probe_timing.py
--rw-r--r--   0 louisr     (501) staff       (20)     1759 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/db_get_ts.py
--rw-r--r--   0 louisr     (501) staff       (20)     1574 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/db_get_variable.py
--rw-r--r--   0 louisr     (501) staff       (20)     1093 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/db_init.py
--rw-r--r--   0 louisr     (501) staff       (20)     2558 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/def2psd.py
--rw-r--r--   0 louisr     (501) staff       (20)     1631 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/dft_time_shift.py
--rw-r--r--   0 louisr     (501) staff       (20)     5503 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/download_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     7477 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/download_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     2533 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/dpf2psd.py
--rw-r--r--   0 louisr     (501) staff       (20)     3166 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/dsl2gse.py
--rw-r--r--   0 louisr     (501) staff       (20)     3041 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/dsl2gsm.py
--rw-r--r--   0 louisr     (501) staff       (20)     6423 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_ang_ang.py
--rw-r--r--   0 louisr     (501) staff       (20)     5431 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_combine_proton_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     1502 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_combine_proton_skymap.py
--rw-r--r--   0 louisr     (501) staff       (20)    10923 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_combine_proton_spec.py
--rw-r--r--   0 louisr     (501) staff       (20)     4645 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_moments.py
--rw-r--r--   0 louisr     (501) staff       (20)     1782 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)     3768 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     1996 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_pad_combine_sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_pad_spinavg.py
--rw-r--r--   0 louisr     (501) staff       (20)     3297 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_proton_correction.py
--rw-r--r--   0 louisr     (501) staff       (20)     2154 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_skymap.py
--rw-r--r--   0 louisr     (501) staff       (20)     4590 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_skymap_combine_sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3515 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_spec_combine_sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3390 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/eis_spin_avg.py
--rw-r--r--   0 louisr     (501) staff       (20)     2983 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/estimate_phase_speed.py
--rw-r--r--   0 louisr     (501) staff       (20)     4386 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_active_eyes.py
--rw-r--r--   0 louisr     (501) staff       (20)     3968 2023-05-15 20:42:14.000000 pyrfu-2.4.4/pyrfu/mms/feeps_bad_data.json
--rw-r--r--   0 louisr     (501) staff       (20)     1697 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_correct_energies.py
--rw-r--r--   0 louisr     (501) staff       (20)     3350 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/feeps_energy_table.py
--rw-r--r--   0 louisr     (501) staff       (20)     1991 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_flat_field_corrections.py
--rw-r--r--   0 louisr     (501) staff       (20)     2982 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)     6204 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     2520 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_pad_spinavg.py
--rw-r--r--   0 louisr     (501) staff       (20)     4567 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_pitch_angles.py
--rw-r--r--   0 louisr     (501) staff       (20)     5604 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_remove_bad_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     2003 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_remove_sun.py
--rw-r--r--   0 louisr     (501) staff       (20)     1810 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_sector_spec.py
--rw-r--r--   0 louisr     (501) staff       (20)     1435 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_spin_avg.py
--rw-r--r--   0 louisr     (501) staff       (20)     1292 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/feeps_split_integral_ch.py
--rw-r--r--   0 louisr     (501) staff       (20)     2797 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/fft_bandpass.py
--rw-r--r--   0 louisr     (501) staff       (20)    11773 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/fk_power_spectrum_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3062 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/get_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     9972 2023-07-27 14:04:04.000000 pyrfu-2.4.4/pyrfu/mms/get_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)     4726 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/get_eis_allt.py
--rw-r--r--   0 louisr     (501) staff       (20)     4496 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/get_feeps_alleyes.py
--rw-r--r--   0 louisr     (501) staff       (20)     2524 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/get_feeps_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)     6176 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/get_hpca_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)     7054 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/get_pitch_angle_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)    11323 2023-07-27 14:04:04.000000 pyrfu-2.4.4/pyrfu/mms/get_ts.py
--rw-r--r--   0 louisr     (501) staff       (20)      926 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/get_variable.py
--rw-r--r--   0 louisr     (501) staff       (20)     1771 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/hpca_calc_anodes.py
--rw-r--r--   0 louisr     (501) staff       (20)     1395 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/hpca_energies.py
--rw-r--r--   0 louisr     (501) staff       (20)     5663 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/hpca_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     1620 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/hpca_spin_sum.py
--rw-r--r--   0 louisr     (501) staff       (20)     5642 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/lh_wave_analysis.py
--rw-r--r--   0 louisr     (501) staff       (20)     6789 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/list_files.py
--rw-r--r--   0 louisr     (501) staff       (20)     4230 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/list_files_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     2795 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/load_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     2860 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/load_brst_segments.py
--rw-r--r--   0 louisr     (501) staff       (20)     4016 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/make_model_kappa.py
--rw-r--r--   0 louisr     (501) staff       (20)     7022 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/make_model_rq.py
--rw-r--r--   0 louisr     (501) staff       (20)     7039 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/make_model_vdf.py
--rw-r--r--   0 louisr     (501) staff       (20)    25195 2023-07-21 11:00:36.000000 pyrfu-2.4.4/pyrfu/mms/mms_keys.json
--rw-r--r--   0 louisr     (501) staff       (20)     6101 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/probe_align_times.py
--rw-r--r--   0 louisr     (501) staff       (20)     2782 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/psd2def.py
--rw-r--r--   0 louisr     (501) staff       (20)     2796 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/psd2dpf.py
--rw-r--r--   0 louisr     (501) staff       (20)    18460 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/psd_moments.py
--rw-r--r--   0 louisr     (501) staff       (20)     3343 2023-07-21 11:04:25.000000 pyrfu-2.4.4/pyrfu/mms/psd_rebin.py
--rw-r--r--   0 louisr     (501) staff       (20)     2610 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/read_feeps_sector_masks_csv.py
--rw-r--r--   0 louisr     (501) staff       (20)     8942 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/reduce.py
--rw-r--r--   0 louisr     (501) staff       (20)     5397 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/remove_edist_background.py
--rw-r--r--   0 louisr     (501) staff       (20)     2034 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/remove_idist_background.py
--rw-r--r--   0 louisr     (501) staff       (20)     3131 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/remove_imoms_background.py
--rw-r--r--   0 louisr     (501) staff       (20)     7075 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/rotate_tensor.py
--rw-r--r--   0 louisr     (501) staff       (20)     4320 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/scpot2ne.py
--rw-r--r--   0 louisr     (501) staff       (20)      945 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/spectr_to_dataset.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.161895 pyrfu-2.4.4/pyrfu/mms/sun/
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3134 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3866 2023-07-21 11:03:34.000000 pyrfu-2.4.4/pyrfu/mms/tokenize.py
--rw-r--r--   0 louisr     (501) staff       (20)     3248 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/vdf_elim.py
--rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/vdf_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)    11440 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/vdf_projection.py
--rw-r--r--   0 louisr     (501) staff       (20)     8287 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/vdf_reduce.py
--rw-r--r--   0 louisr     (501) staff       (20)     2487 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/vdf_to_e64.py
--rw-r--r--   0 louisr     (501) staff       (20)     2337 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/mms/whistler_b2e.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.167242 pyrfu-2.4.4/pyrfu/models/
--rw-r--r--   0 louisr     (501) staff       (20)      347 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/models/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     2810 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/models/igrf.py
--rw-r--r--   0 louisr     (501) staff       (20)    26798 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/models/igrf13coeffs.csv
--rw-r--r--   0 louisr     (501) staff       (20)     6038 2023-07-21 11:40:35.000000 pyrfu-2.4.4/pyrfu/models/magnetopause_normal.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.191429 pyrfu-2.4.4/pyrfu/plot/
--rw-r--r--   0 louisr     (501) staff       (20)     1582 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     1725 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/add_position.py
--rw-r--r--   0 louisr     (501) staff       (20)     2366 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/annotate_heatmap.py
--rw-r--r--   0 louisr     (501) staff       (20)      935 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/colorbar.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.192622 pyrfu-2.4.4/pyrfu/plot/logo/
--rw-r--r--   0 louisr     (501) staff       (20)    43962 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg
--rw-r--r--   0 louisr     (501) staff       (20)     1108 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/make_labels.py
--rw-r--r--   0 louisr     (501) staff       (20)     3808 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/mms_pl_config.py
--rw-r--r--   0 louisr     (501) staff       (20)     2856 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/pl_scatter_matrix.py
--rw-r--r--   0 louisr     (501) staff       (20)     1539 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/pl_tx.py
--rw-r--r--   0 louisr     (501) staff       (20)     3832 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_ang_ang.py
--rw-r--r--   0 louisr     (501) staff       (20)     1764 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_clines.py
--rw-r--r--   0 louisr     (501) staff       (20)     2446 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_heatmap.py
--rw-r--r--   0 louisr     (501) staff       (20)     1431 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_line.py
--rw-r--r--   0 louisr     (501) staff       (20)     3646 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_magnetosphere.py
--rw-r--r--   0 louisr     (501) staff       (20)     2212 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_projection.py
--rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_reduced_2d.py
--rw-r--r--   0 louisr     (501) staff       (20)    11753 2023-07-21 11:05:55.000000 pyrfu-2.4.4/pyrfu/plot/plot_sitl_overview.py
--rw-r--r--   0 louisr     (501) staff       (20)     4627 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_spectr.py
--rw-r--r--   0 louisr     (501) staff       (20)     2423 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/plot_surf.py
--rw-r--r--   0 louisr     (501) staff       (20)     1511 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/span_tint.py
--rw-r--r--   0 louisr     (501) staff       (20)     2455 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/plot/zoom.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.523202 pyrfu-2.4.4/pyrfu/pyrf/
--rw-r--r--   0 louisr     (501) staff       (20)     5552 2023-07-27 14:06:41.000000 pyrfu-2.4.4/pyrfu/pyrf/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     2078 2023-07-21 22:14:58.000000 pyrfu-2.4.4/pyrfu/pyrf/autocorr.py
--rw-r--r--   0 louisr     (501) staff       (20)     2651 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/average_vdf.py
--rw-r--r--   0 louisr     (501) staff       (20)     1489 2023-07-22 21:41:45.000000 pyrfu-2.4.4/pyrfu/pyrf/avg_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     5023 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/c_4_grad.py
--rw-r--r--   0 louisr     (501) staff       (20)     4196 2023-07-21 10:45:02.000000 pyrfu-2.4.4/pyrfu/pyrf/c_4_j.py
--rw-r--r--   0 louisr     (501) staff       (20)     1315 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/c_4_k.py
--rw-r--r--   0 louisr     (501) staff       (20)     2633 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/c_4_v.py
--rw-r--r--   0 louisr     (501) staff       (20)     2510 2023-07-21 20:18:55.000000 pyrfu-2.4.4/pyrfu/pyrf/calc_ag.py
--rw-r--r--   0 louisr     (501) staff       (20)     1842 2023-07-21 20:22:06.000000 pyrfu-2.4.4/pyrfu/pyrf/calc_agyro.py
--rw-r--r--   0 louisr     (501) staff       (20)     2270 2023-07-21 20:51:36.000000 pyrfu-2.4.4/pyrfu/pyrf/calc_dng.py
--rw-r--r--   0 louisr     (501) staff       (20)      738 2023-07-21 17:28:19.000000 pyrfu-2.4.4/pyrfu/pyrf/calc_dt.py
--rw-r--r--   0 louisr     (501) staff       (20)      761 2023-07-21 17:28:19.000000 pyrfu-2.4.4/pyrfu/pyrf/calc_fs.py
--rw-r--r--   0 louisr     (501) staff       (20)     2233 2023-07-21 21:02:32.000000 pyrfu-2.4.4/pyrfu/pyrf/calc_sqrtq.py
--rw-r--r--   0 louisr     (501) staff       (20)     1223 2023-07-27 14:06:45.000000 pyrfu-2.4.4/pyrfu/pyrf/cart2sph.py
--rw-r--r--   0 louisr     (501) staff       (20)     1929 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/cart2sph_ts.py
--rw-r--r--   0 louisr     (501) staff       (20)     1723 2023-07-21 20:27:19.000000 pyrfu-2.4.4/pyrfu/pyrf/cdfepoch2datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)     1746 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/compress_cwt.py
--rw-r--r--   0 louisr     (501) staff       (20)     3430 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/convert_fac.py
--rw-r--r--   0 louisr     (501) staff       (20)     6502 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/corr_deriv.py
--rw-r--r--   0 louisr     (501) staff       (20)    10371 2023-07-21 21:07:03.000000 pyrfu-2.4.4/pyrfu/pyrf/cotrans.py
--rw-r--r--   0 louisr     (501) staff       (20)     1430 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/cross.py
--rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/date_str.py
--rw-r--r--   0 louisr     (501) staff       (20)     1118 2023-07-21 21:18:32.000000 pyrfu-2.4.4/pyrfu/pyrf/datetime2iso8601.py
--rw-r--r--   0 louisr     (501) staff       (20)      842 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/datetime642iso8601.py
--rw-r--r--   0 louisr     (501) staff       (20)      870 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/datetime642ttns.py
--rw-r--r--   0 louisr     (501) staff       (20)      694 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/datetime642unix.py
--rw-r--r--   0 louisr     (501) staff       (20)     2570 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/dec_par_perp.py
--rw-r--r--   0 louisr     (501) staff       (20)     2394 2023-07-27 14:03:26.000000 pyrfu-2.4.4/pyrfu/pyrf/dist_append.py
--rw-r--r--   0 louisr     (501) staff       (20)     1715 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/dot.py
--rw-r--r--   0 louisr     (501) staff       (20)     1594 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/dynamic_press.py
--rw-r--r--   0 louisr     (501) staff       (20)     2283 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/e_vxb.py
--rw-r--r--   0 louisr     (501) staff       (20)     1910 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/eb_nrf.py
--rw-r--r--   0 louisr     (501) staff       (20)    36446 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/ebsp.py
--rw-r--r--   0 louisr     (501) staff       (20)     3678 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/edb.py
--rw-r--r--   0 louisr     (501) staff       (20)      593 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/end.py
--rw-r--r--   0 louisr     (501) staff       (20)     3009 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/estimate.py
--rw-r--r--   0 louisr     (501) staff       (20)     1880 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/extend_tint.py
--rw-r--r--   0 louisr     (501) staff       (20)     3736 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/filt.py
--rw-r--r--   0 louisr     (501) staff       (20)     1971 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/find_closest.py
--rw-r--r--   0 louisr     (501) staff       (20)     3795 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/get_omni_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     1298 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/gradient.py
--rw-r--r--   0 louisr     (501) staff       (20)      987 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/gse2gsm.py
--rw-r--r--   0 louisr     (501) staff       (20)     2401 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/histogram.py
--rw-r--r--   0 louisr     (501) staff       (20)     3155 2023-07-21 10:34:50.000000 pyrfu-2.4.4/pyrfu/pyrf/histogram2d.py
--rw-r--r--   0 louisr     (501) staff       (20)     1684 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/increments.py
--rw-r--r--   0 louisr     (501) staff       (20)    18234 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/int_sph_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)     2024 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/integrate.py
--rw-r--r--   0 louisr     (501) staff       (20)     6075 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/iplasma_calc.py
--rw-r--r--   0 louisr     (501) staff       (20)      585 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/iso2unix.py
--rw-r--r--   0 louisr     (501) staff       (20)      875 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/iso86012datetime.py
--rw-r--r--   0 louisr     (501) staff       (20)      626 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/iso86012datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)     1061 2023-07-21 12:04:40.000000 pyrfu-2.4.4/pyrfu/pyrf/iso86012timevec.py
--rw-r--r--   0 louisr     (501) staff       (20)      999 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/l_shell.py
--rw-r--r--   0 louisr     (501) staff       (20)     1281 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/lowpass.py
--rw-r--r--   0 louisr     (501) staff       (20)     2438 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/magnetosphere.py
--rw-r--r--   0 louisr     (501) staff       (20)     4500 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/match_phibe_dir.py
--rw-r--r--   0 louisr     (501) staff       (20)     1794 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/match_phibe_v.py
--rw-r--r--   0 louisr     (501) staff       (20)     2153 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/mean.py
--rw-r--r--   0 louisr     (501) staff       (20)     2387 2023-07-21 10:33:13.000000 pyrfu-2.4.4/pyrfu/pyrf/mean_bins.py
--rw-r--r--   0 louisr     (501) staff       (20)     1220 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/mean_field.py
--rw-r--r--   0 louisr     (501) staff       (20)     2231 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/medfilt.py
--rw-r--r--   0 louisr     (501) staff       (20)     2358 2023-07-21 10:33:35.000000 pyrfu-2.4.4/pyrfu/pyrf/median_bins.py
--rw-r--r--   0 louisr     (501) staff       (20)     1757 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/movmean.py
--rw-r--r--   0 louisr     (501) staff       (20)     4661 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/mva.py
--rw-r--r--   0 louisr     (501) staff       (20)     8345 2023-07-21 11:08:11.000000 pyrfu-2.4.4/pyrfu/pyrf/mva_gui.py
--rw-r--r--   0 louisr     (501) staff       (20)     1473 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/new_xyz.py
--rw-r--r--   0 louisr     (501) staff       (20)      957 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/norm.py
--rw-r--r--   0 louisr     (501) staff       (20)      957 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/normalize.py
--rw-r--r--   0 louisr     (501) staff       (20)     2046 2023-07-21 10:34:07.000000 pyrfu-2.4.4/pyrfu/pyrf/optimize_nbins_1d.py
--rw-r--r--   0 louisr     (501) staff       (20)     2746 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/optimize_nbins_2d.py
--rw-r--r--   0 louisr     (501) staff       (20)     3593 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/pid_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     1219 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/plasma_beta.py
--rw-r--r--   0 louisr     (501) staff       (20)     7424 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/plasma_calc.py
--rw-r--r--   0 louisr     (501) staff       (20)     2766 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/poynting_flux.py
--rw-r--r--   0 louisr     (501) staff       (20)     1897 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/pres_anis.py
--rw-r--r--   0 louisr     (501) staff       (20)     2958 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/psd.py
--rw-r--r--   0 louisr     (501) staff       (20)     1293 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/pvi.py
--rw-r--r--   0 louisr     (501) staff       (20)     2494 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/pvi_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     1223 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/read_cdf.py
--rw-r--r--   0 louisr     (501) staff       (20)     2017 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/remove_repeated_points.py
--rw-r--r--   0 louisr     (501) staff       (20)     8816 2023-07-21 12:05:30.000000 pyrfu-2.4.4/pyrfu/pyrf/resample.py
--rw-r--r--   0 louisr     (501) staff       (20)      697 2023-06-07 15:24:32.000000 pyrfu-2.4.4/pyrfu/pyrf/shock_models_parameters.json
--rw-r--r--   0 louisr     (501) staff       (20)    15200 2023-07-21 12:11:34.000000 pyrfu-2.4.4/pyrfu/pyrf/shock_normal.py
--rw-r--r--   0 louisr     (501) staff       (20)     9264 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/shock_parameters.py
--rw-r--r--   0 louisr     (501) staff       (20)     1651 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/solid_angle.py
--rw-r--r--   0 louisr     (501) staff       (20)      910 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/sph2cart.py
--rw-r--r--   0 louisr     (501) staff       (20)     2961 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/st_diff.py
--rw-r--r--   0 louisr     (501) staff       (20)      794 2023-07-22 21:11:20.000000 pyrfu-2.4.4/pyrfu/pyrf/start.py
--rw-r--r--   0 louisr     (501) staff       (20)     1857 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/struct_func.py
--rw-r--r--   0 louisr     (501) staff       (20)     1094 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/t_eval.py
--rw-r--r--   0 louisr     (501) staff       (20)     3716 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/time_clip.py
--rw-r--r--   0 louisr     (501) staff       (20)     1163 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/timevec2iso8601.py
--rw-r--r--   0 louisr     (501) staff       (20)    10280 2023-06-20 16:59:32.000000 pyrfu-2.4.4/pyrfu/pyrf/timing_gui.py
--rw-r--r--   0 louisr     (501) staff       (20)     1625 2023-07-22 21:23:02.000000 pyrfu-2.4.4/pyrfu/pyrf/trace.py
--rw-r--r--   0 louisr     (501) staff       (20)      688 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/pyrf/transformation_indices.json
--rw-r--r--   0 louisr     (501) staff       (20)     2422 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/ts_append.py
--rw-r--r--   0 louisr     (501) staff       (20)     1224 2023-07-21 17:28:19.000000 pyrfu-2.4.4/pyrfu/pyrf/ts_scalar.py
--rw-r--r--   0 louisr     (501) staff       (20)     3943 2023-07-22 20:48:02.000000 pyrfu-2.4.4/pyrfu/pyrf/ts_skymap.py
--rw-r--r--   0 louisr     (501) staff       (20)     1320 2023-07-21 17:28:19.000000 pyrfu-2.4.4/pyrfu/pyrf/ts_tensor_xyz.py
--rw-r--r--   0 louisr     (501) staff       (20)      672 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/ts_time.py
--rw-r--r--   0 louisr     (501) staff       (20)     1279 2023-07-21 17:28:19.000000 pyrfu-2.4.4/pyrfu/pyrf/ts_vec_xyz.py
--rw-r--r--   0 louisr     (501) staff       (20)      928 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/ttns2datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)      718 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/unix2datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)     3658 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/vht.py
--rw-r--r--   0 louisr     (501) staff       (20)     1683 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/wave_fft.py
--rw-r--r--   0 louisr     (501) staff       (20)     6301 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/wavelet.py
--rw-r--r--   0 louisr     (501) staff       (20)    14548 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/wavepolarize_means.py
--rw-r--r--   0 louisr     (501) staff       (20)     2375 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/pyrf/waverage.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.531292 pyrfu-2.4.4/pyrfu/solo/
--rw-r--r--   0 louisr     (501) staff       (20)      373 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/solo/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)       48 2023-04-20 14:38:39.000000 pyrfu-2.4.4/pyrfu/solo/config.json
--rw-r--r--   0 louisr     (501) staff       (20)     1109 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/solo/db_init.py
--rw-r--r--   0 louisr     (501) staff       (20)     4619 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/solo/read_lfr_density.py
--rw-r--r--   0 louisr     (501) staff       (20)     8224 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/solo/read_tnr.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.534360 pyrfu-2.4.4/pyrfu/tests/
--rw-r--r--   0 louisr     (501) staff       (20)      210 2023-06-10 21:13:04.000000 pyrfu-2.4.4/pyrfu/tests/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)    21319 2023-07-22 21:43:35.000000 pyrfu-2.4.4/pyrfu/tests/test_pyrf.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.684740 pyrfu-2.4.4/pyrfu.egg-info/
--rw-r--r--   0 louisr     (501) staff       (20)     8802 2023-07-27 14:08:25.000000 pyrfu-2.4.4/pyrfu.egg-info/PKG-INFO
--rw-r--r--   0 louisr     (501) staff       (20)     8434 2023-07-27 14:08:26.000000 pyrfu-2.4.4/pyrfu.egg-info/SOURCES.txt
--rw-r--r--   0 louisr     (501) staff       (20)        1 2023-07-27 14:08:25.000000 pyrfu-2.4.4/pyrfu.egg-info/dependency_links.txt
--rw-r--r--   0 louisr     (501) staff       (20)      193 2023-07-27 14:08:25.000000 pyrfu-2.4.4/pyrfu.egg-info/requires.txt
--rw-r--r--   0 louisr     (501) staff       (20)       27 2023-07-27 14:08:25.000000 pyrfu-2.4.4/pyrfu.egg-info/top_level.txt
--rw-r--r--   0 louisr     (501) staff       (20)     1557 2023-07-21 11:26:29.000000 pyrfu-2.4.4/requirements.txt
--rw-r--r--   0 louisr     (501) staff       (20)       38 2023-07-27 14:08:27.539491 pyrfu-2.4.4/setup.cfg
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:26.634536 pyrfu-2.4.4/venv/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-07-27 14:08:27.536132 pyrfu-2.4.4/venv/bin/
--rw-r--r--   0 louisr     (501) staff       (20)     1175 2023-06-09 14:34:14.000000 pyrfu-2.4.4/venv/bin/activate_this.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.175972 pyrfu-2.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-01 09:02:28.000000 pyrfu-2.4.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-08-01 09:02:28.000000 pyrfu-2.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-08-01 09:02:49.175972 pyrfu-2.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-08-01 09:02:28.000000 pyrfu-2.4.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.075971 pyrfu-2.4.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-08-01 09:02:28.000000 pyrfu-2.4.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.079971 pyrfu-2.4.5/pyrfu/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.079971 pyrfu-2.4.5/pyrfu/dispersion/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/dispersion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/dispersion/disp_surf_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/dispersion/one_fluid_dispersion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.083971 pyrfu-2.4.5/pyrfu/lp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/lp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/lp/photo_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/lp/thermal_current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.123971 pyrfu-2.4.5/pyrfu/mms/
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/ancillary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/calculate_epsilon.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/copy_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/copy_files_ancillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/correct_edp_probe_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/db_get_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/db_get_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/db_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/def2psd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/dft_time_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/download_ancillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/download_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/dpf2psd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/dsl2gse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/dsl2gsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_ang_ang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_combine_proton_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_combine_proton_skymap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_combine_proton_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_omni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_pad_combine_sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_pad_spinavg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_proton_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_skymap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_skymap_combine_sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_spec_combine_sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/eis_spin_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/estimate_phase_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_active_eyes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_bad_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_correct_energies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_energy_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_flat_field_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_omni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_pad_spinavg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_pitch_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_remove_bad_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_remove_sun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_sector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_spin_avg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/feeps_split_integral_ch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/fft_bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11773 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/fk_power_spectrum_4sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_eis_allt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_feeps_alleyes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_feeps_omni.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_hpca_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_pitch_angle_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/get_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/hpca_calc_anodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/hpca_energies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/hpca_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/hpca_spin_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/lh_wave_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/list_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/list_files_ancillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/load_ancillary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/load_brst_segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/make_model_kappa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/make_model_rq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/make_model_vdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/mms_keys.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/probe_align_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/psd2def.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/psd2dpf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18460 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/psd_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/psd_rebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/read_feeps_sector_masks_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/remove_edist_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/remove_idist_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/remove_imoms_background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/rotate_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/scpot2ne.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/spectr_to_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.131971 pyrfu-2.4.5/pyrfu/mms/sun/
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/vdf_elim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/vdf_omni.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/vdf_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/vdf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/vdf_to_e64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/mms/whistler_b2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.135971 pyrfu-2.4.5/pyrfu/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/models/igrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26798 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/models/igrf13coeffs.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/models/magnetopause_normal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.143972 pyrfu-2.4.5/pyrfu/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/add_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/annotate_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/colorbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.143972 pyrfu-2.4.5/pyrfu/plot/logo/
+-rw-r--r--   0 runner    (1001) docker     (123)    43962 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/make_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/mms_pl_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/pl_scatter_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/pl_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_ang_ang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_clines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_magnetosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_reduced_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_sitl_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_spectr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/plot_surf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/span_tint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/plot/zoom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.171972 pyrfu-2.4.5/pyrfu/pyrf/
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/autocorr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/average_vdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/avg_4sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/c_4_grad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/c_4_j.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/c_4_k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/c_4_v.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/calc_ag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/calc_agyro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/calc_dng.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/calc_dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/calc_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/calc_sqrtq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/cart2sph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/cart2sph_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/cdfepoch2datetime64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/compress_cwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/convert_fac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/corr_deriv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/cotrans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/date_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/datetime2iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/datetime642iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/datetime642ttns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/datetime642unix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/dec_par_perp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/dist_append.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/dynamic_press.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/e_vxb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/eb_nrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36446 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ebsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/edb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/end.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/extend_tint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/filt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/find_closest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/get_omni_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/gse2gsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/histogram2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/increments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/int_sph_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/iplasma_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/iso2unix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/iso86012datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/iso86012datetime64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/iso86012timevec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/l_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/lowpass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/magnetosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/match_phibe_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/match_phibe_v.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/mean_bins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/mean_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/medfilt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/median_bins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/movmean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/mva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/mva_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/new_xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/optimize_nbins_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/optimize_nbins_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/pid_4sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/plasma_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/plasma_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/poynting_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/pres_anis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/psd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/pvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/pvi_4sc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/read_cdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/remove_repeated_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/shock_models_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15066 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/shock_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/shock_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/solid_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/sph2cart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/st_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/struct_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/t_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/time_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/timevec2iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/transformation_indices.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ts_append.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ts_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ts_skymap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ts_tensor_xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ts_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ts_vec_xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/ttns2datetime64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/unix2datetime64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/vht.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/wave_fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/wavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14548 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/wavepolarize_means.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/pyrf/waverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.171972 pyrfu-2.4.5/pyrfu/solo/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/solo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/solo/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/solo/db_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/solo/read_lfr_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/solo/read_tnr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.175972 pyrfu-2.4.5/pyrfu/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/tests/test_dispersion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35819 2023-08-01 09:02:28.000000 pyrfu-2.4.5/pyrfu/tests/test_pyrf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 09:02:49.079971 pyrfu-2.4.5/pyrfu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-08-01 09:02:49.000000 pyrfu-2.4.5/pyrfu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-08-01 09:02:49.000000 pyrfu-2.4.5/pyrfu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 09:02:49.000000 pyrfu-2.4.5/pyrfu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-01 09:02:49.000000 pyrfu-2.4.5/pyrfu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 09:02:49.000000 pyrfu-2.4.5/pyrfu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 09:02:49.175972 pyrfu-2.4.5/setup.cfg
```

### Comparing `pyrfu-2.4.4/LICENSE.txt` & `pyrfu-2.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/PKG-INFO` & `pyrfu-2.4.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfu
-Version: 2.4.4
+Version: 2.4.5
 Summary: Python Space Physics (RymdFysik) Utilities
 Author-email: Louis RICHARD <louir@irfu.se>
 License: 
         MIT License
         
         Copyright (c) 2020 L. RICHARD
         
@@ -37,15 +37,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: Microsoft :: MS-DOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -76,16 +75,16 @@
 
 .. |Status| image:: https://img.shields.io/pypi/status/pyrfu?logo=pypi&color=blue
 .. _Status: https://pypi.org/project/pyrfu/
 
 .. |Downloads| image:: https://img.shields.io/pypi/dm/pyrfu?logo=pypi&color=blue
 .. _Downloads: https://pypi.org/project/pyrfu/
 
-.. |Flake8| image:: https://github.com/louis-richard/irfu-python/actions/workflows/flake8.yml/badge.svg
-.. _Flake8: https://github.com/louis-richard/irfu-python/actions/workflows/flake8.yml
+.. |CI| image:: https://github.com/louis-richard/irfu-python/actions/workflows/tests.yml/badge.svg
+.. _CI: https://github.com/louis-richard/irfu-python/actions/workflows/tests.yml
 
 .. |PyLintB| image:: https://github.com/louis-richard/irfu-python/actions/workflows/pylint.yml/badge.svg
 .. _PyLintB: https://github.com/louis-richard/irfu-python/actions/workflows/pylint.yml
 
 .. |Issues| image:: https://img.shields.io/github/issues/louis-richard/irfu-python?logo=github&color=9cf
 .. _Issues: https://github.com/louis-richard/irfu-python/issues
 
@@ -97,176 +96,100 @@
 
 .. |Gitter| image:: https://img.shields.io/gitter/room/louis-richard/pyrfu?logo=gitter&color=orange
 .. _Gitter: https://gitter.im/pyrfu
 
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
 .. _Black: https://github.com/psf/black
 
-|License|_ |Python|_ |PyPi|_ |Format|_ |Wheel|_ |Status|_ |Downloads|_ |Flake8|_ |PyLintB|_ |Issues|_ |Commits|_ |Readthedocs|_ |Gitter|_ |Black|_
+|License|_ |Python|_ |PyPi|_ |Format|_ |Wheel|_ |Status|_ |Downloads|_ |CI|_
+|PyLintB|_ |Issues|_ |Commits|_ |Readthedocs|_ |Gitter|_ |Black|_
 
 The Python package ``pyrfu`` is a software based on the IRFU-MATLAB library to work with space data, particularly the
 Magnetospheric MultiScale (MMS) mission.
 
 It is distributed under the open-source MIT license.
 
 .. end-marker-intro-do-not-remove
 
 Full documentation can be found `here <https://pyrfu.readthedocs.io>`_
 
 
-Installation
-------------
-.. start-marker-install-do-not-remove
+Quickstart
+==========
 
-The package ``pyrfu`` has been tested only for Mac OS.
+Installing pyrfu with pip (`more details here`_):
 
-Using PyPi
-**********
+.. _more details here: https://pyrfu.readthedocs.io/en/latest/installation.html
 
-``pyrfu`` is available for pip.
+.. code-block:: console
 
-.. code-block:: bash
+    $ python -m pip install pyrfu
+    # or
+    $ python -m pip install --user pyrfu
 
-        pip install pyrfu
+Import `pyrfu.mms`_ package with routines specific to work with the
+Magnetospheric Multiscale mission (MMS)
 
+.. _pyrfu.mms: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.mms.html
 
-From sources
-************
-
-The sources are located on **GitHub**:
-
-    https://github.com/louis-richard/irfu-python
-
-1) Clone the GitHub repo:
-
-Open a terminal and write the below command to clone in your PC the ``pyrfu`` repo:
-
-.. code-block:: bash
-
-    git clone https://github.com/louis-richard/irfu-python.git
-    cd irfu-python
-
-
-2) Create a virtual env
-
-pyrfu needs a significant number of dependencies. The easiest
-way to get everything installed is to use a virtual environment.
-
--  Anaconda
-
-You can create a virtual environment and install all the dependencies using conda_
-with the following commands:
-
-.. code-block:: bash
-
-    pip install conda
-    conda create -n pyrfu
-    source activate pyrfu
-
-.. _conda: http://conda.io/
-
-
-- Virtual Env
-
-Virtualenv_ can also be used:
-
-.. code-block:: bash
-
-    pip install virtualenv
-    virtualenv pyrfu
-    source pyrfu/bin/activate
-
-.. _virtualenv: https://virtualenv.pypa.io/en/latest/#
-
-
-3) Install the package via the commands:
-
-.. code-block:: bash
-
-        python setup.py install
-
-
-5) (Optional) Generate the docs: install the extra dependencies of doc and run
-the `setup.py` file:
-
-.. code-block:: bash
-
-        pip install pyrfu
-        python setup.py build_sphinx
-
-Once installed, the doc can be generated with:
-
-.. code-block:: bash
-
-        cd doc
-        make html
-
-
-Dependencies
-************
+.. code:: python
 
-The required dependencies are:
+    from pyrfu import mms
 
-- `cdflib <https://cdflib.readthedocs.io/en/latest/?badge=latest>`_ >=1.0.0
-- `geopack <https://github.com/tsssss/geopack>`_ >=1.0.9
-- `matplotlib <https://matplotlib.org>`_ >=3.5.2
-- `numba <http://numba.pydata.org>`_ >=0.54.1
-- `numpy <https://www.numpy.org>`_ >=1.20.3
-- `pandas <https://pandas.pydata.org/>`_ >=1.3.4
-- `python-datetutil <https://dateutil.readthedocs.io/en/stable/>`_ >=2.8.2
-- `requests <https://requests.readthedocs.io/en/latest/>`_ >=2.26.0
-- `scipy <https://scipy.org>`_ >=1.7.3
-- `tqdm <https://tqdm.github.io/>`_ >=4.62.3
-- `xarray <https://xarray.pydata.org/en/stable/>`_ >=0.20.1
+Setup path to MMS data
 
+.. code:: python
 
-Testing dependencies are:
+    mms.db_init("/Volumes/mms")
 
-- `pytest <https://docs.pytest.org/en/latest/>`_ >= 2.8
+Load magnetic field and ion bulk velocity data
 
-Extra testing dependencies:
+.. code:: python
 
-- `coverage <https://coverage.readthedocs.io>`_ >= 4.4
-- `pylint <https://www.pylint.org>`_ >= 1.6.0
+    tint = ["2019-09-14T07:54:00.000", "2019-09-14T08:11:00.000"]
+    b_gsm = mms.get_data("b_gsm_fgm_srvy_l2", tint, 1)
+    v_gse_i = mms.get_data("vi_gse_fpi_fast_l2", tint, 1)
 
-.. end-marker-install-do-not-remove
+Import `pyrfu.pyrf`_ package with generic routines
 
-Usage
------
-To import generic space plasma physics functions
+.. _pyrfu.pyrf: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.pyrf.html
 
 .. code:: python
 
     from pyrfu import pyrf
 
-
-To import functions specific to Magnetospheric Multi-Scale (MMS)
+Transform ion bulk velocity to geocentric solar magnetospheric (GSM) coordinates
 
 .. code:: python
 
-    from pyrfu import mms
+    v_gsm_i = pyrf.cotrans(v_gse_i, "gse>gsm")
 
+Import `pyrfu.plot`_ package with plotting routines
 
-To import functions specific to Solar Orbiter (SolO)
+.. _pyrfu.plot: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.plot.html
 
 .. code:: python
 
-    from pyrfu import solo
-
+    from pyrfu import plot
 
-To import plotting functions
+Plot time series of magnetic field and ion bulk velocity
 
 .. code:: python
 
-    from pyrfu import plot
+    import matplotlib.pyplot as plt
 
+    f, axs = plt.subplots(2, sharex="all")
+    plot.plot_line(axs[0], b_gsm)
+    axs[0].set_ylabel("$B~[\\mathrm{nT}]$")
+    axs[0].legend(["$B_{x}$", "$B_{y}$", "$B_{z}$"], ncol=4)
+
+    plot.plot_line(axs[1], v_gsm_i)
+    axs[1].set_ylabel("$V_i~[\\mathrm{km}~\\mathrm{s}^{-1}]$")
+    axs[1].legend(["$V_{ix}$", "$V_{iy}$", "$V_{iz}$"], ncol=4)
 
-Configuration
--------------
-Default configuration settings for MMS data (i.e data path) are stored in pyrfu/mms/config.json and can be changed at anytime using mms.db_init(local_path_dir).
 
 Credits
 -------
 This software was developed by Louis RICHARD (louisr@irfu.se) based on the IRFU-MATLAB library.
 
 Acknowledgement
 ---------------
```

### Comparing `pyrfu-2.4.4/README.rst` & `pyrfu-2.4.5/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 .. |Status| image:: https://img.shields.io/pypi/status/pyrfu?logo=pypi&color=blue
 .. _Status: https://pypi.org/project/pyrfu/
 
 .. |Downloads| image:: https://img.shields.io/pypi/dm/pyrfu?logo=pypi&color=blue
 .. _Downloads: https://pypi.org/project/pyrfu/
 
-.. |Flake8| image:: https://github.com/louis-richard/irfu-python/actions/workflows/flake8.yml/badge.svg
-.. _Flake8: https://github.com/louis-richard/irfu-python/actions/workflows/flake8.yml
+.. |CI| image:: https://github.com/louis-richard/irfu-python/actions/workflows/tests.yml/badge.svg
+.. _CI: https://github.com/louis-richard/irfu-python/actions/workflows/tests.yml
 
 .. |PyLintB| image:: https://github.com/louis-richard/irfu-python/actions/workflows/pylint.yml/badge.svg
 .. _PyLintB: https://github.com/louis-richard/irfu-python/actions/workflows/pylint.yml
 
 .. |Issues| image:: https://img.shields.io/github/issues/louis-richard/irfu-python?logo=github&color=9cf
 .. _Issues: https://github.com/louis-richard/irfu-python/issues
 
@@ -43,176 +43,100 @@
 
 .. |Gitter| image:: https://img.shields.io/gitter/room/louis-richard/pyrfu?logo=gitter&color=orange
 .. _Gitter: https://gitter.im/pyrfu
 
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
 .. _Black: https://github.com/psf/black
 
-|License|_ |Python|_ |PyPi|_ |Format|_ |Wheel|_ |Status|_ |Downloads|_ |Flake8|_ |PyLintB|_ |Issues|_ |Commits|_ |Readthedocs|_ |Gitter|_ |Black|_
+|License|_ |Python|_ |PyPi|_ |Format|_ |Wheel|_ |Status|_ |Downloads|_ |CI|_
+|PyLintB|_ |Issues|_ |Commits|_ |Readthedocs|_ |Gitter|_ |Black|_
 
 The Python package ``pyrfu`` is a software based on the IRFU-MATLAB library to work with space data, particularly the
 Magnetospheric MultiScale (MMS) mission.
 
 It is distributed under the open-source MIT license.
 
 .. end-marker-intro-do-not-remove
 
 Full documentation can be found `here <https://pyrfu.readthedocs.io>`_
 
 
-Installation
-------------
-.. start-marker-install-do-not-remove
+Quickstart
+==========
 
-The package ``pyrfu`` has been tested only for Mac OS.
+Installing pyrfu with pip (`more details here`_):
 
-Using PyPi
-**********
+.. _more details here: https://pyrfu.readthedocs.io/en/latest/installation.html
 
-``pyrfu`` is available for pip.
+.. code-block:: console
 
-.. code-block:: bash
+    $ python -m pip install pyrfu
+    # or
+    $ python -m pip install --user pyrfu
 
-        pip install pyrfu
+Import `pyrfu.mms`_ package with routines specific to work with the
+Magnetospheric Multiscale mission (MMS)
 
+.. _pyrfu.mms: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.mms.html
 
-From sources
-************
-
-The sources are located on **GitHub**:
-
-    https://github.com/louis-richard/irfu-python
-
-1) Clone the GitHub repo:
-
-Open a terminal and write the below command to clone in your PC the ``pyrfu`` repo:
-
-.. code-block:: bash
-
-    git clone https://github.com/louis-richard/irfu-python.git
-    cd irfu-python
-
-
-2) Create a virtual env
-
-pyrfu needs a significant number of dependencies. The easiest
-way to get everything installed is to use a virtual environment.
-
--  Anaconda
-
-You can create a virtual environment and install all the dependencies using conda_
-with the following commands:
-
-.. code-block:: bash
-
-    pip install conda
-    conda create -n pyrfu
-    source activate pyrfu
-
-.. _conda: http://conda.io/
-
-
-- Virtual Env
-
-Virtualenv_ can also be used:
-
-.. code-block:: bash
-
-    pip install virtualenv
-    virtualenv pyrfu
-    source pyrfu/bin/activate
-
-.. _virtualenv: https://virtualenv.pypa.io/en/latest/#
-
-
-3) Install the package via the commands:
-
-.. code-block:: bash
-
-        python setup.py install
-
-
-5) (Optional) Generate the docs: install the extra dependencies of doc and run
-the `setup.py` file:
-
-.. code-block:: bash
-
-        pip install pyrfu
-        python setup.py build_sphinx
-
-Once installed, the doc can be generated with:
-
-.. code-block:: bash
-
-        cd doc
-        make html
-
-
-Dependencies
-************
+.. code:: python
 
-The required dependencies are:
+    from pyrfu import mms
 
-- `cdflib <https://cdflib.readthedocs.io/en/latest/?badge=latest>`_ >=1.0.0
-- `geopack <https://github.com/tsssss/geopack>`_ >=1.0.9
-- `matplotlib <https://matplotlib.org>`_ >=3.5.2
-- `numba <http://numba.pydata.org>`_ >=0.54.1
-- `numpy <https://www.numpy.org>`_ >=1.20.3
-- `pandas <https://pandas.pydata.org/>`_ >=1.3.4
-- `python-datetutil <https://dateutil.readthedocs.io/en/stable/>`_ >=2.8.2
-- `requests <https://requests.readthedocs.io/en/latest/>`_ >=2.26.0
-- `scipy <https://scipy.org>`_ >=1.7.3
-- `tqdm <https://tqdm.github.io/>`_ >=4.62.3
-- `xarray <https://xarray.pydata.org/en/stable/>`_ >=0.20.1
+Setup path to MMS data
 
+.. code:: python
 
-Testing dependencies are:
+    mms.db_init("/Volumes/mms")
 
-- `pytest <https://docs.pytest.org/en/latest/>`_ >= 2.8
+Load magnetic field and ion bulk velocity data
 
-Extra testing dependencies:
+.. code:: python
 
-- `coverage <https://coverage.readthedocs.io>`_ >= 4.4
-- `pylint <https://www.pylint.org>`_ >= 1.6.0
+    tint = ["2019-09-14T07:54:00.000", "2019-09-14T08:11:00.000"]
+    b_gsm = mms.get_data("b_gsm_fgm_srvy_l2", tint, 1)
+    v_gse_i = mms.get_data("vi_gse_fpi_fast_l2", tint, 1)
 
-.. end-marker-install-do-not-remove
+Import `pyrfu.pyrf`_ package with generic routines
 
-Usage
------
-To import generic space plasma physics functions
+.. _pyrfu.pyrf: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.pyrf.html
 
 .. code:: python
 
     from pyrfu import pyrf
 
-
-To import functions specific to Magnetospheric Multi-Scale (MMS)
+Transform ion bulk velocity to geocentric solar magnetospheric (GSM) coordinates
 
 .. code:: python
 
-    from pyrfu import mms
+    v_gsm_i = pyrf.cotrans(v_gse_i, "gse>gsm")
 
+Import `pyrfu.plot`_ package with plotting routines
 
-To import functions specific to Solar Orbiter (SolO)
+.. _pyrfu.plot: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.plot.html
 
 .. code:: python
 
-    from pyrfu import solo
-
+    from pyrfu import plot
 
-To import plotting functions
+Plot time series of magnetic field and ion bulk velocity
 
 .. code:: python
 
-    from pyrfu import plot
+    import matplotlib.pyplot as plt
 
+    f, axs = plt.subplots(2, sharex="all")
+    plot.plot_line(axs[0], b_gsm)
+    axs[0].set_ylabel("$B~[\\mathrm{nT}]$")
+    axs[0].legend(["$B_{x}$", "$B_{y}$", "$B_{z}$"], ncol=4)
+
+    plot.plot_line(axs[1], v_gsm_i)
+    axs[1].set_ylabel("$V_i~[\\mathrm{km}~\\mathrm{s}^{-1}]$")
+    axs[1].legend(["$V_{ix}$", "$V_{iy}$", "$V_{iz}$"], ncol=4)
 
-Configuration
--------------
-Default configuration settings for MMS data (i.e data path) are stored in pyrfu/mms/config.json and can be changed at anytime using mms.db_init(local_path_dir).
 
 Credits
 -------
 This software was developed by Louis RICHARD (louisr@irfu.se) based on the IRFU-MATLAB library.
 
 Acknowledgement
 ---------------
```

### Comparing `pyrfu-2.4.4/docs/conf.py` & `pyrfu-2.4.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyproject.toml` & `pyrfu-2.4.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel==0.38.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrfu"
-version = "2.4.4"
+version = "2.4.5"
 description = "Python Space Physics (RymdFysik) Utilities"
 readme = "README.rst"
 authors = [{ name = "Louis RICHARD", email = "louir@irfu.se" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Other Environment",
@@ -22,15 +22,14 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft",
     "Operating System :: Microsoft :: MS-DOS",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 dependencies = [
@@ -106,20 +105,21 @@
 ignore = """
     ancillary.json,
     config.json,
     feeps_bad_data.json,
     igrf13coeffs.csv,
     mms_keys.json,
     transformation_indices.json,
-    test_pyrf.py
+    test_pyrf.py,
+    test_dispersion.py
 """
 ignored-modules = "scipy,cdflib"
 
 [tool.bumpver]
-current_version = "2.4.4"
+current_version = "2.4.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `pyrfu-2.4.4/pyrfu/dispersion/disp_surf_calc.py` & `pyrfu-2.4.5/pyrfu/dispersion/disp_surf_calc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/dispersion/one_fluid_dispersion.py` & `pyrfu-2.4.5/pyrfu/dispersion/one_fluid_dispersion.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/lp/__init__.py` & `pyrfu-2.4.5/pyrfu/lp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/lp/photo_current.py` & `pyrfu-2.4.5/pyrfu/lp/photo_current.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/lp/thermal_current.py` & `pyrfu-2.4.5/pyrfu/lp/thermal_current.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/__init__.py` & `pyrfu-2.4.5/pyrfu/mms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/ancillary.json` & `pyrfu-2.4.5/pyrfu/mms/ancillary.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/calculate_epsilon.py` & `pyrfu-2.4.5/pyrfu/mms/calculate_epsilon.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/copy_files.py` & `pyrfu-2.4.5/pyrfu/mms/copy_files.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/copy_files_ancillary.py` & `pyrfu-2.4.5/pyrfu/mms/copy_files_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/correct_edp_probe_timing.py` & `pyrfu-2.4.5/pyrfu/mms/correct_edp_probe_timing.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/db_get_ts.py` & `pyrfu-2.4.5/pyrfu/mms/db_get_ts.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/db_get_variable.py` & `pyrfu-2.4.5/pyrfu/mms/db_get_variable.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/db_init.py` & `pyrfu-2.4.5/pyrfu/mms/db_init.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/def2psd.py` & `pyrfu-2.4.5/pyrfu/mms/def2psd.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/dft_time_shift.py` & `pyrfu-2.4.5/pyrfu/mms/dft_time_shift.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/download_ancillary.py` & `pyrfu-2.4.5/pyrfu/mms/download_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/download_data.py` & `pyrfu-2.4.5/pyrfu/mms/download_data.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/dpf2psd.py` & `pyrfu-2.4.5/pyrfu/mms/dpf2psd.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/dsl2gse.py` & `pyrfu-2.4.5/pyrfu/mms/dsl2gse.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/dsl2gsm.py` & `pyrfu-2.4.5/pyrfu/mms/dsl2gsm.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_ang_ang.py` & `pyrfu-2.4.5/pyrfu/mms/eis_ang_ang.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_combine_proton_pad.py` & `pyrfu-2.4.5/pyrfu/mms/eis_combine_proton_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_combine_proton_skymap.py` & `pyrfu-2.4.5/pyrfu/mms/eis_combine_proton_skymap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_combine_proton_spec.py` & `pyrfu-2.4.5/pyrfu/mms/eis_combine_proton_spec.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_moments.py` & `pyrfu-2.4.5/pyrfu/mms/eis_moments.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_omni.py` & `pyrfu-2.4.5/pyrfu/mms/eis_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_pad.py` & `pyrfu-2.4.5/pyrfu/mms/eis_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_pad_combine_sc.py` & `pyrfu-2.4.5/pyrfu/mms/eis_pad_combine_sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_pad_spinavg.py` & `pyrfu-2.4.5/pyrfu/mms/eis_pad_spinavg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_proton_correction.py` & `pyrfu-2.4.5/pyrfu/mms/eis_proton_correction.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_skymap.py` & `pyrfu-2.4.5/pyrfu/mms/eis_skymap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_skymap_combine_sc.py` & `pyrfu-2.4.5/pyrfu/mms/eis_skymap_combine_sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_spec_combine_sc.py` & `pyrfu-2.4.5/pyrfu/mms/eis_spec_combine_sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/eis_spin_avg.py` & `pyrfu-2.4.5/pyrfu/mms/eis_spin_avg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/estimate_phase_speed.py` & `pyrfu-2.4.5/pyrfu/mms/estimate_phase_speed.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_active_eyes.py` & `pyrfu-2.4.5/pyrfu/mms/feeps_active_eyes.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_bad_data.json` & `pyrfu-2.4.5/pyrfu/mms/feeps_bad_data.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_correct_energies.py` & `pyrfu-2.4.5/pyrfu/mms/feeps_correct_energies.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_energy_table.py` & `pyrfu-2.4.5/pyrfu/mms/feeps_energy_table.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_flat_field_corrections.py` & `pyrfu-2.4.5/pyrfu/mms/feeps_flat_field_corrections.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_omni.py` & `pyrfu-2.4.5/pyrfu/mms/feeps_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_pad.py` & `pyrfu-2.4.5/pyrfu/mms/feeps_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_pad_spinavg.py` & `pyrfu-2.4.5/pyrfu/mms/feeps_pad_spinavg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_pitch_angles.py` & `pyrfu-2.4.5/pyrfu/mms/feeps_pitch_angles.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_remove_bad_data.py` & `pyrfu-2.4.5/pyrfu/mms/feeps_remove_bad_data.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_remove_sun.py` & `pyrfu-2.4.5/pyrfu/mms/feeps_remove_sun.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_sector_spec.py` & `pyrfu-2.4.5/pyrfu/mms/feeps_sector_spec.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_spin_avg.py` & `pyrfu-2.4.5/pyrfu/mms/feeps_spin_avg.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/feeps_split_integral_ch.py` & `pyrfu-2.4.5/pyrfu/mms/feeps_split_integral_ch.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/fft_bandpass.py` & `pyrfu-2.4.5/pyrfu/mms/fft_bandpass.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/fk_power_spectrum_4sc.py` & `pyrfu-2.4.5/pyrfu/mms/fk_power_spectrum_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/get_data.py` & `pyrfu-2.4.5/pyrfu/mms/get_data.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/get_dist.py` & `pyrfu-2.4.5/pyrfu/mms/get_dist.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/get_eis_allt.py` & `pyrfu-2.4.5/pyrfu/mms/get_eis_allt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/get_feeps_alleyes.py` & `pyrfu-2.4.5/pyrfu/mms/get_feeps_alleyes.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/get_feeps_omni.py` & `pyrfu-2.4.5/pyrfu/mms/get_feeps_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/get_hpca_dist.py` & `pyrfu-2.4.5/pyrfu/mms/get_hpca_dist.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/get_pitch_angle_dist.py` & `pyrfu-2.4.5/pyrfu/mms/get_pitch_angle_dist.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/get_ts.py` & `pyrfu-2.4.5/pyrfu/mms/get_ts.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/get_variable.py` & `pyrfu-2.4.5/pyrfu/mms/get_variable.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/hpca_calc_anodes.py` & `pyrfu-2.4.5/pyrfu/mms/hpca_calc_anodes.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/hpca_energies.py` & `pyrfu-2.4.5/pyrfu/mms/hpca_energies.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/hpca_pad.py` & `pyrfu-2.4.5/pyrfu/mms/hpca_pad.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/hpca_spin_sum.py` & `pyrfu-2.4.5/pyrfu/mms/hpca_spin_sum.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/lh_wave_analysis.py` & `pyrfu-2.4.5/pyrfu/mms/lh_wave_analysis.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/list_files.py` & `pyrfu-2.4.5/pyrfu/mms/list_files.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/list_files_ancillary.py` & `pyrfu-2.4.5/pyrfu/mms/list_files_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/load_ancillary.py` & `pyrfu-2.4.5/pyrfu/mms/load_ancillary.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/load_brst_segments.py` & `pyrfu-2.4.5/pyrfu/mms/load_brst_segments.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/make_model_kappa.py` & `pyrfu-2.4.5/pyrfu/mms/make_model_kappa.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/make_model_rq.py` & `pyrfu-2.4.5/pyrfu/mms/make_model_rq.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/make_model_vdf.py` & `pyrfu-2.4.5/pyrfu/mms/make_model_vdf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/mms_keys.json` & `pyrfu-2.4.5/pyrfu/mms/mms_keys.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/probe_align_times.py` & `pyrfu-2.4.5/pyrfu/mms/probe_align_times.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/psd2def.py` & `pyrfu-2.4.5/pyrfu/mms/psd2def.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/psd2dpf.py` & `pyrfu-2.4.5/pyrfu/mms/psd2dpf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/psd_moments.py` & `pyrfu-2.4.5/pyrfu/mms/psd_moments.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/psd_rebin.py` & `pyrfu-2.4.5/pyrfu/mms/psd_rebin.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/read_feeps_sector_masks_csv.py` & `pyrfu-2.4.5/pyrfu/mms/read_feeps_sector_masks_csv.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/reduce.py` & `pyrfu-2.4.5/pyrfu/mms/reduce.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/remove_edist_background.py` & `pyrfu-2.4.5/pyrfu/mms/remove_edist_background.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/remove_idist_background.py` & `pyrfu-2.4.5/pyrfu/mms/remove_idist_background.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/remove_imoms_background.py` & `pyrfu-2.4.5/pyrfu/mms/remove_imoms_background.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/rotate_tensor.py` & `pyrfu-2.4.5/pyrfu/mms/rotate_tensor.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/scpot2ne.py` & `pyrfu-2.4.5/pyrfu/mms/scpot2ne.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/spectr_to_dataset.py` & `pyrfu-2.4.5/pyrfu/mms/spectr_to_dataset.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/tokenize.py` & `pyrfu-2.4.5/pyrfu/mms/tokenize.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/vdf_elim.py` & `pyrfu-2.4.5/pyrfu/mms/vdf_elim.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/vdf_omni.py` & `pyrfu-2.4.5/pyrfu/mms/vdf_omni.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/vdf_projection.py` & `pyrfu-2.4.5/pyrfu/mms/vdf_projection.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/vdf_reduce.py` & `pyrfu-2.4.5/pyrfu/mms/vdf_reduce.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/vdf_to_e64.py` & `pyrfu-2.4.5/pyrfu/mms/vdf_to_e64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/mms/whistler_b2e.py` & `pyrfu-2.4.5/pyrfu/mms/whistler_b2e.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/models/igrf.py` & `pyrfu-2.4.5/pyrfu/models/igrf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/models/igrf13coeffs.csv` & `pyrfu-2.4.5/pyrfu/models/igrf13coeffs.csv`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/models/magnetopause_normal.py` & `pyrfu-2.4.5/pyrfu/models/magnetopause_normal.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/__init__.py` & `pyrfu-2.4.5/pyrfu/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/add_position.py` & `pyrfu-2.4.5/pyrfu/plot/add_position.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/annotate_heatmap.py` & `pyrfu-2.4.5/pyrfu/plot/annotate_heatmap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/colorbar.py` & `pyrfu-2.4.5/pyrfu/plot/colorbar.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg` & `pyrfu-2.4.5/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/make_labels.py` & `pyrfu-2.4.5/pyrfu/plot/make_labels.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/mms_pl_config.py` & `pyrfu-2.4.5/pyrfu/plot/mms_pl_config.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/pl_scatter_matrix.py` & `pyrfu-2.4.5/pyrfu/plot/pl_scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/pl_tx.py` & `pyrfu-2.4.5/pyrfu/plot/pl_tx.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/plot_ang_ang.py` & `pyrfu-2.4.5/pyrfu/plot/plot_ang_ang.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/plot_clines.py` & `pyrfu-2.4.5/pyrfu/plot/plot_clines.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/plot_heatmap.py` & `pyrfu-2.4.5/pyrfu/plot/plot_heatmap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/plot_line.py` & `pyrfu-2.4.5/pyrfu/plot/plot_line.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/plot_magnetosphere.py` & `pyrfu-2.4.5/pyrfu/plot/plot_magnetosphere.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/plot_projection.py` & `pyrfu-2.4.5/pyrfu/plot/plot_projection.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/plot_reduced_2d.py` & `pyrfu-2.4.5/pyrfu/plot/plot_reduced_2d.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/plot_sitl_overview.py` & `pyrfu-2.4.5/pyrfu/plot/plot_sitl_overview.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/plot_spectr.py` & `pyrfu-2.4.5/pyrfu/plot/plot_spectr.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/plot_surf.py` & `pyrfu-2.4.5/pyrfu/plot/plot_surf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/span_tint.py` & `pyrfu-2.4.5/pyrfu/plot/span_tint.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/plot/zoom.py` & `pyrfu-2.4.5/pyrfu/plot/zoom.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/__init__.py` & `pyrfu-2.4.5/pyrfu/pyrf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 from .mean import mean
 from .mean_bins import mean_bins
 from .mean_field import mean_field
 from .medfilt import medfilt
 from .median_bins import median_bins
 from .movmean import movmean
 from .mva import mva
+from .mva_gui import mva_gui
 from .new_xyz import new_xyz
 from .norm import norm
 from .normalize import normalize
 from .optimize_nbins_1d import optimize_nbins_1d
 from .optimize_nbins_2d import optimize_nbins_2d
 from .pid_4sc import pid_4sc
 from .plasma_calc import plasma_calc
@@ -174,14 +175,15 @@
     "mean",
     "mean_bins",
     "mean_field",
     "medfilt",
     "median_bins",
     "movmean",
     "mva",
+    "mva_gui",
     "new_xyz",
     "norm",
     "normalize",
     "optimize_nbins_1d",
     "optimize_nbins_2d",
     "pid_4sc",
     "plasma_beta",
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/autocorr.py` & `pyrfu-2.4.5/pyrfu/pyrf/autocorr.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/average_vdf.py` & `pyrfu-2.4.5/pyrfu/pyrf/average_vdf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
+import xarray as xr
 
 # Local imports
 from .ts_skymap import ts_skymap
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
@@ -28,17 +29,18 @@
     Returns
     -------
     vdf_avg : xarray.DataArray
         Time series of the time averaged velocity distribution function.
 
     """
 
-    assert n_pts % 2 != 0, "The number of distributions to be averaged must be an odd"
+    # Check input type
+    assert isinstance(vdf, xr.Dataset), "vdf must be a xarray.Dataset"
 
-    assert np.median(vdf.energy.data[0, :] - vdf.energy.data[0, :]) == 0
+    assert n_pts % 2 != 0, "The number of distributions to be averaged must be an odd"
 
     n_vdf = len(vdf.time.data)
     times = vdf.time.data
 
     pad_value = np.floor(n_pts / 2)
     avg_inds = np.arange(pad_value, n_vdf - pad_value, n_pts, dtype=int)
     time_avg = times[avg_inds]
@@ -65,16 +67,19 @@
 
     # Attributes
     glob_attrs = vdf.attrs  # Global attributes
     vdf_attrs = vdf.data.attrs  # VDF attributes
     coords_attrs = {k: vdf[k].attrs for k in ["time", "energy", "phi", "theta"]}
 
     # Get delta energy in global attributes for selected timestamps
-    glob_attrs["delta_energy_minus"] = glob_attrs["delta_energy_minus"][avg_inds]
-    glob_attrs["delta_energy_plus"] = glob_attrs["delta_energy_plus"][avg_inds]
+    if "delta_energy_minus" in glob_attrs:
+        glob_attrs["delta_energy_minus"] = glob_attrs["delta_energy_minus"][avg_inds, :]
+
+    if "delta_energy_plus" in glob_attrs:
+        glob_attrs["delta_energy_plus"] = glob_attrs["delta_energy_plus"][avg_inds, :]
 
     glob_attrs["esteptable"] = glob_attrs["esteptable"][: len(avg_inds)]
 
     vdf_avg = ts_skymap(
         time_avg,
         vdf_avg,
         energy_avg,
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/avg_4sc.py` & `pyrfu-2.4.5/pyrfu/pyrf/avg_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/c_4_grad.py` & `pyrfu-2.4.5/pyrfu/pyrf/c_4_grad.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,24 +32,21 @@
     elif len(out_data.shape) == 2:
         out = xr.DataArray(
             out_data,
             coords=[b_dict["1"].time, ["x", "y", "z"]],
             dims=["time", "comp"],
         )
 
-    elif len(out_data.shape) == 3:
+    else:
         out = xr.DataArray(
             out_data,
             coords=[b_dict["1"].time, ["x", "y", "z"], ["x", "y", "z"]],
             dims=["time", "vcomp", "hcomp"],
         )
 
-    else:
-        raise TypeError("Invalid type")
-
     return out
 
 
 def c_4_grad(r_list, b_list, method: str = "grad"):
     r"""Calculate gradient of physical field using 4 spacecraft technique
     in [2]_ [3]_.
 
@@ -103,14 +100,20 @@
 
     >>> b_mms = [get_data("B_gse_fgm_srvy_l2", tint, m) for m in range(1, 5)]
     >>> r_mms = [get_data("R_gse", tint, m) for m in range(1, 5)]
     >>> gradb = pyrf.c_4_grad(r_mms, b_mms, "grad")
 
     """
 
+    assert isinstance(r_list, list) and len(r_list) == 4, "r_list must a list of s/c"
+    assert isinstance(b_list, list) and len(b_list) == 4, "b_list must a list of s/c"
+
+    assert isinstance(method, str), "method must be a string"
+    assert method.lower() in ["grad", "div", "curl", "bdivb", "curv"], "Invalid method"
+
     # Resample with respect to 1st spacecraft
     r_list = [resample(r, b_list[0]) for r in r_list]
     b_list = [resample(b, b_list[0]) for b in b_list]
 
     # Compute reciprocal vectors in barycentric coordinates (see c_4_k)
     k_list = c_4_k(r_list)
 
@@ -157,18 +160,15 @@
     elif method.lower() == "bdivb":
         out_data = np.zeros(b_avg.shape)
 
         for i in range(3):
             out_data[:, i] = np.sum(b_avg.data * grad_b[:, i, :], axis=1)
 
     # Curvature
-    elif method.lower() == "curv":
+    else:
         b_hat_list = [normalize(b) for b in b_list]
 
         out_data = c_4_grad(r_list, b_hat_list, method="bdivb").data
 
-    else:
-        raise ValueError("Invalid method")
-
     out = _to_ts(out_data, b_dict)
 
     return out
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/c_4_j.py` & `pyrfu-2.4.5/pyrfu/pyrf/c_4_j.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,33 +103,34 @@
 
     Compute current density, divergence of b, etc. using curlometer technique
 
     >>> j_xyz, _, b_xyz, _, _, _ = pyrf.c_4_j(r_mms, b_mms)
 
     """
 
-    mu0 = constants.mu_0
+    assert isinstance(r_list, list) and len(r_list) == 4, "r_list must a list of s/c"
+    assert isinstance(b_list, list) and len(b_list) == 4, "b_list must a list of s/c"
 
     b_avg = 1e-9 * avg_4sc(b_list)
 
     # Estimate divB/mu0. unit is A/m2
     div_b = c_4_grad(r_list, b_list, "div")
 
     # to get right units
-    div_b *= 1.0e-3 * 1e-9 / mu0
+    div_b *= 1.0e-3 * 1e-9 / constants.mu_0
 
     # estimate current j [A/m2]
     j = c_4_grad(r_list, b_list, "curl")
-    j.data *= 1.0e-3 * 1e-9 / mu0
+    j.data *= 1.0e-3 * 1e-9 / constants.mu_0
 
     # estimate jxB force [T A/m2]
     jxb = cross(j, b_avg)
 
     # estimate divTshear = (1/muo) (B*div)B [T A/m2]
     div_t_shear = c_4_grad(r_list, b_list, "bdivb")
-    div_t_shear.data *= 1.0e-3 * 1e-9 * 1e-9 / mu0
+    div_t_shear.data *= 1.0e-3 * 1e-9 * 1e-9 / constants.mu_0
 
     # estimate divPb = (1/muo) grad (B^2/2) = divTshear-jxB
     div_pb = div_t_shear.copy()
     div_pb.data -= jxb.data
 
     return j, div_b, b_avg, jxb, div_t_shear, div_pb
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/c_4_k.py` & `pyrfu-2.4.5/pyrfu/pyrf/c_4_k.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/c_4_v.py` & `pyrfu-2.4.5/pyrfu/pyrf/c_4_v.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/calc_ag.py` & `pyrfu-2.4.5/pyrfu/pyrf/calc_ag.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/calc_agyro.py` & `pyrfu-2.4.5/pyrfu/pyrf/calc_agyro.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/calc_dng.py` & `pyrfu-2.4.5/pyrfu/pyrf/calc_dng.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/calc_dt.py` & `pyrfu-2.4.5/pyrfu/pyrf/calc_dt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/calc_fs.py` & `pyrfu-2.4.5/pyrfu/pyrf/calc_fs.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/calc_sqrtq.py` & `pyrfu-2.4.5/pyrfu/pyrf/calc_sqrtq.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/cart2sph.py` & `pyrfu-2.4.5/pyrfu/pyrf/cart2sph.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/cart2sph_ts.py` & `pyrfu-2.4.5/pyrfu/pyrf/cart2sph_ts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
+import xarray as xr
 
 # Local imports
 from .ts_vec_xyz import ts_vec_xyz
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
@@ -33,30 +34,36 @@
     Returns
     -------
     out : xarray.DataArray
         Input field in spherical/cartesian coordinate system.
 
     """
 
-    if inp.attrs["TENSOR_ORDER"] != 1 or inp.data.ndim != 2:
-        raise TypeError("Input must be vector field")
+    # Check input type
+    assert isinstance(inp, xr.DataArray), "inp must be a xarray.DataArray"
+
+    # Check that inp is a vector time series
+    assert inp.data.ndim == 2 and inp.shape[1] == 3, "inp must be a vector time series"
+
+    # Check direction +/-1
+    assert direction_flag in [-1, 1], "direction_flag must be +/-1"
 
     if direction_flag == -1:
         r_data = inp.data[:, 0]
 
         sin_the = np.sin(np.deg2rad(inp.data[:, 1]))
         cos_the = np.cos(np.deg2rad(inp.data[:, 1]))
         sin_phi = np.sin(np.deg2rad(inp.data[:, 2]))
         cos_phi = np.cos(np.deg2rad(inp.data[:, 2]))
 
         z_data = r_data * sin_the
         x_data = r_data * cos_the * cos_phi
         y_data = r_data * cos_the * sin_phi
 
-        out_data = np.hstack([x_data, y_data, z_data])
+        out_data = np.transpose(np.vstack([x_data, y_data, z_data]))
 
     else:
         xy2 = inp.data[:, 0] ** 2 + inp.data[:, 1] ** 2
 
         r_data = np.sqrt(xy2 + inp.data[:, 2] ** 2)
         theta = np.rad2deg(np.arctan2(inp.data[:, 2], np.sqrt(xy2)))
         phi = np.rad2deg(np.arctan2(inp.data[:, 1], inp.data[:, 0]))
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/cdfepoch2datetime64.py` & `pyrfu-2.4.5/pyrfu/pyrf/cdfepoch2datetime64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/compress_cwt.py` & `pyrfu-2.4.5/pyrfu/pyrf/compress_cwt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/convert_fac.py` & `pyrfu-2.4.5/pyrfu/pyrf/convert_fac.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,14 +68,18 @@
 
     Convert to field aligned coordinates
 
     >>> e_xyzfac = pyrf.convert_fac(e_xyz, b_xyz, numpy.array([1, 0, 0]))
 
     """
 
+    # Check input type
+    assert isinstance(inp, xr.DataArray), "inp must be a xarray.DataArray"
+    assert isinstance(b_bgd, xr.DataArray), "b_xyz must be a xarray.DataArray"
+
     assert r_xyz is None or isinstance(
         r_xyz,
         (xr.DataArray, list, np.ndarray),
     )
 
     if r_xyz is None:
         r_xyz = np.array([1, 0, 0])
@@ -96,32 +100,30 @@
 
     # Perpendicular
     r_perp_y = np.cross(b_hat, r_xyz, axis=1)
     r_perp_y /= np.linalg.norm(r_perp_y, axis=1, keepdims=True)
     r_perp_x = np.cross(r_perp_y, b_bgd, axis=1)
     r_perp_x /= np.linalg.norm(r_perp_x, axis=1, keepdims=True)
 
-    assert inp_data.shape[1] in [1, 3], "Invalid dimension of inp"
-
-    if inp_data.shape[1] == 3:
+    if inp_data.ndim == 2 and inp_data.shape[1] == 3:
         out_data = np.zeros(inp.shape)
 
         out_data[:, 0] = np.sum(r_perp_x * inp_data, axis=1)
         out_data[:, 1] = np.sum(r_perp_y * inp_data, axis=1)
         out_data[:, 2] = np.sum(b_hat * inp_data, axis=1)
 
-        # xarray
-        out = xr.DataArray(
-            out_data,
-            coords=[time, inp.comp],
-            dims=["time", "comp"],
-        )
+        # To xarray
+        out = ts_vec_xyz(time, out_data, attrs=inp.attrs)
 
-    else:
-        out_data = np.zeros([3, inp_data.shape[0]])
+    elif inp_data.ndim == 1:
+        out_data = np.zeros([inp_data.shape[0], 2])
 
-        out_data[:, 0] = inp[:, 0] * np.sum(r_perp_x * r_xyz, axis=1)
-        out_data[:, 1] = inp[:, 0] * np.sum(b_hat * r_xyz, axis=1)
+        out_data[:, 0] = inp * np.sum(r_perp_x * r_xyz, axis=1)
+        out_data[:, 1] = inp * np.sum(b_hat * r_xyz, axis=1)
 
-        out = ts_vec_xyz(time, out_data, attrs=inp.attrs)
+        out = xr.DataArray(
+            out_data, coords=[time, ["perp", "para"]], dims=["time", "comp"]
+        )
+    else:
+        raise TypeError("inp must be a vector or scalar")
 
     return out
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/corr_deriv.py` & `pyrfu-2.4.5/pyrfu/pyrf/corr_deriv.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/cotrans.py` & `pyrfu-2.4.5/pyrfu/pyrf/cotrans.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,30 +232,30 @@
 
     # J2000 reference time
     j2000 = 946727930.8160001
     # j2000 = Time("J2000", format="jyear_str").unix
 
     if isinstance(inp, xr.DataArray):
         time = inp.time.data
-        t = time.view("i8") * 1e-9
+        t = time.astype(int) * 1e-9
 
         #  Terrestial Time (seconds since J2000)
         tts = t - j2000
         inp_ts = inp
         inp = inp.data
 
     elif isinstance(inp, np.ndarray):
         time = (inp[:, 0] * 1e9).astype("datetime64[ns]")
         t = inp[:, 0]
         #  Terrestial Time (seconds since J2000)
         tts = t - j2000
         inp_ts = None
         inp = inp[:, 1:]
     else:
-        raise TypeError("invalid inpu")
+        raise TypeError("invalid input")
 
     if hapgood:
         day_start_epoch = time.astype("datetime64[D]")
         day_start_epoch = day_start_epoch.astype("datetime64[ns]")
         day_start_epoch = day_start_epoch.astype(np.int64) / 1e9
         mjd_ref_epoch = np.datetime64("2000-01-01T12:00:00", "ns")
         mjd_ref_epoch = mjd_ref_epoch.astype(np.int64) / 1e9
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/cross.py` & `pyrfu-2.4.5/pyrfu/pyrf/gradient.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
+import xarray as xr
 
 # Local imports
-from .resample import resample
-from .ts_vec_xyz import ts_vec_xyz
+from .calc_dt import calc_dt
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def cross(inp1, inp2):
-    r"""Computes cross product of two fields.
+def gradient(inp):
+    r"""Computes time derivative of the input variable.
 
     Parameters
     ----------
-    inp1 : xarray.DataArray
-        Time series of the first field X.
-    inp2 : xarray.DataArray
-        Time series of the second field Y.
+    inp : xarray.DataArray
+        Time series of the input variable.
 
     Returns
     -------
     out : xarray.DataArray
-        Time series of the cross product Z = XxY.
+        Time series of the time derivative of the input variable.
 
     Examples
     --------
     >>> from pyrfu import mms, pyrf
 
-    Define time interval
+    Time interval
 
-    >>> tint = ["2019-09-14T07:54:00.000", "2019-09-14T08:11:00.000"]
+    >>> tint = ["2017-07-18T13:03:34.000", "2017-07-18T13:07:00.000"]
 
-    Index of the MMS spacecraft
+    Spacecraft index
 
     >>> mms_id = 1
 
-    Load magnetic field and electric field
+    Load magnetic field
 
-    >>> b_xyz = mms.get_data("B_gse_fgm_srvy_l2", tint, mms_id)
-    >>> e_xyz = mms.get_data("E_gse_edp_fast_l2", tint, mms_id)
+    >>> b_xyz = mms.get_data("B_gse_fgm_brst_l2", tint, mms_id)
 
-    Compute magnitude of the magnetic field
+    Time derivative of the magnetic field
 
-    >>> b_mag = pyrf.norm(b_xyz)
-
-    Compute ExB drift velocity
-
-    >>> v_xyz_exb = pyrf.cross(e_xyz, b_xyz) / b_mag ** 2
+    >>> db_dt = pyrf.gradient(b_xyz)
 
     """
 
-    if len(inp1) != len(inp2):
-        inp2 = resample(inp2, inp1)
+    # guess time step
+    delta_t = calc_dt(inp)
+
+    d_inp_dt = np.gradient(inp.data, axis=0) / delta_t
 
-    out_data = np.cross(inp1.data, inp2.data, axis=1)
+    out = xr.DataArray(
+        d_inp_dt,
+        coords=inp.coords,
+        dims=inp.dims,
+        attrs=inp.attrs,
+    )
 
-    out = ts_vec_xyz(inp1.time.data, out_data)
+    if "UNITS" in out.attrs:
+        out.attrs["UNITS"] += "/s"
 
     return out
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/datetime2iso8601.py` & `pyrfu-2.4.5/pyrfu/pyrf/datetime2iso8601.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/datetime642iso8601.py` & `pyrfu-2.4.5/pyrfu/pyrf/datetime642iso8601.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/datetime642ttns.py` & `pyrfu-2.4.5/pyrfu/pyrf/datetime642ttns.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/datetime642unix.py` & `pyrfu-2.4.5/pyrfu/pyrf/datetime642unix.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/dec_par_perp.py` & `pyrfu-2.4.5/pyrfu/pyrf/dec_par_perp.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/dist_append.py` & `pyrfu-2.4.5/pyrfu/pyrf/dist_append.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/dot.py` & `pyrfu-2.4.5/pyrfu/pyrf/dot.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/dynamic_press.py` & `pyrfu-2.4.5/pyrfu/pyrf/dynamic_press.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/e_vxb.py` & `pyrfu-2.4.5/pyrfu/pyrf/e_vxb.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/eb_nrf.py` & `pyrfu-2.4.5/pyrfu/pyrf/eb_nrf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/ebsp.py` & `pyrfu-2.4.5/pyrfu/pyrf/ebsp.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/edb.py` & `pyrfu-2.4.5/pyrfu/pyrf/edb.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/end.py` & `pyrfu-2.4.5/pyrfu/pyrf/end.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/estimate.py` & `pyrfu-2.4.5/pyrfu/pyrf/estimate.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/extend_tint.py` & `pyrfu-2.4.5/pyrfu/pyrf/extend_tint.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/filt.py` & `pyrfu-2.4.5/pyrfu/pyrf/filt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/find_closest.py` & `pyrfu-2.4.5/pyrfu/pyrf/find_closest.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/get_omni_data.py` & `pyrfu-2.4.5/pyrfu/pyrf/get_omni_data.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/gradient.py` & `pyrfu-2.4.5/pyrfu/pyrf/increments.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
-
-# Local imports
-from .calc_dt import calc_dt
+from scipy.stats import kurtosis
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def gradient(inp):
-    r"""Computes time derivative of the input variable.
+def increments(inp, scale: int = 10):
+    r"""Returns the increments of a time series.
+
+    .. math:: y = |x_i - x_{i+s}|
+
+    where :math:`s` is the scale.
 
     Parameters
     ----------
     inp : xarray.DataArray
-        Time series of the input variable.
+        Input time series.
+    scale : int, Optional
+        Scale at which to compute the increments. Default is 10.
 
     Returns
     -------
-    out : xarray.DataArray
-        Time series of the time derivative of the input variable.
-
-    Examples
-    --------
-    >>> from pyrfu import mms, pyrf
-
-    Time interval
-
-    >>> tint = ["2017-07-18T13:03:34.000", "2017-07-18T13:07:00.000"]
-
-    Spacecraft index
-
-    >>> mms_id = 1
-
-    Load magnetic field
-
-    >>> b_xyz = mms.get_data("B_gse_fgm_brst_l2", tint, mms_id)
-
-    Time derivative of the magnetic field
-
-    >>> db_dt = pyrf.gradient(b_xyz)
+    kurt : ndarray
+        kurtosis of the increments, one per product, using the Fisher's
+        definition (0 value for a normal distribution).
+    result : xarray.DataArray
+        An xarray containing the time series increments, one per
+        product in the original time series.
 
     """
 
-    # guess time step
-    delta_t = calc_dt(inp)
-
-    d_inp_dt = np.gradient(inp.data, axis=0) / delta_t
-
-    out = xr.DataArray(
-        d_inp_dt,
-        coords=inp.coords,
-        dims=inp.dims,
-        attrs=inp.attrs,
-    )
+    if inp.data.ndim == 1:
+        data = inp.data[:, np.newaxis]
+    else:
+        data = inp.data
+
+    delta_inp = data[scale:, :] - data[:-scale, :]
+
+    result = np.array(delta_inp)
+
+    cols = [inp.coords[dim].data for dim in inp.dims]
+
+    if inp.data.ndim == 1:
+        result = xr.DataArray(
+            np.squeeze(result),
+            coords=[cols[0][0 : len(delta_inp)]],
+            dims=inp.dims,
+            attrs=inp.attrs,
+        )
+    else:
+        result = xr.DataArray(
+            np.squeeze(result),
+            coords=[cols[0][0 : len(delta_inp)], *cols[1:]],
+            dims=inp.dims,
+            attrs=inp.attrs,
+        )
 
-    if "UNITS" in out.attrs:
-        out.attrs["UNITS"] += "/s"
+    kurt = kurtosis(result, axis=0, fisher=False)
 
-    return out
+    return kurt, result
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/gse2gsm.py` & `pyrfu-2.4.5/pyrfu/pyrf/gse2gsm.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/histogram.py` & `pyrfu-2.4.5/pyrfu/pyrf/histogram.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/histogram2d.py` & `pyrfu-2.4.5/pyrfu/pyrf/histogram2d.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/increments.py` & `pyrfu-2.4.5/pyrfu/pyrf/pvi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,60 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
-from scipy.stats import kurtosis
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def increments(inp, scale: int = 10):
-    r"""Returns the increments of a time series.
+def pvi(inp, scale: int = 10):
+    r"""Returns the PVI of a time series.
 
-    .. math:: y = |x_i - x_{i+s}|
+    .. math::
+
+        y = \frac{|x_i - x_{i+s}|^2}{<|x_i - x_{i+s}|^2>}
 
     where :math:`s` is the scale.
 
     Parameters
     ----------
     inp : xarray.DataArray
         Input time series.
     scale : int, Optional
-        Scale at which to compute the increments. Default is 10.
+        Scale at which to compute the PVI. Default is 10.
 
     Returns
     -------
-    kurt : ndarray
-        kurtosis of the increments, one per product, using the Fisher's
-        definition (0 value for a normal distribution).
-    result : xarray.DataArray
-        An xarray containing the time series increments, one per
-        product in the original time series.
+    values : xarray.DataArray
+        An xarray containing the pvi of the original time series.
 
     """
 
-    if inp.data.ndim == 1:
+    if len(inp.data.shape) == 1:
         data = inp.data[:, np.newaxis]
     else:
         data = inp.data
 
-    delta_inp = data[scale:, :] - data[:-scale, :]
-
-    result = np.array(delta_inp)
-
-    cols = [inp.coords[dim].data for dim in inp.dims]
-
-    if inp.data.ndim == 1:
-        result = xr.DataArray(
-            np.squeeze(result),
-            coords=[cols[0][0 : len(delta_inp)]],
-            dims=inp.dims,
-            attrs=inp.attrs,
-        )
-    else:
-        result = xr.DataArray(
-            np.squeeze(result),
-            coords=[cols[0][0 : len(delta_inp)], *cols[1:]],
-            dims=inp.dims,
-            attrs=inp.attrs,
-        )
+    delta_inp = np.abs((data[scale:, :] - data[:-scale, :]))
+    delta_inp2 = np.sum(delta_inp**2, axis=1)
+    sigma = np.mean(delta_inp2)
+    result = np.array(delta_inp2 / sigma)
+
+    time = inp.coords[inp.dims[0]].data
+
+    result = xr.DataArray(
+        result,
+        coords=[time[0 : len(delta_inp)]],
+        dims=[inp.dims[0]],
+        attrs=inp.attrs,
+    )
 
-    kurt = kurtosis(result, axis=0, fisher=False)
+    result.attrs["units"] = "dimensionless"
 
-    return kurt, result
+    return result
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/int_sph_dist.py` & `pyrfu-2.4.5/pyrfu/pyrf/int_sph_dist.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/integrate.py` & `pyrfu-2.4.5/pyrfu/pyrf/integrate.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/iplasma_calc.py` & `pyrfu-2.4.5/pyrfu/pyrf/iplasma_calc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/iso2unix.py` & `pyrfu-2.4.5/pyrfu/pyrf/iso2unix.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/iso86012datetime.py` & `pyrfu-2.4.5/pyrfu/pyrf/iso86012datetime.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/iso86012datetime64.py` & `pyrfu-2.4.5/pyrfu/pyrf/iso86012datetime64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/iso86012timevec.py` & `pyrfu-2.4.5/pyrfu/pyrf/iso86012timevec.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/l_shell.py` & `pyrfu-2.4.5/pyrfu/pyrf/l_shell.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/lowpass.py` & `pyrfu-2.4.5/pyrfu/pyrf/lowpass.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/magnetosphere.py` & `pyrfu-2.4.5/pyrfu/pyrf/magnetosphere.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/match_phibe_dir.py` & `pyrfu-2.4.5/pyrfu/pyrf/match_phibe_dir.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/match_phibe_v.py` & `pyrfu-2.4.5/pyrfu/pyrf/match_phibe_v.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/mean.py` & `pyrfu-2.4.5/pyrfu/pyrf/mean.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/mean_bins.py` & `pyrfu-2.4.5/pyrfu/pyrf/mean_bins.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/mean_field.py` & `pyrfu-2.4.5/pyrfu/pyrf/mean_field.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/medfilt.py` & `pyrfu-2.4.5/pyrfu/pyrf/medfilt.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/median_bins.py` & `pyrfu-2.4.5/pyrfu/pyrf/median_bins.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/movmean.py` & `pyrfu-2.4.5/pyrfu/pyrf/movmean.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/mva.py` & `pyrfu-2.4.5/pyrfu/pyrf/mva.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/mva_gui.py` & `pyrfu-2.4.5/pyrfu/pyrf/mva_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-import matplotlib.dates as dates
-import matplotlib.gridspec as gridspec
-import matplotlib.pyplot as plt
-
 # 3rd party imports
+import matplotlib.pyplot as plt
 import numpy as np
+from matplotlib import dates, gridspec
 from matplotlib.widgets import Button, SpanSelector
 
 # Local imports
 from ..plot import plot_line
 from .mva import mva
 from .new_xyz import new_xyz
 from .norm import norm
@@ -68,15 +66,15 @@
         self.resetbutton.on_clicked(self.reset_selection)
 
         self.span = SpanSelector(
             self.fig.axes[0],
             self.update_onselect,
             "horizontal",
             useblit=True,
-            props=dict(alpha=0, facecolor="black"),
+            props={"alpha": 0, "facecolor": "black"},
             interactive=True,
             minspan=0,
             drag_from_anywhere=True,
         )
 
         # Normal vec - to be calculated
         self.minvar = None
@@ -85,21 +83,21 @@
     @staticmethod
     def init_fig(b_xyz):
         r"""Initialize figure window with time series. Returns figure object
         to access the axes.
         """
 
         fig = plt.figure(figsize=(10, 8))
-        legend_options = dict(
-            ncol=1,
-            loc="center left",
-            frameon=True,
-            framealpha=1,
-            bbox_to_anchor=(1, 0.5),
-        )
+        legend_options = {
+            "ncol": 1,
+            "loc": "center left",
+            "frameon": True,
+            "framealpha": 1,
+            "bbox_to_anchor": (1, 0.5),
+        }
         gs = gridspec.GridSpec(
             3, 3, top=0.9, left=0.05, right=0.9, hspace=0.3, wspace=0.35
         )
         # Time series data
         ax1 = fig.add_subplot(gs[0, :])
 
         # MVA transformed frame
@@ -116,15 +114,15 @@
         ax5.axis("off")
 
         # Plot b_xyz in the first axis
         plot_line(ax1, b_xyz)
         plot_line(ax1, norm(b_xyz), color="black")
         ax1.set_ylabel("$B$ [nT]")
 
-        ax1.set_title(f"Time series for magnetic field")
+        ax1.set_title("Time series for magnetic field")
         b_labels = ["$B_x$", "$B_y$", "$B_z$", "$|B|$"]
         ax1.legend(b_labels, **legend_options)
         return fig
 
     def reset_selection(self):
         r"""Resets MVA selection. Event is passed on from button click but has
         no meaning or use here.
@@ -169,21 +167,21 @@
         frame[:, 2] = np.cross(frame[:, 0], frame[:, 1])
         b_lmn = new_xyz(b_xyz, frame)
         return b_lmn, mva_frame[1], frame
 
     def update_fig(self, b_xyz_clip):
         r"""Update figure based on the clipped time series"""
 
-        legend_options = dict(
-            ncol=1,
-            loc="center left",
-            frameon=True,
-            framealpha=1,
-            bbox_to_anchor=(1, 0.5),
-        )
+        legend_options = {
+            "ncol": 1,
+            "loc": "center left",
+            "frameon": True,
+            "framealpha": 1,
+            "bbox_to_anchor": (1, 0.5),
+        }
 
         # Perform MVA on the clipped time series
         b_lmn_clip, lamb_clip, frame_clip = self.force_positive(
             mva(b_xyz_clip), b_xyz_clip
         )
 
         # Pick out time series for each component of the new magnetic field
@@ -284,12 +282,13 @@
         return b_lmn_clip, lamb_clip, frame_clip
 
     def get_minvar(self):
         r"""Access the minimum varience direction vector from mva_gui_class object
         via this method.
         """
 
-        if self.minvar is None:
-            raise Exception("Normal has not been calculated yet")
-        else:
+        if self.minvar is not None:
             out = self.minvar
-            return out
+        else:
+            raise RuntimeError("Normal has not been calculated yet")
+
+        return out
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/new_xyz.py` & `pyrfu-2.4.5/pyrfu/pyrf/new_xyz.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/norm.py` & `pyrfu-2.4.5/pyrfu/pyrf/norm.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/normalize.py` & `pyrfu-2.4.5/pyrfu/pyrf/normalize.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/optimize_nbins_1d.py` & `pyrfu-2.4.5/pyrfu/pyrf/optimize_nbins_1d.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/optimize_nbins_2d.py` & `pyrfu-2.4.5/pyrfu/pyrf/optimize_nbins_2d.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/pid_4sc.py` & `pyrfu-2.4.5/pyrfu/pyrf/pid_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/plasma_beta.py` & `pyrfu-2.4.5/pyrfu/pyrf/plasma_beta.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/plasma_calc.py` & `pyrfu-2.4.5/pyrfu/pyrf/plasma_calc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/poynting_flux.py` & `pyrfu-2.4.5/pyrfu/pyrf/poynting_flux.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/pres_anis.py` & `pyrfu-2.4.5/pyrfu/pyrf/pres_anis.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/psd.py` & `pyrfu-2.4.5/pyrfu/pyrf/psd.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/pvi.py` & `pyrfu-2.4.5/pyrfu/pyrf/ts_scalar.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,52 +9,41 @@
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def pvi(inp, scale: int = 10):
-    r"""Returns the PVI of a time series.
-
-    .. math::
-
-        y = \frac{|x_i - x_{i+s}|^2}{<|x_i - x_{i+s}|^2>}
-
-    where :math:`s` is the scale.
+def ts_scalar(time, data, attrs: dict = None):
+    r"""Create a time series containing a 0th order tensor
 
     Parameters
     ----------
-    inp : xarray.DataArray
-        Input time series.
-    scale : int, Optional
-        Scale at which to compute the PVI. Default is 10.
+    time : numpy.ndarray
+        Array of times.
+    data : numpy.ndarray
+        Data corresponding to the time list.
+    attrs : dict, Optional
+        Attributes of the data list.
 
     Returns
     -------
-    values : xarray.DataArray
-        An xarray containing the pvi of the original time series.
+    out : xarray.DataArray
+        0th order tensor time series.
 
     """
 
-    if len(inp.data.shape) == 1:
-        data = inp.data[:, np.newaxis]
-    else:
-        data = inp.data
-
-    delta_inp = np.abs((data[scale:, :] - data[:-scale, :]))
-    delta_inp2 = np.sum(delta_inp**2, axis=1)
-    sigma = np.mean(delta_inp2)
-    result = np.array(delta_inp2 / sigma)
-
-    time = inp.coords[inp.dims[0]].data
-
-    result = xr.DataArray(
-        result,
-        coords=[time[0 : len(delta_inp)]],
-        dims=[inp.dims[0]],
-        attrs=inp.attrs,
-    )
+    # Check input type
+    assert isinstance(time, np.ndarray), "time must be a numpy.ndarray"
+    assert isinstance(data, np.ndarray), "data must be a numpy.ndarray"
+
+    # Check input shape must be (n, )
+    assert data.ndim == 1, "Input must be a scalar"
+    assert len(time) == len(data), "Time and data must have the same length"
+
+    if attrs is None or not isinstance(attrs, dict):
+        attrs = {}
 
-    result.attrs["units"] = "dimensionless"
+    out = xr.DataArray(data, coords=[time[:]], dims="time", attrs=attrs)
+    out.attrs["TENSOR_ORDER"] = 0
 
-    return result
+    return out
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/pvi_4sc.py` & `pyrfu-2.4.5/pyrfu/pyrf/pvi_4sc.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/read_cdf.py` & `pyrfu-2.4.5/pyrfu/pyrf/read_cdf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/remove_repeated_points.py` & `pyrfu-2.4.5/pyrfu/pyrf/remove_repeated_points.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/resample.py` & `pyrfu-2.4.5/pyrfu/pyrf/resample.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/shock_models_parameters.json` & `pyrfu-2.4.5/pyrfu/pyrf/shock_models_parameters.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/shock_normal.py` & `pyrfu-2.4.5/pyrfu/pyrf/shock_normal.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,20 +121,23 @@
             relations, Journal of Geophysical Research, vol. 93, no. A4, pp. 2730–2734.
             doi:10.1029/JA093iA04p02730.
 
 
 
     """
 
+    # Check input
+    assert isinstance(spec, dict), "spec must be a dictionary"
+
     if spec["b_u"].ndim > 1 or spec["b_d"].ndim > 1:
         n_bu = len(spec["b_u"])
         n_bd = len(spec["b_d"])
 
         # randomize points upstream and downstream
-        n = spec.get("n", 10.0)
+        n = int(np.floor(spec.get("n", 10.0)))
         idt_u, idt_d = [np.random.rand(n) for _ in range(2)]
 
         tmp_spec = {}
         for i in range(n):
             f_bu = interpolate.interp1d(np.linspace(0, 1, n_bu), spec["b_u"], axis=0)
             tmp_spec["b_u"] = f_bu(idt_u[i])
             f_vu = interpolate.interp1d(np.linspace(0, 1, n_bu), spec["v_u"], axis=0)
@@ -245,18 +248,16 @@
     theta = np.arccos(np.sum(au * ad) / (np.linalg.norm(au) * np.linalg.norm(ad)))
     return np.rad2deg(theta)
 
 
 def _shock_angle(spec, n, field, leq90):
     if field.lower() == "b":
         a = spec["b_u"]
-    elif field.lower() == "v":
-        a = spec["v_u"]
     else:
-        raise ValueError("Invalid field. Must be 'b' or 'v'!!")
+        a = spec["v_u"]
 
     theta = {}
 
     for fname in n:
         tmp = np.rad2deg(np.arccos(np.sum(a * n[fname]) / np.linalg.norm(a)))
 
         if tmp > 90.0 and leq90:
@@ -322,39 +323,33 @@
     # normal vector
     n = grad_s / np.linalg.norm(grad_s, keepdims=True)
 
     return n, sig_0.x[0]
 
 
 def _shock_speed(spec, n, theta_bn, method):
-    if method.lower() == "gt":
-        if "f_cp" in spec and "dt_f" in spec and "d2u" in spec:
-            v_sh = _speed_gosling_thomsen(spec, n, theta_bn)
-        else:
-            v_sh = {k: 0.0 for k in n}
+    if method.lower() == "gt" and "f_cp" in spec and "dt_f" in spec and "d2u" in spec:
+        v_sh = _speed_gosling_thomsen(spec, n, theta_bn)
     elif method.lower() == "mf":
         v_sh = _speed_mass_flux(spec, n)
     elif method.lower() == "sb":
         v_sh = _speed_smith_burton(spec, n)
-    elif method.lower() == "mo":
-        if "f_cp" in spec and "dt_f" in spec and "d2u" in spec:
-            v_sh = _speed_moses(spec, n, theta_bn)
-        else:
-            v_sh = {k: 0.0 for k in n}
+    elif method.lower() == "mo" and "f_cp" in spec and "dt_f" in spec and "d2u" in spec:
+        v_sh = _speed_moses(spec, n, theta_bn)
     else:
-        raise ValueError("Invalid method!")
+        v_sh = {k: 0.0 for k in n}
 
     return v_sh
 
 
 def _speed_gosling_thomsen(spec, n, theta_bn):
     v_sh = {}
 
     for k, nvec in n.items():
-        theta = np.deg2rad(theta_bn)
+        theta = np.deg2rad(theta_bn[k])
         nvec = n[k]
 
         # Notation as in (Gosling and Thomsen 1985)
         w = 2 * np.pi * spec["f_cp"]
         t1 = np.arccos((1 - 2 * np.cos(theta) ** 2) / (2 * np.sin(theta) ** 2)) / w
         x_0 = w * t1 * (2 * np.cos(theta) ** 2 - 1) + 2 * np.sin(theta) ** 2 * np.sin(
             w * t1
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/shock_parameters.py` & `pyrfu-2.4.5/pyrfu/pyrf/shock_parameters.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/solid_angle.py` & `pyrfu-2.4.5/pyrfu/pyrf/solid_angle.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/sph2cart.py` & `pyrfu-2.4.5/pyrfu/pyrf/sph2cart.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/st_diff.py` & `pyrfu-2.4.5/pyrfu/pyrf/st_diff.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/start.py` & `pyrfu-2.4.5/pyrfu/pyrf/start.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/struct_func.py` & `pyrfu-2.4.5/pyrfu/pyrf/struct_func.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/t_eval.py` & `pyrfu-2.4.5/pyrfu/pyrf/t_eval.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/time_clip.py` & `pyrfu-2.4.5/pyrfu/pyrf/time_clip.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/timevec2iso8601.py` & `pyrfu-2.4.5/pyrfu/pyrf/timevec2iso8601.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/trace.py` & `pyrfu-2.4.5/pyrfu/pyrf/trace.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/transformation_indices.json` & `pyrfu-2.4.5/pyrfu/pyrf/transformation_indices.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/ts_append.py` & `pyrfu-2.4.5/pyrfu/pyrf/ts_append.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/ts_scalar.py` & `pyrfu-2.4.5/pyrfu/pyrf/ts_tensor_xyz.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,41 +9,47 @@
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def ts_scalar(time, data, attrs: dict = None):
-    r"""Create a time series containing a 0th order tensor
+def ts_tensor_xyz(time, data, attrs: dict = None):
+    r"""Create a time series containing a 2nd order tensor.
 
     Parameters
     ----------
-    time : numpy.ndarray
+    time : ndarray
         Array of times.
-    data : numpy.ndarray
+    data : ndarray
         Data corresponding to the time list.
     attrs : dict, Optional
         Attributes of the data list.
 
     Returns
     -------
     out : xarray.DataArray
-        0th order tensor time series.
+        2nd order tensor time series.
 
     """
 
     # Check input type
     assert isinstance(time, np.ndarray), "time must be a numpy.ndarray"
     assert isinstance(data, np.ndarray), "data must be a numpy.ndarray"
 
-    # Check input shape must be (n, )
-    assert data.ndim == 1, "Input must be a scalar"
+    # Check input shape must be (n, 3, 3)
+    assert data.ndim == 3 and data.shape[1:] == (3, 3)
     assert len(time) == len(data), "Time and data must have the same length"
 
     if attrs is None or not isinstance(attrs, dict):
         attrs = {}
 
-    out = xr.DataArray(data, coords=[time[:]], dims="time", attrs=attrs)
-    out.attrs["TENSOR_ORDER"] = 0
+    out = xr.DataArray(
+        data,
+        coords=[time[:], ["x", "y", "z"], ["x", "y", "z"]],
+        dims=["time", "comp_h", "comp_v"],
+        attrs=attrs,
+    )
+
+    out.attrs["TENSOR_ORDER"] = 2
 
     return out
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/ts_skymap.py` & `pyrfu-2.4.5/pyrfu/pyrf/ts_skymap.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/ts_tensor_xyz.py` & `pyrfu-2.4.5/pyrfu/pyrf/ts_vec_xyz.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,47 +9,47 @@
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
 __version__ = "2.4.2"
 __status__ = "Prototype"
 
 
-def ts_tensor_xyz(time, data, attrs: dict = None):
-    r"""Create a time series containing a 2nd order tensor.
+def ts_vec_xyz(time, data, attrs: dict = None):
+    r"""Create a time series containing a 1st order tensor.
 
     Parameters
     ----------
     time : ndarray
         Array of times.
     data : ndarray
         Data corresponding to the time list.
     attrs : dict, Optional
         Attributes of the data list.
 
     Returns
     -------
     out : xarray.DataArray
-        2nd order tensor time series.
+        1st order tensor time series.
 
     """
 
     # Check input type
     assert isinstance(time, np.ndarray), "time must be a numpy.ndarray"
     assert isinstance(data, np.ndarray), "data must be a numpy.ndarray"
 
-    # Check input shape must be (n, 3, 3)
-    assert data.ndim == 3 and data.shape[1:] == (3, 3)
+    # Check input shape must be (n, 3)
+    assert data.ndim == 2 and data.shape[1] == 3
     assert len(time) == len(data), "Time and data must have the same length"
 
     if attrs is None or not isinstance(attrs, dict):
         attrs = {}
 
     out = xr.DataArray(
         data,
-        coords=[time[:], ["x", "y", "z"], ["x", "y", "z"]],
-        dims=["time", "comp_h", "comp_v"],
+        coords=[time[:], ["x", "y", "z"]],
+        dims=["time", "comp"],
         attrs=attrs,
     )
 
-    out.attrs["TENSOR_ORDER"] = 2
+    out.attrs["TENSOR_ORDER"] = 1
 
     return out
```

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/ts_time.py` & `pyrfu-2.4.5/pyrfu/pyrf/ts_time.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/ttns2datetime64.py` & `pyrfu-2.4.5/pyrfu/pyrf/ttns2datetime64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/unix2datetime64.py` & `pyrfu-2.4.5/pyrfu/pyrf/unix2datetime64.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/vht.py` & `pyrfu-2.4.5/pyrfu/pyrf/vht.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/wave_fft.py` & `pyrfu-2.4.5/pyrfu/pyrf/wave_fft.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/wavelet.py` & `pyrfu-2.4.5/pyrfu/pyrf/wavelet.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/wavepolarize_means.py` & `pyrfu-2.4.5/pyrfu/pyrf/wavepolarize_means.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/pyrf/waverage.py` & `pyrfu-2.4.5/pyrfu/pyrf/waverage.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/solo/db_init.py` & `pyrfu-2.4.5/pyrfu/solo/db_init.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/solo/read_lfr_density.py` & `pyrfu-2.4.5/pyrfu/solo/read_lfr_density.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/solo/read_tnr.py` & `pyrfu-2.4.5/pyrfu/solo/read_tnr.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.4/pyrfu/tests/test_pyrf.py` & `pyrfu-2.4.5/pyrfu/tests/test_pyrf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # Built-in imports
 import datetime
+import itertools
+import random
 import unittest
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
+from ddt import data, ddt, idata
 
 from pyrfu import pyrf
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
@@ -53,14 +56,28 @@
     return out
 
 
 def generate_ts_scalar(f_s, n_pts):
     return pyrf.ts_scalar(generate_timeline(f_s, n_pts), generate_data(n_pts, "vector"))
 
 
+def generate_ts_skymap(f_s, n_pts):
+    return pyrf.ts_skymap(
+        generate_timeline(f_s, n_pts),
+        np.random.random((n_pts, 32, 32, 16)),
+        np.random.random((n_pts, 32)),
+        np.random.random((n_pts, 32)),
+        np.random.random(16),
+        glob_attrs={
+            "delta_energy_plus": np.random.random((n_pts, 32)),
+            "delta_energy_minus": np.random.random((n_pts, 32)),
+        },
+    )
+
+
 class AutoCorrTestCase(unittest.TestCase):
     def test_autocorr_input_type(self):
         self.assertIsNotNone(pyrf.autocorr(generate_ts(64.0, 100, "scalar")))
         self.assertIsNotNone(pyrf.autocorr(generate_ts(64.0, 100, "scalar"), 25))
         self.assertIsNotNone(pyrf.autocorr(generate_ts(64.0, 100, "scalar"), 25, True))
 
     def test_autocorr_input_shape(self):
@@ -90,235 +107,192 @@
 
         result = pyrf.autocorr(generate_ts(64.0, 100, "vector"))
         self.assertEqual(result.ndim, 2)
         self.assertEqual(result.shape[0], 100)
         self.assertEqual(result.shape[1], 3)
 
 
-class TsSkymapTestCase(unittest.TestCase):
-    def test_ts_skymap_input_type(self):
+class AverageVDFTestCase(unittest.TestCase):
+    def test_average_vdf_input_type(self):
         with self.assertRaises(AssertionError):
-            pyrf.ts_skymap(0, 0, 0, 0, 0)
+            pyrf.average_vdf(0, 3)
+            pyrf.average_vdf(np.random.random((100, 32, 32, 16)), 3)
+            pyrf.average_vdf(generate_ts_skymap(64.0, 100), [3, 5])
 
-    def test_ts_skymap_output_type(self):
-        result = pyrf.ts_skymap(
-            generate_timeline(64.0, 100),
-            np.random.random((100, 32, 32, 16)),
-            np.random.random((100, 32)),
-            np.random.random((100, 32)),
-            np.random.random(16),
-        )
-        self.assertIsInstance(result, xr.Dataset)
-
-    def test_ts_skymap_output_shape(self):
-        result = pyrf.ts_skymap(
-            generate_timeline(64.0, 100),
-            np.random.random((100, 32, 32, 16)),
-            np.random.random((100, 32)),
-            np.random.random((100, 32)),
-            np.random.random(16),
-        )
-        self.assertEqual(result.data.ndim, 4)
-        self.assertListEqual(list(result.data.shape), [100, 32, 32, 16])
-        self.assertEqual(result.energy.ndim, 2)
-        self.assertListEqual(list(result.energy.shape), [100, 32])
-        self.assertEqual(result.phi.ndim, 2)
-        self.assertListEqual(list(result.phi.shape), [100, 32])
-        self.assertEqual(result.theta.ndim, 1)
-        self.assertListEqual(list(result.theta.shape), [16])
+    def test_average_vdf_values(self):
+        with self.assertRaises(AssertionError):
+            pyrf.average_vdf(generate_ts_skymap(64.0, 100), 2)
 
-    def test_ts_skymap_output_meta(self):
-        result = pyrf.ts_skymap(
-            generate_timeline(64.0, 100),
-            np.random.random((100, 32, 32, 16)),
-            np.random.random((100, 32)),
-            np.random.random((100, 32)),
-            np.random.random(16),
-        )
-        self.assertListEqual(
-            list(result.attrs.keys()), ["energy0", "energy1", "esteptable"]
-        )
-        self.assertListEqual(
-            list(result.attrs["energy0"].shape),
-            [
-                32,
-            ],
-        )
-        self.assertListEqual(
-            list(result.attrs["energy1"].shape),
-            [
-                32,
-            ],
-        )
-        self.assertListEqual(
-            list(result.attrs["esteptable"].shape),
-            [
-                100,
-            ],
+    def test_average_vdf_output_type(self):
+        self.assertIsInstance(
+            pyrf.average_vdf(generate_ts_skymap(64.0, 100), 3), xr.Dataset
         )
 
-        for k in result:
-            self.assertEqual(result[k].attrs, {})
+    def test_average_vdf_output_meta(self):
+        avg_inds = np.arange(1, 99, 3, dtype=int)
+        result = pyrf.average_vdf(generate_ts_skymap(64.0, 100), 3)
 
+        self.assertIsInstance(result.attrs["delta_energy_plus"], np.ndarray)
+        self.assertEqual(result.attrs["delta_energy_plus"].ndim, 2)
+        self.assertEqual(len(result.attrs["delta_energy_plus"]), len(avg_inds))
 
-class StartTestCase(unittest.TestCase):
-    def test_start_input_type(self):
-        self.assertIsNotNone(pyrf.start(generate_ts(64.0, 100, "scalar")))
-        self.assertIsNotNone(pyrf.start(generate_ts(64.0, 100, "vector")))
-        self.assertIsNotNone(pyrf.start(generate_ts(64.0, 100, "tensor")))
+        self.assertIsInstance(result.attrs["delta_energy_minus"], np.ndarray)
+        self.assertEqual(result.attrs["delta_energy_minus"].ndim, 2)
+        self.assertEqual(len(result.attrs["delta_energy_minus"]), len(avg_inds))
 
-        with self.assertRaises(AssertionError):
-            pyrf.start(0)
-            pyrf.start(generate_timeline(64.0, 100))
 
-    def test_start_output(self):
-        result = pyrf.start(generate_ts(64.0, 100, "scalar"))
-        self.assertIsInstance(result, np.float64)
-        self.assertEqual(
-            np.datetime64(int(result * 1e9), "ns"),
-            np.datetime64("2019-01-01T00:00:00.000"),
+class Avg4SCTestCase(unittest.TestCase):
+    def test_avg_4sc_input(self):
+        self.assertIsNotNone(
+            pyrf.avg_4sc(
+                [
+                    generate_ts(64.0, 100, "scalar"),
+                    generate_ts(64.0, 100, "scalar"),
+                    generate_ts(64.0, 100, "scalar"),
+                    generate_ts(64.0, 100, "scalar"),
+                ]
+            )
         )
-
-
-class TsScalarTestCase(unittest.TestCase):
-    def test_ts_scalar_input_type(self):
-        with self.assertRaises(AssertionError):
-            pyrf.ts_scalar(0, 0)
-            pyrf.ts_scalar(
-                list(generate_timeline(64.0, 100)), list(generate_data(100, "scalar"))
+        self.assertIsNotNone(
+            pyrf.avg_4sc(
+                [
+                    generate_ts(64.0, 100, "vector"),
+                    generate_ts(64.0, 100, "vector"),
+                    generate_ts(64.0, 100, "vector"),
+                    generate_ts(64.0, 100, "vector"),
+                ]
             )
-
-    def test_ts_scalar_input_shape(self):
-        with self.assertRaises(AssertionError):
-            # Raises error if data and timeline don't have the same size
-            pyrf.ts_scalar(generate_timeline(64.0, 100), generate_data(99, "scalar"))
-            # Raises error if vector as input
-            pyrf.ts_scalar(generate_timeline(64.0, 100), generate_data(100, "vector"))
-            # Raises error if tensor as input
-            pyrf.ts_scalar(generate_timeline(64.0, 100), generate_data(100, "tensor"))
-
-    def test_ts_scalar_output_type(self):
-        result = pyrf.ts_scalar(
-            generate_timeline(64.0, 100), generate_data(100, "scalar")
         )
-        self.assertIsInstance(result, xr.DataArray)
-
-    def test_ts_scalar_output_shape(self):
-        result = pyrf.ts_scalar(
-            generate_timeline(64.0, 100), generate_data(100, "scalar")
+        self.assertIsNotNone(
+            pyrf.avg_4sc(
+                [
+                    generate_ts(64.0, 100, "tensor"),
+                    generate_ts(64.0, 100, "tensor"),
+                    generate_ts(64.0, 100, "tensor"),
+                    generate_ts(64.0, 100, "tensor"),
+                ]
+            )
         )
-        self.assertEqual(result.ndim, 1)
-        self.assertEqual(len(result), 100)
 
-    def test_ts_scalar_dims(self):
-        result = pyrf.ts_scalar(
-            generate_timeline(64.0, 100), generate_data(100, "scalar")
-        )
-        self.assertListEqual(list(result.dims), ["time"])
+        with self.assertRaises(TypeError):
+            pyrf.avg_4sc(
+                [
+                    generate_data(100, "tensor"),
+                    generate_data(100, "tensor"),
+                    generate_data(100, "tensor"),
+                    generate_data(100, "tensor"),
+                ]
+            )
 
-    def test_ts_scalar_meta(self):
-        result = pyrf.ts_scalar(
-            generate_timeline(64.0, 100), generate_data(100, "scalar")
+    def test_avg_4sc_output(self):
+        result = pyrf.avg_4sc(
+            [
+                generate_ts(64.0, 100, "tensor"),
+                generate_ts(64.0, 100, "tensor"),
+                generate_ts(64.0, 100, "tensor"),
+                generate_ts(64.0, 100, "tensor"),
+            ]
         )
-        self.assertEqual(result.attrs["TENSOR_ORDER"], 0)
 
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3, 3])
 
-class TsVecXYZTestCase(unittest.TestCase):
-    def test_ts_vec_xyz_input_type(self):
+
+class C4GradTestCase(unittest.TestCase):
+    def test_c_4_grad_input(self):
         with self.assertRaises(AssertionError):
-            pyrf.ts_vec_xyz(0, 0)
-            pyrf.ts_vec_xyz(
-                list(generate_timeline(64.0, 100)), list(generate_data(100, "vector"))
+            pyrf.c_4_grad(
+                generate_ts(64.0, 100, kind="vector"),
+                generate_ts(64.0, 100, kind="vector"),
             )
+            pyrf.c_4_grad([], [])
 
-    def test_ts_vec_xyz_input_shape(self):
-        with self.assertRaises(AssertionError):
-            # Raises error if data and timeline don't have the same size
-            pyrf.ts_vec_xyz(generate_timeline(64.0, 100), generate_data(99, "vector"))
-            # Raises error if vector as input
-            pyrf.ts_vec_xyz(generate_timeline(64.0, 100), generate_data(100, "scalar"))
-            # Raises error if tensor as input
-            pyrf.ts_vec_xyz(generate_timeline(64.0, 100), generate_data(100, "tensor"))
+            pyrf.c_4_grad(
+                [generate_ts(64.0, 100, kind="vector") for _ in range(4)],
+                [generate_ts(64.0, 100, kind="vector") for _ in range(4)],
+                0,
+            )
 
-    def test_ts_vec_xyz_output_type(self):
-        result = pyrf.ts_vec_xyz(
-            generate_timeline(64.0, 100), generate_data(100, "vector")
-        )
+            pyrf.c_4_grad(
+                [generate_ts(64.0, 100, kind="vector") for _ in range(4)],
+                [generate_ts(64.0, 100, kind="vector") for _ in range(4)],
+                "bazinga",
+            )
+
+    def test_c_4_grad_output(self):
+        r_mms = [generate_ts(64.0, 100, kind="vector") for _ in range(4)]
+        b_mms = [generate_ts(64.0, 100, kind="vector") for _ in range(4)]
+        n_mms = [generate_ts(64.0, 100, kind="scalar") for _ in range(4)]
+
+        result = pyrf.c_4_grad(r_mms, b_mms, "grad")
         self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3, 3])
 
-    def test_ts_vec_xyz_output_shape(self):
-        result = pyrf.ts_vec_xyz(
-            generate_timeline(64.0, 100), generate_data(100, "vector")
+        result = pyrf.c_4_grad(r_mms, b_mms, "div")
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(
+            list(result.shape),
+            [
+                100,
+            ],
         )
-        self.assertEqual(result.ndim, 2)
-        self.assertEqual(result.shape[0], 100)
-        self.assertEqual(result.shape[1], 3)
 
-    def test_ts_vec_xyz_dims(self):
-        result = pyrf.ts_vec_xyz(
-            generate_timeline(64.0, 100), generate_data(100, "vector")
-        )
-        self.assertListEqual(list(result.dims), ["time", "comp"])
+        result = pyrf.c_4_grad(r_mms, b_mms, "curl")
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
 
-    def test_ts_vec_xyz_meta(self):
-        result = pyrf.ts_vec_xyz(
-            generate_timeline(64.0, 100), generate_data(100, "vector")
-        )
-        self.assertEqual(result.attrs["TENSOR_ORDER"], 1)
+        result = pyrf.c_4_grad(r_mms, b_mms, "bdivb")
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
 
+        result = pyrf.c_4_grad(r_mms, b_mms, "curv")
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
 
-class TsTensorXYZTestCase(unittest.TestCase):
-    def test_ts_tensor_xyz_input_type(self):
-        with self.assertRaises(AssertionError):
-            pyrf.ts_tensor_xyz(0, 0)
-            pyrf.ts_tensor_xyz(
-                list(generate_timeline(64.0, 100)), list(generate_data(100, "tensor"))
-            )
+        result = pyrf.c_4_grad(r_mms, n_mms, "grad")
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
 
-    def test_ts_tensor_xyz_input_shape(self):
+
+class C4JTestCase(unittest.TestCase):
+    def test_c_4_j_input(self):
         with self.assertRaises(AssertionError):
-            # Raises error if data and timeline don't have the same size
-            pyrf.ts_tensor_xyz(
-                generate_timeline(64.0, 100), generate_data(99, "tensor")
-            )
-            # Raises error if vector as input
-            pyrf.ts_tensor_xyz(
-                generate_timeline(64.0, 100), generate_data(100, "scalar")
-            )
-            # Raises error if tensor as input
-            pyrf.ts_tensor_xyz(
-                generate_timeline(64.0, 100), generate_data(100, "vector")
+            pyrf.c_4_j(
+                generate_ts(64.0, 100, kind="vector"),
+                generate_ts(64.0, 100, kind="vector"),
             )
+            pyrf.c_4_j([], [])
 
-    def test_ts_tensor_xyz_output_type(self):
-        result = pyrf.ts_tensor_xyz(
-            generate_timeline(64.0, 100), generate_data(100, "tensor")
-        )
-        self.assertIsInstance(result, xr.DataArray)
+    def test_c_4_j_output(self):
+        r_mms = [generate_ts(64.0, 100, kind="vector") for _ in range(4)]
+        b_mms = [generate_ts(64.0, 100, kind="vector") for _ in range(4)]
+        j, div_b, b_avg, jxb, div_t_shear, div_pb = pyrf.c_4_j(r_mms, b_mms)
 
-    def test_ts_tensor_xyz_output_shape(self):
-        result = pyrf.ts_tensor_xyz(
-            generate_timeline(64.0, 100), generate_data(100, "tensor")
-        )
-        self.assertEqual(result.ndim, 3)
-        self.assertEqual(result.shape[0], 100)
-        self.assertEqual(result.shape[1], 3)
-        self.assertEqual(result.shape[2], 3)
+        self.assertIsInstance(j, xr.DataArray)
+        self.assertListEqual(list(j.shape), [100, 3])
 
-    def test_ts_tensor_xyz_dims(self):
-        result = pyrf.ts_tensor_xyz(
-            generate_timeline(64.0, 100), generate_data(100, "tensor")
+        self.assertIsInstance(div_b, xr.DataArray)
+        self.assertListEqual(
+            list(div_b.shape),
+            [
+                100,
+            ],
         )
-        self.assertListEqual(list(result.dims), ["time", "comp_h", "comp_v"])
 
-    def test_ts_tensor_xyz_meta(self):
-        result = pyrf.ts_tensor_xyz(
-            generate_timeline(64.0, 100), generate_data(100, "tensor")
-        )
-        self.assertEqual(result.attrs["TENSOR_ORDER"], 2)
+        self.assertIsInstance(b_avg, xr.DataArray)
+        self.assertListEqual(list(b_avg.shape), [100, 3])
+
+        self.assertIsInstance(jxb, xr.DataArray)
+        self.assertListEqual(list(jxb.shape), [100, 3])
+
+        self.assertIsInstance(div_t_shear, xr.DataArray)
+        self.assertListEqual(list(div_t_shear.shape), [100, 3])
+
+        self.assertIsInstance(div_pb, xr.DataArray)
+        self.assertListEqual(list(div_pb.shape), [100, 3])
 
 
 class CalcFsTestCase(unittest.TestCase):
     def test_calc_fs_input_type(self):
         self.assertIsNotNone(pyrf.calc_fs(generate_ts(64.0, 100)))
 
         with self.assertRaises(AssertionError):
@@ -457,14 +431,158 @@
         self.assertListEqual(list(result.dims), ["time"])
 
     def test_calc_sqrtq_meta(self):
         result = pyrf.calc_sqrtq(generate_ts(64.0, 100, "tensor"))
         self.assertEqual(result.attrs["TENSOR_ORDER"], 0)
 
 
+class Cart2SphTestCase(unittest.TestCase):
+    def test_cart2sph_output(self):
+        result = pyrf.cart2sph(1.0, 1.0, 1.0)
+        self.assertIsInstance(result[0], np.float64)
+        self.assertIsInstance(result[1], np.float64)
+        self.assertIsInstance(result[2], np.float64)
+
+        result = pyrf.cart2sph(
+            np.random.random(100), np.random.random(100), np.random.random(100)
+        )
+        self.assertIsInstance(result[0], np.ndarray)
+        self.assertListEqual(
+            list(result[0].shape),
+            [
+                100,
+            ],
+        )
+        self.assertIsInstance(result[1], np.ndarray)
+        self.assertListEqual(
+            list(result[1].shape),
+            [
+                100,
+            ],
+        )
+        self.assertIsInstance(result[2], np.ndarray)
+        self.assertListEqual(
+            list(result[2].shape),
+            [
+                100,
+            ],
+        )
+
+
+class Cart2SphTsTestCase(unittest.TestCase):
+    def test_cart2sph_ts_input(self):
+        with self.assertRaises(AssertionError):
+            pyrf.cart2sph_ts(0.0)
+            pyrf.cart2sph_ts(generate_data(100, "vector"))
+            pyrf.cart2sph_ts(generate_ts(64.0, 100, "scalar"))
+            pyrf.cart2sph_ts(generate_ts(64.0, 100, "vector"), 2)
+
+    def test_cart2sph_ts_output(self):
+        result = pyrf.cart2sph_ts(generate_ts(64.0, 100, "vector"), 1)
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
+
+        result = pyrf.cart2sph_ts(generate_ts(64.0, 100, "vector"), -1)
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
+
+
+class ConvertFACTestCase(unittest.TestCase):
+    def test_convert_fac_input(self):
+        with self.assertRaises(AssertionError):
+            pyrf.convert_fac(0, 0)
+            pyrf.convert_fac(generate_data(100, "vector"), generate_data(100, "vector"))
+
+        with self.assertRaises(TypeError):
+            pyrf.convert_fac(
+                generate_ts(64.0, 100, "tensor"), generate_ts(64.0, 100, "vector")
+            )
+
+    def test_convert_fac_output(self):
+        result = pyrf.convert_fac(
+            generate_ts(64.0, 100, "vector"), generate_ts(64.0, 100, "vector")
+        )
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
+
+        result = pyrf.convert_fac(
+            generate_ts(64.0, 100, "vector"), generate_ts(64.0, 98, "vector")
+        )
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
+
+        result = pyrf.convert_fac(
+            generate_ts(64.0, 100, "vector"),
+            generate_ts(64.0, 100, "vector"),
+            np.random.random(3),
+        )
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
+
+        result = pyrf.convert_fac(
+            generate_ts(64.0, 100, "vector"),
+            generate_ts(64.0, 100, "vector"),
+            generate_ts(64.0, 100, "vector"),
+        )
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
+
+        result = pyrf.convert_fac(
+            generate_ts(64.0, 100, "vector"),
+            generate_ts(64.0, 100, "vector"),
+            generate_ts(64.0, 97, "vector"),
+        )
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
+
+        result = pyrf.convert_fac(
+            generate_ts(64.0, 100, "scalar"),
+            generate_ts(64.0, 100, "vector"),
+            generate_ts(64.0, 100, "vector"),
+        )
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 2])
+
+
+@ddt
+class CotransTestCase(unittest.TestCase):
+    def test_cotrans_input(self):
+        with self.assertRaises(TypeError):
+            pyrf.cotrans(0.0, "gse>gsm")
+
+        with self.assertRaises(IndexError):
+            pyrf.cotrans(generate_data(100), "gse>gsm")
+
+        with self.assertRaises(ValueError):
+            pyrf.cotrans(generate_ts(64.0, 100, "vector"), "gsm")
+
+    @idata(itertools.permutations(["gei", "geo", "gse", "gsm", "mag", "sm"], 2))
+    def test_cotrans_output(self, value):
+        transf = f"{value[0]}>{value[1]}"
+        result = pyrf.cotrans(generate_ts(64.0, 100, "vector"), transf)
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
+
+        result = pyrf.cotrans(generate_ts(64.0, 100, "vector"), transf, hapgood=False)
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
+
+        inp = generate_ts(64.0, 100, "vector")
+        inp.attrs["COORDINATE_SYSTEM"] = value[0]
+        result = pyrf.cotrans(inp, value[1], hapgood=False)
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
+
+        inp = generate_ts(64.0, 100, "vector")
+        inp.attrs["COORDINATE_SYSTEM"] = value[0]
+        result = pyrf.cotrans(inp, value[1], hapgood=True)
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
+
+
 class CdfEpoch2Datetime64TestCase(unittest.TestCase):
     def test_cdfepoch2datetime64_input_type(self):
         ref_time = 599572869184000000
         self.assertIsNotNone(pyrf.cdfepoch2datetime64(ref_time))
         time_line = np.arange(ref_time, int(ref_time + 100))
         self.assertIsNotNone(pyrf.cdfepoch2datetime64(time_line))
         self.assertIsNotNone(pyrf.cdfepoch2datetime64(list(time_line)))
@@ -480,14 +598,60 @@
         ref_time = 599572869184000000
         self.assertEqual(len(pyrf.cdfepoch2datetime64(ref_time)), 1)
         time_line = np.arange(ref_time, int(ref_time + 100))
         self.assertEqual(len(pyrf.cdfepoch2datetime64(time_line)), 100)
         self.assertEqual(len(pyrf.cdfepoch2datetime64(list(time_line))), 100)
 
 
+class CrossTestCase(unittest.TestCase):
+    def test_cross_input(self):
+        with self.assertRaises(AssertionError):
+            pyrf.cross(
+                generate_ts(64.0, 100, "scalar"), generate_ts(64.0, 100, "scalar")
+            )
+            pyrf.cross(
+                generate_ts(64.0, 100, "vector"), generate_ts(64.0, 100, "scalar")
+            )
+            pyrf.cross(
+                generate_ts(64.0, 100, "scalar"), generate_ts(64.0, 100, "vector")
+            )
+
+    def test_cross_output(self):
+        result = pyrf.cross(
+            generate_ts(64.0, 100, "vector"), generate_ts(64.0, 100, "vector")
+        )
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
+
+        result = pyrf.cross(
+            generate_ts(64.0, 100, "vector"), generate_ts(64.0, 97, "vector")
+        )
+        self.assertIsInstance(result, xr.DataArray)
+        self.assertListEqual(list(result.shape), [100, 3])
+
+
+@ddt
+class DateStrTestCase(unittest.TestCase):
+    def test_date_str_input(self):
+        with self.assertRaises(AssertionError):
+            pyrf.date_str("2019-01-01T00:00:00")
+            pyrf.date_str([np.datetime64("2019-01-01T00:00:00"), "2019-01-01T00:10:00"])
+            pyrf.date_str(["2019-01-01T00:00:00", "2019-01-01T00:10:00"], 1)
+
+            tint = ["2019-01-01T00:00:00.000000000", "2019-01-01T00:10:00.000000000"]
+            pyrf.date_str(tint, 0)
+            pyrf.date_str(tint, 5)
+
+    @idata(range(1, 5))
+    def test_date_str_output(self, value):
+        tint = ["2019-01-01T00:00:00.000000000", "2019-01-01T00:10:00.000000000"]
+        result = pyrf.date_str(tint, value)
+        self.assertIsInstance(result, str)
+
+
 class Datetime2Iso8601TestCase(unittest.TestCase):
     def test_datetime2iso8601_input_type(self):
         ref_time = datetime.datetime(2019, 1, 1, 0, 0, 0, 0)
         time_line = [ref_time + datetime.timedelta(seconds=i) for i in range(10)]
         self.assertIsNotNone(pyrf.datetime2iso8601(ref_time))
         self.assertIsNotNone(pyrf.datetime2iso8601(time_line))
 
@@ -522,66 +686,305 @@
             list(result.shape),
             [
                 100,
             ],
         )
 
 
-class Avg4SCTestCase(unittest.TestCase):
-    def test_avg_4sc_input(self):
-        self.assertIsNotNone(
-            pyrf.avg_4sc(
-                [
-                    generate_ts(64.0, 100, "scalar"),
-                    generate_ts(64.0, 100, "scalar"),
-                    generate_ts(64.0, 100, "scalar"),
-                    generate_ts(64.0, 100, "scalar"),
-                ]
+@ddt
+class ShockNormalTestCase(unittest.TestCase):
+    def test_shock_normal_input(self):
+        with self.assertRaises(AssertionError):
+            pyrf.shock_normal([])
+
+        with self.assertRaises(TypeError):
+            pyrf.shock_normal(
+                {
+                    "b_u": np.random.random((3)),
+                    "b_d": np.random.random((3)),
+                    "v_u": np.random.random((3)),
+                    "v_d": np.random.random((3)),
+                    "n_u": random.random(),
+                    "n_d": random.random(),
+                    "r_xyz": random.random(),
+                }
             )
+
+    @data(
+        {
+            "b_u": np.random.random((3)),
+            "b_d": np.random.random((3)),
+            "v_u": np.random.random((3)),
+            "v_d": np.random.random((3)),
+            "n_u": random.random(),
+            "n_d": random.random(),
+        },
+        {
+            "b_u": np.random.random((2, 3)),
+            "b_d": np.random.random((2, 3)),
+            "v_u": np.random.random((2, 3)),
+            "v_d": np.random.random((2, 3)),
+            "n_u": np.random.random((2, 1)),
+            "n_d": np.random.random((2, 1)),
+        },
+        {
+            "b_u": np.random.random((3)),
+            "b_d": np.random.random((3)),
+            "v_u": np.random.random((3)),
+            "v_d": np.random.random((3)),
+            "n_u": random.random(),
+            "n_d": random.random(),
+            "r_xyz": np.random.random((3)),
+        },
+        {
+            "b_u": np.random.random((3)),
+            "b_d": np.random.random((3)),
+            "v_u": np.random.random((3)),
+            "v_d": np.random.random((3)),
+            "n_u": random.random(),
+            "n_d": random.random(),
+            "r_xyz": generate_ts(64.0, 100, "vector"),
+        },
+        {
+            "b_u": np.random.random((3)),
+            "b_d": np.random.random((3)),
+            "v_u": np.random.random((3)),
+            "v_d": np.random.random((3)),
+            "n_u": random.random(),
+            "n_d": random.random(),
+            "r_xyz": generate_ts(64.0, 100, "vector"),
+            "d2u": random.choice([-1, 1]),
+            "dt_f": random.random(),
+            "f_cp": random.random(),
+        },
+    )
+    def test_shock_normal_ouput(self, value):
+        result = pyrf.shock_normal(value)
+        self.assertIsInstance(result, dict)
+        self.assertIsInstance(result["v_sh"], dict)
+
+
+class StartTestCase(unittest.TestCase):
+    def test_start_input_type(self):
+        self.assertIsNotNone(pyrf.start(generate_ts(64.0, 100, "scalar")))
+        self.assertIsNotNone(pyrf.start(generate_ts(64.0, 100, "vector")))
+        self.assertIsNotNone(pyrf.start(generate_ts(64.0, 100, "tensor")))
+
+        with self.assertRaises(AssertionError):
+            pyrf.start(0)
+            pyrf.start(generate_timeline(64.0, 100))
+
+    def test_start_output(self):
+        result = pyrf.start(generate_ts(64.0, 100, "scalar"))
+        self.assertIsInstance(result, np.float64)
+        self.assertEqual(
+            np.datetime64(int(result * 1e9), "ns"),
+            np.datetime64("2019-01-01T00:00:00.000"),
         )
-        self.assertIsNotNone(
-            pyrf.avg_4sc(
-                [
-                    generate_ts(64.0, 100, "vector"),
-                    generate_ts(64.0, 100, "vector"),
-                    generate_ts(64.0, 100, "vector"),
-                    generate_ts(64.0, 100, "vector"),
-                ]
-            )
+
+
+class TsSkymapTestCase(unittest.TestCase):
+    def test_ts_skymap_input_type(self):
+        with self.assertRaises(AssertionError):
+            pyrf.ts_skymap(0, 0, 0, 0, 0)
+
+    def test_ts_skymap_output_type(self):
+        result = pyrf.ts_skymap(
+            generate_timeline(64.0, 100),
+            np.random.random((100, 32, 32, 16)),
+            np.random.random((100, 32)),
+            np.random.random((100, 32)),
+            np.random.random(16),
         )
-        self.assertIsNotNone(
-            pyrf.avg_4sc(
-                [
-                    generate_ts(64.0, 100, "tensor"),
-                    generate_ts(64.0, 100, "tensor"),
-                    generate_ts(64.0, 100, "tensor"),
-                    generate_ts(64.0, 100, "tensor"),
-                ]
+        self.assertIsInstance(result, xr.Dataset)
+
+    def test_ts_skymap_output_shape(self):
+        result = pyrf.ts_skymap(
+            generate_timeline(64.0, 100),
+            np.random.random((100, 32, 32, 16)),
+            np.random.random((100, 32)),
+            np.random.random((100, 32)),
+            np.random.random(16),
+        )
+        self.assertEqual(result.data.ndim, 4)
+        self.assertListEqual(list(result.data.shape), [100, 32, 32, 16])
+        self.assertEqual(result.energy.ndim, 2)
+        self.assertListEqual(list(result.energy.shape), [100, 32])
+        self.assertEqual(result.phi.ndim, 2)
+        self.assertListEqual(list(result.phi.shape), [100, 32])
+        self.assertEqual(result.theta.ndim, 1)
+        self.assertListEqual(list(result.theta.shape), [16])
+
+    def test_ts_skymap_output_meta(self):
+        result = pyrf.ts_skymap(
+            generate_timeline(64.0, 100),
+            np.random.random((100, 32, 32, 16)),
+            np.random.random((100, 32)),
+            np.random.random((100, 32)),
+            np.random.random(16),
+        )
+        self.assertListEqual(
+            list(result.attrs.keys()), ["energy0", "energy1", "esteptable"]
+        )
+        self.assertListEqual(
+            list(result.attrs["energy0"].shape),
+            [
+                32,
+            ],
+        )
+        self.assertListEqual(
+            list(result.attrs["energy1"].shape),
+            [
+                32,
+            ],
+        )
+        self.assertListEqual(
+            list(result.attrs["esteptable"].shape),
+            [
+                100,
+            ],
+        )
+
+        for k in result:
+            self.assertEqual(result[k].attrs, {})
+
+
+class TsScalarTestCase(unittest.TestCase):
+    def test_ts_scalar_input_type(self):
+        with self.assertRaises(AssertionError):
+            pyrf.ts_scalar(0, 0)
+            pyrf.ts_scalar(
+                list(generate_timeline(64.0, 100)), list(generate_data(100, "scalar"))
             )
+
+    def test_ts_scalar_input_shape(self):
+        with self.assertRaises(AssertionError):
+            # Raises error if data and timeline don't have the same size
+            pyrf.ts_scalar(generate_timeline(64.0, 100), generate_data(99, "scalar"))
+            # Raises error if vector as input
+            pyrf.ts_scalar(generate_timeline(64.0, 100), generate_data(100, "vector"))
+            # Raises error if tensor as input
+            pyrf.ts_scalar(generate_timeline(64.0, 100), generate_data(100, "tensor"))
+
+    def test_ts_scalar_output_type(self):
+        result = pyrf.ts_scalar(
+            generate_timeline(64.0, 100), generate_data(100, "scalar")
         )
+        self.assertIsInstance(result, xr.DataArray)
 
-        with self.assertRaises(TypeError):
-            pyrf.avg_4sc(
-                [
-                    generate_data(100, "tensor"),
-                    generate_data(100, "tensor"),
-                    generate_data(100, "tensor"),
-                    generate_data(100, "tensor"),
-                ]
+    def test_ts_scalar_output_shape(self):
+        result = pyrf.ts_scalar(
+            generate_timeline(64.0, 100), generate_data(100, "scalar")
+        )
+        self.assertEqual(result.ndim, 1)
+        self.assertEqual(len(result), 100)
+
+    def test_ts_scalar_dims(self):
+        result = pyrf.ts_scalar(
+            generate_timeline(64.0, 100), generate_data(100, "scalar")
+        )
+        self.assertListEqual(list(result.dims), ["time"])
+
+    def test_ts_scalar_meta(self):
+        result = pyrf.ts_scalar(
+            generate_timeline(64.0, 100), generate_data(100, "scalar")
+        )
+        self.assertEqual(result.attrs["TENSOR_ORDER"], 0)
+
+
+class TsVecXYZTestCase(unittest.TestCase):
+    def test_ts_vec_xyz_input_type(self):
+        with self.assertRaises(AssertionError):
+            pyrf.ts_vec_xyz(0, 0)
+            pyrf.ts_vec_xyz(
+                list(generate_timeline(64.0, 100)), list(generate_data(100, "vector"))
             )
 
-    def test_avg_4sc_output(self):
-        result = pyrf.avg_4sc(
-            [
-                generate_ts(64.0, 100, "tensor"),
-                generate_ts(64.0, 100, "tensor"),
-                generate_ts(64.0, 100, "tensor"),
-                generate_ts(64.0, 100, "tensor"),
-            ]
+    def test_ts_vec_xyz_input_shape(self):
+        with self.assertRaises(AssertionError):
+            # Raises error if data and timeline don't have the same size
+            pyrf.ts_vec_xyz(generate_timeline(64.0, 100), generate_data(99, "vector"))
+            # Raises error if vector as input
+            pyrf.ts_vec_xyz(generate_timeline(64.0, 100), generate_data(100, "scalar"))
+            # Raises error if tensor as input
+            pyrf.ts_vec_xyz(generate_timeline(64.0, 100), generate_data(100, "tensor"))
+
+    def test_ts_vec_xyz_output_type(self):
+        result = pyrf.ts_vec_xyz(
+            generate_timeline(64.0, 100), generate_data(100, "vector")
+        )
+        self.assertIsInstance(result, xr.DataArray)
+
+    def test_ts_vec_xyz_output_shape(self):
+        result = pyrf.ts_vec_xyz(
+            generate_timeline(64.0, 100), generate_data(100, "vector")
         )
+        self.assertEqual(result.ndim, 2)
+        self.assertEqual(result.shape[0], 100)
+        self.assertEqual(result.shape[1], 3)
+
+    def test_ts_vec_xyz_dims(self):
+        result = pyrf.ts_vec_xyz(
+            generate_timeline(64.0, 100), generate_data(100, "vector")
+        )
+        self.assertListEqual(list(result.dims), ["time", "comp"])
+
+    def test_ts_vec_xyz_meta(self):
+        result = pyrf.ts_vec_xyz(
+            generate_timeline(64.0, 100), generate_data(100, "vector")
+        )
+        self.assertEqual(result.attrs["TENSOR_ORDER"], 1)
+
+
+class TsTensorXYZTestCase(unittest.TestCase):
+    def test_ts_tensor_xyz_input_type(self):
+        with self.assertRaises(AssertionError):
+            pyrf.ts_tensor_xyz(0, 0)
+            pyrf.ts_tensor_xyz(
+                list(generate_timeline(64.0, 100)), list(generate_data(100, "tensor"))
+            )
+
+    def test_ts_tensor_xyz_input_shape(self):
+        with self.assertRaises(AssertionError):
+            # Raises error if data and timeline don't have the same size
+            pyrf.ts_tensor_xyz(
+                generate_timeline(64.0, 100), generate_data(99, "tensor")
+            )
+            # Raises error if vector as input
+            pyrf.ts_tensor_xyz(
+                generate_timeline(64.0, 100), generate_data(100, "scalar")
+            )
+            # Raises error if tensor as input
+            pyrf.ts_tensor_xyz(
+                generate_timeline(64.0, 100), generate_data(100, "vector")
+            )
 
+    def test_ts_tensor_xyz_output_type(self):
+        result = pyrf.ts_tensor_xyz(
+            generate_timeline(64.0, 100), generate_data(100, "tensor")
+        )
         self.assertIsInstance(result, xr.DataArray)
-        self.assertListEqual(list(result.shape), [100, 3, 3])
+
+    def test_ts_tensor_xyz_output_shape(self):
+        result = pyrf.ts_tensor_xyz(
+            generate_timeline(64.0, 100), generate_data(100, "tensor")
+        )
+        self.assertEqual(result.ndim, 3)
+        self.assertEqual(result.shape[0], 100)
+        self.assertEqual(result.shape[1], 3)
+        self.assertEqual(result.shape[2], 3)
+
+    def test_ts_tensor_xyz_dims(self):
+        result = pyrf.ts_tensor_xyz(
+            generate_timeline(64.0, 100), generate_data(100, "tensor")
+        )
+        self.assertListEqual(list(result.dims), ["time", "comp_h", "comp_v"])
+
+    def test_ts_tensor_xyz_meta(self):
+        result = pyrf.ts_tensor_xyz(
+            generate_timeline(64.0, 100), generate_data(100, "tensor")
+        )
+        self.assertEqual(result.attrs["TENSOR_ORDER"], 2)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `pyrfu-2.4.4/pyrfu.egg-info/PKG-INFO` & `pyrfu-2.4.5/pyrfu.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfu
-Version: 2.4.4
+Version: 2.4.5
 Summary: Python Space Physics (RymdFysik) Utilities
 Author-email: Louis RICHARD <louir@irfu.se>
 License: 
         MIT License
         
         Copyright (c) 2020 L. RICHARD
         
@@ -37,15 +37,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft
 Classifier: Operating System :: Microsoft :: MS-DOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
@@ -76,16 +75,16 @@
 
 .. |Status| image:: https://img.shields.io/pypi/status/pyrfu?logo=pypi&color=blue
 .. _Status: https://pypi.org/project/pyrfu/
 
 .. |Downloads| image:: https://img.shields.io/pypi/dm/pyrfu?logo=pypi&color=blue
 .. _Downloads: https://pypi.org/project/pyrfu/
 
-.. |Flake8| image:: https://github.com/louis-richard/irfu-python/actions/workflows/flake8.yml/badge.svg
-.. _Flake8: https://github.com/louis-richard/irfu-python/actions/workflows/flake8.yml
+.. |CI| image:: https://github.com/louis-richard/irfu-python/actions/workflows/tests.yml/badge.svg
+.. _CI: https://github.com/louis-richard/irfu-python/actions/workflows/tests.yml
 
 .. |PyLintB| image:: https://github.com/louis-richard/irfu-python/actions/workflows/pylint.yml/badge.svg
 .. _PyLintB: https://github.com/louis-richard/irfu-python/actions/workflows/pylint.yml
 
 .. |Issues| image:: https://img.shields.io/github/issues/louis-richard/irfu-python?logo=github&color=9cf
 .. _Issues: https://github.com/louis-richard/irfu-python/issues
 
@@ -97,176 +96,100 @@
 
 .. |Gitter| image:: https://img.shields.io/gitter/room/louis-richard/pyrfu?logo=gitter&color=orange
 .. _Gitter: https://gitter.im/pyrfu
 
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
 .. _Black: https://github.com/psf/black
 
-|License|_ |Python|_ |PyPi|_ |Format|_ |Wheel|_ |Status|_ |Downloads|_ |Flake8|_ |PyLintB|_ |Issues|_ |Commits|_ |Readthedocs|_ |Gitter|_ |Black|_
+|License|_ |Python|_ |PyPi|_ |Format|_ |Wheel|_ |Status|_ |Downloads|_ |CI|_
+|PyLintB|_ |Issues|_ |Commits|_ |Readthedocs|_ |Gitter|_ |Black|_
 
 The Python package ``pyrfu`` is a software based on the IRFU-MATLAB library to work with space data, particularly the
 Magnetospheric MultiScale (MMS) mission.
 
 It is distributed under the open-source MIT license.
 
 .. end-marker-intro-do-not-remove
 
 Full documentation can be found `here <https://pyrfu.readthedocs.io>`_
 
 
-Installation
-------------
-.. start-marker-install-do-not-remove
+Quickstart
+==========
 
-The package ``pyrfu`` has been tested only for Mac OS.
+Installing pyrfu with pip (`more details here`_):
 
-Using PyPi
-**********
+.. _more details here: https://pyrfu.readthedocs.io/en/latest/installation.html
 
-``pyrfu`` is available for pip.
+.. code-block:: console
 
-.. code-block:: bash
+    $ python -m pip install pyrfu
+    # or
+    $ python -m pip install --user pyrfu
 
-        pip install pyrfu
+Import `pyrfu.mms`_ package with routines specific to work with the
+Magnetospheric Multiscale mission (MMS)
 
+.. _pyrfu.mms: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.mms.html
 
-From sources
-************
-
-The sources are located on **GitHub**:
-
-    https://github.com/louis-richard/irfu-python
-
-1) Clone the GitHub repo:
-
-Open a terminal and write the below command to clone in your PC the ``pyrfu`` repo:
-
-.. code-block:: bash
-
-    git clone https://github.com/louis-richard/irfu-python.git
-    cd irfu-python
-
-
-2) Create a virtual env
-
-pyrfu needs a significant number of dependencies. The easiest
-way to get everything installed is to use a virtual environment.
-
--  Anaconda
-
-You can create a virtual environment and install all the dependencies using conda_
-with the following commands:
-
-.. code-block:: bash
-
-    pip install conda
-    conda create -n pyrfu
-    source activate pyrfu
-
-.. _conda: http://conda.io/
-
-
-- Virtual Env
-
-Virtualenv_ can also be used:
-
-.. code-block:: bash
-
-    pip install virtualenv
-    virtualenv pyrfu
-    source pyrfu/bin/activate
-
-.. _virtualenv: https://virtualenv.pypa.io/en/latest/#
-
-
-3) Install the package via the commands:
-
-.. code-block:: bash
-
-        python setup.py install
-
-
-5) (Optional) Generate the docs: install the extra dependencies of doc and run
-the `setup.py` file:
-
-.. code-block:: bash
-
-        pip install pyrfu
-        python setup.py build_sphinx
-
-Once installed, the doc can be generated with:
-
-.. code-block:: bash
-
-        cd doc
-        make html
-
-
-Dependencies
-************
+.. code:: python
 
-The required dependencies are:
+    from pyrfu import mms
 
-- `cdflib <https://cdflib.readthedocs.io/en/latest/?badge=latest>`_ >=1.0.0
-- `geopack <https://github.com/tsssss/geopack>`_ >=1.0.9
-- `matplotlib <https://matplotlib.org>`_ >=3.5.2
-- `numba <http://numba.pydata.org>`_ >=0.54.1
-- `numpy <https://www.numpy.org>`_ >=1.20.3
-- `pandas <https://pandas.pydata.org/>`_ >=1.3.4
-- `python-datetutil <https://dateutil.readthedocs.io/en/stable/>`_ >=2.8.2
-- `requests <https://requests.readthedocs.io/en/latest/>`_ >=2.26.0
-- `scipy <https://scipy.org>`_ >=1.7.3
-- `tqdm <https://tqdm.github.io/>`_ >=4.62.3
-- `xarray <https://xarray.pydata.org/en/stable/>`_ >=0.20.1
+Setup path to MMS data
 
+.. code:: python
 
-Testing dependencies are:
+    mms.db_init("/Volumes/mms")
 
-- `pytest <https://docs.pytest.org/en/latest/>`_ >= 2.8
+Load magnetic field and ion bulk velocity data
 
-Extra testing dependencies:
+.. code:: python
 
-- `coverage <https://coverage.readthedocs.io>`_ >= 4.4
-- `pylint <https://www.pylint.org>`_ >= 1.6.0
+    tint = ["2019-09-14T07:54:00.000", "2019-09-14T08:11:00.000"]
+    b_gsm = mms.get_data("b_gsm_fgm_srvy_l2", tint, 1)
+    v_gse_i = mms.get_data("vi_gse_fpi_fast_l2", tint, 1)
 
-.. end-marker-install-do-not-remove
+Import `pyrfu.pyrf`_ package with generic routines
 
-Usage
------
-To import generic space plasma physics functions
+.. _pyrfu.pyrf: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.pyrf.html
 
 .. code:: python
 
     from pyrfu import pyrf
 
-
-To import functions specific to Magnetospheric Multi-Scale (MMS)
+Transform ion bulk velocity to geocentric solar magnetospheric (GSM) coordinates
 
 .. code:: python
 
-    from pyrfu import mms
+    v_gsm_i = pyrf.cotrans(v_gse_i, "gse>gsm")
 
+Import `pyrfu.plot`_ package with plotting routines
 
-To import functions specific to Solar Orbiter (SolO)
+.. _pyrfu.plot: https://pyrfu.readthedocs.io/en/latest/dev/pyrfu.plot.html
 
 .. code:: python
 
-    from pyrfu import solo
-
+    from pyrfu import plot
 
-To import plotting functions
+Plot time series of magnetic field and ion bulk velocity
 
 .. code:: python
 
-    from pyrfu import plot
+    import matplotlib.pyplot as plt
 
+    f, axs = plt.subplots(2, sharex="all")
+    plot.plot_line(axs[0], b_gsm)
+    axs[0].set_ylabel("$B~[\\mathrm{nT}]$")
+    axs[0].legend(["$B_{x}$", "$B_{y}$", "$B_{z}$"], ncol=4)
+
+    plot.plot_line(axs[1], v_gsm_i)
+    axs[1].set_ylabel("$V_i~[\\mathrm{km}~\\mathrm{s}^{-1}]$")
+    axs[1].legend(["$V_{ix}$", "$V_{iy}$", "$V_{iz}$"], ncol=4)
 
-Configuration
--------------
-Default configuration settings for MMS data (i.e data path) are stored in pyrfu/mms/config.json and can be changed at anytime using mms.db_init(local_path_dir).
 
 Credits
 -------
 This software was developed by Louis RICHARD (louisr@irfu.se) based on the IRFU-MATLAB library.
 
 Acknowledgement
 ---------------
```

### Comparing `pyrfu-2.4.4/pyrfu.egg-info/SOURCES.txt` & `pyrfu-2.4.5/pyrfu.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,18 @@
-.flake8
-.gitignore
-.pre-commit-config.yaml
-CONTRIBUTING.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 pyproject.toml
-requirements.txt
-.github/workflows/flake8.yml
-.github/workflows/publish-to-pypi.yml
-.github/workflows/pylint.yml
-.idea/aws.xml
-.idea/vcs (LAPTOP-E2ISLACJ's conflicted copy 2022-09-29).xml
-.idea/vcs.xml
-.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml
-.idea/codeStyles/codeStyleConfig.xml
-.idea/inspectionProfiles/Project_Default.xml
-.idea/inspectionProfiles/profiles_settings.xml
-docs/Makefile
 docs/conf.py
 pyrfu/__init__.py
 pyrfu.egg-info/PKG-INFO
 pyrfu.egg-info/SOURCES.txt
 pyrfu.egg-info/dependency_links.txt
 pyrfu.egg-info/requires.txt
 pyrfu.egg-info/top_level.txt
-pyrfu/__pycache__/__init__.cpython-38.pyc
 pyrfu/dispersion/__init__.py
 pyrfu/dispersion/disp_surf_calc.py
 pyrfu/dispersion/one_fluid_dispersion.py
 pyrfu/lp/__init__.py
 pyrfu/lp/photo_current.py
 pyrfu/lp/thermal_current.py
 pyrfu/mms/__init__.py
@@ -260,15 +243,14 @@
 pyrfu/pyrf/sph2cart.py
 pyrfu/pyrf/st_diff.py
 pyrfu/pyrf/start.py
 pyrfu/pyrf/struct_func.py
 pyrfu/pyrf/t_eval.py
 pyrfu/pyrf/time_clip.py
 pyrfu/pyrf/timevec2iso8601.py
-pyrfu/pyrf/timing_gui.py
 pyrfu/pyrf/trace.py
 pyrfu/pyrf/transformation_indices.json
 pyrfu/pyrf/ts_append.py
 pyrfu/pyrf/ts_scalar.py
 pyrfu/pyrf/ts_skymap.py
 pyrfu/pyrf/ts_tensor_xyz.py
 pyrfu/pyrf/ts_time.py
@@ -282,9 +264,9 @@
 pyrfu/pyrf/waverage.py
 pyrfu/solo/__init__.py
 pyrfu/solo/config.json
 pyrfu/solo/db_init.py
 pyrfu/solo/read_lfr_density.py
 pyrfu/solo/read_tnr.py
 pyrfu/tests/__init__.py
-pyrfu/tests/test_pyrf.py
-venv/bin/activate_this.py
+pyrfu/tests/test_dispersion.py
+pyrfu/tests/test_pyrf.py
```

