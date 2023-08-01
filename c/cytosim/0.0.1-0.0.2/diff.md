# Comparing `tmp/cytosim-0.0.1.tar.gz` & `tmp/cytosim-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytosim-0.0.1.tar", last modified: Thu Dec 15 12:46:04 2022, max compression
+gzip compressed data, was "cytosim-0.0.2.tar", last modified: Tue Aug  1 12:28:32 2023, max compression
```

## Comparing `cytosim-0.0.1.tar` & `cytosim-0.0.2.tar`

### file list

```diff
@@ -1,976 +1,978 @@
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.262243 cytosim-0.0.1/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      722 2022-11-30 15:33:17.000000 cytosim-0.0.1/.gitignore
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4328 2022-12-15 10:33:50.000000 cytosim-0.0.1/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    35147 2022-11-30 15:33:17.000000 cytosim-0.0.1/LICENSE.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4031 2022-12-15 12:46:04.262243 cytosim-0.0.1/PKG-INFO
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3576 2022-11-30 15:33:17.000000 cytosim-0.0.1/PYCYTOSIM.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3735 2022-11-30 15:33:17.000000 cytosim-0.0.1/README.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1258 2022-11-30 15:33:17.000000 cytosim-0.0.1/WARRANTY.txt
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.214243 cytosim-0.0.1/cym/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      514 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/actin.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/amplify.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1218 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/arp23.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3330 2022-12-13 08:16:55.000000 cytosim-0.0.1/cym/ashbya.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      614 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/aster.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1172 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/aster_couple.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1127 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/aster_custom.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/aster_dynamic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1897 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/aster_france.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      759 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/aster_guided.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      884 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/aster_pull.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1347 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/aster_pull3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      913 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/aster_texas.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1108 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/aster_tracker.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/axon.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1374 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/axon.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1399 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/baseball.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      897 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/bead.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1793 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/bipolar.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      858 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/buckling.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      839 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/buckling.cym.tpl
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1613 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/capture.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2274 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/capture_amplified.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      856 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/catastrophe_outside.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1228 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/celegans.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1385 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/change.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      563 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/change_confine.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      752 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/change_space.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      873 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/confine_instability.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      983 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/contract.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/contract_always.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1250 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/contract_anchored.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1322 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/contract_clamped.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1222 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/contract_connect.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1135 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/contract_periodic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1857 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/cortex.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      891 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/couple.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3110 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/couple_fork.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1140 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/crushed_shell.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1107 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/cut_aster.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      922 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/cut_fibers.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      954 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/cut_planar.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1233 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/cut_saved.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3683 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/cytokinesis.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      869 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/cytoplasmic_flow.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1266 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/dogic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3225 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/endocytosis.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2103 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/endocytosis.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9924 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/entangled.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1459 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/event.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      945 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fast_diffusion1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      951 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fast_diffusion2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      353 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fiber.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1203 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fiber_anchor.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      527 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fiber_athermal.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      837 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fiber_bent.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      615 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fiber_buckle.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      998 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fiber_classic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      834 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fiber_dynamic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      625 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fiber_forces.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1365 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fiber_glue.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      601 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fiber_grow.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1728 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fiber_mixed.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1329 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fiber_omega.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      847 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fiber_treadmill.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      868 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/field.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      715 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/field_bind.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      637 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/field_cut.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      703 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/fountain.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    24264 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/france.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      643 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/frap.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1277 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/friction.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      968 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1009 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_arcs.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_collect.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1680 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_drag.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1522 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_east.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1353 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_flip.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1959 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_flip_track.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1404 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_flippers.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1770 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_gate.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1126 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_path.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1334 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_ratchet.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1686 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_sort.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1898 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_sort_ortho.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1654 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_sorter.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1349 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_spiral.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_steric.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1369 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_stripe.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1245 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_surface.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      901 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_texas.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2023 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_trap.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1547 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_west.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1624 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_west_blur.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1675 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/glide_yingyang.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1347 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/granules.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1274 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/hand_chew.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      987 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/hand_cut.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1640 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/hand_digit.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      828 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/hand_move.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      861 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/hand_nucleate.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      984 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/hand_rescue.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1330 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/hand_slide.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1025 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/hand_track.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2408 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/hand_walk.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3579 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/lacroix.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1053 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/magic_key.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      672 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/microtubule.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1760 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/minifilaments.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1850 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/minifilaments1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1605 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/minifilaments2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1509 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/motif.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1554 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/motif_blur.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1132 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/motile_bead.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1145 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/motor_pull.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1006 2022-11-30 15:36:20.000000 cytosim-0.0.1/cym/move.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2376 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/muscle.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      972 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/muscle_smooth.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1059 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/needles.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/nematic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      663 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/nucleate.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      842 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/nucleate_edge.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1106 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/nucleus.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1249 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/overlap.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1411 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/overlap3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2044 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/overlap3D_16.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1362 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/overlap_walk.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      458 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/packed_beads.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      459 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/packed_beads_2D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1326 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/packed_gel.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1364 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/placement.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1356 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/pombe.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1528 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/pombe_classic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1724 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/pombe_meiotic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1311 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/push_pull.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1142 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/radial.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1124 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/ring_motors.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1066 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/self.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1012 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/self_cortex.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      754 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/self_vortex.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1086 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/self_walk.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      764 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/side_movement.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      658 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/single.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1348 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/smiley.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1387 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/solid.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      499 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/solid_3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      690 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/space_axisymmetric.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      597 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/space_ellipse.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1122 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/sphere.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1097 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/spider.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2417 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/spindle3.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3712 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/spindle_celegans.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1601 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/spindle_centering.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1585 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/spindle_centering_dynamic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2199 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/spindle_compression.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3423 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/spindle_pombe.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    25433 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/spindle_pombe_em.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    31549 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/spindle_pombe_em1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7568 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/spindle_yeast.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      676 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/spiral.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      977 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/spool.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1068 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1080 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      640 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_artefact.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      649 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_bead_fiber_periodic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      460 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_bead_periodic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      399 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_bead_periodic2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      940 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_bundle.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1243 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_bundling.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      667 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_cylinder.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      857 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_fiber.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      535 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_fiber1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      846 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_fiber_3D.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      654 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_fiber_periodic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      795 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_sphere.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1910 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/steric_test.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      957 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/swimmers.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      841 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/test_binding1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1077 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/test_binding2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1262 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/test_binding3.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      735 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/test_bindingP.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      439 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/test_fiber_diffusion.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      419 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/test_single_diffusion.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      550 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/texas.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      794 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/toy.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      906 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/toy_start.cmi
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      892 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/transport.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1035 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/triangle.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1591 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/tug_of_war.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1485 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/walkers.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1137 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/wash.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1322 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/yossi.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1407 2022-11-30 15:33:18.000000 cytosim-0.0.1/cym/zigzag.cym
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.214243 cytosim-0.0.1/cytosim.xcodeproj/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   335772 2022-11-30 15:36:20.000000 cytosim-0.0.1/cytosim.xcodeproj/project.pbxproj
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.202242 cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.214243 cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3081 2022-11-30 15:33:18.000000 cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/play.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2846 2022-11-30 15:33:18.000000 cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/report.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2828 2022-11-30 15:33:18.000000 cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/sim.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2022-11-30 15:33:18.000000 cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/test_code.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2022-11-30 15:33:18.000000 cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/test_grid.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2876 2022-11-30 15:33:18.000000 cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/test_matrix.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2022-11-30 15:33:18.000000 cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/test_simd.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2377 2022-11-30 15:33:18.000000 cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/tests.xcscheme
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   290228 2022-11-30 15:33:17.000000 cytosim-0.0.1/demo_cythosim.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    90637 2022-11-30 15:33:17.000000 cytosim-0.0.1/demo_frame.ipynb
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.214243 cytosim-0.0.1/doc/
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.214243 cytosim-0.0.1/doc/code/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   106956 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/code/doxygen.cfg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      652 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/code/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5727 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/code/layout.xml
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      881 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/code/mainpage.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4859 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/code/objects.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.218243 cytosim-0.0.1/doc/compile/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4678 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/compile/cygwin.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      931 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/compile/dimensionality.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6519 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/compile/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1459 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/compile/intel_mkl.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      845 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/compile/linux.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1663 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/compile/multithreading.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1361 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/compile/options.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2371 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/compile/vectorization.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.218243 cytosim-0.0.1/doc/cpython/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28284 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/cpython/cpython.css
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5804 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/cpython/cpython_doc.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    90331 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/cpython/doc_PyCytoplay.html
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    90339 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/cpython/doc_PyCytosim.html
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9278 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/cpython/read_cpython.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.218243 cytosim-0.0.1/doc/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   123267 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/data/cytosim.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29497 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/data/modularity.png
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.218243 cytosim-0.0.1/doc/examples/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6671 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/biblio.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.218243 cytosim-0.0.1/doc/examples/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    33685 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/data/actin.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    42409 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/data/ashbya.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    30331 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/data/celegans.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    60174 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/data/centering.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    65951 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/data/droplets.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    50739 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/data/endocytosis.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    97182 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/data/minifilaments.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    77302 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/data/nematics.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   100226 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/data/network.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5254 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/data/patterns.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   110273 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/data/spindle.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    51623 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/data/spindle_length.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16497 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/data/spombe.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2240 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/examples/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1813 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/index.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.222243 cytosim-0.0.1/doc/main/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      404 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/main/cheat.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/main/credits.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1776 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/main/examples.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5237 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/main/executables.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57247 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/main/faq.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1711 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/main/file_types.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3256 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/main/movies.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3969 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/main/overview.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5837 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/main/run_slurm.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7840 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/main/runs.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3784 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/main/starter.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.222243 cytosim-0.0.1/doc/misc/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4057 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/misc/Cytosim.tmbundle.zip
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.222243 cytosim-0.0.1/doc/outreach/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1717 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/outreach/controller.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.222243 cytosim-0.0.1/doc/outreach/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57904 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/outreach/data/CRI-2018-11a.jpg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    39021 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/outreach/data/CRI-2018-11b.jpg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   102453 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/outreach/data/Cambridge-2019-05a.jpg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    61861 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/outreach/data/Cambridge-2019-05b.jpg
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.222243 cytosim-0.0.1/doc/outreach/games/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      643 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/outreach/games/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      198 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/outreach/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6378 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/outreach/installation1.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5304 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/outreach/installation2.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.222243 cytosim-0.0.1/doc/rendering/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)  1462588 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/rendering/actin.blend
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4264 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/rendering/import-actin-ico.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4207 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/rendering/import-actin-sphere.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4207 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/rendering/import-actin.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4413 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/rendering/import-links.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4086 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/rendering/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      292 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/rendering/remove-actin.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.222243 cytosim-0.0.1/doc/sim/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12156 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/commands.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2675 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/config.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.226243 cytosim-0.0.1/doc/sim/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      928 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/data/forces.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6040 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/data/forces.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28232 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/data/meca_links.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3284 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/data/steric.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      263 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/data/steric.tex
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21888 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/data/steric3D.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11926 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/data/steric_math.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    65261 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/data/varying_time_step.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9082 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/fiber_dynamics.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1679 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/fibers.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1283 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/forces.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2513 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/graphics.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      611 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1527 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/motor_detachment.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3731 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/numerical_precision.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4246 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/objects.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       85 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/parameters.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8951 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/placement.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6988 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/report.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2687 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/spaces.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3458 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/steric.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3473 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/stochastic.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1882 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/sim/units.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.226243 cytosim-0.0.1/doc/tutorials/
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.226243 cytosim-0.0.1/doc/tutorials/code/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4790 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/code/collect.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      649 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/code/config.cym.tpl
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      710 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/code/master.sh
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    15382 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/code/preconfig
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2847 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/code/scan.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.226243 cytosim-0.0.1/doc/tutorials/data/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3334 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/data/ashbya.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      793 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/data/aster.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1234 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/data/aster_dynamic.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4119 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/data/capture.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19449 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/data/end_tracking.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28111 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/data/filament_buckling.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      973 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/data/gliding.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28234 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/data/polarity_sorting.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1010 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/data/self.cym
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.226243 cytosim-0.0.1/doc/tutorials/images/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4591 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/H.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4483 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/XTV.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11568 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/aster-vs-nematic.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19716 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/bind_also_end.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    27299 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/bind_end.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20037 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/couples.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7406 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/crosslinks.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    32919 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/droplets.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12570 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/force_velocity.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3561 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/gliding1.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3617 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/gliding2.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57401 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/kinesin_tetramers.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28232 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/meca_links.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10190 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/images/nematic-vs-polar.png
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1172 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/index.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      227 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_bipolarity.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3031 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_capture.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12562 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_centering.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7861 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_contract2.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5433 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_contract3.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7185 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_contract_motor.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5985 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_gliding.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    23732 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_introduction.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      680 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_nucleus.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14458 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_polar_nematic.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      224 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_polarity.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7287 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_scans.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2543 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_scripting.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11632 2022-11-30 15:33:18.000000 cytosim-0.0.1/doc/tutorials/tuto_self.md
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      356 2022-11-30 15:33:17.000000 cytosim-0.0.1/example.cym
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.226243 cytosim-0.0.1/examples/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      591 2022-11-30 15:33:18.000000 cytosim-0.0.1/examples/avoid.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      622 2022-11-30 15:33:18.000000 cytosim-0.0.1/examples/flock.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5830 2022-11-30 15:33:18.000000 cytosim-0.0.1/examples/pycytoplay_callbacks.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   166542 2022-11-30 15:33:18.000000 cytosim-0.0.1/examples/pycytosim_construct.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   156059 2022-11-30 15:33:18.000000 cytosim-0.0.1/examples/pycytosim_extend.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    81199 2022-11-30 15:33:18.000000 cytosim-0.0.1/examples/pycytosim_flock.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6186 2022-11-30 15:33:18.000000 cytosim-0.0.1/examples/pycytosim_import3D.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    95853 2022-11-30 15:33:18.000000 cytosim-0.0.1/examples/pycytosim_meca.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4720 2022-11-30 15:33:18.000000 cytosim-0.0.1/examples/pycytosim_obj_3D.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   268276 2022-11-30 15:33:18.000000 cytosim-0.0.1/examples/pycytosim_objects.ipynb
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4868 2022-11-30 15:33:17.000000 cytosim-0.0.1/makefile
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12543 2022-11-30 15:33:17.000000 cytosim-0.0.1/makefile.inc
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.202242 cytosim-0.0.1/module/
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.230243 cytosim-0.0.1/module/cytosim.egg-info/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4031 2022-12-15 12:46:04.000000 cytosim-0.0.1/module/cytosim.egg-info/PKG-INFO
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22480 2022-12-15 12:46:04.000000 cytosim-0.0.1/module/cytosim.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2022-12-15 12:46:04.000000 cytosim-0.0.1/module/cytosim.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2022-12-15 12:46:04.000000 cytosim-0.0.1/module/cytosim.egg-info/not-zip-safe
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2022-12-15 12:46:04.000000 cytosim-0.0.1/module/cytosim.egg-info/top_level.txt
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.230243 cytosim-0.0.1/python/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1013 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/index.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.230243 cytosim-0.0.1/python/look/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4550 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/look/collect.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3078 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/look/compare_config.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4391 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/look/get_data.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     5061 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/look/make_image.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    12363 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/look/make_movie.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     7827 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/look/make_page.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3854 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/look/make_plots.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    11898 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/look/read_config.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4262 2022-11-30 15:36:20.000000 cytosim-0.0.1/python/look/scan.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3694 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/look/tell.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.230243 cytosim-0.0.1/python/misc/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2504 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/misc/battery_test.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3487 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/misc/cleanup.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4468 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/misc/compare.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2305 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/misc/plot.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5881 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/misc/pyned.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3187 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/misc/reduce.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.230243 cytosim-0.0.1/python/run/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     6691 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/run/go_sim.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7125 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/run/go_sim_lib.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    23181 2022-11-30 15:36:20.000000 cytosim-0.0.1/python/run/preconfig.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4698 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/run/submit_one.py
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     8716 2022-11-30 15:33:18.000000 cytosim-0.0.1/python/run/submit_slurm.py
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       38 2022-12-15 12:46:04.262243 cytosim-0.0.1/setup.cfg
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2281 2022-12-15 12:45:36.000000 cytosim-0.0.1/setup.py
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.230243 cytosim-0.0.1/src/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      266 2022-12-05 09:16:09.000000 cytosim-0.0.1/src/CMakeLists.txt
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.234243 cytosim-0.0.1/src/base/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      684 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/base/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14150 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/array.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2666 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/assert_macro.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      920 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/backtrace.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      679 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/backtrace.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3957 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/buddy.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      187 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/exceptions.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/exceptions.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3924 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/filepath.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2212 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/filepath.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5785 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/filewrapper.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4167 2022-11-30 15:53:53.000000 cytosim-0.0.1/src/base/filewrapper.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19578 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/glossary.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17191 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/glossary.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1210 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/inventoried.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4977 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/inventory.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3158 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/inventory.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13239 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/iowrapper.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6390 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/iowrapper.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      699 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      796 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/messages.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2738 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/messages.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7638 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/node_list.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3624 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/node_list.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      992 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/noder.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1188 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/operator_new.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2722 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/print_color.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      903 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/print_color.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3195 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/property.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6787 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/property.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6819 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/property_list.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4689 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/property_list.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5957 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/stream_func.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/stream_func.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2607 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/tictoc.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1428 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/tictoc.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1595 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/timer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14894 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/tokenizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3438 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/base/tokenizer.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.234243 cytosim-0.0.1/src/cpython/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4211 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/cpython/couple_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11052 2022-11-30 15:45:38.000000 cytosim-0.0.1/src/cpython/fiber_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1776 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/cpython/glossary_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6000 2022-11-30 15:45:05.000000 cytosim-0.0.1/src/cpython/hand_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7736 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/cpython/meca_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3218 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/cpython/object_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2379 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/cpython/organizer_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2190 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/cpython/point_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6444 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/cpython/python_frame.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3683 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/cpython/python_utilities.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10957 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/cpython/simul_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3692 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/cpython/single_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5459 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/cpython/solid_modules.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3441 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/cpython/space_modules.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.238243 cytosim-0.0.1/src/disp/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      911 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    47659 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/display.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8728 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/display.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12449 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/display1.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1676 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/display1.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17736 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/display2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1847 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/display2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29712 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/display3.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/display3.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2017 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/display_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2782 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/display_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6302 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/fiber_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9479 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/fiber_disp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37956 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/glapp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4858 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/glapp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    72505 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/gle.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19541 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/gle.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9397 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/gle_color.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13816 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/gle_color.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    64657 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/gle_color_list.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/gle_color_list.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5234 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/glu_unproject.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      392 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/glut.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2213 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/grid_display.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/grid_display.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      271 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/line_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1050 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/line_disp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1452 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   320003 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/miniz.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    69441 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/miniz.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/offscreen.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      687 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/offscreen.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8985 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/offscreen_fbo.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3408 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/offscreen_glx.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      381 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/opengl.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5347 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/point_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4369 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/point_disp.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19476 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/save_image.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4502 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/save_image.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   199731 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/spng.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13411 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/disp/spng.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21466 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/view.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7272 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/view.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5976 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/view_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6467 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/disp/view_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      863 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/index.md
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.242243 cytosim-0.0.1/src/math/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      990 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/math/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5979 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/SFMT-avx2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5217 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/SFMT-common.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/SFMT-params.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/SFMT-params19937.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3475 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/SFMT-sse2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12768 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/SFMT.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8298 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/SFMT.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2689 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/accumulator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3670 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/allocator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11058 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/bicgstab.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12965 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/cblas.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11429 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/clapack.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10653 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/dgtsv.c
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      241 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/dim.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4633 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/evaluator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7507 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/gmres.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17756 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/grid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    26300 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/grid_base.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1974 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/isometry.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/linear_operator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1291 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3493 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matrix.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3849 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matrix.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      602 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matrix11.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8691 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matrix11.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      802 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matrix22.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20484 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matrix22.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matrix33.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    31444 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matrix33.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22178 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matrix44.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9356 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matrixbase.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9604 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matsparse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matsparse.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matsparsesym.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3776 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matsparsesym.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28081 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matsparsesym1.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7096 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matsparsesym1.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17374 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matsparsesym2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4448 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matsparsesym2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37068 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matsparsesymblk.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8005 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/matsparsesymblk.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3437 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/monitor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15587 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/platonic.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7558 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/platonic.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9504 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/pointsonsphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4817 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/pointsonsphere.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12314 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/polygon.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3531 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/polygon.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7843 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/project_ellipse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      583 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/project_ellipse.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21773 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/quaternion.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12497 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/random.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10100 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/random.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9782 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/random_vector.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1456 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/random_vector.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    18395 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/rasterizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13234 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/rasterizer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/real.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16193 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/simd.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/simd_print.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9993 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/smath.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6221 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/vecprint.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      854 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/vector.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/vector1.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12908 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/vector1.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      935 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/vector2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16056 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/vector2.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1046 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/vector3.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21674 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/vector3.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1090 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/vector4.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15588 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/math/vector4.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.242243 cytosim-0.0.1/src/misc/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6565 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/check_dump.m
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.242243 cytosim-0.0.1/src/misc/installation/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   111922 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/RtMidi.cpp
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    25736 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/RtMidi.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.242243 cytosim-0.0.1/src/misc/installation/builder/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/builder/0-live.command
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2048 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/builder/config.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2156 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/builder/config0.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2184 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/builder/config1.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1901 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/builder/config2.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/builder/config3.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/builder/config4.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1957 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/builder/config5.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2023 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/builder/config6.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2148 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/builder/config7.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2150 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/builder/config8.cym
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    24264 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/builder/france.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14566 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/cytobuilder.cpp
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12900 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/cytomaster.cpp
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.242243 cytosim-0.0.1/src/misc/installation/cytomaster.xcodeproj/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12175 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/cytomaster.xcodeproj/project.pbxproj
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      859 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/makefile
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.242243 cytosim-0.0.1/src/misc/installation/master/
--rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/master/0-live.command
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      982 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/master/config0.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/master/config1.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      896 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/master/config2.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1176 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/master/config4.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3161 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/master/config6.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2765 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/master/config7.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1509 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/master/config8.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3363 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/master/config9.cym
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    24264 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/master/france.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/rtmidi_c.cpp
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9194 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/misc/installation/rtmidi_c.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.242243 cytosim-0.0.1/src/play/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      675 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/play/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2224 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/play/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12390 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/play/play.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        0 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/play/play.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28066 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/play/play_keys.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15403 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/play/play_menus.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2713 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/play/play_mouse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5535 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/play/player.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4136 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/play/player.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11531 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/play/player_disp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3294 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/play/player_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3170 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/play/player_prop.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.250243 cytosim-0.0.1/src/sim/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4848 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3838 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/bead.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4214 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/bead.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       94 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/bead_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      211 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/bead_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2886 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/bead_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1967 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/bead_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    42390 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/chain.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17478 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/chain.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       92 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/common.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2358 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/common.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10436 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couple.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9433 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couple.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6226 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couple_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7748 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couple_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28765 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couple_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8855 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couple_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.254243 cytosim-0.0.1/src/sim/couples/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1025 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/bridge.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1497 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/bridge.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      912 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/bridge_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1064 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/bridge_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3046 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/couple_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1067 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/couple_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1414 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/crosslink.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      875 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/crosslink.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3132 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/crosslink_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1104 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/crosslink_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1131 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/crosslink_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1167 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/crosslink_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3524 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/duo.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1552 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/duo.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3029 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/duo_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1263 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/duo_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/duo_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1492 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/duo_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      880 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/fork.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      870 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/fork.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1439 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/fork_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1437 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/fork_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      989 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/shackle.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      840 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/shackle.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/shackle_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1128 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/shackle_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      881 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/shackle_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1068 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/couples/shackle_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1637 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/event.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2659 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/event.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1477 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/event_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1391 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/event_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    38151 2022-11-30 15:48:06.000000 cytosim-0.0.1/src/sim/fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11570 2022-11-30 15:48:11.000000 cytosim-0.0.1/src/sim/fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14550 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fiber_grid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fiber_grid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3084 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fiber_grid2.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16723 2022-11-30 15:48:16.000000 cytosim-0.0.1/src/sim/fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10297 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8025 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fiber_segment.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4117 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fiber_segment.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    33092 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/fiber_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6069 2022-11-30 15:48:21.000000 cytosim-0.0.1/src/sim/fiber_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5789 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/fiber_site.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6327 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/fiber_site.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.254243 cytosim-0.0.1/src/sim/fibers/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6943 2022-11-30 15:47:46.000000 cytosim-0.0.1/src/sim/fibers/classic_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3215 2022-11-30 15:47:57.000000 cytosim-0.0.1/src/sim/fibers/classic_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6714 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/classic_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5152 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/classic_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8939 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/dynamic_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4818 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/dynamic_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5287 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/dynamic_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3553 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/dynamic_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4654 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/growing_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3288 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/growing_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2072 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/growing_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3092 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/growing_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4130 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/treadmilling_fiber.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2069 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/treadmilling_fiber.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1712 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/treadmilling_fiber_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1565 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/fibers/treadmilling_fiber_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15391 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/field.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10783 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/field.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4526 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/field_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2922 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/field_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2775 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/field_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/field_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2272 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/field_values.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8960 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/frame_reader.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3468 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/frame_reader.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7681 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/hand.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6775 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hand.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       97 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hand_monitor.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1886 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hand_monitor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11612 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hand_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7663 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hand_prop.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.258243 cytosim-0.0.1/src/sim/hands/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      839 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/actor.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/actor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/actor_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1095 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/actor_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2174 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/chewer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/chewer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2337 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/chewer_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1505 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/chewer_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1578 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/cutter.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1216 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/cutter.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1924 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/cutter_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1458 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/cutter_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4188 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/hands/digit.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3741 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/digit.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1640 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/digit_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/digit_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/dynein.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/dynein.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/dynein_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2024 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/dynein_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1909 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/kinesin.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1096 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/kinesin.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1415 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/kinesin_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1451 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/kinesin_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/mighty.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1045 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/mighty.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4003 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/mighty_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2635 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/mighty_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1924 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/motor.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1434 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/motor.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3705 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/motor_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2406 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/motor_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2002 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/myosin.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/myosin.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/myosin_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1441 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/myosin_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/nucleator.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1685 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/nucleator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3856 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/nucleator_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3290 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/nucleator_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      787 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/regulator.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      987 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/regulator.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/regulator_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1260 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/regulator_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2586 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/rescuer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1687 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/rescuer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      909 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/rescuer_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1471 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/rescuer_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1195 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/slider.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1173 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/slider.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2614 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/slider_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2773 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/slider_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1901 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/tracker.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1269 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/tracker.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1236 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/tracker_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1515 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/tracker_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2873 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/walker.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2115 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/walker.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3951 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/walker_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2079 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/hands/walker_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29823 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/interface.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3513 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/interface.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      950 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/interpolation.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4495 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/interpolation.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4417 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/interpolation4.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/interpolation4.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1530 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/lattice.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15313 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/lattice.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5441 2022-11-30 15:48:27.000000 cytosim-0.0.1/src/sim/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    46323 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/meca.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22556 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/meca.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6075 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/meca1d.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   107544 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/meca_inter.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8873 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/mecable.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14168 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/mecable.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8215 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/mecafil.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4652 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/mecafil.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20053 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/mecafil_project.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5581 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/mecafil_projectmat.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1165 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/mecapoint.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2131 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/mecapoint.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/modulo.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2101 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/modulo.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    30312 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/movable.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2997 2022-11-30 15:49:59.000000 cytosim-0.0.1/src/sim/movable.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6062 2022-11-30 15:50:13.000000 cytosim-0.0.1/src/sim/object.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5322 2022-11-30 15:50:27.000000 cytosim-0.0.1/src/sim/object.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14499 2022-11-30 15:50:54.000000 cytosim-0.0.1/src/sim/object_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6995 2022-11-30 15:51:14.000000 cytosim-0.0.1/src/sim/object_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3689 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3630 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizer.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4025 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizer_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizer_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.258243 cytosim-0.0.1/src/sim/organizers/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21643 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/aster.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7228 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/aster.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1822 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/aster_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2014 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/aster_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4663 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/bundle.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1987 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/bundle.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1632 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/bundle_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1613 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/bundle_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3502 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/fake.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1793 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/fake.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      552 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/fake_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/fake_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4326 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/nucleus.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2312 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/nucleus.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      529 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/nucleus_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/organizers/nucleus_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    32594 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/parser.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3009 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/parser.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20108 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/point_grid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9872 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/point_grid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/sim.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      267 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/sim.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11790 2022-11-30 15:39:23.000000 cytosim-0.0.1/src/sim/sim_thread.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6789 2022-11-30 15:39:23.000000 cytosim-0.0.1/src/sim/sim_thread.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13540 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/simul.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19225 2022-11-30 15:51:23.000000 cytosim-0.0.1/src/sim/simul.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1302 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/simul_custom.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20613 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/simul_file.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5550 2022-11-30 15:51:40.000000 cytosim-0.0.1/src/sim/simul_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11565 2022-11-30 15:51:51.000000 cytosim-0.0.1/src/sim/simul_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    71703 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/simul_report.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14266 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/simul_solve.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4736 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/sim/simul_step.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4179 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/single.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6635 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/single.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6389 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/single_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3918 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/single_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15361 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/single_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5655 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/single_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.258243 cytosim-0.0.1/src/sim/singles/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1397 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/singles/picket.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/singles/picket.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2795 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/singles/picket_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      973 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/singles/picket_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2544 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/singles/wrist.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/singles/wrist.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2788 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/singles/wrist_long.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1149 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/singles/wrist_long.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    34548 2022-11-30 15:52:02.000000 cytosim-0.0.1/src/sim/solid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6859 2022-11-30 15:52:10.000000 cytosim-0.0.1/src/sim/solid.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3831 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/solid_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3652 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/solid_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2047 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/solid_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2192 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/solid_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13145 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/space.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7067 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/space.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6180 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/space_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1748 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/space_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3271 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/space_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2122 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/space_set.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.262243 cytosim-0.0.1/src/sim/spaces/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5552 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_banana.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1965 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_banana.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7195 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_capsule.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2416 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_capsule.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6371 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_cylinder.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2316 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_cylinder.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5381 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_cylinderP.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2629 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_cylinderP.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6575 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_cylinderZ.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2297 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_cylinderZ.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6118 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_dice.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2059 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_dice.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_ellipse.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2475 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_ellipse.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3967 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_periodic.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1709 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_periodic.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9539 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_polygon.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2465 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_polygon.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6219 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_polygonZ.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2398 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_polygonZ.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_ring.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2405 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_ring.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3312 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_sphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2110 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_sphere.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8521 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_square.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1903 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_square.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6841 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_strip.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2311 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_strip.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3201 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_torus.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1668 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/spaces/space_torus.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17484 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/sphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5482 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/sphere.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3182 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/sphere_prop.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2579 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/sphere_prop.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1811 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/sphere_set.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1846 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/sphere_set.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       71 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/splash.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1117 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/sim/splash.h
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.262243 cytosim-0.0.1/src/test/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1478 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/test/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4544 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2052 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_blas.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    23464 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/test/test_code.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      527 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_cxx.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      255 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_dispatch.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4808 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_gillespie.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1945 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/test/test_glapp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1059 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_glos.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8701 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/test/test_glut.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7285 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_glut3D.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7968 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/test/test_grid.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3177 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_math.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12435 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/test/test_matrix.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1228 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_omp.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10164 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/test/test_opengl.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4720 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_pipe.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6112 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/test/test_platonic.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4424 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_quaternion.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14340 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_random.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8234 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/test/test_rasterizer.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      795 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_signal.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21749 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_simd.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_sizeof.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7678 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_solve.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13501 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/test/test_space.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4772 2022-11-30 15:36:20.000000 cytosim-0.0.1/src/test/test_sphere.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      404 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_string.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1248 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_thread.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5154 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/test/test_vbo.cc
-drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2022-12-15 12:46:04.262243 cytosim-0.0.1/src/tools/
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1215 2022-12-05 09:11:55.000000 cytosim-0.0.1/src/tools/CMakeLists.txt
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10863 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/tools/cymart.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11657 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/tools/frametool.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2970 2022-11-30 15:53:07.000000 cytosim-0.0.1/src/tools/makefile.inc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13672 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/tools/pycytoplay.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12565 2022-12-05 09:14:41.000000 cytosim-0.0.1/src/tools/pycytosim.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      734 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/tools/pycytosim.h
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4563 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/tools/reader.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7023 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/tools/report.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3324 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/tools/reportF.cc
--rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3378 2022-11-30 15:33:18.000000 cytosim-0.0.1/src/tools/sieve.cc
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.268541 cytosim-0.0.2/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      722 2023-08-01 11:52:34.000000 cytosim-0.0.2/.gitignore
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4328 2023-08-01 11:52:34.000000 cytosim-0.0.2/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    35147 2023-08-01 11:52:34.000000 cytosim-0.0.2/LICENSE.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4048 2023-08-01 12:28:32.268541 cytosim-0.0.2/PKG-INFO
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3576 2023-08-01 11:52:34.000000 cytosim-0.0.2/PYCYTOSIM.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3752 2023-08-01 11:52:34.000000 cytosim-0.0.2/README.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1258 2023-08-01 11:52:34.000000 cytosim-0.0.2/WARRANTY.txt
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.208541 cytosim-0.0.2/cym/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      514 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/actin.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/amplify.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1218 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/arp23.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3330 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/ashbya.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      614 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1172 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_couple.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1127 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_custom.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_dynamic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1897 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_france.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      759 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_guided.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      884 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_pull.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1347 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_pull3D.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      913 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_texas.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1108 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/aster_tracker.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/axon.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1374 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/axon.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1399 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/baseball.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      897 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/bead.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1793 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/bipolar.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      858 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/buckling.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      839 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/buckling.cym.tpl
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1613 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/capture.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2274 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/capture_amplified.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      856 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/catastrophe_outside.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1228 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/celegans.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1385 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/change.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      563 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/change_confine.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      752 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/change_space.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      873 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/confine_instability.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      983 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/contract.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/contract_always.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1250 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/contract_anchored.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1322 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/contract_clamped.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1222 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/contract_connect.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1135 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/contract_periodic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1857 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cortex.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      891 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/couple.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3110 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/couple_fork.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1140 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/crushed_shell.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1107 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cut_aster.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      922 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cut_fibers.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      954 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cut_planar.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1233 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cut_saved.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3683 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cytokinesis.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      869 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/cytoplasmic_flow.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1266 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/dogic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3225 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/endocytosis.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2103 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/endocytosis.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9924 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/entangled.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1459 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/event.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      945 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fast_diffusion1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      951 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fast_diffusion2.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      353 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1203 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_anchor.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      527 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_athermal.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      837 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_bent.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      615 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_buckle.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      998 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_classic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      834 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_dynamic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      625 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_forces.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1365 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_glue.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      601 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_grow.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1728 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_mixed.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1329 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_omega.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      847 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fiber_treadmill.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      868 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/field.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      715 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/field_bind.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      637 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/field_cut.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      703 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/fountain.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/france.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      643 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/frap.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1277 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/friction.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      968 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1009 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_arcs.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_collect.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1680 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_drag.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1522 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_east.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1353 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_flip.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1959 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_flip_track.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1404 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_flippers.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1770 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_gate.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1126 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_path.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1334 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_ratchet.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1686 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_sort.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1898 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_sort_ortho.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1654 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_sorter.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1349 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_spiral.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_steric.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1369 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_stripe.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1245 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_surface.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      901 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_texas.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2023 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_trap.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1547 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_west.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1624 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_west_blur.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1675 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/glide_yingyang.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1347 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/granules.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1274 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_chew.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      987 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_cut.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1640 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_digit.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      828 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_move.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      861 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_nucleate.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      984 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_rescue.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1330 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_slide.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1025 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_track.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2408 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/hand_walk.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3579 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/lacroix.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1053 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/magic_key.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      672 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/microtubule.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1760 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/minifilaments.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1850 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/minifilaments1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1605 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/minifilaments2.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1509 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/motif.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1554 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/motif_blur.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1132 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/motile_bead.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1145 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/motor_pull.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1006 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/move.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2376 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/muscle.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      972 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/muscle_smooth.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1059 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/needles.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/nematic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      663 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/nucleate.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      842 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/nucleate_edge.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1106 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/nucleus.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1249 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/overlap.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1411 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/overlap3D.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2044 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/overlap3D_16.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1362 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/overlap_walk.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      458 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/packed_beads.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      459 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/packed_beads_2D.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1326 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/packed_gel.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1364 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/placement.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1356 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/pombe.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1528 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/pombe_classic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1724 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/pombe_meiotic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1311 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/push_pull.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1142 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/radial.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1124 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/ring_motors.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1066 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/self.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1012 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/self_cortex.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      754 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/self_vortex.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1086 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/self_walk.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      764 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/side_movement.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      658 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/single.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1348 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/smiley.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1387 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/solid.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      499 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/solid_3D.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      690 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/space_axisymmetric.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      597 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/space_ellipse.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1122 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/sphere.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1097 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spider.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2417 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle3.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3712 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_celegans.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1601 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_centering.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1585 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_centering_dynamic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2199 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_compression.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3423 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_pombe.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    25433 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_pombe_em.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    31549 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_pombe_em1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7568 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spindle_yeast.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      676 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spiral.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      977 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/spool.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1068 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1080 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_3D.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      640 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_artefact.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      649 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_bead_fiber_periodic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      460 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_bead_periodic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      399 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_bead_periodic2.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      940 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_bundle.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1243 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_bundling.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      667 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_cylinder.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      857 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_fiber.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      535 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_fiber1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      846 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_fiber_3D.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      654 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_fiber_periodic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      795 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_sphere.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1910 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/steric_test.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      957 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/swimmers.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      841 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/test_binding1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1077 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/test_binding2.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1262 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/test_binding3.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      735 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/test_bindingP.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      439 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/test_fiber_diffusion.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      419 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/test_single_diffusion.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      550 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/texas.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      794 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/toy.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      906 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/toy_start.cmi
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      892 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/transport.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1035 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/triangle.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1591 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/tug_of_war.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1485 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/walkers.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1137 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/wash.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1322 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/yossi.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1407 2023-08-01 11:52:34.000000 cytosim-0.0.2/cym/zigzag.cym
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.208541 cytosim-0.0.2/cytosim.xcodeproj/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   336632 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/project.pbxproj
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.188541 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3081 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/play.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2846 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/report.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2828 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/sim.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_code.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_grid.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2876 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_matrix.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2864 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_simd.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2377 2023-08-01 11:52:34.000000 cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/tests.xcscheme
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   210863 2023-08-01 11:52:34.000000 cytosim-0.0.2/demo_frame.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    81188 2023-08-01 11:52:34.000000 cytosim-0.0.2/demo_pycytosim.ipynb
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/code/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   106956 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/code/doxygen.cfg
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      652 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/code/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5727 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/code/layout.xml
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      881 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/code/mainpage.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4859 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/code/objects.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/compile/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4678 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/cygwin.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      931 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/dimensionality.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6519 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1459 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/intel_mkl.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      845 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/linux.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1663 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/multithreading.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1361 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/options.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2371 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/compile/vectorization.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/cpython/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28284 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/cpython/cpython.css
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6251 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/cpython/cpython_doc.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   101654 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/cpython/doc_PyCytoplay.html
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   100729 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/cpython/doc_PyCytosim.html
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9278 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/cpython/read_cpython.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/data/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   123267 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/data/cytosim.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29497 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/data/modularity.png
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/examples/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6671 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/biblio.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.212541 cytosim-0.0.2/doc/examples/data/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    33685 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/actin.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    42409 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/ashbya.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    30331 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/celegans.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    60174 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/centering.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    65951 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/droplets.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    50739 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/endocytosis.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    97182 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/minifilaments.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    77302 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/nematics.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   100226 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/network.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5254 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/patterns.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   110273 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/spindle.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    51623 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/spindle_length.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16497 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/data/spombe.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2240 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/examples/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1813 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/index.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.216541 cytosim-0.0.2/doc/main/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      404 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/cheat.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1259 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/credits.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1776 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/examples.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5237 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/executables.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57247 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/faq.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1711 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/file_types.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3256 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/movies.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3969 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/overview.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5837 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/run_slurm.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7840 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/runs.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3784 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/main/starter.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.216541 cytosim-0.0.2/doc/misc/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4057 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/misc/Cytosim.tmbundle.zip
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.216541 cytosim-0.0.2/doc/outreach/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1717 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/controller.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.216541 cytosim-0.0.2/doc/outreach/data/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57904 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/data/CRI-2018-11a.jpg
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    39021 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/data/CRI-2018-11b.jpg
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   102453 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/data/Cambridge-2019-05a.jpg
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    61861 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/data/Cambridge-2019-05b.jpg
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.216541 cytosim-0.0.2/doc/outreach/games/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      643 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/games/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      198 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6378 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/installation1.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5304 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/outreach/installation2.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.216541 cytosim-0.0.2/doc/rendering/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)  1462588 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/actin.blend
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4264 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/import-actin-ico.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4207 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/import-actin-sphere.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4207 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/import-actin.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4413 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/import-links.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4086 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      292 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/rendering/remove-actin.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.220541 cytosim-0.0.2/doc/sim/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12156 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/commands.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2675 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/config.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.220541 cytosim-0.0.2/doc/sim/data/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      928 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/forces.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6040 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/forces.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28232 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/meca_links.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3284 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/steric.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      263 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/steric.tex
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21888 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/steric3D.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11926 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/steric_math.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    65261 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/data/varying_time_step.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9082 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/fiber_dynamics.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1679 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/fibers.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1283 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/forces.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2513 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/graphics.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      611 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1527 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/motor_detachment.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3731 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/numerical_precision.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4246 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/objects.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       85 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/parameters.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8951 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/placement.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6988 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/report.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2687 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/spaces.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3458 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/steric.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3473 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/stochastic.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1882 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/sim/units.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.220541 cytosim-0.0.2/doc/tutorials/
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.220541 cytosim-0.0.2/doc/tutorials/code/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4790 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/code/collect.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      649 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/code/config.cym.tpl
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      710 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/code/master.sh
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    15382 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/code/preconfig
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/code/scan.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.220541 cytosim-0.0.2/doc/tutorials/data/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3334 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/ashbya.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      793 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/aster.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1234 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/aster_dynamic.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4119 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/capture.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19449 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/end_tracking.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28111 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/filament_buckling.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      973 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/gliding.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28234 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/polarity_sorting.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1010 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/data/self.cym
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.224541 cytosim-0.0.2/doc/tutorials/images/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4591 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/H.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4483 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/XTV.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11568 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/aster-vs-nematic.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19716 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/bind_also_end.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    27299 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/bind_end.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20037 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/couples.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7406 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/crosslinks.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    32919 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/droplets.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12570 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/force_velocity.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3561 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/gliding1.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3617 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/gliding2.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    57401 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/kinesin_tetramers.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28232 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/meca_links.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10190 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/images/nematic-vs-polar.png
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1172 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/index.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      227 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_bipolarity.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3031 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_capture.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12562 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_centering.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7861 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_contract2.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5433 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_contract3.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7185 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_contract_motor.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5985 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_gliding.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    23732 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_introduction.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      680 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_nucleus.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14458 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_polar_nematic.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      224 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_polarity.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7287 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_scans.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2543 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_scripting.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11632 2023-08-01 11:52:34.000000 cytosim-0.0.2/doc/tutorials/tuto_self.md
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      356 2023-08-01 11:52:34.000000 cytosim-0.0.2/example.cym
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.224541 cytosim-0.0.2/examples/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      591 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/avoid.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2061 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/callbacks_pycytoplay.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      622 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/flock.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5745 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytoplay_callbacks.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   321969 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_construct.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   279239 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_extend.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   139505 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_flock.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6248 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_import3D.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   160711 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_meca.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4782 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_obj_3D.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   492525 2023-08-01 11:52:34.000000 cytosim-0.0.2/examples/pycytosim_objects.ipynb
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4868 2023-08-01 11:52:34.000000 cytosim-0.0.2/makefile
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12556 2023-08-01 11:52:34.000000 cytosim-0.0.2/makefile.inc
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.224541 cytosim-0.0.2/python/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1013 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/index.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.228541 cytosim-0.0.2/python/look/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4550 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/collect.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3078 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/compare_config.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4391 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/get_data.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     5061 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/make_image.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    12363 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/make_movie.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     7827 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/make_page.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3854 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/make_plots.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    11898 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/read_config.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4262 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/scan.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3694 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/look/tell.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.228541 cytosim-0.0.2/python/misc/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2504 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/misc/battery_test.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3487 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/misc/cleanup.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4468 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/misc/compare.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2305 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/misc/plot.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5881 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/misc/pyned.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     3187 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/misc/reduce.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.228541 cytosim-0.0.2/python/run/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     6691 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/run/go_sim.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7125 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/run/go_sim_lib.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    23500 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/run/preconfig.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     4698 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/run/submit_one.py
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     8716 2023-08-01 11:52:34.000000 cytosim-0.0.2/python/run/submit_slurm.py
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       38 2023-08-01 12:28:32.268541 cytosim-0.0.2/setup.cfg
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2281 2023-08-01 12:27:57.000000 cytosim-0.0.2/setup.py
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.228541 cytosim-0.0.2/src/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      266 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/CMakeLists.txt
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.228541 cytosim-0.0.2/src/base/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      684 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14150 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/array.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2666 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/assert_macro.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      920 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/backtrace.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      679 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/backtrace.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3957 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/buddy.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      187 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/exceptions.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/exceptions.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3924 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/filepath.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2212 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/filepath.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5785 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/filewrapper.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4167 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/filewrapper.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19578 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/glossary.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17191 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/glossary.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1210 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/inventoried.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4977 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/inventory.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3158 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/inventory.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13239 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/iowrapper.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6390 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/iowrapper.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      699 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      796 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/messages.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2738 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/messages.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7638 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/node_list.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3624 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/node_list.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      992 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/noder.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1188 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/operator_new.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2722 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/print_color.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      903 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/print_color.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3195 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/property.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6787 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/property.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6819 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/property_list.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4689 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/property_list.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5957 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/stream_func.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/stream_func.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2607 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/tictoc.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1428 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/tictoc.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1595 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/timer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14894 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/tokenizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3438 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/base/tokenizer.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.232541 cytosim-0.0.2/src/cpython/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4555 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/couple_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13219 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/fiber_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1776 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/glossary_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6128 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/hand_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6486 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/interface_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8178 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/meca_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3303 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/object_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2379 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/organizer_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2330 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/point_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9076 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/python_frame.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3217 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/python_utilities.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8838 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/simul_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3692 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/single_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5534 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/solid_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3441 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/space_modules.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2669 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/cpython/thread_modules.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.232541 cytosim-0.0.2/src/cytosim.egg-info/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4048 2023-08-01 12:28:32.000000 cytosim-0.0.2/src/cytosim.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22560 2023-08-01 12:28:32.000000 cytosim-0.0.2/src/cytosim.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-01 12:28:32.000000 cytosim-0.0.2/src/cytosim.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        1 2023-08-01 12:00:54.000000 cytosim-0.0.2/src/cytosim.egg-info/not-zip-safe
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       48 2023-08-01 12:28:32.000000 cytosim-0.0.2/src/cytosim.egg-info/top_level.txt
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.236541 cytosim-0.0.2/src/disp/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      911 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    47659 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8728 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12450 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display1.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1676 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display1.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17737 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1847 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29713 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display3.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display3.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2017 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2782 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/display_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6302 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/fiber_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9479 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/fiber_disp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37956 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/glapp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4858 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/glapp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    72505 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/gle.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19541 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/gle.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9397 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/gle_color.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13816 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/gle_color.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    64657 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/gle_color_list.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/gle_color_list.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5234 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/glu_unproject.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      392 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/glut.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2213 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/grid_display.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/grid_display.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      271 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/line_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1050 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/line_disp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1452 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   320003 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/miniz.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    69441 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/miniz.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      693 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/offscreen.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      687 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/offscreen.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8985 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/offscreen_fbo.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3408 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/offscreen_glx.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      381 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/opengl.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5347 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/point_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4369 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/point_disp.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19476 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/save_image.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4502 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/save_image.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   199731 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/spng.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13411 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/spng.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21466 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/view.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7272 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/view.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5971 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/view_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6467 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/disp/view_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      863 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/index.md
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.240541 cytosim-0.0.2/src/math/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      990 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5979 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT-avx2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5217 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT-common.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT-params.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT-params19937.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3475 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT-sse2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12768 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8298 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/SFMT.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2689 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/accumulator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3670 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/allocator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11058 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/bicgstab.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12965 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/cblas.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11429 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/clapack.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10653 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/dgtsv.c
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      241 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/dim.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4633 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/evaluator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7507 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/gmres.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17756 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/grid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    26300 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/grid_base.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1974 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/isometry.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/linear_operator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1291 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3493 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3849 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      602 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix11.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8691 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix11.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      802 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix22.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20484 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix22.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3777 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix33.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    31444 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix33.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22178 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrix44.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9356 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matrixbase.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9604 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparse.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesym.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3776 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesym.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28081 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesym1.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7096 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesym1.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17374 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesym2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4448 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesym2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    37068 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesymblk.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8005 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/matsparsesymblk.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3437 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/monitor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15587 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/platonic.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7558 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/platonic.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9504 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/pointsonsphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4817 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/pointsonsphere.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12314 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/polygon.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3531 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/polygon.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7843 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/project_ellipse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      583 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/project_ellipse.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21773 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/quaternion.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12497 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/random.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10100 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/random.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9782 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/random_vector.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1456 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/random_vector.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    18395 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/rasterizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13234 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/rasterizer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5412 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/real.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16193 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/simd.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/simd_print.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9993 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/smath.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6221 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vecprint.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      854 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector1.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12908 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector1.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      935 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16056 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector2.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1046 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector3.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21674 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector3.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1090 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector4.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15588 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/math/vector4.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.240541 cytosim-0.0.2/src/misc/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6565 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/check_dump.m
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.240541 cytosim-0.0.2/src/misc/installation/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   111922 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/RtMidi.cpp
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    25736 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/RtMidi.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.244541 cytosim-0.0.2/src/misc/installation/builder/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/0-live.command
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2048 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2156 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config0.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2184 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config1.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config2.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config3.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1899 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config4.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config5.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2023 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config6.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2148 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config7.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)     2150 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/config8.cym
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/builder/france.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14566 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/cytobuilder.cpp
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12900 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/cytomaster.cpp
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.244541 cytosim-0.0.2/src/misc/installation/cytomaster.xcodeproj/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12175 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/cytomaster.xcodeproj/project.pbxproj
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      859 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/makefile
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.244541 cytosim-0.0.2/src/misc/installation/master/
+-rwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)      561 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/0-live.command
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      982 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config0.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config1.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      896 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config2.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1176 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config4.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3161 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config6.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2765 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config7.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1509 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config8.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3363 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/config9.cym
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    24264 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/master/france.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9945 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/rtmidi_c.cpp
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9194 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/misc/installation/rtmidi_c.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.244541 cytosim-0.0.2/src/play/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      675 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2224 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12390 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/play.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/play.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28066 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/play_keys.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15403 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/play_menus.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2713 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/play_mouse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5535 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/player.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4136 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/player.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11531 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/player_disp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3294 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/player_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3170 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/play/player_prop.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.256541 cytosim-0.0.2/src/sim/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4848 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3838 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/bead.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4214 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/bead.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       94 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/bead_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      211 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/bead_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2886 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/bead_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1967 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/bead_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    42390 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/chain.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17478 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/chain.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       92 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/common.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2358 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/common.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10436 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couple.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9433 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couple.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6226 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couple_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7748 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couple_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    28765 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couple_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8855 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couple_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.256541 cytosim-0.0.2/src/sim/couples/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1025 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/bridge.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1497 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/bridge.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      912 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/bridge_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1064 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/bridge_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3046 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/couple_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1067 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/couple_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1414 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/crosslink.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      875 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/crosslink.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3132 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/crosslink_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1104 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/crosslink_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1131 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/crosslink_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1167 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/crosslink_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3524 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/duo.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1552 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/duo.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3029 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/duo_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1263 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/duo_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/duo_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1492 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/duo_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      880 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/fork.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      870 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/fork.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1439 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/fork_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1437 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/fork_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      989 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/shackle.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      840 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/shackle.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2847 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/shackle_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1128 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/shackle_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      881 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/shackle_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1068 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/couples/shackle_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1637 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/event.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2659 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/event.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1477 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/event_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1391 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/event_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    38151 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11570 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14550 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_grid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_grid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3084 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_grid2.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    16712 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10297 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8025 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_segment.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4117 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_segment.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    33092 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6069 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5789 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_site.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6327 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fiber_site.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.256541 cytosim-0.0.2/src/sim/fibers/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6943 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/classic_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3215 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/classic_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6714 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/classic_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5152 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/classic_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8939 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/dynamic_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4818 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/dynamic_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5287 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/dynamic_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3553 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/dynamic_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4654 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/growing_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3288 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/growing_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2072 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/growing_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3092 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/growing_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4130 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/treadmilling_fiber.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2069 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/treadmilling_fiber.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1712 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/treadmilling_fiber_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1565 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/fibers/treadmilling_fiber_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15391 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10783 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4522 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2922 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2775 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2272 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/field_values.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8960 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/frame_reader.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3468 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/frame_reader.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7681 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hand.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6855 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hand.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       97 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hand_monitor.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1886 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hand_monitor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11612 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hand_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7663 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hand_prop.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.260541 cytosim-0.0.2/src/sim/hands/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      839 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/actor.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      936 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/actor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/actor_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1095 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/actor_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2174 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/chewer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/chewer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2337 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/chewer_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1505 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/chewer_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1578 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/cutter.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1216 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/cutter.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1914 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/cutter_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1458 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/cutter_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4188 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/digit.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3741 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/digit.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1640 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/digit_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1588 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/digit_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1896 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/dynein.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/dynein.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/dynein_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2024 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/dynein_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1909 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/kinesin.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1096 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/kinesin.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1415 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/kinesin_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1451 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/kinesin_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2394 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/mighty.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1045 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/mighty.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4003 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/mighty_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2635 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/mighty_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1924 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/motor.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1434 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/motor.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3705 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/motor_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2406 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/motor_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2002 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/myosin.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1083 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/myosin.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/myosin_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1441 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/myosin_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/nucleator.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1685 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/nucleator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3856 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/nucleator_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3290 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/nucleator_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      787 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/regulator.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      987 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/regulator.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      866 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/regulator_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1260 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/regulator_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2586 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/rescuer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1687 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/rescuer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      909 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/rescuer_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1471 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/rescuer_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1195 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/slider.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1173 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/slider.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2614 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/slider_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2773 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/slider_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1901 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/tracker.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1269 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/tracker.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1236 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/tracker_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1515 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/tracker_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2873 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/walker.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2115 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/walker.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3951 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/walker_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2079 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/hands/walker_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    29823 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/interface.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3513 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/interface.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      950 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/interpolation.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4495 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/interpolation.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4417 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/interpolation4.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1957 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/interpolation4.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1530 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/lattice.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15313 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/lattice.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5441 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    46323 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/meca.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    22723 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/meca.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6075 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/meca1d.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)   107544 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/meca_inter.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8873 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecable.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14168 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecable.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8215 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecafil.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4652 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecafil.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20053 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecafil_project.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5581 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecafil_projectmat.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1165 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecapoint.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2131 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/mecapoint.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1992 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/modulo.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2101 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/modulo.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    30312 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/movable.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2997 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/movable.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6062 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/object.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5322 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/object.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14499 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/object_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6995 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/object_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3689 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3630 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizer.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4025 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizer_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1584 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizer_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.264541 cytosim-0.0.2/src/sim/organizers/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21643 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/aster.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7228 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/aster.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1822 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/aster_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2014 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/aster_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4663 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/bundle.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1987 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/bundle.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1632 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/bundle_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1613 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/bundle_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3502 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/fake.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1793 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/fake.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      552 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/fake_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1076 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/fake_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4326 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/nucleus.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2312 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/nucleus.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      529 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/nucleus_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1082 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/organizers/nucleus_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    32594 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/parser.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3009 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/parser.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20108 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/point_grid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9872 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/point_grid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4054 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sim.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      267 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sim.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11790 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sim_thread.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6789 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sim_thread.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13540 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    19507 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1302 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_custom.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    20613 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_file.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5550 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11565 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    71703 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_report.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14266 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_solve.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4736 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/simul_step.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4179 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/single.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6635 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/single.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6389 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/single_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3918 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/single_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    15361 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/single_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5655 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/single_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.264541 cytosim-0.0.2/src/sim/singles/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1397 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/picket.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1406 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/picket.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2795 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/picket_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      973 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/picket_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2544 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/wrist.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2609 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/wrist.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2788 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/wrist_long.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1149 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/singles/wrist_long.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    34548 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/solid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6859 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/solid.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3831 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/solid_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3652 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/solid_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2047 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/solid_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2192 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/solid_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13145 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/space.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7067 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/space.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6180 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/space_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1748 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/space_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3271 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/space_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2122 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/space_set.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.264541 cytosim-0.0.2/src/sim/spaces/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5552 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_banana.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1965 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_banana.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7195 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_capsule.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2416 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_capsule.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6371 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_cylinder.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2316 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_cylinder.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5381 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_cylinderP.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2629 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_cylinderP.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6575 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_cylinderZ.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2297 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_cylinderZ.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6118 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_dice.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2059 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_dice.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7872 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_ellipse.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2475 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_ellipse.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3967 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_periodic.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1709 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_periodic.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     9540 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_polygon.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2465 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_polygon.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6219 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_polygonZ.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2398 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_polygonZ.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4878 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_ring.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2405 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_ring.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3312 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_sphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2110 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_sphere.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8521 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_square.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1903 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_square.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6841 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_strip.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2311 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_strip.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3201 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_torus.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1668 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/spaces/space_torus.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    17484 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5482 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sphere.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3182 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sphere_prop.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2579 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sphere_prop.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1811 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sphere_set.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1846 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/sphere_set.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)       71 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/splash.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1117 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/sim/splash.h
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.268541 cytosim-0.0.2/src/test/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1478 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4544 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1368 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2052 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_blas.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    23464 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_code.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      527 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_cxx.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      255 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_dispatch.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4808 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_gillespie.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1945 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_glapp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1059 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_glos.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8701 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_glut.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7285 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_glut3D.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7968 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_grid.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3177 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_math.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    12435 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_matrix.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1228 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_omp.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10164 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_opengl.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4720 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_pipe.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     6112 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_platonic.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4424 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_quaternion.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    14340 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_random.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     8234 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_rasterizer.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      795 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_signal.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    21749 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_simd.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1831 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_sizeof.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7678 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_solve.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    13501 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_space.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4772 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_sphere.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      404 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_string.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1248 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_thread.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5154 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/test/test_vbo.cc
+drwxrwxr-x   0 dmitrief  (1000) dmitrief  (1000)        0 2023-08-01 12:28:32.268541 cytosim-0.0.2/src/tools/
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     1215 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/CMakeLists.txt
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10863 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/cymart.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    11657 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/frametool.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     2970 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/makefile.inc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)    10045 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/pycytoplay.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     5543 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/pycytosim.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)      794 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/pycytosim.h
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     4563 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/reader.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     7023 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/report.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3324 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/reportF.cc
+-rw-rw-r--   0 dmitrief  (1000) dmitrief  (1000)     3378 2023-08-01 11:52:34.000000 cytosim-0.0.2/src/tools/sieve.cc
```

### Comparing `cytosim-0.0.1/.gitignore` & `cytosim-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/CMakeLists.txt` & `cytosim-0.0.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/LICENSE.txt` & `cytosim-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/PKG-INFO` & `cytosim-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cytosim
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cytosim: Langevin dynamics of active polymer networks
 Keywords: simulation actin microtubule polymer
 Platform: Windows
 Platform: Linux
 Platform: Mac OS-X
 Platform: Unix
 Description-Content-Type: text/markdown
@@ -69,15 +69,15 @@
 	git clone https://gitlab.com/f.nedelec/cytosim
 	cd cytosim
 	
 To compile using [make](https://www.gnu.org/software/make), try:
 	
 	make
 
-If this fails, parameters of `makefile.inc` need to be updated.
+If this fails, parameters of `makefile.inc` need to be updated manually.
 Altermatively, it is possible to use [cmake](https://cmake.org) to configure `make` automatically:
 
 	mkdir build
 	cd build
 	cmake ..
 	make
 
@@ -100,15 +100,15 @@
 *  Jonathan Ward           2008-2014
 *  Antonio Politi          2010-2012
 *  Andre-Claude Clapson    2011-2013
 *  Jamie-Li Rickman        2014-2019
 *  Serge Dmitrieff         2013-
 *  Julio Belmonte          2014-
 *  Gaelle Letort           2014-
-*  Manuel Lera-Ramirez     2017-
-*  Maud Formanek           2020-
+*  Manuel Lera-Ramirez     2017-2022
+*  Maud Formanek           2020-2021
 
 # Contact
 
 Email: cytosim@cytosim.org
```

### Comparing `cytosim-0.0.1/PYCYTOSIM.md` & `cytosim-0.0.2/PYCYTOSIM.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/README.md` & `cytosim-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 	git clone https://gitlab.com/f.nedelec/cytosim
 	cd cytosim
 	
 To compile using [make](https://www.gnu.org/software/make), try:
 	
 	make
 
-If this fails, parameters of `makefile.inc` need to be updated.
+If this fails, parameters of `makefile.inc` need to be updated manually.
 Altermatively, it is possible to use [cmake](https://cmake.org) to configure `make` automatically:
 
 	mkdir build
 	cd build
 	cmake ..
 	make
 
@@ -88,15 +88,15 @@
 *  Jonathan Ward           2008-2014
 *  Antonio Politi          2010-2012
 *  Andre-Claude Clapson    2011-2013
 *  Jamie-Li Rickman        2014-2019
 *  Serge Dmitrieff         2013-
 *  Julio Belmonte          2014-
 *  Gaelle Letort           2014-
-*  Manuel Lera-Ramirez     2017-
-*  Maud Formanek           2020-
+*  Manuel Lera-Ramirez     2017-2022
+*  Maud Formanek           2020-2021
 
 # Contact
 
 Email: cytosim@cytosim.org
```

### Comparing `cytosim-0.0.1/WARRANTY.txt` & `cytosim-0.0.2/WARRANTY.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/actin.cym` & `cytosim-0.0.2/cym/actin.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/amplify.cym` & `cytosim-0.0.2/cym/amplify.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/arp23.cym` & `cytosim-0.0.2/cym/arp23.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/ashbya.cym` & `cytosim-0.0.2/cym/ashbya.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/aster.cym` & `cytosim-0.0.2/cym/aster.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/aster_couple.cym` & `cytosim-0.0.2/cym/aster_couple.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/aster_custom.cym` & `cytosim-0.0.2/cym/aster_custom.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/aster_dynamic.cym` & `cytosim-0.0.2/cym/aster_dynamic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/aster_france.cym` & `cytosim-0.0.2/cym/aster_france.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/aster_guided.cym` & `cytosim-0.0.2/cym/aster_guided.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/aster_pull.cym` & `cytosim-0.0.2/cym/aster_pull.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/aster_pull3D.cym` & `cytosim-0.0.2/cym/aster_pull3D.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/aster_texas.cym` & `cytosim-0.0.2/cym/aster_texas.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/aster_tracker.cym` & `cytosim-0.0.2/cym/aster_tracker.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/axon.cym` & `cytosim-0.0.2/cym/axon.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/axon.txt` & `cytosim-0.0.2/cym/axon.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/baseball.cym` & `cytosim-0.0.2/cym/baseball.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/bead.cym` & `cytosim-0.0.2/cym/bead.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/bipolar.cym` & `cytosim-0.0.2/cym/bipolar.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/buckling.cym` & `cytosim-0.0.2/cym/buckling.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/buckling.cym.tpl` & `cytosim-0.0.2/cym/buckling.cym.tpl`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/capture.cym` & `cytosim-0.0.2/cym/capture.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/capture_amplified.cym` & `cytosim-0.0.2/cym/capture_amplified.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/catastrophe_outside.cym` & `cytosim-0.0.2/cym/catastrophe_outside.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/celegans.cym` & `cytosim-0.0.2/cym/celegans.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/change.cym` & `cytosim-0.0.2/cym/change.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/change_confine.cym` & `cytosim-0.0.2/cym/change_confine.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/change_space.cym` & `cytosim-0.0.2/cym/change_space.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/confine_instability.cym` & `cytosim-0.0.2/cym/confine_instability.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/contract.cym` & `cytosim-0.0.2/cym/contract.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/contract_always.cym` & `cytosim-0.0.2/cym/contract_always.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/contract_anchored.cym` & `cytosim-0.0.2/cym/contract_anchored.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/contract_clamped.cym` & `cytosim-0.0.2/cym/contract_clamped.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/contract_connect.cym` & `cytosim-0.0.2/cym/contract_connect.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/contract_periodic.cym` & `cytosim-0.0.2/cym/contract_periodic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/cortex.cym` & `cytosim-0.0.2/cym/cortex.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/couple.cym` & `cytosim-0.0.2/cym/couple.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/couple_fork.cym` & `cytosim-0.0.2/cym/couple_fork.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/crushed_shell.cym` & `cytosim-0.0.2/cym/crushed_shell.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/cut_aster.cym` & `cytosim-0.0.2/cym/cut_aster.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/cut_fibers.cym` & `cytosim-0.0.2/cym/cut_fibers.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/cut_planar.cym` & `cytosim-0.0.2/cym/cut_planar.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/cut_saved.cym` & `cytosim-0.0.2/cym/cut_saved.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/cytokinesis.txt` & `cytosim-0.0.2/cym/cytokinesis.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/cytoplasmic_flow.cym` & `cytosim-0.0.2/cym/cytoplasmic_flow.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/dogic.cym` & `cytosim-0.0.2/cym/dogic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/endocytosis.cym` & `cytosim-0.0.2/cym/endocytosis.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/endocytosis.txt` & `cytosim-0.0.2/cym/endocytosis.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/entangled.cym` & `cytosim-0.0.2/cym/entangled.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/event.cym` & `cytosim-0.0.2/cym/event.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fast_diffusion1.cym` & `cytosim-0.0.2/cym/fast_diffusion1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fast_diffusion2.cym` & `cytosim-0.0.2/cym/fast_diffusion2.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fiber_anchor.cym` & `cytosim-0.0.2/cym/fiber_anchor.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fiber_athermal.cym` & `cytosim-0.0.2/cym/fiber_athermal.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fiber_bent.cym` & `cytosim-0.0.2/cym/fiber_bent.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fiber_buckle.cym` & `cytosim-0.0.2/cym/fiber_buckle.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fiber_classic.cym` & `cytosim-0.0.2/cym/fiber_classic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fiber_dynamic.cym` & `cytosim-0.0.2/cym/fiber_dynamic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fiber_forces.cym` & `cytosim-0.0.2/cym/fiber_forces.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fiber_glue.cym` & `cytosim-0.0.2/cym/fiber_glue.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fiber_grow.cym` & `cytosim-0.0.2/cym/fiber_grow.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fiber_mixed.cym` & `cytosim-0.0.2/cym/fiber_mixed.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fiber_omega.cym` & `cytosim-0.0.2/cym/fiber_omega.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fiber_treadmill.cym` & `cytosim-0.0.2/cym/fiber_treadmill.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/field.cym` & `cytosim-0.0.2/cym/field.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/field_bind.cym` & `cytosim-0.0.2/cym/field_bind.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/field_cut.cym` & `cytosim-0.0.2/cym/field_cut.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/fountain.cym` & `cytosim-0.0.2/cym/fountain.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/france.txt` & `cytosim-0.0.2/cym/france.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/frap.cym` & `cytosim-0.0.2/cym/frap.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/friction.cym` & `cytosim-0.0.2/cym/friction.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide.cym` & `cytosim-0.0.2/cym/glide.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_arcs.cym` & `cytosim-0.0.2/cym/glide_arcs.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_collect.cym` & `cytosim-0.0.2/cym/glide_collect.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_drag.cym` & `cytosim-0.0.2/cym/glide_drag.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_east.cym` & `cytosim-0.0.2/cym/glide_east.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_flip.cym` & `cytosim-0.0.2/cym/glide_flip.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_flip_track.cym` & `cytosim-0.0.2/cym/glide_flip_track.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_flippers.cym` & `cytosim-0.0.2/cym/glide_flippers.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_gate.cym` & `cytosim-0.0.2/cym/glide_gate.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_path.cym` & `cytosim-0.0.2/cym/glide_path.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_ratchet.cym` & `cytosim-0.0.2/cym/glide_ratchet.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_sort.cym` & `cytosim-0.0.2/cym/glide_sort.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_sort_ortho.cym` & `cytosim-0.0.2/cym/glide_sort_ortho.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_sorter.cym` & `cytosim-0.0.2/cym/glide_sorter.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_spiral.cym` & `cytosim-0.0.2/cym/glide_spiral.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_steric.cym` & `cytosim-0.0.2/cym/glide_steric.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_stripe.cym` & `cytosim-0.0.2/cym/glide_stripe.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_surface.cym` & `cytosim-0.0.2/cym/glide_surface.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_texas.cym` & `cytosim-0.0.2/cym/glide_texas.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_trap.cym` & `cytosim-0.0.2/cym/glide_trap.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_west.cym` & `cytosim-0.0.2/cym/glide_west.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_west_blur.cym` & `cytosim-0.0.2/cym/glide_west_blur.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/glide_yingyang.cym` & `cytosim-0.0.2/cym/glide_yingyang.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/granules.cym` & `cytosim-0.0.2/cym/granules.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/hand_chew.cym` & `cytosim-0.0.2/cym/hand_chew.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/hand_cut.cym` & `cytosim-0.0.2/cym/hand_cut.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/hand_digit.cym` & `cytosim-0.0.2/cym/hand_digit.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/hand_move.cym` & `cytosim-0.0.2/cym/hand_move.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/hand_nucleate.cym` & `cytosim-0.0.2/cym/hand_nucleate.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/hand_rescue.cym` & `cytosim-0.0.2/cym/hand_rescue.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/hand_slide.cym` & `cytosim-0.0.2/cym/hand_slide.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/hand_track.cym` & `cytosim-0.0.2/cym/hand_track.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/hand_walk.cym` & `cytosim-0.0.2/cym/hand_walk.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/lacroix.cym` & `cytosim-0.0.2/cym/lacroix.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/magic_key.cym` & `cytosim-0.0.2/cym/magic_key.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/microtubule.cym` & `cytosim-0.0.2/cym/microtubule.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/minifilaments.cym` & `cytosim-0.0.2/cym/minifilaments.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/minifilaments1.cym` & `cytosim-0.0.2/cym/minifilaments1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/minifilaments2.cym` & `cytosim-0.0.2/cym/minifilaments2.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/motif.cym` & `cytosim-0.0.2/cym/motif.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/motif_blur.cym` & `cytosim-0.0.2/cym/motif_blur.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/motile_bead.cym` & `cytosim-0.0.2/cym/motile_bead.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/motor_pull.cym` & `cytosim-0.0.2/cym/motor_pull.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/move.cym` & `cytosim-0.0.2/cym/move.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/muscle.cym` & `cytosim-0.0.2/cym/muscle.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/muscle_smooth.cym` & `cytosim-0.0.2/cym/muscle_smooth.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/needles.cym` & `cytosim-0.0.2/cym/needles.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/nematic.cym` & `cytosim-0.0.2/cym/nematic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/nucleate.cym` & `cytosim-0.0.2/cym/nucleate.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/nucleate_edge.cym` & `cytosim-0.0.2/cym/nucleate_edge.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/nucleus.cym` & `cytosim-0.0.2/cym/nucleus.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/overlap.cym` & `cytosim-0.0.2/cym/overlap.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/overlap3D.cym` & `cytosim-0.0.2/cym/overlap3D.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/overlap3D_16.cym` & `cytosim-0.0.2/cym/overlap3D_16.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/overlap_walk.cym` & `cytosim-0.0.2/cym/overlap_walk.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/packed_gel.cym` & `cytosim-0.0.2/cym/packed_gel.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/placement.cym` & `cytosim-0.0.2/cym/placement.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/pombe.cym` & `cytosim-0.0.2/cym/pombe.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/pombe_classic.cym` & `cytosim-0.0.2/cym/pombe_classic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/pombe_meiotic.cym` & `cytosim-0.0.2/cym/pombe_meiotic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/push_pull.cym` & `cytosim-0.0.2/cym/push_pull.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/radial.cym` & `cytosim-0.0.2/cym/radial.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/ring_motors.cym` & `cytosim-0.0.2/cym/ring_motors.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/self.cym` & `cytosim-0.0.2/cym/self.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/self_cortex.cym` & `cytosim-0.0.2/cym/self_cortex.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/self_vortex.cym` & `cytosim-0.0.2/cym/self_vortex.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/self_walk.cym` & `cytosim-0.0.2/cym/self_walk.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/side_movement.cym` & `cytosim-0.0.2/cym/side_movement.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/single.cym` & `cytosim-0.0.2/cym/single.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/smiley.cym` & `cytosim-0.0.2/cym/smiley.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/solid.cym` & `cytosim-0.0.2/cym/solid.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/space_axisymmetric.cym` & `cytosim-0.0.2/cym/space_axisymmetric.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/space_ellipse.cym` & `cytosim-0.0.2/cym/space_ellipse.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/sphere.cym` & `cytosim-0.0.2/cym/sphere.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/spider.cym` & `cytosim-0.0.2/cym/spider.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/spindle3.cym` & `cytosim-0.0.2/cym/spindle3.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/spindle_celegans.cym` & `cytosim-0.0.2/cym/spindle_celegans.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/spindle_centering.cym` & `cytosim-0.0.2/cym/spindle_centering.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/spindle_centering_dynamic.cym` & `cytosim-0.0.2/cym/spindle_centering_dynamic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/spindle_compression.cym` & `cytosim-0.0.2/cym/spindle_compression.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/spindle_pombe.cym` & `cytosim-0.0.2/cym/spindle_pombe.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/spindle_pombe_em.cym` & `cytosim-0.0.2/cym/spindle_pombe_em.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/spindle_pombe_em1.cym` & `cytosim-0.0.2/cym/spindle_pombe_em1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/spindle_yeast.cym` & `cytosim-0.0.2/cym/spindle_yeast.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/spiral.cym` & `cytosim-0.0.2/cym/spiral.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/spool.cym` & `cytosim-0.0.2/cym/spool.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/steric.cym` & `cytosim-0.0.2/cym/steric.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/steric_3D.cym` & `cytosim-0.0.2/cym/steric_3D.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/steric_artefact.cym` & `cytosim-0.0.2/cym/steric_artefact.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/steric_bead_fiber_periodic.cym` & `cytosim-0.0.2/cym/steric_bead_fiber_periodic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/steric_bundle.cym` & `cytosim-0.0.2/cym/steric_bundle.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/steric_bundling.cym` & `cytosim-0.0.2/cym/steric_bundling.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/steric_cylinder.cym` & `cytosim-0.0.2/cym/steric_cylinder.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/steric_fiber.cym` & `cytosim-0.0.2/cym/steric_fiber.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/steric_fiber1.cym` & `cytosim-0.0.2/cym/steric_fiber1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/steric_fiber_3D.cym` & `cytosim-0.0.2/cym/steric_fiber_3D.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/steric_fiber_periodic.cym` & `cytosim-0.0.2/cym/steric_fiber_periodic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/steric_sphere.cym` & `cytosim-0.0.2/cym/steric_sphere.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/steric_test.cym` & `cytosim-0.0.2/cym/steric_test.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/swimmers.cym` & `cytosim-0.0.2/cym/swimmers.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/test_binding1.cym` & `cytosim-0.0.2/cym/test_binding1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/test_binding2.cym` & `cytosim-0.0.2/cym/test_binding2.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/test_binding3.cym` & `cytosim-0.0.2/cym/test_binding3.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/test_bindingP.cym` & `cytosim-0.0.2/cym/test_bindingP.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/texas.txt` & `cytosim-0.0.2/cym/texas.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/toy.cym` & `cytosim-0.0.2/cym/toy.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/toy_start.cmi` & `cytosim-0.0.2/cym/toy_start.cmi`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/transport.cym` & `cytosim-0.0.2/cym/transport.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/triangle.cym` & `cytosim-0.0.2/cym/triangle.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/tug_of_war.cym` & `cytosim-0.0.2/cym/tug_of_war.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/walkers.cym` & `cytosim-0.0.2/cym/walkers.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/wash.cym` & `cytosim-0.0.2/cym/wash.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/yossi.cym` & `cytosim-0.0.2/cym/yossi.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cym/zigzag.cym` & `cytosim-0.0.2/cym/zigzag.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cytosim.xcodeproj/project.pbxproj` & `cytosim-0.0.2/cytosim.xcodeproj/project.pbxproj`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 		BB07F48A11627E2200A15828 /* fiber_prop.cc in Sources */ = {isa = PBXBuildFile; fileRef = BB07F48811627E2200A15828 /* fiber_prop.cc */; };
 		BB07F48B11627E2200A15828 /* fiber_prop.h in Headers */ = {isa = PBXBuildFile; fileRef = BB07F48911627E2200A15828 /* fiber_prop.h */; };
 		BB07F523116291E800A15828 /* fiber_set.cc in Sources */ = {isa = PBXBuildFile; fileRef = BB07F521116291E800A15828 /* fiber_set.cc */; };
 		BB07F524116291E800A15828 /* fiber_set.h in Headers */ = {isa = PBXBuildFile; fileRef = BB07F522116291E800A15828 /* fiber_set.h */; };
 		BB089A0A2228A26D00C070E7 /* matrix11.cc in Sources */ = {isa = PBXBuildFile; fileRef = BB089A072228A26D00C070E7 /* matrix11.cc */; };
 		BB089A0B2228A26D00C070E7 /* matrix22.cc in Sources */ = {isa = PBXBuildFile; fileRef = BB089A082228A26D00C070E7 /* matrix22.cc */; };
 		BB089A0C2228A26D00C070E7 /* matrix33.cc in Sources */ = {isa = PBXBuildFile; fileRef = BB089A092228A26D00C070E7 /* matrix33.cc */; };
+		BB0A82A829B34143001287EF /* display_prop.h in Headers */ = {isa = PBXBuildFile; fileRef = BB0A82A529B34142001287EF /* display_prop.h */; };
+		BB0A82A929B34143001287EF /* display.h in Headers */ = {isa = PBXBuildFile; fileRef = BB0A82A629B34142001287EF /* display.h */; };
+		BB0A82AA29B34143001287EF /* display.cc in Sources */ = {isa = PBXBuildFile; fileRef = BB0A82A729B34142001287EF /* display.cc */; };
 		BB0DF4810D93F11F006CB71A /* lattice.cc in Sources */ = {isa = PBXBuildFile; fileRef = BB1749A407D798E600BC7BDC /* lattice.cc */; };
 		BB0E4BD81002698100A96B34 /* random_vector.h in Headers */ = {isa = PBXBuildFile; fileRef = BB0E4BD61002698100A96B34 /* random_vector.h */; };
 		BB0E4BD91002698100A96B34 /* random_vector.cc in Sources */ = {isa = PBXBuildFile; fileRef = BB0E4BD71002698100A96B34 /* random_vector.cc */; };
 		BB0E885616FBC81400451517 /* sim_thread.cc in Sources */ = {isa = PBXBuildFile; fileRef = BB0E885416FBC81400451517 /* sim_thread.cc */; };
 		BB0E885716FBC81400451517 /* sim_thread.h in Headers */ = {isa = PBXBuildFile; fileRef = BB0E885516FBC81400451517 /* sim_thread.h */; };
 		BB0F033114C5FDF2002FA598 /* report.cc in Sources */ = {isa = PBXBuildFile; fileRef = BBA721BB1462C3B900ACF26D /* report.cc */; };
 		BB10378310B8032E00CEC5C6 /* assert_macro.h in Headers */ = {isa = PBXBuildFile; fileRef = BB73586E05B98DA3006956D5 /* assert_macro.h */; };
@@ -424,15 +427,14 @@
 		BBA98688132245DB0031200B /* crosslink_prop.h in Headers */ = {isa = PBXBuildFile; fileRef = BBA98684132245DB0031200B /* crosslink_prop.h */; };
 		BBA98689132245DB0031200B /* crosslink.cc in Sources */ = {isa = PBXBuildFile; fileRef = BBA98685132245DB0031200B /* crosslink.cc */; };
 		BBA9868A132245DB0031200B /* crosslink.h in Headers */ = {isa = PBXBuildFile; fileRef = BBA98686132245DB0031200B /* crosslink.h */; };
 		BBA9869A132246870031200B /* bridge_prop.cc in Sources */ = {isa = PBXBuildFile; fileRef = BBA98696132246870031200B /* bridge_prop.cc */; };
 		BBA9869B132246870031200B /* bridge_prop.h in Headers */ = {isa = PBXBuildFile; fileRef = BBA98697132246870031200B /* bridge_prop.h */; };
 		BBA9869C132246870031200B /* bridge.cc in Sources */ = {isa = PBXBuildFile; fileRef = BBA98698132246870031200B /* bridge.cc */; };
 		BBA9869D132246870031200B /* bridge.h in Headers */ = {isa = PBXBuildFile; fileRef = BBA98699132246870031200B /* bridge.h */; };
-		BBADE815091F4427007BB791 /* disp in Sources */ = {isa = PBXBuildFile; fileRef = BBADE80D091F4427007BB791 /* disp */; };
 		BBADE817091F4427007BB791 /* display1.cc in Sources */ = {isa = PBXBuildFile; fileRef = BBADE80F091F4427007BB791 /* display1.cc */; };
 		BBADE819091F4427007BB791 /* display3.cc in Sources */ = {isa = PBXBuildFile; fileRef = BBADE811091F4427007BB791 /* display3.cc */; };
 		BBAEC4F80EF1D1DD00955B64 /* libcytomath.a in Frameworks */ = {isa = PBXBuildFile; fileRef = BB7191C50EF1CD9900CED9E2 /* libcytomath.a */; };
 		BBAEC4FE0EF1D20000955B64 /* libcytomath.a in Frameworks */ = {isa = PBXBuildFile; fileRef = BB7191C50EF1CD9900CED9E2 /* libcytomath.a */; };
 		BBAEC5080EF1D22300955B64 /* libcytomath.a in Frameworks */ = {isa = PBXBuildFile; fileRef = BB7191C50EF1CD9900CED9E2 /* libcytomath.a */; };
 		BBAEC50B0EF1D22B00955B64 /* libcytomath.a in Frameworks */ = {isa = PBXBuildFile; fileRef = BB7191C50EF1CD9900CED9E2 /* libcytomath.a */; };
 		BBAEC50D0EF1D23000955B64 /* libcytomath.a in Frameworks */ = {isa = PBXBuildFile; fileRef = BB7191C50EF1CD9900CED9E2 /* libcytomath.a */; };
@@ -892,14 +894,17 @@
 		BB07F48811627E2200A15828 /* fiber_prop.cc */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.cpp.cpp; name = fiber_prop.cc; path = src/sim/fiber_prop.cc; sourceTree = SOURCE_ROOT; };
 		BB07F48911627E2200A15828 /* fiber_prop.h */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.c.h; name = fiber_prop.h; path = src/sim/fiber_prop.h; sourceTree = SOURCE_ROOT; };
 		BB07F521116291E800A15828 /* fiber_set.cc */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.cpp.cpp; name = fiber_set.cc; path = src/sim/fiber_set.cc; sourceTree = SOURCE_ROOT; };
 		BB07F522116291E800A15828 /* fiber_set.h */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.c.h; name = fiber_set.h; path = src/sim/fiber_set.h; sourceTree = SOURCE_ROOT; };
 		BB089A072228A26D00C070E7 /* matrix11.cc */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.cpp.cpp; path = matrix11.cc; sourceTree = "<group>"; };
 		BB089A082228A26D00C070E7 /* matrix22.cc */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.cpp.cpp; path = matrix22.cc; sourceTree = "<group>"; };
 		BB089A092228A26D00C070E7 /* matrix33.cc */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.cpp.cpp; path = matrix33.cc; sourceTree = "<group>"; };
+		BB0A82A529B34142001287EF /* display_prop.h */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.c.h; name = display_prop.h; path = src/disp/display_prop.h; sourceTree = SOURCE_ROOT; };
+		BB0A82A629B34142001287EF /* display.h */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.c.h; name = display.h; path = src/disp/display.h; sourceTree = SOURCE_ROOT; };
+		BB0A82A729B34142001287EF /* display.cc */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.cpp.cpp; name = display.cc; path = src/disp/display.cc; sourceTree = SOURCE_ROOT; };
 		BB0AB41E201BBA41004739CE /* doc */ = {isa = PBXFileReference; lastKnownFileType = folder; path = doc; sourceTree = "<group>"; };
 		BB0C409E069A043600CF45A8 /* matsparsesym.cc */ = {isa = PBXFileReference; explicitFileType = sourcecode.cpp.cpp; fileEncoding = 30; name = matsparsesym.cc; path = src/math/matsparsesym.cc; sourceTree = SOURCE_ROOT; };
 		BB0C409F069A043600CF45A8 /* matsparsesym.h */ = {isa = PBXFileReference; explicitFileType = sourcecode.cpp.h; fileEncoding = 30; name = matsparsesym.h; path = src/math/matsparsesym.h; sourceTree = SOURCE_ROOT; };
 		BB0E4BD61002698100A96B34 /* random_vector.h */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.c.h; name = random_vector.h; path = src/math/random_vector.h; sourceTree = SOURCE_ROOT; };
 		BB0E4BD71002698100A96B34 /* random_vector.cc */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.cpp.cpp; name = random_vector.cc; path = src/math/random_vector.cc; sourceTree = SOURCE_ROOT; };
 		BB0E75E505E1440E00BC9B7A /* matrix.cc */ = {isa = PBXFileReference; explicitFileType = sourcecode.cpp.cpp; fileEncoding = 30; name = matrix.cc; path = src/math/matrix.cc; sourceTree = SOURCE_ROOT; };
 		BB0E885416FBC81400451517 /* sim_thread.cc */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.cpp.cpp; name = sim_thread.cc; path = ../sim/sim_thread.cc; sourceTree = "<group>"; };
@@ -1238,16 +1243,14 @@
 		BBA98686132245DB0031200B /* crosslink.h */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.c.h; name = crosslink.h; path = couples/crosslink.h; sourceTree = "<group>"; };
 		BBA98696132246870031200B /* bridge_prop.cc */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.cpp.cpp; name = bridge_prop.cc; path = couples/bridge_prop.cc; sourceTree = "<group>"; };
 		BBA98697132246870031200B /* bridge_prop.h */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.c.h; name = bridge_prop.h; path = couples/bridge_prop.h; sourceTree = "<group>"; };
 		BBA98698132246870031200B /* bridge.cc */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.cpp.cpp; name = bridge.cc; path = couples/bridge.cc; sourceTree = "<group>"; };
 		BBA98699132246870031200B /* bridge.h */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.c.h; name = bridge.h; path = couples/bridge.h; sourceTree = "<group>"; };
 		BBAB0D36138FAEC6006DEAF9 /* reader.cc */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.cpp.cpp; path = reader.cc; sourceTree = "<group>"; };
 		BBAD0F610BF712D8005BFFFA /* python */ = {isa = PBXFileReference; lastKnownFileType = folder; path = python; sourceTree = "<group>"; };
-		BBADE80D091F4427007BB791 /* disp */ = {isa = PBXFileReference; explicitFileType = sourcecode.cpp.cpp; name = disp; path = src/disp; sourceTree = SOURCE_ROOT; };
-		BBADE80E091F4427007BB791 /* disp */ = {isa = PBXFileReference; explicitFileType = sourcecode.cpp.h; fileEncoding = 30; name = disp; path = src/disp; sourceTree = SOURCE_ROOT; };
 		BBADE80F091F4427007BB791 /* display1.cc */ = {isa = PBXFileReference; explicitFileType = sourcecode.cpp.cpp; fileEncoding = 30; name = display1.cc; path = src/disp/display1.cc; sourceTree = SOURCE_ROOT; };
 		BBADE810091F4427007BB791 /* display1.h */ = {isa = PBXFileReference; explicitFileType = sourcecode.cpp.h; fileEncoding = 30; name = display1.h; path = src/disp/display1.h; sourceTree = SOURCE_ROOT; };
 		BBADE811091F4427007BB791 /* display3.cc */ = {isa = PBXFileReference; explicitFileType = sourcecode.cpp.cpp; fileEncoding = 30; name = display3.cc; path = src/disp/display3.cc; sourceTree = SOURCE_ROOT; };
 		BBADE812091F4427007BB791 /* display3.h */ = {isa = PBXFileReference; explicitFileType = sourcecode.cpp.h; fileEncoding = 30; name = display3.h; path = src/disp/display3.h; sourceTree = SOURCE_ROOT; };
 		BBAF2B2E0FD01048006E8E27 /* hand_prop.h */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.c.h; name = hand_prop.h; path = src/sim/hand_prop.h; sourceTree = SOURCE_ROOT; };
 		BBAF2B2F0FD01048006E8E27 /* hand_prop.cc */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.cpp.cpp; name = hand_prop.cc; path = src/sim/hand_prop.cc; sourceTree = SOURCE_ROOT; };
 		BBB1E479126DC70B00B19D26 /* actor_prop.cc */ = {isa = PBXFileReference; fileEncoding = 4; lastKnownFileType = sourcecode.cpp.cpp; name = actor_prop.cc; path = hands/actor_prop.cc; sourceTree = "<group>"; };
@@ -2393,16 +2396,17 @@
 			);
 			name = Bridge;
 			sourceTree = "<group>";
 		};
 		BBADE80A091F4406007BB791 /* display */ = {
 			isa = PBXGroup;
 			children = (
-				BBADE80E091F4427007BB791 /* disp */,
-				BBADE80D091F4427007BB791 /* disp */,
+				BB0A82A729B34142001287EF /* display.cc */,
+				BB0A82A629B34142001287EF /* display.h */,
+				BB0A82A529B34142001287EF /* display_prop.h */,
 				BB7F683E12D0F1B100F8FC84 /* display_prop.cc */,
 				BBADE810091F4427007BB791 /* display1.h */,
 				BBADE80F091F4427007BB791 /* display1.cc */,
 				BBF7BB1910CD44E00089F5B1 /* display2.h */,
 				BBF7BB1810CD44E00089F5B1 /* display2.cc */,
 				BBADE812091F4427007BB791 /* display3.h */,
 				BBADE811091F4427007BB791 /* display3.cc */,
@@ -2957,17 +2961,19 @@
 			runOnlyForDeploymentPostprocessing = 0;
 		};
 		BBA5793105FA64A3009AE66E /* Headers */ = {
 			isa = PBXHeadersBuildPhase;
 			buildActionMask = 2147483647;
 			files = (
 				BBF7BB1B10CD44E00089F5B1 /* display2.h in Headers */,
+				BB0A82A929B34143001287EF /* display.h in Headers */,
 				BB56FA7712D0A0BF008B2260 /* player_prop.h in Headers */,
 				BB0E885716FBC81400451517 /* sim_thread.h in Headers */,
 				BBCA7D081803EAF4000DFD95 /* player.h in Headers */,
+				BB0A82A829B34143001287EF /* display_prop.h in Headers */,
 			);
 			runOnlyForDeploymentPostprocessing = 0;
 		};
 		BBCA9EEB06AFCB4600638608 /* Headers */ = {
 			isa = PBXHeadersBuildPhase;
 			buildActionMask = 2147483647;
 			files = (
@@ -3723,16 +3729,16 @@
 			runOnlyForDeploymentPostprocessing = 0;
 		};
 		BBA5793205FA64A3009AE66E /* Sources */ = {
 			isa = PBXSourcesBuildPhase;
 			buildActionMask = 2147483647;
 			files = (
 				BB217A881AAA67AA006DD82E /* play.cc in Sources */,
-				BBADE815091F4427007BB791 /* disp in Sources */,
 				BBADE817091F4427007BB791 /* display1.cc in Sources */,
+				BB0A82AA29B34143001287EF /* display.cc in Sources */,
 				BBADE819091F4427007BB791 /* display3.cc in Sources */,
 				BB6E174E223E5B3D00AF850D /* operator_new.cc in Sources */,
 				BBF7BB1A10CD44E00089F5B1 /* display2.cc in Sources */,
 				BB7662C510E923A200C93DF6 /* frame_reader.cc in Sources */,
 				BB56FA7812D0A0BF008B2260 /* player_prop.cc in Sources */,
 				BB8BBD0621537DD50033BC7A /* player.cc in Sources */,
 				BB7F684012D0F1B100F8FC84 /* display_prop.cc in Sources */,
@@ -4363,36 +4369,39 @@
 		BB87B94F08CDC50600A05F58 /* Development */ = {
 			isa = XCBuildConfiguration;
 			buildSettings = {
 				CLANG_ENABLE_OBJC_WEAK = YES;
 				CLANG_USE_OPTIMIZATION_PROFILE = NO;
 				COMBINE_HIDPI_IMAGES = YES;
 				LIBRARY_STYLE = STATIC;
+				MACOSX_DEPLOYMENT_TARGET = 10.14;
 				PRODUCT_NAME = cytobase;
 			};
 			name = Development;
 		};
 		BB87B95008CDC50600A05F58 /* Deployment */ = {
 			isa = XCBuildConfiguration;
 			buildSettings = {
 				CLANG_ENABLE_OBJC_WEAK = YES;
 				CLANG_USE_OPTIMIZATION_PROFILE = NO;
 				COMBINE_HIDPI_IMAGES = YES;
 				LIBRARY_STYLE = STATIC;
+				MACOSX_DEPLOYMENT_TARGET = 10.14;
 				PRODUCT_NAME = cytobase;
 			};
 			name = Deployment;
 		};
 		BB87B95108CDC50600A05F58 /* Default */ = {
 			isa = XCBuildConfiguration;
 			buildSettings = {
 				CLANG_ENABLE_OBJC_WEAK = YES;
 				CLANG_USE_OPTIMIZATION_PROFILE = NO;
 				COMBINE_HIDPI_IMAGES = YES;
 				LIBRARY_STYLE = STATIC;
+				MACOSX_DEPLOYMENT_TARGET = 10.14;
 				PRODUCT_NAME = cytobase;
 			};
 			name = Default;
 		};
 		BB87B95308CDC50600A05F58 /* Development */ = {
 			isa = XCBuildConfiguration;
 			buildSettings = {
```

### Comparing `cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/play.xcscheme` & `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/play.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/report.xcscheme` & `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/report.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/sim.xcscheme` & `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/sim.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/test_code.xcscheme` & `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_code.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/test_grid.xcscheme` & `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_grid.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/test_matrix.xcscheme` & `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_matrix.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/test_simd.xcscheme` & `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/test_simd.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/cytosim.xcodeproj/xcshareddata/xcschemes/tests.xcscheme` & `cytosim-0.0.2/cytosim.xcodeproj/xcshareddata/xcschemes/tests.xcscheme`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/code/doxygen.cfg` & `cytosim-0.0.2/doc/code/doxygen.cfg`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/code/index.md` & `cytosim-0.0.2/doc/code/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/code/layout.xml` & `cytosim-0.0.2/doc/code/layout.xml`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/code/mainpage.md` & `cytosim-0.0.2/doc/code/mainpage.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/code/objects.md` & `cytosim-0.0.2/doc/code/objects.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/compile/cygwin.md` & `cytosim-0.0.2/doc/compile/cygwin.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/compile/dimensionality.md` & `cytosim-0.0.2/doc/compile/dimensionality.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/compile/index.md` & `cytosim-0.0.2/doc/compile/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/compile/intel_mkl.md` & `cytosim-0.0.2/doc/compile/intel_mkl.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/compile/linux.md` & `cytosim-0.0.2/doc/compile/linux.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/compile/multithreading.md` & `cytosim-0.0.2/doc/compile/multithreading.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/compile/options.md` & `cytosim-0.0.2/doc/compile/options.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/compile/vectorization.md` & `cytosim-0.0.2/doc/compile/vectorization.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/cpython/cpython.css` & `cytosim-0.0.2/doc/cpython/cpython.css`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/cpython/cpython_doc.py` & `cytosim-0.0.2/doc/cpython/cpython_doc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import read_cpython as rcp
 from os import listdir
 from os.path import isfile, join
 
 def read_to_modules(header_files, name=None):
+    """
+        Reads header files and create a module representation
+    """
     if name is None:
         name="PyCytosim"
     module = rcp.Module(name=name)
     for fname in header_files:
         with open(fname) as file:
             current_class = None
             current_def = None
@@ -18,14 +21,17 @@
                 elif line.find(".def") >= 0:
                     current_def = rcp.parse_def(module, current_class, line)
                 elif line.find("@PYD;"):
                     current_def = rcp.parse_comment(module, current_def, line)
     return module
 
 def print_member(member, classe, classe_link=None, link_pref=None):
+    """ 
+        Prints a member to HTML
+    """
     text = ""
     member_link = None
     if member is not None:
         member_text = member.name
         text += "<div class='contents'>"
         if classe_link is not None:
             with open(classe_link,"r") as cl:
@@ -38,22 +44,26 @@
             text += "<span class='membertext'>  %s  </span> \n" % member.text
         text += "</div>"
         text += "</div>"
 
     return text
 
 def get_link(text):
+    """ Try to extract a link from a line of HTML code"""
     try:
         link = text.split('"')[3]
     except:
         link = None
     return link
 
 
 def print_classe(classe, lines, link_pref=None):
+    """ 
+        Prints a class to HTML
+    """
     text = ""
     classe_link=None
     if classe is not None:
         classe_text = classe.name
         text += "<div class='contents' data-class data-depth-%s data-state='0'>" %classe.depth
 
         if lines is not None:
@@ -82,43 +92,51 @@
             text += "</div>"
 
         text += "</div> \n"
     return   text
 
 
 def get_classe_text(lines, classe_text, link_pref=None):
+    """
+        Tries to find the name of a class in the HTML documentation
+    """
     for line in lines:
         l = line.find(">"+classe_text+"<")
         if l>0:
             b = line.find('<a class="el"')
             d = line.find('</a>')
-            if b>0 and d>b:
+            if b>=0 and d>b:
                 link = line[b:d+4]
                 k = link.find("href=")
                 link = link[:(k+6)] + link_pref + link[(k+6):]
                 return link
     return classe_text
 
 def make_page(module, html_list, output, link_pref=None):
+    """
+        Writes the HTML page
+    """
     with open(output, "w") as out:
         lines = None
         out.write("<!DOCTYPE html> \
         <html xmlns='http://www.w3.org/1999/xhtml' > \
         <link href='cpython.css' rel='stylesheet' type='text/css'/> \
         <head > <title>%s: Bound classes and members</title> \
         <script type='text/javascript'> \
         function activate(element) {element.parentElement.parentElement.setAttribute('data-state','1');} \
         function deactivate(element) {element.parentElement.parentElement.setAttribute('data-state','0');} \
         </script> \
         </head > \
         \n" %module.name)
         out.write("<body>")
-        out.write("<div class ='header' ><h1> Bound classes and members.</h1></div >")
+        out.write("<div class ='header' ><h1> %s</h1> A python interface for Cytosim</div >" % module.name)
         out.write("<div class ='header' > To use the links, please compile the cytosim documentation.  \
-        For this run the command : <p/> <span class='membertext'>make doc </span> </div >")
+            For this run the command : <p/> <span class='membertext'>make doc </span> </div >")
+        out.write("<div class ='header' ><h3> List of bound classes and members :</h3></div >")
+
         try:
             page = open(html_list,"r")
             lines = [line.split("</td>")[0] for line in page.readlines() if line.find("entry")>0]
         except:
             out.write("<div class ='textblock' > Could not open the code documentation. Try typing 'make doc' in your terminal.</div >")
 
         text = print_classe(module, lines, link_pref=link_pref)
@@ -126,15 +144,14 @@
         out.write("</body>")
         out.write("</html>")
 
 if __name__=="__main__":
     folder = "../../src/cpython/"
     modules_tools = {"PyCytosim" : "../../src/tools/pycytosim.cc", "PyCytoplay" : "../../src/tools/pycytoplay.cc"}
     html_list = "../code/doxygen/annotated.html"
-    #output = "cpython_bindings.html"
     link_pref = "../code/doxygen/"
     header_files = []
     header_files.extend([join(folder, f) for f in listdir(folder) if isfile(join(folder, f)) and f.endswith(".h") or f.endswith(".cc") ])
 
     for name, file in modules_tools.items():
         files = [file]
         files.extend(header_files)
```

### Comparing `cytosim-0.0.1/doc/cpython/doc_PyCytoplay.html` & `cytosim-0.0.2/doc/cpython/doc_PyCytoplay.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,79 @@
 <!DOCTYPE html>         <html xmlns='http://www.w3.org/1999/xhtml' >         <link href='cpython.css' rel='stylesheet' type='text/css'/>         <head > <title>PyCytoplay: Bound classes and members</title>         <script type='text/javascript'>         function activate(element) {element.parentElement.parentElement.setAttribute('data-state','1');}         function deactivate(element) {element.parentElement.parentElement.setAttribute('data-state','0');}         </script>         </head >         
-<body><div class ='header' ><h1> Bound classes and members.</h1></div ><div class ='header' > To use the links, please compile the cytosim documentation.          For this run the command : <p/> <span class='membertext'>make doc </span> </div ><div class='contents' data-class data-depth-0 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>PyCytoplay</div> <div class='directory' data-member><div class='contents'><div class='textblock'>simul<span class='membertext'>  The ongoing simulation  </span> 
-</div></div><div class='contents'><div class='textblock'>setNormalKey<span class='membertext'>   sets the callback function for normal keys  </span> 
+<body><div class ='header' ><h1> PyCytoplay</h1> A python interface for Cytosim</div ><div class ='header' > To use the links, please compile the cytosim documentation.              For this run the command : <p/> <span class='membertext'>make doc </span> </div ><div class ='header' ><h3> List of bound classes and members :</h3></div ><div class='contents' data-class data-depth-0 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>PyCytoplay</div> <div class='directory' data-member><div class='contents'><div class='textblock'>play</div></div><div class='contents'><div class='textblock'>setNormalKey<span class='membertext'>   sets the callback function for normal keys  </span> 
 </div></div><div class='contents'><div class='textblock'>setRuntimeCheck<span class='membertext'>   sets the callback function for runtime checks  </span> 
 </div></div><div class='contents'><div class='textblock'>setMouseClick<span class='membertext'>   sets the callback function for mouse clicks  </span> 
-</div></div></div><div class='directory'><div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Frame</div> <div class='directory' data-member><div class='contents'><div class='textblock'>fibers</div></div><div class='contents'><div class='textblock'>time</div></div><div class='contents'><div class='textblock'>index</div></div><div class='contents'><div class='textblock'>loaded</div></div><div class='contents'><div class='textblock'>update</div></div><div class='contents'><div class='textblock'>keys</div></div><div class='contents'><div class='textblock'>items</div></div><div class='contents'><div class='textblock'>__getitem__</div></div><div class='contents'><div class='textblock'>start</div></div><div class='contents'><div class='textblock'>play</div></div><div class='contents'><div class='textblock'>str_to_glos</div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_simul.html" target="_self">Simul</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>frame<span class='membertext'>  returns current frame, e.g. frame = sim.frame()  </span> 
-</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ab6123d07890548356b8e8e16306afebc">writeObjects</a><span class='membertext'>   writes Objects to default trajectory file  </span> 
-</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ab6123d07890548356b8e8e16306afebc">writeObjects</a><span class='membertext'>   writes Objects to a trajectory file, e.g. writeOjects('file.cmo')  </span> 
-</div></div><div class='contents'><div class='textblock'>save<span class='membertext'>   saves current state to trajectory file  </span> 
-</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ad96ee952118ebbb111f9a4e5fafe77c7">add</a><span class='membertext'>   adds objects to simulation, see provided examples  </span> 
-</div></div><div class='contents'><div class='textblock'>cut<span class='membertext'>   performes a cut : sim.cut(filament_name, where), see Parser.execute_cut  (C++)  </span> 
-</div></div><div class='contents'><div class='textblock'>delete<span class='membertext'>   deletes objects from simulation, see provided examples  </span> 
-</div></div><div class='contents'><div class='textblock'>import<span class='membertext'>   imports objects from text file, see provided examples  </span> 
-</div></div><div class='contents'><div class='textblock'>export<span class='membertext'>   export objects to text file, see provided examples  </span> 
-</div></div><div class='contents'><div class='textblock'>run<span class='membertext'>   runs the simulation   </span> 
-</div></div><div class='contents'><div class='textblock'>set</div></div><div class='contents'><div class='textblock'>prop</div></div><div class='contents'><div class='textblock'>sMeca</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#abc276d8f0be5c9306d78a96fe3f0bb3c">properties</a></div></div><div class='contents'><div class='textblock'>spaces</div></div><div class='contents'><div class='textblock'>spaces</div></div><div class='contents'><div class='textblock'>fields</div></div><div class='contents'><div class='textblock'>fibers</div></div><div class='contents'><div class='textblock'>spheres</div></div><div class='contents'><div class='textblock'>beads</div></div><div class='contents'><div class='textblock'>solids</div></div><div class='contents'><div class='textblock'>couples</div></div><div class='contents'><div class='textblock'>singles</div></div><div class='contents'><div class='textblock'>organizers</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#adee9554e2b226484bc4ad97738921c7e">remove</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a7469c8b960cb87d16c8eba8eb394df66">erase</a></div></div><div class='contents'><div class='textblock'>nuke</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a6fc92e0e88a1173babd33b596d8708b3">time</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#abd0d359bb6ab680bd594236024523982">time_step</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ac6bf1a12c5c98ddec5b65e07fe74cabe">step</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ab0380d45afea9d3e61fafa037813b88c">computeForces</a></div></div><div class='contents'><div class='textblock'>run</div></div><div class='contents'><div class='textblock'>change</div></div><div class='contents'><div class='textblock'>change_glos</div></div><div class='contents'><div class='textblock'>once</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ad6f453d4213e53f481790aeebf7d0218">prepared_solve</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ad73dc00fdaaf2b7c9ca0642761ec3ec8">prepare_meca</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a1825b40ca3bc3a1ba67fdb58fac5015c">prepare</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#af7d39f0eac0af0ed5785935ac72a1e7d">solve</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a2a12e3cfd714da39e7debdf79b26092f">solve_auto</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a8857182b8b3e917ffc87b00951ad8e36">dump</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ab467c1ecbdfff6b842c12d2330adb4cb">saveSystem</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a06546b83defb6adccda00cb02c1f5eb7">evaluate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'>findSpace</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ae239fb10694daf9db05092bcaae4cf04">rename</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a6a241606b95c6fc87e29b421e05a02a8">isCategory</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#afc9d6c25b56d0c550942ef3ddf1f30cb">findProperty</a></div></div><div class='contents'><div class='textblock'>writePropertiesTo</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a154828edf4c8ce031527f3a8c8860f2a">writeProperties</a></div></div><div class='contents'><div class='textblock'>writePropertiesToNoPrune</div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_mecapoint.html" target="_self">Mecapoint</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a25a2df970ceb94dcb93cda76db2ae3ea">set</a></div></div><div class='contents'><div class='textblock'>mecable</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a315419f26d3c59fa143b49b90a019049">valid</a></div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a91a9b6ce06bef6eb4b1821326126ffc9">pos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a147e754875d4485765ac6f4c95a59336">overlapping</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a50ff3e3d8eec65ec4cfaa1a44f7150ca">near</a></div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_interpolation.html" target="_self">Interpolation</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#ac8bb3912a3ce86b15842e79d0b421204">clear</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#afc73e9a784e97a810e37f01ebde54c7a">set</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a315419f26d3c59fa143b49b90a019049">valid</a></div></div><div class='contents'><div class='textblock'>mecable</div></div><div class='contents'><div class='textblock'>exact1</div></div><div class='contents'><div class='textblock'>exact2</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#ae29cb7b310f29ebf4339144694d26522">coef1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a93d94ab33cef0c62fa68b706a112ea70">coef2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a584e9899b630c45e6cc14c63da587b3f">coef</a></div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a91a9b6ce06bef6eb4b1821326126ffc9">pos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#ad2423055f6ad4c002f972ab37b512a5c">pos1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a599e435c9a8f18680ecd9c30ecd4dd95">pos2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a5ab2c008283f29ab4db80d13bcea3a15">diff</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a65be88abb82a600f90626f3c407f189c">len</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a441bfb1b33ab87ccea2a94acbf33b8e9">lenSqr</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a3997c1a68d3914a1e2af1cbf3bee000c">dir</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a231eaf39e8bfd3e5e212261bd087e8ed">inside</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a147e754875d4485765ac6f4c95a59336">overlapping</a></div></div><div class='contents'><div class='textblock'>overlapPoint</div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_meca.html" target="_self">Meca</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a00f46d823ada4eccd4c9fa1d7174a1d0">nb_points</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a75aa79248b769329ed6b7d62280aa08c">dimension</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ab835a572eb9c814cf49f0fa7d3b9916a">prepare</a></div></div><div class='contents'><div class='textblock'>addForcePt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a8c36d9df22beccf44aab4f03765275df">addForce</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a725e8b8b1e88c53fa1d428d8d9ddfcaf">addTorque</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ab07faf9b5bccbe926c197e90a3c506c2">addTorqueClamp</a></div></div><div class='contents'><div class='textblock'>addTorqueParrallel</div></div><div class='contents'><div class='textblock'>addTorqueAngle</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a6dc94321c28ab9975d777cddf69c9ec5">addTorquePoliti</a></div></div><div class='contents'><div class='textblock'>addPointClampPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a7179179a9bdcd12bce4af82e42958cb6">addPointClamp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ac00ca74a27cc0064f0611b63b132cdc3">addSphereClamp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a1588131f444ba29d78a29216a414d3b7">addCylinderClampZ</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#aa870055bd24ddc32647b14d965c59c0e">addCylinderClampX</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a6796012aec793f18ca396d96e5715e68">addSidePointClamp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ace08d61a7fecb37e4ab269afb2fea173">addLineClamp</a></div></div><div class='contents'><div class='textblock'>addLineClampPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a2548f1a83e94e5f8e8680ded8cebea37">addPlaneClamp</a></div></div><div class='contents'><div class='textblock'>addPlaneClampPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a28659b9ca1f5a0d59fdd29ea0d3fd9d0">addLink</a></div></div><div class='contents'><div class='textblock'>addLinkPtI</div></div><div class='contents'><div class='textblock'>addLinkIPt</div></div><div class='contents'><div class='textblock'>addLinkPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a52da1f3a6f9e9b3f357aa45a85ca7515">addLongLink</a></div></div><div class='contents'><div class='textblock'>addLongLinkPt</div></div><div class='contents'><div class='textblock'>addLongLinkPtI</div></div><div class='contents'><div class='textblock'>addSideLink2D</div></div><div class='contents'><div class='textblock'>addSideLink2DIPt</div></div><div class='contents'><div class='textblock'>addSideSideLink2D</div></div><div class='contents'><div class='textblock'>addSideSlidingLink2D</div></div><div class='contents'><div class='textblock'>addSideSlidingLink2DIPt</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkS</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkSIPt</div></div><div class='contents'><div class='textblock'>addSideLink3D</div></div><div class='contents'><div class='textblock'>addSideLinkS</div></div><div class='contents'><div class='textblock'>addSideLinkSIpt</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkS</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkSIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a1e56a74a63fd5319a0a46b196b682025">addSideLink</a></div></div><div class='contents'><div class='textblock'>addSideLinkIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ad3811b376eaa3ae617b3b6fd3b72c3d7">addSideSideLink</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a5ca9f81627da4be0a6da4674bb75585e">addSlidingLink</a></div></div><div class='contents'><div class='textblock'>addSlidingLinkIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a6b8794d6b2956b45d8dd87eef2f73a48">addSideSlidingLink</a></div></div><div class='contents'><div class='textblock'>addSideSlidingLinkIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#af7e036bd79e169e22676d34909fa5432">addTriLink</a></div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_object.html" target="_self">Object</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html#ac4676f3cc02884e13816f02297d87682">reference</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html#ace9ef785c9d0ec30f908396c5571652d">property</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_movable.html#ad624fda53a1713016ff082c46da88669">position</a></div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>__next__</div></div><div class='contents'><div class='textblock'>prev</div></div><div class='contents'><div class='textblock'>id</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html#aab41ee90c8599ea042c4843df912b00b">writeHeader</a></div></div><div class='contents'><div class='textblock'>points</div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_space.html" target="_self">Space</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a698861183e4cd233c0adc3eee628d911">thickness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ac30219811cfcb86e195477c165c18a5f">resize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a6fa3310f56de73e730b8050b5b8544c4">volume</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a6a7f066111371b55d909ce38791d841a">boundaries</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a8c90e38ceddbd5fbaf015263209642bc">inside</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ac5f310d4dcbd5aeea8104ab662a7bbb1">project</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a852c5e4cdf4f880461c23ee7e0c5f3c5">allInside</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a022f4e7547e8869994cbe798639344bd">allOutside</a></div></div><div class='contents'><div class='textblock'>toSpace</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a650154e5931ac28f374161f81313bd7d">max_extension</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a95caf802881b0cd12c56c58a59d4bb4d">projectDeflated</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a1d56de008507a862a0738c29b10c8b36">distanceToEdgeSqr</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#adced8eb2fc67ffdbf466a30f8f455f8c">distanceToEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a603c748be20553699fc2d52aa3e63de7">signedDistanceToEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a9cc94f7136747635b9d61a3114d0c5ba">bounce</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a20348398cd84dbf188287d06ccbcd289">normalToEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ab638802c149c21b952acdc28f56ef39a">randomPlace</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a5381a9546b0a8f860c83fbef32da2231">randomPlaceNearEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ac6f71047665796f6fdfccd301c580fe8">randomPlaceOnEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a684d9ae11971c7a91195af780e718f2c">estimateVolume</a></div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_couple.html" target="_self">Couple</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#af835342337022ce2d50420f766eda7f5">active</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#ac15de46b6db835d101cb026d3b00f050">stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a35671221583000fc2ddd7aa89257b5a0">force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a3699aaed45aca84acd573c5fc7193a14">cosAngle</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a922b3f3998f2e945d69c9a95a25066e5">sidePos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a0ecbd1ecf9a3d7b30719044ab87cef88">posFree</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#ac5d01183f3dea554080c7562141243ef">attachEnd1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#afa8e22aac660c824d21a17c59a3e2ac6">attachEnd2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#acbc2233baf1ebb2423709c2b84676342">moveToEnd1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#aacc63cae7f406dc44ed01e7528ca6e3c">moveToEnd2</a></div></div><div class='contents'><div class='textblock'>fiber2</div></div><div class='contents'><div class='textblock'>abcissa</div></div><div class='contents'><div class='textblock'>toCouple</div></div><div class='contents'><div class='textblock'>hand1</div></div><div class='contents'><div class='textblock'>hand2</div></div><div class='contents'><div class='textblock'>hand</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a6de3ae1bc365515f6970323b44d3d983">state</a></div></div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_organizer.html" target="_self">Organizer</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#aa68d1ed0efa1960c9665848614c80b74">nbOrganized</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#a592193b879b25cd2ecb649bfe57b964f">positionP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>prev</div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_aster.html" target="_self">Aster</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>solid</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a137b14b7e404c5036ad5479b4a91d74e">nbFibers</a></div></div><div class='contents'><div class='textblock'>fiber</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a0505c1142c7ecbf7568aa3507ad103c2">posLink1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a2f8269c5f717aafaa9532ec778fdd4c3">posLink2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a6c2153bd31bbb6e00f0e672a342620d0">posFiber1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a9ded7ba76407f8e77f9aa3e707462058">posFiber2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a33e055da50bc2afc1cae9284054c10a3">getLink1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a8e5151dadbb4978eac986046130a7636">getLink2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a4a4b50f68883ff81796082eeadf9df4e">getLink</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a5d9895c039bde2ea31c8ba069a31bc74">property</a></div></div></div></div> 
+</div></div></div><div class='directory'><div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>PyCytosim</div> <div class='directory' data-member><div class='contents'><div class='textblock'>open<span class='membertext'>  loads simulation from object files  </span> 
+</div></div><div class='contents'><div class='textblock'>start<span class='membertext'>  loads simulation from config files  </span> 
+</div></div><div class='contents'><div class='textblock'>str_to_glos<span class='membertext'>  converts string to Glossary  </span> 
+</div></div><div class='contents'><div class='textblock'>str_to_glos<span class='membertext'>  converts string to Glossary  </span> 
+</div></div><div class='contents'><div class='textblock'>toVector<span class='membertext'>  converts numpy array to vector  </span> 
+</div></div><div class='contents'><div class='textblock'>toTorque<span class='membertext'>  converts numpy array to torque  </span> 
+</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_object.html" target="_self">Object</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html#ac4676f3cc02884e13816f02297d87682">reference</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html#ace9ef785c9d0ec30f908396c5571652d">property</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_movable.html#ad624fda53a1713016ff082c46da88669">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'>__next__</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'>id</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html#aab41ee90c8599ea042c4843df912b00b">writeHeader</a></div></div><div class='contents'><div class='textblock'>points</div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_space.html" target="_self">Space</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a698861183e4cd233c0adc3eee628d911">thickness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ac30219811cfcb86e195477c165c18a5f">resize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a6fa3310f56de73e730b8050b5b8544c4">volume</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a6a7f066111371b55d909ce38791d841a">boundaries</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a8c90e38ceddbd5fbaf015263209642bc">inside</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ac5f310d4dcbd5aeea8104ab662a7bbb1">project</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a852c5e4cdf4f880461c23ee7e0c5f3c5">allInside</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a022f4e7547e8869994cbe798639344bd">allOutside</a></div></div><div class='contents'><div class='textblock'>toSpace</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a650154e5931ac28f374161f81313bd7d">max_extension</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a95caf802881b0cd12c56c58a59d4bb4d">projectDeflated</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a1d56de008507a862a0738c29b10c8b36">distanceToEdgeSqr</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#adced8eb2fc67ffdbf466a30f8f455f8c">distanceToEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a603c748be20553699fc2d52aa3e63de7">signedDistanceToEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a9cc94f7136747635b9d61a3114d0c5ba">bounce</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a20348398cd84dbf188287d06ccbcd289">normalToEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ab638802c149c21b952acdc28f56ef39a">randomPlace</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a5381a9546b0a8f860c83fbef32da2231">randomPlaceNearEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ac6f71047665796f6fdfccd301c580fe8">randomPlaceOnEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a684d9ae11971c7a91195af780e718f2c">estimateVolume</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_mecable.html" target="_self">Mecable</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#aa073fce85239bcb6a3104b9e72055161">data</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a289e74a02e184e27a71ce1adf3883bf1">nbPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a8bc3e142a14a07815b29e230cefacd3e">allocated</a></div></div><div class='contents'><div class='textblock'>points<span class='membertext'>   Returns read-only point coordinates of the mecable  </span> 
+</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a030f8164696551d58123cf373655d9ce">posPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#abb809f1939f978a9abdbc3e49a1e87d0">setPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#abb809f1939f978a9abdbc3e49a1e87d0">setPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a720e68bfecf70eabf91384fc2af4aaff">addPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#adbd23bceacee22d13226a020a9ccb23b">removePoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a54d93424ae45b23df413c5cfd5820b79">clearPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a9c0978f6f953be030e66be7629d18a8a">shiftPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a07b95fbcb40cb557ad282af05689c6da">truncateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#ae6d6812c7ec1a56e590ba5559736b1c2">truncateP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a26827539688fc54c4bf1474a8b3f3f1c">calculateMomentum</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a1b27ae44a7c7b1f924d54695bc1a7641">netForce</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a1dba38e58fd08f3f70d4a521cd904577">translate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a124d881969afe4378d1d36c1a9fc6916">allInside</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_sphere.html" target="_self">Sphere</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'>pos</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a66f8268c3614689bddb7e9508ec50abb">Sphere</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a9e4bd1a51f41a59e059adc7fccb4cc4c">resize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a63b5230e86ff1b3d58cfe70429fe4956">reshape</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a0301a31b9d311381e37a1c41406248d3">orthogonalize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#aa61b3e120c4324b62f1fe42a3ce95ed1">addSurfacePoint</a></div></div><div class='contents'><div class='textblock'>nbbSurfacePoints</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html">Sphere</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html">Sphere</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html">Sphere</a></div></div></div></div> 
+<div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_bead.html" target="_self">Bead</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a205d3670324a950673bb464cd507827e">Bead</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a224123905bed58e68a4b277eb4b6c289">setPosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#afc6e66e226b54ad058211db1a9ea3acc">radius</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a0756681ed4cffa41dcbec5825eea0765">radiusSqr</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a5199eca3fe77f7dffd1e6b44605f15fe">resize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a7345ca77d5e0a1371c7373786d650ef2">volume</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html">Bead</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html">Bead</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html">Bead</a></div></div></div></div> 
+<div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_chain.html" target="_self">Chain</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ade97cb1630fbb84f8937e872632fff1c">nbSegments</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a0055db6e3444cfdd7783663d206a87c0">lastSegment</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a62249a99fd0a422d8766e4bf63c3d554">setStraight</a></div></div><div class='contents'><div class='textblock'>setStraightLength</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a853f22938de7a0d33597587da11da092">placeEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a4edb26c5275b8ee111af7b4177efe826">setEquilibrated</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a1930a9adf88969fc4b7b15cf9fe7108a">birthTime</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a19411a4cc4b0381e06007ccb8eb27e9b">age</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html">Mecapoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'>interpolateFromEnd</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a4edb26c5275b8ee111af7b4177efe826">setEquilibrated</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a9ec30ab32a36e4c0e678cc53311599d7">length1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a794290003b8229b0e5427e2472ed97e2">trueLength</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a149e71e7a76b780e37b8bbc59ef72d7f">betweenMP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a8138c56ab72b0cb3cc342fd2604847ae">outsideMP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ac46cb99bde6530da54ab9046be9310a8">belowP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad1377568e189c84519e58e5506dafd4b">aboveM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#a6cc8f8124cf3efec82ea724346597dde">FiberEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad30f5d0f543f0fe757e82d931046cab9">clampedIndexM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad0d77e016a5c4f7683ddea47b8692d9f">setOrigin</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a2395c6041facb79aadf409637ec59172">abscissaM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a5113c828524ceb520533d984abc54a74">abscissaC</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#afc94966444dc56109d43a0e9a9a84aea">abscissaP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a043e4b9942be8d992caf7c0c33df7989">abscissaPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ab53240451117802d75bdf4ce8bfff5ff">abscissaEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a1663517f441656976661844bff51a75e">abscissaFrom</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aef30f06e27bda8676062c876aab50288">someAbscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a9556ce5e695f7af85f0ea3706b6121f6">posM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a62249a99fd0a422d8766e4bf63c3d554">setStraight</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a70ed4893ded81126c279dbf86bde029c">posFrom</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a3d95856990f79cd338e73f8d0a1a9db4">posMiddle</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a127a26975c292b6a951ef378728e53ff">posEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#acb5765074baf5abb14cb2e0967b351a3">posEndP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#adbab2f3e6fb1662a6f4a4ee9fc36ab95">posEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aeee12a9eb9f3b9862cc9a615dd7a2287">netForceEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad642529b9e17cf07bc3cd6744f675dee">netForceEndP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aa6c712d0987324e96e2bf7d9fca31afc">projectedForceEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ab68a15d872cf86dec8bc883407bb00f5">projectedForceEndP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aa6c712d0987324e96e2bf7d9fca31afc">projectedForceEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a6408a7cbd00fadc0db10ef528e9bb5a9">avgDirection</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a17598f35c35f991a317071b9edb718d1">segmentation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a43e24153dfb4b2be1437dc48bab618ed">flipChainPolarity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#af45fb76a686d5bf3ed398bc70966f1c5">curvature</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aab47087140d4066eec10338eb203a9d8">bendingEnergy0</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#af6e0e170e1cac14151a76628ccaa49aa">planarIntersect</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#acd775993f2e15a2905bb6cbf5bbf5d07">growM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aadc04c51e3184c13ca74473262672f34">addSegmentM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a2c9dc9b22febc0b83cf2bc691c7f5b3f">cutM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a92308cf0ac8c65cb2c3bb1dffc5c5e19">growP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a5ddc78be861218a4d511580c0561afa7">addSegmentP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a33f46f9d38054801961d95a7032971fa">cutP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a66c42f788e7d0f2641e79c28daaa0cf2">grow</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a6f74d2a21a83c31983142e2e73734523">adjustLength</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a999f75df61342bbc6b4d6fa5c1cb2cfe">truncateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aa7ccc502af2dfadf28c36bdf67f6860f">truncateP</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-4 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_mecafil.html" target="_self">Mecafil</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecafil.html#af86966d8cc47fe44b15bd6e55dc6bcae">tension</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecafil.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecafil.html#aec775e777f2888a830cf2e7270930a55">leftoverMobility</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-5 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber.html" target="_self">Fiber</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>points</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a289e74a02e184e27a71ce1adf3883bf1">nbPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a8855988fb953c48f770d7da5e7d8fcbe">cutM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#afcbe3a24c88dfd97abd739e3b468dc43">cutP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a1485fd899f48f7395627a6c78ecc1071">sever</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a6cea692446c106c98789f2f20853918b">severNow</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a4387b72a2db3733dfec1b10b9c20af42">join</a></div></div><div class='contents'><div class='textblock'>stateM</div></div><div class='contents'><div class='textblock'>stateP</div></div><div class='contents'><div class='textblock'>setStateM</div></div><div class='contents'><div class='textblock'>setStateP</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a3a495090170d36b3da6c7cd95f53ae86">setDynamicState</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a0702bb0654fa4fceaf3cbae366b832a8">freshAssembly</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a7dfc07cca7d08be5a84bc1e3259902b3">nbHands</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#aa7383b1a4473b50c50edec33bfcda435">addHand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#adeb3c522f7304851881551707dcc4706">removeHand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a1b9467c7cc981f10085c131d0d2bbad7">updateHands</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a33d23ba81d903c935822468735f908d8">detachHands</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#ad17baf33afac710aa199eaead637d6c6">sortHands</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#ac8a4e8f2c4d61aaf91171d20b101dcc2">nbHandsInRange</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a0874dfd020a5bd0a6e49f2991b0d1a7b">nbHandsNearEnd</a></div></div><div class='contents'><div class='textblock'>__next__</div></div></div><div class='directory'><div class='contents' data-class data-depth-6 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_classic_fiber.html" target="_self">ClassicFiber</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_classic_fiber.html#a6a0c10d4ee0fb78722c7fee2d4806b9c">freshAssemblyM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_classic_fiber.html#ae0f68d2181b1a6d3fd9edda105cb1412">freshAssemblyP</a></div></div></div></div> 
+<div class='contents' data-class data-depth-6 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_dynamic_fiber.html" target="_self">DynamicFiber</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_dynamic_fiber.html#a6a0c10d4ee0fb78722c7fee2d4806b9c">freshAssemblyM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_dynamic_fiber.html#ae0f68d2181b1a6d3fd9edda105cb1412">freshAssemblyP</a></div></div></div></div> 
 </div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_mecable.html" target="_self">Mecable</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#aa073fce85239bcb6a3104b9e72055161">data</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a289e74a02e184e27a71ce1adf3883bf1">nbPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a8bc3e142a14a07815b29e230cefacd3e">allocated</a></div></div><div class='contents'><div class='textblock'>points</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a030f8164696551d58123cf373655d9ce">posPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#abb809f1939f978a9abdbc3e49a1e87d0">setPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#abb809f1939f978a9abdbc3e49a1e87d0">setPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a720e68bfecf70eabf91384fc2af4aaff">addPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#adbd23bceacee22d13226a020a9ccb23b">removePoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a54d93424ae45b23df413c5cfd5820b79">clearPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a9c0978f6f953be030e66be7629d18a8a">shiftPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a07b95fbcb40cb557ad282af05689c6da">truncateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#ae6d6812c7ec1a56e590ba5559736b1c2">truncateP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a26827539688fc54c4bf1474a8b3f3f1c">calculateMomentum</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a1b27ae44a7c7b1f924d54695bc1a7641">netForce</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a1dba38e58fd08f3f70d4a521cd904577">translate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a124d881969afe4378d1d36c1a9fc6916">allInside</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_chain.html" target="_self">Chain</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ade97cb1630fbb84f8937e872632fff1c">nbSegments</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a0055db6e3444cfdd7783663d206a87c0">lastSegment</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a62249a99fd0a422d8766e4bf63c3d554">setStraight</a></div></div><div class='contents'><div class='textblock'>setStraightLength</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a853f22938de7a0d33597587da11da092">placeEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a4edb26c5275b8ee111af7b4177efe826">setEquilibrated</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a1930a9adf88969fc4b7b15cf9fe7108a">birthTime</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a19411a4cc4b0381e06007ccb8eb27e9b">age</a></div></div><div class='contents'><div class='textblock'>exactEnd</div></div><div class='contents'><div class='textblock'>interpolateEndM</div></div><div class='contents'><div class='textblock'>interpolateEndP</div></div><div class='contents'><div class='textblock'>interpolateCenter</div></div><div class='contents'><div class='textblock'>interpolateEnd</div></div><div class='contents'><div class='textblock'>interpolateFromEnd</div></div><div class='contents'><div class='textblock'>interpolate</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a4edb26c5275b8ee111af7b4177efe826">setEquilibrated</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a9ec30ab32a36e4c0e678cc53311599d7">length1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a794290003b8229b0e5427e2472ed97e2">trueLength</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a149e71e7a76b780e37b8bbc59ef72d7f">betweenMP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a8138c56ab72b0cb3cc342fd2604847ae">outsideMP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ac46cb99bde6530da54ab9046be9310a8">belowP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad1377568e189c84519e58e5506dafd4b">aboveM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#a6cc8f8124cf3efec82ea724346597dde">FiberEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad30f5d0f543f0fe757e82d931046cab9">clampedIndexM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad0d77e016a5c4f7683ddea47b8692d9f">setOrigin</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a2395c6041facb79aadf409637ec59172">abscissaM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a5113c828524ceb520533d984abc54a74">abscissaC</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#afc94966444dc56109d43a0e9a9a84aea">abscissaP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a043e4b9942be8d992caf7c0c33df7989">abscissaPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ab53240451117802d75bdf4ce8bfff5ff">abscissaEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a1663517f441656976661844bff51a75e">abscissaFrom</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aef30f06e27bda8676062c876aab50288">someAbscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a9556ce5e695f7af85f0ea3706b6121f6">posM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a62249a99fd0a422d8766e4bf63c3d554">setStraight</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a70ed4893ded81126c279dbf86bde029c">posFrom</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a3d95856990f79cd338e73f8d0a1a9db4">posMiddle</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a127a26975c292b6a951ef378728e53ff">posEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#acb5765074baf5abb14cb2e0967b351a3">posEndP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#adbab2f3e6fb1662a6f4a4ee9fc36ab95">posEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aeee12a9eb9f3b9862cc9a615dd7a2287">netForceEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad642529b9e17cf07bc3cd6744f675dee">netForceEndP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aa6c712d0987324e96e2bf7d9fca31afc">projectedForceEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ab68a15d872cf86dec8bc883407bb00f5">projectedForceEndP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aa6c712d0987324e96e2bf7d9fca31afc">projectedForceEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a6408a7cbd00fadc0db10ef528e9bb5a9">avgDirection</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a17598f35c35f991a317071b9edb718d1">segmentation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a43e24153dfb4b2be1437dc48bab618ed">flipChainPolarity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#af45fb76a686d5bf3ed398bc70966f1c5">curvature</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aab47087140d4066eec10338eb203a9d8">bendingEnergy0</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#af6e0e170e1cac14151a76628ccaa49aa">planarIntersect</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#acd775993f2e15a2905bb6cbf5bbf5d07">growM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aadc04c51e3184c13ca74473262672f34">addSegmentM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a2c9dc9b22febc0b83cf2bc691c7f5b3f">cutM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a92308cf0ac8c65cb2c3bb1dffc5c5e19">growP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a5ddc78be861218a4d511580c0561afa7">addSegmentP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a33f46f9d38054801961d95a7032971fa">cutP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a66c42f788e7d0f2641e79c28daaa0cf2">grow</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a6f74d2a21a83c31983142e2e73734523">adjustLength</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a999f75df61342bbc6b4d6fa5c1cb2cfe">truncateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aa7ccc502af2dfadf28c36bdf67f6860f">truncateP</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_mecafil.html" target="_self">Mecafil</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecafil.html#af86966d8cc47fe44b15bd6e55dc6bcae">tension</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecafil.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecafil.html#aec775e777f2888a830cf2e7270930a55">leftoverMobility</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-4 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber.html" target="_self">Fiber</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>points</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a289e74a02e184e27a71ce1adf3883bf1">nbPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a8855988fb953c48f770d7da5e7d8fcbe">cutM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#afcbe3a24c88dfd97abd739e3b468dc43">cutP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a1485fd899f48f7395627a6c78ecc1071">sever</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a6cea692446c106c98789f2f20853918b">severNow</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'>nowSever</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a4387b72a2db3733dfec1b10b9c20af42">join</a></div></div><div class='contents'><div class='textblock'>stateM</div></div><div class='contents'><div class='textblock'>stateP</div></div><div class='contents'><div class='textblock'>setStateM</div></div><div class='contents'><div class='textblock'>setStateP</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a3a495090170d36b3da6c7cd95f53ae86">setDynamicState</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a0702bb0654fa4fceaf3cbae366b832a8">freshAssembly</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a7dfc07cca7d08be5a84bc1e3259902b3">nbHands</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#ac8a4e8f2c4d61aaf91171d20b101dcc2">nbHandsInRange</a></div></div><div class='contents'><div class='textblock'>__next__</div></div></div><div class='directory'><div class='contents' data-class data-depth-5 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_classic_fiber.html" target="_self">ClassicFiber</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_classic_fiber.html#a6a0c10d4ee0fb78722c7fee2d4806b9c">freshAssemblyM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_classic_fiber.html#ae0f68d2181b1a6d3fd9edda105cb1412">freshAssemblyP</a></div></div></div></div> 
 </div></div> 
 </div></div> 
 </div></div> 
-<div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_sphere.html" target="_self">Sphere</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'>pos</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a66f8268c3614689bddb7e9508ec50abb">Sphere</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a9e4bd1a51f41a59e059adc7fccb4cc4c">resize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a63b5230e86ff1b3d58cfe70429fe4956">reshape</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a0301a31b9d311381e37a1c41406248d3">orthogonalize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#aa61b3e120c4324b62f1fe42a3ce95ed1">addSurfacePoint</a></div></div><div class='contents'><div class='textblock'>nbbSurfacePoints</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>prev</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html">Sphere</a></div></div></div></div> 
-<div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_bead.html" target="_self">Bead</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a205d3670324a950673bb464cd507827e">Bead</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a224123905bed58e68a4b277eb4b6c289">setPosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#afc6e66e226b54ad058211db1a9ea3acc">radius</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a0756681ed4cffa41dcbec5825eea0765">radiusSqr</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a5199eca3fe77f7dffd1e6b44605f15fe">resize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a7345ca77d5e0a1371c7373786d650ef2">volume</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>prev</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html">Bead</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_solid.html" target="_self">Solid</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'>points</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#ab4d58012b7bc78b8c0a1efa482acaf84">addSphere</a></div></div><div class='contents'><div class='textblock'>setRadius</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#ab4d58012b7bc78b8c0a1efa482acaf84">addSphere</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#af6a9acdfad3dd47796dd317cca2d5560">centroid</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html">Solid</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html">Solid</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#ae6fb4d0b832ee89eb207dd98da5865ed">tag</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#a5d9895c039bde2ea31c8ba069a31bc74">property</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a289e74a02e184e27a71ce1adf3883bf1">nbPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html">Solid</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_organizer.html" target="_self">Organizer</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#aa68d1ed0efa1960c9665848614c80b74">nbOrganized</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#a592193b879b25cd2ecb649bfe57b964f">positionP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html">Organizer</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html">Organizer</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_aster.html" target="_self">Aster</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html">Solid</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a137b14b7e404c5036ad5479b4a91d74e">nbFibers</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a0505c1142c7ecbf7568aa3507ad103c2">posLink1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a2f8269c5f717aafaa9532ec778fdd4c3">posLink2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a6c2153bd31bbb6e00f0e672a342620d0">posFiber1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a9ded7ba76407f8e77f9aa3e707462058">posFiber2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a33e055da50bc2afc1cae9284054c10a3">getLink1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a8e5151dadbb4978eac986046130a7636">getLink2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a4a4b50f68883ff81796082eeadf9df4e">getLink</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a5d9895c039bde2ea31c8ba069a31bc74">property</a></div></div></div></div> 
 </div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_solid.html" target="_self">Solid</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'>points</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#ab4d58012b7bc78b8c0a1efa482acaf84">addSphere</a></div></div><div class='contents'><div class='textblock'>setRadius</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#ab4d58012b7bc78b8c0a1efa482acaf84">addSphere</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#af6a9acdfad3dd47796dd317cca2d5560">centroid</a></div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>prev</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#ae6fb4d0b832ee89eb207dd98da5865ed">tag</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#a5d9895c039bde2ea31c8ba069a31bc74">property</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a289e74a02e184e27a71ce1adf3883bf1">nbPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html">Solid</a></div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_single.html" target="_self">Single</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>toSingle</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a6de3ae1bc365515f6970323b44d3d983">state</a></div></div><div class='contents'><div class='textblock'>__getitem__</div></div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'>hand</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html" title="A point-like object containing one Hand. ">Single</a></div></div><div class='contents'><div class='textblock'>fiber</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#acd4ae97f5dd9516b38df9cad09f5a54e">abscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac32af0048104e04b946190884239b681">posHand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#abb4674e86652b8145df4f947634f446a">dirFiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a0cc627377931cdb970f6c9da2fe2975c">attach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ae5949466ed8951a7c706095e9c41a833">attachEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac61bdddfe1f2437d88bf92041af4df36">moveToEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac295bade8aee589f6718dfa79edc2a34">detach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a55bb5045e5a6cce3e45c6a04821f99e8">mobile</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#af9c87a998410f54900993d5add04e78f">translate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#abbcf4a043ead606e034072c253caf18f">setPosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a243a4ae5e156567d0241de936986b336">randomizePosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac9b487785e64912d738b5d886944839c">posFoot</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a922b3f3998f2e945d69c9a95a25066e5">sidePos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a55bb5045e5a6cce3e45c6a04821f99e8">mobile</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a318425477b2d6704ff1de4d37c9a391a">force</a></div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>prev</div></div><div class='contents'><div class='textblock'>confineSpace</div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_couple.html" target="_self">Couple</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#af835342337022ce2d50420f766eda7f5">active</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#ac15de46b6db835d101cb026d3b00f050">stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a35671221583000fc2ddd7aa89257b5a0">force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a3699aaed45aca84acd573c5fc7193a14">cosAngle</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a922b3f3998f2e945d69c9a95a25066e5">sidePos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a0ecbd1ecf9a3d7b30719044ab87cef88">posFree</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#ac5d01183f3dea554080c7562141243ef">attachEnd1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#afa8e22aac660c824d21a17c59a3e2ac6">attachEnd2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#acbc2233baf1ebb2423709c2b84676342">moveToEnd1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#aacc63cae7f406dc44ed01e7528ca6e3c">moveToEnd2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'>abcissa</div></div><div class='contents'><div class='textblock'>toCouple</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'>hand</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a6de3ae1bc365515f6970323b44d3d983">state</a></div></div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_single.html" target="_self">Single</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>toSingle</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a6de3ae1bc365515f6970323b44d3d983">state</a></div></div><div class='contents'><div class='textblock'>__getitem__</div></div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html" title="A point-like object containing one Hand.">Single</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#acd4ae97f5dd9516b38df9cad09f5a54e">abscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac32af0048104e04b946190884239b681">posHand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#abb4674e86652b8145df4f947634f446a">dirFiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a0cc627377931cdb970f6c9da2fe2975c">attach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ae5949466ed8951a7c706095e9c41a833">attachEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac61bdddfe1f2437d88bf92041af4df36">moveToEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac295bade8aee589f6718dfa79edc2a34">detach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a55bb5045e5a6cce3e45c6a04821f99e8">mobile</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#af9c87a998410f54900993d5add04e78f">translate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#abbcf4a043ead606e034072c253caf18f">setPosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a243a4ae5e156567d0241de936986b336">randomizePosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac9b487785e64912d738b5d886944839c">posFoot</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a922b3f3998f2e945d69c9a95a25066e5">sidePos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a55bb5045e5a6cce3e45c6a04821f99e8">mobile</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a318425477b2d6704ff1de4d37c9a391a">force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html">Single</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html">Single</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html">Space</a></div></div></div></div> 
 </div></div> 
 <div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Property</div> <div class='directory' data-member><div class='contents'><div class='textblock'>name</div></div><div class='contents'><div class='textblock'>change</div></div><div class='contents'><div class='textblock'>read</div></div><div class='contents'><div class='textblock'>change_glos</div></div><div class='contents'><div class='textblock'>read_glos</div></div><div class='contents'><div class='textblock'>complete</div></div><div class='contents'><div class='textblock'>rename</div></div><div class='contents'><div class='textblock'>is_named</div></div><div class='contents'><div class='textblock'>number</div></div><div class='contents'><div class='textblock'>renumber</div></div><div class='contents'><div class='textblock'>clear</div></div><div class='contents'><div class='textblock'>clone</div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_space_prop.html" target="_self">SpaceProp</a></div> </div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_couple_prop.html" target="_self">CoupleProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga103de20cbd1e6b0cda8f5a2a17df575d">hand1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gaea9b1d8250cb587f3e6e90e627422adf">hand2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga575ccdd0e4c30d7c82343fe313533356">stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga780020b647987365a5a7280ba79e059c">length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gab69c79ec9456e615f41c6af1850da983">diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gad988df56af78ff8a949fa43aa279aa34">fast_diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga0c8c31e73b2b393e04b4c033ca8a8869">stiff</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple_prop.html#a2b6018f958ecd9fd2574082f0b6dfd07">Specificity</a></div></div><div class='contents'><div class='textblock'>confine</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'>hand1_prop</div></div><div class='contents'><div class='textblock'>hand2_prop</div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber_prop.html" target="_self">FiberProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gae9cb302aee80c6b6d700bb819563da67">segmentation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaa49d9ce314729739966f40e3babfaf0e">rigidity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga1cfafcb5a4f95cab8630811ed1234a84">min_length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga6a22df6cc0302e9b9c67c82ed5a1fd3e">max_length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga6ef4a1d00af970a715d4420c21471ed4">total_polymer</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaea39f2c5cb5ec83de4d1f81b1a74f0cc">persistent</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga816f13f493c4ad26b49e715afa17632c">viscosity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga1d7c289df62d5cc769290fa173b69e44">drag_radius</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga21239f90a6fb2c0842046344691b33a6">drag_length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga962259ef18b27c2066e2625b07f6d314">drag_model</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga4cec2aa9e2f2ed945c3a40b892de5f70">drag_gap</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaba923853d8f165530e05df9a8ff3079a">binding_key</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga94b59d3ee243a20d8fb40a2bac66eeba">lattice</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gab25be625ee763a05b85e0a24ad8315a1">lattice_unit</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#ae05f8c1156eea5e8bd6a9fbf181b4134">Confinement</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaef88f3cd69d3efb00fa13ff79b602495">confine_stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga09ca671af9b8e13dc8212fd14b76ea2d">steric</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gad7a5acf48cf8480363e97fa9ee005bbe">steric_radius</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga79a65a48123b5fdbee499f5bd550e870">steric_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gacea5b6e35581d9d8dbf04647b05a6ee3">glue</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gacc919e6961fd8baa1c313552037d8f4e">glue_single</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_prop.html#a207131365a7c95b985fbb3ac841a1472">display_fresh</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_solid_prop.html" target="_self">SolidProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga1c9993dba2c798ab1e7216211d54210f">drag</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga816f13f493c4ad26b49e715afa17632c">viscosity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga09ca671af9b8e13dc8212fd14b76ea2d">steric</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga79a65a48123b5fdbee499f5bd550e870">steric_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#ae05f8c1156eea5e8bd6a9fbf181b4134">Confinement</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#gaef88f3cd69d3efb00fa13ff79b602495">confine_stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid_prop.html#a207131365a7c95b985fbb3ac841a1472">display_fresh</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_hand_prop.html" target="_self">HandProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#gaf0ab51c3ebb07f8a0204ec2fa84ba84c">binding_rate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html" title="Simulates the stochastic binding/unbinding of a FiberSite.">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#gaba923853d8f165530e05df9a8ff3079a">binding_key</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga6f7c89db19de7c19666fe34515cc091c">unbinding_rate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#gada5f3500c0056c48d814c7445eb16b66">unbinding_force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga11a9781744f0e9667f43f3ae78fe31b9">bind_also_end</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga727176c11f75111ffb56dd11b279a3ed">bind_end_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga780e1719024062c6f4cc4dfc4d0d09a9">hold_growing_end</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga0f816ba324afa2c1d3517efa23b9d662">hold_shrinking_end</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_motor_prop.html" target="_self">MotorProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___motor_par.html#ga22d593fb145923c1d6b08bec61ef807e">stall_force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___motor_par.html#ga46b808e3b9bb7a8f717979fcc735dd41">unloaded_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___motor_par.html#ga094300e05909448478c30cb6511a7429">limit_speed</a></div></div></div></div> 
+</div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber_prop.html" target="_self">FiberProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gae9cb302aee80c6b6d700bb819563da67">segmentation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaa49d9ce314729739966f40e3babfaf0e">rigidity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga1cfafcb5a4f95cab8630811ed1234a84">min_length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga6a22df6cc0302e9b9c67c82ed5a1fd3e">max_length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga6ef4a1d00af970a715d4420c21471ed4">total_polymer</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaea39f2c5cb5ec83de4d1f81b1a74f0cc">persistent</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga816f13f493c4ad26b49e715afa17632c">viscosity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga1d7c289df62d5cc769290fa173b69e44">drag_radius</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga21239f90a6fb2c0842046344691b33a6">drag_length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga962259ef18b27c2066e2625b07f6d314">drag_model</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga4cec2aa9e2f2ed945c3a40b892de5f70">drag_gap</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaba923853d8f165530e05df9a8ff3079a">binding_key</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga94b59d3ee243a20d8fb40a2bac66eeba">lattice</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gab25be625ee763a05b85e0a24ad8315a1">lattice_unit</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#ae05f8c1156eea5e8bd6a9fbf181b4134">Confinement</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaef88f3cd69d3efb00fa13ff79b602495">confine_stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga09ca671af9b8e13dc8212fd14b76ea2d">steric</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gad7a5acf48cf8480363e97fa9ee005bbe">steric_radius</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga79a65a48123b5fdbee499f5bd550e870">steric_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gacea5b6e35581d9d8dbf04647b05a6ee3">glue</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gacc919e6961fd8baa1c313552037d8f4e">glue_single</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_prop.html#a207131365a7c95b985fbb3ac841a1472">display_fresh</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_classic_fiber_prop.html" target="_self">ClassicFiberProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___classic_fiber_par.html#gae1f11153d0c02e5450e7bd0da081fc05">growing_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___classic_fiber_par.html#ga631bd8742a85fff733d22f410b18621b">growing_off_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___classic_fiber_par.html#ga9c8e5e8ca707b087e73f4848f27b6f11">growing_force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___classic_fiber_par.html#gacf8a42c4e207c11bfeef6dc5254151f1">shrinking_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___classic_fiber_par.html#ga1d29395da00ae2c6e4f8d414436ad2bb">catastrophe_rate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___classic_fiber_par.html#ga3e72a845d13f65d7e3b12109d8b09798">catastrophe_rate_stalled</a></div></div></div></div> 
+<div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_dynamic_fiber_prop.html" target="_self">DynamicFiberProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___dynamic_fiber_par.html#gae1f11153d0c02e5450e7bd0da081fc05">growing_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___dynamic_fiber_par.html#ga631bd8742a85fff733d22f410b18621b">growing_off_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___dynamic_fiber_par.html#ga9c8e5e8ca707b087e73f4848f27b6f11">growing_force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___dynamic_fiber_par.html#gacf8a42c4e207c11bfeef6dc5254151f1">shrinking_speed</a></div></div></div></div> 
+</div></div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_simul_prop.html" target="_self">SimulProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#gaf1d4f29e7f0a2828126f4ea8335d7f17">time</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga5873848f9003055866bb6647374432ce">time_step</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga816f13f493c4ad26b49e715afa17632c">viscosity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#gafe75f1fd9847dfd7826e89caeeeab9dc">kT</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga73b7915f7d7ae31cd8261f404d3a8c74">tolerance</a></div></div><div class='contents'><div class='textblock'>acceptable_prop</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga1d0898295332ea1b58d9d7a2aac435e1">precondition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga09ca671af9b8e13dc8212fd14b76ea2d">steric</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#gac3589077a5077b9460edecd1959960b3">steric_stiffness_push</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#gaada6e15bcd71e84fd762ee7a40795a88">steric_stiffness_pull</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga4bd197701fe216bc11ef724536ac227a">steric_max_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga0f3dfd0699cf7d2ac133531edda2e48e">binding_grid_step</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga0b2caeb4b6f130be43e5a2f0267dd453">verbose</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga2352c06fef330221367dcff7715a071f">config_file</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#gaaf200c91c2dace9dcf3d8cca17a51227">property_file</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga9cb0feeca84b787e8d246988bc280a63">trajectory_file</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga37d87007b0e0ee8974b6875dea667066">clear_trajectory</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#gab49370f739a445ca87df438259a86964">skip_free_couple</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul_prop.html#a207131365a7c95b985fbb3ac841a1472">display_fresh</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul_prop.html#a79302f6d5ed23c67123fb65933b76990">read</a></div></div><div class='contents'><div class='textblock'>read_str</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul_prop.html#a33900dad01a57f50ce4e494b5758321f">clone</a></div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_hand_prop.html" target="_self">HandProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#gaf0ab51c3ebb07f8a0204ec2fa84ba84c">binding_rate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html" title="Simulates the stochastic binding/unbinding of a FiberSite. ">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#gaba923853d8f165530e05df9a8ff3079a">binding_key</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga6f7c89db19de7c19666fe34515cc091c">unbinding_rate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#gada5f3500c0056c48d814c7445eb16b66">unbinding_force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga11a9781744f0e9667f43f3ae78fe31b9">bind_also_end</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga727176c11f75111ffb56dd11b279a3ed">bind_end_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga780e1719024062c6f4cc4dfc4d0d09a9">hold_growing_end</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga0f816ba324afa2c1d3517efa23b9d662">hold_shrinking_end</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_motor_prop.html" target="_self">MotorProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___motor_par.html#ga22d593fb145923c1d6b08bec61ef807e">stall_force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___motor_par.html#ga46b808e3b9bb7a8f717979fcc735dd41">unloaded_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___motor_par.html#ga094300e05909448478c30cb6511a7429">limit_speed</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_couple_prop.html" target="_self">CoupleProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga103de20cbd1e6b0cda8f5a2a17df575d">hand1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gaea9b1d8250cb587f3e6e90e627422adf">hand2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga575ccdd0e4c30d7c82343fe313533356">stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga780020b647987365a5a7280ba79e059c">length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gab69c79ec9456e615f41c6af1850da983">diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gad988df56af78ff8a949fa43aa279aa34">fast_diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga0c8c31e73b2b393e04b4c033ca8a8869">stiff</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple_prop.html#a2b6018f958ecd9fd2574082f0b6dfd07">Specificity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#ae05f8c1156eea5e8bd6a9fbf181b4134">Confinement</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand_prop.html">HandProp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand_prop.html">HandProp</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_single_prop.html" target="_self">SingleProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gace8fe07b79d67d0ce0564806f65e4b90">hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#ga575ccdd0e4c30d7c82343fe313533356">stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#ga780020b647987365a5a7280ba79e059c">length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gab69c79ec9456e615f41c6af1850da983">diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gad988df56af78ff8a949fa43aa279aa34">fast_diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#ae05f8c1156eea5e8bd6a9fbf181b4134">Confinement</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand_prop.html">HandProp</a></div></div></div></div> 
 </div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_solid_prop.html" target="_self">SolidProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga1c9993dba2c798ab1e7216211d54210f">drag</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga816f13f493c4ad26b49e715afa17632c">viscosity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga09ca671af9b8e13dc8212fd14b76ea2d">steric</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga79a65a48123b5fdbee499f5bd550e870">steric_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#ae05f8c1156eea5e8bd6a9fbf181b4134">Confinement</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#gaef88f3cd69d3efb00fa13ff79b602495">confine_stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid_prop.html#a207131365a7c95b985fbb3ac841a1472">display_fresh</a></div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_single_prop.html" target="_self">SingleProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gace8fe07b79d67d0ce0564806f65e4b90">hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#ga575ccdd0e4c30d7c82343fe313533356">stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#ga780020b647987365a5a7280ba79e059c">length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gab69c79ec9456e615f41c6af1850da983">diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gad988df56af78ff8a949fa43aa279aa34">fast_diffusion</a></div></div><div class='contents'><div class='textblock'>confine</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'>hand_prop</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_interface.html" target="_self">Interface</a></div> <div class='directory' data-member><div class='classcomment'> an interface to cytosim </div><div class='contents'><div class='textblock'>add<span class='membertext'>   adds objects to simulation, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interface.html#a1009a882e99e8e20c9acb7f7f8689584">execute_new</a><span class='membertext'>   adds objects to simulation, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'>run<span class='membertext'>   runs simulation a given number of steps, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interface.html#ae6c1ea315d29b9483ed924622c379b90">execute_run</a><span class='membertext'>   runs simulation a given number of steps, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'>set<span class='membertext'>   defines objects to simulation, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interface.html#ac7431baf2435e560c6c28238df1e3d34">execute_set</a><span class='membertext'>   defines objects to simulation, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interface.html#a014ec99ae7e8eac617780e944829c26f">execute_change</a><span class='membertext'>   changes objects properties in  simulation, see provided examples  </span> 
+</div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_parser.html" target="_self">Parser</a></div> <div class='directory' data-member><div class='classcomment'> a cytosim parser </div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>PythonParser</div> <div class='directory' data-member><div class='classcomment'> Python interface to a parser </div><div class='contents'><div class='textblock'>simul</div></div><div class='contents'><div class='textblock'>load</div></div><div class='contents'><div class='textblock'>frame</div></div><div class='contents'><div class='textblock'>next</div></div></div></div> 
+</div></div> 
+</div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_simul.html" target="_self">Simul</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>execute_cut<span class='membertext'>   performes a cut : sim.cut(filament_name, where), see Parser.execute_cut  (C++)  </span> 
+</div></div><div class='contents'><div class='textblock'>execute_delete<span class='membertext'>   deletes objects from simulation, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'>execute_import<span class='membertext'>   imports objects from text file, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'>export<span class='membertext'>   export objects to text file, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'>save<span class='membertext'>   saves current state to trajectory file  </span> 
+</div></div><div class='contents'><div class='textblock'>frame</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul_prop.html">SimulProp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html">Meca</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#abc276d8f0be5c9306d78a96fe3f0bb3c">properties</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space_set.html">SpaceSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space_set.html">SpaceSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_field_set.html">FieldSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_set.html">FiberSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere_set.html">SphereSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead_set.html">BeadSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid_set.html">SolidSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple_set.html">CoupleSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single_set.html">SingleSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer_set.html">OrganizerSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#adee9554e2b226484bc4ad97738921c7e">remove</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a7469c8b960cb87d16c8eba8eb394df66">erase</a></div></div><div class='contents'><div class='textblock'>nuke</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a6fc92e0e88a1173babd33b596d8708b3">time</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#abd0d359bb6ab680bd594236024523982">time_step</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ac6bf1a12c5c98ddec5b65e07fe74cabe">step</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ab0380d45afea9d3e61fafa037813b88c">computeForces</a></div></div><div class='contents'><div class='textblock'>once</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ad6f453d4213e53f481790aeebf7d0218">prepared_solve</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ad73dc00fdaaf2b7c9ca0642761ec3ec8">prepare_meca</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a1825b40ca3bc3a1ba67fdb58fac5015c">prepare</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#af7d39f0eac0af0ed5785935ac72a1e7d">solve</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a2a12e3cfd714da39e7debdf79b26092f">solve_auto</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a8857182b8b3e917ffc87b00951ad8e36">dump</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ab467c1ecbdfff6b842c12d2330adb4cb">saveSystem</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a06546b83defb6adccda00cb02c1f5eb7">evaluate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html">Space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ae239fb10694daf9db05092bcaae4cf04">rename</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a6a241606b95c6fc87e29b421e05a02a8">isCategory</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#afc9d6c25b56d0c550942ef3ddf1f30cb">findProperty</a></div></div><div class='contents'><div class='textblock'>writePropertiesTo</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a154828edf4c8ce031527f3a8c8860f2a">writeProperties</a></div></div><div class='contents'><div class='textblock'>writePropertiesToNoPrune</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Frame</div> <div class='directory' data-member><div class='classcomment'> Python interface to timeframe : behaves as a Python dictionary of Objectsets </div><div class='contents'><div class='textblock'>fibers</div></div><div class='contents'><div class='textblock'>time</div></div><div class='contents'><div class='textblock'>simul</div></div><div class='contents'><div class='textblock'>index</div></div><div class='contents'><div class='textblock'>loaded</div></div><div class='contents'><div class='textblock'>update</div></div><div class='contents'><div class='textblock'>update</div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>__iter__</div></div><div class='contents'><div class='textblock'>keys</div></div><div class='contents'><div class='textblock'>items</div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Group</div> <div class='directory' data-member><div class='classcomment'> Behaves as a list of objects with the same properties </div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'>size</div></div><div class='contents'><div class='textblock'>prop</div></div><div class='contents'><div class='textblock'>__iter__</div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Glossary::val_type</div> <div class='directory' data-member><div class='contents'><div class='textblock'>value_</div></div><div class='contents'><div class='textblock'>defined_</div></div><div class='contents'><div class='textblock'>count_</div></div><div class='contents'><div class='textblock'>__repr__</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Glossary</div> <div class='directory' data-member><div class='contents'><div class='textblock'>terms</div></div><div class='contents'><div class='textblock'>__repr__</div></div><div class='contents'><div class='textblock'>__iter__</div></div><div class='contents'><div class='textblock'>__getitem__</div></div><div class='contents'><div class='textblock'>__setitem__</div></div><div class='contents'><div class='textblock'>keys</div></div><div class='contents'><div class='textblock'>items</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_mecapoint.html" target="_self">Mecapoint</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#aaac3dd297dfd324cef3efe3c2ab0464d">Mecapoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a25a2df970ceb94dcb93cda76db2ae3ea">set</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a315419f26d3c59fa143b49b90a019049">valid</a></div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a91a9b6ce06bef6eb4b1821326126ffc9">pos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a147e754875d4485765ac6f4c95a59336">overlapping</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a50ff3e3d8eec65ec4cfaa1a44f7150ca">near</a></div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_interpolation.html" target="_self">Interpolation</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#ac8bb3912a3ce86b15842e79d0b421204">clear</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#afc73e9a784e97a810e37f01ebde54c7a">set</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a315419f26d3c59fa143b49b90a019049">valid</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html">Mecapoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html">Mecapoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#ae29cb7b310f29ebf4339144694d26522">coef1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a93d94ab33cef0c62fa68b706a112ea70">coef2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a584e9899b630c45e6cc14c63da587b3f">coef</a></div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a91a9b6ce06bef6eb4b1821326126ffc9">pos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#ad2423055f6ad4c002f972ab37b512a5c">pos1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a599e435c9a8f18680ecd9c30ecd4dd95">pos2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a5ab2c008283f29ab4db80d13bcea3a15">diff</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a65be88abb82a600f90626f3c407f189c">len</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a441bfb1b33ab87ccea2a94acbf33b8e9">lenSqr</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a3997c1a68d3914a1e2af1cbf3bee000c">dir</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a231eaf39e8bfd3e5e212261bd087e8ed">inside</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a147e754875d4485765ac6f4c95a59336">overlapping</a></div></div><div class='contents'><div class='textblock'>overlapPoint</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber_site.html" target="_self">FiberSite</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a42c054ef76542ddbe88a0eb28a25e7e1">moveTo</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a1317c8e2441c1fb1c1a39062c2de77d6">relocateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a68d817c102f53a45f7b72fcb9996eae3">relocateP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html" title="a Mecafil to which many Hand may bind">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html" title="a Mecafil to which many Hand may bind">Fiber</a></div></div><div class='contents'><div class='textblock'>update</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac32af0048104e04b946190884239b681">posHand</a></div></div><div class='contents'><div class='textblock'>direction</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#abb4674e86652b8145df4f947634f446a">dirFiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#acd4ae97f5dd9516b38df9cad09f5a54e">abscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a3e47e3dc5ff1791e70284bcede13b1d4">abscissaFromM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a4aa543e7f3e66f8c11bfb8b76f4b0d43">abscissaFromP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a2416da92936f2c84de4d7a6d8292d9b5">abscissaFrom</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#a6cc8f8124cf3efec82ea724346597dde">FiberEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac1658015cd53a01231bb7743ca6520b9">distanceToEnd</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_hand.html" target="_self">Hand</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand_prop.html">HandProp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand_prop.html">HandProp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a36bf4fc11df8e3e6e1e9ff0fcb6a338b">relocate</a></div></div><div class='contents'><div class='textblock'>relocateTo</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a759ad7675832f44a4f9af0a191817f56">moveToEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#aee2127b1e015609a34b956856ea4dc4c">locate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a976377e5e6127dde63e92ae02b074487">attach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#ac295bade8aee589f6718dfa79edc2a34">detach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#ae5949466ed8951a7c706095e9c41a833">attachEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a48640c2f63c1e466a70ca541365ce72c">attachTo</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#ae8f79c56d3405dc8a6cd8d92c45e2bb4">otherPosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a0436cf24ac27b68cd919f2ae79534722">linkStiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a42c054ef76542ddbe88a0eb28a25e7e1">moveTo</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a1317c8e2441c1fb1c1a39062c2de77d6">relocateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a68d817c102f53a45f7b72fcb9996eae3">relocateP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a54cea165fa6f814c13969e970eddcfcc">unattached</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a81139954b9600495023a917578da3d38">attached</a></div></div><div class='contents'><div class='textblock'>update</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac32af0048104e04b946190884239b681">posHand</a></div></div><div class='contents'><div class='textblock'>direction</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#abb4674e86652b8145df4f947634f446a">dirFiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#acd4ae97f5dd9516b38df9cad09f5a54e">abscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a3e47e3dc5ff1791e70284bcede13b1d4">abscissaFromM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a4aa543e7f3e66f8c11bfb8b76f4b0d43">abscissaFromP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a2416da92936f2c84de4d7a6d8292d9b5">abscissaFrom</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#a6cc8f8124cf3efec82ea724346597dde">FiberEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac1658015cd53a01231bb7743ca6520b9">distanceToEnd</a></div></div></div></div> 
 </div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_object_set.html" target="_self">ObjectSet</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#ad96ee952118ebbb111f9a4e5fafe77c7">add</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#adee9554e2b226484bc4ad97738921c7e">remove</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#a472941576c3755215ccd8a0b3a3b6cdf">link</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#ae3fc7a4c891c56d1c75de26d9bc613a1">unlink</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#a7469c8b960cb87d16c8eba8eb394df66">erase</a></div></div><div class='contents'><div class='textblock'>erase_all</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#a7fd4678662f9e4d095477fecf01935df">size</a></div></div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'>first</div></div><div class='contents'><div class='textblock'>last</div></div><div class='contents'><div class='textblock'>findID</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_couple_set.html" target="_self">CoupleSet</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_space_set.html" target="_self">SpaceSet</a></div> </div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_meca.html" target="_self">Meca</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a00f46d823ada4eccd4c9fa1d7174a1d0">nb_points</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a75aa79248b769329ed6b7d62280aa08c">dimension</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ab835a572eb9c814cf49f0fa7d3b9916a">prepare</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a3072d2eb9c72165502a6384e22ed10fe">base</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ab89684eb1f58288c0ffbab32e612e67a">points</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a89232f99d47d6c6b88009b26c277206f">force</a></div></div><div class='contents'><div class='textblock'>addForcePt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a8c36d9df22beccf44aab4f03765275df">addForce</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a725e8b8b1e88c53fa1d428d8d9ddfcaf">addTorque</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ab07faf9b5bccbe926c197e90a3c506c2">addTorqueClamp</a></div></div><div class='contents'><div class='textblock'>addTorqueParrallel</div></div><div class='contents'><div class='textblock'>addTorqueAngle</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a6dc94321c28ab9975d777cddf69c9ec5">addTorquePoliti</a></div></div><div class='contents'><div class='textblock'>addPointClampPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a7179179a9bdcd12bce4af82e42958cb6">addPointClamp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ac00ca74a27cc0064f0611b63b132cdc3">addSphereClamp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a1588131f444ba29d78a29216a414d3b7">addCylinderClampZ</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#aa870055bd24ddc32647b14d965c59c0e">addCylinderClampX</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a6796012aec793f18ca396d96e5715e68">addSidePointClamp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ace08d61a7fecb37e4ab269afb2fea173">addLineClamp</a></div></div><div class='contents'><div class='textblock'>addLineClampPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a2548f1a83e94e5f8e8680ded8cebea37">addPlaneClamp</a></div></div><div class='contents'><div class='textblock'>addPlaneClampPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a28659b9ca1f5a0d59fdd29ea0d3fd9d0">addLink</a></div></div><div class='contents'><div class='textblock'>addLinkPtI</div></div><div class='contents'><div class='textblock'>addLinkIPt</div></div><div class='contents'><div class='textblock'>addLinkPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a52da1f3a6f9e9b3f357aa45a85ca7515">addLongLink</a></div></div><div class='contents'><div class='textblock'>addLongLinkPt</div></div><div class='contents'><div class='textblock'>addLongLinkPtI</div></div><div class='contents'><div class='textblock'>addSideLink2D</div></div><div class='contents'><div class='textblock'>addSideLink2DIPt</div></div><div class='contents'><div class='textblock'>addSideSideLink2D</div></div><div class='contents'><div class='textblock'>addSideSlidingLink2D</div></div><div class='contents'><div class='textblock'>addSideSlidingLink2DIPt</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkS</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkSIPt</div></div><div class='contents'><div class='textblock'>addSideLink3D</div></div><div class='contents'><div class='textblock'>addSideLinkS</div></div><div class='contents'><div class='textblock'>addSideLinkSIpt</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkS</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkSIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a1e56a74a63fd5319a0a46b196b682025">addSideLink</a></div></div><div class='contents'><div class='textblock'>addSideLinkIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ad3811b376eaa3ae617b3b6fd3b72c3d7">addSideSideLink</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a5ca9f81627da4be0a6da4674bb75585e">addSlidingLink</a></div></div><div class='contents'><div class='textblock'>addSlidingLinkIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a6b8794d6b2956b45d8dd87eef2f73a48">addSideSlidingLink</a></div></div><div class='contents'><div class='textblock'>addSideSlidingLinkIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#af7e036bd79e169e22676d34909fa5432">addTriLink</a></div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Vector</div> </div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Vector3</div> </div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>realArray</div> </div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_object_set.html" target="_self">ObjectSet</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#ad96ee952118ebbb111f9a4e5fafe77c7">add</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#adee9554e2b226484bc4ad97738921c7e">remove</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#a472941576c3755215ccd8a0b3a3b6cdf">link</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#ae3fc7a4c891c56d1c75de26d9bc613a1">unlink</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#a7469c8b960cb87d16c8eba8eb394df66">erase</a></div></div><div class='contents'><div class='textblock'>erase_all</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#a7fd4678662f9e4d095477fecf01935df">size</a></div></div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_space_set.html" target="_self">SpaceSet</a></div> </div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber_set.html" target="_self">FiberSet</a></div> </div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_field_set.html" target="_self">FieldSet</a></div> </div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_sphere_set.html" target="_self">SphereSet</a></div> </div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_bead_set.html" target="_self">BeadSet</a></div> </div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_solid_set.html" target="_self">SolidSet</a></div> </div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_organizer_set.html" target="_self">OrganizerSet</a></div> </div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_couple_set.html" target="_self">CoupleSet</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_single_set.html" target="_self">SingleSet</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
 </div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Glossary::val_type</div> <div class='directory' data-member><div class='contents'><div class='textblock'>value_</div></div><div class='contents'><div class='textblock'>defined_</div></div><div class='contents'><div class='textblock'>count_</div></div><div class='contents'><div class='textblock'>__repr__</div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Glossary</div> <div class='directory' data-member><div class='contents'><div class='textblock'>terms</div></div><div class='contents'><div class='textblock'>__repr__</div></div><div class='contents'><div class='textblock'>__iter__</div></div><div class='contents'><div class='textblock'>__getitem__</div></div><div class='contents'><div class='textblock'>__setitem__</div></div><div class='contents'><div class='textblock'>keys</div></div><div class='contents'><div class='textblock'>items</div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Vector</div> </div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Vector3</div> </div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>realArray</div> </div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber_site.html" target="_self">FiberSite</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a42c054ef76542ddbe88a0eb28a25e7e1">moveTo</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a1317c8e2441c1fb1c1a39062c2de77d6">relocateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a68d817c102f53a45f7b72fcb9996eae3">relocateP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html" title="a Mecafil to which many Hand may bind ">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html" title="a Mecafil to which many Hand may bind ">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac5c54df7ed3b930268c8d7752c101725">update</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'>fiber</div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac32af0048104e04b946190884239b681">posHand</a></div></div><div class='contents'><div class='textblock'>direction</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#abb4674e86652b8145df4f947634f446a">dirFiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#acd4ae97f5dd9516b38df9cad09f5a54e">abscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a3e47e3dc5ff1791e70284bcede13b1d4">abscissaFromM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a4aa543e7f3e66f8c11bfb8b76f4b0d43">abscissaFromP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a2416da92936f2c84de4d7a6d8292d9b5">abscissaFrom</a></div></div><div class='contents'><div class='textblock'>nearestEnd</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac1658015cd53a01231bb7743ca6520b9">distanceToEnd</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_hand.html" target="_self">Hand</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>property</div></div><div class='contents'><div class='textblock'>prop</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a36bf4fc11df8e3e6e1e9ff0fcb6a338b">relocate</a></div></div><div class='contents'><div class='textblock'>relocateTo</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a759ad7675832f44a4f9af0a191817f56">moveToEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#aee2127b1e015609a34b956856ea4dc4c">locate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a976377e5e6127dde63e92ae02b074487">attach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#ac295bade8aee589f6718dfa79edc2a34">detach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#ae5949466ed8951a7c706095e9c41a833">attachEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a48640c2f63c1e466a70ca541365ce72c">attachTo</a></div></div><div class='contents'><div class='textblock'>otherHand</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#ae8f79c56d3405dc8a6cd8d92c45e2bb4">otherPosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a0436cf24ac27b68cd919f2ae79534722">linkStiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a42c054ef76542ddbe88a0eb28a25e7e1">moveTo</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a1317c8e2441c1fb1c1a39062c2de77d6">relocateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a68d817c102f53a45f7b72fcb9996eae3">relocateP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a54cea165fa6f814c13969e970eddcfcc">unattached</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a81139954b9600495023a917578da3d38">attached</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac5c54df7ed3b930268c8d7752c101725">update</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'>fiber</div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac32af0048104e04b946190884239b681">posHand</a></div></div><div class='contents'><div class='textblock'>direction</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#abb4674e86652b8145df4f947634f446a">dirFiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#acd4ae97f5dd9516b38df9cad09f5a54e">abscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a3e47e3dc5ff1791e70284bcede13b1d4">abscissaFromM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a4aa543e7f3e66f8c11bfb8b76f4b0d43">abscissaFromP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a2416da92936f2c84de4d7a6d8292d9b5">abscissaFrom</a></div></div><div class='contents'><div class='textblock'>nearestEnd</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac1658015cd53a01231bb7743ca6520b9">distanceToEnd</a></div></div></div></div> 
-</div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Group</div> <div class='directory' data-member><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'>size</div></div><div class='contents'><div class='textblock'>prop</div></div><div class='contents'><div class='textblock'>__iter__</div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>PyCytosim</div> <div class='directory' data-member><div class='contents'><div class='textblock'>toVector<span class='membertext'>  converts numpy array to vector  </span> 
-</div></div><div class='contents'><div class='textblock'>toTorque<span class='membertext'>  converts numpy array to torque  </span> 
-</div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>ObjectList</div> <div class='directory' data-member><div class='contents'><div class='textblock'>__getitem__</div></div><div class='contents'><div class='textblock'>__len__</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>ObjectList</div> <div class='directory' data-member><div class='classcomment'> A list-like structure of Cytosim objects </div><div class='contents'><div class='textblock'>__getitem__</div></div><div class='contents'><div class='textblock'>__len__</div></div></div></div> 
 </div></div> 
 </body></html>
```

#### html2text {}

```diff
@@ -1,166 +1,32 @@
-****** Bound classes and members. ******
+****** PyCytoplay ******
+A python interface for Cytosim
 To use the links, please compile the cytosim documentation. For this run the
 command :
 make doc
+**** List of bound classes and members : ****
 ▼▲PyCytoplay
-simul The ongoing simulation
+play
 setNormalKey sets the callback function for normal keys
 setRuntimeCheck sets the callback function for runtime checks
 setMouseClick sets the callback function for mouse clicks
-▼▲Frame
-fibers
-time
-index
-loaded
-update
-keys
-items
-__getitem__
-start
-play
-str_to_glos
-▼▲Simul
-frame returns current frame, e.g. frame = sim.frame()
-writeObjects writes Objects to default trajectory file
-writeObjects writes Objects to a trajectory file, e.g. writeOjects('file.cmo')
-save saves current state to trajectory file
-add adds objects to simulation, see provided examples
-cut performes a cut : sim.cut(filament_name, where), see Parser.execute_cut
-(C++)
-delete deletes objects from simulation, see provided examples
-import imports objects from text file, see provided examples
-export export objects to text file, see provided examples
-run runs the simulation
-set
-prop
-sMeca
-properties
-spaces
-spaces
-fields
-fibers
-spheres
-beads
-solids
-couples
-singles
-organizers
-remove
-erase
-nuke
-time
-time_step
-step
-computeForces
-run
-change
-change_glos
-once
-prepared_solve
-prepare_meca
-prepare
-solve
-solve_auto
-dump
-saveSystem
-evaluate
-Mecable
-Mecable
-findSpace
-rename
-isCategory
-findProperty
-writePropertiesTo
-writeProperties
-writePropertiesToNoPrune
-▼▲Mecapoint
-set
-mecable
-valid
-position
-pos
-overlapping
-near
-▼▲Interpolation
-clear
-set
-valid
-mecable
-exact1
-exact2
-coef1
-coef2
-coef
-position
-pos
-pos1
-pos2
-diff
-len
-lenSqr
-dir
-inside
-overlapping
-overlapPoint
-▼▲Meca
-nb_points
-dimension
-prepare
-addForcePt
-addForce
-addTorque
-addTorqueClamp
-addTorqueParrallel
-addTorqueAngle
-addTorquePoliti
-addPointClampPt
-addPointClamp
-addSphereClamp
-addCylinderClampZ
-addCylinderClampX
-addSidePointClamp
-addLineClamp
-addLineClampPt
-addPlaneClamp
-addPlaneClampPt
-addLink
-addLinkPtI
-addLinkIPt
-addLinkPt
-addLongLink
-addLongLinkPt
-addLongLinkPtI
-addSideLink2D
-addSideLink2DIPt
-addSideSideLink2D
-addSideSlidingLink2D
-addSideSlidingLink2DIPt
-addSideSlidingLinkS
-addSideSlidingLinkSIPt
-addSideLink3D
-addSideLinkS
-addSideLinkSIpt
-addSideSlidingLinkS
-addSideSlidingLinkSIpt
-addSideLink
-addSideLinkIpt
-addSideSideLink
-addSlidingLink
-addSlidingLinkIpt
-addSideSlidingLink
-addSideSlidingLinkIpt
-addTriLink
+▼▲PyCytosim
+open loads simulation from object files
+start loads simulation from config files
+str_to_glos converts string to Glossary
+str_to_glos converts string to Glossary
+toVector converts numpy array to vector
+toTorque converts numpy array to torque
 ▼▲Object
 reference
 property
 position
-next
+Object
 __next__
-prev
+Object
 id
 writeHeader
 points
 ▼▲Space
 thickness
 resize
 volume
@@ -177,90 +43,74 @@
 signedDistanceToEdge
 bounce
 normalToEdge
 randomPlace
 randomPlaceNearEdge
 randomPlaceOnEdge
 estimateVolume
-▼▲Couple
-position
-active
-stiffness
-force
-cosAngle
-sidePos
-posFree
-attachEnd1
-attachEnd2
-moveToEnd1
-moveToEnd2
-fiber2
-abcissa
-toCouple
-hand1
-hand2
-hand
-state
-__len__
-__getitem__
-▼▲Organizer
-nbOrganized
-position
-positionP
-dragCoefficient
-next
-prev
-▼▲Aster
-solid
-position
-nbFibers
-fiber
-posLink1
-posLink2
-posFiber1
-posFiber2
-getLink1
-getLink2
-getLink
-property
 ▼▲Mecable
 data
 nbPoints
 allocated
-points
+points Returns read-only point coordinates of the mecable
 posPoint
 setPoint
 setPoint
 addPoint
 removePoints
 clearPoints
 shiftPoints
 truncateM
 truncateP
 calculateMomentum
 netForce
 position
 translate
 allInside
+▼▲Sphere
+position
+pos
+Sphere
+resize
+reshape
+orthogonalize
+addSurfacePoint
+nbbSurfacePoints
+dragCoefficient
+Sphere
+Sphere
+Sphere
+▼▲Bead
+position
+Bead
+setPosition
+radius
+radiusSqr
+resize
+volume
+dragCoefficient
+Bead
+Bead
+Bead
 ▼▲Chain
 nbSegments
 lastSegment
 setStraight
 setStraightLength
 placeEnd
 setEquilibrated
 birthTime
 age
-exactEnd
-interpolateEndM
-interpolateEndP
-interpolateCenter
-interpolateEnd
+Mecapoint
+Interpolation
+Interpolation
+Interpolation
+Interpolation
 interpolateFromEnd
-interpolate
+Interpolation
 setEquilibrated
 length1
 trueLength
 betweenMP
 outsideMP
 belowP
 aboveM
@@ -311,75 +161,100 @@
 Fiber
 nbPoints
 cutM
 cutP
 sever
 severNow
 Fiber
-nowSever
 join
 stateM
 stateP
 setStateM
 setStateP
 setDynamicState
 freshAssembly
 nbHands
+addHand
+removeHand
+updateHands
+detachHands
+sortHands
+Hand
 nbHandsInRange
+nbHandsNearEnd
 __next__
 ▼▲ClassicFiber
 freshAssemblyM
 freshAssemblyP
-▼▲Sphere
-position
-pos
-Sphere
-resize
-reshape
-orthogonalize
-addSurfacePoint
-nbbSurfacePoints
-dragCoefficient
-next
-prev
-Sphere
-▼▲Bead
-position
-Bead
-setPosition
-radius
-radiusSqr
-resize
-volume
-dragCoefficient
-next
-prev
-Bead
+▼▲DynamicFiber
+freshAssemblyM
+freshAssemblyP
 ▼▲Solid
 position
 points
 dragCoefficient
 addSphere
 setRadius
 addSphere
 centroid
-next
-prev
+Solid
+Solid
 tag
 property
 nbPoints
 Solid
+▼▲Organizer
+nbOrganized
+position
+positionP
+dragCoefficient
+Organizer
+Organizer
+▼▲Aster
+Solid
+position
+nbFibers
+Fiber
+posLink1
+posLink2
+posFiber1
+posFiber2
+getLink1
+getLink2
+getLink
+property
+▼▲Couple
+position
+active
+stiffness
+force
+cosAngle
+sidePos
+posFree
+attachEnd1
+attachEnd2
+moveToEnd1
+moveToEnd2
+Fiber
+abcissa
+toCouple
+Hand
+Hand
+hand
+state
+__len__
+__getitem__
 ▼▲Single
 toSingle
 state
 __getitem__
 __len__
-hand
+Hand
 Single
-fiber
+Fiber
 abscissa
 posHand
 dirFiber
 attach
 attachEnd
 moveToEnd
 detach
@@ -389,45 +264,57 @@
 setPosition
 randomizePosition
 posFoot
 sidePos
 Mecable
 mobile
 force
-next
-prev
-confineSpace
+Single
+Single
+Space
 ▼▲Property
 name
 change
 read
 change_glos
 read_glos
 complete
 rename
 is_named
 number
 renumber
 clear
 clone
 ▼▲SpaceProp
-▼▲CoupleProp
-hand1
-hand2
-stiffness
-length
-diffusion
-fast_diffusion
-stiff
-Specificity
-confine
+▼▲SolidProp
+drag
+viscosity
+steric
+steric_range
+Confinement
+confine_stiffness
 confine_space
+display
+display_fresh
+▼▲HandProp
+binding_rate
+Hand
+binding_key
+unbinding_rate
+unbinding_force
+bind_also_end
+bind_end_range
+hold_growing_end
+hold_shrinking_end
 activity
-hand1_prop
-hand2_prop
+display
+▼▲MotorProp
+stall_force
+unloaded_speed
+limit_speed
 ▼▲FiberProp
 segmentation
 rigidity
 min_length
 max_length
 total_polymer
 persistent
@@ -446,14 +333,26 @@
 steric_radius
 steric_range
 glue
 glue_single
 activity
 display_fresh
 display
+▼▲ClassicFiberProp
+growing_speed
+growing_off_speed
+growing_force
+shrinking_speed
+catastrophe_rate
+catastrophe_rate_stalled
+▼▲DynamicFiberProp
+growing_speed
+growing_off_speed
+growing_force
+shrinking_speed
 ▼▲SimulProp
 time
 time_step
 viscosity
 kT
 tolerance
 acceptable_prop
@@ -470,147 +369,294 @@
 clear_trajectory
 skip_free_couple
 display_fresh
 display
 read
 read_str
 clone
-▼▲HandProp
-binding_rate
-Hand
-binding_key
-unbinding_rate
-unbinding_force
-bind_also_end
-bind_end_range
-hold_growing_end
-hold_shrinking_end
-activity
-display
-▼▲MotorProp
-stall_force
-unloaded_speed
-limit_speed
-▼▲SolidProp
-drag
-viscosity
-steric
-steric_range
+▼▲CoupleProp
+hand1
+hand2
+stiffness
+length
+diffusion
+fast_diffusion
+stiff
+Specificity
 Confinement
-confine_stiffness
 confine_space
-display
-display_fresh
+activity
+HandProp
+HandProp
 ▼▲SingleProp
 hand
 stiffness
 length
 diffusion
 fast_diffusion
-confine
+Confinement
 confine_space
 activity
-hand_prop
-▼▲ObjectSet
-add
+HandProp
+▼▲Interface
+an interface to cytosim
+add adds objects to simulation, see provided examples
+execute_new adds objects to simulation, see provided examples
+run runs simulation a given number of steps, see provided examples
+execute_run runs simulation a given number of steps, see provided examples
+set defines objects to simulation, see provided examples
+execute_set defines objects to simulation, see provided examples
+execute_change changes objects properties in simulation, see provided examples
+▼▲Parser
+a cytosim parser
+▼▲PythonParser
+Python interface to a parser
+simul
+load
+frame
+next
+▼▲Simul
+execute_cut performes a cut : sim.cut(filament_name, where), see
+Parser.execute_cut (C++)
+execute_delete deletes objects from simulation, see provided examples
+execute_import imports objects from text file, see provided examples
+export export objects to text file, see provided examples
+save saves current state to trajectory file
+frame
+SimulProp
+Meca
+properties
+SpaceSet
+SpaceSet
+FieldSet
+FiberSet
+SphereSet
+BeadSet
+SolidSet
+CoupleSet
+SingleSet
+OrganizerSet
 remove
-link
-unlink
 erase
-erase_all
-size
-__len__
-first
-last
-findID
-Object
-__getitem__
-▼▲CoupleSet
+nuke
+time
+time_step
+step
+computeForces
+once
+prepared_solve
+prepare_meca
+prepare
+solve
+solve_auto
+dump
+saveSystem
+evaluate
+Mecable
+Mecable
+Space
+rename
+isCategory
+findProperty
+writePropertiesTo
+writeProperties
+writePropertiesToNoPrune
+▼▲Frame
+Python interface to timeframe : behaves as a Python dictionary of Objectsets
+fibers
+time
+simul
+index
+loaded
+update
+update
+next
+__iter__
+keys
+items
 __getitem__
-▼▲SpaceSet
-▼▲FiberSet
-▼▲FieldSet
-▼▲SphereSet
-▼▲BeadSet
-▼▲SolidSet
-▼▲OrganizerSet
-▼▲SingleSet
+▼▲Group
+Behaves as a list of objects with the same properties
+__len__
+size
+prop
+__iter__
 __getitem__
 ▼▲Glossary::val_type
 value_
 defined_
 count_
 __repr__
 ▼▲Glossary
 terms
 __repr__
 __iter__
 __getitem__
 __setitem__
 keys
 items
-▼▲Vector
-▼▲Vector3
-▼▲realArray
+▼▲Mecapoint
+Mecapoint
+set
+Mecable
+valid
+position
+pos
+overlapping
+near
+▼▲Interpolation
+clear
+set
+valid
+Mecable
+Mecapoint
+Mecapoint
+coef1
+coef2
+coef
+position
+pos
+pos1
+pos2
+diff
+len
+lenSqr
+dir
+inside
+overlapping
+overlapPoint
 ▼▲FiberSite
 moveTo
 relocateM
 relocateP
 Fiber
 Fiber
 update
 Interpolation
-fiber
+Fiber
 position
 posHand
 direction
 dirFiber
 abscissa
 abscissaFromM
 abscissaFromP
 abscissaFrom
-nearestEnd
+FiberEnd
 distanceToEnd
 ▼▲Hand
-property
-prop
+Hand
+Hand
+HandProp
+HandProp
 relocate
 relocateTo
 moveToEnd
 locate
 attach
 detach
 attachEnd
 attachTo
-otherHand
+Hand
 otherPosition
 linkStiffness
 moveTo
 relocateM
 relocateP
 unattached
 attached
 update
 Interpolation
-fiber
+Fiber
 position
 posHand
 direction
 dirFiber
 abscissa
 abscissaFromM
 abscissaFromP
 abscissaFrom
-nearestEnd
+FiberEnd
 distanceToEnd
-▼▲Group
-__len__
+▼▲Meca
+nb_points
+dimension
+prepare
+base
+points
+force
+addForcePt
+addForce
+addTorque
+addTorqueClamp
+addTorqueParrallel
+addTorqueAngle
+addTorquePoliti
+addPointClampPt
+addPointClamp
+addSphereClamp
+addCylinderClampZ
+addCylinderClampX
+addSidePointClamp
+addLineClamp
+addLineClampPt
+addPlaneClamp
+addPlaneClampPt
+addLink
+addLinkPtI
+addLinkIPt
+addLinkPt
+addLongLink
+addLongLinkPt
+addLongLinkPtI
+addSideLink2D
+addSideLink2DIPt
+addSideSideLink2D
+addSideSlidingLink2D
+addSideSlidingLink2DIPt
+addSideSlidingLinkS
+addSideSlidingLinkSIPt
+addSideLink3D
+addSideLinkS
+addSideLinkSIpt
+addSideSlidingLinkS
+addSideSlidingLinkSIpt
+addSideLink
+addSideLinkIpt
+addSideSideLink
+addSlidingLink
+addSlidingLinkIpt
+addSideSlidingLink
+addSideSlidingLinkIpt
+addTriLink
+▼▲Vector
+▼▲Vector3
+▼▲realArray
+▼▲ObjectSet
+add
+remove
+link
+unlink
+erase
+erase_all
 size
-prop
-__iter__
+__len__
+Object
+Object
+Object
+Object
+__getitem__
+▼▲SpaceSet
+▼▲FiberSet
+▼▲FieldSet
+▼▲SphereSet
+▼▲BeadSet
+▼▲SolidSet
+▼▲OrganizerSet
+▼▲CoupleSet
+__getitem__
+▼▲SingleSet
 __getitem__
-▼▲PyCytosim
-toVector converts numpy array to vector
-toTorque converts numpy array to torque
 ▼▲ObjectList
+A list-like structure of Cytosim objects
 __getitem__
 __len__
```

### Comparing `cytosim-0.0.1/doc/cpython/doc_PyCytosim.html` & `cytosim-0.0.2/doc/cpython/doc_PyCytosim.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,74 @@
 <!DOCTYPE html>         <html xmlns='http://www.w3.org/1999/xhtml' >         <link href='cpython.css' rel='stylesheet' type='text/css'/>         <head > <title>PyCytosim: Bound classes and members</title>         <script type='text/javascript'>         function activate(element) {element.parentElement.parentElement.setAttribute('data-state','1');}         function deactivate(element) {element.parentElement.parentElement.setAttribute('data-state','0');}         </script>         </head >         
-<body><div class ='header' ><h1> Bound classes and members.</h1></div ><div class ='header' > To use the links, please compile the cytosim documentation.          For this run the command : <p/> <span class='membertext'>make doc </span> </div ><div class='contents' data-class data-depth-0 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>PyCytosim</div> <div class='directory' data-member><div class='contents'><div class='textblock'>open<span class='membertext'>  loads simulation from object files  </span> 
+<body><div class ='header' ><h1> PyCytosim</h1> A python interface for Cytosim</div ><div class ='header' > To use the links, please compile the cytosim documentation.              For this run the command : <p/> <span class='membertext'>make doc </span> </div ><div class ='header' ><h3> List of bound classes and members :</h3></div ><div class='contents' data-class data-depth-0 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>PyCytosim</div> <div class='directory' data-member><div class='contents'><div class='textblock'>open<span class='membertext'>  loads simulation from object files  </span> 
 </div></div><div class='contents'><div class='textblock'>start<span class='membertext'>  loads simulation from config files  </span> 
 </div></div><div class='contents'><div class='textblock'>str_to_glos<span class='membertext'>  converts string to Glossary  </span> 
 </div></div><div class='contents'><div class='textblock'>toVector<span class='membertext'>  converts numpy array to vector  </span> 
 </div></div><div class='contents'><div class='textblock'>toTorque<span class='membertext'>  converts numpy array to torque  </span> 
-</div></div></div><div class='directory'><div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Frame</div> <div class='directory' data-member><div class='classcomment'> Python interface to timeframe : behaves as a Python dictionary of Objectsets </div><div class='contents'><div class='textblock'>fibers</div></div><div class='contents'><div class='textblock'>time</div></div><div class='contents'><div class='textblock'>simul</div></div><div class='contents'><div class='textblock'>index</div></div><div class='contents'><div class='textblock'>loaded</div></div><div class='contents'><div class='textblock'>update</div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>__iter__</div></div><div class='contents'><div class='textblock'>keys</div></div><div class='contents'><div class='textblock'>items</div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_simul.html" target="_self">Simul</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>load<span class='membertext'>  loads a frame by index, e.g. frame = sim.load(2)  </span> 
-</div></div><div class='contents'><div class='textblock'>next<span class='membertext'>  loads next frame, e.g. frame = sim.next()  </span> 
-</div></div><div class='contents'><div class='textblock'>loadframe</div></div><div class='contents'><div class='textblock'>frame<span class='membertext'>  returns current frame, e.g. frame = sim.frame()  </span> 
-</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ab6123d07890548356b8e8e16306afebc">writeObjects</a><span class='membertext'>   writes Objects to default trajectory file  </span> 
-</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ab6123d07890548356b8e8e16306afebc">writeObjects</a><span class='membertext'>   writes Objects to a trajectory file, e.g. writeOjects('file.cmo')  </span> 
-</div></div><div class='contents'><div class='textblock'>save<span class='membertext'>   saves current state to trajectory file  </span> 
-</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ad96ee952118ebbb111f9a4e5fafe77c7">add</a><span class='membertext'>   adds objects to simulation, see provided examples  </span> 
-</div></div><div class='contents'><div class='textblock'>cut<span class='membertext'>   performes a cut : sim.cut(filament_name, where), see Parser.execute_cut  (C++)  </span> 
-</div></div><div class='contents'><div class='textblock'>delete<span class='membertext'>   deletes objects from simulation, see provided examples  </span> 
-</div></div><div class='contents'><div class='textblock'>import<span class='membertext'>   imports objects from text file, see provided examples  </span> 
-</div></div><div class='contents'><div class='textblock'>export<span class='membertext'>   export objects to text file, see provided examples  </span> 
-</div></div><div class='contents'><div class='textblock'>run<span class='membertext'>   runs the simulation   </span> 
-</div></div><div class='contents'><div class='textblock'>set</div></div><div class='contents'><div class='textblock'>prop</div></div><div class='contents'><div class='textblock'>sMeca</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#abc276d8f0be5c9306d78a96fe3f0bb3c">properties</a></div></div><div class='contents'><div class='textblock'>spaces</div></div><div class='contents'><div class='textblock'>spaces</div></div><div class='contents'><div class='textblock'>fields</div></div><div class='contents'><div class='textblock'>fibers</div></div><div class='contents'><div class='textblock'>spheres</div></div><div class='contents'><div class='textblock'>beads</div></div><div class='contents'><div class='textblock'>solids</div></div><div class='contents'><div class='textblock'>couples</div></div><div class='contents'><div class='textblock'>singles</div></div><div class='contents'><div class='textblock'>organizers</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#adee9554e2b226484bc4ad97738921c7e">remove</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a7469c8b960cb87d16c8eba8eb394df66">erase</a></div></div><div class='contents'><div class='textblock'>nuke</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a6fc92e0e88a1173babd33b596d8708b3">time</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#abd0d359bb6ab680bd594236024523982">time_step</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ac6bf1a12c5c98ddec5b65e07fe74cabe">step</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ab0380d45afea9d3e61fafa037813b88c">computeForces</a></div></div><div class='contents'><div class='textblock'>run</div></div><div class='contents'><div class='textblock'>change</div></div><div class='contents'><div class='textblock'>change_glos</div></div><div class='contents'><div class='textblock'>once</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ad6f453d4213e53f481790aeebf7d0218">prepared_solve</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ad73dc00fdaaf2b7c9ca0642761ec3ec8">prepare_meca</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a1825b40ca3bc3a1ba67fdb58fac5015c">prepare</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#af7d39f0eac0af0ed5785935ac72a1e7d">solve</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a2a12e3cfd714da39e7debdf79b26092f">solve_auto</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a8857182b8b3e917ffc87b00951ad8e36">dump</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ab467c1ecbdfff6b842c12d2330adb4cb">saveSystem</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a06546b83defb6adccda00cb02c1f5eb7">evaluate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'>findSpace</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ae239fb10694daf9db05092bcaae4cf04">rename</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a6a241606b95c6fc87e29b421e05a02a8">isCategory</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#afc9d6c25b56d0c550942ef3ddf1f30cb">findProperty</a></div></div><div class='contents'><div class='textblock'>writePropertiesTo</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a154828edf4c8ce031527f3a8c8860f2a">writeProperties</a></div></div><div class='contents'><div class='textblock'>writePropertiesToNoPrune</div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_mecapoint.html" target="_self">Mecapoint</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a25a2df970ceb94dcb93cda76db2ae3ea">set</a></div></div><div class='contents'><div class='textblock'>mecable</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a315419f26d3c59fa143b49b90a019049">valid</a></div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a91a9b6ce06bef6eb4b1821326126ffc9">pos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a147e754875d4485765ac6f4c95a59336">overlapping</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a50ff3e3d8eec65ec4cfaa1a44f7150ca">near</a></div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_interpolation.html" target="_self">Interpolation</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#ac8bb3912a3ce86b15842e79d0b421204">clear</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#afc73e9a784e97a810e37f01ebde54c7a">set</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a315419f26d3c59fa143b49b90a019049">valid</a></div></div><div class='contents'><div class='textblock'>mecable</div></div><div class='contents'><div class='textblock'>exact1</div></div><div class='contents'><div class='textblock'>exact2</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#ae29cb7b310f29ebf4339144694d26522">coef1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a93d94ab33cef0c62fa68b706a112ea70">coef2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a584e9899b630c45e6cc14c63da587b3f">coef</a></div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a91a9b6ce06bef6eb4b1821326126ffc9">pos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#ad2423055f6ad4c002f972ab37b512a5c">pos1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a599e435c9a8f18680ecd9c30ecd4dd95">pos2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a5ab2c008283f29ab4db80d13bcea3a15">diff</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a65be88abb82a600f90626f3c407f189c">len</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a441bfb1b33ab87ccea2a94acbf33b8e9">lenSqr</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a3997c1a68d3914a1e2af1cbf3bee000c">dir</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a231eaf39e8bfd3e5e212261bd087e8ed">inside</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a147e754875d4485765ac6f4c95a59336">overlapping</a></div></div><div class='contents'><div class='textblock'>overlapPoint</div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_meca.html" target="_self">Meca</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a00f46d823ada4eccd4c9fa1d7174a1d0">nb_points</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a75aa79248b769329ed6b7d62280aa08c">dimension</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ab835a572eb9c814cf49f0fa7d3b9916a">prepare</a></div></div><div class='contents'><div class='textblock'>addForcePt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a8c36d9df22beccf44aab4f03765275df">addForce</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a725e8b8b1e88c53fa1d428d8d9ddfcaf">addTorque</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ab07faf9b5bccbe926c197e90a3c506c2">addTorqueClamp</a></div></div><div class='contents'><div class='textblock'>addTorqueParrallel</div></div><div class='contents'><div class='textblock'>addTorqueAngle</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a6dc94321c28ab9975d777cddf69c9ec5">addTorquePoliti</a></div></div><div class='contents'><div class='textblock'>addPointClampPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a7179179a9bdcd12bce4af82e42958cb6">addPointClamp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ac00ca74a27cc0064f0611b63b132cdc3">addSphereClamp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a1588131f444ba29d78a29216a414d3b7">addCylinderClampZ</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#aa870055bd24ddc32647b14d965c59c0e">addCylinderClampX</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a6796012aec793f18ca396d96e5715e68">addSidePointClamp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ace08d61a7fecb37e4ab269afb2fea173">addLineClamp</a></div></div><div class='contents'><div class='textblock'>addLineClampPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a2548f1a83e94e5f8e8680ded8cebea37">addPlaneClamp</a></div></div><div class='contents'><div class='textblock'>addPlaneClampPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a28659b9ca1f5a0d59fdd29ea0d3fd9d0">addLink</a></div></div><div class='contents'><div class='textblock'>addLinkPtI</div></div><div class='contents'><div class='textblock'>addLinkIPt</div></div><div class='contents'><div class='textblock'>addLinkPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a52da1f3a6f9e9b3f357aa45a85ca7515">addLongLink</a></div></div><div class='contents'><div class='textblock'>addLongLinkPt</div></div><div class='contents'><div class='textblock'>addLongLinkPtI</div></div><div class='contents'><div class='textblock'>addSideLink2D</div></div><div class='contents'><div class='textblock'>addSideLink2DIPt</div></div><div class='contents'><div class='textblock'>addSideSideLink2D</div></div><div class='contents'><div class='textblock'>addSideSlidingLink2D</div></div><div class='contents'><div class='textblock'>addSideSlidingLink2DIPt</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkS</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkSIPt</div></div><div class='contents'><div class='textblock'>addSideLink3D</div></div><div class='contents'><div class='textblock'>addSideLinkS</div></div><div class='contents'><div class='textblock'>addSideLinkSIpt</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkS</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkSIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a1e56a74a63fd5319a0a46b196b682025">addSideLink</a></div></div><div class='contents'><div class='textblock'>addSideLinkIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ad3811b376eaa3ae617b3b6fd3b72c3d7">addSideSideLink</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a5ca9f81627da4be0a6da4674bb75585e">addSlidingLink</a></div></div><div class='contents'><div class='textblock'>addSlidingLinkIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a6b8794d6b2956b45d8dd87eef2f73a48">addSideSlidingLink</a></div></div><div class='contents'><div class='textblock'>addSideSlidingLinkIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#af7e036bd79e169e22676d34909fa5432">addTriLink</a></div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_object.html" target="_self">Object</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html#ac4676f3cc02884e13816f02297d87682">reference</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html#ace9ef785c9d0ec30f908396c5571652d">property</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_movable.html#ad624fda53a1713016ff082c46da88669">position</a></div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>__next__</div></div><div class='contents'><div class='textblock'>prev</div></div><div class='contents'><div class='textblock'>id</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html#aab41ee90c8599ea042c4843df912b00b">writeHeader</a></div></div><div class='contents'><div class='textblock'>points</div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_space.html" target="_self">Space</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a698861183e4cd233c0adc3eee628d911">thickness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ac30219811cfcb86e195477c165c18a5f">resize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a6fa3310f56de73e730b8050b5b8544c4">volume</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a6a7f066111371b55d909ce38791d841a">boundaries</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a8c90e38ceddbd5fbaf015263209642bc">inside</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ac5f310d4dcbd5aeea8104ab662a7bbb1">project</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a852c5e4cdf4f880461c23ee7e0c5f3c5">allInside</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a022f4e7547e8869994cbe798639344bd">allOutside</a></div></div><div class='contents'><div class='textblock'>toSpace</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a650154e5931ac28f374161f81313bd7d">max_extension</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a95caf802881b0cd12c56c58a59d4bb4d">projectDeflated</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a1d56de008507a862a0738c29b10c8b36">distanceToEdgeSqr</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#adced8eb2fc67ffdbf466a30f8f455f8c">distanceToEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a603c748be20553699fc2d52aa3e63de7">signedDistanceToEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a9cc94f7136747635b9d61a3114d0c5ba">bounce</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a20348398cd84dbf188287d06ccbcd289">normalToEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ab638802c149c21b952acdc28f56ef39a">randomPlace</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a5381a9546b0a8f860c83fbef32da2231">randomPlaceNearEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ac6f71047665796f6fdfccd301c580fe8">randomPlaceOnEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a684d9ae11971c7a91195af780e718f2c">estimateVolume</a></div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_couple.html" target="_self">Couple</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#af835342337022ce2d50420f766eda7f5">active</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#ac15de46b6db835d101cb026d3b00f050">stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a35671221583000fc2ddd7aa89257b5a0">force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a3699aaed45aca84acd573c5fc7193a14">cosAngle</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a922b3f3998f2e945d69c9a95a25066e5">sidePos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a0ecbd1ecf9a3d7b30719044ab87cef88">posFree</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#ac5d01183f3dea554080c7562141243ef">attachEnd1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#afa8e22aac660c824d21a17c59a3e2ac6">attachEnd2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#acbc2233baf1ebb2423709c2b84676342">moveToEnd1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#aacc63cae7f406dc44ed01e7528ca6e3c">moveToEnd2</a></div></div><div class='contents'><div class='textblock'>fiber2</div></div><div class='contents'><div class='textblock'>abcissa</div></div><div class='contents'><div class='textblock'>toCouple</div></div><div class='contents'><div class='textblock'>hand1</div></div><div class='contents'><div class='textblock'>hand2</div></div><div class='contents'><div class='textblock'>hand</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a6de3ae1bc365515f6970323b44d3d983">state</a></div></div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_organizer.html" target="_self">Organizer</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#aa68d1ed0efa1960c9665848614c80b74">nbOrganized</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#a592193b879b25cd2ecb649bfe57b964f">positionP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>prev</div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_aster.html" target="_self">Aster</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>solid</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a137b14b7e404c5036ad5479b4a91d74e">nbFibers</a></div></div><div class='contents'><div class='textblock'>fiber</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a0505c1142c7ecbf7568aa3507ad103c2">posLink1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a2f8269c5f717aafaa9532ec778fdd4c3">posLink2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a6c2153bd31bbb6e00f0e672a342620d0">posFiber1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a9ded7ba76407f8e77f9aa3e707462058">posFiber2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a33e055da50bc2afc1cae9284054c10a3">getLink1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a8e5151dadbb4978eac986046130a7636">getLink2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a4a4b50f68883ff81796082eeadf9df4e">getLink</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a5d9895c039bde2ea31c8ba069a31bc74">property</a></div></div></div></div> 
+</div></div></div><div class='directory'><div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_object.html" target="_self">Object</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html#ac4676f3cc02884e13816f02297d87682">reference</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html#ace9ef785c9d0ec30f908396c5571652d">property</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_movable.html#ad624fda53a1713016ff082c46da88669">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'>__next__</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'>id</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html#aab41ee90c8599ea042c4843df912b00b">writeHeader</a></div></div><div class='contents'><div class='textblock'>points</div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_space.html" target="_self">Space</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a698861183e4cd233c0adc3eee628d911">thickness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ac30219811cfcb86e195477c165c18a5f">resize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a6fa3310f56de73e730b8050b5b8544c4">volume</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a6a7f066111371b55d909ce38791d841a">boundaries</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a8c90e38ceddbd5fbaf015263209642bc">inside</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ac5f310d4dcbd5aeea8104ab662a7bbb1">project</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a852c5e4cdf4f880461c23ee7e0c5f3c5">allInside</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a022f4e7547e8869994cbe798639344bd">allOutside</a></div></div><div class='contents'><div class='textblock'>toSpace</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a650154e5931ac28f374161f81313bd7d">max_extension</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a95caf802881b0cd12c56c58a59d4bb4d">projectDeflated</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a1d56de008507a862a0738c29b10c8b36">distanceToEdgeSqr</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#adced8eb2fc67ffdbf466a30f8f455f8c">distanceToEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a603c748be20553699fc2d52aa3e63de7">signedDistanceToEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a9cc94f7136747635b9d61a3114d0c5ba">bounce</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a20348398cd84dbf188287d06ccbcd289">normalToEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ab638802c149c21b952acdc28f56ef39a">randomPlace</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a5381a9546b0a8f860c83fbef32da2231">randomPlaceNearEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#ac6f71047665796f6fdfccd301c580fe8">randomPlaceOnEdge</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html#a684d9ae11971c7a91195af780e718f2c">estimateVolume</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_mecable.html" target="_self">Mecable</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#aa073fce85239bcb6a3104b9e72055161">data</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a289e74a02e184e27a71ce1adf3883bf1">nbPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a8bc3e142a14a07815b29e230cefacd3e">allocated</a></div></div><div class='contents'><div class='textblock'>points<span class='membertext'>   Returns read-only point coordinates of the mecable  </span> 
+</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a030f8164696551d58123cf373655d9ce">posPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#abb809f1939f978a9abdbc3e49a1e87d0">setPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#abb809f1939f978a9abdbc3e49a1e87d0">setPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a720e68bfecf70eabf91384fc2af4aaff">addPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#adbd23bceacee22d13226a020a9ccb23b">removePoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a54d93424ae45b23df413c5cfd5820b79">clearPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a9c0978f6f953be030e66be7629d18a8a">shiftPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a07b95fbcb40cb557ad282af05689c6da">truncateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#ae6d6812c7ec1a56e590ba5559736b1c2">truncateP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a26827539688fc54c4bf1474a8b3f3f1c">calculateMomentum</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a1b27ae44a7c7b1f924d54695bc1a7641">netForce</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a1dba38e58fd08f3f70d4a521cd904577">translate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a124d881969afe4378d1d36c1a9fc6916">allInside</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_sphere.html" target="_self">Sphere</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'>pos</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a66f8268c3614689bddb7e9508ec50abb">Sphere</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a9e4bd1a51f41a59e059adc7fccb4cc4c">resize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a63b5230e86ff1b3d58cfe70429fe4956">reshape</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a0301a31b9d311381e37a1c41406248d3">orthogonalize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#aa61b3e120c4324b62f1fe42a3ce95ed1">addSurfacePoint</a></div></div><div class='contents'><div class='textblock'>nbbSurfacePoints</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html">Sphere</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html">Sphere</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html">Sphere</a></div></div></div></div> 
+<div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_bead.html" target="_self">Bead</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a205d3670324a950673bb464cd507827e">Bead</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a224123905bed58e68a4b277eb4b6c289">setPosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#afc6e66e226b54ad058211db1a9ea3acc">radius</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a0756681ed4cffa41dcbec5825eea0765">radiusSqr</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a5199eca3fe77f7dffd1e6b44605f15fe">resize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a7345ca77d5e0a1371c7373786d650ef2">volume</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html">Bead</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html">Bead</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html">Bead</a></div></div></div></div> 
+<div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_chain.html" target="_self">Chain</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ade97cb1630fbb84f8937e872632fff1c">nbSegments</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a0055db6e3444cfdd7783663d206a87c0">lastSegment</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a62249a99fd0a422d8766e4bf63c3d554">setStraight</a></div></div><div class='contents'><div class='textblock'>setStraightLength</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a853f22938de7a0d33597587da11da092">placeEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a4edb26c5275b8ee111af7b4177efe826">setEquilibrated</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a1930a9adf88969fc4b7b15cf9fe7108a">birthTime</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a19411a4cc4b0381e06007ccb8eb27e9b">age</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html">Mecapoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'>interpolateFromEnd</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a4edb26c5275b8ee111af7b4177efe826">setEquilibrated</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a9ec30ab32a36e4c0e678cc53311599d7">length1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a794290003b8229b0e5427e2472ed97e2">trueLength</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a149e71e7a76b780e37b8bbc59ef72d7f">betweenMP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a8138c56ab72b0cb3cc342fd2604847ae">outsideMP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ac46cb99bde6530da54ab9046be9310a8">belowP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad1377568e189c84519e58e5506dafd4b">aboveM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#a6cc8f8124cf3efec82ea724346597dde">FiberEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad30f5d0f543f0fe757e82d931046cab9">clampedIndexM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad0d77e016a5c4f7683ddea47b8692d9f">setOrigin</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a2395c6041facb79aadf409637ec59172">abscissaM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a5113c828524ceb520533d984abc54a74">abscissaC</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#afc94966444dc56109d43a0e9a9a84aea">abscissaP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a043e4b9942be8d992caf7c0c33df7989">abscissaPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ab53240451117802d75bdf4ce8bfff5ff">abscissaEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a1663517f441656976661844bff51a75e">abscissaFrom</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aef30f06e27bda8676062c876aab50288">someAbscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a9556ce5e695f7af85f0ea3706b6121f6">posM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a62249a99fd0a422d8766e4bf63c3d554">setStraight</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a70ed4893ded81126c279dbf86bde029c">posFrom</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a3d95856990f79cd338e73f8d0a1a9db4">posMiddle</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a127a26975c292b6a951ef378728e53ff">posEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#acb5765074baf5abb14cb2e0967b351a3">posEndP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#adbab2f3e6fb1662a6f4a4ee9fc36ab95">posEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aeee12a9eb9f3b9862cc9a615dd7a2287">netForceEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad642529b9e17cf07bc3cd6744f675dee">netForceEndP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aa6c712d0987324e96e2bf7d9fca31afc">projectedForceEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ab68a15d872cf86dec8bc883407bb00f5">projectedForceEndP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aa6c712d0987324e96e2bf7d9fca31afc">projectedForceEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a6408a7cbd00fadc0db10ef528e9bb5a9">avgDirection</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a17598f35c35f991a317071b9edb718d1">segmentation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a43e24153dfb4b2be1437dc48bab618ed">flipChainPolarity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#af45fb76a686d5bf3ed398bc70966f1c5">curvature</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aab47087140d4066eec10338eb203a9d8">bendingEnergy0</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#af6e0e170e1cac14151a76628ccaa49aa">planarIntersect</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#acd775993f2e15a2905bb6cbf5bbf5d07">growM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aadc04c51e3184c13ca74473262672f34">addSegmentM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a2c9dc9b22febc0b83cf2bc691c7f5b3f">cutM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a92308cf0ac8c65cb2c3bb1dffc5c5e19">growP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a5ddc78be861218a4d511580c0561afa7">addSegmentP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a33f46f9d38054801961d95a7032971fa">cutP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a66c42f788e7d0f2641e79c28daaa0cf2">grow</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a6f74d2a21a83c31983142e2e73734523">adjustLength</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a999f75df61342bbc6b4d6fa5c1cb2cfe">truncateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aa7ccc502af2dfadf28c36bdf67f6860f">truncateP</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-4 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_mecafil.html" target="_self">Mecafil</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecafil.html#af86966d8cc47fe44b15bd6e55dc6bcae">tension</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecafil.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecafil.html#aec775e777f2888a830cf2e7270930a55">leftoverMobility</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-5 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber.html" target="_self">Fiber</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>points</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a289e74a02e184e27a71ce1adf3883bf1">nbPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a8855988fb953c48f770d7da5e7d8fcbe">cutM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#afcbe3a24c88dfd97abd739e3b468dc43">cutP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a1485fd899f48f7395627a6c78ecc1071">sever</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a6cea692446c106c98789f2f20853918b">severNow</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a4387b72a2db3733dfec1b10b9c20af42">join</a></div></div><div class='contents'><div class='textblock'>stateM</div></div><div class='contents'><div class='textblock'>stateP</div></div><div class='contents'><div class='textblock'>setStateM</div></div><div class='contents'><div class='textblock'>setStateP</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a3a495090170d36b3da6c7cd95f53ae86">setDynamicState</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a0702bb0654fa4fceaf3cbae366b832a8">freshAssembly</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a7dfc07cca7d08be5a84bc1e3259902b3">nbHands</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#aa7383b1a4473b50c50edec33bfcda435">addHand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#adeb3c522f7304851881551707dcc4706">removeHand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a1b9467c7cc981f10085c131d0d2bbad7">updateHands</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a33d23ba81d903c935822468735f908d8">detachHands</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#ad17baf33afac710aa199eaead637d6c6">sortHands</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#ac8a4e8f2c4d61aaf91171d20b101dcc2">nbHandsInRange</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a0874dfd020a5bd0a6e49f2991b0d1a7b">nbHandsNearEnd</a></div></div><div class='contents'><div class='textblock'>__next__</div></div></div><div class='directory'><div class='contents' data-class data-depth-6 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_classic_fiber.html" target="_self">ClassicFiber</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_classic_fiber.html#a6a0c10d4ee0fb78722c7fee2d4806b9c">freshAssemblyM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_classic_fiber.html#ae0f68d2181b1a6d3fd9edda105cb1412">freshAssemblyP</a></div></div></div></div> 
+<div class='contents' data-class data-depth-6 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_dynamic_fiber.html" target="_self">DynamicFiber</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_dynamic_fiber.html#a6a0c10d4ee0fb78722c7fee2d4806b9c">freshAssemblyM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_dynamic_fiber.html#ae0f68d2181b1a6d3fd9edda105cb1412">freshAssemblyP</a></div></div></div></div> 
 </div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_mecable.html" target="_self">Mecable</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#aa073fce85239bcb6a3104b9e72055161">data</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a289e74a02e184e27a71ce1adf3883bf1">nbPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a8bc3e142a14a07815b29e230cefacd3e">allocated</a></div></div><div class='contents'><div class='textblock'>points</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a030f8164696551d58123cf373655d9ce">posPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#abb809f1939f978a9abdbc3e49a1e87d0">setPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#abb809f1939f978a9abdbc3e49a1e87d0">setPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a720e68bfecf70eabf91384fc2af4aaff">addPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#adbd23bceacee22d13226a020a9ccb23b">removePoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a54d93424ae45b23df413c5cfd5820b79">clearPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a9c0978f6f953be030e66be7629d18a8a">shiftPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a07b95fbcb40cb557ad282af05689c6da">truncateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#ae6d6812c7ec1a56e590ba5559736b1c2">truncateP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a26827539688fc54c4bf1474a8b3f3f1c">calculateMomentum</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a1b27ae44a7c7b1f924d54695bc1a7641">netForce</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a1dba38e58fd08f3f70d4a521cd904577">translate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a124d881969afe4378d1d36c1a9fc6916">allInside</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_chain.html" target="_self">Chain</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ade97cb1630fbb84f8937e872632fff1c">nbSegments</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a0055db6e3444cfdd7783663d206a87c0">lastSegment</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a62249a99fd0a422d8766e4bf63c3d554">setStraight</a></div></div><div class='contents'><div class='textblock'>setStraightLength</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a853f22938de7a0d33597587da11da092">placeEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a4edb26c5275b8ee111af7b4177efe826">setEquilibrated</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a1930a9adf88969fc4b7b15cf9fe7108a">birthTime</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a19411a4cc4b0381e06007ccb8eb27e9b">age</a></div></div><div class='contents'><div class='textblock'>exactEnd</div></div><div class='contents'><div class='textblock'>interpolateEndM</div></div><div class='contents'><div class='textblock'>interpolateEndP</div></div><div class='contents'><div class='textblock'>interpolateCenter</div></div><div class='contents'><div class='textblock'>interpolateEnd</div></div><div class='contents'><div class='textblock'>interpolateFromEnd</div></div><div class='contents'><div class='textblock'>interpolate</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a4edb26c5275b8ee111af7b4177efe826">setEquilibrated</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a9ec30ab32a36e4c0e678cc53311599d7">length1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a794290003b8229b0e5427e2472ed97e2">trueLength</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a149e71e7a76b780e37b8bbc59ef72d7f">betweenMP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a8138c56ab72b0cb3cc342fd2604847ae">outsideMP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ac46cb99bde6530da54ab9046be9310a8">belowP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad1377568e189c84519e58e5506dafd4b">aboveM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#a6cc8f8124cf3efec82ea724346597dde">FiberEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad30f5d0f543f0fe757e82d931046cab9">clampedIndexM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad0d77e016a5c4f7683ddea47b8692d9f">setOrigin</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a2395c6041facb79aadf409637ec59172">abscissaM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a5113c828524ceb520533d984abc54a74">abscissaC</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#afc94966444dc56109d43a0e9a9a84aea">abscissaP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a043e4b9942be8d992caf7c0c33df7989">abscissaPoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ab53240451117802d75bdf4ce8bfff5ff">abscissaEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a1663517f441656976661844bff51a75e">abscissaFrom</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aef30f06e27bda8676062c876aab50288">someAbscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a9556ce5e695f7af85f0ea3706b6121f6">posM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a62249a99fd0a422d8766e4bf63c3d554">setStraight</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a70ed4893ded81126c279dbf86bde029c">posFrom</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a3d95856990f79cd338e73f8d0a1a9db4">posMiddle</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a127a26975c292b6a951ef378728e53ff">posEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#acb5765074baf5abb14cb2e0967b351a3">posEndP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#adbab2f3e6fb1662a6f4a4ee9fc36ab95">posEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aeee12a9eb9f3b9862cc9a615dd7a2287">netForceEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ad642529b9e17cf07bc3cd6744f675dee">netForceEndP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aa6c712d0987324e96e2bf7d9fca31afc">projectedForceEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#ab68a15d872cf86dec8bc883407bb00f5">projectedForceEndP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aa6c712d0987324e96e2bf7d9fca31afc">projectedForceEndM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a6408a7cbd00fadc0db10ef528e9bb5a9">avgDirection</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a17598f35c35f991a317071b9edb718d1">segmentation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a43e24153dfb4b2be1437dc48bab618ed">flipChainPolarity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#af45fb76a686d5bf3ed398bc70966f1c5">curvature</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aab47087140d4066eec10338eb203a9d8">bendingEnergy0</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#af6e0e170e1cac14151a76628ccaa49aa">planarIntersect</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#acd775993f2e15a2905bb6cbf5bbf5d07">growM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aadc04c51e3184c13ca74473262672f34">addSegmentM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a2c9dc9b22febc0b83cf2bc691c7f5b3f">cutM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a92308cf0ac8c65cb2c3bb1dffc5c5e19">growP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a5ddc78be861218a4d511580c0561afa7">addSegmentP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a33f46f9d38054801961d95a7032971fa">cutP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a66c42f788e7d0f2641e79c28daaa0cf2">grow</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a6f74d2a21a83c31983142e2e73734523">adjustLength</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#a999f75df61342bbc6b4d6fa5c1cb2cfe">truncateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_chain.html#aa7ccc502af2dfadf28c36bdf67f6860f">truncateP</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_mecafil.html" target="_self">Mecafil</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecafil.html#af86966d8cc47fe44b15bd6e55dc6bcae">tension</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecafil.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecafil.html#aec775e777f2888a830cf2e7270930a55">leftoverMobility</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-4 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber.html" target="_self">Fiber</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>points</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a289e74a02e184e27a71ce1adf3883bf1">nbPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a8855988fb953c48f770d7da5e7d8fcbe">cutM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#afcbe3a24c88dfd97abd739e3b468dc43">cutP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a1485fd899f48f7395627a6c78ecc1071">sever</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a6cea692446c106c98789f2f20853918b">severNow</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'>nowSever</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a4387b72a2db3733dfec1b10b9c20af42">join</a></div></div><div class='contents'><div class='textblock'>stateM</div></div><div class='contents'><div class='textblock'>stateP</div></div><div class='contents'><div class='textblock'>setStateM</div></div><div class='contents'><div class='textblock'>setStateP</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a3a495090170d36b3da6c7cd95f53ae86">setDynamicState</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a0702bb0654fa4fceaf3cbae366b832a8">freshAssembly</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#a7dfc07cca7d08be5a84bc1e3259902b3">nbHands</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html#ac8a4e8f2c4d61aaf91171d20b101dcc2">nbHandsInRange</a></div></div><div class='contents'><div class='textblock'>__next__</div></div></div><div class='directory'><div class='contents' data-class data-depth-5 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_classic_fiber.html" target="_self">ClassicFiber</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_classic_fiber.html#a6a0c10d4ee0fb78722c7fee2d4806b9c">freshAssemblyM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_classic_fiber.html#ae0f68d2181b1a6d3fd9edda105cb1412">freshAssemblyP</a></div></div></div></div> 
 </div></div> 
 </div></div> 
 </div></div> 
-<div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_sphere.html" target="_self">Sphere</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'>pos</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a66f8268c3614689bddb7e9508ec50abb">Sphere</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a9e4bd1a51f41a59e059adc7fccb4cc4c">resize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a63b5230e86ff1b3d58cfe70429fe4956">reshape</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#a0301a31b9d311381e37a1c41406248d3">orthogonalize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#aa61b3e120c4324b62f1fe42a3ce95ed1">addSurfacePoint</a></div></div><div class='contents'><div class='textblock'>nbbSurfacePoints</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>prev</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere.html">Sphere</a></div></div></div></div> 
-<div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_bead.html" target="_self">Bead</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a205d3670324a950673bb464cd507827e">Bead</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a224123905bed58e68a4b277eb4b6c289">setPosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#afc6e66e226b54ad058211db1a9ea3acc">radius</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a0756681ed4cffa41dcbec5825eea0765">radiusSqr</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a5199eca3fe77f7dffd1e6b44605f15fe">resize</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#a7345ca77d5e0a1371c7373786d650ef2">volume</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>prev</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead.html">Bead</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_solid.html" target="_self">Solid</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'>points</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#ab4d58012b7bc78b8c0a1efa482acaf84">addSphere</a></div></div><div class='contents'><div class='textblock'>setRadius</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#ab4d58012b7bc78b8c0a1efa482acaf84">addSphere</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#af6a9acdfad3dd47796dd317cca2d5560">centroid</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html">Solid</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html">Solid</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#ae6fb4d0b832ee89eb207dd98da5865ed">tag</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#a5d9895c039bde2ea31c8ba069a31bc74">property</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a289e74a02e184e27a71ce1adf3883bf1">nbPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html">Solid</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_organizer.html" target="_self">Organizer</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#aa68d1ed0efa1960c9665848614c80b74">nbOrganized</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#a592193b879b25cd2ecb649bfe57b964f">positionP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html">Organizer</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer.html">Organizer</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_aster.html" target="_self">Aster</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html">Solid</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a137b14b7e404c5036ad5479b4a91d74e">nbFibers</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a0505c1142c7ecbf7568aa3507ad103c2">posLink1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a2f8269c5f717aafaa9532ec778fdd4c3">posLink2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a6c2153bd31bbb6e00f0e672a342620d0">posFiber1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a9ded7ba76407f8e77f9aa3e707462058">posFiber2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a33e055da50bc2afc1cae9284054c10a3">getLink1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a8e5151dadbb4978eac986046130a7636">getLink2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a4a4b50f68883ff81796082eeadf9df4e">getLink</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_aster.html#a5d9895c039bde2ea31c8ba069a31bc74">property</a></div></div></div></div> 
 </div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_solid.html" target="_self">Solid</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'>points</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#aad555a67f7f0756d5984f323ed3071e9">dragCoefficient</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#ab4d58012b7bc78b8c0a1efa482acaf84">addSphere</a></div></div><div class='contents'><div class='textblock'>setRadius</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#ab4d58012b7bc78b8c0a1efa482acaf84">addSphere</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#af6a9acdfad3dd47796dd317cca2d5560">centroid</a></div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>prev</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#ae6fb4d0b832ee89eb207dd98da5865ed">tag</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html#a5d9895c039bde2ea31c8ba069a31bc74">property</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html#a289e74a02e184e27a71ce1adf3883bf1">nbPoints</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid.html">Solid</a></div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_single.html" target="_self">Single</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>toSingle</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a6de3ae1bc365515f6970323b44d3d983">state</a></div></div><div class='contents'><div class='textblock'>__getitem__</div></div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'>hand</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html" title="A point-like object containing one Hand. ">Single</a></div></div><div class='contents'><div class='textblock'>fiber</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#acd4ae97f5dd9516b38df9cad09f5a54e">abscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac32af0048104e04b946190884239b681">posHand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#abb4674e86652b8145df4f947634f446a">dirFiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a0cc627377931cdb970f6c9da2fe2975c">attach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ae5949466ed8951a7c706095e9c41a833">attachEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac61bdddfe1f2437d88bf92041af4df36">moveToEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac295bade8aee589f6718dfa79edc2a34">detach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a55bb5045e5a6cce3e45c6a04821f99e8">mobile</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#af9c87a998410f54900993d5add04e78f">translate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#abbcf4a043ead606e034072c253caf18f">setPosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a243a4ae5e156567d0241de936986b336">randomizePosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac9b487785e64912d738b5d886944839c">posFoot</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a922b3f3998f2e945d69c9a95a25066e5">sidePos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a55bb5045e5a6cce3e45c6a04821f99e8">mobile</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a318425477b2d6704ff1de4d37c9a391a">force</a></div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>prev</div></div><div class='contents'><div class='textblock'>confineSpace</div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_couple.html" target="_self">Couple</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#af835342337022ce2d50420f766eda7f5">active</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#ac15de46b6db835d101cb026d3b00f050">stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a35671221583000fc2ddd7aa89257b5a0">force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a3699aaed45aca84acd573c5fc7193a14">cosAngle</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a922b3f3998f2e945d69c9a95a25066e5">sidePos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a0ecbd1ecf9a3d7b30719044ab87cef88">posFree</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#ac5d01183f3dea554080c7562141243ef">attachEnd1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#afa8e22aac660c824d21a17c59a3e2ac6">attachEnd2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#acbc2233baf1ebb2423709c2b84676342">moveToEnd1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#aacc63cae7f406dc44ed01e7528ca6e3c">moveToEnd2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'>abcissa</div></div><div class='contents'><div class='textblock'>toCouple</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'>hand</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple.html#a6de3ae1bc365515f6970323b44d3d983">state</a></div></div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_single.html" target="_self">Single</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>toSingle</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a6de3ae1bc365515f6970323b44d3d983">state</a></div></div><div class='contents'><div class='textblock'>__getitem__</div></div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html" title="A point-like object containing one Hand.">Single</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#acd4ae97f5dd9516b38df9cad09f5a54e">abscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac32af0048104e04b946190884239b681">posHand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#abb4674e86652b8145df4f947634f446a">dirFiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a0cc627377931cdb970f6c9da2fe2975c">attach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ae5949466ed8951a7c706095e9c41a833">attachEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac61bdddfe1f2437d88bf92041af4df36">moveToEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac295bade8aee589f6718dfa79edc2a34">detach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a50b4483a6174b489792e4a46f73f7c99">position</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a55bb5045e5a6cce3e45c6a04821f99e8">mobile</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#af9c87a998410f54900993d5add04e78f">translate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#abbcf4a043ead606e034072c253caf18f">setPosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a243a4ae5e156567d0241de936986b336">randomizePosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#ac9b487785e64912d738b5d886944839c">posFoot</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a922b3f3998f2e945d69c9a95a25066e5">sidePos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a55bb5045e5a6cce3e45c6a04821f99e8">mobile</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html#a318425477b2d6704ff1de4d37c9a391a">force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html">Single</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single.html">Single</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html">Space</a></div></div></div></div> 
 </div></div> 
 <div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Property</div> <div class='directory' data-member><div class='contents'><div class='textblock'>name</div></div><div class='contents'><div class='textblock'>change</div></div><div class='contents'><div class='textblock'>read</div></div><div class='contents'><div class='textblock'>change_glos</div></div><div class='contents'><div class='textblock'>read_glos</div></div><div class='contents'><div class='textblock'>complete</div></div><div class='contents'><div class='textblock'>rename</div></div><div class='contents'><div class='textblock'>is_named</div></div><div class='contents'><div class='textblock'>number</div></div><div class='contents'><div class='textblock'>renumber</div></div><div class='contents'><div class='textblock'>clear</div></div><div class='contents'><div class='textblock'>clone</div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_space_prop.html" target="_self">SpaceProp</a></div> </div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_couple_prop.html" target="_self">CoupleProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga103de20cbd1e6b0cda8f5a2a17df575d">hand1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gaea9b1d8250cb587f3e6e90e627422adf">hand2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga575ccdd0e4c30d7c82343fe313533356">stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga780020b647987365a5a7280ba79e059c">length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gab69c79ec9456e615f41c6af1850da983">diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gad988df56af78ff8a949fa43aa279aa34">fast_diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga0c8c31e73b2b393e04b4c033ca8a8869">stiff</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple_prop.html#a2b6018f958ecd9fd2574082f0b6dfd07">Specificity</a></div></div><div class='contents'><div class='textblock'>confine</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'>hand1_prop</div></div><div class='contents'><div class='textblock'>hand2_prop</div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber_prop.html" target="_self">FiberProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gae9cb302aee80c6b6d700bb819563da67">segmentation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaa49d9ce314729739966f40e3babfaf0e">rigidity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga1cfafcb5a4f95cab8630811ed1234a84">min_length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga6a22df6cc0302e9b9c67c82ed5a1fd3e">max_length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga6ef4a1d00af970a715d4420c21471ed4">total_polymer</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaea39f2c5cb5ec83de4d1f81b1a74f0cc">persistent</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga816f13f493c4ad26b49e715afa17632c">viscosity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga1d7c289df62d5cc769290fa173b69e44">drag_radius</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga21239f90a6fb2c0842046344691b33a6">drag_length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga962259ef18b27c2066e2625b07f6d314">drag_model</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga4cec2aa9e2f2ed945c3a40b892de5f70">drag_gap</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaba923853d8f165530e05df9a8ff3079a">binding_key</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga94b59d3ee243a20d8fb40a2bac66eeba">lattice</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gab25be625ee763a05b85e0a24ad8315a1">lattice_unit</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#ae05f8c1156eea5e8bd6a9fbf181b4134">Confinement</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaef88f3cd69d3efb00fa13ff79b602495">confine_stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga09ca671af9b8e13dc8212fd14b76ea2d">steric</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gad7a5acf48cf8480363e97fa9ee005bbe">steric_radius</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga79a65a48123b5fdbee499f5bd550e870">steric_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gacea5b6e35581d9d8dbf04647b05a6ee3">glue</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gacc919e6961fd8baa1c313552037d8f4e">glue_single</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_prop.html#a207131365a7c95b985fbb3ac841a1472">display_fresh</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_solid_prop.html" target="_self">SolidProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga1c9993dba2c798ab1e7216211d54210f">drag</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga816f13f493c4ad26b49e715afa17632c">viscosity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga09ca671af9b8e13dc8212fd14b76ea2d">steric</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga79a65a48123b5fdbee499f5bd550e870">steric_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#ae05f8c1156eea5e8bd6a9fbf181b4134">Confinement</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#gaef88f3cd69d3efb00fa13ff79b602495">confine_stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid_prop.html#a207131365a7c95b985fbb3ac841a1472">display_fresh</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_hand_prop.html" target="_self">HandProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#gaf0ab51c3ebb07f8a0204ec2fa84ba84c">binding_rate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html" title="Simulates the stochastic binding/unbinding of a FiberSite.">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#gaba923853d8f165530e05df9a8ff3079a">binding_key</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga6f7c89db19de7c19666fe34515cc091c">unbinding_rate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#gada5f3500c0056c48d814c7445eb16b66">unbinding_force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga11a9781744f0e9667f43f3ae78fe31b9">bind_also_end</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga727176c11f75111ffb56dd11b279a3ed">bind_end_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga780e1719024062c6f4cc4dfc4d0d09a9">hold_growing_end</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga0f816ba324afa2c1d3517efa23b9d662">hold_shrinking_end</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_motor_prop.html" target="_self">MotorProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___motor_par.html#ga22d593fb145923c1d6b08bec61ef807e">stall_force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___motor_par.html#ga46b808e3b9bb7a8f717979fcc735dd41">unloaded_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___motor_par.html#ga094300e05909448478c30cb6511a7429">limit_speed</a></div></div></div></div> 
+</div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber_prop.html" target="_self">FiberProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gae9cb302aee80c6b6d700bb819563da67">segmentation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaa49d9ce314729739966f40e3babfaf0e">rigidity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga1cfafcb5a4f95cab8630811ed1234a84">min_length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga6a22df6cc0302e9b9c67c82ed5a1fd3e">max_length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga6ef4a1d00af970a715d4420c21471ed4">total_polymer</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaea39f2c5cb5ec83de4d1f81b1a74f0cc">persistent</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga816f13f493c4ad26b49e715afa17632c">viscosity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga1d7c289df62d5cc769290fa173b69e44">drag_radius</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga21239f90a6fb2c0842046344691b33a6">drag_length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga962259ef18b27c2066e2625b07f6d314">drag_model</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga4cec2aa9e2f2ed945c3a40b892de5f70">drag_gap</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaba923853d8f165530e05df9a8ff3079a">binding_key</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga94b59d3ee243a20d8fb40a2bac66eeba">lattice</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gab25be625ee763a05b85e0a24ad8315a1">lattice_unit</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#ae05f8c1156eea5e8bd6a9fbf181b4134">Confinement</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gaef88f3cd69d3efb00fa13ff79b602495">confine_stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga09ca671af9b8e13dc8212fd14b76ea2d">steric</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gad7a5acf48cf8480363e97fa9ee005bbe">steric_radius</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga79a65a48123b5fdbee499f5bd550e870">steric_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gacea5b6e35581d9d8dbf04647b05a6ee3">glue</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#gacc919e6961fd8baa1c313552037d8f4e">glue_single</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_prop.html#a207131365a7c95b985fbb3ac841a1472">display_fresh</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___fiber_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_classic_fiber_prop.html" target="_self">ClassicFiberProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___classic_fiber_par.html#gae1f11153d0c02e5450e7bd0da081fc05">growing_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___classic_fiber_par.html#ga631bd8742a85fff733d22f410b18621b">growing_off_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___classic_fiber_par.html#ga9c8e5e8ca707b087e73f4848f27b6f11">growing_force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___classic_fiber_par.html#gacf8a42c4e207c11bfeef6dc5254151f1">shrinking_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___classic_fiber_par.html#ga1d29395da00ae2c6e4f8d414436ad2bb">catastrophe_rate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___classic_fiber_par.html#ga3e72a845d13f65d7e3b12109d8b09798">catastrophe_rate_stalled</a></div></div></div></div> 
+<div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_dynamic_fiber_prop.html" target="_self">DynamicFiberProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___dynamic_fiber_par.html#gae1f11153d0c02e5450e7bd0da081fc05">growing_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___dynamic_fiber_par.html#ga631bd8742a85fff733d22f410b18621b">growing_off_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___dynamic_fiber_par.html#ga9c8e5e8ca707b087e73f4848f27b6f11">growing_force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___dynamic_fiber_par.html#gacf8a42c4e207c11bfeef6dc5254151f1">shrinking_speed</a></div></div></div></div> 
+</div></div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_simul_prop.html" target="_self">SimulProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#gaf1d4f29e7f0a2828126f4ea8335d7f17">time</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga5873848f9003055866bb6647374432ce">time_step</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga816f13f493c4ad26b49e715afa17632c">viscosity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#gafe75f1fd9847dfd7826e89caeeeab9dc">kT</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga73b7915f7d7ae31cd8261f404d3a8c74">tolerance</a></div></div><div class='contents'><div class='textblock'>acceptable_prop</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga1d0898295332ea1b58d9d7a2aac435e1">precondition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga09ca671af9b8e13dc8212fd14b76ea2d">steric</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#gac3589077a5077b9460edecd1959960b3">steric_stiffness_push</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#gaada6e15bcd71e84fd762ee7a40795a88">steric_stiffness_pull</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga4bd197701fe216bc11ef724536ac227a">steric_max_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga0f3dfd0699cf7d2ac133531edda2e48e">binding_grid_step</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga0b2caeb4b6f130be43e5a2f0267dd453">verbose</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga2352c06fef330221367dcff7715a071f">config_file</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#gaaf200c91c2dace9dcf3d8cca17a51227">property_file</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga9cb0feeca84b787e8d246988bc280a63">trajectory_file</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga37d87007b0e0ee8974b6875dea667066">clear_trajectory</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#gab49370f739a445ca87df438259a86964">skip_free_couple</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul_prop.html#a207131365a7c95b985fbb3ac841a1472">display_fresh</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___simul_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul_prop.html#a79302f6d5ed23c67123fb65933b76990">read</a></div></div><div class='contents'><div class='textblock'>read_str</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul_prop.html#a33900dad01a57f50ce4e494b5758321f">clone</a></div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_hand_prop.html" target="_self">HandProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#gaf0ab51c3ebb07f8a0204ec2fa84ba84c">binding_rate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html" title="Simulates the stochastic binding/unbinding of a FiberSite. ">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#gaba923853d8f165530e05df9a8ff3079a">binding_key</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga6f7c89db19de7c19666fe34515cc091c">unbinding_rate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#gada5f3500c0056c48d814c7445eb16b66">unbinding_force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga11a9781744f0e9667f43f3ae78fe31b9">bind_also_end</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga727176c11f75111ffb56dd11b279a3ed">bind_end_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga780e1719024062c6f4cc4dfc4d0d09a9">hold_growing_end</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga0f816ba324afa2c1d3517efa23b9d662">hold_shrinking_end</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___hand_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_motor_prop.html" target="_self">MotorProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___motor_par.html#ga22d593fb145923c1d6b08bec61ef807e">stall_force</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___motor_par.html#ga46b808e3b9bb7a8f717979fcc735dd41">unloaded_speed</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___motor_par.html#ga094300e05909448478c30cb6511a7429">limit_speed</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_couple_prop.html" target="_self">CoupleProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga103de20cbd1e6b0cda8f5a2a17df575d">hand1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gaea9b1d8250cb587f3e6e90e627422adf">hand2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga575ccdd0e4c30d7c82343fe313533356">stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga780020b647987365a5a7280ba79e059c">length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gab69c79ec9456e615f41c6af1850da983">diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gad988df56af78ff8a949fa43aa279aa34">fast_diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga0c8c31e73b2b393e04b4c033ca8a8869">stiff</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple_prop.html#a2b6018f958ecd9fd2574082f0b6dfd07">Specificity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#ae05f8c1156eea5e8bd6a9fbf181b4134">Confinement</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___couple_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand_prop.html">HandProp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand_prop.html">HandProp</a></div></div></div></div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_single_prop.html" target="_self">SingleProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gace8fe07b79d67d0ce0564806f65e4b90">hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#ga575ccdd0e4c30d7c82343fe313533356">stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#ga780020b647987365a5a7280ba79e059c">length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gab69c79ec9456e615f41c6af1850da983">diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gad988df56af78ff8a949fa43aa279aa34">fast_diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#ae05f8c1156eea5e8bd6a9fbf181b4134">Confinement</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand_prop.html">HandProp</a></div></div></div></div> 
 </div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_solid_prop.html" target="_self">SolidProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga1c9993dba2c798ab1e7216211d54210f">drag</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga816f13f493c4ad26b49e715afa17632c">viscosity</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga09ca671af9b8e13dc8212fd14b76ea2d">steric</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga79a65a48123b5fdbee499f5bd550e870">steric_range</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#ae05f8c1156eea5e8bd6a9fbf181b4134">Confinement</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#gaef88f3cd69d3efb00fa13ff79b602495">confine_stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___solid_par.html#ga752a5eb77ec7c529726fc6c1c88f0331">display</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid_prop.html#a207131365a7c95b985fbb3ac841a1472">display_fresh</a></div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_single_prop.html" target="_self">SingleProp</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gace8fe07b79d67d0ce0564806f65e4b90">hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#ga575ccdd0e4c30d7c82343fe313533356">stiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#ga780020b647987365a5a7280ba79e059c">length</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gab69c79ec9456e615f41c6af1850da983">diffusion</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gad988df56af78ff8a949fa43aa279aa34">fast_diffusion</a></div></div><div class='contents'><div class='textblock'>confine</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#gad31e61ceb9c0970c3c15ca60d38761b6">confine_space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/group___single_par.html#ga1d2167339bd750012f7e30ca8061e23e">activity</a></div></div><div class='contents'><div class='textblock'>hand_prop</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_interface.html" target="_self">Interface</a></div> <div class='directory' data-member><div class='classcomment'> an interface to cytosim </div><div class='contents'><div class='textblock'>add<span class='membertext'>   adds objects to simulation, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interface.html#a1009a882e99e8e20c9acb7f7f8689584">execute_new</a><span class='membertext'>   adds objects to simulation, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'>run<span class='membertext'>   runs simulation a given number of steps, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interface.html#ae6c1ea315d29b9483ed924622c379b90">execute_run</a><span class='membertext'>   runs simulation a given number of steps, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'>set<span class='membertext'>   defines objects to simulation, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interface.html#ac7431baf2435e560c6c28238df1e3d34">execute_set</a><span class='membertext'>   defines objects to simulation, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interface.html#a014ec99ae7e8eac617780e944829c26f">execute_change</a><span class='membertext'>   changes objects properties in  simulation, see provided examples  </span> 
+</div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_parser.html" target="_self">Parser</a></div> <div class='directory' data-member><div class='classcomment'> a cytosim parser </div></div><div class='directory'><div class='contents' data-class data-depth-3 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>PythonParser</div> <div class='directory' data-member><div class='classcomment'> Python interface to a parser </div><div class='contents'><div class='textblock'>simul</div></div><div class='contents'><div class='textblock'>load</div></div><div class='contents'><div class='textblock'>frame</div></div><div class='contents'><div class='textblock'>next</div></div></div></div> 
+</div></div> 
+</div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_simul.html" target="_self">Simul</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>execute_cut<span class='membertext'>   performes a cut : sim.cut(filament_name, where), see Parser.execute_cut  (C++)  </span> 
+</div></div><div class='contents'><div class='textblock'>execute_delete<span class='membertext'>   deletes objects from simulation, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'>execute_import<span class='membertext'>   imports objects from text file, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'>export<span class='membertext'>   export objects to text file, see provided examples  </span> 
+</div></div><div class='contents'><div class='textblock'>save<span class='membertext'>   saves current state to trajectory file  </span> 
+</div></div><div class='contents'><div class='textblock'>frame</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul_prop.html">SimulProp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html">Meca</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#abc276d8f0be5c9306d78a96fe3f0bb3c">properties</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space_set.html">SpaceSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space_set.html">SpaceSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_field_set.html">FieldSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_set.html">FiberSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_sphere_set.html">SphereSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_bead_set.html">BeadSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_solid_set.html">SolidSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_couple_set.html">CoupleSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_single_set.html">SingleSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_organizer_set.html">OrganizerSet</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#adee9554e2b226484bc4ad97738921c7e">remove</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a7469c8b960cb87d16c8eba8eb394df66">erase</a></div></div><div class='contents'><div class='textblock'>nuke</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a6fc92e0e88a1173babd33b596d8708b3">time</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#abd0d359bb6ab680bd594236024523982">time_step</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ac6bf1a12c5c98ddec5b65e07fe74cabe">step</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ab0380d45afea9d3e61fafa037813b88c">computeForces</a></div></div><div class='contents'><div class='textblock'>once</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ad6f453d4213e53f481790aeebf7d0218">prepared_solve</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ad73dc00fdaaf2b7c9ca0642761ec3ec8">prepare_meca</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a1825b40ca3bc3a1ba67fdb58fac5015c">prepare</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#af7d39f0eac0af0ed5785935ac72a1e7d">solve</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a2a12e3cfd714da39e7debdf79b26092f">solve_auto</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a8857182b8b3e917ffc87b00951ad8e36">dump</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ab467c1ecbdfff6b842c12d2330adb4cb">saveSystem</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a06546b83defb6adccda00cb02c1f5eb7">evaluate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_space.html">Space</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#ae239fb10694daf9db05092bcaae4cf04">rename</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a6a241606b95c6fc87e29b421e05a02a8">isCategory</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#afc9d6c25b56d0c550942ef3ddf1f30cb">findProperty</a></div></div><div class='contents'><div class='textblock'>writePropertiesTo</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_simul.html#a154828edf4c8ce031527f3a8c8860f2a">writeProperties</a></div></div><div class='contents'><div class='textblock'>writePropertiesToNoPrune</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Frame</div> <div class='directory' data-member><div class='classcomment'> Python interface to timeframe : behaves as a Python dictionary of Objectsets </div><div class='contents'><div class='textblock'>fibers</div></div><div class='contents'><div class='textblock'>time</div></div><div class='contents'><div class='textblock'>simul</div></div><div class='contents'><div class='textblock'>index</div></div><div class='contents'><div class='textblock'>loaded</div></div><div class='contents'><div class='textblock'>update</div></div><div class='contents'><div class='textblock'>update</div></div><div class='contents'><div class='textblock'>next</div></div><div class='contents'><div class='textblock'>__iter__</div></div><div class='contents'><div class='textblock'>keys</div></div><div class='contents'><div class='textblock'>items</div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Group</div> <div class='directory' data-member><div class='classcomment'> Behaves as a list of objects with the same properties </div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'>size</div></div><div class='contents'><div class='textblock'>prop</div></div><div class='contents'><div class='textblock'>__iter__</div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Glossary::val_type</div> <div class='directory' data-member><div class='contents'><div class='textblock'>value_</div></div><div class='contents'><div class='textblock'>defined_</div></div><div class='contents'><div class='textblock'>count_</div></div><div class='contents'><div class='textblock'>__repr__</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Glossary</div> <div class='directory' data-member><div class='contents'><div class='textblock'>terms</div></div><div class='contents'><div class='textblock'>__repr__</div></div><div class='contents'><div class='textblock'>__iter__</div></div><div class='contents'><div class='textblock'>__getitem__</div></div><div class='contents'><div class='textblock'>__setitem__</div></div><div class='contents'><div class='textblock'>keys</div></div><div class='contents'><div class='textblock'>items</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_mecapoint.html" target="_self">Mecapoint</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#aaac3dd297dfd324cef3efe3c2ab0464d">Mecapoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a25a2df970ceb94dcb93cda76db2ae3ea">set</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a315419f26d3c59fa143b49b90a019049">valid</a></div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a91a9b6ce06bef6eb4b1821326126ffc9">pos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a147e754875d4485765ac6f4c95a59336">overlapping</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html#a50ff3e3d8eec65ec4cfaa1a44f7150ca">near</a></div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_interpolation.html" target="_self">Interpolation</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#ac8bb3912a3ce86b15842e79d0b421204">clear</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#afc73e9a784e97a810e37f01ebde54c7a">set</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a315419f26d3c59fa143b49b90a019049">valid</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecable.html">Mecable</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html">Mecapoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_mecapoint.html">Mecapoint</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#ae29cb7b310f29ebf4339144694d26522">coef1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a93d94ab33cef0c62fa68b706a112ea70">coef2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a584e9899b630c45e6cc14c63da587b3f">coef</a></div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a91a9b6ce06bef6eb4b1821326126ffc9">pos</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#ad2423055f6ad4c002f972ab37b512a5c">pos1</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a599e435c9a8f18680ecd9c30ecd4dd95">pos2</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a5ab2c008283f29ab4db80d13bcea3a15">diff</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a65be88abb82a600f90626f3c407f189c">len</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a441bfb1b33ab87ccea2a94acbf33b8e9">lenSqr</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a3997c1a68d3914a1e2af1cbf3bee000c">dir</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a231eaf39e8bfd3e5e212261bd087e8ed">inside</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html#a147e754875d4485765ac6f4c95a59336">overlapping</a></div></div><div class='contents'><div class='textblock'>overlapPoint</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber_site.html" target="_self">FiberSite</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a42c054ef76542ddbe88a0eb28a25e7e1">moveTo</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a1317c8e2441c1fb1c1a39062c2de77d6">relocateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a68d817c102f53a45f7b72fcb9996eae3">relocateP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html" title="a Mecafil to which many Hand may bind">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html" title="a Mecafil to which many Hand may bind">Fiber</a></div></div><div class='contents'><div class='textblock'>update</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac32af0048104e04b946190884239b681">posHand</a></div></div><div class='contents'><div class='textblock'>direction</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#abb4674e86652b8145df4f947634f446a">dirFiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#acd4ae97f5dd9516b38df9cad09f5a54e">abscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a3e47e3dc5ff1791e70284bcede13b1d4">abscissaFromM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a4aa543e7f3e66f8c11bfb8b76f4b0d43">abscissaFromP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a2416da92936f2c84de4d7a6d8292d9b5">abscissaFrom</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#a6cc8f8124cf3efec82ea724346597dde">FiberEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac1658015cd53a01231bb7743ca6520b9">distanceToEnd</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_hand.html" target="_self">Hand</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand_prop.html">HandProp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand_prop.html">HandProp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a36bf4fc11df8e3e6e1e9ff0fcb6a338b">relocate</a></div></div><div class='contents'><div class='textblock'>relocateTo</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a759ad7675832f44a4f9af0a191817f56">moveToEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#aee2127b1e015609a34b956856ea4dc4c">locate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a976377e5e6127dde63e92ae02b074487">attach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#ac295bade8aee589f6718dfa79edc2a34">detach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#ae5949466ed8951a7c706095e9c41a833">attachEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a48640c2f63c1e466a70ca541365ce72c">attachTo</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html">Hand</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#ae8f79c56d3405dc8a6cd8d92c45e2bb4">otherPosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a0436cf24ac27b68cd919f2ae79534722">linkStiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a42c054ef76542ddbe88a0eb28a25e7e1">moveTo</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a1317c8e2441c1fb1c1a39062c2de77d6">relocateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a68d817c102f53a45f7b72fcb9996eae3">relocateP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a54cea165fa6f814c13969e970eddcfcc">unattached</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a81139954b9600495023a917578da3d38">attached</a></div></div><div class='contents'><div class='textblock'>update</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html">Fiber</a></div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac32af0048104e04b946190884239b681">posHand</a></div></div><div class='contents'><div class='textblock'>direction</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#abb4674e86652b8145df4f947634f446a">dirFiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#acd4ae97f5dd9516b38df9cad09f5a54e">abscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a3e47e3dc5ff1791e70284bcede13b1d4">abscissaFromM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a4aa543e7f3e66f8c11bfb8b76f4b0d43">abscissaFromP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a2416da92936f2c84de4d7a6d8292d9b5">abscissaFrom</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/common_8h.html#a6cc8f8124cf3efec82ea724346597dde">FiberEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac1658015cd53a01231bb7743ca6520b9">distanceToEnd</a></div></div></div></div> 
 </div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_object_set.html" target="_self">ObjectSet</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#ad96ee952118ebbb111f9a4e5fafe77c7">add</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#adee9554e2b226484bc4ad97738921c7e">remove</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#a472941576c3755215ccd8a0b3a3b6cdf">link</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#ae3fc7a4c891c56d1c75de26d9bc613a1">unlink</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#a7469c8b960cb87d16c8eba8eb394df66">erase</a></div></div><div class='contents'><div class='textblock'>erase_all</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#a7fd4678662f9e4d095477fecf01935df">size</a></div></div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'>first</div></div><div class='contents'><div class='textblock'>last</div></div><div class='contents'><div class='textblock'>findID</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_couple_set.html" target="_self">CoupleSet</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
-<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_space_set.html" target="_self">SpaceSet</a></div> </div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_meca.html" target="_self">Meca</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a00f46d823ada4eccd4c9fa1d7174a1d0">nb_points</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a75aa79248b769329ed6b7d62280aa08c">dimension</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ab835a572eb9c814cf49f0fa7d3b9916a">prepare</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a3072d2eb9c72165502a6384e22ed10fe">base</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ab89684eb1f58288c0ffbab32e612e67a">points</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a89232f99d47d6c6b88009b26c277206f">force</a></div></div><div class='contents'><div class='textblock'>addForcePt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a8c36d9df22beccf44aab4f03765275df">addForce</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a725e8b8b1e88c53fa1d428d8d9ddfcaf">addTorque</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ab07faf9b5bccbe926c197e90a3c506c2">addTorqueClamp</a></div></div><div class='contents'><div class='textblock'>addTorqueParrallel</div></div><div class='contents'><div class='textblock'>addTorqueAngle</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a6dc94321c28ab9975d777cddf69c9ec5">addTorquePoliti</a></div></div><div class='contents'><div class='textblock'>addPointClampPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a7179179a9bdcd12bce4af82e42958cb6">addPointClamp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ac00ca74a27cc0064f0611b63b132cdc3">addSphereClamp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a1588131f444ba29d78a29216a414d3b7">addCylinderClampZ</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#aa870055bd24ddc32647b14d965c59c0e">addCylinderClampX</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a6796012aec793f18ca396d96e5715e68">addSidePointClamp</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ace08d61a7fecb37e4ab269afb2fea173">addLineClamp</a></div></div><div class='contents'><div class='textblock'>addLineClampPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a2548f1a83e94e5f8e8680ded8cebea37">addPlaneClamp</a></div></div><div class='contents'><div class='textblock'>addPlaneClampPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a28659b9ca1f5a0d59fdd29ea0d3fd9d0">addLink</a></div></div><div class='contents'><div class='textblock'>addLinkPtI</div></div><div class='contents'><div class='textblock'>addLinkIPt</div></div><div class='contents'><div class='textblock'>addLinkPt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a52da1f3a6f9e9b3f357aa45a85ca7515">addLongLink</a></div></div><div class='contents'><div class='textblock'>addLongLinkPt</div></div><div class='contents'><div class='textblock'>addLongLinkPtI</div></div><div class='contents'><div class='textblock'>addSideLink2D</div></div><div class='contents'><div class='textblock'>addSideLink2DIPt</div></div><div class='contents'><div class='textblock'>addSideSideLink2D</div></div><div class='contents'><div class='textblock'>addSideSlidingLink2D</div></div><div class='contents'><div class='textblock'>addSideSlidingLink2DIPt</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkS</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkSIPt</div></div><div class='contents'><div class='textblock'>addSideLink3D</div></div><div class='contents'><div class='textblock'>addSideLinkS</div></div><div class='contents'><div class='textblock'>addSideLinkSIpt</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkS</div></div><div class='contents'><div class='textblock'>addSideSlidingLinkSIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a1e56a74a63fd5319a0a46b196b682025">addSideLink</a></div></div><div class='contents'><div class='textblock'>addSideLinkIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#ad3811b376eaa3ae617b3b6fd3b72c3d7">addSideSideLink</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a5ca9f81627da4be0a6da4674bb75585e">addSlidingLink</a></div></div><div class='contents'><div class='textblock'>addSlidingLinkIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#a6b8794d6b2956b45d8dd87eef2f73a48">addSideSlidingLink</a></div></div><div class='contents'><div class='textblock'>addSideSlidingLinkIpt</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_meca.html#af7e036bd79e169e22676d34909fa5432">addTriLink</a></div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Vector</div> </div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Vector3</div> </div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>realArray</div> </div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_object_set.html" target="_self">ObjectSet</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#ad96ee952118ebbb111f9a4e5fafe77c7">add</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#adee9554e2b226484bc4ad97738921c7e">remove</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#a472941576c3755215ccd8a0b3a3b6cdf">link</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#ae3fc7a4c891c56d1c75de26d9bc613a1">unlink</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#a7469c8b960cb87d16c8eba8eb394df66">erase</a></div></div><div class='contents'><div class='textblock'>erase_all</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object_set.html#a7fd4678662f9e4d095477fecf01935df">size</a></div></div><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_object.html">Object</a></div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_space_set.html" target="_self">SpaceSet</a></div> </div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber_set.html" target="_self">FiberSet</a></div> </div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_field_set.html" target="_self">FieldSet</a></div> </div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_sphere_set.html" target="_self">SphereSet</a></div> </div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_bead_set.html" target="_self">BeadSet</a></div> </div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_solid_set.html" target="_self">SolidSet</a></div> </div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_organizer_set.html" target="_self">OrganizerSet</a></div> </div> 
+<div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_couple_set.html" target="_self">CoupleSet</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
 <div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_single_set.html" target="_self">SingleSet</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
 </div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Glossary::val_type</div> <div class='directory' data-member><div class='contents'><div class='textblock'>value_</div></div><div class='contents'><div class='textblock'>defined_</div></div><div class='contents'><div class='textblock'>count_</div></div><div class='contents'><div class='textblock'>__repr__</div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Glossary</div> <div class='directory' data-member><div class='contents'><div class='textblock'>terms</div></div><div class='contents'><div class='textblock'>__repr__</div></div><div class='contents'><div class='textblock'>__iter__</div></div><div class='contents'><div class='textblock'>__getitem__</div></div><div class='contents'><div class='textblock'>__setitem__</div></div><div class='contents'><div class='textblock'>keys</div></div><div class='contents'><div class='textblock'>items</div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Vector</div> </div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Vector3</div> </div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>realArray</div> </div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_fiber_site.html" target="_self">FiberSite</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a42c054ef76542ddbe88a0eb28a25e7e1">moveTo</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a1317c8e2441c1fb1c1a39062c2de77d6">relocateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a68d817c102f53a45f7b72fcb9996eae3">relocateP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html" title="a Mecafil to which many Hand may bind ">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber.html" title="a Mecafil to which many Hand may bind ">Fiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac5c54df7ed3b930268c8d7752c101725">update</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'>fiber</div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac32af0048104e04b946190884239b681">posHand</a></div></div><div class='contents'><div class='textblock'>direction</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#abb4674e86652b8145df4f947634f446a">dirFiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#acd4ae97f5dd9516b38df9cad09f5a54e">abscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a3e47e3dc5ff1791e70284bcede13b1d4">abscissaFromM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a4aa543e7f3e66f8c11bfb8b76f4b0d43">abscissaFromP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a2416da92936f2c84de4d7a6d8292d9b5">abscissaFrom</a></div></div><div class='contents'><div class='textblock'>nearestEnd</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac1658015cd53a01231bb7743ca6520b9">distanceToEnd</a></div></div></div><div class='directory'><div class='contents' data-class data-depth-2 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span><a class="el" href="../code/doxygen/class_hand.html" target="_self">Hand</a></div> <div class='directory' data-member><div class='contents'><div class='textblock'>property</div></div><div class='contents'><div class='textblock'>prop</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a36bf4fc11df8e3e6e1e9ff0fcb6a338b">relocate</a></div></div><div class='contents'><div class='textblock'>relocateTo</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a759ad7675832f44a4f9af0a191817f56">moveToEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#aee2127b1e015609a34b956856ea4dc4c">locate</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a976377e5e6127dde63e92ae02b074487">attach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#ac295bade8aee589f6718dfa79edc2a34">detach</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#ae5949466ed8951a7c706095e9c41a833">attachEnd</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a48640c2f63c1e466a70ca541365ce72c">attachTo</a></div></div><div class='contents'><div class='textblock'>otherHand</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#ae8f79c56d3405dc8a6cd8d92c45e2bb4">otherPosition</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_hand.html#a0436cf24ac27b68cd919f2ae79534722">linkStiffness</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a42c054ef76542ddbe88a0eb28a25e7e1">moveTo</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a1317c8e2441c1fb1c1a39062c2de77d6">relocateM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a68d817c102f53a45f7b72fcb9996eae3">relocateP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a54cea165fa6f814c13969e970eddcfcc">unattached</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a81139954b9600495023a917578da3d38">attached</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac5c54df7ed3b930268c8d7752c101725">update</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_interpolation.html">Interpolation</a></div></div><div class='contents'><div class='textblock'>fiber</div></div><div class='contents'><div class='textblock'>position</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac32af0048104e04b946190884239b681">posHand</a></div></div><div class='contents'><div class='textblock'>direction</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#abb4674e86652b8145df4f947634f446a">dirFiber</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#acd4ae97f5dd9516b38df9cad09f5a54e">abscissa</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a3e47e3dc5ff1791e70284bcede13b1d4">abscissaFromM</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a4aa543e7f3e66f8c11bfb8b76f4b0d43">abscissaFromP</a></div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#a2416da92936f2c84de4d7a6d8292d9b5">abscissaFrom</a></div></div><div class='contents'><div class='textblock'>nearestEnd</div></div><div class='contents'><div class='textblock'><a class="el" href="../code/doxygen/class_fiber_site.html#ac1658015cd53a01231bb7743ca6520b9">distanceToEnd</a></div></div></div></div> 
-</div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>Group</div> <div class='directory' data-member><div class='contents'><div class='textblock'>__len__</div></div><div class='contents'><div class='textblock'>size</div></div><div class='contents'><div class='textblock'>prop</div></div><div class='contents'><div class='textblock'>__iter__</div></div><div class='contents'><div class='textblock'>__getitem__</div></div></div></div> 
-<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>ObjectList</div> <div class='directory' data-member><div class='contents'><div class='textblock'>__getitem__</div></div><div class='contents'><div class='textblock'>__len__</div></div></div></div> 
+<div class='contents' data-class data-depth-1 data-state='0'><div class='title'> <span data-arr onclick='activate(this)'><a>&#9660;</a></span><span data-arr onclick='deactivate(this)'><a>&#9650;</a></span>ObjectList</div> <div class='directory' data-member><div class='classcomment'> A list-like structure of Cytosim objects </div><div class='contents'><div class='textblock'>__getitem__</div></div><div class='contents'><div class='textblock'>__len__</div></div></div></div> 
 </div></div> 
 </body></html>
```

#### html2text {}

```diff
@@ -1,171 +1,26 @@
-****** Bound classes and members. ******
+****** PyCytosim ******
+A python interface for Cytosim
 To use the links, please compile the cytosim documentation. For this run the
 command :
 make doc
+**** List of bound classes and members : ****
 ▼▲PyCytosim
 open loads simulation from object files
 start loads simulation from config files
 str_to_glos converts string to Glossary
 toVector converts numpy array to vector
 toTorque converts numpy array to torque
-▼▲Frame
-Python interface to timeframe : behaves as a Python dictionary of Objectsets
-fibers
-time
-simul
-index
-loaded
-update
-next
-__iter__
-keys
-items
-__getitem__
-▼▲Simul
-load loads a frame by index, e.g. frame = sim.load(2)
-next loads next frame, e.g. frame = sim.next()
-loadframe
-frame returns current frame, e.g. frame = sim.frame()
-writeObjects writes Objects to default trajectory file
-writeObjects writes Objects to a trajectory file, e.g. writeOjects('file.cmo')
-save saves current state to trajectory file
-add adds objects to simulation, see provided examples
-cut performes a cut : sim.cut(filament_name, where), see Parser.execute_cut
-(C++)
-delete deletes objects from simulation, see provided examples
-import imports objects from text file, see provided examples
-export export objects to text file, see provided examples
-run runs the simulation
-set
-prop
-sMeca
-properties
-spaces
-spaces
-fields
-fibers
-spheres
-beads
-solids
-couples
-singles
-organizers
-remove
-erase
-nuke
-time
-time_step
-step
-computeForces
-run
-change
-change_glos
-once
-prepared_solve
-prepare_meca
-prepare
-solve
-solve_auto
-dump
-saveSystem
-evaluate
-Mecable
-Mecable
-findSpace
-rename
-isCategory
-findProperty
-writePropertiesTo
-writeProperties
-writePropertiesToNoPrune
-▼▲Mecapoint
-set
-mecable
-valid
-position
-pos
-overlapping
-near
-▼▲Interpolation
-clear
-set
-valid
-mecable
-exact1
-exact2
-coef1
-coef2
-coef
-position
-pos
-pos1
-pos2
-diff
-len
-lenSqr
-dir
-inside
-overlapping
-overlapPoint
-▼▲Meca
-nb_points
-dimension
-prepare
-addForcePt
-addForce
-addTorque
-addTorqueClamp
-addTorqueParrallel
-addTorqueAngle
-addTorquePoliti
-addPointClampPt
-addPointClamp
-addSphereClamp
-addCylinderClampZ
-addCylinderClampX
-addSidePointClamp
-addLineClamp
-addLineClampPt
-addPlaneClamp
-addPlaneClampPt
-addLink
-addLinkPtI
-addLinkIPt
-addLinkPt
-addLongLink
-addLongLinkPt
-addLongLinkPtI
-addSideLink2D
-addSideLink2DIPt
-addSideSideLink2D
-addSideSlidingLink2D
-addSideSlidingLink2DIPt
-addSideSlidingLinkS
-addSideSlidingLinkSIPt
-addSideLink3D
-addSideLinkS
-addSideLinkSIpt
-addSideSlidingLinkS
-addSideSlidingLinkSIpt
-addSideLink
-addSideLinkIpt
-addSideSideLink
-addSlidingLink
-addSlidingLinkIpt
-addSideSlidingLink
-addSideSlidingLinkIpt
-addTriLink
 ▼▲Object
 reference
 property
 position
-next
+Object
 __next__
-prev
+Object
 id
 writeHeader
 points
 ▼▲Space
 thickness
 resize
 volume
@@ -182,90 +37,74 @@
 signedDistanceToEdge
 bounce
 normalToEdge
 randomPlace
 randomPlaceNearEdge
 randomPlaceOnEdge
 estimateVolume
-▼▲Couple
-position
-active
-stiffness
-force
-cosAngle
-sidePos
-posFree
-attachEnd1
-attachEnd2
-moveToEnd1
-moveToEnd2
-fiber2
-abcissa
-toCouple
-hand1
-hand2
-hand
-state
-__len__
-__getitem__
-▼▲Organizer
-nbOrganized
-position
-positionP
-dragCoefficient
-next
-prev
-▼▲Aster
-solid
-position
-nbFibers
-fiber
-posLink1
-posLink2
-posFiber1
-posFiber2
-getLink1
-getLink2
-getLink
-property
 ▼▲Mecable
 data
 nbPoints
 allocated
-points
+points Returns read-only point coordinates of the mecable
 posPoint
 setPoint
 setPoint
 addPoint
 removePoints
 clearPoints
 shiftPoints
 truncateM
 truncateP
 calculateMomentum
 netForce
 position
 translate
 allInside
+▼▲Sphere
+position
+pos
+Sphere
+resize
+reshape
+orthogonalize
+addSurfacePoint
+nbbSurfacePoints
+dragCoefficient
+Sphere
+Sphere
+Sphere
+▼▲Bead
+position
+Bead
+setPosition
+radius
+radiusSqr
+resize
+volume
+dragCoefficient
+Bead
+Bead
+Bead
 ▼▲Chain
 nbSegments
 lastSegment
 setStraight
 setStraightLength
 placeEnd
 setEquilibrated
 birthTime
 age
-exactEnd
-interpolateEndM
-interpolateEndP
-interpolateCenter
-interpolateEnd
+Mecapoint
+Interpolation
+Interpolation
+Interpolation
+Interpolation
 interpolateFromEnd
-interpolate
+Interpolation
 setEquilibrated
 length1
 trueLength
 betweenMP
 outsideMP
 belowP
 aboveM
@@ -316,75 +155,100 @@
 Fiber
 nbPoints
 cutM
 cutP
 sever
 severNow
 Fiber
-nowSever
 join
 stateM
 stateP
 setStateM
 setStateP
 setDynamicState
 freshAssembly
 nbHands
+addHand
+removeHand
+updateHands
+detachHands
+sortHands
+Hand
 nbHandsInRange
+nbHandsNearEnd
 __next__
 ▼▲ClassicFiber
 freshAssemblyM
 freshAssemblyP
-▼▲Sphere
-position
-pos
-Sphere
-resize
-reshape
-orthogonalize
-addSurfacePoint
-nbbSurfacePoints
-dragCoefficient
-next
-prev
-Sphere
-▼▲Bead
-position
-Bead
-setPosition
-radius
-radiusSqr
-resize
-volume
-dragCoefficient
-next
-prev
-Bead
+▼▲DynamicFiber
+freshAssemblyM
+freshAssemblyP
 ▼▲Solid
 position
 points
 dragCoefficient
 addSphere
 setRadius
 addSphere
 centroid
-next
-prev
+Solid
+Solid
 tag
 property
 nbPoints
 Solid
+▼▲Organizer
+nbOrganized
+position
+positionP
+dragCoefficient
+Organizer
+Organizer
+▼▲Aster
+Solid
+position
+nbFibers
+Fiber
+posLink1
+posLink2
+posFiber1
+posFiber2
+getLink1
+getLink2
+getLink
+property
+▼▲Couple
+position
+active
+stiffness
+force
+cosAngle
+sidePos
+posFree
+attachEnd1
+attachEnd2
+moveToEnd1
+moveToEnd2
+Fiber
+abcissa
+toCouple
+Hand
+Hand
+hand
+state
+__len__
+__getitem__
 ▼▲Single
 toSingle
 state
 __getitem__
 __len__
-hand
+Hand
 Single
-fiber
+Fiber
 abscissa
 posHand
 dirFiber
 attach
 attachEnd
 moveToEnd
 detach
@@ -394,45 +258,57 @@
 setPosition
 randomizePosition
 posFoot
 sidePos
 Mecable
 mobile
 force
-next
-prev
-confineSpace
+Single
+Single
+Space
 ▼▲Property
 name
 change
 read
 change_glos
 read_glos
 complete
 rename
 is_named
 number
 renumber
 clear
 clone
 ▼▲SpaceProp
-▼▲CoupleProp
-hand1
-hand2
-stiffness
-length
-diffusion
-fast_diffusion
-stiff
-Specificity
-confine
+▼▲SolidProp
+drag
+viscosity
+steric
+steric_range
+Confinement
+confine_stiffness
 confine_space
+display
+display_fresh
+▼▲HandProp
+binding_rate
+Hand
+binding_key
+unbinding_rate
+unbinding_force
+bind_also_end
+bind_end_range
+hold_growing_end
+hold_shrinking_end
 activity
-hand1_prop
-hand2_prop
+display
+▼▲MotorProp
+stall_force
+unloaded_speed
+limit_speed
 ▼▲FiberProp
 segmentation
 rigidity
 min_length
 max_length
 total_polymer
 persistent
@@ -451,14 +327,26 @@
 steric_radius
 steric_range
 glue
 glue_single
 activity
 display_fresh
 display
+▼▲ClassicFiberProp
+growing_speed
+growing_off_speed
+growing_force
+shrinking_speed
+catastrophe_rate
+catastrophe_rate_stalled
+▼▲DynamicFiberProp
+growing_speed
+growing_off_speed
+growing_force
+shrinking_speed
 ▼▲SimulProp
 time
 time_step
 viscosity
 kT
 tolerance
 acceptable_prop
@@ -475,144 +363,294 @@
 clear_trajectory
 skip_free_couple
 display_fresh
 display
 read
 read_str
 clone
-▼▲HandProp
-binding_rate
-Hand
-binding_key
-unbinding_rate
-unbinding_force
-bind_also_end
-bind_end_range
-hold_growing_end
-hold_shrinking_end
-activity
-display
-▼▲MotorProp
-stall_force
-unloaded_speed
-limit_speed
-▼▲SolidProp
-drag
-viscosity
-steric
-steric_range
+▼▲CoupleProp
+hand1
+hand2
+stiffness
+length
+diffusion
+fast_diffusion
+stiff
+Specificity
 Confinement
-confine_stiffness
 confine_space
-display
-display_fresh
+activity
+HandProp
+HandProp
 ▼▲SingleProp
 hand
 stiffness
 length
 diffusion
 fast_diffusion
-confine
+Confinement
 confine_space
 activity
-hand_prop
-▼▲ObjectSet
-add
+HandProp
+▼▲Interface
+an interface to cytosim
+add adds objects to simulation, see provided examples
+execute_new adds objects to simulation, see provided examples
+run runs simulation a given number of steps, see provided examples
+execute_run runs simulation a given number of steps, see provided examples
+set defines objects to simulation, see provided examples
+execute_set defines objects to simulation, see provided examples
+execute_change changes objects properties in simulation, see provided examples
+▼▲Parser
+a cytosim parser
+▼▲PythonParser
+Python interface to a parser
+simul
+load
+frame
+next
+▼▲Simul
+execute_cut performes a cut : sim.cut(filament_name, where), see
+Parser.execute_cut (C++)
+execute_delete deletes objects from simulation, see provided examples
+execute_import imports objects from text file, see provided examples
+export export objects to text file, see provided examples
+save saves current state to trajectory file
+frame
+SimulProp
+Meca
+properties
+SpaceSet
+SpaceSet
+FieldSet
+FiberSet
+SphereSet
+BeadSet
+SolidSet
+CoupleSet
+SingleSet
+OrganizerSet
 remove
-link
-unlink
 erase
-erase_all
-size
-__len__
-first
-last
-findID
-Object
-__getitem__
-▼▲CoupleSet
+nuke
+time
+time_step
+step
+computeForces
+once
+prepared_solve
+prepare_meca
+prepare
+solve
+solve_auto
+dump
+saveSystem
+evaluate
+Mecable
+Mecable
+Space
+rename
+isCategory
+findProperty
+writePropertiesTo
+writeProperties
+writePropertiesToNoPrune
+▼▲Frame
+Python interface to timeframe : behaves as a Python dictionary of Objectsets
+fibers
+time
+simul
+index
+loaded
+update
+update
+next
+__iter__
+keys
+items
 __getitem__
-▼▲SpaceSet
-▼▲FiberSet
-▼▲FieldSet
-▼▲SphereSet
-▼▲BeadSet
-▼▲SolidSet
-▼▲OrganizerSet
-▼▲SingleSet
+▼▲Group
+Behaves as a list of objects with the same properties
+__len__
+size
+prop
+__iter__
 __getitem__
 ▼▲Glossary::val_type
 value_
 defined_
 count_
 __repr__
 ▼▲Glossary
 terms
 __repr__
 __iter__
 __getitem__
 __setitem__
 keys
 items
-▼▲Vector
-▼▲Vector3
-▼▲realArray
+▼▲Mecapoint
+Mecapoint
+set
+Mecable
+valid
+position
+pos
+overlapping
+near
+▼▲Interpolation
+clear
+set
+valid
+Mecable
+Mecapoint
+Mecapoint
+coef1
+coef2
+coef
+position
+pos
+pos1
+pos2
+diff
+len
+lenSqr
+dir
+inside
+overlapping
+overlapPoint
 ▼▲FiberSite
 moveTo
 relocateM
 relocateP
 Fiber
 Fiber
 update
 Interpolation
-fiber
+Fiber
 position
 posHand
 direction
 dirFiber
 abscissa
 abscissaFromM
 abscissaFromP
 abscissaFrom
-nearestEnd
+FiberEnd
 distanceToEnd
 ▼▲Hand
-property
-prop
+Hand
+Hand
+HandProp
+HandProp
 relocate
 relocateTo
 moveToEnd
 locate
 attach
 detach
 attachEnd
 attachTo
-otherHand
+Hand
 otherPosition
 linkStiffness
 moveTo
 relocateM
 relocateP
 unattached
 attached
 update
 Interpolation
-fiber
+Fiber
 position
 posHand
 direction
 dirFiber
 abscissa
 abscissaFromM
 abscissaFromP
 abscissaFrom
-nearestEnd
+FiberEnd
 distanceToEnd
-▼▲Group
-__len__
+▼▲Meca
+nb_points
+dimension
+prepare
+base
+points
+force
+addForcePt
+addForce
+addTorque
+addTorqueClamp
+addTorqueParrallel
+addTorqueAngle
+addTorquePoliti
+addPointClampPt
+addPointClamp
+addSphereClamp
+addCylinderClampZ
+addCylinderClampX
+addSidePointClamp
+addLineClamp
+addLineClampPt
+addPlaneClamp
+addPlaneClampPt
+addLink
+addLinkPtI
+addLinkIPt
+addLinkPt
+addLongLink
+addLongLinkPt
+addLongLinkPtI
+addSideLink2D
+addSideLink2DIPt
+addSideSideLink2D
+addSideSlidingLink2D
+addSideSlidingLink2DIPt
+addSideSlidingLinkS
+addSideSlidingLinkSIPt
+addSideLink3D
+addSideLinkS
+addSideLinkSIpt
+addSideSlidingLinkS
+addSideSlidingLinkSIpt
+addSideLink
+addSideLinkIpt
+addSideSideLink
+addSlidingLink
+addSlidingLinkIpt
+addSideSlidingLink
+addSideSlidingLinkIpt
+addTriLink
+▼▲Vector
+▼▲Vector3
+▼▲realArray
+▼▲ObjectSet
+add
+remove
+link
+unlink
+erase
+erase_all
 size
-prop
-__iter__
+__len__
+Object
+Object
+Object
+Object
+__getitem__
+▼▲SpaceSet
+▼▲FiberSet
+▼▲FieldSet
+▼▲SphereSet
+▼▲BeadSet
+▼▲SolidSet
+▼▲OrganizerSet
+▼▲CoupleSet
+__getitem__
+▼▲SingleSet
 __getitem__
 ▼▲ObjectList
+A list-like structure of Cytosim objects
 __getitem__
 __len__
```

### Comparing `cytosim-0.0.1/doc/cpython/read_cpython.py` & `cytosim-0.0.2/doc/cpython/read_cpython.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/data/cytosim.png` & `cytosim-0.0.2/doc/data/cytosim.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/data/modularity.png` & `cytosim-0.0.2/doc/data/modularity.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/biblio.md` & `cytosim-0.0.2/doc/examples/biblio.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/data/actin.png` & `cytosim-0.0.2/doc/examples/data/actin.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/data/ashbya.png` & `cytosim-0.0.2/doc/examples/data/ashbya.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/data/celegans.png` & `cytosim-0.0.2/doc/examples/data/celegans.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/data/centering.png` & `cytosim-0.0.2/doc/examples/data/centering.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/data/droplets.png` & `cytosim-0.0.2/doc/examples/data/droplets.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/data/endocytosis.png` & `cytosim-0.0.2/doc/examples/data/endocytosis.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/data/minifilaments.png` & `cytosim-0.0.2/doc/examples/data/minifilaments.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/data/nematics.png` & `cytosim-0.0.2/doc/examples/data/nematics.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/data/network.png` & `cytosim-0.0.2/doc/examples/data/network.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/data/patterns.png` & `cytosim-0.0.2/doc/examples/data/patterns.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/data/spindle.png` & `cytosim-0.0.2/doc/examples/data/spindle.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/data/spindle_length.png` & `cytosim-0.0.2/doc/examples/data/spindle_length.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/data/spombe.png` & `cytosim-0.0.2/doc/examples/data/spombe.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/examples/index.md` & `cytosim-0.0.2/doc/examples/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/index.md` & `cytosim-0.0.2/doc/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/main/credits.md` & `cytosim-0.0.2/doc/main/credits.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/main/examples.md` & `cytosim-0.0.2/doc/main/examples.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/main/executables.md` & `cytosim-0.0.2/doc/main/executables.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/main/faq.md` & `cytosim-0.0.2/doc/main/faq.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/main/file_types.md` & `cytosim-0.0.2/doc/main/file_types.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/main/movies.md` & `cytosim-0.0.2/doc/main/movies.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/main/overview.md` & `cytosim-0.0.2/doc/main/overview.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/main/run_slurm.md` & `cytosim-0.0.2/doc/main/run_slurm.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/main/runs.md` & `cytosim-0.0.2/doc/main/runs.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/main/starter.md` & `cytosim-0.0.2/doc/main/starter.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/misc/Cytosim.tmbundle.zip` & `cytosim-0.0.2/doc/misc/Cytosim.tmbundle.zip`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/outreach/controller.md` & `cytosim-0.0.2/doc/outreach/controller.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/outreach/data/CRI-2018-11a.jpg` & `cytosim-0.0.2/doc/outreach/data/CRI-2018-11a.jpg`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/outreach/data/CRI-2018-11b.jpg` & `cytosim-0.0.2/doc/outreach/data/CRI-2018-11b.jpg`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/outreach/data/Cambridge-2019-05a.jpg` & `cytosim-0.0.2/doc/outreach/data/Cambridge-2019-05a.jpg`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/outreach/data/Cambridge-2019-05b.jpg` & `cytosim-0.0.2/doc/outreach/data/Cambridge-2019-05b.jpg`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/outreach/games/index.md` & `cytosim-0.0.2/doc/outreach/games/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/outreach/installation1.md` & `cytosim-0.0.2/doc/outreach/installation1.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/outreach/installation2.md` & `cytosim-0.0.2/doc/outreach/installation2.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/rendering/actin.blend` & `cytosim-0.0.2/doc/rendering/actin.blend`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/rendering/import-actin-ico.py` & `cytosim-0.0.2/doc/rendering/import-actin-ico.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/rendering/import-actin-sphere.py` & `cytosim-0.0.2/doc/rendering/import-actin-sphere.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/rendering/import-actin.py` & `cytosim-0.0.2/doc/rendering/import-actin.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/rendering/import-links.py` & `cytosim-0.0.2/doc/rendering/import-links.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/rendering/index.md` & `cytosim-0.0.2/doc/rendering/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/commands.md` & `cytosim-0.0.2/doc/sim/commands.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/config.md` & `cytosim-0.0.2/doc/sim/config.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/data/forces.cym` & `cytosim-0.0.2/doc/sim/data/forces.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/data/forces.png` & `cytosim-0.0.2/doc/sim/data/forces.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/data/meca_links.png` & `cytosim-0.0.2/doc/sim/data/meca_links.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/data/steric.png` & `cytosim-0.0.2/doc/sim/data/steric.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/data/steric3D.png` & `cytosim-0.0.2/doc/sim/data/steric3D.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/data/steric_math.png` & `cytosim-0.0.2/doc/sim/data/steric_math.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/data/varying_time_step.png` & `cytosim-0.0.2/doc/sim/data/varying_time_step.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/fiber_dynamics.md` & `cytosim-0.0.2/doc/sim/fiber_dynamics.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/fibers.md` & `cytosim-0.0.2/doc/sim/fibers.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/forces.md` & `cytosim-0.0.2/doc/sim/forces.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/graphics.md` & `cytosim-0.0.2/doc/sim/graphics.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/index.md` & `cytosim-0.0.2/doc/sim/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/motor_detachment.md` & `cytosim-0.0.2/doc/sim/motor_detachment.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/numerical_precision.md` & `cytosim-0.0.2/doc/sim/numerical_precision.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/objects.md` & `cytosim-0.0.2/doc/sim/objects.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/placement.md` & `cytosim-0.0.2/doc/sim/placement.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/report.md` & `cytosim-0.0.2/doc/sim/report.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/spaces.md` & `cytosim-0.0.2/doc/sim/spaces.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/steric.md` & `cytosim-0.0.2/doc/sim/steric.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/stochastic.md` & `cytosim-0.0.2/doc/sim/stochastic.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/sim/units.md` & `cytosim-0.0.2/doc/sim/units.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/code/collect.py` & `cytosim-0.0.2/doc/tutorials/code/collect.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/code/config.cym.tpl` & `cytosim-0.0.2/doc/tutorials/code/config.cym.tpl`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/code/master.sh` & `cytosim-0.0.2/doc/tutorials/code/master.sh`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/code/preconfig` & `cytosim-0.0.2/doc/tutorials/code/preconfig`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/code/scan.py` & `cytosim-0.0.2/doc/tutorials/code/scan.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/data/ashbya.cym` & `cytosim-0.0.2/doc/tutorials/data/ashbya.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/data/aster.cym` & `cytosim-0.0.2/doc/tutorials/data/aster.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/data/aster_dynamic.cym` & `cytosim-0.0.2/doc/tutorials/data/aster_dynamic.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/data/capture.cym` & `cytosim-0.0.2/doc/tutorials/data/capture.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/data/end_tracking.png` & `cytosim-0.0.2/doc/tutorials/data/end_tracking.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/data/filament_buckling.png` & `cytosim-0.0.2/doc/tutorials/data/filament_buckling.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/data/gliding.cym` & `cytosim-0.0.2/doc/tutorials/data/gliding.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/data/polarity_sorting.png` & `cytosim-0.0.2/doc/tutorials/data/polarity_sorting.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/data/self.cym` & `cytosim-0.0.2/doc/tutorials/data/self.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/H.png` & `cytosim-0.0.2/doc/tutorials/images/H.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/XTV.png` & `cytosim-0.0.2/doc/tutorials/images/XTV.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/aster-vs-nematic.png` & `cytosim-0.0.2/doc/tutorials/images/aster-vs-nematic.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/bind_also_end.png` & `cytosim-0.0.2/doc/tutorials/images/bind_also_end.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/bind_end.png` & `cytosim-0.0.2/doc/tutorials/images/bind_end.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/couples.png` & `cytosim-0.0.2/doc/tutorials/images/couples.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/crosslinks.png` & `cytosim-0.0.2/doc/tutorials/images/crosslinks.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/droplets.png` & `cytosim-0.0.2/doc/tutorials/images/droplets.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/force_velocity.png` & `cytosim-0.0.2/doc/tutorials/images/force_velocity.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/gliding1.png` & `cytosim-0.0.2/doc/tutorials/images/gliding1.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/gliding2.png` & `cytosim-0.0.2/doc/tutorials/images/gliding2.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/kinesin_tetramers.png` & `cytosim-0.0.2/doc/tutorials/images/kinesin_tetramers.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/meca_links.png` & `cytosim-0.0.2/doc/tutorials/images/meca_links.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/images/nematic-vs-polar.png` & `cytosim-0.0.2/doc/tutorials/images/nematic-vs-polar.png`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/index.md` & `cytosim-0.0.2/doc/tutorials/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/tuto_capture.md` & `cytosim-0.0.2/doc/tutorials/tuto_capture.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/tuto_centering.md` & `cytosim-0.0.2/doc/tutorials/tuto_centering.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/tuto_contract2.md` & `cytosim-0.0.2/doc/tutorials/tuto_contract2.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/tuto_contract3.md` & `cytosim-0.0.2/doc/tutorials/tuto_contract3.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/tuto_contract_motor.md` & `cytosim-0.0.2/doc/tutorials/tuto_contract_motor.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/tuto_gliding.md` & `cytosim-0.0.2/doc/tutorials/tuto_gliding.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/tuto_introduction.md` & `cytosim-0.0.2/doc/tutorials/tuto_introduction.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/tuto_nucleus.md` & `cytosim-0.0.2/doc/tutorials/tuto_nucleus.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/tuto_polar_nematic.md` & `cytosim-0.0.2/doc/tutorials/tuto_polar_nematic.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/tuto_scans.md` & `cytosim-0.0.2/doc/tutorials/tuto_scans.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/tuto_scripting.md` & `cytosim-0.0.2/doc/tutorials/tuto_scripting.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/doc/tutorials/tuto_self.md` & `cytosim-0.0.2/doc/tutorials/tuto_self.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/examples/avoid.cym` & `cytosim-0.0.2/examples/avoid.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/examples/flock.cym` & `cytosim-0.0.2/examples/flock.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/examples/pycytoplay_callbacks.ipynb` & `cytosim-0.0.2/examples/pycytoplay_callbacks.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9901570266153599%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(10, 'Warning : this notebook may not work on all platforms. "*

 * *            "You might have to run *callbacks_pycytoplay.py* instead.')], delete: [10]}}, 3: "*

 * *            '{\'outputs\': [], \'source\': [\'parser = cytoplay.start("avoid.cym")\\n\', \'sim = '*

 * *            "parser.simul']}, 7: {'source': {insert: [(0, 'def runtime_all(s, speed, acc, "*

 * *            'parser):\\n\'), (10, \'            parser.execute_change("good","display = (color = '*

 * *            'red)")\\n\')] […]*

```diff
@@ -10,15 +10,15 @@
                 "Here we showcase a simple cytosim simulation where an object can be controled by the keyboard.  \n",
                 "Before running, copy or move the cytoplay module (cytoplay.---.so) to the current folder. \n",
                 "```bash\n",
                 "$ make -j4 pycytoplay\n",
                 "$ cp bin/*.so examples/\n",
                 "```\n",
                 "\n",
-                "Warning : this notebook may not work on all platforms. You might have to run *pycytoplay_callbacks.py* instead."
+                "Warning : this notebook may not work on all platforms. You might have to run *callbacks_pycytoplay.py* instead."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
@@ -35,25 +35,18 @@
                 "Here we simulate one hero bead trying to avoid larger beads."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "WARNING : live usage of PyCytosim is still experimental.\n"
-                    ]
-                }
-            ],
+            "outputs": [],
             "source": [
-                "sim = cytoplay.start(\"avoid.cym\")"
+                "parser = cytoplay.start(\"avoid.cym\")\n",
+                "sim = parser.simul"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [],
@@ -86,25 +79,25 @@
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
             "outputs": [],
             "source": [
-                "def runtime_all(s, speed, acc):\n",
+                "def runtime_all(s, speed, acc, parser):\n",
                 "    frame = s.frame()\n",
                 "    hero = frame[\"good\"][0]\n",
                 "    bads = frame[\"bad\"]\n",
                 "    pts =  np.array(hero.data(), copy=False)\n",
                 "    for bad in bads:\n",
                 "        id = bad.id()\n",
                 "        pt = np.array(bad.data(), copy=False) \n",
                 "        pt += speedos[int(id)]\n",
                 "        if np.sum(np.square(pts-pt)) < distSqr:\n",
-                "            s.change(\"good\",\"display = (color = red)\")\n",
+                "            parser.execute_change(\"good\",\"display = (color = red)\")\n",
                 "    \n",
                 "    speed -= speed*decel\n",
                 "    speed += acc*dt\n",
                 "    ns = np.sqrt(np.sum(np.square(speed)))\n",
                 "    if ns>maxspeed:\n",
                 "        speed *= maxspeed/ns\n",
                 "    pts += speed*dt\n",
@@ -114,15 +107,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
             "outputs": [],
             "source": [
-                "runtime = lambda s:runtime_all(s, speed, acc)"
+                "runtime = lambda s:runtime_all(s, speed, acc, parser)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Defining a callback function for input keys\n",
@@ -222,27 +215,27 @@
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.9.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `cytosim-0.0.1/examples/pycytosim_import3D.ipynb` & `cytosim-0.0.2/examples/pycytosim_import3D.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9899636243386244%*

 * *Differences: {"'cells'": '{4: {\'source\': [\'parser = cytosim.start("../cym/fiber.cym")\\n\', \'sim = '*

 * *            "parser.simul']}, 7: {'source': {insert: [(2, "*

 * *            '\'parser.set("fiber","actin",actin_props);\')], delete: [2]}}, 11: {\'source\': '*

 * *            "{insert: [(1, 'parser.save()\\n'), (4, '    parser.save()')], delete: [4, 1]}}, 13: "*

 * *            '{\'source\': [\'parser.change("actin","segmentation = %s" %(ds*5))\']}, 14: '*

 * *            "{'source': {insert: [(0, 'parser.save()\\n'), (3, '    parser. […]*

```diff
@@ -42,15 +42,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sim = cytosim.start(\"../cym/fiber.cym\")"
+                "parser = cytosim.start(\"../cym/fiber.cym\")\n",
+                "sim = parser.simul"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [],
@@ -71,15 +72,15 @@
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [],
             "source": [
                 "ds = 0.003\n",
                 "actin_props = \"rigidity = 0.01 ; segmentation = %s ; confine = inside, 200, cell\" %ds\n",
-                "sim.set(\"fiber\",\"actin\",actin_props);"
+                "parser.set(\"fiber\",\"actin\",actin_props);"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Loading from file \n",
@@ -125,18 +126,18 @@
         {
             "cell_type": "code",
             "execution_count": 7,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Running several timesteps and saving\n",
-                "sim.save()\n",
+                "parser.save()\n",
                 "for i in range(10):\n",
                 "    sim.once()\n",
-                "    sim.save()"
+                "    parser.save()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Changing segmentation size\n",
@@ -145,27 +146,27 @@
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sim.change(\"actin\",\"segmentation = %s\" %(ds*5))"
+                "parser.change(\"actin\",\"segmentation = %s\" %(ds*5))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sim.save()\n",
+                "parser.save()\n",
                 "for i in range(20):\n",
                 "    sim.once()\n",
-                "    sim.save()"
+                "    parser.save()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Playing the results\n",
@@ -227,27 +228,27 @@
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.9.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `cytosim-0.0.1/examples/pycytosim_obj_3D.ipynb` & `cytosim-0.0.2/examples/pycytosim_obj_3D.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9889938186813187%*

 * *Differences: {"'cells'": '{4: {\'source\': [\'parser = cytosim.start("../cym/fiber.cym")\\n\', \'sim = '*

 * *            'parser.simul\']}, 5: {\'source\': {insert: [(1, \'parser.add("filament","length = '*

 * *            '5",50)\\n\'), (2, \'parser.run(10)\\n\')], delete: [2, 1]}}, 6: {\'source\': {insert: '*

 * *            '[(3, \'s = parser.set("hand","kinesin",kin_props)\\n\'), (5, '*

 * *            '\'parser.set("couple","motor",mot_props)\\n\'), (6, \'a = '*

 * *            'parser.add("motor","",1000)\\n\'), (7, \'parser.run(500)\\n\ […]*

```diff
@@ -73,15 +73,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [],
             "source": [
-                "sim = cytosim.start(\"../cym/fiber.cym\")"
+                "parser = cytosim.start(\"../cym/fiber.cym\")\n",
+                "sim = parser.simul"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
@@ -98,16 +99,16 @@
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "# Adding with instructions\n",
-                "sim.add(\"filament\",\"length = 5\",50)\n",
-                "sim.run(10)\n",
+                "parser.add(\"filament\",\"length = 5\",50)\n",
+                "parser.run(10)\n",
                 "plot_sim(sim)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "metadata": {},
@@ -127,45 +128,45 @@
                     "output_type": "display_data"
                 }
             ],
             "source": [
                 "kin_props = \"binding_rate=10; binding_range=0.1; \\\n",
                 "    unbinding_rate = 0.3 ; unbinding_force = 5 ; \\\n",
                 "    activity=move; unloaded_speed = 1.0 ; stall_force = 5 ;hold_growing_end=1 ; \"\n",
-                "s = sim.set(\"hand\",\"kinesin\",kin_props)\n",
+                "s = parser.set(\"hand\",\"kinesin\",kin_props)\n",
                 "mot_props = \"hand1=kinesin ; hand2=kinesin ; stiffness=100 ; diffusion=100 ; length = 0.05\"\n",
-                "sim.set(\"couple\",\"motor\",mot_props)\n",
-                "a = sim.add(\"motor\",\"\",1000)\n",
-                "sim.run(500)\n",
+                "parser.set(\"couple\",\"motor\",mot_props)\n",
+                "a = parser.add(\"motor\",\"\",1000)\n",
+                "parser.run(500)\n",
                 "plot_sim(sim)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.9.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `cytosim-0.0.1/makefile` & `cytosim-0.0.2/makefile`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/makefile.inc` & `cytosim-0.0.2/makefile.inc`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 
 
 # common options for all C++ objects:
 CXXFLG := -std=gnu++14 -Wredeclared-class-member -Wno-deprecated-declarations
 CXXFLG := -std=gnu++14 -fopenmp #-g -fno-inline
 #CXXFLG := -std=gnu++14 -fPIC $(PYTHON1)
-CXXFLG := -std=gnu++14 -fPIC
+CXXFLG := -std=gnu++14 -fPIC -fno-builtin
 
 # option concerning memory alignment:
 ALIGN  := -malign-double -falign-loops -falign-jumps -falign-functions
 ALIGN  :=
 
 # options concerning warnings:
 WARN   := -Wundef -Wall -Wno-unknown-pragmas# -Wno-unused
```

### Comparing `cytosim-0.0.1/module/cytosim.egg-info/PKG-INFO` & `cytosim-0.0.2/src/cytosim.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cytosim
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cytosim: Langevin dynamics of active polymer networks
 Keywords: simulation actin microtubule polymer
 Platform: Windows
 Platform: Linux
 Platform: Mac OS-X
 Platform: Unix
 Description-Content-Type: text/markdown
@@ -69,15 +69,15 @@
 	git clone https://gitlab.com/f.nedelec/cytosim
 	cd cytosim
 	
 To compile using [make](https://www.gnu.org/software/make), try:
 	
 	make
 
-If this fails, parameters of `makefile.inc` need to be updated.
+If this fails, parameters of `makefile.inc` need to be updated manually.
 Altermatively, it is possible to use [cmake](https://cmake.org) to configure `make` automatically:
 
 	mkdir build
 	cd build
 	cmake ..
 	make
 
@@ -100,15 +100,15 @@
 *  Jonathan Ward           2008-2014
 *  Antonio Politi          2010-2012
 *  Andre-Claude Clapson    2011-2013
 *  Jamie-Li Rickman        2014-2019
 *  Serge Dmitrieff         2013-
 *  Julio Belmonte          2014-
 *  Gaelle Letort           2014-
-*  Manuel Lera-Ramirez     2017-
-*  Maud Formanek           2020-
+*  Manuel Lera-Ramirez     2017-2022
+*  Maud Formanek           2020-2021
 
 # Contact
 
 Email: cytosim@cytosim.org
```

### Comparing `cytosim-0.0.1/module/cytosim.egg-info/SOURCES.txt` & `cytosim-0.0.2/src/cytosim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .gitignore
 CMakeLists.txt
 LICENSE.txt
 PYCYTOSIM.md
 README.md
 WARRANTY.txt
-demo_cythosim.ipynb
 demo_frame.ipynb
+demo_pycytosim.ipynb
 example.cym
 makefile
 makefile.inc
 setup.py
 cym/actin.cym
 cym/amplify.cym
 cym/arp23.cym
@@ -341,28 +341,24 @@
 doc/tutorials/images/force_velocity.png
 doc/tutorials/images/gliding1.png
 doc/tutorials/images/gliding2.png
 doc/tutorials/images/kinesin_tetramers.png
 doc/tutorials/images/meca_links.png
 doc/tutorials/images/nematic-vs-polar.png
 examples/avoid.cym
+examples/callbacks_pycytoplay.py
 examples/flock.cym
 examples/pycytoplay_callbacks.ipynb
 examples/pycytosim_construct.ipynb
 examples/pycytosim_extend.ipynb
 examples/pycytosim_flock.ipynb
 examples/pycytosim_import3D.ipynb
 examples/pycytosim_meca.ipynb
 examples/pycytosim_obj_3D.ipynb
 examples/pycytosim_objects.ipynb
-module/cytosim.egg-info/PKG-INFO
-module/cytosim.egg-info/SOURCES.txt
-module/cytosim.egg-info/dependency_links.txt
-module/cytosim.egg-info/not-zip-safe
-module/cytosim.egg-info/top_level.txt
 python/index.md
 python/look/collect.py
 python/look/compare_config.py
 python/look/get_data.py
 python/look/make_image.py
 python/look/make_movie.py
 python/look/make_page.py
@@ -422,24 +418,31 @@
 src/base/timer.h
 src/base/tokenizer.cc
 src/base/tokenizer.h
 src/cpython/couple_modules.h
 src/cpython/fiber_modules.h
 src/cpython/glossary_modules.h
 src/cpython/hand_modules.h
+src/cpython/interface_modules.h
 src/cpython/meca_modules.h
 src/cpython/object_modules.h
 src/cpython/organizer_modules.h
 src/cpython/point_modules.h
 src/cpython/python_frame.h
 src/cpython/python_utilities.h
 src/cpython/simul_modules.h
 src/cpython/single_modules.h
 src/cpython/solid_modules.h
 src/cpython/space_modules.h
+src/cpython/thread_modules.h
+src/cytosim.egg-info/PKG-INFO
+src/cytosim.egg-info/SOURCES.txt
+src/cytosim.egg-info/dependency_links.txt
+src/cytosim.egg-info/not-zip-safe
+src/cytosim.egg-info/top_level.txt
 src/disp/CMakeLists.txt
 src/disp/display.cc
 src/disp/display.h
 src/disp/display1.cc
 src/disp/display1.h
 src/disp/display2.cc
 src/disp/display2.h
```

### Comparing `cytosim-0.0.1/python/index.md` & `cytosim-0.0.2/python/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/look/collect.py` & `cytosim-0.0.2/python/look/collect.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/look/compare_config.py` & `cytosim-0.0.2/python/look/compare_config.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/look/get_data.py` & `cytosim-0.0.2/python/look/get_data.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/look/make_image.py` & `cytosim-0.0.2/python/look/make_image.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/look/make_movie.py` & `cytosim-0.0.2/python/look/make_movie.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/look/make_page.py` & `cytosim-0.0.2/python/look/make_page.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/look/make_plots.py` & `cytosim-0.0.2/python/look/make_plots.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/look/read_config.py` & `cytosim-0.0.2/python/look/read_config.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/look/scan.py` & `cytosim-0.0.2/python/look/scan.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/look/tell.py` & `cytosim-0.0.2/python/look/tell.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/misc/battery_test.py` & `cytosim-0.0.2/python/misc/battery_test.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/misc/cleanup.py` & `cytosim-0.0.2/python/misc/cleanup.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/misc/compare.py` & `cytosim-0.0.2/python/misc/compare.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/misc/plot.py` & `cytosim-0.0.2/python/misc/plot.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/misc/pyned.py` & `cytosim-0.0.2/python/misc/pyned.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/misc/reduce.py` & `cytosim-0.0.2/python/misc/reduce.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/run/go_sim.py` & `cytosim-0.0.2/python/run/go_sim.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/run/go_sim_lib.py` & `cytosim-0.0.2/python/run/go_sim_lib.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/run/preconfig.py` & `cytosim-0.0.2/python/run/preconfig.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
 #
 # PRECONFIG, a versatile configuration file generator for varying parameters
 #
 # Copyright Francois J. Nedelec and  Serge Dmitrieff, 
 # EMBL 2010--2017, Cambridge University 2019--2022
-# This is PRECONFIG version 1.57, last modified on 15.06.2022
+# This is PRECONFIG version 1.59, last modified on 03.02.2023
 
 """
 # SYNOPSIS
 
    Preconfig generates files from a template by evaluating doubly-bracketed Python code.
    
 # Article:
@@ -171,20 +171,20 @@
 ## Example 7
 
    Randomize a value, and print this value as a comment in the file.
    The second line below the [[...]] prints a comment, from which the value
    of 'x' can be read. This can be useful to process the results later.
 
     [[ x = random.uniform(0,1) ]]
-    %preconfig.x= [[ x ]]
+    %config.x= [[ x ]]
     binding_rate = [[ 10*x ]]
     unbinding_rate = [[ 2*x ]]
 
    Command: `preconfig 256 TEMPLATE_FILE` to make 256 files.
-   Extract values:  awk '/%preconfig./{sub("%preconfig.","");print}' config0000.cym
+   To get values: awk '/%config./{sub("%config.","");print}' config0000.cym
 
 ## Example 8
 
    Quotations can be used to aggregate values:
 
     [[ vec = ['-1 0 1', '0 1 1', '-1 0 -1'] ]]
     new microtubule
@@ -222,17 +222,17 @@
     GLOBALS = { 'random': __import__('random'), 'math': __import__('math') }
 except ImportError as e:
     sys.stderr.write("Preconfig could not load `%s`\n"%str(e))
     sys.exit(7)
 
 #-------------------------------------------------------------------------------
 
-__VERSION__="1.57"
+__VERSION__="1.58"
 
-__DATE__ ="15.06.2022"
+__DATE__ ="29.09.2022"
 
 # code snippets are surrounded by double square brackets:
 CODE = '['
 DECO = ']'
 
 
 # A function to return version to be able to pip package it
@@ -403,15 +403,15 @@
                 sys.stderr.write("Preconfig kept `%s' verbatim since %s" % (code, str(e)))
                 sys.stderr.write("\033[0m")
                 sys.stderr.write("\n")
             exit_code = 1
             #print(self.locals)
             self.report(blok, '', blok)
             return ('', blok)
-        self.report(code, k, v)
+        self.report(code, k, res)
         return (k, res)
     
     def process(self, file, text):
         """
             Identify and recursively substitute bracketed code blocks embedded
             in the input `file`. Generate output file evetytime EOF is reached.
         """
@@ -429,24 +429,24 @@
                 # having exhausted the input, we generate a file:
                 self.make_file(output)
                 return
             # remove outer brackets:
             key = ''
             code = blok[2:-2].strip()
             # print("%4i characters... " % len(pre), end='')
-            # print("code block `%s'" % blok)
             if code[0]==CODE and code[1]==CODE and code[-1]==DECO and code[-2]==DECO:
                 # any further level of bracketting is not evaluated:
                 val = code
             elif code in self.locals:
                 # a defined variable is substituted but not expanded:
                 val = repr(self.locals[code])
             else:
                 # check the code for assigment, and evaluate code:
                 key, vals = self.try_assignment(code, blok)
+                # print("code block `%s' -> %s" % (blok, vals))
                 if key:
                     self.locals[key] = vals
                 try:
                     # use 'pop()' to probe if multiple values were specified...
                     # setting last value aside for later:
                     val = vals.pop()
                     ipos = file.tell()
@@ -518,14 +518,19 @@
         self.out.write('  \\'+('> '+dst+'\n').rjust(96, '-'))
         # write log:
         if self.log:
             self.write_log(dst)
         # get ready for next file:
         self.locals['n'] += 1
 
+    def clear_locals(self):
+        n = self.locals['n']
+        self.locals.clear()
+        self.locals['n'] = n
+
     def expand(self, values, file, text):
         """
             Calls itself recursively to remove all entries of the `values`
             dictionary that are associated with multiple values.
         """
         (key, vals) = pop_sequence(values, self.protected)
         if key:
@@ -543,31 +548,31 @@
             #copy variables to local dictionnary:
             for k, v in values.items():
                 self.locals[k] = v
             #the file index should only be copied once:
             values.pop('n', 0)
             self.process(file, text)
 
-    def parse(self, name, values, repeat=1, path=''):
+    def parse(self, name, file, values, repeat=1, path=''):
         """
             process one file, and return the list of files generated
         """
         self.set_template(name)
         if not self.pattern:
             self.set_pattern(name, path)
         if not os.path.isdir(path):
             self.file_name = path
         for x in range(repeat):
             try:
-                f = open(name, 'r')
-                self.expand(values, f, '')
-                f.close()
+                self.expand(values, file, '')
             except IOError:
                 sys.stderr.write("Preconfig could not load `%s`\n"%name)
                 break
+            self.clear_locals()
+            file.seek(0)
         return self.files_made
 
     def main(self, args):
         """
             process arguments and perform corresponding task
         """
         repeat = 1
@@ -623,29 +628,35 @@
 
         if not inputs:
             sys.stderr.write("Preconfig expects an input template file\n")
             sys.exit(3)
 
         for i in inputs:
             #out.write("Reading %s\n" % i)
-            res = self.parse(i, values, repeat, path)
+            with open(i, 'r') as f:
+                res = self.parse(i, f, values, repeat, path)
             if self.verbose > 0:
                 if len(res) == 1:
                     print("generated %s" % res[0])
                 else:
                     print("%i files generated: %s ... %s" % (len(res), res[0], res[-1]))
 
 
 #-------------------------------------------------------------------------------
 
 def parse(name, values, repeat=1, path=''):
     """
     Process one file, and return the list of files generated
     """
-    return Preconfig().parse(name, values, repeat, path)
+    try:
+        with open(name, 'r') as file:
+            return Preconfig().parse(name, file, values, repeat, path)
+    except FileNotFoundError:
+        print("No such file `%s`" % name)
+    return []
 
 
 if __name__ == "__main__":
     if len(sys.argv) < 2:
         print("You must specify a template file (for instructions, invoke with option '--help')")
     elif sys.argv[1].endswith("help"):
         print(__doc__)
```

### Comparing `cytosim-0.0.1/python/run/submit_one.py` & `cytosim-0.0.2/python/run/submit_one.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/python/run/submit_slurm.py` & `cytosim-0.0.2/python/run/submit_slurm.py`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/setup.py` & `cytosim-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 Cytosim is a simulation tool for cytoskeleton and polymers.
 """
 # setup.py stolen from mem3dg : https://github.com/RangamaniLabUCSD/Mem3DG
 import os
 import sys
 import subprocess
 import re
-version = "0.0.1"
+version = "0.0.2"
 cmake_args=[]
 
 if('CONDA_PREFIX' in os.environ):
     print("Setting library search path (CMAKE_PREFIX_PATH): %s"%(os.environ['CONDA_PREFIX']))
     cmake_args.append('-DCMAKE_PREFIX_PATH=%s'%(os.environ['CONDA_PREFIX']))
 
 DOCLINES = __doc__.split("\n")
 
 CLASSIFIERS = """\
 Development Status :: 3 - Alpha
 Environment :: Console
 Intended Audience :: Science/Research
-License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+License :: OSI Approved :: GNU Public License 3.0 (GPL 3.0)
 Natural Language :: English
 Operating System :: OS Independent
 Programming Language :: C++
 Programming Language :: Python :: 3 :: Only
 Programming Language :: Python :: Implementation :: CPython
 Topic :: Scientific/Engineering :: Chemistry
 Topic :: Scientific/Engineering :: Mathematics
@@ -51,19 +51,19 @@
     version=version,
     #packages=find_packages(where="python_src"),
     #package_dir={"": "python_src"},
     #cmake_install_dir="build",
     #include_package_data=True,
     #extras_require={"test": ["pytest"]},
     #packages=find_packages(where="src/tools"),
-    packages=find_packages(where="module"),
-    package_dir={"": "module"},
-    cmake_install_dir="module",
+    #packages=find_packages(where="module"),
+    #package_dir={"": "module"},
+    #cmake_install_dir="module",
     description=DOCLINES[0],
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     platforms=["Windows", "Linux", "Mac OS-X", "Unix"],
     #classifiers=[c for c in CLASSIFIERS.split("\n") if c],
     keywords="simulation actin microtubule polymer",
     cmake_args=cmake_args,
     zip_safe=False,
-)
+)
```

### Comparing `cytosim-0.0.1/src/base/CMakeLists.txt` & `cytosim-0.0.2/src/base/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/array.h` & `cytosim-0.0.2/src/base/array.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/assert_macro.h` & `cytosim-0.0.2/src/base/assert_macro.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/backtrace.cc` & `cytosim-0.0.2/src/base/backtrace.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/backtrace.h` & `cytosim-0.0.2/src/base/backtrace.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/buddy.h` & `cytosim-0.0.2/src/base/buddy.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/exceptions.h` & `cytosim-0.0.2/src/base/exceptions.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/filepath.cc` & `cytosim-0.0.2/src/base/filepath.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/filepath.h` & `cytosim-0.0.2/src/base/filepath.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/filewrapper.cc` & `cytosim-0.0.2/src/base/filewrapper.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/filewrapper.h` & `cytosim-0.0.2/src/base/filewrapper.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/glossary.cc` & `cytosim-0.0.2/src/base/glossary.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/glossary.h` & `cytosim-0.0.2/src/base/glossary.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/inventoried.h` & `cytosim-0.0.2/src/base/inventoried.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/inventory.cc` & `cytosim-0.0.2/src/base/inventory.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/inventory.h` & `cytosim-0.0.2/src/base/inventory.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/iowrapper.cc` & `cytosim-0.0.2/src/base/iowrapper.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/iowrapper.h` & `cytosim-0.0.2/src/base/iowrapper.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/makefile.inc` & `cytosim-0.0.2/src/base/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/messages.cc` & `cytosim-0.0.2/src/base/messages.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/messages.h` & `cytosim-0.0.2/src/base/messages.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/node_list.cc` & `cytosim-0.0.2/src/base/node_list.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/node_list.h` & `cytosim-0.0.2/src/base/node_list.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/noder.h` & `cytosim-0.0.2/src/base/noder.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/operator_new.cc` & `cytosim-0.0.2/src/base/operator_new.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/print_color.cc` & `cytosim-0.0.2/src/base/print_color.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/print_color.h` & `cytosim-0.0.2/src/base/print_color.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/property.cc` & `cytosim-0.0.2/src/base/property.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/property.h` & `cytosim-0.0.2/src/base/property.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/property_list.cc` & `cytosim-0.0.2/src/base/property_list.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/property_list.h` & `cytosim-0.0.2/src/base/property_list.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/stream_func.cc` & `cytosim-0.0.2/src/base/stream_func.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/stream_func.h` & `cytosim-0.0.2/src/base/stream_func.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/tictoc.cc` & `cytosim-0.0.2/src/base/tictoc.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/tictoc.h` & `cytosim-0.0.2/src/base/tictoc.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/timer.h` & `cytosim-0.0.2/src/base/timer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/tokenizer.cc` & `cytosim-0.0.2/src/base/tokenizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/base/tokenizer.h` & `cytosim-0.0.2/src/base/tokenizer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/cpython/couple_modules.h` & `cytosim-0.0.2/src/cpython/couple_modules.h`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,22 @@
         return static_cast<Couple*>(obj);
     return nullptr;
 }
 
 /// a utility to enrich the cytosim python module
 void load_couple_classes(py::module_ &m) {
      /// Python interface to couple
-    py::class_<Couple,Object>(m, "Couple")
+	py::class_<HandMonitor>(m, "HandMonitor")
+		.def("allowAttachment", &HandMonitor::allowAttachment)
+		.def("afterAttachment", &HandMonitor::afterAttachment)
+		.def("beforeDetachment", &HandMonitor::beforeDetachment)
+		.def("linkRestingLength", &HandMonitor::linkRestingLength)
+		.def("linkStiffness", &HandMonitor::linkStiffness);
+
+    py::class_<Couple,Object,HandMonitor>(m, "Couple")
         .def("position",  [](Couple * s) {return to_numpy(s->position());})
         .def("active",  [](Couple * s) {return s->active();})
         .def("stiffness",  [](Couple * s) {return s->stiffness();})
         .def("force",  [](Couple * s) {return to_numpy(s->force());})
         .def("cosAngle",  [](Couple * s) {return s->cosAngle();})
         .def("sidePos",  [](Couple * s) {return to_numpy(s->sidePos());})
         .def("posFree",  [](Couple * s) {return to_numpy(s->posFree());})
```

### Comparing `cytosim-0.0.1/src/cpython/fiber_modules.h` & `cytosim-0.0.2/src/cpython/fiber_modules.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 #include "fiber.h"
+#include "classic_fiber_prop.h"
+#include "dynamic_fiber_prop.h"
 #include "classic_fiber.h"
+#include "dynamic_fiber.h"
+#include "growing_fiber_prop.h"
+#include "treadmilling_fiber_prop.h"
+#include "growing_fiber.h"
+#include "treadmilling_fiber.h"
+
 #include <pybind11/pybind11.h>
 #include "python_utilities.h"
 //#include <pybind11/numpy.h>
 //#include <pybind11/stl.h>
 namespace py = pybind11;
 
 class Fiber;
@@ -92,20 +100,25 @@
         .def("dragCoefficient",  [](Mecafil * mec) {return mec->dragCoefficient();})
         .def("leftoverMobility",  [](Mecafil * mec) {return mec->leftoverMobility();});
     
     py::class_<Fiber,Mecafil>(m, "Fiber")
         .def("points",  [](Fiber * fib) {return get_obj_points(fib);})
         .def("toFiber",  [](Object * obj) {return Fiber::toFiber(obj);},  py::return_value_policy::reference)
         .def("nbPoints",  [](Fiber * fib) {return fib->nbPoints();})
+		.def("setDragCoefficient", &Fiber::setDragCoefficient)
+		.def("flipHandsPolarity", &Fiber::flipHandsPolarity)
         .def("cutM",  [](Fiber * fib, real len) {return fib->cutM(len);})
         .def("cutP",  [](Fiber * fib, real len) {return fib->cutP(len);})
         .def("sever",  [](Fiber * fib, real a, int p, int m) {return fib->sever(a, p, m);})
         .def("severNow",  &Fiber::severNow)
         .def("severM",  &Fiber::severM)
         .def("join",  [](Fiber * fib, Fiber * fob) {return fib->join(fob);})
+		.def("step", &Fiber::step)
+		.def("updateFiber", &Fiber::updateFiber)
+		.def("bendingEnergy", &Fiber::bendingEnergy)
         .def("stateM",  [](const Fiber * fib) {return py::cast(fib->dynamicStateM());})
         .def("stateP",  [](const Fiber * fib) {return py::cast(fib->dynamicStateP());})
         .def("setStateM",  [](Fiber * fib, int stat) {return fib->setDynamicStateM(stat);})
         .def("setStateP",  [](Fiber * fib, int stat) {return fib->setDynamicStateP(stat);})
         .def("setDynamicState",  [](Fiber * fib, int end, int stat) {return fib->setDynamicState(static_cast<FiberEnd>(end),stat);})
         .def("freshAssembly",  [](Fiber * fib, int end) {return fib->freshAssembly(static_cast<FiberEnd>(end));})
 		.def("nbHands",  [](Fiber * fib) {return fib->nbHands();})
@@ -115,28 +128,15 @@
 		.def("detachHands",  &Fiber::detachHands) 
 		.def("sortHands",  &Fiber::sortHands) 
 		.def("firstHand",  &Fiber::firstHand, py::return_value_policy::reference) 
         .def("nbHandsInRange",  [](Fiber * fib, real amin, real amax, int end) {return fib->nbHandsInRange(amin, amax, static_cast<FiberEnd>(end));})
 		.def("nbHandsNearEnd",  [](Fiber * fib, real len, int end) {return fib->nbHandsNearEnd(len, static_cast<FiberEnd>(end));})
         .def("__next__", [](const Fiber * fib) {return fib->next();});
         
-        
-    py::class_<ClassicFiber,Fiber>(m, "ClassicFiber")
-        .def("freshAssemblyM",  [](ClassicFiber * fib) {return fib->freshAssemblyM();})
-        .def("freshAssemblyP",  [](ClassicFiber * fib) {return fib->freshAssemblyP();});
-        /**
-         * 
-            @TODO : complete with fiber base functions
-         * 
-        */
-         
-         /**
-            @TODO : ADD SPECIALIZED FIBER CLASSES
-         */
-         
+ 
     /// Python interface to FiberProp
     py::class_<FiberProp,Property>(m, "FiberProp")
         .def_readwrite("segmentation", &FiberProp::segmentation)
         .def_readwrite("rigidity", &FiberProp::rigidity)
         .def_readwrite("min_length", &FiberProp::min_length)
         .def_readwrite("max_length", &FiberProp::max_length)
         .def_readwrite("total_polymer", &FiberProp::total_polymer)
@@ -175,9 +175,49 @@
             .value("STATE_GREEN", STATE_GREEN)
             .value("STATE_YELLOW", STATE_YELLOW)
             .value("STATE_ORANGE", STATE_ORANGE)
             .value("STATE_RED", STATE_RED)
             .value("STATE_BLACK", STATE_BLACK)
             .export_values();
         
+		       
+    py::class_<ClassicFiber,Fiber>(m, "ClassicFiber")
+        .def("freshAssemblyM",  [](ClassicFiber * fib) {return fib->freshAssemblyM();})
+        .def("freshAssemblyP",  [](ClassicFiber * fib) {return fib->freshAssemblyP();});
+		
+	py::class_<DynamicFiber,Fiber>(m, "DynamicFiber")
+		.def("freshAssemblyM",  [](DynamicFiber * fib) {return fib->freshAssemblyM();})
+        .def("freshAssemblyP",  [](DynamicFiber * fib) {return fib->freshAssemblyP();});
+
+    py::class_<ClassicFiberProp,FiberProp>(m, "ClassicFiberProp")
+		.def("growing_speed",  [](ClassicFiberProp * prop) {return to_numpy_raw(prop->growing_speed, 1, 2); })
+		.def("growing_off_speed",  [](ClassicFiberProp * prop) {return to_numpy_raw(prop->growing_off_speed, 1, 2);})
+		.def("growing_force",  [](ClassicFiberProp * prop) {return to_numpy_raw(prop->growing_force, 1, 2);})
+		.def("shrinking_speed",  [](ClassicFiberProp * prop) {return to_numpy_raw(prop->shrinking_speed, 1, 2);})
+		.def("catastrophe_rate",  [](ClassicFiberProp * prop) {return to_numpy_raw(prop->catastrophe_rate, 1, 2);})
+		.def("catastrophe_rate_stalled",  [](ClassicFiberProp * prop) {return to_numpy_raw(prop->catastrophe_rate_stalled, 1, 2);});
+	
+	py::class_<DynamicFiberProp,FiberProp>(m, "DynamicFiberProp")
+		.def("growing_speed",  [](DynamicFiberProp * prop) {return to_numpy_raw(prop->growing_speed, 1, 2); })
+		.def("growing_off_speed",  [](DynamicFiberProp * prop) {return to_numpy_raw(prop->growing_off_speed, 1, 2);})
+		.def("growing_force",  [](DynamicFiberProp * prop) {return to_numpy_raw(prop->growing_force, 1, 2);})
+		.def("shrinking_speed",  [](DynamicFiberProp * prop) {return to_numpy_raw(prop->shrinking_speed, 1, 2);});
+	
+	py::class_<GrowingFiber,Fiber>(m, "GrowingFiber");
+	py::class_<GrowingFiberProp,FiberProp>(m, "GrowingFiberProp");
+	
+	py::class_<TreadmillingFiber,Fiber>(m, "TreadmillingFiber");
+	py::class_<TreadmillingFiberProp,FiberProp>(m, "TreadmillingFiberProp");
+	
+	
+        /**
+         * 
+            @TODO : complete with fiber base functions
+         * 
+        */
+         
+         /**
+            @TODO : ADD SPECIALIZED FIBER CLASSES
+         */
+         
 }
```

### Comparing `cytosim-0.0.1/src/cpython/glossary_modules.h` & `cytosim-0.0.2/src/cpython/glossary_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/cpython/hand_modules.h` & `cytosim-0.0.2/src/cpython/hand_modules.h`

 * *Files 3% similar despite different names*

```diff
@@ -36,18 +36,19 @@
         .def("abscissaFromP",  [](FiberSite * h) {return h->abscissaFromP();})
         .def("abscissaFrom",  [](FiberSite * h, int end) {return h->abscissaFrom(static_cast<FiberEnd>(end));})
         .def("nearestEnd",  [](FiberSite * h) {return static_cast<int>(h->nearestEnd());})
         .def("distanceToEnd",  [](FiberSite * h, int end) {return h->distanceToEnd(static_cast<FiberEnd>(end));});
     
         
     py::class_<Hand,FiberSite>(m, "Hand")
+		.def("monitor", [](Hand * h) {return  h->monitor();}, py::return_value_policy::reference)
 		.def("next",  [](Hand * h) {return  h->next();}, py::return_value_policy::reference)
 		.def("prev",  [](Hand * h) {return h->prev();}, py::return_value_policy::reference)
         .def("property",  [](Hand * h) {return h->property();})
-        .def("prop",  [](Hand * h) {return h->prop;})
+        .def("prop",  [](Hand * h) {return h->prop;}, py::return_value_policy::reference)
         .def("relocate",  [](Hand * h, Fiber * fib) {return h->relocate(fib);})
         .def("relocateTo",  [](Hand * h, Fiber * fib, real a) {return h->relocate(fib,a);})
         .def("moveToEnd",  [](Hand * h, int end) {return h->moveToEnd(static_cast<FiberEnd>(end));})
         .def("locate",  [](Hand * h, Fiber * fib, real a) {return h->locate(fib,a);})
         .def("attach",  [](Hand * h, Fiber * fib, real a,  int end) {return h->attach(fib, a, static_cast<FiberEnd>(end));})
         .def("detach",  [](Hand * h) {return h->detach();})
         .def("attachEnd",  [](Hand * h, Fiber * fib, int end) {return h->attachEnd(fib, static_cast<FiberEnd>(end));})
```

### Comparing `cytosim-0.0.1/src/cpython/meca_modules.h` & `cytosim-0.0.2/src/cpython/meca_modules.h`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 
 /// a utility to enrich the cytosim python module
 void load_meca_classes(py::module_ &m) {
     py::class_<Meca>(m, "Meca")
         .def("nb_points", &Meca::nb_points)
         .def("dimension", &Meca::dimension)
         .def("prepare", &Meca::prepare)
+        .def("apply", &Meca::apply)
+        .def("solve", &Meca::solve)
+        .def("computeForces", &Meca::computeForces)
+        .def("base", [](Meca & mec) { return to_numpy_raw(mec.base(), mec.nb_points(), (int) DIM ); } )
+        .def("points", [](Meca & mec) { return to_numpy_raw(mec.points(), mec.nb_points(), (int) DIM ); } )
+        .def("force", [](Meca & mec) { return to_numpy_raw(mec.force(), mec.nb_points(), (int) DIM ); } )
         .def("addForcePt", [](Meca & mec, const Mecapoint & pt, pyarray force) {mec.addForce(pt,to_vector(force));})
         .def("addForce", [](Meca & mec, const Interpolation & pt, pyarray force) {mec.addForce(pt,to_vector(force));})
         .def("addTorque", [](Meca & mec, const Interpolation & pt, pyarray torque) {mec.addTorque(pt,to_torque(torque));})
         .def("addTorqueClamp", [](Meca & mec, const Interpolation & pt, pyarray dir, real w) {mec.addTorqueClamp(pt,to_vector(dir),w);})
         .def("addTorqueParrallel", [](Meca & mec, const Interpolation & pt1, const Interpolation & pt2, real w) {mec.addTorque(pt1,pt2,w);})
         .def("addTorqueAngle", [](Meca & mec, const Interpolation & pt1, const Interpolation & pt2, real cosi, real sinu, real w) 
             {mec.addTorque(pt1,pt2,cosi,sinu,w);})
```

### Comparing `cytosim-0.0.1/src/cpython/object_modules.h` & `cytosim-0.0.2/src/cpython/object_modules.h`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 /// a utility to enrich the cytosim python module
 void load_object_classes(py::module_ &m) {
     m.def("toVector", &to_vector, "@PYD;C:PyCytosim;T:converts numpy array to vector");
     m.def("toTorque", &to_torque, "@PYD;C:PyCytosim;T:converts numpy array to torque");
     
 	py::class_<ObjectSet>(m, "ObjectSet")
-		.def("add",  [](ObjectSet * set, Object * obj) {return set->add(obj) ;},"C:ObjectSet")
+		.def("add",  [](ObjectSet * set, Object * obj) {return set->add(obj) ;},"@PYD;C:ObjectSet")
 		.def("remove",  [](ObjectSet * set, Object * obj) {return set->remove(obj) ;})
 		.def("link",  [](ObjectSet * set, Object * obj) {return set->link(obj) ;})
 		.def("unlink",  [](ObjectSet * set, Object * obj) {return set->unlink(obj) ;})
 		.def("erase",  [](ObjectSet * set, Object * obj) {return set->erase(obj) ;})
 		.def("erase_all",  [](ObjectSet * set) {return set->erase() ;})
 		.def("size",  [](ObjectSet * set) {return set->size() ;})
 		.def("__len__",  [](ObjectSet * set) {return set->size() ;})
@@ -40,25 +40,25 @@
 				}
 				return obj;
              }, py::return_value_policy::reference);
      
      /// Python interface to Organizer
     py::class_<Object>(m, "Object")
         .def("reference",  [](Object * obj) {return obj->reference() ;})
-        .def("property",  [](Object * obj) {return obj->property() ;})
+        .def("property",  [](Object * obj) {return obj->property() ;}, py::return_value_policy::reference)
         .def("position", [](const Object * obj) {return to_numpy(obj->position());})
         .def("next",  [](Object * obj) {return obj->next() ;}, py::return_value_policy::reference)
 		.def("__next__",  [](Object * obj) {return obj->next() ;}, py::return_value_policy::reference)
         .def("prev",  [](Object * obj) {return obj->prev() ;}, py::return_value_policy::reference)
         .def("id",  [](const Object * obj) {return obj->identity();})
         .def("tag",  &Object::tag)
         .def("points", [](const Object * obj) {return pyarray();});
     
     /// Python interface to ObjectList
-    py::class_<ObjectList>(m, "ObjectList")
+    py::class_<ObjectList>(m, "ObjectList", "A list-like structure of Cytosim objects")
         .def("__getitem__",[](ObjectList & lis, int i) {
 				int s = lis.size();
                 if (i<0) {i+=s;} // Python time negative indexing
 				if (i >= s or i<0) {
 					 throw py::index_error();
 				}
 				Object * obj = lis[i];
```

### Comparing `cytosim-0.0.1/src/cpython/organizer_modules.h` & `cytosim-0.0.2/src/cpython/organizer_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/cpython/point_modules.h` & `cytosim-0.0.2/src/cpython/point_modules.h`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 namespace py = pybind11;
 
 class Interpolation;
 
 /// a utility to enrich the cytosim python module
 void load_point_classes(py::module_ &m) {
     py::class_<Mecapoint>(m, "Mecapoint")
+        .def("Mecapoint",  [](Mecable * mec, int pt) {unsigned pti = pt; return Mecapoint(mec, pti);},  py::return_value_policy::reference)
         .def("set", &Mecapoint::set)
         .def("mecable", &Mecapoint::mecable, py::return_value_policy::reference)
         .def("valid", &Mecapoint::valid)
         .def("position", [](const Mecapoint * pol) {return to_numpy(pol->pos());})
         .def("pos", [](const Mecapoint * pol) {return to_numpy(pol->pos());})
         .def("overlapping", &Mecapoint::overlapping)
         .def("near", &Mecapoint::near);
```

### Comparing `cytosim-0.0.1/src/cpython/python_frame.h` & `cytosim-0.0.2/src/cpython/python_frame.h`

 * *Files 25% similar despite different names*

```diff
@@ -19,14 +19,107 @@
 #include "python_utilities.h"
 namespace py = pybind11;
 
 class Simul;
 class SimulProp;
 class Organizer;
 
+void void_callback(void) {};
+
+
+class PythonParser : public Parser
+{
+public:
+        
+    /// construct a Parser with given permissions
+    PythonParser(Simul& simul) :Parser(simul,  0, 1, 0, 0, 0) {
+        // Has not been loaded yet
+        is_loaded = 0;
+        // Has not been saved yet
+        is_saved = 0;
+        // Creating a SimThread, maybe
+        sim = &simul;
+    }
+
+    /// activates the parser (from existing sim)
+    void activate(std::string & input, SimThread * existing_thread) {
+        thread = existing_thread;
+        //thread->start();
+        reader.openFile(input);
+        is_loaded = 1;
+    }
+
+    /// activates the parser (from existing sim)
+    void activate(std::string & input) {
+        thread = new SimThread(*sim, &void_callback);
+        //thread->start();
+        reader.openFile(input);
+        is_loaded = 1;
+    }
+    
+    /// activates the parser (new sim)
+    void activate(SimThread * existing_thread) {
+        Parser::readConfig();
+        thread = existing_thread;
+        thread->start();
+        is_loaded = 2;
+    }
+    
+    /// activates the parser (new sim)
+    void activate() {
+        Parser::readConfig();
+        thread = new SimThread(*sim, &void_callback);
+        thread->start();
+        is_loaded = 2;
+    }
+    
+    /// A framereader
+    FrameReader reader;
+    
+    /// Check if simulation is loaded
+    int is_loaded ;
+    
+    /// A thread
+    SimThread * thread;
+    
+    /// Has the simulation been saved 
+    bool is_saved ;
+    
+    /// is the simulation
+    Simul * sim;
+    
+    /// Loads the simulation at a given time
+    int load(int fr) {
+        int loader = 1;
+        if (is_loaded == 1) {
+            try 
+            {
+                //loader = thread->loadFrame(fr);
+                loader = reader.loadFrame(*sim,fr);
+                if (loader!=0) {
+                    std::clog << "Unable to load frame " << fr << ". Maybe frame does not exist." << std::endl;
+                } 
+                    
+            }
+            catch( Exception & e )
+            {
+                std::clog << "Aborted: " << e.what() << '\n';
+            }
+        }
+        else{
+            std::clog << "Simulation not loaded : use cytosim.open() first" << std::endl;
+        }
+        
+        return loader;
+    }
+    
+    int next() {
+        return reader.loadNextFrame(*sim);
+    }
+};
 
 /// ObjGroup : a vector of objects of same type having the same property
 template<typename Obj, typename Prp> 
 class ObjGroup : public std::vector<Obj*>{
     public:
     Prp * prop;
     ObjGroup() = default;
@@ -34,47 +127,18 @@
     ~ObjGroup() = default;
 };
 
 /// ObjMap : a map <string, ObjGroup>
 template<typename Obj, typename Prp> 
 using ObjMap = std::map<std::string,ObjGroup<Obj,Prp>> ;
 
-/// A time frame ; basically a wrapper around a object dictionnary
-class Frame 
-{
-public:
-        /// An Objectmap is map of  (string,objectgroup)
-        ObjMap<Fiber,FiberProp> fibers;
-        ObjMap<Solid,SolidProp> solids;
-        ObjMap<Bead,BeadProp> beads;
-        ObjMap<Sphere,SphereProp> spheres;
-        ObjMap<Organizer,Property> organs;
-        ObjMap<Space,SpaceProp> spaces;
-        ObjMap<Couple,CoupleProp> couples;
-        ObjMap<Single,SingleProp> singles;
-
-        // Time of the frame
-        real time;
-        int index;
-        int loaded;
-        
-        /// pointer to simul
-        Simul * simul;
-        
-        /// The party zone
-        py::dict objects;
-        
-        /// Default constr and destrc
-        Frame() = default;
-        ~Frame() = default;
-};
 
 /// Distribute the objects (pointers) in the groups and in the dict.
 template<typename Obj, typename Prp, typename Set> 
-void distribute_objects(Simul * sim, Frame * current, ObjMap<Obj,Prp> mappe, Set & set, std::string categ ) {
+void distribute_objects(Simul * sim, py::dict & objects, ObjMap<Obj,Prp> mappe, Set & set, std::string categ ) {
     // First we list all objects in category, and create the ObjGroups in the map
     PropertyList plist = sim->properties.find_all(categ);
     if (!plist.empty()) {
         for ( Property * i : plist )
             {
                 Prp * fp = static_cast<Prp*>(i);
                 mappe[fp->name()] = ObjGroup<Obj,Prp>(fp);
@@ -83,24 +147,24 @@
         Obj * obj = set.first();
         while (obj) {
             mappe[obj->property()->name()].push_back(obj);
             obj = obj->next();
         }
         // Then we fill the dictionnary
         for (const auto &[name, group] : mappe) {
-            current->objects[py::cast(name)] = group;
+            objects[py::cast(name)] = group;
         }
         
     }
 }
  
 /// Distribute the objects (pointers) in the groups and in the dict ; 
 // special case for couple, single, where firstID needs to be used
 template<typename Obj, typename Prp, typename Set> 
-void distribute_objects_wID(Simul * sim, Frame * current, ObjMap<Obj,Prp> mappe, Set & set, std::string categ )
+void distribute_objects_wID(Simul * sim, py::dict & objects, ObjMap<Obj,Prp> mappe, Set & set, std::string categ )
 {
     // First we list all objects in category, and create the ObjGroups in the map
     PropertyList plist = sim->properties.find_all(categ);
     if (!plist.empty()) {
         for ( Property * i : plist )
             {
                 Prp * fp = static_cast<Prp*>(i);
@@ -115,24 +179,24 @@
         while (obj) 
        {
             mappe[obj->property()->name()].push_back(obj);
             obj = set.nextID(obj);
         }
         // Then we fill the dictionnary
         for (const auto &[name, group] : mappe) {
-            current->objects[py::cast(name)] = group;
+            objects[py::cast(name)] = group;
         }
         
     }
 }
 
 /// declare_group() : creates a python interface for an ObjGroup
 template<typename Group>
-auto declare_group(py::module &mod, Group group, std::string name) {
-        return py::class_<Group>(mod, name.c_str())
+auto declare_group(py::module &mod, Group group, std::string name) { 
+        return py::class_<Group>(mod, name.c_str(),  "Behaves as a list of objects with the same properties")
             .def("__len__", [](const Group &v) { return v.size(); })
             .def("size", &Group::size)
             .def_readwrite("prop",   &Group::prop , py::return_value_policy::reference)
             .def("__iter__", [](Group &v) {
                 return py::make_iterator(v.begin(), v.end());
             }, py::keep_alive<0, 1>())
             .def("__getitem__",[](const Group &v, size_t i) {
@@ -141,45 +205,83 @@
 				if (i >= s or i<0) {
                          throw py::index_error();
                      }
                      return v[i];
                  }, py::return_value_policy::reference);
 }
 
-/// Prepares a given frame by sorting objects into object groups
-Frame * make_frame( Simul * sim) 
-{   
-    std::vector<std::string> categories = std::vector<std::string>{"aster","nucleus","bundle","fake"};
-    //extern std::vector<std::string>  categories;
-    Frame * current = new Frame;
-    current->simul = sim;
-    
-    distribute_objects(sim,current, current->fibers, sim->fibers, std::string("fiber") ) ;
-    distribute_objects(sim,current, current->solids, sim->solids, std::string("solid") ) ;
-    distribute_objects(sim,current, current->spaces, sim->spaces, std::string("space") ) ;
-    distribute_objects(sim,current, current->beads, sim->beads, std::string("bead") ) ;
-    distribute_objects(sim,current, current->spheres, sim->spheres, std::string("sphere") ) ;
-    // For organizer, the we have to check the different categories
-    for (auto categ : categories) {
-        distribute_objects(sim,current, current->organs, sim->organizers, std::string(categ) ) ;
-    }
-    // for couple and single we need to use firstID, nextID
-    distribute_objects_wID(sim,current, current->couples, sim->couples, std::string("couple") ) ;
-    distribute_objects_wID(sim,current, current->singles, sim->singles, std::string("single") ) ;
-    
-    current->time = sim->time();
-    //current->index = frame;
-    current->loaded = 1;
 
-    return current;
-    
-}
+/// A time frame ; basically a wrapper around a object dictionnary
+// This would need to be better done
+class Frame 
+{
+public:
+        /// An Objectmap is map of  (string,objectgroup)
+        ObjMap<Fiber,FiberProp> fibers;
+        ObjMap<Solid,SolidProp> solids;
+        ObjMap<Bead,BeadProp> beads;
+        ObjMap<Sphere,SphereProp> spheres;
+        ObjMap<Organizer,Property> organs;
+        ObjMap<Space,SpaceProp> spaces;
+        ObjMap<Couple,CoupleProp> couples;
+        ObjMap<Single,SingleProp> singles;
+
+        // Time of the frame
+        real time;
+        int index;
+        int loaded;
+        
+        /// pointer to simul
+        Simul * simul;
+        
+        /// pointer to parser
+        //PythonParser * parser;
+        
+        /// The party zone
+        py::dict objects;
+        
+        /// Default constr and destrc
+        Frame(PythonParser & pyParse) {
+            //parser = &pyParse;
+            simul = pyParse.sim;
+            update();
+        }
+        
+        /// Default constr and destrc
+        Frame(Simul * sim) {
+            simul = sim;
+            update();
+        }
+        
+        
+        void load(int t) {
+            
+        }
+        void update() {
+            std::vector<std::string> categories = std::vector<std::string>{"aster","nucleus","bundle","fake"};
+            //extern std::vector<std::string>  categories;
+            
+            distribute_objects(simul,objects, fibers, simul->fibers, std::string("fiber") ) ;
+            distribute_objects(simul,objects, solids, simul->solids, std::string("solid") ) ;
+            distribute_objects(simul,objects, spaces, simul->spaces, std::string("space") ) ;
+            distribute_objects(simul,objects, beads, simul->beads, std::string("bead") ) ;
+            distribute_objects(simul,objects, spheres, simul->spheres, std::string("sphere") ) ;
+            // For organizer, the we have to check the different categories
+            for (auto categ : categories) {
+                distribute_objects(simul,objects, organs, simul->organizers, std::string(categ) ) ;
+            }
+            // for couple and single we need to use firstID, nextID
+            distribute_objects_wID(simul,objects, couples, simul->couples, std::string("couple") ) ;
+            distribute_objects_wID(simul,objects, singles, simul->singles, std::string("single") ) ;
+            
+            time = simul->time();
+            //current->index = frame;
+            loaded = 1;
+        };
+        
+        Frame() = default;
+        ~Frame() = default;
+};
 
-/// Prepares a given frame and attibutes an index
-Frame * make_frame_index( Simul * sim, int i)  {
-	Frame * current = make_frame(sim);
-	current->index = i;
-	return current;
-}
 
 
 #endif
```

### Comparing `cytosim-0.0.1/src/cpython/python_utilities.h` & `cytosim-0.0.2/src/cpython/python_utilities.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,53 @@
 #ifndef UTILITIES_H
 #define UTILITIES_H
-//#include "fiber.h"
 #include <pybind11/pybind11.h>
 #include "glossary.h"
-//#include <pybind11/numpy.h>
-//#include <pybind11/stl.h>
-//#include "object_info.h"
+
 class Glossary;
 
 /// A vector of ints
 typedef std::vector<int> int_vect;
 /// contains adress, sizes, and strides
 namespace py = pybind11;
 typedef py::array_t<real> pyarray;
 
-struct realArray {
-    void * ptr;
-    int_vect sizes;
-    int_vect strides;
-};
+/// An empty capsule to create numpy array from raw pointers
+auto cleanup_callback = []() {} ;
+py::capsule no_delete(cleanup_callback);
+
+/// Get a numpy array from a pointer to real array (raw data)
+pyarray & to_numpy_raw(real * pointer, int nb_pts, int dim ) {
+    int_vect sizes = {nb_pts, dim};
+    int_vect strides = { static_cast<int>(dim*sizeof(real)),  static_cast<int>(sizeof(real)) };
+    pyarray * arr =  new pyarray(sizes, strides, pointer, no_delete);
+    return * arr;
+}
+
+/// Get a numpy array from a pointer to real array (copy)
+pyarray & to_numpy(const real * pointer, int nb_pts, int dim )  {
+    int_vect sizes = {nb_pts, dim};
+    int_vect strides = { static_cast<int>(dim*sizeof(real)),  static_cast<int>(sizeof(real)) };
+    pyarray * arr =new pyarray(sizes, strides, pointer);
+    return *arr;
+}
 
 /// Get points for cytosim objects such as fibers or solids
 template<typename Obj>
 pyarray & get_obj_points(Obj * obj) {
-    int_vect sizes = {(int)obj->nbPoints(), (int)DIM};
-    int_vect strides = {DIM*sizeof(real), sizeof(real)};
-    pyarray * arr =new pyarray(sizes, strides, obj->data());
-    return *arr;
+    return to_numpy( obj->data(), obj->nbPoints(), DIM);
 };
 
-/// Get real points for cytosim mecables
-realArray * get_pointsarray(Mecable * obj) {
-    int_vect sizes = {(int)obj->nbPoints(), (int)DIM};
-    int_vect strides = {DIM*sizeof(real), sizeof(real)};
-    realArray * arr =new realArray{obj->nonConstData(), sizes, strides};
-    return arr;
+/// Get raw data for cytosim mecables
+pyarray & get_obj_data(Mecable * obj) {
+    return to_numpy_raw( obj->nonConstData(), obj->nbPoints(), DIM);
 };
 
 
-/// Converts a real array * to numpy array
-/*
-pyarray & to_numpy(real_array * rar) {
-    if (rar) {
-        pyarray * arr =new pyarray(std::get<1>(*rar),std::get<2>(*rar), std::get<0>(*rar));
-        return *arr;
-    } else {
-        pyarray * arr = new pyarray();
-        return *arr;
-    }
-}
-
-/// Converts a real array to numpy array
-pyarray & to_numpy(real_array  rar) {
-    pyarray * arr =new pyarray(std::get<1>(rar),std::get<2>(rar), std::get<0>(rar));
-    return *arr;
-}
-*/
-
-/// Converts a Vector to numpy array
+/// Converts a Vector to numpy array (copy)
 pyarray & to_numpy(Vector vec) {    
     pyarray * par = new pyarray;
 #if DIM==1
     *par = py::cast(std::vector<real>{vec[0]});
 #elif DIM==2
     *par = py::cast(std::vector<real>{vec[0],vec[1]});
 #else
@@ -117,28 +103,14 @@
     py::dict * dico = new py::dict;
     for (const auto &[name, rec] : mappe) {
             (*dico)[py::str(name)] = py::cast(rec);
         }
     return *dico;
 }
 
-
 /// Converts a string to a glossary
 Glossary & str_to_glos(std::string str) {
     Glossary * glos = new Glossary(str);
     return *glos;
 }
 
-/// Converts an ObjectInfo * to a python dict
-/*
-py::dict & to_dict(ObjectInfo * info) {
-    py::dict * dico = new py::dict;
-    dico->attr("update")(py::cast(info->reals));
-    dico->attr("update")(py::cast(info->strings));
-    dico->attr("update")(py::cast(info->ints));
-    dico->attr("update")(py::cast(info->vecs));
-    
-    return *dico;
-}
-*/
-
-#endif
+#endif
```

### Comparing `cytosim-0.0.1/src/cpython/single_modules.h` & `cytosim-0.0.2/src/cpython/single_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/cpython/solid_modules.h` & `cytosim-0.0.2/src/cpython/solid_modules.h`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 class Solid;
 class Object;
 
 /// a utility to enrich the cytosim python module
 void load_solid_classes(py::module_ &m) {
     /// Python interface to Solid
     py::class_<Mecable,Object>(m, "Mecable")
-        .def("data",   [](Mecable * mec) {return get_pointsarray(mec);})
+        .def("data",   [](Mecable * mec) {return get_obj_data(mec);})
         .def("nbPoints", &Mecable::nbPoints)
         .def("allocated", &Mecable::allocated)
-        .def("points",  [](Mecable * mec) {return get_obj_points(mec);})
+        .def("points",  [](Mecable * mec) {return get_obj_points(mec);},
+                "@PYD;T: Returns read-only point coordinates of the mecable")
         .def("posPoint",  [](Mecable * mec,int p) {return to_numpy(mec->posPoint(p));})
         .def("setPoint",  [](Mecable * mec, int i, pyarray vec) 
             {   Vector p = to_vector(vec);
                 return mec->setPoint(i,p);})
         .def("setPoint",  [](Mecable * mec, int i, pyarray vec) 
             {   Vector p = to_vector(vec);
                 return mec->movePoint(i,p);})
```

### Comparing `cytosim-0.0.1/src/cpython/space_modules.h` & `cytosim-0.0.2/src/cpython/space_modules.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/CMakeLists.txt` & `cytosim-0.0.2/src/disp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/display.cc` & `cytosim-0.0.2/src/disp/display.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/display.h` & `cytosim-0.0.2/src/disp/display.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/display1.cc` & `cytosim-0.0.2/src/disp/display1.cc`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
             gleObject(obj.posP(0), obj.diffPoints(1, 0), obj.radius(0), gleCircleB);
 #endif
     }
     
     //print the number for each solid
     if ( disp->style & 8 )
     {
-        char tmp[8];
+        char tmp[32];
         bodyColor(disp, obj.signature());
         snprintf(tmp, sizeof(tmp), "%u", obj.identity());
         gleDrawText(obj.posP(0), tmp, GLUT_BITMAP_HELVETICA_10);
     }
     
     //draw polygon around vertices of Solid
     if ( disp->style & 16 )
```

### Comparing `cytosim-0.0.1/src/disp/display1.h` & `cytosim-0.0.2/src/disp/display1.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/display2.cc` & `cytosim-0.0.2/src/disp/display2.cc`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
             gleObject(obj.posP(0), obj.diffPoints(1, 0), obj.radius(0), gleCircleB);
 #endif
     }
     
     //print the number for each Solid
     if ( disp->style & 8 )
     {
-        char tmp[8];
+        char tmp[32];
         bodyColor2(disp, obj.signature());
         snprintf(tmp, sizeof(tmp), "%u", obj.identity());
         gleDrawText(obj.posP(0), tmp, GLUT_BITMAP_HELVETICA_10);
     }
     
     //draw polygon around vertices of Solid
     if ( disp->style & 16 )
```

### Comparing `cytosim-0.0.1/src/disp/display2.h` & `cytosim-0.0.2/src/disp/display2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/display3.cc` & `cytosim-0.0.2/src/disp/display3.cc`

 * *Files 0% similar despite different names*

```diff
@@ -758,15 +758,15 @@
         gleObject(obj.posP(0), obj.diffPoints(1, 0), obj.radius(0), gleCircleB);
     }
 #endif
     
     //display a signature for each Solid
     if ( disp->style & 8 )
     {
-        char tmp[8];
+        char tmp[32];
         bodyColor(disp, obj.signature());
         snprintf(tmp, sizeof(tmp), "%u", obj.identity());
         gleDrawText(obj.posP(0), tmp, GLUT_BITMAP_HELVETICA_10);
     }
     
     //draw polygon around vertices of Solid
     if ( disp->style & 16 )
```

### Comparing `cytosim-0.0.1/src/disp/display3.h` & `cytosim-0.0.2/src/disp/display3.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/display_prop.cc` & `cytosim-0.0.2/src/disp/display_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/display_prop.h` & `cytosim-0.0.2/src/disp/display_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/fiber_disp.cc` & `cytosim-0.0.2/src/disp/fiber_disp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/fiber_disp.h` & `cytosim-0.0.2/src/disp/fiber_disp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/glapp.cc` & `cytosim-0.0.2/src/disp/glapp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/glapp.h` & `cytosim-0.0.2/src/disp/glapp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/gle.cc` & `cytosim-0.0.2/src/disp/gle.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/gle.h` & `cytosim-0.0.2/src/disp/gle.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/gle_color.cc` & `cytosim-0.0.2/src/disp/gle_color.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/gle_color.h` & `cytosim-0.0.2/src/disp/gle_color.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/gle_color_list.cc` & `cytosim-0.0.2/src/disp/gle_color_list.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/gle_color_list.h` & `cytosim-0.0.2/src/disp/gle_color_list.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/glu_unproject.cc` & `cytosim-0.0.2/src/disp/glu_unproject.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/grid_display.cc` & `cytosim-0.0.2/src/disp/grid_display.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/grid_display.h` & `cytosim-0.0.2/src/disp/grid_display.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/line_disp.h` & `cytosim-0.0.2/src/disp/line_disp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/makefile.inc` & `cytosim-0.0.2/src/disp/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/miniz.c` & `cytosim-0.0.2/src/disp/miniz.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/miniz.h` & `cytosim-0.0.2/src/disp/miniz.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/offscreen.cc` & `cytosim-0.0.2/src/disp/offscreen.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/offscreen.h` & `cytosim-0.0.2/src/disp/offscreen.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/offscreen_fbo.cc` & `cytosim-0.0.2/src/disp/offscreen_fbo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/offscreen_glx.cc` & `cytosim-0.0.2/src/disp/offscreen_glx.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/point_disp.cc` & `cytosim-0.0.2/src/disp/point_disp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/point_disp.h` & `cytosim-0.0.2/src/disp/point_disp.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/save_image.cc` & `cytosim-0.0.2/src/disp/save_image.cc`

 * *Files 0% similar despite different names*

```diff
@@ -570,15 +570,15 @@
         
         free(rows);
     }
     
     return res;
 }
 
-#elif 1
+#elif 0
 
 //------------------------------------------------------------------------------
 #pragma mark - PNG export using libspng (https://libspng.org)
 
 #include "spng.h"
 
 int SaveImage::savePNG(FILE* file, const uint8_t pixels[],
```

### Comparing `cytosim-0.0.1/src/disp/save_image.h` & `cytosim-0.0.2/src/disp/save_image.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/spng.c` & `cytosim-0.0.2/src/disp/spng.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/spng.h` & `cytosim-0.0.2/src/disp/spng.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/view.cc` & `cytosim-0.0.2/src/disp/view.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/view.h` & `cytosim-0.0.2/src/disp/view.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/disp/view_prop.cc` & `cytosim-0.0.2/src/disp/view_prop.cc`

 * *Files 0% similar despite different names*

```diff
@@ -130,18 +130,18 @@
     {
         std::string var = "clip_plane" + std::to_string(k);
         glos.set(clip_plane_mode[k],   var);
         glos.set(clip_plane_vector[k], var, 1);
         glos.set(clip_plane_scalar[k], var, 2);
     }
     
-    Glossary::dict_type<GLint> keys({{"off",          0},
-                                     {"linear",       1},
-                                     {"exponential",  2},
-                                     {"exponential2", 3}});
+    Glossary::dict_type<GLint> keys{{"off",          0},
+                                    {"linear",       1},
+                                    {"exponential",  2},
+                                    {"exponential2", 3}};
 
     glos.set(fog_type,     "fog_type", keys);
     glos.set(fog_param,    "fog_param");
     glos.set(fog_color,    "fog_color");
  
     glos.set(fog_type,     "fog", keys);
     glos.set(fog_param,    "fog", 1);
```

### Comparing `cytosim-0.0.1/src/disp/view_prop.h` & `cytosim-0.0.2/src/disp/view_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/index.md` & `cytosim-0.0.2/src/index.md`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/CMakeLists.txt` & `cytosim-0.0.2/src/math/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/SFMT-avx2.h` & `cytosim-0.0.2/src/math/SFMT-avx2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/SFMT-common.h` & `cytosim-0.0.2/src/math/SFMT-common.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/SFMT-params.h` & `cytosim-0.0.2/src/math/SFMT-params.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/SFMT-params19937.h` & `cytosim-0.0.2/src/math/SFMT-params19937.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/SFMT-sse2.h` & `cytosim-0.0.2/src/math/SFMT-sse2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/SFMT.c` & `cytosim-0.0.2/src/math/SFMT.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/SFMT.h` & `cytosim-0.0.2/src/math/SFMT.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/accumulator.h` & `cytosim-0.0.2/src/math/accumulator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/allocator.h` & `cytosim-0.0.2/src/math/allocator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/bicgstab.h` & `cytosim-0.0.2/src/math/bicgstab.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/cblas.h` & `cytosim-0.0.2/src/math/cblas.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/clapack.h` & `cytosim-0.0.2/src/math/clapack.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/dgtsv.c` & `cytosim-0.0.2/src/math/dgtsv.c`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/evaluator.h` & `cytosim-0.0.2/src/math/evaluator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/gmres.h` & `cytosim-0.0.2/src/math/gmres.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/grid.h` & `cytosim-0.0.2/src/math/grid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/grid_base.h` & `cytosim-0.0.2/src/math/grid_base.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/isometry.h` & `cytosim-0.0.2/src/math/isometry.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/linear_operator.h` & `cytosim-0.0.2/src/math/linear_operator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/makefile.inc` & `cytosim-0.0.2/src/math/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matrix.cc` & `cytosim-0.0.2/src/math/matrix.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matrix.h` & `cytosim-0.0.2/src/math/matrix.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matrix11.cc` & `cytosim-0.0.2/src/math/matrix11.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matrix11.h` & `cytosim-0.0.2/src/math/matrix11.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matrix22.cc` & `cytosim-0.0.2/src/math/matrix22.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matrix22.h` & `cytosim-0.0.2/src/math/matrix22.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matrix33.cc` & `cytosim-0.0.2/src/math/matrix33.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matrix33.h` & `cytosim-0.0.2/src/math/matrix33.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matrix44.h` & `cytosim-0.0.2/src/math/matrix44.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matrixbase.h` & `cytosim-0.0.2/src/math/matrixbase.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matsparse.cc` & `cytosim-0.0.2/src/math/matsparse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matsparse.h` & `cytosim-0.0.2/src/math/matsparse.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matsparsesym.cc` & `cytosim-0.0.2/src/math/matsparsesym.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matsparsesym.h` & `cytosim-0.0.2/src/math/matsparsesym.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matsparsesym1.cc` & `cytosim-0.0.2/src/math/matsparsesym1.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matsparsesym1.h` & `cytosim-0.0.2/src/math/matsparsesym1.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matsparsesym2.cc` & `cytosim-0.0.2/src/math/matsparsesym2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matsparsesym2.h` & `cytosim-0.0.2/src/math/matsparsesym2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matsparsesymblk.cc` & `cytosim-0.0.2/src/math/matsparsesymblk.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/matsparsesymblk.h` & `cytosim-0.0.2/src/math/matsparsesymblk.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/monitor.h` & `cytosim-0.0.2/src/math/monitor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/platonic.cc` & `cytosim-0.0.2/src/math/platonic.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/platonic.h` & `cytosim-0.0.2/src/math/platonic.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/pointsonsphere.cc` & `cytosim-0.0.2/src/math/pointsonsphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/pointsonsphere.h` & `cytosim-0.0.2/src/math/pointsonsphere.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/polygon.cc` & `cytosim-0.0.2/src/math/polygon.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/polygon.h` & `cytosim-0.0.2/src/math/polygon.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/project_ellipse.cc` & `cytosim-0.0.2/src/math/project_ellipse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/project_ellipse.h` & `cytosim-0.0.2/src/math/project_ellipse.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/quaternion.h` & `cytosim-0.0.2/src/math/quaternion.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/random.cc` & `cytosim-0.0.2/src/math/random.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/random.h` & `cytosim-0.0.2/src/math/random.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/random_vector.cc` & `cytosim-0.0.2/src/math/random_vector.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/random_vector.h` & `cytosim-0.0.2/src/math/random_vector.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/rasterizer.cc` & `cytosim-0.0.2/src/math/rasterizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/rasterizer.h` & `cytosim-0.0.2/src/math/rasterizer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/real.h` & `cytosim-0.0.2/src/math/real.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/simd.h` & `cytosim-0.0.2/src/math/simd.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/simd_print.h` & `cytosim-0.0.2/src/math/simd_print.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/smath.h` & `cytosim-0.0.2/src/math/smath.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/vecprint.h` & `cytosim-0.0.2/src/math/vecprint.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/vector.h` & `cytosim-0.0.2/src/math/vector.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/vector1.cc` & `cytosim-0.0.2/src/math/vector1.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/vector1.h` & `cytosim-0.0.2/src/math/vector1.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/vector2.cc` & `cytosim-0.0.2/src/math/vector2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/vector2.h` & `cytosim-0.0.2/src/math/vector2.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/vector3.cc` & `cytosim-0.0.2/src/math/vector3.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/vector3.h` & `cytosim-0.0.2/src/math/vector3.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/vector4.cc` & `cytosim-0.0.2/src/math/vector4.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/math/vector4.h` & `cytosim-0.0.2/src/math/vector4.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/check_dump.m` & `cytosim-0.0.2/src/misc/check_dump.m`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/RtMidi.cpp` & `cytosim-0.0.2/src/misc/installation/RtMidi.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/RtMidi.h` & `cytosim-0.0.2/src/misc/installation/RtMidi.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/builder/0-live.command` & `cytosim-0.0.2/src/misc/installation/builder/0-live.command`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/builder/config.cym` & `cytosim-0.0.2/src/misc/installation/builder/config.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/builder/config0.cym` & `cytosim-0.0.2/src/misc/installation/builder/config0.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/builder/config1.cym` & `cytosim-0.0.2/src/misc/installation/builder/config1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/builder/config2.cym` & `cytosim-0.0.2/src/misc/installation/builder/config2.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/builder/config3.cym` & `cytosim-0.0.2/src/misc/installation/builder/config3.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/builder/config4.cym` & `cytosim-0.0.2/src/misc/installation/builder/config4.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/builder/config5.cym` & `cytosim-0.0.2/src/misc/installation/builder/config5.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/builder/config6.cym` & `cytosim-0.0.2/src/misc/installation/builder/config6.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/builder/config7.cym` & `cytosim-0.0.2/src/misc/installation/builder/config7.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/builder/config8.cym` & `cytosim-0.0.2/src/misc/installation/builder/config8.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/builder/france.txt` & `cytosim-0.0.2/src/misc/installation/builder/france.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/cytobuilder.cpp` & `cytosim-0.0.2/src/misc/installation/cytobuilder.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/cytomaster.cpp` & `cytosim-0.0.2/src/misc/installation/cytomaster.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/cytomaster.xcodeproj/project.pbxproj` & `cytosim-0.0.2/src/misc/installation/cytomaster.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/makefile` & `cytosim-0.0.2/src/misc/installation/makefile`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/master/0-live.command` & `cytosim-0.0.2/src/misc/installation/master/0-live.command`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/master/config0.cym` & `cytosim-0.0.2/src/misc/installation/master/config0.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/master/config1.cym` & `cytosim-0.0.2/src/misc/installation/master/config1.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/master/config2.cym` & `cytosim-0.0.2/src/misc/installation/master/config2.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/master/config4.cym` & `cytosim-0.0.2/src/misc/installation/master/config4.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/master/config6.cym` & `cytosim-0.0.2/src/misc/installation/master/config6.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/master/config7.cym` & `cytosim-0.0.2/src/misc/installation/master/config7.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/master/config8.cym` & `cytosim-0.0.2/src/misc/installation/master/config8.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/master/config9.cym` & `cytosim-0.0.2/src/misc/installation/master/config9.cym`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/master/france.txt` & `cytosim-0.0.2/src/misc/installation/master/france.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/rtmidi_c.cpp` & `cytosim-0.0.2/src/misc/installation/rtmidi_c.cpp`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/misc/installation/rtmidi_c.h` & `cytosim-0.0.2/src/misc/installation/rtmidi_c.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/play/CMakeLists.txt` & `cytosim-0.0.2/src/play/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/play/makefile.inc` & `cytosim-0.0.2/src/play/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/play/play.cc` & `cytosim-0.0.2/src/play/play.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/play/play_keys.cc` & `cytosim-0.0.2/src/play/play_keys.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/play/play_menus.cc` & `cytosim-0.0.2/src/play/play_menus.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/play/play_mouse.cc` & `cytosim-0.0.2/src/play/play_mouse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/play/player.cc` & `cytosim-0.0.2/src/play/player.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/play/player.h` & `cytosim-0.0.2/src/play/player.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/play/player_disp.cc` & `cytosim-0.0.2/src/play/player_disp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/play/player_prop.cc` & `cytosim-0.0.2/src/play/player_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/play/player_prop.h` & `cytosim-0.0.2/src/play/player_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/CMakeLists.txt` & `cytosim-0.0.2/src/sim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/bead.cc` & `cytosim-0.0.2/src/sim/bead.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/bead.h` & `cytosim-0.0.2/src/sim/bead.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/bead_set.cc` & `cytosim-0.0.2/src/sim/bead_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/bead_set.h` & `cytosim-0.0.2/src/sim/bead_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/chain.cc` & `cytosim-0.0.2/src/sim/chain.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/chain.h` & `cytosim-0.0.2/src/sim/chain.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/common.h` & `cytosim-0.0.2/src/sim/common.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couple.cc` & `cytosim-0.0.2/src/sim/couple.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couple.h` & `cytosim-0.0.2/src/sim/couple.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couple_prop.cc` & `cytosim-0.0.2/src/sim/couple_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couple_prop.h` & `cytosim-0.0.2/src/sim/couple_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couple_set.cc` & `cytosim-0.0.2/src/sim/couple_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couple_set.h` & `cytosim-0.0.2/src/sim/couple_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/bridge.cc` & `cytosim-0.0.2/src/sim/couples/bridge.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/bridge.h` & `cytosim-0.0.2/src/sim/couples/bridge.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/bridge_prop.cc` & `cytosim-0.0.2/src/sim/couples/bridge_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/bridge_prop.h` & `cytosim-0.0.2/src/sim/couples/bridge_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/couple_long.cc` & `cytosim-0.0.2/src/sim/couples/couple_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/couple_long.h` & `cytosim-0.0.2/src/sim/couples/couple_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/crosslink.cc` & `cytosim-0.0.2/src/sim/couples/crosslink.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/crosslink.h` & `cytosim-0.0.2/src/sim/couples/crosslink.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/crosslink_long.cc` & `cytosim-0.0.2/src/sim/couples/crosslink_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/crosslink_long.h` & `cytosim-0.0.2/src/sim/couples/crosslink_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/crosslink_prop.cc` & `cytosim-0.0.2/src/sim/couples/crosslink_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/crosslink_prop.h` & `cytosim-0.0.2/src/sim/couples/crosslink_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/duo.cc` & `cytosim-0.0.2/src/sim/couples/duo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/duo.h` & `cytosim-0.0.2/src/sim/couples/duo.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/duo_long.cc` & `cytosim-0.0.2/src/sim/couples/duo_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/duo_long.h` & `cytosim-0.0.2/src/sim/couples/duo_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/duo_prop.cc` & `cytosim-0.0.2/src/sim/couples/duo_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/duo_prop.h` & `cytosim-0.0.2/src/sim/couples/duo_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/fork.cc` & `cytosim-0.0.2/src/sim/couples/fork.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/fork.h` & `cytosim-0.0.2/src/sim/couples/fork.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/fork_prop.cc` & `cytosim-0.0.2/src/sim/couples/fork_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/fork_prop.h` & `cytosim-0.0.2/src/sim/couples/fork_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/shackle.cc` & `cytosim-0.0.2/src/sim/couples/shackle.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/shackle.h` & `cytosim-0.0.2/src/sim/couples/shackle.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/shackle_long.cc` & `cytosim-0.0.2/src/sim/couples/shackle_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/shackle_long.h` & `cytosim-0.0.2/src/sim/couples/shackle_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/shackle_prop.cc` & `cytosim-0.0.2/src/sim/couples/shackle_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/couples/shackle_prop.h` & `cytosim-0.0.2/src/sim/couples/shackle_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/event.cc` & `cytosim-0.0.2/src/sim/event.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/event.h` & `cytosim-0.0.2/src/sim/event.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/event_set.cc` & `cytosim-0.0.2/src/sim/event_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/event_set.h` & `cytosim-0.0.2/src/sim/event_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fiber.cc` & `cytosim-0.0.2/src/sim/fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fiber.h` & `cytosim-0.0.2/src/sim/fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fiber_grid.cc` & `cytosim-0.0.2/src/sim/fiber_grid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fiber_grid.h` & `cytosim-0.0.2/src/sim/fiber_grid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fiber_grid2.cc` & `cytosim-0.0.2/src/sim/fiber_grid2.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fiber_prop.cc` & `cytosim-0.0.2/src/sim/fiber_prop.cc`

 * *Files 0% similar despite different names*

```diff
@@ -199,24 +199,24 @@
         
         FiberEnd ref = CENTER;
         if ( opt.set(ref, "reference", {{"plus_end", PLUS_END}, {"minus_end", MINUS_END}, {"center", CENTER}}) )
             fib->placeEnd(ref);
     }
     
     // possible dynamic states of the ends
-    Glossary::dict_type<state_t> keys({{"white",     STATE_WHITE},
-                                       {"green",     STATE_GREEN},
-                                       {"yellow",    STATE_YELLOW},
-                                       {"orange",    STATE_ORANGE},
-                                       {"red",       STATE_RED},
-                                       {"static",    STATE_WHITE},
-                                       {"grow",      STATE_GREEN},
-                                       {"growing",   STATE_GREEN},
-                                       {"shrink",    STATE_RED},
-                                       {"shrinking", STATE_RED}});
+    Glossary::dict_type<state_t> keys{{"white",     STATE_WHITE},
+                                      {"green",     STATE_GREEN},
+                                      {"yellow",    STATE_YELLOW},
+                                      {"orange",    STATE_ORANGE},
+                                      {"red",       STATE_RED},
+                                      {"static",    STATE_WHITE},
+                                      {"grow",      STATE_GREEN},
+                                      {"growing",   STATE_GREEN},
+                                      {"shrink",    STATE_RED},
+                                      {"shrinking", STATE_RED}};
     
     
     // set state of plus ends:
     state_t p = STATE_WHITE;
 #ifdef BACKWARD_COMPATIBILITY
     if ( opt.set(p, "plus_end_state") )
     {
```

### Comparing `cytosim-0.0.1/src/sim/fiber_prop.h` & `cytosim-0.0.2/src/sim/fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fiber_segment.cc` & `cytosim-0.0.2/src/sim/fiber_segment.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fiber_segment.h` & `cytosim-0.0.2/src/sim/fiber_segment.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fiber_set.cc` & `cytosim-0.0.2/src/sim/fiber_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fiber_set.h` & `cytosim-0.0.2/src/sim/fiber_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fiber_site.cc` & `cytosim-0.0.2/src/sim/fiber_site.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fiber_site.h` & `cytosim-0.0.2/src/sim/fiber_site.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/classic_fiber.cc` & `cytosim-0.0.2/src/sim/fibers/classic_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/classic_fiber.h` & `cytosim-0.0.2/src/sim/fibers/classic_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/classic_fiber_prop.cc` & `cytosim-0.0.2/src/sim/fibers/classic_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/classic_fiber_prop.h` & `cytosim-0.0.2/src/sim/fibers/classic_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/dynamic_fiber.cc` & `cytosim-0.0.2/src/sim/fibers/dynamic_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/dynamic_fiber.h` & `cytosim-0.0.2/src/sim/fibers/dynamic_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/dynamic_fiber_prop.cc` & `cytosim-0.0.2/src/sim/fibers/dynamic_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/dynamic_fiber_prop.h` & `cytosim-0.0.2/src/sim/fibers/dynamic_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/growing_fiber.cc` & `cytosim-0.0.2/src/sim/fibers/growing_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/growing_fiber.h` & `cytosim-0.0.2/src/sim/fibers/growing_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/growing_fiber_prop.cc` & `cytosim-0.0.2/src/sim/fibers/growing_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/growing_fiber_prop.h` & `cytosim-0.0.2/src/sim/fibers/growing_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/treadmilling_fiber.cc` & `cytosim-0.0.2/src/sim/fibers/treadmilling_fiber.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/treadmilling_fiber.h` & `cytosim-0.0.2/src/sim/fibers/treadmilling_fiber.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/treadmilling_fiber_prop.cc` & `cytosim-0.0.2/src/sim/fibers/treadmilling_fiber_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/fibers/treadmilling_fiber_prop.h` & `cytosim-0.0.2/src/sim/fibers/treadmilling_fiber_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/field.cc` & `cytosim-0.0.2/src/sim/field.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/field.h` & `cytosim-0.0.2/src/sim/field.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/field_prop.cc` & `cytosim-0.0.2/src/sim/field_prop.cc`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     time_step             = 0;
 }
 
 
 //------------------------------------------------------------------------------
 void FieldProp::read(Glossary& glos)
 {
-    Glossary::dict_type<int> keys({{"flux", 0}, {"edge", 7},
-                                   {"edgeX", 1}, {"edgeY", 2}, {"edgeZ", 4},
-                                   {"edgeXY", 3}, {"edgeYZ", 6}, {"edgeXZ", 5}});
+    Glossary::dict_type<int> keys{{"flux", 0}, {"edge", 7},
+                                  {"edgeX", 1}, {"edgeY", 2}, {"edgeZ", 4},
+                                  {"edgeXY", 3}, {"edgeYZ", 6}, {"edgeXZ", 5}};
     
     glos.set(step,               "step");
     glos.set(periodic,           "periodic");
     glos.set(confine_space,      "space");
     glos.set(diffusion,          "diffusion");
     glos.set(full_diffusion,     "full_diffusion");
     glos.set(boundary_condition, "boundary_condition", keys);
```

### Comparing `cytosim-0.0.1/src/sim/field_prop.h` & `cytosim-0.0.2/src/sim/field_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/field_set.cc` & `cytosim-0.0.2/src/sim/field_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/field_set.h` & `cytosim-0.0.2/src/sim/field_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/field_values.h` & `cytosim-0.0.2/src/sim/field_values.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/frame_reader.cc` & `cytosim-0.0.2/src/sim/frame_reader.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/frame_reader.h` & `cytosim-0.0.2/src/sim/frame_reader.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hand.cc` & `cytosim-0.0.2/src/sim/hand.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hand.h` & `cytosim-0.0.2/src/sim/hand.h`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
     /// the monitor associated with this Hand
     HandMonitor *  haMonitor;
     
     /// Gillespie normalized time for detachment (must be set at attachment)
     real           nextDetach;
     
 public:
+	/// The monitor of that hand
+	HandMonitor const* monitor() {return haMonitor;} 
     
     /// Property is constant, so we do not need to make it private
     HandProp const* prop;
 
     /// Property
     HandProp const* property() const { return prop; }
     
@@ -78,15 +80,14 @@
          Hand * h = hp->newHand(this);
      */
     Hand(HandProp const*, HandMonitor*);
 
     /// destructor
     virtual ~Hand();
 
-
     /// return next Hand in Fiber's list
     Hand *  next()  const  { return haNext; }
     
     /// return previous Hand in Fiber's list
     Hand *  prev()  const  { return haPrev; }
 
     /// set next Hand in Fiber's list
```

### Comparing `cytosim-0.0.1/src/sim/hand_monitor.h` & `cytosim-0.0.2/src/sim/hand_monitor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hand_prop.cc` & `cytosim-0.0.2/src/sim/hand_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hand_prop.h` & `cytosim-0.0.2/src/sim/hand_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/actor.cc` & `cytosim-0.0.2/src/sim/hands/actor.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/actor.h` & `cytosim-0.0.2/src/sim/hands/actor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/actor_prop.cc` & `cytosim-0.0.2/src/sim/hands/actor_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/actor_prop.h` & `cytosim-0.0.2/src/sim/hands/actor_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/chewer.cc` & `cytosim-0.0.2/src/sim/hands/chewer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/chewer.h` & `cytosim-0.0.2/src/sim/hands/chewer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/chewer_prop.cc` & `cytosim-0.0.2/src/sim/hands/chewer_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/chewer_prop.h` & `cytosim-0.0.2/src/sim/hands/chewer_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/cutter.cc` & `cytosim-0.0.2/src/sim/hands/cutter.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/cutter.h` & `cytosim-0.0.2/src/sim/hands/cutter.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/cutter_prop.cc` & `cytosim-0.0.2/src/sim/hands/cutter_prop.cc`

 * *Files 5% similar despite different names*

```diff
@@ -29,23 +29,23 @@
 void CutterProp::read(Glossary& glos)
 {
     HandProp::read(glos);
     
     glos.set(cutting_rate,  "cutting_rate");
     
     // possible dynamic states of the ends
-    Glossary::dict_type<state_t> keys({{"white",     STATE_WHITE},
-                                       {"green",     STATE_GREEN},
-                                       {"yellow",    STATE_YELLOW},
-                                       {"orange",    STATE_ORANGE},
-                                       {"red",       STATE_RED},
-                                       {"static",    STATE_WHITE},
-                                       {"growing",   STATE_GREEN},
-                                       {"shrinking", STATE_RED},
-                                       {"delete",    STATE_BLACK}});
+    Glossary::dict_type<state_t> keys{{"white",     STATE_WHITE},
+                                      {"green",     STATE_GREEN},
+                                      {"yellow",    STATE_YELLOW},
+                                      {"orange",    STATE_ORANGE},
+                                      {"red",       STATE_RED},
+                                      {"static",    STATE_WHITE},
+                                      {"growing",   STATE_GREEN},
+                                      {"shrinking", STATE_RED},
+                                      {"delete",    STATE_BLACK}};
     
     glos.set(new_end_state[0], "new_end_state", keys);
     glos.set(new_end_state[1], "new_end_state", 1, keys);
 }
 
 
 void CutterProp::complete(Simul const& sim)
```

### Comparing `cytosim-0.0.1/src/sim/hands/cutter_prop.h` & `cytosim-0.0.2/src/sim/hands/cutter_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/digit.cc` & `cytosim-0.0.2/src/sim/hands/digit.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/digit.h` & `cytosim-0.0.2/src/sim/hands/digit.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/digit_prop.cc` & `cytosim-0.0.2/src/sim/hands/digit_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/digit_prop.h` & `cytosim-0.0.2/src/sim/hands/digit_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/dynein.cc` & `cytosim-0.0.2/src/sim/hands/dynein.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/dynein.h` & `cytosim-0.0.2/src/sim/hands/dynein.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/dynein_prop.cc` & `cytosim-0.0.2/src/sim/hands/dynein_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/dynein_prop.h` & `cytosim-0.0.2/src/sim/hands/dynein_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/kinesin.cc` & `cytosim-0.0.2/src/sim/hands/kinesin.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/kinesin.h` & `cytosim-0.0.2/src/sim/hands/kinesin.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/kinesin_prop.cc` & `cytosim-0.0.2/src/sim/hands/kinesin_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/kinesin_prop.h` & `cytosim-0.0.2/src/sim/hands/kinesin_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/mighty.cc` & `cytosim-0.0.2/src/sim/hands/mighty.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/mighty.h` & `cytosim-0.0.2/src/sim/hands/mighty.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/mighty_prop.cc` & `cytosim-0.0.2/src/sim/hands/mighty_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/mighty_prop.h` & `cytosim-0.0.2/src/sim/hands/mighty_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/motor.cc` & `cytosim-0.0.2/src/sim/hands/motor.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/motor.h` & `cytosim-0.0.2/src/sim/hands/motor.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/motor_prop.cc` & `cytosim-0.0.2/src/sim/hands/motor_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/motor_prop.h` & `cytosim-0.0.2/src/sim/hands/motor_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/myosin.cc` & `cytosim-0.0.2/src/sim/hands/myosin.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/myosin.h` & `cytosim-0.0.2/src/sim/hands/myosin.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/myosin_prop.cc` & `cytosim-0.0.2/src/sim/hands/myosin_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/myosin_prop.h` & `cytosim-0.0.2/src/sim/hands/myosin_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/nucleator.cc` & `cytosim-0.0.2/src/sim/hands/nucleator.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/nucleator.h` & `cytosim-0.0.2/src/sim/hands/nucleator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/nucleator_prop.cc` & `cytosim-0.0.2/src/sim/hands/nucleator_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/nucleator_prop.h` & `cytosim-0.0.2/src/sim/hands/nucleator_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/regulator.cc` & `cytosim-0.0.2/src/sim/hands/regulator.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/regulator.h` & `cytosim-0.0.2/src/sim/hands/regulator.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/regulator_prop.cc` & `cytosim-0.0.2/src/sim/hands/regulator_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/regulator_prop.h` & `cytosim-0.0.2/src/sim/hands/regulator_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/rescuer.cc` & `cytosim-0.0.2/src/sim/hands/rescuer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/rescuer.h` & `cytosim-0.0.2/src/sim/hands/rescuer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/rescuer_prop.cc` & `cytosim-0.0.2/src/sim/hands/rescuer_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/rescuer_prop.h` & `cytosim-0.0.2/src/sim/hands/rescuer_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/slider.cc` & `cytosim-0.0.2/src/sim/hands/slider.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/slider.h` & `cytosim-0.0.2/src/sim/hands/slider.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/slider_prop.cc` & `cytosim-0.0.2/src/sim/hands/slider_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/slider_prop.h` & `cytosim-0.0.2/src/sim/hands/slider_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/tracker.cc` & `cytosim-0.0.2/src/sim/hands/tracker.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/tracker.h` & `cytosim-0.0.2/src/sim/hands/tracker.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/tracker_prop.cc` & `cytosim-0.0.2/src/sim/hands/tracker_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/tracker_prop.h` & `cytosim-0.0.2/src/sim/hands/tracker_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/walker.cc` & `cytosim-0.0.2/src/sim/hands/walker.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/walker.h` & `cytosim-0.0.2/src/sim/hands/walker.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/walker_prop.cc` & `cytosim-0.0.2/src/sim/hands/walker_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/hands/walker_prop.h` & `cytosim-0.0.2/src/sim/hands/walker_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/interface.cc` & `cytosim-0.0.2/src/sim/interface.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/interface.h` & `cytosim-0.0.2/src/sim/interface.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/interpolation.cc` & `cytosim-0.0.2/src/sim/interpolation.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/interpolation.h` & `cytosim-0.0.2/src/sim/interpolation.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/interpolation4.cc` & `cytosim-0.0.2/src/sim/interpolation4.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/interpolation4.h` & `cytosim-0.0.2/src/sim/interpolation4.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/lattice.cc` & `cytosim-0.0.2/src/sim/lattice.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/lattice.h` & `cytosim-0.0.2/src/sim/lattice.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/makefile.inc` & `cytosim-0.0.2/src/sim/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/meca.cc` & `cytosim-0.0.2/src/sim/meca.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/meca.h` & `cytosim-0.0.2/src/sim/meca.h`

 * *Files 0% similar despite different names*

```diff
@@ -171,20 +171,26 @@
     /** 
      This is a symmetric square matrix of size `DIM*nbPoints()`
      It contains terms which are different in the X, Y, Z subspaces,
      arising from interactions which link coordinates from different subspaces.
     */
     MatrixSparseSymmetricBlock  mC;
     
-    /// base for force
+    /// base for force derivative
     real*   base()             { return vBAS; }
 
     /// base for force
     real&   base(index_t i) { return vBAS[i]; }
     
+    /// base for points
+    real*   points()             { return vPTS; }
+    
+    /// base for force
+    real*   force()             { return vFOR; }
+    
     /// position of point stored at vPTS[i]
     Vector  position1(const index_t inx) const
     {
         return Vector(vPTS+inx);
     }
     
     /// position interpolated from two points in vPTS[]
```

### Comparing `cytosim-0.0.1/src/sim/meca1d.h` & `cytosim-0.0.2/src/sim/meca1d.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/meca_inter.cc` & `cytosim-0.0.2/src/sim/meca_inter.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/mecable.cc` & `cytosim-0.0.2/src/sim/mecable.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/mecable.h` & `cytosim-0.0.2/src/sim/mecable.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/mecafil.cc` & `cytosim-0.0.2/src/sim/mecafil.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/mecafil.h` & `cytosim-0.0.2/src/sim/mecafil.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/mecafil_project.cc` & `cytosim-0.0.2/src/sim/mecafil_project.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/mecafil_projectmat.cc` & `cytosim-0.0.2/src/sim/mecafil_projectmat.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/mecapoint.cc` & `cytosim-0.0.2/src/sim/mecapoint.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/mecapoint.h` & `cytosim-0.0.2/src/sim/mecapoint.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/modulo.cc` & `cytosim-0.0.2/src/sim/modulo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/modulo.h` & `cytosim-0.0.2/src/sim/modulo.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/movable.cc` & `cytosim-0.0.2/src/sim/movable.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/movable.h` & `cytosim-0.0.2/src/sim/movable.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/object.cc` & `cytosim-0.0.2/src/sim/object.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/object.h` & `cytosim-0.0.2/src/sim/object.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/object_set.cc` & `cytosim-0.0.2/src/sim/object_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/object_set.h` & `cytosim-0.0.2/src/sim/object_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizer.cc` & `cytosim-0.0.2/src/sim/organizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizer.h` & `cytosim-0.0.2/src/sim/organizer.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizer_set.cc` & `cytosim-0.0.2/src/sim/organizer_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizer_set.h` & `cytosim-0.0.2/src/sim/organizer_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/aster.cc` & `cytosim-0.0.2/src/sim/organizers/aster.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/aster.h` & `cytosim-0.0.2/src/sim/organizers/aster.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/aster_prop.cc` & `cytosim-0.0.2/src/sim/organizers/aster_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/aster_prop.h` & `cytosim-0.0.2/src/sim/organizers/aster_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/bundle.cc` & `cytosim-0.0.2/src/sim/organizers/bundle.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/bundle.h` & `cytosim-0.0.2/src/sim/organizers/bundle.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/bundle_prop.cc` & `cytosim-0.0.2/src/sim/organizers/bundle_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/bundle_prop.h` & `cytosim-0.0.2/src/sim/organizers/bundle_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/fake.cc` & `cytosim-0.0.2/src/sim/organizers/fake.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/fake.h` & `cytosim-0.0.2/src/sim/organizers/fake.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/fake_prop.cc` & `cytosim-0.0.2/src/sim/organizers/fake_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/fake_prop.h` & `cytosim-0.0.2/src/sim/organizers/fake_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/nucleus.cc` & `cytosim-0.0.2/src/sim/organizers/nucleus.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/nucleus.h` & `cytosim-0.0.2/src/sim/organizers/nucleus.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/nucleus_prop.cc` & `cytosim-0.0.2/src/sim/organizers/nucleus_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/organizers/nucleus_prop.h` & `cytosim-0.0.2/src/sim/organizers/nucleus_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/parser.cc` & `cytosim-0.0.2/src/sim/parser.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/parser.h` & `cytosim-0.0.2/src/sim/parser.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/point_grid.cc` & `cytosim-0.0.2/src/sim/point_grid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/point_grid.h` & `cytosim-0.0.2/src/sim/point_grid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/sim.cc` & `cytosim-0.0.2/src/sim/sim.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/sim_thread.cc` & `cytosim-0.0.2/src/sim/sim_thread.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/sim_thread.h` & `cytosim-0.0.2/src/sim/sim_thread.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/simul.cc` & `cytosim-0.0.2/src/sim/simul.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/simul.h` & `cytosim-0.0.2/src/sim/simul.h`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,25 @@
 class SimulProp;
 
 /// default name for output trajectory file
 const char TRAJECTORY[] = "objects.cmo";
 
 
 /// Simulator class containing all Objects
+/**
+
+ Simul is the core class of cytosim. 
+ It holds the various sets of objects in the simulation, and methods to alter 
+ these objects, and progress the simulation.
+ It holds for example : 
+ - `Fibers` (a FiberSet)
+ - `Spaces` (a SpaceSet)
+ - `Singles` (a SingleSet)
+ - Etc. 
+ */
 class Simul
 {
 public:
     
     /// Meca used to set and integrate the equations of motion of Mecables
     mutable Meca      sMeca;
```

### Comparing `cytosim-0.0.1/src/sim/simul_custom.cc` & `cytosim-0.0.2/src/sim/simul_custom.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/simul_file.cc` & `cytosim-0.0.2/src/sim/simul_file.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/simul_prop.cc` & `cytosim-0.0.2/src/sim/simul_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/simul_prop.h` & `cytosim-0.0.2/src/sim/simul_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/simul_report.cc` & `cytosim-0.0.2/src/sim/simul_report.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/simul_solve.cc` & `cytosim-0.0.2/src/sim/simul_solve.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/simul_step.cc` & `cytosim-0.0.2/src/sim/simul_step.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/single.cc` & `cytosim-0.0.2/src/sim/single.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/single.h` & `cytosim-0.0.2/src/sim/single.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/single_prop.cc` & `cytosim-0.0.2/src/sim/single_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/single_prop.h` & `cytosim-0.0.2/src/sim/single_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/single_set.cc` & `cytosim-0.0.2/src/sim/single_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/single_set.h` & `cytosim-0.0.2/src/sim/single_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/singles/picket.cc` & `cytosim-0.0.2/src/sim/singles/picket.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/singles/picket.h` & `cytosim-0.0.2/src/sim/singles/picket.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/singles/picket_long.cc` & `cytosim-0.0.2/src/sim/singles/picket_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/singles/picket_long.h` & `cytosim-0.0.2/src/sim/singles/picket_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/singles/wrist.cc` & `cytosim-0.0.2/src/sim/singles/wrist.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/singles/wrist.h` & `cytosim-0.0.2/src/sim/singles/wrist.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/singles/wrist_long.cc` & `cytosim-0.0.2/src/sim/singles/wrist_long.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/singles/wrist_long.h` & `cytosim-0.0.2/src/sim/singles/wrist_long.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/solid.cc` & `cytosim-0.0.2/src/sim/solid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/solid.h` & `cytosim-0.0.2/src/sim/solid.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/solid_prop.cc` & `cytosim-0.0.2/src/sim/solid_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/solid_prop.h` & `cytosim-0.0.2/src/sim/solid_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/solid_set.cc` & `cytosim-0.0.2/src/sim/solid_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/solid_set.h` & `cytosim-0.0.2/src/sim/solid_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/space.cc` & `cytosim-0.0.2/src/sim/space.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/space.h` & `cytosim-0.0.2/src/sim/space.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/space_prop.cc` & `cytosim-0.0.2/src/sim/space_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/space_prop.h` & `cytosim-0.0.2/src/sim/space_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/space_set.cc` & `cytosim-0.0.2/src/sim/space_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/space_set.h` & `cytosim-0.0.2/src/sim/space_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_banana.cc` & `cytosim-0.0.2/src/sim/spaces/space_banana.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_banana.h` & `cytosim-0.0.2/src/sim/spaces/space_banana.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_capsule.cc` & `cytosim-0.0.2/src/sim/spaces/space_capsule.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_capsule.h` & `cytosim-0.0.2/src/sim/spaces/space_capsule.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_cylinder.cc` & `cytosim-0.0.2/src/sim/spaces/space_cylinder.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_cylinder.h` & `cytosim-0.0.2/src/sim/spaces/space_cylinder.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_cylinderP.cc` & `cytosim-0.0.2/src/sim/spaces/space_cylinderP.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_cylinderP.h` & `cytosim-0.0.2/src/sim/spaces/space_cylinderP.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_cylinderZ.cc` & `cytosim-0.0.2/src/sim/spaces/space_cylinderZ.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_cylinderZ.h` & `cytosim-0.0.2/src/sim/spaces/space_cylinderZ.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_dice.cc` & `cytosim-0.0.2/src/sim/spaces/space_dice.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_dice.h` & `cytosim-0.0.2/src/sim/spaces/space_dice.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_ellipse.cc` & `cytosim-0.0.2/src/sim/spaces/space_ellipse.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_ellipse.h` & `cytosim-0.0.2/src/sim/spaces/space_ellipse.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_periodic.cc` & `cytosim-0.0.2/src/sim/spaces/space_periodic.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_periodic.h` & `cytosim-0.0.2/src/sim/spaces/space_periodic.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_polygon.cc` & `cytosim-0.0.2/src/sim/spaces/space_polygon.cc`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
     glBegin(GL_POINTS);
     for ( unsigned n=0; n < npts; ++n )
         gle::gleVertex(pts[n].xx, pts[n].yy);
     glEnd();
 #endif
 #if ( 0 )
     // indicate index of each point:
-    char tmp[8];
+    char tmp[32];
     for ( unsigned n=0; n < npts; ++n )
     {
         snprintf(tmp, sizeof(tmp), "%i", n);
         Vector p(pts[n].xx, pts[n].yy, height_);
         gle::gleDrawText(p, tmp, 0);
     }
 #endif
```

### Comparing `cytosim-0.0.1/src/sim/spaces/space_polygon.h` & `cytosim-0.0.2/src/sim/spaces/space_polygon.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_polygonZ.cc` & `cytosim-0.0.2/src/sim/spaces/space_polygonZ.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_polygonZ.h` & `cytosim-0.0.2/src/sim/spaces/space_polygonZ.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_ring.cc` & `cytosim-0.0.2/src/sim/spaces/space_ring.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_ring.h` & `cytosim-0.0.2/src/sim/spaces/space_ring.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_sphere.cc` & `cytosim-0.0.2/src/sim/spaces/space_sphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_sphere.h` & `cytosim-0.0.2/src/sim/spaces/space_sphere.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_square.cc` & `cytosim-0.0.2/src/sim/spaces/space_square.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_square.h` & `cytosim-0.0.2/src/sim/spaces/space_square.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_strip.cc` & `cytosim-0.0.2/src/sim/spaces/space_strip.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_strip.h` & `cytosim-0.0.2/src/sim/spaces/space_strip.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_torus.cc` & `cytosim-0.0.2/src/sim/spaces/space_torus.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/spaces/space_torus.h` & `cytosim-0.0.2/src/sim/spaces/space_torus.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/sphere.cc` & `cytosim-0.0.2/src/sim/sphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/sphere.h` & `cytosim-0.0.2/src/sim/sphere.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/sphere_prop.cc` & `cytosim-0.0.2/src/sim/sphere_prop.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/sphere_prop.h` & `cytosim-0.0.2/src/sim/sphere_prop.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/sphere_set.cc` & `cytosim-0.0.2/src/sim/sphere_set.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/sphere_set.h` & `cytosim-0.0.2/src/sim/sphere_set.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/sim/splash.h` & `cytosim-0.0.2/src/sim/splash.h`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/CMakeLists.txt` & `cytosim-0.0.2/src/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/makefile.inc` & `cytosim-0.0.2/src/test/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test.cc` & `cytosim-0.0.2/src/test/test.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_blas.cc` & `cytosim-0.0.2/src/test/test_blas.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_code.cc` & `cytosim-0.0.2/src/test/test_code.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_cxx.cc` & `cytosim-0.0.2/src/test/test_cxx.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_gillespie.cc` & `cytosim-0.0.2/src/test/test_gillespie.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_glapp.cc` & `cytosim-0.0.2/src/test/test_glapp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_glos.cc` & `cytosim-0.0.2/src/test/test_glos.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_glut.cc` & `cytosim-0.0.2/src/test/test_glut.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_glut3D.cc` & `cytosim-0.0.2/src/test/test_glut3D.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_grid.cc` & `cytosim-0.0.2/src/test/test_grid.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_math.cc` & `cytosim-0.0.2/src/test/test_math.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_matrix.cc` & `cytosim-0.0.2/src/test/test_matrix.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_omp.cc` & `cytosim-0.0.2/src/test/test_omp.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_opengl.cc` & `cytosim-0.0.2/src/test/test_opengl.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_pipe.cc` & `cytosim-0.0.2/src/test/test_pipe.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_platonic.cc` & `cytosim-0.0.2/src/test/test_platonic.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_quaternion.cc` & `cytosim-0.0.2/src/test/test_quaternion.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_random.cc` & `cytosim-0.0.2/src/test/test_random.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_rasterizer.cc` & `cytosim-0.0.2/src/test/test_rasterizer.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_signal.cc` & `cytosim-0.0.2/src/test/test_signal.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_simd.cc` & `cytosim-0.0.2/src/test/test_simd.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_sizeof.cc` & `cytosim-0.0.2/src/test/test_sizeof.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_solve.cc` & `cytosim-0.0.2/src/test/test_solve.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_space.cc` & `cytosim-0.0.2/src/test/test_space.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_sphere.cc` & `cytosim-0.0.2/src/test/test_sphere.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_thread.cc` & `cytosim-0.0.2/src/test/test_thread.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/test/test_vbo.cc` & `cytosim-0.0.2/src/test/test_vbo.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/tools/CMakeLists.txt` & `cytosim-0.0.2/src/tools/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/tools/cymart.cc` & `cytosim-0.0.2/src/tools/cymart.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/tools/frametool.cc` & `cytosim-0.0.2/src/tools/frametool.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/tools/makefile.inc` & `cytosim-0.0.2/src/tools/makefile.inc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/tools/pycytoplay.cc` & `cytosim-0.0.2/src/tools/pycytoplay.cc`

 * *Files 26% similar despite different names*

```diff
@@ -37,25 +37,18 @@
 #include "view.h"
 #include "gle.h"
 #include <pybind11/functional.h>
 #include <thread>
 namespace py = pybind11;
 
 Player player;
-
-
-
-
-/// Using global vars, sorry not sorry.
-FrameReader reader ;
 Simul&      simul = player.simul;
-int __is_loaded__ = 0;
 SimThread & thread = player.thread;
-bool __saved__ = 0;
-Parser * parser;
+
+/// Using global vars, sorry not sorry.
 PlayerProp&  prop = player.prop;
 DisplayProp& disp = player.disp;
 
 
 #  include "glut.h"
 #  include "glapp.h"
 #  include "fiber_prop.h"
@@ -63,27 +56,24 @@
 #  include "point_disp.h"
 using glApp::flashText;
 #  include "play_keys.cc"
 #  include "play_menus.cc"
 #  include "play_mouse.cc"
 
 
-extern FrameReader reader;
-extern int __is_loaded__;
+//extern Simul simul;
 extern SimThread & thread;
-extern bool __saved__;
-extern Parser * parser;
 extern Player player;
 extern PlayerProp& prop;
 extern DisplayProp& disp;
 
 /// A holder for normalKey callback
 inline std::function<unsigned char(unsigned char, int, int)>& normalKey()
 {
-    // returns a different object for each thread that calls it
+    // returns a different object for each threadthread that calls it
     static thread_local std::function<unsigned char(unsigned char, int, int)> fn;
     return fn;
 }
 /// A proxy for the normalKeyy callback
 inline void proxyNormalKey(unsigned char c, int i, int j){ c = normalKey()(c, i ,j ); processNormalKey(c,i,j); };
 
 inline std::function<int(int, int, const Vector3&, int)>& mouseClick()
@@ -130,71 +120,115 @@
     else
     {
         thread.debug("display: trylock failed");
         glutPostRedisplay();
     }
 }
 
-/// Initiates a simulation
-Simul * start(std::string fname ) {
+
+PythonParser * open()
+{   
+    
+    int verbose = 1;
+    int prefix = 0;
+    
+    Glossary arg;
+
+    std::string input = TRAJECTORY;
+    std::string str;
+
+    //Simul * sim = new Simul;
+    
+    unsigned period = 1;
+
+    arg.set(input, ".cmo") || arg.set(input, "input");    
+    if ( arg.use_key("-") ) verbose = 0;
+
+    PythonParser * pyParse = new PythonParser(simul);
+
+    try
+    {
+        RNG.seed();
+        simul.loadProperties();
+        pyParse->activate(input, &thread);
+        Cytosim::all_silent();
+        
+    }
+    catch( Exception & e )
+    {
+        std::clog << "Aborted: " << e.what() << '\n';
+        return nullptr;
+    }
+	
+    
+    // Default null callbacks
+    normalKey() = [](unsigned char c, int i, int j) {return c;} ;
+    mouseClick() = [](int i, int j, const Vector3 v, int k) {return k;} ;
+    runtimeCheck() = [](Simul& sim) {};
+    
+    
+    return pyParse;
+}
+
+/**
+ * @brief Starts a simulation from a config file fname
+ * @param fname
+ * @return 
+ */
+PythonParser * start(std::string fname) {
     int n = fname.length();
     char inp[n] ;
     std::strcpy(inp, fname.c_str());
     Glossary arg;
     arg.read_string(inp,2);
     
     if ( ! arg.use_key("+") )
     {
         Cytosim::out.open("messages.cmo");
         Cytosim::log.redirect(Cytosim::out);
         Cytosim::warn.redirect(Cytosim::out);
     }
-    
+        
     try {
         simul.initialize(arg);
     }
     catch( Exception & e ) {
         print_magenta(std::cerr, e.brief());
         std::cerr << '\n' << e.info() << '\n';
     }
     catch(...) {
         print_red(std::cerr, "Error: an unknown exception occurred during initialization\n");
     }
     
-    //arg.print_warning(std::cerr, 1, " on command line\n");
     time_t sec = TicToc::seconds_since_1970();
     
     std::string file = simul.prop->config_file;
     std::string setup = file;
     
-    parser = new Parser(simul, 0, 1, 0, 0, 0);
-    parser->readConfig();
+    PythonParser * pyParse = new PythonParser(simul);
+    pyParse->activate(&thread);
     
-    thread.period(prop.period);
-    thread.start();
-    __is_loaded__ = 2;
-
+   
     // Default null callbacks
     normalKey() = [](unsigned char c, int i, int j) {return c;} ;
     mouseClick() = [](int i, int j, const Vector3 v, int k) {return k;} ;
     runtimeCheck() = [](Simul& sim) {};
     
-    std::cout << "WARNING : live usage of PyCytosim is still experimental." << std::endl;
-    
-    return &simul;
+    return pyParse;
 }
 
+
 void play_default(std::string opt){
 //#ifdef __APPLE__
 #if (1)
-    int argc = 1;
-    std::string st = "";
-    char * inp[1];
-    std::strcpy(*inp, st.c_str());
-    glutInit(&argc, inp);
+    int argc = 1 ;
+    char * str1 = (char*) malloc(10);
+    strcpy(str1," ");
+    char ** test = &str1;
+    glutInit(&argc, test);
 #endif
     Glossary arg = Glossary(opt);
     
     glApp::setDimensionality(DIM);
     if ( arg.use_key("fullscreen") )
         glApp::setFullScreen(1);
     View& view = glApp::views[0];
@@ -245,14 +279,15 @@
                 "def runtimeCheck(simul): \n"
                 "   print(simul.time()) \n"
                 "cytoplay.setRuntimeCheck(runtimeCheck) \n"
                 "cytoplay.play() \n";
                  // optional module docstring
     
     /// Loading properties into the module
+    load_interface_classes(m);
     load_object_classes(m);
     load_meca_classes(m);
     load_point_classes(m);
     auto pysim = load_simul_classes(m);
     load_glossary_classes(m);
     load_solid_classes(m);
     load_fiber_classes(m);
@@ -268,121 +303,40 @@
     auto sols = declare_group(m, ObjGroup<Solid,SolidProp>(), "SolidGroup");
     auto spas = declare_group(m, ObjGroup<Space,SpaceProp>(), "SpaceGroup");
     auto beds = declare_group(m, ObjGroup<Bead,BeadProp>(), "BeadGroup");
     auto sfrs = declare_group(m, ObjGroup<Sphere,SphereProp>(), "SphereGroup");
     auto orgs = declare_group(m, ObjGroup<Organizer,Property>(), "OrganizerGroup");
     auto sins = declare_group(m, ObjGroup<Single,SingleProp>(), "SingleGroup");
     auto cous = declare_group(m, ObjGroup<Couple,CoupleProp>(), "CoupleGroup");
-    
-    /// Python interface to timeframe : behaves roughly as a Python dict of ObjectGroup
-    py::class_<Frame>(m, "Timeframe")
-        .def_readwrite("fibers", &Frame::fibers, py::return_value_policy::reference)
-        .def_readwrite("time", &Frame::time)
-        .def_readwrite("index", &Frame::index)
-        .def_readwrite("loaded", &Frame::loaded)
-        .def("update", [](Frame &f) {  return make_frame(f.simul) ; })
-        .def("keys", [](Frame &f) {  return f.objects.attr("keys")() ; })
-        .def("items", [](Frame &f) { return f.objects.attr("items")() ; })
-        .def("__getitem__",[](const Frame &f, std::string s) {
-                 return f.objects[py::cast(s)];
-             }, py::return_value_policy::reference);
 
     /// Python interface to play/start a simulation
-    m.def("simul",[](){return &simul ;}, "@PYD;C:PyCytoplay;T:The ongoing simulation", py::return_value_policy::reference);
-    m.def("start",[](std::string fname ){return start(fname) ;}, py::return_value_policy::reference);
+    m.def("open", &open, "@PYD;C:PyCytosim;T:loads simulation from object files", py::return_value_policy::reference);
+    m.def("start", &start, "@PYD;C:PyCytosim;T:loads simulation from config files", py::return_value_policy::reference);
+    m.def("str_to_glos", &str_to_glos, "@PYD;C:PyCytosim;T:converts string to Glossary");
     m.def("play", [](py::args args) {
         int nargs = args.size();
         if (nargs == 0) { play_default("")  ; }
         else {
             std::string opt;
             for (auto arg : args) {
                 opt += py::cast<std::string>(arg);
                 }
             std::cout << opt << std::endl;
             play_default(opt);
             }
-        }, py::call_guard<py::gil_scoped_release>());
+        }, "@PYD;C:PyCytoplay;T: plays a simulation in live", py::call_guard<py::gil_scoped_release>());
+        
     m.def("setNormalKey",[](py::function f) { //@PYD;C:PyCytoplay;T: sets the callback function for normal keys
         normalKey() = py::cast<std::function<unsigned char(unsigned char, int, int)>>(f);
         });
     m.def("setRuntimeCheck",[](py::function f) { //@PYD;C:PyCytoplay;T: sets the callback function for runtime checks
         runtimeCheck() = py::cast<std::function<void(Simul&)>>(f);
     });
     m.def("setMouseClick",[](py::function f) { //@PYD;C:PyCytoplay;T: sets the callback function for mouse clicks
         mouseClick() = py::cast<std::function<int(int, int, Vector3, int)>>(f);
     });
- 
-    m.def("str_to_glos", &str_to_glos, "converts string to Glossary");
+    m.def("str_to_glos", &str_to_glos, "@PYD;C:PyCytosim;T:converts string to Glossary");
+
     
 
-    /// Expading Python interface to simul
-    pysim.def("frame", [](Simul * sim) // @PYD;C:Simul;T:returns current frame, e.g. frame = sim.frame();
-            {return make_frame(sim);} ); //py::return_value_policy::reference
-    pysim.def("writeObjects",  [](Simul * sim) { // @PYD;C:Simul;T: writes Objects to default trajectory file
-        sim->writeObjects(sim->prop->trajectory_file,__saved__,1);
-        if (!__saved__) {__saved__ = 1;}  ;} );
-    pysim.def("writeObjects",  [](Simul * sim, std::string & str) { // @PYD;C:Simul;T: writes Objects to a trajectory file, e.g. writeOjects('file.cmo')
-        sim->writeObjects(str,__saved__,1);
-        if (!__saved__) {__saved__ = 1;}  ;} );
-    pysim.def("save", [](Simul * sim) { // @PYD;C:Simul;T: saves current state to trajectory file
-            sim->writeObjects(sim->prop->trajectory_file,__saved__,1);
-            if (!__saved__) {__saved__ = 1;};
-            sim->writeProperties(&sim->prop->property_file[0],1);
-        });
-    pysim.def("add",  [](Simul * sim, py::args args) { // @PYD;C:Simul;T: adds objects to simulation, see provided examples 
-        std::string name = "";
-        std::string how = "";
-        int many = 1;
-        int nargs = args.size();
-        if (nargs>0) {
-            name = py::cast<std::string>(args[0]);
-        }
-        if (nargs>1) {
-            how = py::cast<std::string>(args[1]);
-        }
-        if (nargs>2) {
-            many = py::cast<int>(args[2]);
-        }
-        Glossary glos = Glossary(how);
-        ObjectList objects;
-        for (int i=0;i<many;++i) {
-            auto objs = parser->execute_new(name, glos);
-            objects.push_back(objs[0]);
-        }
-        return objects;
-        }, py::return_value_policy::reference); 
-    pysim.def("cut",  [](Simul * sim, std::string & name, std::string & where) { // @PYD;C:Simul;T: performes a cut : sim.cut(filament_name, where), see Parser.execute_cut  (C++)
-            Glossary glos = Glossary(where);
-            parser->execute_cut(name, glos);
-            });
-    pysim.def("delete",  [](Simul * sim, std::string & name, std::string & how, int number) { // @PYD;C:Simul;T: deletes objects from simulation, see provided examples
-            Glossary glos = Glossary(how);
-            parser->execute_delete(name, glos, number);
-            });
-    pysim.def("import",  [](Simul * sim, std::string & file, std::string & what, std::string & how) { // @PYD;C:Simul;T: imports objects from text file, see provided examples
-            Glossary glos = Glossary(how);
-            parser->execute_import(file, what, glos);
-            });
-    pysim.def("export",  [](Simul * sim, std::string & file, std::string & what, std::string & how) { // @PYD;C:Simul;T: export objects to text file, see provided examples
-            Glossary glos = Glossary(how);
-            parser->execute_export(file, what, glos);
-            });
-    pysim.def("run",  [](Simul * sim, py::args args) { // @PYD;C:Simul;T: runs the simulation ; eg. sim.run(1) ; sim.run(1,arguments)
-            std::string how = "";
-            int many = 1;
-            int nargs = args.size();
-            if (nargs>0) {
-                many = py::cast<int>(args[0]);
-            }
-            if (nargs>1) {
-                how = py::cast<std::string>(args[1]);
-            }
-            Glossary glos = Glossary(how);
-            parser->execute_run(many, glos,0);
-            });
-    pysim.def("set",  [](Simul * sim, std::string & cat, std::string & name, std::string & how) { // @PYD;C:Simul; defines a new object, see provided example
-            Glossary glos = Glossary(how);
-            parser->execute_set(cat, name, glos);
-            return glos;
-            });
 }
```

### Comparing `cytosim-0.0.1/src/tools/pycytosim.h` & `cytosim-0.0.2/src/tools/pycytosim.h`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,27 @@
 #include "filepath.h"
 #include "splash.h"
 #include "tictoc.h"
 #include <csignal>
 #include "unistd.h"
 #include "python_frame.h"
 #include "simul_modules.h"
+#include "interface_modules.h"
 #include "fiber_modules.h"
 #include "solid_modules.h"
 #include "space_modules.h"
 #include "point_modules.h"
+#include "thread_modules.h"
 #include "single_modules.h"
 #include "meca_modules.h"
 #include "couple_modules.h"
 #include "organizer_modules.h"
 #include "object_modules.h"
 #include "hand_modules.h"
 #include "glossary_modules.h"
 #include <functional>
 namespace py = pybind11;
 
 void bar(void);
 class SimThread;
+
 #endif
```

### Comparing `cytosim-0.0.1/src/tools/reader.cc` & `cytosim-0.0.2/src/tools/reader.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/tools/report.cc` & `cytosim-0.0.2/src/tools/report.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/tools/reportF.cc` & `cytosim-0.0.2/src/tools/reportF.cc`

 * *Files identical despite different names*

### Comparing `cytosim-0.0.1/src/tools/sieve.cc` & `cytosim-0.0.2/src/tools/sieve.cc`

 * *Files identical despite different names*

