# Comparing `tmp/pmbootstrap-1.9.0.tar.gz` & `tmp/pmbootstrap-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmbootstrap-1.9.0.tar", last modified: Mon Oct  7 21:01:03 2019, max compression
+gzip compressed data, was "pmbootstrap-2.0.0.tar", last modified: Tue Aug  1 06:20:35 2023, max compression
```

## Comparing `pmbootstrap-1.9.0.tar` & `pmbootstrap-2.0.0.tar`

### file list

```diff
@@ -1,157 +1,192 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/
--rwxrwxr-x   0 user      (1000) user      (1000)     2077 2018-10-12 07:16:05.000000 pmbootstrap-1.9.0/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3556 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)       26 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       42 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     7261 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmbootstrap.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     4930 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/test/
--rw-rw-r--   0 user      (1000) user      (1000)     2127 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_cross_compile_distcc.py
--rw-rw-r--   0 user      (1000) user      (1000)     2963 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_config_user.py
--rw-rw-r--   0 user      (1000) user      (1000)     1128 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_version_validate.py
--rw-rw-r--   0 user      (1000) user      (1000)     6643 2019-09-18 20:07:36.000000 pmbootstrap-1.9.0/test/test_aportgen_device_wizard.py
--rw-rw-r--   0 user      (1000) user      (1000)     5324 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/test/test_helpers_package.py
--rw-rw-r--   0 user      (1000) user      (1000)     2771 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_bootimg.py
--rw-rw-r--   0 user      (1000) user      (1000)     5481 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/test/test_helpers_repo_missing.py
--rw-rw-r--   0 user      (1000) user      (1000)     2483 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_chroot_interactive_shell.py
--rw-rw-r--   0 user      (1000) user      (1000)    11921 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_parse_apkindex.py
--rw-rw-r--   0 user      (1000) user      (1000)     1578 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_repo.py
--rw-rw-r--   0 user      (1000) user      (1000)    15171 2019-09-18 20:07:36.000000 pmbootstrap-1.9.0/test/test_build_package.py
--rw-rw-r--   0 user      (1000) user      (1000)     1236 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_frontend.py
--rw-rw-r--   0 user      (1000) user      (1000)     6723 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_pkgrel_bump.py
--rw-rw-r--   0 user      (1000) user      (1000)     1622 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_file.py
--rw-rw-r--   0 user      (1000) user      (1000)     2968 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_keys.py
--rw-rw-r--   0 user      (1000) user      (1000)     5330 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/test/test_run_core.py
--rw-rw-r--   0 user      (1000) user      (1000)     9736 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_questions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2633 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/test/test_parse_apkbuild.py
--rw-rw-r--   0 user      (1000) user      (1000)     2542 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/test/test_newapkbuild.py
--rw-rw-r--   0 user      (1000) user      (1000)     1865 2019-01-22 07:57:30.000000 pmbootstrap-1.9.0/test/test_folder_size.py
--rw-rw-r--   0 user      (1000) user      (1000)     5459 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_parse_depends.py
--rw-rw-r--   0 user      (1000) user      (1000)     6844 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/test/test_qemu_running_processes.py
--rw-rw-r--   0 user      (1000) user      (1000)     2103 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_install.py
--rw-rw-r--   0 user      (1000) user      (1000)     4830 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/test/test_aportgen.py
--rw-rw-r--   0 user      (1000) user      (1000)     2700 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/test/test_version.py
--rw-rw-r--   0 user      (1000) user      (1000)     1644 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_helpers_pmaports.py
--rw-rw-r--   0 user      (1000) user      (1000)     1658 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_mount.py
--rw-rw-r--   0 user      (1000) user      (1000)     3352 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_build_is_necessary.py
--rw-rw-r--   0 user      (1000) user      (1000)     5488 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_apk_static.py
--rw-rw-r--   0 user      (1000) user      (1000)     5923 2019-02-15 15:54:55.000000 pmbootstrap-1.9.0/test/test_envkernel.py
--rw-rw-r--   0 user      (1000) user      (1000)     4104 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/test/test_shell_escape.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/chroot/
--rw-rw-r--   0 user      (1000) user      (1000)     3774 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/shutdown.py
--rw-rw-r--   0 user      (1000) user      (1000)      964 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/chroot/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2212 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/binfmt.py
--rw-rw-r--   0 user      (1000) user      (1000)     3503 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/other.py
--rw-rw-r--   0 user      (1000) user      (1000)     4218 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/init.py
--rw-rw-r--   0 user      (1000) user      (1000)     3334 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/root.py
--rw-rw-r--   0 user      (1000) user      (1000)     4870 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/initfs.py
--rw-rw-r--   0 user      (1000) user      (1000)     1968 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/user.py
--rw-rw-r--   0 user      (1000) user      (1000)    10337 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/apk.py
--rw-rw-r--   0 user      (1000) user      (1000)     6260 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/zap.py
--rw-rw-r--   0 user      (1000) user      (1000)     2385 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/initfs_hooks.py
--rw-rw-r--   0 user      (1000) user      (1000)     4581 2019-05-19 17:55:07.000000 pmbootstrap-1.9.0/pmb/chroot/mount.py
--rw-rw-r--   0 user      (1000) user      (1000)     9424 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/distccd.py
--rw-rw-r--   0 user      (1000) user      (1000)     6789 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/chroot/apk_static.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/config/
--rw-rw-r--   0 user      (1000) user      (1000)    14567 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/pmb/config/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    15606 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/pmb/config/init.py
--rw-rw-r--   0 user      (1000) user      (1000)      906 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/config/save.py
--rw-rw-r--   0 user      (1000) user      (1000)     1767 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/config/load.py
--rw-rw-r--   0 user      (1000) user      (1000)     2005 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/config/merge_with_args.py
--rw-rw-r--   0 user      (1000) user      (1000)     5143 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/config/pmaports.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/data/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/data/keys/
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-4a6a0840.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-58cbb476.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-5243ef4b.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      499 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/README
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-5261cecb.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/pmos-5a03a13a.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-58199dcc.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-58e4f17d.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-524d27bb.rsa.pub
--rw-rw-r--   0 user      (1000) user      (1000)     5932 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/data/qemu-user-binfmt.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/flasher/
--rw-rw-r--   0 user      (1000) user      (1000)      887 2019-03-03 09:44:00.000000 pmbootstrap-1.9.0/pmb/flasher/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2016 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/flasher/init.py
--rw-rw-r--   0 user      (1000) user      (1000)     2701 2019-09-26 21:12:43.000000 pmbootstrap-1.9.0/pmb/flasher/run.py
--rw-rw-r--   0 user      (1000) user      (1000)     4766 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/flasher/frontend.py
--rw-rw-r--   0 user      (1000) user      (1000)     2249 2019-09-26 21:12:43.000000 pmbootstrap-1.9.0/pmb/flasher/variables.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/export/
--rw-rw-r--   0 user      (1000) user      (1000)      796 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/export/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2909 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/export/symlinks.py
--rw-rw-r--   0 user      (1000) user      (1000)     4758 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/export/odin.py
--rw-rw-r--   0 user      (1000) user      (1000)     1017 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/pmb/export/frontend.py
--rw-rw-r--   0 user      (1000) user      (1000)     3248 2019-02-15 15:54:55.000000 pmbootstrap-1.9.0/pmb/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/parse/
--rw-rw-r--   0 user      (1000) user      (1000)     5745 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/pmb/parse/kconfig.py
--rw-rw-r--   0 user      (1000) user      (1000)     9845 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/parse/version.py
--rw-rw-r--   0 user      (1000) user      (1000)      996 2019-02-15 15:54:55.000000 pmbootstrap-1.9.0/pmb/parse/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3833 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/parse/bootimg.py
--rw-rw-r--   0 user      (1000) user      (1000)     3976 2019-09-26 21:12:43.000000 pmbootstrap-1.9.0/pmb/parse/deviceinfo.py
--rw-rw-r--   0 user      (1000) user      (1000)     1639 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/parse/binfmt_info.py
--rw-rw-r--   0 user      (1000) user      (1000)     5336 2019-09-18 20:07:36.000000 pmbootstrap-1.9.0/pmb/parse/arch.py
--rw-rw-r--   0 user      (1000) user      (1000)    28173 2019-09-18 20:07:36.000000 pmbootstrap-1.9.0/pmb/parse/arguments.py
--rw-rw-r--   0 user      (1000) user      (1000)     6245 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/parse/depends.py
--rw-rw-r--   0 user      (1000) user      (1000)    14350 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/parse/apkindex.py
--rw-rw-r--   0 user      (1000) user      (1000)    10159 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/parse/_apkbuild.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/qemu/
--rw-rw-r--   0 user      (1000) user      (1000)      714 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/qemu/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    12179 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/qemu/run.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/aportgen/
--rw-rw-r--   0 user      (1000) user      (1000)     3798 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/pmb/aportgen/gcc.py
--rw-rw-r--   0 user      (1000) user      (1000)     2517 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/pmb/aportgen/binutils.py
--rw-rw-r--   0 user      (1000) user      (1000)     3493 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/aportgen/grub_efi.py
--rw-rw-r--   0 user      (1000) user      (1000)     3233 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/pmb/aportgen/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3790 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/aportgen/busybox_static.py
--rw-rw-r--   0 user      (1000) user      (1000)     9632 2019-03-03 09:44:00.000000 pmbootstrap-1.9.0/pmb/aportgen/device.py
--rw-rw-r--   0 user      (1000) user      (1000)     5355 2019-03-10 01:44:16.000000 pmbootstrap-1.9.0/pmb/aportgen/musl.py
--rw-rw-r--   0 user      (1000) user      (1000)     7707 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/pmb/aportgen/core.py
--rw-rw-r--   0 user      (1000) user      (1000)     4737 2019-01-22 07:57:30.000000 pmbootstrap-1.9.0/pmb/aportgen/linux.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/helpers/
--rw-rw-r--   0 user      (1000) user      (1000)     2615 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/file.py
--rw-rw-r--   0 user      (1000) user      (1000)     6785 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/pmb/helpers/package.py
--rw-rw-r--   0 user      (1000) user      (1000)      681 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     6673 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/helpers/other.py
--rw-rw-r--   0 user      (1000) user      (1000)     5936 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/pmb/helpers/repo_missing.py
--rw-rw-r--   0 user      (1000) user      (1000)     2663 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/http.py
--rw-rw-r--   0 user      (1000) user      (1000)     1211 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/ui.py
--rw-rw-r--   0 user      (1000) user      (1000)     3122 2019-05-19 17:55:07.000000 pmbootstrap-1.9.0/pmb/helpers/git.py
--rw-rw-r--   0 user      (1000) user      (1000)     3768 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/logging.py
--rw-rw-r--   0 user      (1000) user      (1000)     3886 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/mount.py
--rw-rw-r--   0 user      (1000) user      (1000)     7388 2019-03-03 09:44:00.000000 pmbootstrap-1.9.0/pmb/helpers/repo.py
--rw-rw-r--   0 user      (1000) user      (1000)     3171 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/run.py
--rw-rw-r--   0 user      (1000) user      (1000)    12449 2019-09-16 20:00:48.000000 pmbootstrap-1.9.0/pmb/helpers/frontend.py
--rw-rw-r--   0 user      (1000) user      (1000)     2329 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/cli.py
--rw-rw-r--   0 user      (1000) user      (1000)     7915 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/args.py
--rw-rw-r--   0 user      (1000) user      (1000)     6376 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/helpers/pmaports.py
--rw-rw-r--   0 user      (1000) user      (1000)     6502 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/pkgrel_bump.py
--rw-rw-r--   0 user      (1000) user      (1000)    12983 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/helpers/run_core.py
--rw-rw-r--   0 user      (1000) user      (1000)     1608 2019-01-10 21:07:28.000000 pmbootstrap-1.9.0/pmb/helpers/devices.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/build/
--rw-rw-r--   0 user      (1000) user      (1000)      988 2019-09-18 20:07:36.000000 pmbootstrap-1.9.0/pmb/build/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3078 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/build/autodetect.py
--rw-rw-r--   0 user      (1000) user      (1000)     6775 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/pmb/build/other.py
--rw-rw-r--   0 user      (1000) user      (1000)     3712 2019-09-18 20:07:36.000000 pmbootstrap-1.9.0/pmb/build/init.py
--rw-rw-r--   0 user      (1000) user      (1000)    19436 2019-04-24 14:07:00.000000 pmbootstrap-1.9.0/pmb/build/_package.py
--rw-rw-r--   0 user      (1000) user      (1000)     7499 2019-05-19 17:55:07.000000 pmbootstrap-1.9.0/pmb/build/envkernel.py
--rw-rw-r--   0 user      (1000) user      (1000)     2495 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/build/newapkbuild.py
--rw-rw-r--   0 user      (1000) user      (1000)     5956 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/build/menuconfig.py
--rw-rw-r--   0 user      (1000) user      (1000)     1788 2019-07-05 19:13:40.000000 pmbootstrap-1.9.0/pmb/build/checksum.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/pmb/install/
--rw-rw-r--   0 user      (1000) user      (1000)     1864 2019-05-19 17:55:07.000000 pmbootstrap-1.9.0/pmb/install/file.py
--rw-rw-r--   0 user      (1000) user      (1000)     2919 2019-03-03 09:44:00.000000 pmbootstrap-1.9.0/pmb/install/recovery.py
--rw-rw-r--   0 user      (1000) user      (1000)      907 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/install/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3300 2019-01-22 07:57:30.000000 pmbootstrap-1.9.0/pmb/install/format.py
--rw-rw-r--   0 user      (1000) user      (1000)     2988 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/install/losetup.py
--rw-rw-r--   0 user      (1000) user      (1000)    20576 2019-10-07 21:01:02.000000 pmbootstrap-1.9.0/pmb/install/_install.py
--rw-rw-r--   0 user      (1000) user      (1000)     5990 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/install/blockdevice.py
--rw-rw-r--   0 user      (1000) user      (1000)     3014 2019-01-03 07:47:42.000000 pmbootstrap-1.9.0/pmb/install/partition.py
--rw-rw-r--   0 user      (1000) user      (1000)    35141 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       67 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)       45 2018-10-09 04:56:02.000000 pmbootstrap-1.9.0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     7261 2019-10-07 21:01:03.000000 pmbootstrap-1.9.0/PKG-INFO
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:35.045000 pmbootstrap-2.0.0/
+-rw-rw-r--   0 user      (1000) user      (1000)    35141 2018-10-09 04:56:02.000000 pmbootstrap-2.0.0/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       45 2018-10-09 04:56:02.000000 pmbootstrap-2.0.0/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     7611 2023-08-01 06:20:35.045000 pmbootstrap-2.0.0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     6719 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.844000 pmbootstrap-2.0.0/pmb/
+-rw-r--r--   0 user      (1000) user      (1000)     3498 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.848000 pmbootstrap-2.0.0/pmb/aportgen/
+-rw-rw-r--   0 user      (1000) user      (1000)     2737 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/aportgen/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1075 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/aportgen/binutils.py
+-rw-r--r--   0 user      (1000) user      (1000)     2624 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/aportgen/busybox_static.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8238 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/aportgen/core.py
+-rw-r--r--   0 user      (1000) user      (1000)    11624 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/aportgen/device.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3506 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/aportgen/gcc.py
+-rw-r--r--   0 user      (1000) user      (1000)     2405 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/aportgen/grub_efi.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4506 2023-04-18 19:29:48.000000 pmbootstrap-2.0.0/pmb/aportgen/linux.py
+-rw-r--r--   0 user      (1000) user      (1000)     3952 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/aportgen/musl.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.853000 pmbootstrap-2.0.0/pmb/build/
+-rw-r--r--   0 user      (1000) user      (1000)      409 2023-05-17 19:01:45.000000 pmbootstrap-2.0.0/pmb/build/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    20627 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/build/_package.py
+-rw-r--r--   0 user      (1000) user      (1000)     2682 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/build/autodetect.py
+-rw-r--r--   0 user      (1000) user      (1000)     1211 2023-05-17 19:01:45.000000 pmbootstrap-2.0.0/pmb/build/checksum.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9122 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/build/envkernel.py
+-rw-r--r--   0 user      (1000) user      (1000)     4118 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/build/init.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5843 2023-04-18 19:29:48.000000 pmbootstrap-2.0.0/pmb/build/kconfig.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1882 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/build/newapkbuild.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7187 2023-04-18 19:29:48.000000 pmbootstrap-2.0.0/pmb/build/other.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.862000 pmbootstrap-2.0.0/pmb/chroot/
+-rw-rw-r--   0 user      (1000) user      (1000)      368 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/chroot/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9801 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/chroot/apk.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6082 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/chroot/apk_static.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1973 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/chroot/binfmt.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4899 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/chroot/init.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4481 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/chroot/initfs.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1740 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/chroot/initfs_hooks.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4198 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/chroot/mount.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2781 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/chroot/other.py
+-rw-r--r--   0 user      (1000) user      (1000)     2866 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/chroot/root.py
+-rw-r--r--   0 user      (1000) user      (1000)     3632 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/chroot/shutdown.py
+-rw-r--r--   0 user      (1000) user      (1000)     1394 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/chroot/user.py
+-rw-r--r--   0 user      (1000) user      (1000)     6239 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/chroot/zap.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.862000 pmbootstrap-2.0.0/pmb/ci/
+-rw-r--r--   0 user      (1000) user      (1000)     6260 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/ci/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.882000 pmbootstrap-2.0.0/pmb/config/
+-rw-r--r--   0 user      (1000) user      (1000)    36478 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/config/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    30834 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/config/init.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1245 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/config/load.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1460 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/config/merge_with_args.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8130 2023-04-18 19:29:48.000000 pmbootstrap-2.0.0/pmb/config/pmaports.py
+-rw-rw-r--   0 user      (1000) user      (1000)      299 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/config/save.py
+-rw-r--r--   0 user      (1000) user      (1000)     1216 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/config/sudo.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3609 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/config/workdir.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.883000 pmbootstrap-2.0.0/pmb/data/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.919000 pmbootstrap-2.0.0/pmb/data/keys/
+-rw-rw-r--   0 user      (1000) user      (1000)      475 2019-11-21 23:15:31.000000 pmbootstrap-2.0.0/pmb/data/keys/README
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-4a6a0840.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-5243ef4b.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-524d27bb.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-5261cecb.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-58199dcc.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-58cbb476.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2018-10-09 04:56:02.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-58e4f17d.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2021-11-06 20:19:25.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-5e69ca50.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      451 2021-11-06 20:19:25.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-60ac2099.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      800 2021-11-06 20:19:25.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-6165ee59.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      800 2021-11-06 20:19:25.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-61666e3f.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      800 2021-11-06 20:19:25.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-616a9724.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      800 2021-11-06 20:19:25.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-616abc23.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      800 2021-11-06 20:19:25.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-616ac3bc.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      800 2021-11-06 20:19:25.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-616adfeb.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      800 2021-11-06 20:19:25.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-616ae350.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      800 2021-11-06 20:19:25.000000 pmbootstrap-2.0.0/pmb/data/keys/alpine-devel@lists.alpinelinux.org-616db30d.rsa.pub
+-rw-rw-r--   0 user      (1000) user      (1000)      800 2019-11-10 12:52:13.000000 pmbootstrap-2.0.0/pmb/data/keys/build.postmarketos.org.rsa.pub
+-rw-r--r--   0 user      (1000) user      (1000)     1882 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/data/locales
+-rw-rw-r--   0 user      (1000) user      (1000)     5932 2018-10-09 04:56:02.000000 pmbootstrap-2.0.0/pmb/data/qemu-user-binfmt.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.922000 pmbootstrap-2.0.0/pmb/export/
+-rw-rw-r--   0 user      (1000) user      (1000)      189 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/export/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1064 2020-02-23 02:48:06.000000 pmbootstrap-2.0.0/pmb/export/frontend.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4410 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/export/odin.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2815 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/export/symlinks.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.929000 pmbootstrap-2.0.0/pmb/flasher/
+-rw-rw-r--   0 user      (1000) user      (1000)      325 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/flasher/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     6181 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/flasher/frontend.py
+-rw-r--r--   0 user      (1000) user      (1000)     2321 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/flasher/init.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3195 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/flasher/run.py
+-rw-r--r--   0 user      (1000) user      (1000)     4101 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/flasher/variables.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.956000 pmbootstrap-2.0.0/pmb/helpers/
+-rw-rw-r--   0 user      (1000) user      (1000)       74 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     5044 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/helpers/apk.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9848 2023-04-18 19:29:48.000000 pmbootstrap-2.0.0/pmb/helpers/aportupgrade.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5631 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/args.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4783 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/cli.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2170 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/devices.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3297 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/file.py
+-rw-r--r--   0 user      (1000) user      (1000)    23170 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/helpers/frontend.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11311 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/git.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3461 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/http.py
+-rw-r--r--   0 user      (1000) user      (1000)     1664 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/helpers/lint.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4010 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/logging.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3462 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/mount.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11618 2023-04-18 19:29:48.000000 pmbootstrap-2.0.0/pmb/helpers/other.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7036 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/package.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5189 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/pkgrel_bump.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10491 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/pmaports.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8491 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/repo.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5329 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/repo_missing.py
+-rw-r--r--   0 user      (1000) user      (1000)     1622 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/helpers/run.py
+-rw-r--r--   0 user      (1000) user      (1000)    15698 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/helpers/run_core.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6106 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/status.py
+-rw-rw-r--   0 user      (1000) user      (1000)      911 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/helpers/ui.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.972000 pmbootstrap-2.0.0/pmb/install/
+-rw-rw-r--   0 user      (1000) user      (1000)      400 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/install/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    48036 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/install/_install.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6259 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/install/blockdevice.py
+-rw-r--r--   0 user      (1000) user      (1000)     5929 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/install/format.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2427 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/install/losetup.py
+-rw-r--r--   0 user      (1000) user      (1000)     6729 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/install/partition.py
+-rw-r--r--   0 user      (1000) user      (1000)     2685 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/install/recovery.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2142 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/install/ui.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.976000 pmbootstrap-2.0.0/pmb/netboot/
+-rw-rw-r--   0 user      (1000) user      (1000)     2661 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/netboot/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.984000 pmbootstrap-2.0.0/pmb/parse/
+-rw-rw-r--   0 user      (1000) user      (1000)      452 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/parse/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14706 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/parse/_apkbuild.py
+-rw-r--r--   0 user      (1000) user      (1000)    14755 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/parse/apkindex.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3845 2023-04-18 19:29:48.000000 pmbootstrap-2.0.0/pmb/parse/arch.py
+-rw-r--r--   0 user      (1000) user      (1000)    45128 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/parse/arguments.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1006 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/parse/binfmt_info.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7598 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/parse/bootimg.py
+-rw-rw-r--   0 user      (1000) user      (1000)      997 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/parse/cpuinfo.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6910 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/parse/depends.py
+-rw-r--r--   0 user      (1000) user      (1000)     6335 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/parse/deviceinfo.py
+-rw-r--r--   0 user      (1000) user      (1000)    12866 2023-05-17 19:01:45.000000 pmbootstrap-2.0.0/pmb/parse/kconfig.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9235 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/parse/version.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.987000 pmbootstrap-2.0.0/pmb/qemu/
+-rw-rw-r--   0 user      (1000) user      (1000)      107 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/pmb/qemu/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)    13896 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/qemu/run.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.987000 pmbootstrap-2.0.0/pmb/sideload/
+-rw-r--r--   0 user      (1000) user      (1000)     3609 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmb/sideload/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:34.991000 pmbootstrap-2.0.0/pmbootstrap.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     7611 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmbootstrap.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     4734 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmbootstrap.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmbootstrap.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       41 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmbootstrap.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       26 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmbootstrap.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pmbootstrap.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)      152 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       67 2023-08-01 06:20:35.046000 pmbootstrap-2.0.0/setup.cfg
+-rwxrwxr-x   0 user      (1000) user      (1000)     2214 2023-04-18 19:29:48.000000 pmbootstrap-2.0.0/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-08-01 06:20:35.045000 pmbootstrap-2.0.0/test/
+-rw-rw-r--   0 user      (1000) user      (1000)     4951 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_apk.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4849 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_apk_static.py
+-rw-r--r--   0 user      (1000) user      (1000)     4463 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/test/test_aportgen.py
+-rw-r--r--   0 user      (1000) user      (1000)     7083 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/test/test_aportgen_device_wizard.py
+-rw-rw-r--   0 user      (1000) user      (1000)      789 2022-04-14 07:38:22.000000 pmbootstrap-2.0.0/test/test_arguments.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5066 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_bootimg.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3266 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_build_is_necessary.py
+-rw-r--r--   0 user      (1000) user      (1000)    17646 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/test/test_build_package.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1863 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_chroot_interactive_shell.py
+-rw-rw-r--   0 user      (1000) user      (1000)      514 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_config_init.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2324 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_config_pmaports.py
+-rw-r--r--   0 user      (1000) user      (1000)     2316 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/test/test_config_user.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4669 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_config_workdir.py
+-rw-r--r--   0 user      (1000) user      (1000)     3284 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/test/test_crossdirect.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4722 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_envkernel.py
+-rw-rw-r--   0 user      (1000) user      (1000)      932 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_file.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1141 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_folder_size.py
+-rw-rw-r--   0 user      (1000) user      (1000)      521 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_frontend.py
+-rw-r--r--   0 user      (1000) user      (1000)     6186 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/test/test_helpers_git.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1252 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_helpers_lint.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4663 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_helpers_package.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1591 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_helpers_pmaports.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2667 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_helpers_repo.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4780 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_helpers_repo_missing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2819 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_helpers_status.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1302 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_helpers_ui.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6358 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_install.py
+-rw-rw-r--   0 user      (1000) user      (1000)      931 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_mount.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2088 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_newapkbuild.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5529 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_parse_apkbuild.py
+-rw-rw-r--   0 user      (1000) user      (1000)    13601 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_parse_apkindex.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5324 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_parse_depends.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1113 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_parse_deviceinfo.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14520 2023-04-18 19:29:48.000000 pmbootstrap-2.0.0/test/test_parse_kconfig.py
+-rw-r--r--   0 user      (1000) user      (1000)     6576 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/test/test_pkgrel_bump.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6608 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_qemu_running_processes.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10581 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_questions.py
+-rw-r--r--   0 user      (1000) user      (1000)     5246 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/test/test_run_core.py
+-rw-r--r--   0 user      (1000) user      (1000)     3439 2023-08-01 06:20:34.000000 pmbootstrap-2.0.0/test/test_shell_escape.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2003 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_version.py
+-rw-rw-r--   0 user      (1000) user      (1000)      401 2023-02-19 15:20:53.000000 pmbootstrap-2.0.0/test/test_version_validate.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2436 2023-04-18 19:29:48.000000 pmbootstrap-2.0.0/test/test_zzz_keys.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pmbootstrap-1.9.0/setup.py` & `pmbootstrap-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,42 +22,46 @@
         import shlex
         import pytest
         errno = pytest.main(shlex.split(self.pytest_args))
         sys.exit(errno)
 
 
 here = path.abspath(path.dirname(__file__))
-_version_re = re.compile(r'version\s+=\s+(.*)')
+_version_re = re.compile(r'__version__\s+=\s+(.*)')
 
-with open(path.join(here, 'pmb/config/__init__.py'), 'rb') as f:
-    version = str(ast.literal_eval(_version_re.search(f.read().decode('utf-8')).group(1)))
+with open(path.join(here, 'pmb/__init__.py'), 'rb') as f:
+    version = str(ast.literal_eval(_version_re.search(
+        f.read().decode('utf-8')).group(1)))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='pmbootstrap',
     version=version,
-    description='A sophisticated chroot / build / flash tool to develop and install postmarketOS',
+    description='A sophisticated chroot / build / flash tool to '
+                'develop and install postmarketOS',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='postmarketOS Developers',
     author_email='info@postmarketos.org',
     url='https://www.postmarketos.org',
     license='GPLv3',
-    python_requires='>=3.4',
+    python_requires='>=3.7',
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     keywords='postmarketos pmbootstrap',
     packages=find_packages(exclude=['aports', 'keys', 'test']),
     tests_require=['pytest'],
     cmdclass={'test': PyTest},
     extras_require={
         'completion': ['argcomplete'],
```

### Comparing `pmbootstrap-1.9.0/pmbootstrap.egg-info/SOURCES.txt` & `pmbootstrap-2.0.0/pmbootstrap.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 pmb/__init__.py
 pmb/aportgen/__init__.py
 pmb/aportgen/binutils.py
 pmb/aportgen/busybox_static.py
 pmb/aportgen/core.py
@@ -15,126 +16,157 @@
 pmb/aportgen/musl.py
 pmb/build/__init__.py
 pmb/build/_package.py
 pmb/build/autodetect.py
 pmb/build/checksum.py
 pmb/build/envkernel.py
 pmb/build/init.py
-pmb/build/menuconfig.py
+pmb/build/kconfig.py
 pmb/build/newapkbuild.py
 pmb/build/other.py
 pmb/chroot/__init__.py
 pmb/chroot/apk.py
 pmb/chroot/apk_static.py
 pmb/chroot/binfmt.py
-pmb/chroot/distccd.py
 pmb/chroot/init.py
 pmb/chroot/initfs.py
 pmb/chroot/initfs_hooks.py
 pmb/chroot/mount.py
 pmb/chroot/other.py
 pmb/chroot/root.py
 pmb/chroot/shutdown.py
 pmb/chroot/user.py
 pmb/chroot/zap.py
+pmb/ci/__init__.py
 pmb/config/__init__.py
 pmb/config/init.py
 pmb/config/load.py
 pmb/config/merge_with_args.py
 pmb/config/pmaports.py
 pmb/config/save.py
+pmb/config/sudo.py
+pmb/config/workdir.py
+pmb/data/locales
 pmb/data/qemu-user-binfmt.txt
 pmb/data/keys/README
 pmb/data/keys/alpine-devel@lists.alpinelinux.org-4a6a0840.rsa.pub
 pmb/data/keys/alpine-devel@lists.alpinelinux.org-5243ef4b.rsa.pub
 pmb/data/keys/alpine-devel@lists.alpinelinux.org-524d27bb.rsa.pub
 pmb/data/keys/alpine-devel@lists.alpinelinux.org-5261cecb.rsa.pub
 pmb/data/keys/alpine-devel@lists.alpinelinux.org-58199dcc.rsa.pub
 pmb/data/keys/alpine-devel@lists.alpinelinux.org-58cbb476.rsa.pub
 pmb/data/keys/alpine-devel@lists.alpinelinux.org-58e4f17d.rsa.pub
-pmb/data/keys/pmos-5a03a13a.rsa.pub
+pmb/data/keys/alpine-devel@lists.alpinelinux.org-5e69ca50.rsa.pub
+pmb/data/keys/alpine-devel@lists.alpinelinux.org-60ac2099.rsa.pub
+pmb/data/keys/alpine-devel@lists.alpinelinux.org-6165ee59.rsa.pub
+pmb/data/keys/alpine-devel@lists.alpinelinux.org-61666e3f.rsa.pub
+pmb/data/keys/alpine-devel@lists.alpinelinux.org-616a9724.rsa.pub
+pmb/data/keys/alpine-devel@lists.alpinelinux.org-616abc23.rsa.pub
+pmb/data/keys/alpine-devel@lists.alpinelinux.org-616ac3bc.rsa.pub
+pmb/data/keys/alpine-devel@lists.alpinelinux.org-616adfeb.rsa.pub
+pmb/data/keys/alpine-devel@lists.alpinelinux.org-616ae350.rsa.pub
+pmb/data/keys/alpine-devel@lists.alpinelinux.org-616db30d.rsa.pub
+pmb/data/keys/build.postmarketos.org.rsa.pub
 pmb/export/__init__.py
 pmb/export/frontend.py
 pmb/export/odin.py
 pmb/export/symlinks.py
 pmb/flasher/__init__.py
 pmb/flasher/frontend.py
 pmb/flasher/init.py
 pmb/flasher/run.py
 pmb/flasher/variables.py
 pmb/helpers/__init__.py
+pmb/helpers/apk.py
+pmb/helpers/aportupgrade.py
 pmb/helpers/args.py
 pmb/helpers/cli.py
 pmb/helpers/devices.py
 pmb/helpers/file.py
 pmb/helpers/frontend.py
 pmb/helpers/git.py
 pmb/helpers/http.py
+pmb/helpers/lint.py
 pmb/helpers/logging.py
 pmb/helpers/mount.py
 pmb/helpers/other.py
 pmb/helpers/package.py
 pmb/helpers/pkgrel_bump.py
 pmb/helpers/pmaports.py
 pmb/helpers/repo.py
 pmb/helpers/repo_missing.py
 pmb/helpers/run.py
 pmb/helpers/run_core.py
+pmb/helpers/status.py
 pmb/helpers/ui.py
 pmb/install/__init__.py
 pmb/install/_install.py
 pmb/install/blockdevice.py
-pmb/install/file.py
 pmb/install/format.py
 pmb/install/losetup.py
 pmb/install/partition.py
 pmb/install/recovery.py
+pmb/install/ui.py
+pmb/netboot/__init__.py
 pmb/parse/__init__.py
 pmb/parse/_apkbuild.py
 pmb/parse/apkindex.py
 pmb/parse/arch.py
 pmb/parse/arguments.py
 pmb/parse/binfmt_info.py
 pmb/parse/bootimg.py
+pmb/parse/cpuinfo.py
 pmb/parse/depends.py
 pmb/parse/deviceinfo.py
 pmb/parse/kconfig.py
 pmb/parse/version.py
 pmb/qemu/__init__.py
 pmb/qemu/run.py
+pmb/sideload/__init__.py
 pmbootstrap.egg-info/PKG-INFO
 pmbootstrap.egg-info/SOURCES.txt
 pmbootstrap.egg-info/dependency_links.txt
 pmbootstrap.egg-info/entry_points.txt
 pmbootstrap.egg-info/requires.txt
 pmbootstrap.egg-info/top_level.txt
+test/test_apk.py
 test/test_apk_static.py
 test/test_aportgen.py
 test/test_aportgen_device_wizard.py
+test/test_arguments.py
 test/test_bootimg.py
 test/test_build_is_necessary.py
 test/test_build_package.py
 test/test_chroot_interactive_shell.py
+test/test_config_init.py
+test/test_config_pmaports.py
 test/test_config_user.py
-test/test_cross_compile_distcc.py
+test/test_config_workdir.py
+test/test_crossdirect.py
 test/test_envkernel.py
 test/test_file.py
 test/test_folder_size.py
 test/test_frontend.py
+test/test_helpers_git.py
+test/test_helpers_lint.py
 test/test_helpers_package.py
 test/test_helpers_pmaports.py
+test/test_helpers_repo.py
 test/test_helpers_repo_missing.py
+test/test_helpers_status.py
+test/test_helpers_ui.py
 test/test_install.py
-test/test_keys.py
 test/test_mount.py
 test/test_newapkbuild.py
 test/test_parse_apkbuild.py
 test/test_parse_apkindex.py
 test/test_parse_depends.py
+test/test_parse_deviceinfo.py
+test/test_parse_kconfig.py
 test/test_pkgrel_bump.py
 test/test_qemu_running_processes.py
 test/test_questions.py
-test/test_repo.py
 test/test_run_core.py
 test/test_shell_escape.py
 test/test_version.py
-test/test_version_validate.py
+test/test_version_validate.py
+test/test_zzz_keys.py
```

### Comparing `pmbootstrap-1.9.0/pmbootstrap.egg-info/PKG-INFO` & `pmbootstrap-2.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,214 +1,286 @@
-Metadata-Version: 2.1
-Name: pmbootstrap
-Version: 1.9.0
-Summary: A sophisticated chroot / build / flash tool to develop and install postmarketOS
-Home-page: https://www.postmarketos.org
-Author: postmarketOS Developers
-Author-email: info@postmarketos.org
-License: GPLv3
-Description: # pmbootstrap
-        [**Introduction**](https://postmarketos.org/blog/2017/05/26/intro/) | [**Security Warning**](https://ollieparanoid.github.io/post/security-warning/) | [**Devices**](https://wiki.postmarketos.org/wiki/Devices)
-        
-        Sophisticated chroot/build/flash tool to develop and install [postmarketOS](https://postmarketos.org).
-        
-        Package build scripts live in the [`pmaports`](https://gitlab.com/postmarketOS/pmaports) repository now.
-        
-        ## Requirements
-        * 2 GB of RAM recommended for compiling
-        * Linux distribution on the host system (`x86`, `x86_64`, or `aarch64`)
-          * [Windows subsystem for Linux (WSL)](https://en.wikipedia.org/wiki/Windows_Subsystem_for_Linux) does **not** work! Please use [VirtualBox](https://www.virtualbox.org/) instead.
-          * Kernels based on the grsec patchset [do **not** work](https://github.com/postmarketOS/pmbootstrap/issues/107) *(Alpine: use linux-vanilla instead of linux-hardened, Arch: linux-hardened [is not based on grsec](https://www.reddit.com/r/archlinux/comments/68b2jn/linuxhardened_in_community_repo_a_grsecurity/))*
-          * On Alpine Linux only: `apk add coreutils procps`
-          * [Linux kernel 3.17 or higher](https://postmarketos.org/oldkernel)
-        * Python 3.4+
-        * OpenSSL
-        
-        ## Usage Examples
-        Please refer to the [postmarketOS wiki](https://wiki.postmarketos.org) for in-depth coverage of topics such as [porting to a new device](https://wiki.postmarketos.org/wiki/Porting_to_a_new_device) or [installation](https://wiki.postmarketos.org/wiki/Installation_guide). The help output (`pmbootstrap -h`) has detailed usage instructions for every command. Read on for some generic examples of what can be done with `pmbootstrap`.
-        
-        ### Installing pmbootstrap
-        <https://wiki.postmarketos.org/wiki/Installing_pmbootstrap>
-        
-        ### Basics
-        Initial setup:
-        ```
-        $ pmbootstrap init
-        ```
-        
-        Run this in a second window to see all shell commands that get executed:
-        ```
-        $ pmbootstrap log
-        ```
-        
-        ### Packages
-        Build `aports/main/hello-world`:
-        ```
-        $ pmbootstrap build hello-world
-        ```
-        
-        Cross-compile to `armhf`:
-        ```
-        $ pmbootstrap build --arch=armhf hello-world
-        ```
-        
-        Build with source code from local folder:
-        ```
-        $ pmbootstrap build linux-postmarketos-mainline --src=~/code/linux
-        ```
-        
-        Update checksums:
-        ```
-        $ pmbootstrap checksum hello-world
-        ```
-        
-        Generate a template for a new package:
-        ```
-        $ pmbootstrap newapkbuild "https://gitlab.com/postmarketOS/osk-sdl/-/archive/0.52/osk-sdl-0.52.tar.bz2"
-        ```
-        
-        ### Chroots
-        Enter the `armhf` building chroot:
-        ```
-        $ pmbootstrap chroot -b armhf
-        ```
-        
-        Run a command inside a chroot:
-        ```
-        $ pmbootstrap chroot -- echo test
-        ```
-        
-        Safely delete all chroots:
-        ```
-        $ pmbootstrap zap
-        ```
-        
-        ### Device Porting Assistance
-        Analyze Android [`boot.img`](https://wiki.postmarketos.org/wiki/Glossary#boot.img) files (also works with recovery OS images like TWRP):
-        ```
-        $ pmbootstrap bootimg_analyze ~/Downloads/twrp-3.2.1-0-fp2.img
-        ```
-        
-        Check kernel configs:
-        ```
-        $ pmbootstrap kconfig check
-        ```
-        
-        Edit a kernel config:
-        ```
-        $ pmbootstrap kconfig edit --arch=armhf postmarketos-mainline
-        ```
-        
-        ### Root File System
-        Build the rootfs:
-        ```
-        $ pmbootstrap install
-        ```
-        
-        Build the rootfs with full disk encryption:
-        ```
-        $ pmbootstrap install --fde
-        ```
-        
-        Update existing installation on SD card:
-        ```
-        $ pmbootstrap install --sdcard=/dev/mmcblk0 --rsync
-        ```
-        
-        Run the image in QEMU:
-        ```
-        $ pmbootstrap qemu --image-size=1G
-        ```
-        
-        Flash to the device:
-        ```
-        $ pmbootstrap flasher flash_kernel
-        $ pmbootstrap flasher flash_rootfs --partition=userdata
-        ```
-        
-        Export the rootfs, kernel, initramfs, `boot.img` etc.:
-        ```
-        $ pmbootstrap export
-        ```
-        
-        Extract the initramfs
-        ```
-        $ pmbootstrap initfs extract
-        ```
-        
-        Build and flash Android recovery zip:
-        ```
-        $ pmbootstrap install --android-recovery-zip
-        $ pmbootstrap flasher --method=adb sideload
-        ```
-        
-        ### Repository Maintenance
-        List pmaports that don't have a binary package:
-        ```
-        $ pmbootstrap repo_missing --arch=armhf --overview
-        ```
-        
-        Increase the `pkgrel` for each aport where the binary package has outdated dependencies (e.g. after soname bumps):
-        ```
-        $ pmbootstrap pkgrel_bump --auto
-        ```
-        
-        Generate cross-compiler aports based on the latest version from Alpine's aports:
-        ```
-        $ pmbootstrap aportgen binutils-armhf gcc-armhf
-        ```
-        
-        Manually rebuild package index:
-        ```
-        $ pmbootstrap index
-        ```
-        
-        Delete local binary packages without existing aport of same version:
-        ```
-        $ pmbootstrap zap -m
-        ```
-        
-        ### Debugging
-        Use `-v` on any action to get verbose logging:
-        ```
-        $ pmbootstrap -v build hello-world
-        ```
-        
-        Parse a single APKBUILD and return it as JSON:
-        ```
-        $ pmbootstrap apkbuild_parse hello-world
-        ```
-        
-        Parse a package from an APKINDEX and return it as JSON:
-        ```
-        $ pmbootstrap apkindex_parse $WORK/cache_apk_x86_64/APKINDEX.8b865e19.tar.gz hello-world
-        ```
-        
-        `ccache` statistics:
-        ```
-        $ pmbootstrap stats --arch=armhf
-        ```
-        
-        `distccd` log:
-        ```
-        $ pmbootstrap log_distccd
-        ```
-        
-        ## Development
-        ### Testing
-        Install `pytest` (via your package manager or pip) and run it inside the pmbootstrap folder.
-        
-        ## License
-        [GPLv3](LICENSE)
-        
-Keywords: postmarketos pmbootstrap
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-Provides-Extra: completion
+# pmbootstrap
+
+Sophisticated chroot/build/flash tool to develop and install
+[postmarketOS](https://postmarketos.org).
+
+## Development
+
+pmbootstrap is being developed on SourceHut
+([what](https://postmarketos.org/blog/2022/07/25/considering-sourcehut/)):
+
+https://git.sr.ht/~postmarketos/pmbootstrap
+
+Send patches via mail or web UI to
+[pmbootstrap-devel](https://lists.sr.ht/~postmarketos/pmbootstrap-devel)
+([subscribe](mailto:~postmarketos/pmbootstrap-devel+subscribe@lists.sr.ht)):
+```
+~postmarketos/pmbootstrap-devel@lists.sr.ht
+```
+
+You can set the default values for sending email in the git checkout
+```
+$ git config sendemail.to "~postmarketos/pmbootstrap-devel@lists.sr.ht"
+$ git config format.subjectPrefix "PATCH pmbootstrap"
+```
+
+Run CI scripts locally with:
+```
+$ pmbootstrap ci
+```
+
+Run a single test file:
+```
+$ pytest -vv ./test/test_keys.py
+```
+
+## Issues
+
+Issues are being tracked
+[here](https://gitlab.com/postmarketOS/pmbootstrap/-/issues).
+
+## Requirements
+* Linux distribution on the host system (`x86`, `x86_64`, or `aarch64`)
+  * [Windows subsystem for Linux (WSL)](https://en.wikipedia.org/wiki/Windows_Subsystem_for_Linux)
+    does **not** work! Please use [VirtualBox](https://www.virtualbox.org/) instead.
+  * [Linux kernel 3.17 or higher](https://postmarketos.org/oldkernel)
+* Python 3.7+
+* OpenSSL
+* git
+* ps
+* tar
+
+## Usage Examples
+Please refer to the [postmarketOS wiki](https://wiki.postmarketos.org) for
+in-depth coverage of topics such as
+[porting to a new device](https://wiki.postmarketos.org/wiki/Porting_to_a_new_device)
+or [installation](https://wiki.postmarketos.org/wiki/Installation_guide). The
+help output (`pmbootstrap -h`) has detailed usage instructions for every
+command. Read on for some generic examples of what can be done with
+`pmbootstrap`.
+
+### Installing pmbootstrap
+<https://wiki.postmarketos.org/wiki/Installing_pmbootstrap>
+
+### Basics
+Initial setup:
+```
+$ pmbootstrap init
+```
+
+Run this in a second window to see all shell commands that get executed:
+```
+$ pmbootstrap log
+```
+
+Quick health check and config overview:
+```
+$ pmbootstrap status
+```
+
+### Packages
+Build `aports/main/hello-world`:
+```
+$ pmbootstrap build hello-world
+```
+
+Cross-compile to `armhf`:
+```
+$ pmbootstrap build --arch=armhf hello-world
+```
+
+Build with source code from local folder:
+```
+$ pmbootstrap build linux-postmarketos-mainline --src=~/code/linux
+```
+
+Update checksums:
+```
+$ pmbootstrap checksum hello-world
+```
+
+Generate a template for a new package:
+```
+$ pmbootstrap newapkbuild "https://gitlab.com/postmarketOS/osk-sdl/-/archive/0.52/osk-sdl-0.52.tar.bz2"
+```
+
+#### Default architecture
+
+Packages will be compiled for the architecture of the device running
+pmbootstrap by default. For example, if your `x86_64` PC runs pmbootstrap, it
+would build a package for `x86_64` with this command:
+```
+$ pmbootstrap build hello-world
+```
+
+If you would rather build for the target device selected in `pmbootstrap init`
+by default, then use the `build_default_device_arch` option:
+```
+$ pmbootstrap config build_default_device_arch True
+```
+
+If your target device is `pine64-pinephone` for example, pmbootstrap will now
+build this package for `aarch64`:
+```
+$ pmbootstrap build hello-world
+```
+
+### Chroots
+Enter the `armhf` building chroot:
+```
+$ pmbootstrap chroot -b armhf
+```
+
+Run a command inside a chroot:
+```
+$ pmbootstrap chroot -- echo test
+```
+
+Safely delete all chroots:
+```
+$ pmbootstrap zap
+```
+
+### Device Porting Assistance
+Analyze Android
+[`boot.img`](https://wiki.postmarketos.org/wiki/Glossary#boot.img) files (also
+works with recovery OS images like TWRP):
+```
+$ pmbootstrap bootimg_analyze ~/Downloads/twrp-3.2.1-0-fp2.img
+```
+
+Check kernel configs:
+```
+$ pmbootstrap kconfig check
+```
+
+Edit a kernel config:
+```
+$ pmbootstrap kconfig edit --arch=armhf postmarketos-mainline
+```
+
+### Root File System
+Build the rootfs:
+```
+$ pmbootstrap install
+```
+
+Build the rootfs with full disk encryption:
+```
+$ pmbootstrap install --fde
+```
+
+Update existing installation on SD card:
+```
+$ pmbootstrap install --sdcard=/dev/mmcblk0 --rsync
+```
+
+Run the image in QEMU:
+```
+$ pmbootstrap qemu --image-size=1G
+```
+
+Flash to the device:
+```
+$ pmbootstrap flasher flash_kernel
+$ pmbootstrap flasher flash_rootfs --partition=userdata
+```
+
+Export the rootfs, kernel, initramfs, `boot.img` etc.:
+```
+$ pmbootstrap export
+```
+
+Extract the initramfs
+```
+$ pmbootstrap initfs extract
+```
+
+Build and flash Android recovery zip:
+```
+$ pmbootstrap install --android-recovery-zip
+$ pmbootstrap flasher --method=adb sideload
+```
+
+### Repository Maintenance
+List pmaports that don't have a binary package:
+```
+$ pmbootstrap repo_missing --arch=armhf --overview
+```
+
+Increase the `pkgrel` for each aport where the binary package has outdated
+dependencies (e.g. after soname bumps):
+```
+$ pmbootstrap pkgrel_bump --auto
+```
+
+Generate cross-compiler aports based on the latest version from Alpine's
+aports:
+```
+$ pmbootstrap aportgen binutils-armhf gcc-armhf
+```
+
+Manually rebuild package index:
+```
+$ pmbootstrap index
+```
+
+Delete local binary packages without existing aport of same version:
+```
+$ pmbootstrap zap -m
+```
+
+### Debugging
+Use `-v` on any action to get verbose logging:
+```
+$ pmbootstrap -v build hello-world
+```
+
+Parse a single deviceinfo and return it as JSON:
+```
+$ pmbootstrap deviceinfo_parse pine64-pinephone
+```
+
+Parse a single APKBUILD and return it as JSON:
+```
+$ pmbootstrap apkbuild_parse hello-world
+```
+
+Parse a package from an APKINDEX and return it as JSON:
+```
+$ pmbootstrap apkindex_parse $WORK/cache_apk_x86_64/APKINDEX.8b865e19.tar.gz hello-world
+```
+
+`ccache` statistics:
+```
+$ pmbootstrap stats --arch=armhf
+```
+
+### Use alternative sudo
+
+pmbootstrap supports `doas` and `sudo`.
+If multiple sudo implementations are installed, pmbootstrap will use `doas`.
+You can set the `PMB_SUDO` environmental variable to define the sudo
+implementation you want to use.
+
+### Select SSH keys to include and make authorized in new images
+
+If the config file option `ssh_keys` is set to `True` (it defaults to `False`),
+then all files matching the glob `~/.ssh/id_*.pub` will be placed in
+`~/.ssh/authorized_keys` in the user's home directory in newly-built images.
+
+Sometimes, for example if you have a large number of SSH keys, you may wish to
+select a different set of public keys to include in an image. To do this, set
+the `ssh_key_glob` configuration parameter in the pmbootstrap config file to a
+string containing a glob that is to match the file or files you wish to
+include.
+
+For example, a `~/.config/pmbootstrap.cfg` may contain:
+
+    [pmbootstrap]
+    # ...
+    ssh_keys = True
+    ssh_key_glob = ~/.ssh/postmarketos-dev.pub
+    # ...
+
+## License
+[GPLv3](LICENSE)
```

### Comparing `pmbootstrap-1.9.0/test/test_config_user.py` & `pmbootstrap-2.0.0/test/test_config_user.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,35 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import os
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import sys
 import pytest
 
-# Import from parent directory
-sys.path.insert(0, os.path.realpath(
-    os.path.join(os.path.dirname(__file__) + "/..")))
+import pmb_test  # noqa
 import pmb.aportgen
 import pmb.config
 import pmb.helpers.frontend
 import pmb.helpers.logging
 import pmb.helpers.run
+import pmb.helpers.run_core
 
 
 @pytest.fixture
 def args(tmpdir, request):
     import pmb.parse
     sys.argv = ["pmbootstrap.py", "chroot"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
 def change_config(monkeypatch, path_config, key, value):
-    args = args_patched(monkeypatch, ["pmbootstrap.py", "-c", path_config, "config",
-                                      key, value])
+    args = args_patched(monkeypatch, ["pmbootstrap.py", "-c", path_config,
+                                      "config", key, value])
     pmb.helpers.frontend.config(args)
 
 
 def args_patched(monkeypatch, argv):
     monkeypatch.setattr(sys, "argv", argv)
     return pmb.parse.arguments()
 
@@ -55,19 +37,19 @@
 def test_config_user(args, tmpdir, monkeypatch):
     # Temporary paths
     tmpdir = str(tmpdir)
     path_work = tmpdir + "/work"
     path_config = tmpdir + "/pmbootstrap.cfg"
 
     # Generate default config (only uses tmpdir)
-    cmd = pmb.helpers.run.flat_cmd(["./pmbootstrap.py",
-                                    "-c", path_config,
-                                    "-w", path_work,
-                                    "--aports", args.aports,
-                                    "init"])
+    cmd = pmb.helpers.run_core.flat_cmd(["./pmbootstrap.py",
+                                         "-c", path_config,
+                                         "-w", path_work,
+                                         "--aports", args.aports,
+                                         "init"])
     pmb.helpers.run.user(args, ["sh", "-c", "yes '' | " + cmd],
                          pmb.config.pmb_src)
 
     # Load and verify default config
     argv = ["pmbootstrap.py", "-c", path_config, "config"]
     args_default = args_patched(monkeypatch, argv)
     assert args_default.work == path_work
```

### Comparing `pmbootstrap-1.9.0/test/test_aportgen_device_wizard.py` & `pmbootstrap-2.0.0/test/test_aportgen_device_wizard.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,164 +1,182 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
-import os
 import pytest
 import sys
+import shutil
 
-# Import from parent directory
-sys.path.insert(0, os.path.realpath(
-    os.path.join(os.path.dirname(__file__) + "/..")))
+import pmb_test  # noqa
+import pmb_test.git
+import pmb_test.const
 import pmb.aportgen
 import pmb.config
 import pmb.helpers.logging
 import pmb.parse
 
 
 @pytest.fixture
 def args(tmpdir, request):
-    sys.argv = ["pmbootstrap.py", "build", "-i", "device-testsuite-testdevice"]
+    cfg = f"{pmb_test.const.testdata}/channels.cfg"
+    sys.argv = ["pmbootstrap.py", "--config-channels", cfg, "build", "-i",
+                "device-testsuite-testdevice"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
 
     # Fake aports folder:
     tmpdir = str(tmpdir)
+    pmb_test.git.copy_dotgit(args, tmpdir)
     setattr(args, "_aports_real", args.aports)
     args.aports = tmpdir
 
     # Copy the devicepkg-dev package (shared device-* APKBUILD code)
     pmb.helpers.run.user(args, ["mkdir", "-p", tmpdir + "/main"])
     path_dev = args._aports_real + "/main/devicepkg-dev"
     pmb.helpers.run.user(args, ["cp", "-r", path_dev, tmpdir + "/main"])
 
     # Copy the linux-lg-mako aport (we currently copy patches from there)
-    pmb.helpers.run.user(args, ["mkdir", "-p", tmpdir + "/device"])
-    path_mako = args._aports_real + "/device/linux-lg-mako"
-    pmb.helpers.run.user(args, ["cp", "-r", path_mako, tmpdir + "/device"])
+    pmb.helpers.run.user(args, ["mkdir", "-p", tmpdir + "/device/testing"])
+    path_mako = args._aports_real + "/device/testing/linux-lg-mako"
+    pmb.helpers.run.user(args, ["cp", "-r", path_mako,
+                                f"{tmpdir}/device/testing"])
+
+    # Copy pmaports.cfg
+    shutil.copy(f"{pmb_test.const.testdata}/pmaports.cfg", args.aports)
     return args
 
 
 def generate(args, monkeypatch, answers):
     """
-    Generate the device-new-device and linux-new-device aports (with a patched pmb.helpers.cli()).
+    Generate the device-new-device and linux-new-device aports (with a patched
+    pmb.helpers.cli()).
 
     :returns: (deviceinfo, apkbuild, apkbuild_linux) - the parsed dictionaries
               of the created files, as returned by pmb.parse.apkbuild() and
               pmb.parse.deviceinfo().
     """
     # Patched function
-    def fake_ask(args, question="Continue?", choices=["y", "n"], default="n",
-                 lowercase_answer=True, validation_regex=None):
+    def fake_ask(question="Continue?", choices=["y", "n"], default="n",
+                 lowercase_answer=True, validation_regex=None, complete=None):
         for substr, answer in answers.items():
             if substr in question:
                 logging.info(question + ": " + answer)
                 # raise RuntimeError("test>" + answer)
                 return answer
         raise RuntimeError("This testcase didn't expect the question '" +
                            question + "', please add it to the mapping.")
 
     # Generate the aports
     monkeypatch.setattr(pmb.helpers.cli, "ask", fake_ask)
     pmb.aportgen.generate(args, "device-testsuite-testdevice")
     pmb.aportgen.generate(args, "linux-testsuite-testdevice")
     monkeypatch.undo()
 
-    # Parse the deviceinfo and apkbuilds
-    args.cache["apkbuild"] = {}
-    apkbuild_path = (args.aports + "/device/device-testsuite-testdevice/"
-                     "APKBUILD")
-    apkbuild_path_linux = (args.aports + "/device/"
+    apkbuild_path = (f"{args.aports}/device/testing/"
+                     "device-testsuite-testdevice/APKBUILD")
+    apkbuild_path_linux = (args.aports + "/device/testing/"
                            "linux-testsuite-testdevice/APKBUILD")
-    apkbuild = pmb.parse.apkbuild(args, apkbuild_path)
-    apkbuild_linux = pmb.parse.apkbuild(args, apkbuild_path_linux,
+
+    # The build fails if the email is not a valid email, so remove them just
+    # for tests
+    remove_contributor_maintainer_lines(args, apkbuild_path)
+    remove_contributor_maintainer_lines(args, apkbuild_path_linux)
+
+    # Parse the deviceinfo and apkbuilds
+    pmb.helpers.other.cache["apkbuild"] = {}
+    apkbuild = pmb.parse.apkbuild(apkbuild_path)
+    apkbuild_linux = pmb.parse.apkbuild(apkbuild_path_linux,
                                         check_pkgver=False)
     deviceinfo = pmb.parse.deviceinfo(args, "testsuite-testdevice")
     return (deviceinfo, apkbuild, apkbuild_linux)
 
 
+def remove_contributor_maintainer_lines(args, path):
+    with open(path, "r+", encoding="utf-8") as handle:
+        lines_new = []
+        for line in handle.readlines():
+            # Skip maintainer/contributor
+            if line.startswith("# Maintainer") or line.startswith(
+                    "# Contributor"):
+                continue
+            lines_new.append(line)
+        # Write back
+        handle.seek(0)
+        handle.write("".join(lines_new))
+        handle.truncate()
+
+
 def test_aportgen_device_wizard(args, monkeypatch):
     """
     Generate a device-testsuite-testdevice and linux-testsuite-testdevice
     package multiple times and check if the output is correct. Also build the
     device package once.
     """
     # Answers to interactive questions
     answers = {
-        "Device architecture": "armhf",
+        "Device architecture": "armv7",
         "external storage": "y",
         "hardware keyboard": "n",
         "Flash method": "heimdall",
         "Manufacturer": "Testsuite",
         "Name": "Testsuite Testdevice",
+        "Year": "1337",
+        "Chassis": "handset",
         "Type": "isorec",
     }
 
     # First run
     deviceinfo, apkbuild, apkbuild_linux = generate(args, monkeypatch, answers)
     assert apkbuild["pkgname"] == "device-testsuite-testdevice"
     assert apkbuild["pkgdesc"] == "Testsuite Testdevice"
-    assert apkbuild["depends"] == ["postmarketos-base",
-                                   "linux-testsuite-testdevice",
-                                   "mesa-dri-swrast"]
+    assert apkbuild["depends"] == ["linux-testsuite-testdevice",
+                                   "postmarketos-base"]
 
     assert apkbuild_linux["pkgname"] == "linux-testsuite-testdevice"
     assert apkbuild_linux["pkgdesc"] == "Testsuite Testdevice kernel fork"
-    assert apkbuild_linux["arch"] == ["armhf"]
+    assert apkbuild_linux["arch"] == ["armv7"]
     assert apkbuild_linux["_flavor"] == "testsuite-testdevice"
 
     assert deviceinfo["name"] == "Testsuite Testdevice"
     assert deviceinfo["manufacturer"] == answers["Manufacturer"]
-    assert deviceinfo["arch"] == "armhf"
+    assert deviceinfo["arch"] == "armv7"
+    assert deviceinfo["year"] == "1337"
+    assert deviceinfo["chassis"] == "handset"
     assert deviceinfo["keyboard"] == "false"
     assert deviceinfo["external_storage"] == "true"
     assert deviceinfo["flash_method"] == "heimdall-isorec"
     assert deviceinfo["generate_bootimg"] == ""
     assert deviceinfo["generate_legacy_uboot_initfs"] == ""
 
     # Build the device package
     pkgname = "device-testsuite-testdevice"
     pmb.build.checksum.update(args, pkgname)
-    pmb.build.package(args, pkgname, "armhf", force=True)
+    pmb.build.package(args, pkgname, "armv7", force=True)
 
     # Abort on overwrite confirmation
     answers["overwrite"] = "n"
     with pytest.raises(RuntimeError) as e:
         deviceinfo, apkbuild, apkbuild_linux = generate(args, monkeypatch,
                                                         answers)
     assert "Aborted." in str(e.value)
 
     # fastboot (mkbootimg)
     answers["overwrite"] = "y"
     answers["Flash method"] = "fastboot"
     answers["Path"] = ""
     deviceinfo, apkbuild, apkbuild_linux = generate(args, monkeypatch, answers)
-    assert apkbuild["depends"] == ["postmarketos-base",
-                                   "linux-testsuite-testdevice", "mkbootimg",
-                                   "mesa-dri-swrast"]
+    assert apkbuild["depends"] == ["linux-testsuite-testdevice",
+                                   "mkbootimg",
+                                   "postmarketos-base"]
+
     assert deviceinfo["flash_method"] == answers["Flash method"]
     assert deviceinfo["generate_bootimg"] == "true"
 
     # 0xffff (legacy uboot initfs)
     answers["Flash method"] = "0xffff"
     deviceinfo, apkbuild, apkbuild_linux = generate(args, monkeypatch, answers)
-    assert apkbuild["depends"] == ["postmarketos-base",
-                                   "linux-testsuite-testdevice", "uboot-tools",
-                                   "mesa-dri-swrast"]
+    assert apkbuild["depends"] == ["linux-testsuite-testdevice",
+                                   "postmarketos-base",
+                                   "uboot-tools"]
+
     assert deviceinfo["generate_legacy_uboot_initfs"] == "true"
```

### Comparing `pmbootstrap-1.9.0/test/test_helpers_package.py` & `pmbootstrap-2.0.0/test/test_helpers_package.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,132 +1,113 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import os
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import sys
 import pytest
 
-# Import from parent directory
-sys.path.insert(0, os.path.realpath(
-    os.path.join(os.path.dirname(__file__) + "/..")))
+import pmb_test  # noqa
 import pmb.helpers.logging
 import pmb.helpers.package
 
 
 @pytest.fixture
 def args(request):
     import pmb.parse
     sys.argv = ["pmbootstrap", "init"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
 def test_helpers_package_get_pmaports_and_cache(args, monkeypatch):
     """ Test pmb.helpers.package.get(): find in pmaports, use cached result """
 
     # Fake APKBUILD data
     def stub(args, pkgname, must_exist):
-        return {"arch": ["armhf"],
+        return {"arch": ["armv7"],
                 "depends": ["testdepend"],
                 "pkgname": "testpkgname",
                 "provides": ["testprovide"],
                 "options": [],
                 "checkdepends": [],
-                "subpackages": [],
+                "subpackages": {},
                 "makedepends": [],
                 "pkgver": "1.0",
                 "pkgrel": "1"}
     monkeypatch.setattr(pmb.helpers.pmaports, "get", stub)
 
-    package = {"arch": ["armhf"],
+    package = {"arch": ["armv7"],
                "depends": ["testdepend"],
                "pkgname": "testpkgname",
                "provides": ["testprovide"],
                "version": "1.0-r1"}
     func = pmb.helpers.package.get
-    assert func(args, "testpkgname", "armhf") == package
+    assert func(args, "testpkgname", "armv7") == package
 
     # Cached result
     monkeypatch.delattr(pmb.helpers.pmaports, "get")
-    assert func(args, "testpkgname", "armhf") == package
+    assert func(args, "testpkgname", "armv7") == package
 
 
 def test_helpers_package_get_apkindex(args, monkeypatch):
     """ Test pmb.helpers.package.get(): find in apkindex """
 
     # Fake APKINDEX data
-    fake_apkindex_data = {"arch": "armhf",
+    fake_apkindex_data = {"arch": "armv7",
                           "depends": ["testdepend"],
                           "pkgname": "testpkgname",
                           "provides": ["testprovide"],
                           "version": "1.0-r1"}
 
     def stub(args, pkgname, arch, must_exist):
         if arch != fake_apkindex_data["arch"]:
             return None
         return fake_apkindex_data
     monkeypatch.setattr(pmb.parse.apkindex, "package", stub)
 
     # Given arch
-    package = {"arch": ["armhf"],
+    package = {"arch": ["armv7"],
                "depends": ["testdepend"],
                "pkgname": "testpkgname",
                "provides": ["testprovide"],
                "version": "1.0-r1"}
     func = pmb.helpers.package.get
-    assert func(args, "testpkgname", "armhf") == package
+    assert func(args, "testpkgname", "armv7") == package
 
     # Other arch
     assert func(args, "testpkgname", "x86_64") == package
 
 
 def test_helpers_package_depends_recurse(args):
     """ Test pmb.helpers.package.depends_recurse() """
 
     # Put fake data into the pmb.helpers.package.get() cache
     cache = {"a": {False: {"pkgname": "a", "depends": ["b", "c"]}},
              "b": {False: {"pkgname": "b", "depends": []}},
              "c": {False: {"pkgname": "c", "depends": ["d"]}},
              "d": {False: {"pkgname": "d", "depends": ["b"]}}}
-    args.cache["pmb.helpers.package.get"]["armhf"] = cache
+    pmb.helpers.other.cache["pmb.helpers.package.get"]["armhf"] = cache
 
     # Normal runs
     func = pmb.helpers.package.depends_recurse
     assert func(args, "a", "armhf") == ["a", "b", "c", "d"]
     assert func(args, "d", "armhf") == ["b", "d"]
 
     # Cached result
-    args.cache["pmb.helpers.package.get"]["armhf"] = {}
+    pmb.helpers.other.cache["pmb.helpers.package.get"]["armhf"] = {}
     assert func(args, "d", "armhf") == ["b", "d"]
 
 
 def test_helpers_package_check_arch_package(args):
     """ Test pmb.helpers.package.check_arch(): binary = True """
     # Put fake data into the pmb.helpers.package.get() cache
     func = pmb.helpers.package.check_arch
     cache = {"a": {False: {"arch": []}}}
-    args.cache["pmb.helpers.package.get"]["armhf"] = cache
+    pmb.helpers.other.cache["pmb.helpers.package.get"]["armhf"] = cache
 
     cache["a"][False]["arch"] = ["all !armhf"]
     assert func(args, "a", "armhf") is False
 
     cache["a"][False]["arch"] = ["all"]
     assert func(args, "a", "armhf") is True
```

### Comparing `pmbootstrap-1.9.0/test/test_helpers_repo_missing.py` & `pmbootstrap-2.0.0/test/test_helpers_repo_missing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,24 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-import os
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import pytest
 import sys
 
-# Import from parent directory
-sys.path.insert(0, os.path.realpath(
-    os.path.join(os.path.dirname(__file__) + "/..")))
+import pmb_test  # noqa
 import pmb.build.other
 
 
 @pytest.fixture
 def args(request):
     import pmb.parse
     sys.argv = ["pmbootstrap", "init"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
 def test_filter_missing_packages_invalid(args):
     """ Test ...repo_missing.filter_missing_packages(): invalid package """
     func = pmb.helpers.repo_missing.filter_missing_packages
     with pytest.raises(RuntimeError) as e:
```

### Comparing `pmbootstrap-1.9.0/test/test_parse_apkindex.py` & `pmbootstrap-2.0.0/test/test_parse_apkindex.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,51 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-"""
-This file tests all functions from pmb.parse.apkindex.
-"""
-
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
+""" Test pmb.parse.apkindex """
 import collections
 import os
 import pytest
 import sys
 
-# Import from parent directory
-sys.path.insert(0, os.path.realpath(
-    os.path.join(os.path.dirname(__file__) + "/..")))
+import pmb_test  # noqa
 import pmb.parse.apkindex
 import pmb.helpers.logging
 import pmb.helpers.repo
 
 
 @pytest.fixture
 def args(tmpdir, request):
     import pmb.parse
     sys.argv = ["pmbootstrap", "init"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
-def test_parse_next_block_exceptions(args):
+def test_parse_next_block_exceptions():
     # Mapping of input files (inside the /test/testdata/apkindex) to
     # error message substrings
     mapping = {"key_twice": "specified twice",
                "key_missing": "Missing required key",
                "new_line_missing": "does not end with a new line!"}
 
     # Parse the files
     for file, error_substr in mapping.items():
         path = pmb.config.pmb_src + "/test/testdata/apkindex/" + file
         with open(path, "r", encoding="utf-8") as handle:
             lines = handle.readlines()
 
         with pytest.raises(RuntimeError) as e:
-            pmb.parse.apkindex.parse_next_block(args, path, lines, [0])
+            pmb.parse.apkindex.parse_next_block(path, lines, [0])
         assert error_substr in str(e.value)
 
 
-def test_parse_next_block_no_error(args):
+def test_parse_next_block_no_error():
     # Read the file
     func = pmb.parse.apkindex.parse_next_block
     path = pmb.config.pmb_src + "/test/testdata/apkindex/no_error"
     with open(path, "r", encoding="utf-8") as handle:
         lines = handle.readlines()
 
     # First block
@@ -75,37 +53,37 @@
     block = {'arch': 'x86_64',
              'depends': [],
              'origin': 'musl',
              'pkgname': 'musl',
              'provides': ['so:libc.musl-x86_64.so.1'],
              'timestamp': '1515217616',
              'version': '1.1.18-r5'}
-    assert func(args, path, lines, start) == block
+    assert func(path, lines, start) == block
     assert start == [24]
 
     # Second block
     block = {'arch': 'x86_64',
              'depends': ['ca-certificates',
                          'so:libc.musl-x86_64.so.1',
                          'so:libcurl.so.4',
                          'so:libz.so.1'],
              'origin': 'curl',
              'pkgname': 'curl',
              'provides': ['cmd:curl'],
              'timestamp': '1512030418',
              'version': '7.57.0-r0'}
-    assert func(args, path, lines, start) == block
+    assert func(path, lines, start) == block
     assert start == [45]
 
     # No more blocks
-    assert func(args, path, lines, start) is None
+    assert func(path, lines, start) is None
     assert start == [45]
 
 
-def test_parse_next_block_virtual(args):
+def test_parse_next_block_virtual():
     """
     Test parsing a virtual package from an APKINDEX.
     """
     # Read the file
     func = pmb.parse.apkindex.parse_next_block
     path = pmb.config.pmb_src + "/test/testdata/apkindex/virtual_package"
     with open(path, "r", encoding="utf-8") as handle:
@@ -116,31 +94,59 @@
     block = {'arch': 'x86_64',
              'depends': ['so:libc.musl-x86_64.so.1'],
              'origin': 'hello-world',
              'pkgname': 'hello-world',
              'provides': ['cmd:hello-world'],
              'timestamp': '1500000000',
              'version': '2-r0'}
-    assert func(args, path, lines, start) == block
+    assert func(path, lines, start) == block
     assert start == [20]
 
     # Second block: virtual package
     block = {'arch': 'noarch',
              'depends': ['hello-world'],
              'pkgname': '.pmbootstrap',
              'provides': [],
              'version': '0'}
-    assert func(args, path, lines, start) == block
+    assert func(path, lines, start) == block
     assert start == [31]
 
     # No more blocks
-    assert func(args, path, lines, start) is None
+    assert func(path, lines, start) is None
     assert start == [31]
 
 
+def test_parse_next_block_conflict():
+    """
+    Test parsing a package that specifies a conflicting dependency from an
+    APKINDEX.
+    """
+    # Read the file
+    func = pmb.parse.apkindex.parse_next_block
+    path = pmb.config.pmb_src + "/test/testdata/apkindex/conflict"
+    with open(path, "r", encoding="utf-8") as handle:
+        lines = handle.readlines()
+
+    # First block
+    start = [0]
+    block = {'arch': 'x86_64',
+             'depends': ['!conflict', 'so:libc.musl-x86_64.so.1'],
+             'origin': 'hello-world',
+             'pkgname': 'hello-world',
+             'provides': ['cmd:hello-world'],
+             'timestamp': '1500000000',
+             'version': '2-r0'}
+    assert func(path, lines, start) == block
+    assert start == [20]
+
+    # No more blocks
+    assert func(path, lines, start) is None
+    assert start == [20]
+
+
 def test_parse_add_block(args):
     func = pmb.parse.apkindex.parse_add_block
     multiple_providers = False
 
     # One package without alias
     ret = {}
     block = {"pkgname": "test", "version": "2"}
@@ -194,47 +200,47 @@
     alias = "test_alias"
     block_test2 = {"pkgname": "test2", "version": "1"}
     func(ret, block_test2, alias)
     assert ret == {"test": {"test": block_new},
                    "test_alias": {"test": block_new, "test2": block_test2}}
 
 
-def test_parse_invalid_path(args):
-    assert pmb.parse.apkindex.parse(args, "/invalid/path/APKINDEX") == {}
+def test_parse_invalid_path():
+    assert pmb.parse.apkindex.parse("/invalid/path/APKINDEX") == {}
 
 
 def test_parse_cached(args, tmpdir):
     # Create a real file (cache looks at the last modified date)
     path = str(tmpdir) + "/APKINDEX"
     pmb.helpers.run.user(args, ["touch", path])
     lastmod = os.path.getmtime(path)
 
     # Fill the cache
-    args.cache["apkindex"][path] = {
+    pmb.helpers.other.cache["apkindex"][path] = {
         "lastmod": lastmod,
         "multiple": "cached_result_multiple",
         "single": "cached_result_single",
     }
 
     # Verify cache usage
     func = pmb.parse.apkindex.parse
-    assert func(args, path, True) == "cached_result_multiple"
-    assert func(args, path, False) == "cached_result_single"
+    assert func(path, True) == "cached_result_multiple"
+    assert func(path, False) == "cached_result_single"
 
     # Make cache invalid
-    args.cache["apkindex"][path]["lastmod"] -= 10
-    assert func(args, path, True) == {}
+    pmb.helpers.other.cache["apkindex"][path]["lastmod"] -= 10
+    assert func(path, True) == {}
 
     # Delete the cache (run twice for both code paths)
-    assert pmb.parse.apkindex.clear_cache(args, path) is True
-    assert args.cache["apkindex"] == {}
-    assert pmb.parse.apkindex.clear_cache(args, path) is False
+    assert pmb.parse.apkindex.clear_cache(path) is True
+    assert pmb.helpers.other.cache["apkindex"] == {}
+    assert pmb.parse.apkindex.clear_cache(path) is False
 
 
-def test_parse(args):
+def test_parse():
     path = pmb.config.pmb_src + "/test/testdata/apkindex/no_error"
     block_musl = {'arch': 'x86_64',
                   'depends': [],
                   'origin': 'musl',
                   'pkgname': 'musl',
                   'provides': ['so:libc.musl-x86_64.so.1'],
                   'timestamp': '1515217616',
@@ -251,42 +257,44 @@
                   'version': '7.57.0-r0'}
 
     # Test without multiple_providers
     ret_single = {'cmd:curl': block_curl,
                   'curl': block_curl,
                   'musl': block_musl,
                   'so:libc.musl-x86_64.so.1': block_musl}
-    assert pmb.parse.apkindex.parse(args, path, False) == ret_single
-    assert args.cache["apkindex"][path]["single"] == ret_single
+    assert pmb.parse.apkindex.parse(path, False) == ret_single
+    assert pmb.helpers.other.cache["apkindex"][path]["single"] == ret_single
 
     # Test with multiple_providers
     ret_multiple = {'cmd:curl': {"curl": block_curl},
                     'curl': {"curl": block_curl},
                     'musl': {"musl": block_musl},
                     'so:libc.musl-x86_64.so.1': {"musl": block_musl}}
-    assert pmb.parse.apkindex.parse(args, path, True) == ret_multiple
-    assert args.cache["apkindex"][path]["multiple"] == ret_multiple
+    assert pmb.parse.apkindex.parse(path, True) == ret_multiple
+    assert (
+        pmb.helpers.other.cache["apkindex"][path]["multiple"] == ret_multiple
+    )
 
 
-def test_parse_virtual(args):
+def test_parse_virtual():
     """
     This APKINDEX contains a virtual package .pbmootstrap. It must not be part
     of the output.
     """
     path = pmb.config.pmb_src + "/test/testdata/apkindex/virtual_package"
     block = {'arch': 'x86_64',
              'depends': ['so:libc.musl-x86_64.so.1'],
              'origin': 'hello-world',
              'pkgname': 'hello-world',
              'provides': ['cmd:hello-world'],
              'timestamp': '1500000000',
              'version': '2-r0'}
     ret = {"hello-world": block, "cmd:hello-world": block}
-    assert pmb.parse.apkindex.parse(args, path, False) == ret
-    assert args.cache["apkindex"][path]["single"] == ret
+    assert pmb.parse.apkindex.parse(path, False) == ret
+    assert pmb.helpers.other.cache["apkindex"][path]["single"] == ret
 
 
 def test_providers_invalid_package(args, tmpdir):
     # Create empty APKINDEX
     path = str(tmpdir) + "/APKINDEX"
     pmb.helpers.run.user(args, ["touch", path])
 
@@ -306,26 +314,63 @@
     """
     In this test, we simulate 3 APKINDEX files ("i0", "i1", "i2" instead of
     full paths to real APKINDEX.tar.gz files), and each of them has a different
     version of the same package. The highest version must win, no matter in
     which order the APKINDEX files are processed.
     """
     # Fake parse function
-    def return_fake_parse(args, path):
+    def return_fake_parse(path):
         version_mapping = {"i0": "2", "i1": "3", "i2": "1"}
         package_block = {"pkgname": "test", "version": version_mapping[path]}
         return {"test": {"test": package_block}}
     monkeypatch.setattr(pmb.parse.apkindex, "parse", return_fake_parse)
 
     # Verify that it picks the highest version
     func = pmb.parse.apkindex.providers
     providers = func(args, "test", indexes=["i0", "i1", "i2"])
     assert providers["test"]["version"] == "3"
 
 
+def test_provider_highest_priority(args, monkeypatch):
+    # Verify that it picks the provider with highest priority
+    func = pmb.parse.apkindex.provider_highest_priority
+
+    provider_none_a = {"pkgname": "a", "provides": ["test"]}
+    provider_none_b = {"pkgname": "b", "provides": ["test"]}
+    provider_low_c = {"pkgname": "c", "provides": ["test"],
+                      "provider_priority": 42}
+    provider_low_d = {"pkgname": "d", "provides": ["test"],
+                      "provider_priority": 42}
+    provider_high = {"pkgname": "e", "provides": ["test"],
+                     "provider_priority": 1337}
+
+    # No provider has a priority
+    providers = {"a": provider_none_a}
+    assert func(providers, "test") == providers
+    providers = {"a": provider_none_a, "b": provider_none_b}
+    assert func(providers, "test") == providers
+
+    # One provider has a priority, another one does not
+    providers = {"a": provider_none_a, "e": provider_high}
+    assert func(providers, "test") == {"e": provider_high}
+
+    # One provider has a priority, another one has a higher priority
+    providers = {"c": provider_low_c, "e": provider_high}
+    assert func(providers, "test") == {"e": provider_high}
+
+    # One provider has a priority, another one has the same priority
+    providers = {"c": provider_low_c, "d": provider_low_d}
+    assert func(providers, "test") == providers
+
+    # + some package without priority at all should be filtered out
+    providers2 = providers.copy()
+    providers2["a"] = provider_none_a
+    assert func(providers2, "test") == providers
+
+
 def test_package(args, monkeypatch):
     # Override pmb.parse.apkindex.providers()
     providers = collections.OrderedDict()
 
     def return_providers(*args, **kwargs):
         return providers
     monkeypatch.setattr(pmb.parse.apkindex, "providers", return_providers)
```

### Comparing `pmbootstrap-1.9.0/test/test_build_package.py` & `pmbootstrap-2.0.0/test/test_build_package.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,34 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-"""
-This file tests all functions from pmb.build._package.
-"""
-
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
+""" Tests all functions from pmb.build._package """
 import datetime
 import glob
 import os
 import pytest
 import shutil
 import sys
 
-# Import from parent directory
-sys.path.insert(0, os.path.realpath(
-    os.path.join(os.path.dirname(__file__) + "/..")))
+import pmb_test  # noqa
+import pmb_test.git
 import pmb.build
 import pmb.build._package
 import pmb.config
 import pmb.config.init
 import pmb.helpers.logging
 
 
 @pytest.fixture
 def args(tmpdir, request):
     import pmb.parse
     sys.argv = ["pmbootstrap", "init"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
 def return_none(*args, **kwargs):
     return None
 
 
@@ -76,18 +55,18 @@
 def args_patched(monkeypatch, argv):
     monkeypatch.setattr(sys, "argv", argv)
     return pmb.parse.arguments()
 
 
 def test_skip_already_built(args):
     func = pmb.build._package.skip_already_built
-    assert args.cache["built"] == {}
-    assert func(args, "test-package", "armhf") is False
-    assert args.cache["built"] == {"armhf": ["test-package"]}
-    assert func(args, "test-package", "armhf") is True
+    assert pmb.helpers.other.cache["built"] == {}
+    assert func("test-package", "armhf") is False
+    assert pmb.helpers.other.cache["built"] == {"armhf": ["test-package"]}
+    assert func("test-package", "armhf") is True
 
 
 def test_get_apkbuild(args):
     func = pmb.build._package.get_apkbuild
 
     # Valid aport
     pkgname = "postmarketos-base"
@@ -132,15 +111,15 @@
                 "pkgrel": "0"}
     assert func(args, "mesa", "x86_64") is False
 
 
 def test_get_depends(monkeypatch):
     func = pmb.build._package.get_depends
     apkbuild = {"pkgname": "test", "depends": ["a"], "makedepends": ["c", "b"],
-                "checkdepends": "e", "subpackages": ["d"], "options": []}
+                "checkdepends": "e", "subpackages": {"d": None}, "options": []}
 
     # Depends + makedepends
     args = args_patched(monkeypatch, ["pmbootstrap", "build", "test"])
     assert func(args, apkbuild) == ["a", "b", "c", "e"]
     args = args_patched(monkeypatch, ["pmbootstrap", "install"])
     assert func(args, apkbuild) == ["a", "b", "c", "e"]
 
@@ -158,31 +137,33 @@
     args = args_patched(monkeypatch, ["pmbootstrap", "build", "test"])
     assert func(args, apkbuild) == ["a", "b", "c", "e"]
 
 
 def test_build_depends(args, monkeypatch):
     # Shortcut and fake apkbuild
     func = pmb.build._package.build_depends
-    apkbuild = {"pkgname": "test", "depends": ["a"], "makedepends": ["b"],
-                "checkdepends": [], "subpackages": ["d"], "options": []}
+    apkbuild = {"pkgname": "test", "depends": ["a", "!c"],
+                "makedepends": ["b"], "checkdepends": [],
+                "subpackages": {"d": None}, "options": []}
 
     # No depends built (first makedepends + depends, then only makedepends)
     monkeypatch.setattr(pmb.build._package, "package", return_none)
-    assert func(args, apkbuild, "armhf", True) == (["a", "b"], [])
+    assert func(args, apkbuild, "armhf", True) == (["!c", "a", "b"], [])
 
     # All depends built (makedepends only)
     monkeypatch.setattr(pmb.build._package, "package", return_string)
-    assert func(args, apkbuild, "armhf", False) == (["a", "b"], ["a", "b"])
+    assert func(args, apkbuild, "armhf", False) == (["!c", "a", "b"],
+                                                    ["a", "b"])
 
 
 def test_build_depends_no_binary_error(args, monkeypatch):
     # Shortcut and fake apkbuild
     func = pmb.build._package.build_depends
     apkbuild = {"pkgname": "test", "depends": ["some-invalid-package-here"],
-                "makedepends": [], "checkdepends": [], "subpackages": [],
+                "makedepends": [], "checkdepends": [], "subpackages": {},
                 "options": []}
 
     # pmbootstrap build --no-depends
     args.no_depends = True
 
     # Missing binary package error
     with pytest.raises(RuntimeError) as e:
@@ -190,14 +171,45 @@
     assert str(e.value).startswith("Missing binary package for dependency")
 
     # All depends exist
     apkbuild["depends"] = ["alpine-base"]
     assert func(args, apkbuild, "armhf", True) == (["alpine-base"], [])
 
 
+def test_build_depends_binary_outdated(args, monkeypatch):
+    """ pmbootstrap runs with --no-depends and dependency binary package is
+        outdated (#1895) """
+    # Override pmb.parse.apkindex.package(): pretend hello-world-wrapper is
+    # missing and hello-world is outdated
+    func_orig = pmb.parse.apkindex.package
+
+    def func_patch(args, package, *args2, **kwargs):
+        print(f"func_patch: called for package: {package}")
+        if package == "hello-world-wrapper":
+            print("pretending that it does not exist")
+            return None
+        if package == "hello-world":
+            print("pretending that it is outdated")
+            ret = func_orig(args, package, *args2, **kwargs)
+            ret["version"] = "0-r0"
+            return ret
+        return func_orig(args, package, *args2, **kwargs)
+    monkeypatch.setattr(pmb.parse.apkindex, "package", func_patch)
+
+    # Build hello-world-wrapper with --no-depends and expect failure
+    args.no_depends = True
+    pkgname = "hello-world-wrapper"
+    arch = "x86_64"
+    force = False
+    strict = True
+    with pytest.raises(RuntimeError) as e:
+        pmb.build.package(args, pkgname, arch, force, strict)
+    assert "'hello-world' of 'hello-world-wrapper' is outdated" in str(e.value)
+
+
 def test_is_necessary_warn_depends(args, monkeypatch):
     # Shortcut and fake apkbuild
     func = pmb.build._package.is_necessary_warn_depends
     apkbuild = {"pkgname": "test"}
 
     # Necessary
     monkeypatch.setattr(pmb.build, "is_necessary", return_true)
@@ -218,24 +230,23 @@
 
     # Disable effects of functions we don't want to test here
     monkeypatch.setattr(pmb.build._package, "build_depends",
                         return_fake_build_depends)
     monkeypatch.setattr(pmb.build._package, "is_necessary_warn_depends",
                         return_true)
     monkeypatch.setattr(pmb.chroot.apk, "install", return_none)
-    monkeypatch.setattr(pmb.chroot.distccd, "start", return_none)
 
     # Shortcut and fake apkbuild
     func = pmb.build._package.init_buildenv
-    apkbuild = {"pkgname": "test", "depends": ["a"], "makedepends": ["b"], "options": []}
+    apkbuild = {"pkgname": "test", "depends": ["a"], "makedepends": ["b"],
+                "options": []}
 
     # Build is necessary (various code paths)
     assert func(args, apkbuild, "armhf", strict=True) is True
     assert func(args, apkbuild, "armhf", cross="native") is True
-    assert func(args, apkbuild, "armhf", cross="distcc") is True
 
     # Build is not necessary (only builds dependencies)
     monkeypatch.setattr(pmb.build._package, "is_necessary_warn_depends",
                         return_false)
     assert func(args, apkbuild, "armhf") is False
 
 
@@ -257,40 +268,33 @@
 
     # Shortcut and fake apkbuild
     func = pmb.build._package.run_abuild
     apkbuild = {"pkgname": "test", "pkgver": "1", "pkgrel": "2", "options": []}
 
     # Normal run
     output = "armhf/test-1-r2.apk"
-    env = {"CARCH": "armhf", "SUDO_APK": "abuild-apk --no-progress"}
+    env = {"CARCH": "armhf",
+           "GOCACHE": "/home/pmos/.cache/go-build",
+           "SUDO_APK": "abuild-apk --no-progress"}
     cmd = ["abuild", "-D", "postmarketOS", "-d"]
     assert func(args, apkbuild, "armhf") == (output, cmd, env)
 
     # Force and strict
     cmd = ["abuild", "-D", "postmarketOS", "-r", "-f"]
     assert func(args, apkbuild, "armhf", True, True) == (output, cmd, env)
 
     # cross=native
     env = {"CARCH": "armhf",
+           "GOCACHE": "/home/pmos/.cache/go-build",
            "SUDO_APK": "abuild-apk --no-progress",
            "CROSS_COMPILE": "armv6-alpine-linux-musleabihf-",
            "CC": "armv6-alpine-linux-musleabihf-gcc"}
     cmd = ["abuild", "-D", "postmarketOS", "-d"]
     assert func(args, apkbuild, "armhf", cross="native") == (output, cmd, env)
 
-    # cross=distcc
-    (output, cmd, env) = func(args, apkbuild, "armhf", cross="distcc")
-    assert output == "armhf/test-1-r2.apk"
-    assert env["CARCH"] == "armhf"
-    assert env["CCACHE_PREFIX"] == "distcc"
-    assert env["CCACHE_PATH"] == "/usr/lib/arch-bin-masquerade/armhf:/usr/bin"
-    assert env["CCACHE_COMPILERCHECK"].startswith("string:")
-    assert env["DISTCC_HOSTS"] == "@127.0.0.1:/home/pmos/.distcc-sshd/distccd"
-    assert env["DISTCC_BACKOFF_PERIOD"] == "0"
-
 
 def test_finish(args, monkeypatch):
     # Real output path
     output = pmb.build.package(args, "hello-world", force=True)
 
     # Disable effects of functions we don't want to test below
     monkeypatch.setattr(pmb.chroot, "user", return_none)
@@ -301,27 +305,27 @@
 
     # Non-existing output path
     with pytest.raises(RuntimeError) as e:
         func(args, apkbuild, "armhf", "/invalid/path")
     assert "Package not found" in str(e.value)
 
     # Existing output path
-    func(args, apkbuild, args.arch_native, output)
+    func(args, apkbuild, pmb.config.arch_native, output)
 
 
 def test_package(args):
     # First build
     assert pmb.build.package(args, "hello-world", force=True)
 
     # Package exists
-    args.cache["built"] = {}
+    pmb.helpers.other.cache["built"] = {}
     assert pmb.build.package(args, "hello-world") is None
 
     # Force building again
-    args.cache["built"] = {}
+    pmb.helpers.other.cache["built"] = {}
     assert pmb.build.package(args, "hello-world", force=True)
 
     # Build for another architecture
     assert pmb.build.package(args, "hello-world", "armhf", force=True)
 
     # Upstream package, for which we don't have an aport
     assert pmb.build.package(args, "alpine-base") is None
@@ -338,76 +342,79 @@
             return True
         return pmb.build.other.is_necessary(args, arch, apkbuild,
                                             apkindex_path)
     monkeypatch.setattr(pmb.build, "is_necessary",
                         fake_build_is_necessary)
 
     # Build hello-world to get its full output path
+    channel = pmb.config.pmaports.read_config(args)["channel"]
     output_hello = pmb.build.package(args, "hello-world")
-    output_hello_outside = args.work + "/packages/" + output_hello
+    output_hello_outside = f"{args.work}/packages/{channel}/{output_hello}"
     assert os.path.exists(output_hello_outside)
 
     # Make sure the wrapper exists
     pmb.build.package(args, "hello-world-wrapper")
 
     # Remove hello-world
     pmb.helpers.run.root(args, ["rm", output_hello_outside])
-    pmb.build.index_repo(args, args.arch_native)
-    args.cache["built"] = {}
+    pmb.build.index_repo(args, pmb.config.arch_native)
+    pmb.helpers.other.cache["built"] = {}
 
     # Ask to build the wrapper. It should not build the wrapper (it exists, not
     # using force), but build/update its missing dependency "hello-world"
     # instead.
     assert pmb.build.package(args, "hello-world-wrapper") is None
     assert os.path.exists(output_hello_outside)
 
 
 def test_build_local_source_high_level(args, tmpdir):
     """
     Test building a package with overriding the source code:
         pmbootstrap build --src=/some/path hello-world
 
-    We use a copy of the hello-world APKBUILD here, that doesn't have the
+    We use a copy of the hello-world APKBUILD here that doesn't have the
     source files it needs to build included. And we use the original aport
     folder as local source folder, so pmbootstrap should take the source files
     from there and the build should succeed.
     """
     # aports: Add deviceinfo (required by pmbootstrap to start)
     tmpdir = str(tmpdir)
     aports = tmpdir + "/aports"
-    aport = aports + "/device/device-" + args.device
+    aport = aports + "/device/testing/device-" + args.device
     os.makedirs(aport)
-    shutil.copy(args.aports + "/device/device-" + args.device + "/deviceinfo",
-                aport)
+    path_original = pmb.helpers.pmaports.find(args, f"device-{args.device}")
+    shutil.copy(f"{path_original}/deviceinfo", aport)
 
     # aports: Add modified hello-world aport (source="", uses $builddir)
     aport = aports + "/main/hello-world"
     os.makedirs(aport)
     shutil.copy(pmb.config.pmb_src + "/test/testdata/build_local_src/APKBUILD",
                 aport)
 
-    # aports: Add pmaports.cfg
+    # aports: Add pmaports.cfg, .git
     shutil.copy(args.aports + "/pmaports.cfg", aports)
+    pmb_test.git.copy_dotgit(args, tmpdir)
 
     # src: Copy hello-world source files
     src = tmpdir + "/src"
     os.makedirs(src)
     shutil.copy(args.aports + "/main/hello-world/Makefile", src)
     shutil.copy(args.aports + "/main/hello-world/main.c", src)
 
     # src: Create unreadable file (rsync should skip it)
     unreadable = src + "/_unreadable_file"
     shutil.copy(args.aports + "/main/hello-world/main.c", unreadable)
     pmb.helpers.run.root(args, ["chown", "root:root", unreadable])
     pmb.helpers.run.root(args, ["chmod", "500", unreadable])
 
     # Test native arch and foreign arch chroot
-    for arch in [args.arch_native, "armhf"]:
+    channel = pmb.config.pmaports.read_config(args)["channel"]
+    for arch in [pmb.config.arch_native, "armhf"]:
         # Delete all hello-world --src packages
-        pattern = args.work + "/packages/" + arch + "/hello-world-*_p*.apk"
+        pattern = f"{args.work}/packages/{channel}/{arch}/hello-world-*_p*.apk"
         for path in glob.glob(pattern):
             pmb.helpers.run.root(args, ["rm", path])
         assert len(glob.glob(pattern)) == 0
 
         # Build hello-world --src package
         pmb.helpers.run.user(args, [pmb.config.pmb_src + "/pmbootstrap.py",
                                     "--aports", aports, "build", "--src", src,
@@ -415,9 +422,60 @@
 
         # Verify that the package has been built and delete it
         paths = glob.glob(pattern)
         assert len(paths) == 1
         pmb.helpers.run.root(args, ["rm", paths[0]])
 
     # Clean up: update index, delete temp folder
-    pmb.build.index_repo(args, args.arch_native)
+    pmb.build.index_repo(args, pmb.config.arch_native)
+    pmb.helpers.run.root(args, ["rm", "-r", tmpdir])
+
+
+def test_build_abuild_leftovers(args, tmpdir):
+    """
+    Test building a package with having abuild leftovers, that will error if
+    copied:
+        pmbootstrap build hello-world
+    """
+    # aports: Add deviceinfo (required by pmbootstrap to start)
+    tmpdir = str(tmpdir)
+    aports = f"{tmpdir}/aports"
+    aport = f"{aports}/device/testing/device-{args.device}"
+    os.makedirs(aport)
+    path_original = pmb.helpers.pmaports.find(args, f"device-{args.device}")
+    shutil.copy(f"{path_original}/deviceinfo", aport)
+
+    # aports: Add modified hello-world aport (source="", uses $builddir)
+    test_aport = "main/hello-world"
+    aport = f"{aports}/{test_aport}"
+    shutil.copytree(f"{args.aports}/{test_aport}", aport)
+
+    # aports: Add pmaports.cfg, .git
+    shutil.copy(f"{args.aports}/pmaports.cfg", aports)
+    pmb_test.git.copy_dotgit(args, aports)
+
+    # aport: create abuild dir with broken symlink
+    src = f"{aport}/src"
+    os.makedirs(src)
+    os.symlink("/var/cache/distfiles/non-existent.tar.gz",
+               f"{src}/broken-tarball-symlink.tar.gz")
+
+    # Delete all hello-world packages
+    channel = pmb.config.pmaports.read_config(args)["channel"]
+    pattern = f"{args.work}/packages/{channel}/*/hello-world-*_p*.apk"
+    for path in glob.glob(pattern):
+        pmb.helpers.run.root(args, ["rm", path])
+    assert len(glob.glob(pattern)) == 0
+
+    # Build hello-world package
+    pmb.helpers.run.user(args, [f"{pmb.config.pmb_src}/pmbootstrap.py",
+                                "--aports", aports, "build", "--src", src,
+                                "hello-world", "--arch", pmb.config.arch_native])
+
+    # Verify that the package has been built and delete it
+    paths = glob.glob(pattern)
+    assert len(paths) == 1
+    pmb.helpers.run.root(args, ["rm", paths[0]])
+
+    # Clean up: update index, delete temp folder
+    pmb.build.index_repo(args, pmb.config.arch_native)
     pmb.helpers.run.root(args, ["rm", "-r", tmpdir])
```

### Comparing `pmbootstrap-1.9.0/test/test_pkgrel_bump.py` & `pmbootstrap-2.0.0/test/test_pkgrel_bump.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,55 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-"""
-This file tests pmb.helper.pkgrel_bump
-"""
-
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
+""" Test pmb.helper.pkgrel_bump """
 import glob
 import os
 import pytest
 import sys
 
-# Import from parent directory
-pmb_src = os.path.realpath(os.path.join(os.path.dirname(__file__) + "/.."))
-sys.path.insert(0, pmb_src)
+import pmb_test  # noqa
+import pmb_test.git
 import pmb.helpers.pkgrel_bump
 import pmb.helpers.logging
 
 
 @pytest.fixture
 def args(request):
     import pmb.parse
     sys.argv = ["pmbootstrap.py", "chroot"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
 def pmbootstrap(args, tmpdir, parameters, zero_exit=True):
     """
-    Helper function for running pmbootstrap inside the fake work folder (created
-    by setup() below) with the binary repo disabled and with the testdata
-    configured as aports.
+    Helper function for running pmbootstrap inside the fake work folder
+    (created by setup() below) with the binary repo disabled and with the
+    testdata configured as aports.
 
     :param parameters: what to pass to pmbootstrap, e.g. ["build", "testlib"]
     :param zero_exit: expect pmbootstrap to exit with 0 (no error)
     """
     # Run pmbootstrap
     aports = tmpdir + "/_aports"
     config = tmpdir + "/_pmbootstrap.cfg"
 
+    # Copy .git dir to fake pmaports
+    dot_git = tmpdir + "/_aports/.git"
+    if not os.path.exists(dot_git):
+        pmb_test.git.copy_dotgit(args, aports)
+
     try:
         pmb.helpers.run.user(args, ["./pmbootstrap.py", "--work=" + tmpdir,
                                     "--mirror-pmOS=", "--aports=" + aports,
                                     "--config=" + config] + parameters,
-                             working_dir=pmb_src)
+                             working_dir=pmb.config.pmb_src)
 
     # Verify that it exits as desired
     except Exception as exc:
         if zero_exit:
             raise RuntimeError("pmbootstrap failed") from exc
         else:
             return
@@ -76,103 +60,112 @@
 def setup_work(args, tmpdir):
     """
     Create fake work folder in tmpdir with everything symlinked except for the
     built packages. The aports testdata gets copied to the tempfolder as
     well, so it can be modified during testing.
     """
     # Clean the chroots, and initialize the build chroot in the native chroot.
-    # We do this before creating the fake work folder, because then all packages
-    # are still present.
-    os.chdir(pmb_src)
+    # We do this before creating the fake work folder, because then all
+    # packages are still present.
+    os.chdir(pmb.config.pmb_src)
     pmb.helpers.run.user(args, ["./pmbootstrap.py", "-y", "zap"])
     pmb.helpers.run.user(args, ["./pmbootstrap.py", "build_init"])
     pmb.helpers.run.user(args, ["./pmbootstrap.py", "shutdown"])
 
     # Link everything from work (except for "packages") to the tmpdir
     for path in glob.glob(args.work + "/*"):
         if os.path.basename(path) != "packages":
             pmb.helpers.run.user(args, ["ln", "-s", path, tmpdir + "/"])
 
     # Copy testdata and selected device aport
-    for folder in ["device", "main"]:
+    for folder in ["device/testing", "main"]:
         pmb.helpers.run.user(args, ["mkdir", "-p", args.aports, tmpdir +
                                     "/_aports/" + folder])
-    pmb.helpers.run.user(args, ["cp", "-r", args.aports + "/device/device-" +
-                                args.device, tmpdir + "/_aports/device"])
+    path_original = pmb.helpers.pmaports.find(args, f"device-{args.device}")
+    pmb.helpers.run.user(args, ["cp", "-r", path_original,
+                                f"{tmpdir}/_aports/device/testing"])
     for pkgname in ["testlib", "testapp", "testsubpkg"]:
         pmb.helpers.run.user(args, ["cp", "-r",
-                                    "test/testdata/pkgrel_bump/aports/" + pkgname,
-                                    tmpdir + "/_aports/main/" + pkgname])
+                                    "test/testdata/pkgrel_bump/aports/"
+                                    f"{pkgname}",
+                                    f"{tmpdir}/_aports/main/{pkgname}"])
 
     # Copy pmaports.cfg
     pmb.helpers.run.user(args, ["cp", args.aports + "/pmaports.cfg", tmpdir +
                                 "/_aports"])
 
     # Empty packages folder
-    pmb.helpers.run.user(args, ["mkdir", "-p", tmpdir + "/packages"])
-    pmb.helpers.run.user(args, ["chmod", "777", tmpdir + "/packages"])
+    channel = pmb.config.pmaports.read_config(args)["channel"]
+    packages_path = f"{tmpdir}/packages/{channel}"
+    pmb.helpers.run.user(args, ["mkdir", "-p", packages_path])
+    pmb.helpers.run.user(args, ["chmod", "777", packages_path])
 
     # Copy over the pmbootstrap config
     pmb.helpers.run.user(args, ["cp", args.config, tmpdir +
                                 "/_pmbootstrap.cfg"])
 
 
-def verify_pkgrels(args, tmpdir, pkgrel_testlib, pkgrel_testapp,
+def verify_pkgrels(tmpdir, pkgrel_testlib, pkgrel_testapp,
                    pkgrel_testsubpkg):
     """
     Verify the pkgrels of the three test APKBUILDs ("testlib", "testapp",
     "testsubpkg").
     """
-    args.cache["apkbuild"] = {}
+    pmb.helpers.other.cache["apkbuild"] = {}
     mapping = {"testlib": pkgrel_testlib,
                "testapp": pkgrel_testapp,
                "testsubpkg": pkgrel_testsubpkg}
     for pkgname, pkgrel in mapping.items():
         # APKBUILD path
         path = tmpdir + "/_aports/main/" + pkgname + "/APKBUILD"
 
         # Parse and verify
-        apkbuild = pmb.parse.apkbuild(args, path)
+        apkbuild = pmb.parse.apkbuild(path)
         assert pkgrel == int(apkbuild["pkgrel"])
 
 
 def test_pkgrel_bump_high_level(args, tmpdir):
     # Tempdir setup
     tmpdir = str(tmpdir)
     setup_work(args, tmpdir)
 
+    # Make sure we don't try and cross compile
+    pmbootstrap(args, tmpdir, ["config", "build_default_device_arch", "False"])
+
     # Let pkgrel_bump exit normally
     pmbootstrap(args, tmpdir, ["build", "testlib", "testapp", "testsubpkg"])
     pmbootstrap(args, tmpdir, ["pkgrel_bump", "--dry", "--auto"])
-    verify_pkgrels(args, tmpdir, 0, 0, 0)
+    verify_pkgrels(tmpdir, 0, 0, 0)
 
     # Increase soname (testlib soname changes with the pkgrel)
     pmbootstrap(args, tmpdir, ["pkgrel_bump", "testlib"])
-    verify_pkgrels(args, tmpdir, 1, 0, 0)
+    verify_pkgrels(tmpdir, 1, 0, 0)
     pmbootstrap(args, tmpdir, ["build", "testlib"])
     pmbootstrap(args, tmpdir, ["pkgrel_bump", "--dry", "--auto"])
-    verify_pkgrels(args, tmpdir, 1, 0, 0)
+    verify_pkgrels(tmpdir, 1, 0, 0)
 
     # Delete package with previous soname (--auto-dry exits with >0 now)
-    pmb.helpers.run.root(args, ["rm", tmpdir + "/packages/" +
-                                args.arch_native + "/testlib-1.0-r0.apk"])
+    channel = pmb.config.pmaports.read_config(args)["channel"]
+    arch = pmb.config.arch_native
+    apk_path = f"{tmpdir}/packages/{channel}/{arch}/testlib-1.0-r0.apk"
+    pmb.helpers.run.root(args, ["rm", apk_path])
     pmbootstrap(args, tmpdir, ["index"])
     pmbootstrap(args, tmpdir, ["pkgrel_bump", "--dry", "--auto"], False)
-    verify_pkgrels(args, tmpdir, 1, 0, 0)
+    verify_pkgrels(tmpdir, 1, 0, 0)
 
     # Bump pkgrel and build testapp/testsubpkg
     pmbootstrap(args, tmpdir, ["pkgrel_bump", "--auto"])
-    verify_pkgrels(args, tmpdir, 1, 1, 1)
+    verify_pkgrels(tmpdir, 1, 1, 1)
     pmbootstrap(args, tmpdir, ["build", "testapp", "testsubpkg"])
 
     # After rebuilding, pkgrel_bump --auto-dry exits with 0
     pmbootstrap(args, tmpdir, ["pkgrel_bump", "--dry", "--auto"])
-    verify_pkgrels(args, tmpdir, 1, 1, 1)
+    verify_pkgrels(tmpdir, 1, 1, 1)
 
     # Test running with specific package names
     pmbootstrap(args, tmpdir, ["pkgrel_bump", "invalid_package_name"], False)
     pmbootstrap(args, tmpdir, ["pkgrel_bump", "--dry", "testlib"], False)
-    verify_pkgrels(args, tmpdir, 1, 1, 1)
+    verify_pkgrels(tmpdir, 1, 1, 1)
 
     # Clean up
     pmbootstrap(args, tmpdir, ["shutdown"])
     pmb.helpers.run.root(args, ["rm", "-rf", tmpdir])
```

### Comparing `pmbootstrap-1.9.0/test/test_keys.py` & `pmbootstrap-2.0.0/test/test_zzz_keys.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,40 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
+# This file has a _zzz_ prefix so it runs last, because it tends to fail on
+# sourcehut currently. Related to some CDN caching issue probably.
 import os
 import sys
 import pytest
 import glob
 import filecmp
 
-# Import from parent directory
-sys.path.insert(0, os.path.realpath(
-    os.path.join(os.path.dirname(__file__) + "/..")))
+import pmb_test  # noqa
 import pmb.parse.apkindex
 import pmb.helpers.logging
 import pmb.config
 
 
 @pytest.fixture
 def args(request):
     import pmb.parse
     sys.argv = ["pmbootstrap.py", "chroot"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
 def test_keys(args):
     # Get the alpine-keys apk filename
     pmb.chroot.init(args)
     version = pmb.parse.apkindex.package(args, "alpine-keys")["version"]
-    pattern = (args.work + "/cache_apk_" + args.arch_native + "/alpine-keys-" +
-               version + ".*.apk")
+    pattern = (args.work + "/cache_apk_" + pmb.config.arch_native +
+               "/alpine-keys-" + version + ".*.apk")
     filename = os.path.basename(glob.glob(pattern)[0])
 
     # Extract it to a temporary folder
     temp = "/tmp/test_keys_extract"
     temp_outside = args.work + "/chroot_native" + temp
     if os.path.exists(temp_outside):
         pmb.chroot.root(args, ["rm", "-r", temp])
@@ -69,15 +53,15 @@
     # Check if the keys are mirrored correctly
     mirror_path_keys = pmb.config.apk_keys_path
     for key, original_path in keys_upstream.items():
         mirror_path = mirror_path_keys + "/" + key
         assert filecmp.cmp(mirror_path, original_path, False)
 
     # Find postmarketOS keys
-    keys_pmos = ["pmos-5a03a13a.rsa.pub"]
+    keys_pmos = ["build.postmarketos.org.rsa.pub"]
     for key in keys_pmos:
         assert os.path.exists(mirror_path_keys + "/" + key)
 
     # Find outdated keys, which need to be removed
     glob_result = glob.glob(mirror_path_keys + "/*.pub")
     assert len(glob_result)
     for path in glob_result:
```

### Comparing `pmbootstrap-1.9.0/test/test_run_core.py` & `pmbootstrap-2.0.0/test/test_run_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,29 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-"""
-This file tests functions from pmb.helpers.run_core
-"""
-
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
+""" Test pmb.helpers.run_core """
 import os
-import sys
-import subprocess
 import pytest
+import re
+import subprocess
+import sys
+import time
 
-# Import from parent directory
-pmb_src = os.path.realpath(os.path.join(os.path.dirname(__file__) + "/.."))
-sys.path.insert(0, pmb_src)
+import pmb_test  # noqa
 import pmb.helpers.run_core
 
 
 @pytest.fixture
 def args(request):
     import pmb.parse
     sys.argv = ["pmbootstrap.py", "chroot"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
 def test_sanity_checks():
     func = pmb.helpers.run_core.sanity_checks
 
     # Invalid output
@@ -60,29 +40,37 @@
 
     # output_return
     func("log", output_return=True)
     with pytest.raises(RuntimeError) as e:
         func("tui", output_return=True)
     assert str(e.value).startswith("Can't use output_return with")
 
-    # kill_as_root
-    func("log", kill_as_root=True)
-    with pytest.raises(RuntimeError) as e:
-        func("tui", kill_as_root=True)
-    assert str(e.value).startswith("Can't use kill_as_root with")
-
 
 def test_background(args):
     # Sleep in background
-    process = pmb.helpers.run_core.background(args, ["sleep", "1"], "/")
+    process = pmb.helpers.run_core.background(["sleep", "1"], "/")
 
     # Check if it is still running
     assert process.poll() is None
 
 
+def test_pipe(args):
+    # Sleep in background
+    process = pmb.helpers.run_core.pipe(["sleep", "1"], "/")
+
+    # Check if it is still running
+    assert process.poll() is None
+
+    # Print output in background
+    process = pmb.helpers.run_core.pipe(["echo", "-n", "hello"], "/")
+
+    # Read output
+    assert process.communicate()[0].decode('utf-8') == "hello"
+
+
 def test_foreground_pipe(args):
     func = pmb.helpers.run_core.foreground_pipe
     cmd = ["echo", "test"]
 
     # Normal run
     assert func(args, cmd) == (0, "")
 
@@ -92,41 +80,43 @@
     # Kill with output timeout
     cmd = ["sh", "-c", "echo first; sleep 2; echo second"]
     args.timeout = 0.3
     ret = func(args, cmd, output_return=True, output_timeout=True)
     assert ret == (-9, "first\n")
 
     # Kill with output timeout as root
-    cmd = ["sudo", "sh", "-c", "printf first; sleep 2; printf second"]
+    cmd = pmb.config.sudo(["sh", "-c", "printf first; sleep 2; printf second"])
     args.timeout = 0.3
     ret = func(args, cmd, output_return=True, output_timeout=True,
-               kill_as_root=True)
+               sudo=True)
     assert ret == (-9, "first")
 
     # Finish before timeout
     cmd = ["sh", "-c", "echo first; sleep 0.1; echo second; sleep 0.1;"
            "echo third; sleep 0.1; echo fourth"]
     args.timeout = 0.2
     ret = func(args, cmd, output_return=True, output_timeout=True)
     assert ret == (0, "first\nsecond\nthird\nfourth\n")
 
     # Check if all child processes are killed after timeout.
     # The first command uses ps to get its process group id (pgid) and echo it
     # to stdout. All of the test commands will be running under that pgid.
-    cmd = ["sudo", "sh", "-c",
-           "pgid=$(ps -p ${1:-$$} -o pgid=);echo $pgid | tr -d '\n';" +
-           "sleep 10 | sleep 20 | sleep 30"]
+    cmd = pmb.config.sudo([
+        "sh", "-c",
+        "pgid=$(ps -o pgid= | grep ^${1:-$$});echo $pgid | tr -d '\n';"
+        "sleep 10 | sleep 20 | sleep 30"
+    ])
     args.timeout = 0.3
     ret = func(args, cmd, output_return=True, output_timeout=True,
-               kill_as_root=True)
+               sudo=True)
     pgid = str(ret[1])
 
-    cmd = ["ps", "-e", "-o", "pgid=,comm=", "--noheaders"]
+    cmd = ["ps", "-e", "-o", "pgid,comm"]
     ret = subprocess.run(cmd, check=True, stdout=subprocess.PIPE)
-    procs = str(ret.stdout.decode("utf-8")).rstrip().split('\n')
+    procs = str(ret.stdout.decode("utf-8")).rstrip().split('\n')[1:]
     child_procs = []
     for process in procs:
         items = process.split(maxsplit=1)
         if len(items) != 2:
             continue
         if pgid == items[0] and "sleep" in items[1]:
             child_procs.append(items)
@@ -134,15 +124,15 @@
 
 
 def test_foreground_tui():
     func = pmb.helpers.run_core.foreground_tui
     assert func(["echo", "test"]) == 0
 
 
-def test_core(args):
+def test_core(args, monkeypatch):
     # Background
     func = pmb.helpers.run_core.core
     msg = "test"
     process = func(args, msg, ["sleep", "1"], output="background")
     assert process.poll() is None
 
     # Foreground (TUI)
@@ -156,14 +146,30 @@
     # Return output
     ret = func(args, msg, ["echo", "test"], output="log", output_return=True)
     assert ret == "test\n"
 
     # Check the return code
     with pytest.raises(RuntimeError) as e:
         func(args, msg, ["false"], output="log")
-    assert str(e.value).startswith("Command failed:")
+    assert re.search(r"^Command failed \(exit code -?\d*\): ", str(e.value))
 
     # Kill with timeout
     args.timeout = 0.2
     with pytest.raises(RuntimeError) as e:
         func(args, msg, ["sleep", "1"], output="log")
-    assert str(e.value).startswith("Command failed:")
+    assert re.search(r"^Command failed \(exit code -?\d*\): ", str(e.value))
+
+    # Preserve proxy environment variables
+    monkeypatch.setattr(os, "environ", {"FTP_PROXY": "testproxy"})
+    ret = func(args, msg, ["sh", "-c", 'echo "$FTP_PROXY"'], output_return=True)
+    assert ret == "testproxy\n"
+
+
+@pytest.mark.skip_ci
+def test_sudo_timer(args):
+    pmb.helpers.run.root(args, ["whoami"])
+
+    time.sleep(300)
+
+    out = pmb.helpers.run.root(args, ["whoami"])
+
+    assert out == 0
```

### Comparing `pmbootstrap-1.9.0/test/test_questions.py` & `pmbootstrap-2.0.0/test/test_questions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,56 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 import os
 import pytest
 import sys
 
-# Import from parent directory
-pmb_src = os.path.realpath(os.path.join(os.path.dirname(__file__) + "/.."))
-sys.path.insert(0, pmb_src)
+import pmb_test
+import pmb_test.const
 import pmb.aportgen.device
 import pmb.config
 import pmb.config.init
 import pmb.helpers.logging
+import pmb.parse.deviceinfo
 
 
 @pytest.fixture
 def args(tmpdir, request):
     import pmb.parse
-    sys.argv = ["pmbootstrap.py", "init"]
+    cfg = f"{pmb_test.const.testdata}/channels.cfg"
+    sys.argv = ["pmbootstrap.py", "--config-channels", cfg, "init"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
 def fake_answers(monkeypatch, answers):
     """
     Patch pmb.helpers.cli.ask() function to return defined answers instead of
     asking the user for an answer.
 
     :param answers: list of answer strings, e.g. ["y", "n", "invalid-device"].
                     In this example, the first question is answered with "y",
                     the second question with "n" and so on.
     """
-    def fake_ask(args, question="Continue?", choices=["y", "n"], default="n",
-                 lowercase_answer=True, validation_regex=None):
+    def fake_ask(question="Continue?", choices=["y", "n"], default="n",
+                 lowercase_answer=True, validation_regex=None, complete=None):
         answer = answers.pop(0)
         logging.info("pmb.helpers.cli.ask() fake answer: " + answer)
         return answer
     monkeypatch.setattr(pmb.helpers.cli, "ask", fake_ask)
 
 
 def test_fake_answers_selftest(monkeypatch):
     fake_answers(monkeypatch, ["first", "second"])
-    assert pmb.helpers.cli.ask(args) == "first"
-    assert pmb.helpers.cli.ask(args) == "second"
+    assert pmb.helpers.cli.ask() == "first"
+    assert pmb.helpers.cli.ask() == "second"
 
 
 def test_questions_booleans(args, monkeypatch):
     functions = [pmb.aportgen.device.ask_for_keyboard,
                  pmb.aportgen.device.ask_for_external_storage]
     for func in functions:
         fake_answers(monkeypatch, ["y", "n"])
@@ -73,86 +58,97 @@
         assert func(args) is False
 
 
 def test_questions_strings(args, monkeypatch):
     functions = [pmb.aportgen.device.ask_for_manufacturer]
     for func in functions:
         fake_answers(monkeypatch, ["Simple string answer"])
-        assert func(args) == "Simple string answer"
+        assert func() == "Simple string answer"
 
 
 def test_questions_name(args, monkeypatch):
     func = pmb.aportgen.device.ask_for_name
 
     # Manufacturer should get added automatically, but not twice
     fake_answers(monkeypatch, ["Amazon Thor"])
-    assert func(args, "Amazon") == "Amazon Thor"
+    assert func("Amazon") == "Amazon Thor"
     fake_answers(monkeypatch, ["Thor"])
-    assert func(args, "Amazon") == "Amazon Thor"
+    assert func("Amazon") == "Amazon Thor"
 
     # Don't add the manufacturer when it starts with "Google"
     fake_answers(monkeypatch, ["Google Nexus 12345"])
-    assert func(args, "Amazon") == "Google Nexus 12345"
+    assert func("Amazon") == "Google Nexus 12345"
 
 
 def test_questions_arch(args, monkeypatch):
     fake_answers(monkeypatch, ["invalid_arch", "aarch64"])
-    assert pmb.aportgen.device.ask_for_architecture(args) == "aarch64"
+    assert pmb.aportgen.device.ask_for_architecture() == "aarch64"
 
 
 def test_questions_bootimg(args, monkeypatch):
     func = pmb.aportgen.device.ask_for_bootimg
     fake_answers(monkeypatch, ["invalid_path", ""])
     assert func(args) is None
 
-    bootimg_path = pmb_src + "/test/testdata/bootimg/normal-boot.img"
+    bootimg_path = pmb_test.const.testdata + "/bootimg/normal-boot.img"
     fake_answers(monkeypatch, [bootimg_path])
-    output = {"base": "0x80000000",
+    output = {"header_version": "0",
+              "base": "0x80000000",
               "kernel_offset": "0x00008000",
               "ramdisk_offset": "0x04000000",
               "second_offset": "0x00f00000",
               "tags_offset": "0x0e000000",
               "pagesize": "2048",
               "cmdline": "bootopt=64S3,32S1,32S1",
-              "qcdt": "false"}
+              "qcdt": "false",
+              "mtk_mkimage": "false",
+              "dtb_second": "false"}
     assert func(args) == output
 
 
 def test_questions_device(args, monkeypatch):
     # Prepare args
-    args.aports = pmb_src + "/test/testdata/init_questions_device/aports"
+    args.aports = pmb_test.const.testdata + "/init_questions_device/aports"
     args.device = "lg-mako"
     args.nonfree_firmware = True
     args.nonfree_userland = False
     args.kernel = "downstream"
 
     # Do not generate aports
     def fake_generate(args, pkgname):
         return
     monkeypatch.setattr(pmb.aportgen, "generate", fake_generate)
 
     # Existing device (without non-free components so we have defaults there)
     func = pmb.config.init.ask_for_device
     nonfree = {"firmware": True, "userland": False}
-    fake_answers(monkeypatch, ["lg-mako"])
+    fake_answers(monkeypatch, ["lg", "mako"])
     kernel = args.kernel
     assert func(args) == ("lg-mako", True, kernel, nonfree)
 
-    # Non-existing device, go back, existing device
-    fake_answers(monkeypatch, ["whoops-typo", "n", "lg-mako"])
+    # Non-existing vendor, go back, existing vendor+device
+    fake_answers(monkeypatch, ["whoops", "n", "lg", "mako"])
+    assert func(args) == ("lg-mako", True, kernel, nonfree)
+
+    # Existing vendor, new device, go back, existing vendor+device
+    fake_answers(monkeypatch, ["lg", "nonexistent", "n", "lg", "mako"])
     assert func(args) == ("lg-mako", True, kernel, nonfree)
 
-    # New device
-    fake_answers(monkeypatch, ["new-device", "y"])
+    # New vendor and new device (new port)
+    fake_answers(monkeypatch, ["new", "y", "device", "y"])
     assert func(args) == ("new-device", False, kernel, nonfree)
 
+    # Existing vendor, new device (new port)
+    fake_answers(monkeypatch, ["lg", "nonexistent", "y"])
+    assert func(args) == ("lg-nonexistent", False, kernel, nonfree)
+
 
 def test_questions_device_kernel(args, monkeypatch):
     # Prepare args
-    args.aports = pmb_src + "/test/testdata/init_questions_device/aports"
+    args.aports = pmb_test.const.testdata + "/init_questions_device/aports"
     args.kernel = "downstream"
 
     # Kernel hardcoded in depends
     func = pmb.config.init.ask_for_device_kernel
     device = "lg-mako"
     assert func(args, device) == args.kernel
 
@@ -164,15 +160,15 @@
     # Choose "downstream"
     fake_answers(monkeypatch, ["downstream"])
     assert func(args, device) == "downstream"
 
 
 def test_questions_device_nonfree(args, monkeypatch):
     # Prepare args
-    args.aports = pmb_src + "/test/testdata/init_questions_device/aports"
+    args.aports = pmb_test.const.testdata + "/init_questions_device/aports"
     args.nonfree_firmware = False
     args.nonfree_userland = False
 
     # APKBUILD with firmware and userland (all yes)
     func = pmb.config.init.ask_for_device_nonfree
     device = "nonfree-firmware-and-userland"
     fake_answers(monkeypatch, ["y", "y"])
@@ -198,43 +194,54 @@
     nonfree = {"firmware": False, "userland": True}
     assert func(args, device) == nonfree
 
 
 def test_questions_flash_methods(args, monkeypatch):
     func = pmb.aportgen.device.ask_for_flash_method
     fake_answers(monkeypatch, ["invalid_flash_method", "fastboot"])
-    assert func(args) == "fastboot"
+    assert func() == "fastboot"
 
     fake_answers(monkeypatch, ["0xffff"])
-    assert func(args) == "0xffff"
+    assert func() == "0xffff"
 
     fake_answers(monkeypatch, ["heimdall", "invalid_type", "isorec"])
-    assert func(args) == "heimdall-isorec"
+    assert func() == "heimdall-isorec"
 
     fake_answers(monkeypatch, ["heimdall", "bootimg"])
-    assert func(args) == "heimdall-bootimg"
+    assert func() == "heimdall-bootimg"
 
 
 def test_questions_keymaps(args, monkeypatch):
     func = pmb.config.init.ask_for_keymaps
     fake_answers(monkeypatch, ["invalid_keymap", "us/rx51_us"])
-    assert func(args, "nokia-n900") == "us/rx51_us"
-    assert func(args, "lg-mako") == ""
+    assert func(args, pmb.parse.deviceinfo(args, "nokia-n900")) == "us/rx51_us"
+    assert func(args, pmb.parse.deviceinfo(args, "lg-mako")) == ""
 
 
-def test_questions_qemu_native_mesa(args, monkeypatch):
-    func = pmb.config.init.ask_for_qemu_native_mesa_driver
-    fake_answers(monkeypatch, ["invalid_driver", "dri-swrast"])
-    assert func(args, "qemu-amd64", "x86_64") == "dri-swrast"
-    assert func(args, "qemu-aarch64", "x86_64") is None
+def test_questions_ui(args, monkeypatch):
+    args.aports = pmb_test.const.testdata + "/init_questions_device/aports"
+    device = "lg-mako"
+    info = pmb.parse.deviceinfo(args, device)
 
+    fake_answers(monkeypatch, ["none"])
+    assert pmb.config.init.ask_for_ui(args, info) == "none"
 
-def test_questions_ui(args, monkeypatch):
     fake_answers(monkeypatch, ["invalid_UI", "weston"])
-    assert pmb.config.init.ask_for_ui(args) == "weston"
+    assert pmb.config.init.ask_for_ui(args, info) == "weston"
+
+
+def test_questions_ui_extras(args, monkeypatch):
+    args.aports = pmb_test.const.testdata + "/init_questions_device/aports"
+    assert not pmb.config.init.ask_for_ui_extras(args, "none")
+
+    fake_answers(monkeypatch, ["n"])
+    assert not pmb.config.init.ask_for_ui_extras(args, "weston")
+
+    fake_answers(monkeypatch, ["y"])
+    assert pmb.config.init.ask_for_ui_extras(args, "weston")
 
 
 def test_questions_work_path(args, monkeypatch, tmpdir):
     # Existing paths (triggering various errors)
     func = pmb.config.init.ask_for_work_path
     tmpdir = str(tmpdir)
     fake_answers(monkeypatch, ["/dev/null", os.path.dirname(__file__),
@@ -243,28 +250,34 @@
 
     # Non-existing path
     work = tmpdir + "/non_existing_subfolder"
     fake_answers(monkeypatch, [work])
     assert func(args) == (work, False)
 
 
-def test_questions_build_options(args, monkeypatch):
-    func = pmb.config.init.ask_for_build_options
+def test_questions_additional_options(args, monkeypatch):
+    func = pmb.config.init.ask_for_additional_options
     cfg = {"pmbootstrap": {}}
 
     # Skip changing anything
     fake_answers(monkeypatch, ["n"])
     func(args, cfg)
     assert cfg == {"pmbootstrap": {}}
 
     # Answer everything
-    fake_answers(monkeypatch, ["y", "5", "2G", "n"])
+    fake_answers(monkeypatch, ["y", "128", "64", "5", "2G", "n", "y", "1",
+                               "n"])
     func(args, cfg)
-    assert cfg == {"pmbootstrap": {"jobs": "5",
-                                   "ccache_size": "2G"}}
+    mirror = pmb.config.defaults["mirrors_postmarketos"]
+    assert cfg == {"pmbootstrap": {"extra_space": "128",
+                                   "boot_size": "64",
+                                   "jobs": "5",
+                                   "ccache_size": "2G",
+                                   "sudo_timer": "False",
+                                   "mirrors_postmarketos": mirror}}
 
 
 def test_questions_hostname(args, monkeypatch):
     func = pmb.config.init.ask_for_hostname
     device = "test-device"
 
     # Valid hostname
@@ -282,7 +295,12 @@
     # Begins or ends with minus
     fake_answers(monkeypatch, ["-invalid", "invalid-", "valid"])
     assert func(args, device) == "valid"
 
     # Device name: empty string
     fake_answers(monkeypatch, [device])
     assert func(args, device) == ""
+
+
+def test_questions_channel(args, monkeypatch):
+    fake_answers(monkeypatch, ["invalid-channel", "v20.05"])
+    assert pmb.config.init.ask_for_channel(args) == "v20.05"
```

### Comparing `pmbootstrap-1.9.0/test/test_newapkbuild.py` & `pmbootstrap-2.0.0/test/test_crossdirect.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,85 +1,81 @@
-"""
-Copyright 2017 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import glob
-import os
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import pytest
 import sys
 
-# Import from parent directory
-sys.path.insert(0, os.path.realpath(
-    os.path.join(os.path.dirname(__file__) + "/..")))
-import pmb.build.newapkbuild
-import pmb.config
-import pmb.config.init
+import pmb_test  # noqa
+import pmb.chroot.apk_static
+import pmb.config.pmaports
+import pmb.parse.apkindex
 import pmb.helpers.logging
+import pmb.helpers.run
+import pmb.parse.bootimg
 
 
 @pytest.fixture
-def args(tmpdir, request):
+def args(request):
     import pmb.parse
-    sys.argv = ["pmbootstrap.py", "init"]
+    sys.argv = ["pmbootstrap.py", "chroot"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
-def test_newapkbuild(args, monkeypatch, tmpdir):
-    # Fake functions
-    def confirm_true(*nargs):
-        return True
-
-    def confirm_false(*nargs):
-        return False
-
-    # Preparation
-    monkeypatch.setattr(pmb.helpers.cli, "confirm", confirm_false)
-    pmb.build.init(args)
-    args.aports = tmpdir = str(tmpdir)
-    func = pmb.build.newapkbuild
-
-    # Show the help
-    func(args, "main", ["-h"])
-    assert glob.glob(tmpdir + "/*") == []
-
-    # Test package
-    pkgname = "testpackage"
-    func(args, "main", [pkgname])
-    apkbuild_path = tmpdir + "/main/" + pkgname + "/APKBUILD"
-    apkbuild = pmb.parse.apkbuild(args, apkbuild_path)
-    assert apkbuild["pkgname"] == pkgname
-    assert apkbuild["pkgdesc"] == ""
-
-    # Don't overwrite
-    with pytest.raises(RuntimeError) as e:
-        func(args, "main", [pkgname])
-    assert "Aborted" in str(e.value)
-
-    # Overwrite
-    monkeypatch.setattr(pmb.helpers.cli, "confirm", confirm_true)
-    pkgdesc = "testdescription"
-    func(args, "main", ["-d", pkgdesc, pkgname])
-    args.cache["apkbuild"] = {}
-    apkbuild = pmb.parse.apkbuild(args, apkbuild_path)
-    assert apkbuild["pkgname"] == pkgname
-    assert apkbuild["pkgdesc"] == pkgdesc
-
-    # There should be no src folder
-    assert not os.path.exists(tmpdir + "/main/" + pkgname + "/src")
+def pmbootstrap_run(args, parameters, check=True):
+    """Execute pmbootstrap.py with a test pmbootstrap.conf."""
+    return pmb.helpers.run.user(args, ["./pmbootstrap.py"] + parameters,
+                                working_dir=pmb.config.pmb_src,
+                                check=check)
+
+
+def test_crossdirect_rust(args):
+    """ Set up buildroot_armv7 chroot for building, but remove /usr/bin/rustc.
+        Build hello-world-rust for armv7, to verify that it uses
+        /native/usr/bin/rustc instead of /usr/bin/rustc. The package has a
+        check() function, which makes sure that the built program is actually
+        working. """
+    pmbootstrap_run(args, ["-y", "zap"])
+
+    # Remember previously selected device
+    cfg = pmb.config.load(args)
+    old_device = cfg['pmbootstrap']['device']
+
+    try:
+        # First, switch to device that is known to exist on all channels,
+        # such as qemu-amd64. Currently selected device may not exist in
+        # stable branch!
+        cfg['pmbootstrap']['device'] = 'qemu-amd64'
+        pmb.config.save(args, cfg)
+
+        # Switch to "v20.05" channel, as a stable release of alpine is more
+        # likely to have the same rustc version across various architectures.
+        # If armv7/x86_64 have a different rustc version, this test will fail:
+        # 'found crate `std` compiled by an incompatible version of rustc'
+        pmb.config.pmaports.switch_to_channel_branch(args, "v23.06")
+
+        pmbootstrap_run(args, ["build_init", "-barmv7"])
+        pmbootstrap_run(args, ["chroot", "--add=rust", "-barmv7", "--",
+                               "mv", "/usr/bin/rustc", "/usr/bin/rustc_"])
+        pmbootstrap_run(args, ["build", "hello-world-rust", "--arch=armv7",
+                               "--force"])
+        # Make /native/usr/bin/rustc unusable too, to make the build fail
+        pmbootstrap_run(args, ["chroot", "--", "rm", "/usr/bin/rustc"])
+        assert pmbootstrap_run(args, ["build", "hello-world-rust",
+                                      "--arch=armv7", "--force"],
+                               check=False) == 1
+
+        # Make /usr/bin/rustc usable again, to test fallback with qemu
+        pmbootstrap_run(args, ["chroot", "-barmv7", "--",
+                               "mv", "/usr/bin/rustc_", "/usr/bin/rustc"])
+        pmbootstrap_run(args, ["build", "hello-world-rust", "--arch=armv7",
+                               "--force"])
+    finally:
+        # Clean up
+        pmb.config.pmaports.switch_to_channel_branch(args, "edge")
+        pmbootstrap_run(args, ["-y", "zap"])
+
+        # Restore previously selected device
+        cfg['pmbootstrap']['device'] = old_device
+        pmb.config.save(args, cfg)
```

### Comparing `pmbootstrap-1.9.0/test/test_parse_depends.py` & `pmbootstrap-2.0.0/test/test_parse_depends.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,61 +1,38 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
-"""
-This file tests all functions from pmb.parse.depends.
-"""
-
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
+""" Test pmb.parse.depends """
 import collections
-import os
 import pytest
 import sys
 
-# Import from parent directory
-sys.path.insert(0, os.path.realpath(
-    os.path.join(os.path.dirname(__file__) + "/..")))
+import pmb_test  # noqa
 import pmb.config
 import pmb.config.init
 import pmb.helpers.logging
 import pmb.parse.depends
 
 
 @pytest.fixture
 def args(tmpdir, request):
     import pmb.parse
     sys.argv = ["pmbootstrap", "init"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
 def test_package_from_aports(args):
     func = pmb.parse.depends.package_from_aports
     assert func(args, "invalid-package") is None
     assert func(args, "hello-world") == {"pkgname": "hello-world",
                                          "depends": [],
-                                         "version": "1-r4"}
+                                         "version": "1-r6"}
 
 
 def test_package_provider(args, monkeypatch):
     # Override pmb.parse.apkindex.providers()
     providers = collections.OrderedDict()
 
     def return_providers(*args, **kwargs):
@@ -81,25 +58,33 @@
     assert func(args, pkgname, pkgnames_install) == package
 
     # 2. Provider with the same package name
     package_two = {"pkgname": "test-two", "provides": ["test"]}
     providers = {"test-two": package_two, "test": package}
     assert func(args, pkgname, pkgnames_install) == package
 
-    # 3. Pick a package, that will be installed anyway
+    # 3. Pick a package that will be installed anyway
     providers = {"test_": package, "test-two": package_two}
     installed = {"test_": package}
     pkgnames_install = ["test-two"]
     assert func(args, pkgname, pkgnames_install) == package_two
 
-    # 4. Pick a package, that is already installed
+    # 4. Pick a package that is already installed
     pkgnames_install = []
     assert func(args, pkgname, pkgnames_install) == package
 
-    # 5. Pick the first one
+    # 5. Pick package with highest priority
+    package_with_priority = {"pkgname": "test-priority", "provides": ["test"],
+                             "provider_priority": 100}
+    providers = {"test-two": package_two,
+                 "test-priority": package_with_priority}
+    assert func(args, pkgname, pkgnames_install) == package_with_priority
+
+    # 6. Pick the first one
+    providers = {"test_": package, "test-two": package_two}
     installed = {}
     assert func(args, pkgname, pkgnames_install) == package
 
 
 def test_package_from_index(args, monkeypatch):
     # Override pmb.parse.depends.package_provider()
     provider = None
@@ -157,21 +142,26 @@
     monkeypatch.setattr(pmb.parse.depends, "package_from_aports",
                         return_none)
 
     # Override depends returned from APKINDEX
     depends = {
         "test": ["libtest", "so:libtest.so.1"],
         "libtest": ["libtest_depend"],
-        "libtest_depend": [],
+        "libtest_depend": ["!libtest_conflict", "!libtest_conflict_missing"],
+        "libtest_conflict": [],
         "so:libtest.so.1": ["libtest_depend"],
     }
 
     def package_from_index(args, pkgname, install, aport, suffix):
-        return {"pkgname": pkgname, "depends": depends[pkgname]}
+        if pkgname in depends:
+            return {"pkgname": pkgname, "depends": depends[pkgname]}
+        else:
+            return None
     monkeypatch.setattr(pmb.parse.depends, "package_from_index",
                         package_from_index)
 
     # Run
     func = pmb.parse.depends.recurse
     pkgnames = ["test", "so:libtest.so.1"]
-    result = ["test", "so:libtest.so.1", "libtest", "libtest_depend"]
+    result = ["test", "so:libtest.so.1", "libtest", "libtest_depend",
+              "!libtest_conflict"]
     assert func(args, pkgnames) == result
```

### Comparing `pmbootstrap-1.9.0/test/test_qemu_running_processes.py` & `pmbootstrap-2.0.0/test/test_qemu_running_processes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,52 @@
-"""
-Copyright 2017 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 """
 This file runs various installations and boots into them with QEMU, then checks
 via SSH if expected processes are running.
 
 We use an extra config file (based on ~/.config/pmbootstrap.cfg), because we
 need to change it a lot (e.g. UI, username, ...).
 """
-
-import os
 import pytest
 import sys
 import shutil
 import shlex
 import time
 
-# Import from parent directory
-pmb_src = os.path.realpath(os.path.join(os.path.dirname(__file__) + "/.."))
-sys.path.insert(0, pmb_src)
+import pmb_test  # noqa
 import pmb.chroot.apk_static
 import pmb.parse.apkindex
 import pmb.helpers.logging
 import pmb.helpers.run
 import pmb.parse.bootimg
 
 
 @pytest.fixture
 def args(request):
     import pmb.parse
     sys.argv = ["pmbootstrap.py", "chroot"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
 def ssh_create_askpass_script(args):
     """Create /tmp/y.sh, which we need to automatically login via SSH."""
     with open(args.work + "/chroot_native/tmp/y.sh", "w") as handle:
         handle.write("#!/bin/sh\necho y\n")
     pmb.chroot.root(args, ["chmod", "+x", "/tmp/y.sh"])
 
 
 def pmbootstrap_run(args, config, parameters, output="log"):
     """Execute pmbootstrap.py with a test pmbootstrap.conf."""
     return pmb.helpers.run.user(args, ["./pmbootstrap.py", "-c", config] +
-                                parameters, working_dir=pmb_src,
+                                parameters, working_dir=pmb.config.pmb_src,
                                 output=output)
 
 
 def pmbootstrap_yes(args, config, parameters):
     """
     Execute pmbootstrap.py with a test pmbootstrap.conf, and pipe "yes" into it
     (so we can do a fully automated installation, using "y" as password
@@ -76,15 +55,15 @@
     it would write no output, and get killed by the timeout).
     """
     command = ("yes | ./pmbootstrap.py --details-to-stdout -c " +
                shlex.quote(config))
     for parameter in parameters:
         command += " " + shlex.quote(parameter)
     return pmb.helpers.run.user(args, ["/bin/sh", "-c", command],
-                                working_dir=pmb_src)
+                                working_dir=pmb.config.pmb_src)
 
 
 class QEMU(object):
     def __init__(self, request):
         self.process = None
         request.addfinalizer(self.terminate)
 
@@ -94,21 +73,20 @@
         else:
             print("WARNING: The QEMU process wasn't set, so it could not be"
                   " terminated.")
 
     def run(self, args, tmpdir, ui="none"):
         # Copy and adjust user's pmbootstrap.cfg
         config = str(tmpdir) + "/pmbootstrap.cfg"
-        shutil.copyfile(os.path.expanduser("~") + "/.config/pmbootstrap.cfg",
-                        config)
+        shutil.copyfile(args.config, config)
         pmbootstrap_run(args, config, ["config", "device", "qemu-amd64"])
+        pmbootstrap_run(args, config, ["config", "kernel", "virt"])
         pmbootstrap_run(args, config, ["config", "extra_packages", "none"])
         pmbootstrap_run(args, config, ["config", "user", "testuser"])
         pmbootstrap_run(args, config, ["config", "ui", ui])
-        pmbootstrap_run(args, config, ["config", "qemu_native_mesa_driver", "dri-swrast"])
 
         # Prepare native chroot
         pmbootstrap_run(args, config, ["-y", "zap"])
         pmb.chroot.apk.install(args, ["openssh-client"])
         ssh_create_askpass_script(args)
 
         # Create and run rootfs
@@ -126,39 +104,46 @@
     """
     Run a command in the QEMU VM on localhost via SSH.
 
     :param command: flat string of the command to execute, e.g. "ps au"
     :returns: the result from the SSH server
     """
     ret = pmb.chroot.user(args, ["SSH_ASKPASS=/tmp/y.sh", "DISPLAY=", "ssh",
+                                 "-o", "ConnectTimeout=10",
                                  "-o", "UserKnownHostsFile=/dev/null",
                                  "-o", "StrictHostKeyChecking=no",
                                  "-p", "2222", "testuser@localhost", "--",
                                  command], output_return=True, check=False)
     return ret
 
 
-def is_running(args, programs, tries=300, sleep_before_retry=1):
+def is_running(args, programs, timeout=300, sleep_before_retry=1):
     """
     Simple check that looks for program names in the output of "ps ax".
     This is error-prone, only use it with programs that have a unique name.
-    With defaults retries and sleep_before_retry values, it will try each
-    second for 5 minutes.
+    With defaults timeout and sleep_before_retry values, it will try keep
+    trying for 5 minutes, but not more than once per second.
 
     :param programs: list of programs to check for, e.g. ["xfce4-desktop"]
-    :param tries: amount of tries with the wrong result before giving up
+    :param timeout: approximate time in seconds until timeout
     :param sleep_before_retry: time in seconds to sleep before trying again
     """
-    print("Looking for programs to appear in the VM (tries: " + str(tries) +
-          "): " + ", ".join(programs))
+    print(f"Looking for programs to appear in the VM (timeout: {timeout}): " +
+          ", ".join(programs))
     ssh_works = False
-    for i in range(0, tries):
-        # Sleep
-        if i > 0:
-            time.sleep(sleep_before_retry)
+
+    end = time.monotonic() + timeout
+    last_try = 0
+
+    while last_try < end:
+        # Sleep only when last try exited immediately
+        sleep = last_try - time.monotonic() + sleep_before_retry
+        if sleep > 0:
+            time.sleep(sleep)
+        last_try = time.monotonic()
 
         # Get running programs via SSH
         all = ssh_run(args, "ps ax")
         if not all:
             continue
         ssh_works = True
 
@@ -175,21 +160,32 @@
     if ssh_works:
         print("Programs not running: " + ", ".join(missing))
     else:
         print("Could not connect to the VM via SSH")
     return False
 
 
+@pytest.mark.skip_ci
+def test_none(args, tmpdir, qemu):
+    qemu.run(args, tmpdir)
+
+    # Check that at least SSH works (no special process running)
+    assert is_running(args, [])
+
+    # self-test of is_running() - invalid-process should not be detected as
+    # running
+    assert is_running(args, ["invalid-process"], 1) is False
+
+
+@pytest.mark.skip_ci
 def test_xfce4(args, tmpdir, qemu):
     qemu.run(args, tmpdir, "xfce4")
     assert is_running(args, ["xfce4-session", "xfdesktop", "xfce4-panel",
                              "Thunar", "dbus-daemon", "xfwm4"])
 
-    # self-test of is_running()
-    assert is_running(args, ["invalid-process"], 1) is False
-
 
+@pytest.mark.skip_ci
 def test_plasma_mobile(args, tmpdir, qemu):
-    # NOTE: Once we have plasma mobile running properly without GL, we can check
-    # for more processes
+    # NOTE: Once we have plasma mobile running properly without GL, we can
+    # check for more processes
     qemu.run(args, tmpdir, "plasma-mobile")
     assert is_running(args, ["polkitd"])
```

### Comparing `pmbootstrap-1.9.0/test/test_aportgen.py` & `pmbootstrap-2.0.0/test/test_parse_apkbuild.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,140 +1,156 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import os
-import sys
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import pytest
-import filecmp
+import sys
 
-# Import from parent directory
-pmb_src = os.path.realpath(os.path.join(os.path.dirname(__file__) + "/.."))
-sys.path.insert(0, pmb_src)
-
-import pmb.aportgen
-import pmb.aportgen.core
-import pmb.config
-import pmb.helpers.logging
+import pmb_test
+import pmb_test.const
+import pmb.parse._apkbuild
 
 
 @pytest.fixture
 def args(tmpdir, request):
     import pmb.parse
-    sys.argv = ["pmbootstrap.py", "chroot"]
+    sys.argv = ["pmbootstrap.py", "init"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
-    args.fork_alpine = False
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
-def test_aportgen_compare_output(args, tmpdir, monkeypatch):
-    # Fake aports folder in tmpdir
-    args.aports = str(tmpdir)
-    os.mkdir(tmpdir + "/cross")
-    testdata = pmb_src + "/test/testdata/aportgen"
-
-    # Override get_upstream_aport() to point to testdata
-    def func(args, upstream_path):
-        return testdata + "/aports/main/" + upstream_path
-    monkeypatch.setattr(pmb.aportgen.core, "get_upstream_aport", func)
-
-    # Run aportgen and compare output
-    pkgnames = ["binutils-armhf", "gcc-armhf"]
-    for pkgname in pkgnames:
-        pmb.aportgen.generate(args, pkgname)
-        path_new = args.aports + "/cross/" + pkgname + "/APKBUILD"
-        path_old = testdata + "/pmaports/cross/" + pkgname + "/APKBUILD"
-        assert os.path.exists(path_new)
-        assert filecmp.cmp(path_new, path_old, False)
-
-
-def test_aportgen_fork_alpine_compare_output(args, tmpdir, monkeypatch):
-    # Fake aports folder in tmpdir
-    args.aports = str(tmpdir)
-    os.mkdir(tmpdir + "/temp")
-    testdata = pmb_src + "/test/testdata/aportgen"
-    args.fork_alpine = True
-
-    # Override get_upstream_aport() to point to testdata
-    def func(args, upstream_path):
-        return testdata + "/aports/main/" + upstream_path
-    monkeypatch.setattr(pmb.aportgen.core, "get_upstream_aport", func)
-
-    # Run aportgen and compare output
-    pkgname = "binutils"
-    pmb.aportgen.generate(args, pkgname)
-    path_new = args.aports + "/temp/" + pkgname + "/APKBUILD"
-    path_old = testdata + "/pmaports/temp/" + pkgname + "/APKBUILD"
-    assert os.path.exists(path_new)
-    assert filecmp.cmp(path_new, path_old, False)
-
-
-def test_aportgen(args, tmpdir):
-    # Fake aports folder in tmpdir
-    args.aports = str(tmpdir)
-    os.mkdir(tmpdir + "/cross")
-
-    # Create aportgen folder -> code path where it still exists
-    pmb.helpers.run.user(args, ["mkdir", "-p", args.work + "/aportgen"])
-
-    # Generate all valid packages (gcc twice -> different code path)
-    pkgnames = ["binutils-armhf", "musl-armhf", "busybox-static-armhf",
-                "gcc-armhf", "gcc-armhf"]
-    for pkgname in pkgnames:
-        pmb.aportgen.generate(args, pkgname)
-
-
-def test_aportgen_invalid_generator(args):
-    with pytest.raises(ValueError) as e:
-        pmb.aportgen.generate(args, "pkgname-with-no-generator")
-    assert "No generator available" in str(e.value)
-
-
-def test_aportgen_get_upstream_aport(args, monkeypatch):
-    # Fake pmb.parse.apkbuild()
-    def fake_apkbuild(*args, **kwargs):
-        return apkbuild
-    monkeypatch.setattr(pmb.parse, "apkbuild", fake_apkbuild)
-
-    # Fake pmb.parse.apkindex.package()
-    def fake_package(*args, **kwargs):
-        return package
-    monkeypatch.setattr(pmb.parse.apkindex, "package", fake_package)
-
-    # Equal version
-    func = pmb.aportgen.core.get_upstream_aport
-    upstream = "gcc"
-    upstream_full = args.work + "/cache_git/aports_upstream/main/" + upstream
-    apkbuild = {"pkgver": "2.0", "pkgrel": "0"}
-    package = {"version": "2.0-r0"}
-    assert func(args, upstream) == upstream_full
-
-    # APKBUILD < binary
-    apkbuild = {"pkgver": "1.0", "pkgrel": "0"}
-    package = {"version": "2.0-r0"}
+def test_subpackages():
+    testdata = pmb_test.const.testdata
+    path = testdata + "/apkbuild/APKBUILD.subpackages"
+    apkbuild = pmb.parse.apkbuild(path, check_pkgname=False)
+
+    subpkg = apkbuild["subpackages"]["simple"]
+    assert subpkg["pkgdesc"] == ""
+    # Inherited from parent package
+    assert subpkg["depends"] == ["postmarketos-base"]
+
+    subpkg = apkbuild["subpackages"]["custom"]
+    assert subpkg["pkgdesc"] == "This is one of the custom subpackages"
+    assert subpkg["depends"] == ["postmarketos-base", "glibc"]
+
+    # Successful extraction
+    path = (testdata + "/init_questions_device/aports/device/testing/"
+            "device-nonfree-firmware/APKBUILD")
+    apkbuild = pmb.parse.apkbuild(path)
+    subpkg = (apkbuild["subpackages"]
+              ["device-nonfree-firmware-nonfree-firmware"])
+    assert subpkg["pkgdesc"] == "firmware description"
+
+    # Can't find the pkgdesc in the function
+    path = testdata + "/apkbuild/APKBUILD.missing-pkgdesc-in-subpackage"
+    apkbuild = pmb.parse.apkbuild(path, check_pkgname=False)
+    subpkg = (apkbuild["subpackages"]
+              ["missing-pkgdesc-in-subpackage-subpackage"])
+    assert subpkg["pkgdesc"] == ""
+
+    # Can't find the function
+    assert apkbuild["subpackages"]["invalid-function"] is None
+
+
+def test_kernels(args):
+    # Kernel hardcoded in depends
+    args.aports = pmb_test.const.testdata + "/init_questions_device/aports"
+    func = pmb.parse._apkbuild.kernels
+    device = "lg-mako"
+    assert func(args, device) is None
+
+    # Upstream and downstream kernel
+    device = "sony-amami"
+    ret = {"downstream": "Downstream description",
+           "mainline": "Mainline description"}
+    assert func(args, device) == ret
+
+    # Long kernel name (e.g. two different mainline kernels)
+    device = "wileyfox-crackling"
+    ret = {"mainline": "Mainline kernel (no modem)",
+           "mainline-modem": "Mainline kernel (with modem)",
+           "downstream": "Downstream kernel"}
+    assert func(args, device) == ret
+
+
+def test_depends_in_depends():
+    path = pmb_test.const.testdata + "/apkbuild/APKBUILD.depends-in-depends"
+    apkbuild = pmb.parse.apkbuild(path, check_pkgname=False)
+    assert apkbuild["depends"] == ["first", "second", "third"]
+
+
+def test_parse_attributes():
+    # Convenience function for calling the function with a block of text
+    def func(attribute, block):
+        lines = block.split("\n")
+        for i in range(0, len(lines)):
+            lines[i] += "\n"
+        i = 0
+        path = "(testcase in " + __file__ + ")"
+        print("=== parsing attribute '" + attribute + "' in test block:")
+        print(block)
+        print("===")
+        return pmb.parse._apkbuild.parse_attribute(attribute, lines, i, path)
+
+    assert func("depends", "pkgname='test'") == (False, None, 0)
+
+    assert func("pkgname", 'pkgname="test"') == (True, "test", 0)
+
+    assert func("pkgname", "pkgname='test'") == (True, "test", 0)
+
+    assert func("pkgname", "pkgname=test") == (True, "test", 0)
+
+    assert func("pkgname", 'pkgname="test\n"') == (True, "test", 1)
+
+    assert func("pkgname", 'pkgname="\ntest\n"') == (True, "test", 2)
+
+    assert func("pkgname", 'pkgname="test" # random comment\npkgrel=3') == \
+        (True, "test", 0)
+
+    assert func("pkgver", 'pkgver=2.37 # random comment\npkgrel=3') == \
+           (True, "2.37", 0)
+
+    assert func("depends", "depends='\nfirst\nsecond\nthird\n'#") == \
+        (True, "first second third", 4)
+
+    assert func("depends", 'depends="\nfirst\n\tsecond third"') == \
+        (True, "first second third", 2)
+
+    assert func("depends", 'depends=') == (True, "", 0)
+
     with pytest.raises(RuntimeError) as e:
-        func(args, upstream)
-    assert str(e.value).startswith("You can update your local checkout with")
+        func("depends", 'depends="\nmissing\nend\nquote\nsign')
+    assert str(e.value).startswith("Can't find closing")
 
-    # APKBUILD > binary
-    apkbuild = {"pkgver": "3.0", "pkgrel": "0"}
-    package = {"version": "2.0-r0"}
     with pytest.raises(RuntimeError) as e:
-        func(args, upstream)
-    assert str(e.value).startswith("You can force an update of your binary")
+        func("depends", 'depends="')
+    assert str(e.value).startswith("Can't find closing")
+
+
+def test_variable_replacements():
+    path = pmb_test.const.testdata + "/apkbuild/APKBUILD.variable-replacements"
+    apkbuild = pmb.parse.apkbuild(path, check_pkgname=False)
+    assert apkbuild["pkgdesc"] == "this should not affect variable replacement"
+    assert apkbuild["url"] == "replacements variable string-replacements"
+    assert list(apkbuild["subpackages"].keys()) == ["replacements", "test"]
+
+    assert apkbuild["subpackages"]["replacements"] is None
+    test_subpkg = apkbuild["subpackages"]["test"]
+    assert test_subpkg["pkgdesc"] == ("this should not affect variable "
+                                      "replacement")
+
+
+def test_parse_maintainers():
+    path = pmb_test.const.testdata + "/apkbuild/APKBUILD.lint"
+    maintainers = [
+        "Oliver Smith <ollieparanoid@postmarketos.org>",
+        "Hello World <hello@world>"
+    ]
+
+    assert pmb.parse._apkbuild.maintainers(path) == maintainers
+
+
+def test_parse_unmaintained():
+    path = (f"{pmb_test.const.testdata}/apkbuild"
+            "/APKBUILD.missing-pkgdesc-in-subpackage")
+    assert pmb.parse._apkbuild.unmaintained(path) == "This is broken!"
```

### Comparing `pmbootstrap-1.9.0/test/test_build_is_necessary.py` & `pmbootstrap-2.0.0/test/test_build_is_necessary.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,89 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import os
 import sys
 import pytest
 
-# Import from parent directory
-sys.path.insert(0, os.path.realpath(
-    os.path.join(os.path.dirname(__file__) + "/..")))
+import pmb_test  # noqa
 import pmb.helpers.logging
 import pmb.helpers.pmaports
 
 
 @pytest.fixture
 def args(request, tmpdir):
     import pmb.parse
     sys.argv = ["pmbootstrap.py", "chroot"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
 
     # Create an empty APKINDEX.tar.gz file, so we can use its path and
     # timestamp to put test information in the cache.
     apkindex_path = str(tmpdir) + "/APKINDEX.tar.gz"
     open(apkindex_path, "a").close()
     lastmod = os.path.getmtime(apkindex_path)
-    args.cache["apkindex"][apkindex_path] = {"lastmod": lastmod, "multiple": {}}
+    pmb.helpers.other.cache["apkindex"][apkindex_path] = {"lastmod": lastmod,
+                                                          "multiple": {}}
     return args
 
 
-def cache_apkindex(args, version):
+def cache_apkindex(version):
     """
     Modify the cache of the parsed binary package repository's APKINDEX
     for the "hello-world" package.
     :param version: full version string, includes pkgver and pkgrl (e.g. 1-r2)
     """
-    apkindex_path = list(args.cache["apkindex"].keys())[0]
+    apkindex_path = list(pmb.helpers.other.cache["apkindex"].keys())[0]
 
-    providers = args.cache["apkindex"][apkindex_path]["multiple"]["hello-world"]
+    providers = pmb.helpers.other.cache[
+        "apkindex"][apkindex_path]["multiple"]["hello-world"]
     providers["hello-world"]["version"] = version
 
 
 def test_build_is_necessary(args):
     # Prepare APKBUILD and APKINDEX data
     aport = pmb.helpers.pmaports.find(args, "hello-world")
-    apkbuild = pmb.parse.apkbuild(args, aport + "/APKBUILD")
+    apkbuild = pmb.parse.apkbuild(f"{aport}/APKBUILD")
     apkbuild["pkgver"] = "1"
     apkbuild["pkgrel"] = "2"
-    indexes = list(args.cache["apkindex"].keys())
+    indexes = list(pmb.helpers.other.cache["apkindex"].keys())
     apkindex_path = indexes[0]
     cache = {"hello-world": {"hello-world": {"pkgname": "hello-world",
                                              "version": "1-r2"}}}
-    args.cache["apkindex"][apkindex_path]["multiple"] = cache
+    pmb.helpers.other.cache["apkindex"][apkindex_path]["multiple"] = cache
 
     # Binary repo has a newer version
-    cache_apkindex(args, "999-r1")
+    cache_apkindex("999-r1")
     assert pmb.build.is_necessary(args, None, apkbuild, indexes) is False
 
     # Aports folder has a newer version
-    cache_apkindex(args, "0-r0")
+    cache_apkindex("0-r0")
     assert pmb.build.is_necessary(args, None, apkbuild, indexes) is True
 
     # Same version
-    cache_apkindex(args, "1-r2")
+    cache_apkindex("1-r2")
     assert pmb.build.is_necessary(args, None, apkbuild, indexes) is False
 
 
 def test_build_is_necessary_no_binary_available(args):
     """
-    APKINDEX cache is set up to fake an empty APKINDEX, which means, that the
+    APKINDEX cache is set up to fake an empty APKINDEX, which means that the
     hello-world package has not been built yet.
     """
-    indexes = list(args.cache["apkindex"].keys())
+    indexes = list(pmb.helpers.other.cache["apkindex"].keys())
     aport = pmb.helpers.pmaports.find(args, "hello-world")
-    apkbuild = pmb.parse.apkbuild(args, aport + "/APKBUILD")
+    apkbuild = pmb.parse.apkbuild(f"{aport}/APKBUILD")
     assert pmb.build.is_necessary(args, None, apkbuild, indexes) is True
+
+
+def test_build_is_necessary_cant_build_pmaport_for_arch(args):
+    """ pmaport version is higher than Alpine's binary package, but pmaport
+        can't be built for given arch. (#1897) """
+
+    apkbuild = {"pkgname": "alpine-base",
+                "arch": "armhf",  # can't build for x86_64!
+                "pkgver": "9999",
+                "pkgrel": "0"}
+    assert pmb.build.is_necessary(args, "x86_64", apkbuild) is False
+    assert pmb.build.is_necessary(args, "armhf", apkbuild) is True
```

### Comparing `pmbootstrap-1.9.0/test/test_apk_static.py` & `pmbootstrap-2.0.0/test/test_apk_static.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,31 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import os
+import copy
 import sys
 import tarfile
 import glob
 import pytest
 
-# Import from parent directory
-pmb_src = os.path.realpath(os.path.join(os.path.dirname(__file__) + "/.."))
-sys.path.insert(0, pmb_src)
+import pmb_test  # noqa
 import pmb.chroot.apk_static
 import pmb.config
 import pmb.parse.apkindex
 import pmb.helpers.logging
 
 
 @pytest.fixture
 def args(request):
     import pmb.parse
     sys.argv = ["pmbootstrap.py", "chroot"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
 def test_read_signature_info(args):
     # Tempfolder inside chroot for fake apk files
     tmp_path = "/tmp/test_read_signature_info"
     tmp_path_outside = args.work + "/chroot_native" + tmp_path
@@ -70,19 +53,21 @@
             pmb.chroot.apk_static.read_signature_info(tar)
         assert "Invalid signature key" in str(e.value)
 
     # Signature file with realistic name
     path = glob.glob(pmb.config.apk_keys_path + "/*.pub")[0]
     name = os.path.basename(path)
     path_archive = "sbin/apk.static.SIGN.RSA." + name
-    pmb.chroot.user(args, ["mv", tmp_path + "/sbin/apk.static.SIGN.RSA.invalid.pub",
-                           tmp_path + "/" + path_archive])
+    pmb.chroot.user(args, ["mv",
+                           f"{tmp_path}/sbin/apk.static.SIGN.RSA.invalid.pub",
+                           f"{tmp_path}/{path_archive}"])
     pmb.chroot.user(args, ["tar", "-czf", tmp_path + "/realistic_name_sig.apk",
                            path_archive], working_dir=tmp_path)
-    with tarfile.open(tmp_path_outside + "/realistic_name_sig.apk", "r:gz") as tar:
+    with tarfile.open(f"{tmp_path_outside}/realistic_name_sig.apk", "r:gz")\
+            as tar:
         sigfilename, sigkey_path = pmb.chroot.apk_static.read_signature_info(
             tar)
         assert sigfilename == path_archive
         assert sigkey_path == path
 
     # Clean up
     pmb.chroot.user(args, ["rm", "-r", tmp_path])
@@ -98,16 +83,16 @@
 
 
 def test_signature_verification(args, tmpdir):
     if os.path.exists(args.work + "/apk.static"):
         os.remove(args.work + "/apk.static")
 
     version = pmb.parse.apkindex.package(args, "apk-tools-static")["version"]
-    apk_path = pmb.chroot.apk_static.download(args,
-                                              "apk-tools-static-" + version + ".apk")
+    apk_path = pmb.chroot.apk_static.download(
+        args, f"apk-tools-static-{version}.apk")
 
     # Extract to temporary folder
     with tarfile.open(apk_path, "r:gz") as tar:
         sigfilename, sigkey_path = pmb.chroot.apk_static.read_signature_info(
             tar)
         files = pmb.chroot.apk_static.extract_temp(tar, sigfilename)
 
@@ -127,21 +112,20 @@
     # Test "apk.static --version" check
     #
     with pytest.raises(RuntimeError) as e:
         pmb.chroot.apk_static.extract(args, "99.1.2-r1", apk_path)
     assert "downgrade attack" in str(e.value)
 
 
-def test_outdated_version(args):
+def test_outdated_version(args, monkeypatch):
     if os.path.exists(args.work + "/apk.static"):
         os.remove(args.work + "/apk.static")
 
-    # change min version
-    min = pmb.config.apk_tools_static_min_version
-    pmb.config.apk_tools_static_min_version = "99.1.2-r1"
+    # Change min version for all branches
+    min_copy = copy.copy(pmb.config.apk_tools_min_version)
+    for key, old_ver in min_copy.items():
+        min_copy[key] = "99.1.2-r1"
+    monkeypatch.setattr(pmb.config, "apk_tools_min_version", min_copy)
 
     with pytest.raises(RuntimeError) as e:
         pmb.chroot.apk_static.init(args)
     assert "outdated version" in str(e.value)
-
-    # reset min version
-    pmb.config.apk_tools_static_min_version = min
```

### Comparing `pmbootstrap-1.9.0/test/test_envkernel.py` & `pmbootstrap-2.0.0/test/test_envkernel.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,14 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import os
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import sys
 import pytest
 
-# Import from parent directory
-pmb_src = os.path.realpath(os.path.join(os.path.dirname(__file__) + "/.."))
-sys.path.insert(0, pmb_src)
-
+import pmb_test
+import pmb_test.const
 import pmb.aportgen
 import pmb.aportgen.core
 import pmb.build
 import pmb.build.envkernel
 import pmb.config
 import pmb.helpers.logging
 
@@ -35,34 +16,32 @@
 @pytest.fixture
 def args(tmpdir, request):
     import pmb.parse
     sys.argv = ["pmbootstrap.py", "init"]
     args = pmb.parse.arguments()
     args.log = args.work + "/log_testsuite.txt"
     pmb.helpers.logging.init(args)
-    request.addfinalizer(args.logfd.close)
+    request.addfinalizer(pmb.helpers.logging.logfd.close)
     return args
 
 
 def test_package_kernel_args(args):
     args.packages = ["package-one", "package-two"]
     with pytest.raises(RuntimeError) as e:
         pmb.build.envkernel.package_kernel(args)
     assert "--envkernel needs exactly one linux-* package as argument." in \
         str(e.value)
 
 
-def test_find_kbuild_output_dir(args):
+def test_find_kbuild_output_dir():
     # Test parsing an APKBUILD
     pkgname = "linux-envkernel-test"
-    testdata = pmb_src + "/test/testdata"
-    path = testdata + "/apkbuild/APKBUILD." + pkgname
+    path = pmb_test.const.testdata + "/apkbuild/APKBUILD." + pkgname
     function_body = pmb.parse.function_body(path, "package")
-    kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(args,
-                                                            function_body)
+    kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(function_body)
     assert kbuild_out == "build"
 
     # Test full function body
     function_body = [
         "   install -Dm644 \"$srcdir\"/build/arch/arm/boot/dt.img ",
         "       \"$pkgdir\"/boot/dt.img",
         "",
@@ -75,72 +54,66 @@
         "   cd \"$srcdir\"/build",
         "   unset LDFLAGS",
         "",
         "   make ARCH=\"$_carch\" CC=\"${CC:-gcc}\" ",
         "       KBUILD_BUILD_VERSION=\"$((pkgrel + 1))-Alpine\" ",
         "       INSTALL_MOD_PATH=\"$pkgdir\" modules_install",
     ]
-    kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(args,
-                                                            function_body)
+    kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(function_body)
     assert kbuild_out == "build"
 
     # Test no kbuild out dir
     function_body = [
         "   install -Dm644 \"$srcdir\"/arch/arm/boot/zImage ",
         "       \"$pkgdir\"/boot/vmlinuz-$_flavor",
         "   install -D \"$srcdir\"/include/config/kernel.release ",
         "       \"$pkgdir\"/usr/share/kernel/$_flavor/kernel.release",
     ]
-    kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(args,
-                                                            function_body)
+    kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(function_body)
     assert kbuild_out == ""
 
     # Test curly brackets around srcdir
     function_body = [
         "   install -Dm644 \"${srcdir}\"/build/arch/arm/boot/zImage ",
         "       \"$pkgdir\"/boot/vmlinuz-$_flavor",
         "   install -D \"${srcdir}\"/build/include/config/kernel.release ",
         "       \"$pkgdir\"/usr/share/kernel/$_flavor/kernel.release",
     ]
-    kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(args,
-                                                            function_body)
+    kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(function_body)
     assert kbuild_out == "build"
 
     # Test multiple sub directories
     function_body = [
         "   install -Dm644 \"${srcdir}\"/sub/dir/arch/arm/boot/zImage-dtb ",
         "       \"$pkgdir\"/boot/vmlinuz-$_flavor",
         "   install -D \"${srcdir}\"/sub/dir/include/config/kernel.release ",
         "       \"$pkgdir\"/usr/share/kernel/$_flavor/kernel.release",
     ]
-    kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(args,
-                                                            function_body)
+    kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(function_body)
     assert kbuild_out == "sub/dir"
 
     # Test no kbuild out dir found
     function_body = [
         "   install -Dm644 \"$srcdir\"/build/not/found/zImage-dtb ",
         "       \"$pkgdir\"/boot/vmlinuz-$_flavor",
         "   install -D \"$srcdir\"/not/found/kernel.release ",
         "       \"$pkgdir\"/usr/share/kernel/$_flavor/kernel.release",
     ]
     with pytest.raises(RuntimeError) as e:
-        kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(args,
-                                                                function_body)
+        kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(function_body)
     assert ("Couldn't find a kbuild out directory. Is your APKBUILD messed up?"
             " If not, then consider adjusting the patterns in "
             "pmb/build/envkernel.py to work with your APKBUILD, or submit an "
             "issue.") in str(e.value)
 
     # Test multiple different kbuild out dirs
     function_body = [
         "   install -Dm644 \"$srcdir\"/build/arch/arm/boot/zImage-dtb ",
         "       \"$pkgdir\"/boot/vmlinuz-$_flavor",
         "   install -D \"$srcdir\"/include/config/kernel.release ",
         "       \"$pkgdir\"/usr/share/kernel/$_flavor/kernel.release",
     ]
     with pytest.raises(RuntimeError) as e:
-        kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(args,
-                                                                function_body)
+        kbuild_out = pmb.build.envkernel.find_kbuild_output_dir(function_body)
     assert ("Multiple kbuild out directories found. Can you modify your "
             "APKBUILD so it only has one output path? If you can't resolve it,"
             " please open an issue.") in str(e.value)
```

### Comparing `pmbootstrap-1.9.0/pmb/chroot/shutdown.py` & `pmbootstrap-2.0.0/pmb/chroot/shutdown.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,16 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 import glob
 import os
 import socket
 from contextlib import closing
 
 import pmb.chroot
-import pmb.chroot.distccd
 import pmb.helpers.mount
 import pmb.install.losetup
 import pmb.parse.arch
 
 
 def kill_adb(args):
     """
@@ -61,42 +44,49 @@
         # have a left over file (#83)
         pmb.chroot.root(args, ["rm", "/dev/mapper/" + name])
     else:
         raise RuntimeError("Failed to parse 'cryptsetup status' output!")
 
 
 def shutdown(args, only_install_related=False):
-    pmb.chroot.distccd.stop(args)
-
     # Stop adb server
     kill_adb(args)
 
     # Umount installation-related paths (order is important!)
     pmb.helpers.mount.umount_all(args, args.work +
                                  "/chroot_native/mnt/install")
     shutdown_cryptsetup_device(args, "pm_crypt")
 
     # Umount all losetup mounted images
     chroot = args.work + "/chroot_native"
     if pmb.helpers.mount.ismount(chroot + "/dev/loop-control"):
         pattern = chroot + "/home/pmos/rootfs/*.img"
         for path_outside in glob.glob(pattern):
             path = path_outside[len(chroot):]
-            pmb.install.losetup.umount(args, path)
+            pmb.install.losetup.umount(args, path, auto_init=False)
+
+    # Umount device rootfs and installer chroots
+    for prefix in ["rootfs", "installer"]:
+        path = f"{args.work}/chroot_{prefix}_{args.device}"
+        if os.path.exists(path):
+            pmb.helpers.mount.umount_all(args, path)
 
-    # Umount device rootfs chroot
-    chroot_rootfs = args.work + "/chroot_rootfs_" + args.device
-    if os.path.exists(chroot_rootfs):
-        pmb.helpers.mount.umount_all(args, chroot_rootfs)
+    # Remove "in-pmbootstrap" marker from all chroots. This marker indicates
+    # that pmbootstrap has set up all mount points etc. to run programs inside
+    # the chroots, but we want it gone afterwards (e.g. when the chroot
+    # contents get copied to a rootfs / installer image, or if creating an
+    # android recovery zip from its contents).
+    for marker in glob.glob(f"{args.work}/chroot_*/in-pmbootstrap"):
+        pmb.helpers.run.root(args, ["rm", marker])
 
     if not only_install_related:
         # Umount all folders inside args.work
         # The folders are explicitly iterated over, so folders symlinked inside
         # args.work get umounted as well (used in test_pkgrel_bump.py, #1595)
         for path in glob.glob(args.work + "/*"):
             pmb.helpers.mount.umount_all(args, path)
 
         # Clean up the rest
         for arch in pmb.config.build_device_architectures:
-            if pmb.parse.arch.cpu_emulation_required(args, arch):
+            if pmb.parse.arch.cpu_emulation_required(arch):
                 pmb.chroot.binfmt.unregister(args, arch)
         logging.debug("Shutdown complete")
```

### Comparing `pmbootstrap-1.9.0/pmb/chroot/binfmt.py` & `pmbootstrap-2.0.0/pmb/chroot/binfmt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import os
 import logging
 
 import pmb.helpers.run
 import pmb.helpers.other
 import pmb.parse
 import pmb.parse.arch
@@ -30,19 +14,30 @@
 
 
 def register(args, arch):
     """
     Get arch, magic, mask.
     """
     arch_qemu = pmb.parse.arch.alpine_to_qemu(arch)
+
+    # always make sure the qemu-<arch> binary is installed, since registering
+    # may happen outside of this method (e.g. by OS)
+    if f"qemu-{arch_qemu}" not in pmb.chroot.apk.installed(args):
+        pmb.chroot.apk.install(args, ["qemu-" + arch_qemu])
+
     if is_registered(arch_qemu):
         return
     pmb.helpers.other.check_binfmt_misc(args)
-    pmb.chroot.apk.install(args, ["qemu-" + arch_qemu])
-    info = pmb.parse.binfmt_info(args, arch_qemu)
+
+    # Don't continue if the actions from check_binfmt_misc caused the OS to
+    # automatically register the target arch
+    if is_registered(arch_qemu):
+        return
+
+    info = pmb.parse.binfmt_info(arch_qemu)
 
     # Build registration string
     # https://en.wikipedia.org/wiki/Binfmt_misc
     # :name:type:offset:magic:mask:interpreter:flags
     name = "qemu-" + arch_qemu
     type = "M"
     offset = ""
```

### Comparing `pmbootstrap-1.9.0/pmb/chroot/other.py` & `pmbootstrap-2.0.0/pmb/chroot/other.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,43 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import os
 import glob
 import logging
 import pmb.chroot.apk
 import pmb.install
 
 
-def kernel_flavors_installed(args, suffix, autoinstall=True):
+def kernel_flavor_installed(args, suffix, autoinstall=True):
     """
-    Get all installed kernel flavors and make sure that there's at least one
+    Get installed kernel flavor. Optionally install the device's kernel
+    beforehand.
 
     :param suffix: the chroot suffix, e.g. "native" or "rootfs_qemu-amd64"
-    :param autoinstall: make sure that at least one kernel flavor is installed
-    :returns: list of installed kernel flavors, e.g. ["postmarketos-mainline"]
+    :param autoinstall: install the device's kernel if it is not installed
+    :returns: * string with the installed kernel flavor,
+                e.g. ["postmarketos-qcom-sdm845"]
+              * None if no kernel is installed
     """
     # Automatically install the selected kernel
     if autoinstall:
-        packages = (["device-" + args.device] +
+        packages = ([f"device-{args.device}"] +
                     pmb.install.get_kernel_package(args, args.device))
         pmb.chroot.apk.install(args, packages, suffix)
 
-    # Find all kernels in /boot
-    prefix = "vmlinuz-"
-    prefix_len = len(prefix)
-    pattern = args.work + "/chroot_" + suffix + "/boot/" + prefix + "*"
-    ret = []
-    for file in glob.glob(pattern):
-        flavor = os.path.basename(file)[prefix_len:]
-        if flavor[-4:] == "-dtb":
-            flavor = flavor[:-4]
-        ret.append(flavor)
+    pattern = f"{args.work}/chroot_{suffix}/usr/share/kernel/*"
+    glob_result = glob.glob(pattern)
 
-    # Return without duplicates
-    return list(set(ret))
+    # There should be only one directory here
+    return os.path.basename(glob_result[0]) if glob_result else None
 
 
 def tempfolder(args, path, suffix="native"):
     """
-    Create a temporary folder inside the chroot, that belongs to "user".
+    Create a temporary folder inside the chroot that belongs to "user".
     The folder gets deleted, if it already exists.
 
     :param path: of the temporary folder inside the chroot
     :returns: the path
     """
     if os.path.exists(args.work + "/chroot_" + suffix + path):
         pmb.chroot.root(args, ["rm", "-r", path])
```

### Comparing `pmbootstrap-1.9.0/pmb/chroot/init.py` & `pmbootstrap-2.0.0/pmb/chroot/init.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,109 +1,129 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 import os
 import glob
 import filecmp
 
 import pmb.chroot
 import pmb.chroot.apk_static
 import pmb.config
+import pmb.config.workdir
 import pmb.helpers.repo
 import pmb.helpers.run
 import pmb.parse.arch
 
 
 def copy_resolv_conf(args, suffix="native"):
     """
     Use pythons super fast file compare function (due to caching)
     and copy the /etc/resolv.conf to the chroot, in case it is
     different from the host.
     If the file doesn't exist, create an empty file with 'touch'.
     """
     host = "/etc/resolv.conf"
-    chroot = args.work + "/chroot_" + suffix + host
+    chroot = f"{args.work}/chroot_{suffix}{host}"
     if os.path.exists(host):
         if not os.path.exists(chroot) or not filecmp.cmp(host, chroot):
             pmb.helpers.run.root(args, ["cp", host, chroot])
     else:
         pmb.helpers.run.root(args, ["touch", chroot])
 
 
+def mark_in_chroot(args, suffix="native"):
+    """
+    Touch a flag so we can know when we're running in chroot (and
+    don't accidentally flash partitions on our host). This marker
+    gets removed in pmb.chroot.shutdown (pmbootstrap shutdown).
+    """
+    in_chroot_file = f"{args.work}/chroot_{suffix}/in-pmbootstrap"
+    if not os.path.exists(in_chroot_file):
+        pmb.helpers.run.root(args, ["touch", in_chroot_file])
+
+
+def setup_qemu_emulation(args, suffix):
+    arch = pmb.parse.arch.from_chroot_suffix(args, suffix)
+    if not pmb.parse.arch.cpu_emulation_required(arch):
+        return
+
+    chroot = f"{args.work}/chroot_{suffix}"
+    arch_qemu = pmb.parse.arch.alpine_to_qemu(arch)
+
+    # mount --bind the qemu-user binary
+    pmb.chroot.binfmt.register(args, arch)
+    pmb.helpers.mount.bind_file(args, f"{args.work}/chroot_native"
+                                      f"/usr/bin/qemu-{arch_qemu}",
+                                f"{chroot}/usr/bin/qemu-{arch_qemu}-static",
+                                create_folders=True)
+
+
+def init_keys(args):
+    """
+    All Alpine and postmarketOS repository keys are shipped with pmbootstrap.
+    Copy them into $WORK/config_apk_keys, which gets mounted inside the various
+    chroots as /etc/apk/keys.
+
+    This is done before installing any package, so apk can verify APKINDEX
+    files of binary repositories even though alpine-keys/postmarketos-keys are
+    not installed yet.
+    """
+    for key in glob.glob(f"{pmb.config.apk_keys_path}/*.pub"):
+        target = f"{args.work}/config_apk_keys/{os.path.basename(key)}"
+        if not os.path.exists(target):
+            # Copy as root, so the resulting files in chroots are owned by root
+            pmb.helpers.run.root(args, ["cp", key, target])
+
+
 def init(args, suffix="native"):
     # When already initialized: just prepare the chroot
-    chroot = args.work + "/chroot_" + suffix
+    chroot = f"{args.work}/chroot_{suffix}"
     arch = pmb.parse.arch.from_chroot_suffix(args, suffix)
-    emulate = pmb.parse.arch.cpu_emulation_required(args, arch)
 
     pmb.chroot.mount(args, suffix)
-    if os.path.islink(chroot + "/bin/sh"):
-        if emulate:
-            pmb.chroot.binfmt.register(args, arch)
+    setup_qemu_emulation(args, suffix)
+    mark_in_chroot(args, suffix)
+    if os.path.islink(f"{chroot}/bin/sh"):
+        pmb.config.workdir.chroot_check_channel(args, suffix)
         copy_resolv_conf(args, suffix)
         pmb.chroot.apk.update_repository_list(args, suffix)
         return
 
     # Require apk-tools-static
     pmb.chroot.apk_static.init(args)
 
-    # Non-native chroot: set up QEMU with binfmt_misc
-    if emulate:
-        pmb.chroot.binfmt.register(args, arch)
-
-    logging.info("(" + suffix + ") install alpine-base")
+    logging.info(f"({suffix}) install alpine-base")
 
     # Initialize cache
-    apk_cache = args.work + "/cache_apk_" + arch
-    pmb.helpers.run.root(args, ["ln", "-s", "-f", "/var/cache/apk", chroot +
-                                "/etc/apk/cache"])
+    apk_cache = f"{args.work}/cache_apk_{arch}"
+    pmb.helpers.run.root(args, ["ln", "-s", "-f", "/var/cache/apk",
+                                f"{chroot}/etc/apk/cache"])
 
     # Initialize /etc/apk/keys/, resolv.conf, repositories
-    for key in glob.glob(pmb.config.apk_keys_path + "/*.pub"):
-        pmb.helpers.run.root(args, ["cp", key, args.work +
-                                    "/config_apk_keys/"])
+    init_keys(args)
     copy_resolv_conf(args, suffix)
     pmb.chroot.apk.update_repository_list(args, suffix)
 
-    # Non-native chroot: install qemu-user-binary
-    if emulate:
-        arch_qemu = pmb.parse.arch.alpine_to_qemu(arch)
-        pmb.helpers.run.root(args, ["mkdir", "-p", chroot + "/usr/bin"])
-        pmb.helpers.run.root(args, ["cp", args.work +
-                                    "/chroot_native/usr/bin/qemu-" + arch_qemu,
-                                    chroot + "/usr/bin/qemu-" + arch_qemu + "-static"])
+    pmb.config.workdir.chroot_save_init(args, suffix)
 
     # Install alpine-base
     pmb.helpers.repo.update(args, arch)
-    pmb.chroot.apk_static.run(args, ["--no-progress", "--root", chroot,
-                                     "--cache-dir", apk_cache, "--initdb", "--arch", arch,
+    pmb.chroot.apk_static.run(args, ["--root", chroot,
+                                     "--cache-dir", apk_cache,
+                                     "--initdb", "--arch", arch,
                                      "add", "alpine-base"])
 
     # Building chroots: create "pmos" user, add symlinks to /home/pmos
     if not suffix.startswith("rootfs_"):
         pmb.chroot.root(args, ["adduser", "-D", "pmos", "-u",
-                               pmb.config.chroot_uid_user], suffix, auto_init=False)
+                               pmb.config.chroot_uid_user],
+                        suffix, auto_init=False)
 
         # Create the links (with subfolders if necessary)
         for target, link_name in pmb.config.chroot_home_symlinks.items():
             link_dir = os.path.dirname(link_name)
-            if not os.path.exists(chroot + link_dir):
+            if not os.path.exists(f"{chroot}{link_dir}"):
                 pmb.chroot.user(args, ["mkdir", "-p", link_dir], suffix)
+            if not os.path.exists(f"{chroot}{target}"):
+                pmb.chroot.root(args, ["mkdir", "-p", target], suffix)
             pmb.chroot.user(args, ["ln", "-s", target, link_name], suffix)
-            pmb.chroot.root(args, ["chown", "pmos:pmos", target],
-                            suffix)
+            pmb.chroot.root(args, ["chown", "pmos:pmos", target], suffix)
```

### Comparing `pmbootstrap-1.9.0/pmb/chroot/root.py` & `pmbootstrap-2.0.0/pmb/chroot/root.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import os
 import shutil
 
 import pmb.config
 import pmb.chroot
 import pmb.chroot.binfmt
 import pmb.helpers.run
@@ -30,62 +14,68 @@
     """
     Get the absolute paths to the sh and chroot executables.
     """
     ret = {}
     for binary in ["sh", "chroot"]:
         path = shutil.which(binary, path=pmb.config.chroot_host_path)
         if not path:
-            raise RuntimeError("Could not find the '" + binary +
-                               "' executable. Make sure, that it is in" " your current user's PATH.")
+            raise RuntimeError(f"Could not find the '{binary}'"
+                               " executable. Make sure that it is in"
+                               " your current user's PATH.")
         ret[binary] = path
     return ret
 
 
 def root(args, cmd, suffix="native", working_dir="/", output="log",
-         output_return=False, check=None, env={}, auto_init=True):
+         output_return=False, check=None, env={}, auto_init=True,
+         disable_timeout=False):
     """
     Run a command inside a chroot as root.
 
     :param env: dict of environment variables to be passed to the command, e.g.
                 {"JOBS": "5"}
     :param auto_init: automatically initialize the chroot
 
     See pmb.helpers.run_core.core() for a detailed description of all other
     arguments and the return value.
     """
     # Initialize chroot
-    chroot = args.work + "/chroot_" + suffix
-    if not auto_init and not os.path.islink(chroot + "/bin/sh"):
-        raise RuntimeError("Chroot does not exist: " + chroot)
+    chroot = f"{args.work}/chroot_{suffix}"
+    if not auto_init and not os.path.islink(f"{chroot}/bin/sh"):
+        raise RuntimeError(f"Chroot does not exist: {chroot}")
     if auto_init:
         pmb.chroot.init(args, suffix)
 
     # Readable log message (without all the escaping)
-    msg = "(" + suffix + ") % "
+    msg = f"({suffix}) % "
     for key, value in env.items():
-        msg += key + "=" + value + " "
+        msg += f"{key}={value} "
     if working_dir != "/":
-        msg += "cd " + working_dir + "; "
+        msg += f"cd {working_dir}; "
     msg += " ".join(cmd)
 
     # Merge env with defaults into env_all
     env_all = {"CHARSET": "UTF-8",
                "HISTFILE": "~/.ash_history",
                "HOME": "/root",
+               "LANG": "UTF-8",
                "PATH": pmb.config.chroot_path,
+               "PYTHONUNBUFFERED": "1",
                "SHELL": "/bin/ash",
                "TERM": "xterm"}
     for key, value in env.items():
         env_all[key] = value
 
     # Build the command in steps and run it, e.g.:
     # cmd: ["echo", "test"]
     # cmd_chroot: ["/sbin/chroot", "/..._native", "/bin/sh", "-c", "echo test"]
     # cmd_sudo: ["sudo", "env", "-i", "sh", "-c", "PATH=... /sbin/chroot ..."]
     executables = executables_absolute_path()
     cmd_chroot = [executables["chroot"], chroot, "/bin/sh", "-c",
-                  pmb.helpers.run.flat_cmd(cmd, working_dir)]
-    cmd_sudo = ["sudo", "env", "-i", executables["sh"], "-c",
-                pmb.helpers.run.flat_cmd(cmd_chroot, env=env_all)]
-    kill_as_root = output in ["log", "stdout"]
+                  pmb.helpers.run_core.flat_cmd(cmd, working_dir)]
+    cmd_sudo = pmb.config.sudo([
+        "env", "-i", executables["sh"], "-c",
+        pmb.helpers.run_core.flat_cmd(cmd_chroot, env=env_all)]
+    )
     return pmb.helpers.run_core.core(args, msg, cmd_sudo, None, output,
-                                     output_return, check, kill_as_root)
+                                     output_return, check, True,
+                                     disable_timeout)
```

### Comparing `pmbootstrap-1.9.0/pmb/chroot/initfs.py` & `pmbootstrap-2.0.0/pmb/chroot/initfs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,84 +1,77 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import os
 import logging
 import pmb.chroot.initfs_hooks
 import pmb.chroot.other
 import pmb.chroot.apk
+import pmb.config.pmaports
 import pmb.helpers.cli
 
 
 def build(args, flavor, suffix):
-    # Bail out when '-s' is set
-    if args.skip_initfs:
-        logging.info("NOTE: Skipped initramfs generation (-s)!")
-        return
-
     # Update mkinitfs and hooks
     pmb.chroot.apk.install(args, ["postmarketos-mkinitfs"], suffix)
     pmb.chroot.initfs_hooks.update(args, suffix)
+    pmaports_cfg = pmb.config.pmaports.read_config(args)
 
     # Call mkinitfs
-    logging.info("(" + suffix + ") mkinitfs " + flavor)
-    release_file = (args.work + "/chroot_" + suffix + "/usr/share/kernel/" +
-                    flavor + "/kernel.release")
-    with open(release_file, "r") as handle:
-        release = handle.read().rstrip()
-    pmb.chroot.root(args, ["mkinitfs", "-o", "/boot/initramfs-" + flavor, release],
-                    suffix)
+    logging.info(f"({suffix}) mkinitfs {flavor}")
+    if pmaports_cfg.get("supported_mkinitfs_without_flavors", False):
+        pmb.chroot.root(args, ["mkinitfs"], suffix)
+    else:
+        release_file = (f"{args.work}/chroot_{suffix}/usr/share/kernel/"
+                        f"{flavor}/kernel.release")
+        with open(release_file, "r") as handle:
+            release = handle.read().rstrip()
+            pmb.chroot.root(args, ["mkinitfs", "-o",
+                                   f"/boot/initramfs-{flavor}", release],
+                            suffix)
 
 
 def extract(args, flavor, suffix, extra=False):
     """
     Extract the initramfs to /tmp/initfs-extracted or the initramfs-extra to
     /tmp/initfs-extra-extracted and return the outside extraction path.
     """
     # Extraction folder
     inside = "/tmp/initfs-extracted"
+
+    pmaports_cfg = pmb.config.pmaports.read_config(args)
+    if pmaports_cfg.get("supported_mkinitfs_without_flavors", False):
+        initfs_file = "/boot/initramfs"
+    else:
+        initfs_file = f"/boot/initramfs-${flavor}"
     if extra:
         inside = "/tmp/initfs-extra-extracted"
-        flavor += "-extra"
-    outside = args.work + "/chroot_" + suffix + inside
+        initfs_file += "-extra"
+
+    outside = f"{args.work}/chroot_{suffix}{inside}"
     if os.path.exists(outside):
-        if not pmb.helpers.cli.confirm(args, "Extraction folder " + outside +
-                                       " already exists. Do you want to overwrite it?"):
+        if not pmb.helpers.cli.confirm(args, f"Extraction folder {outside}"
+                                       " already exists."
+                                       " Do you want to overwrite it?"):
             raise RuntimeError("Aborted!")
         pmb.chroot.root(args, ["rm", "-r", inside], suffix)
 
     # Extraction script (because passing a file to stdin is not allowed
     # in pmbootstrap's chroot/shell functions for security reasons)
-    with open(args.work + "/chroot_" + suffix + "/tmp/_extract.sh", "w") as handle:
+    with open(f"{args.work}/chroot_{suffix}/tmp/_extract.sh", "w") as handle:
         handle.write(
             "#!/bin/sh\n"
-            "cd " + inside + " && cpio -i < _initfs\n")
+            f"cd {inside} && cpio -i < _initfs\n")
 
     # Extract
     commands = [["mkdir", "-p", inside],
-                ["cp", "/boot/initramfs-" + flavor, inside + "/_initfs.gz"],
-                ["gzip", "-d", inside + "/_initfs.gz"],
+                ["cp", initfs_file, f"{inside}/_initfs.gz"],
+                ["gzip", "-d", f"{inside}/_initfs.gz"],
                 ["cat", "/tmp/_extract.sh"],  # for the log
                 ["sh", "/tmp/_extract.sh"],
-                ["rm", "/tmp/_extract.sh", inside + "/_initfs"]
+                ["rm", "/tmp/_extract.sh", f"{inside}/_initfs"]
                 ]
     for command in commands:
         pmb.chroot.root(args, command, suffix)
 
     # Return outside path for logging
     return outside
 
@@ -90,29 +83,26 @@
     extract(args, flavor, suffix, extra)
     pmb.chroot.root(args, ["ls", "-lahR", "."], suffix, tmp, "stdout")
     pmb.chroot.root(args, ["rm", "-r", tmp], suffix)
 
 
 def frontend(args):
     # Find the appropriate kernel flavor
-    suffix = "rootfs_" + args.device
-    flavors = pmb.chroot.other.kernel_flavors_installed(args, suffix)
-    flavor = flavors[0]
-    if hasattr(args, "flavor") and args.flavor:
-        flavor = args.flavor
+    suffix = f"rootfs_{args.device}"
+    flavor = pmb.chroot.other.kernel_flavor_installed(args, suffix)
 
     # Handle initfs actions
     action = args.action_initfs
     if action == "build":
         build(args, flavor, suffix)
     elif action == "extract":
         dir = extract(args, flavor, suffix)
-        logging.info("Successfully extracted initramfs to: " + dir)
+        logging.info(f"Successfully extracted initramfs to: {dir}")
         dir_extra = extract(args, flavor, suffix, True)
-        logging.info("Successfully extracted initramfs-extra to: " + dir_extra)
+        logging.info(f"Successfully extracted initramfs-extra to: {dir_extra}")
     elif action == "ls":
         logging.info("*** initramfs ***")
         ls(args, flavor, suffix)
         logging.info("*** initramfs-extra ***")
         ls(args, flavor, suffix, True)
 
     # Handle hook actions
@@ -120,14 +110,13 @@
         pmb.chroot.initfs_hooks.ls(args, suffix)
     else:
         if action == "hook_add":
             pmb.chroot.initfs_hooks.add(args, args.hook, suffix)
         elif action == "hook_del":
             pmb.chroot.initfs_hooks.delete(args, args.hook, suffix)
 
-        # Rebuild the initfs for all kernels after adding/removing a hook
-        for flavor in flavors:
-            build(args, flavor, suffix)
+        # Rebuild the initfs after adding/removing a hook
+        build(args, flavor, suffix)
 
     if action in ["ls", "extract"]:
         link = "https://wiki.postmarketos.org/wiki/Initramfs_development"
-        logging.info("See also: <" + link + ">")
+        logging.info(f"See also: <{link}>")
```

### Comparing `pmbootstrap-1.9.0/pmb/chroot/apk.py` & `pmbootstrap-2.0.0/pmb/chroot/apk.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,16 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import os
 import logging
 import shlex
 
 import pmb.chroot
 import pmb.config
+import pmb.helpers.apk
 import pmb.helpers.pmaports
 import pmb.parse.apkindex
 import pmb.parse.arch
 import pmb.parse.depends
 import pmb.parse.version
 
 
@@ -36,219 +21,230 @@
 
     :param check: This function calls it self after updating the
                   /etc/apk/repositories file, to check if it was successful.
                   Only for this purpose, the "check" parameter should be set to
                   True.
     """
     # Skip if we already did this
-    if suffix in args.cache["apk_repository_list_updated"]:
+    if suffix in pmb.helpers.other.cache["apk_repository_list_updated"]:
         return
 
     # Read old entries or create folder structure
-    path = args.work + "/chroot_" + suffix + "/etc/apk/repositories"
+    path = f"{args.work}/chroot_{suffix}/etc/apk/repositories"
     lines_old = []
     if os.path.exists(path):
         # Read all old lines
         lines_old = []
         with open(path) as handle:
             for line in handle:
                 lines_old.append(line[:-1])
     else:
         pmb.helpers.run.root(args, ["mkdir", "-p", os.path.dirname(path)])
 
     # Up to date: Save cache, return
     lines_new = pmb.helpers.repo.urls(args)
     if lines_old == lines_new:
-        args.cache["apk_repository_list_updated"].append(suffix)
+        pmb.helpers.other.cache["apk_repository_list_updated"].append(suffix)
         return
 
     # Check phase: raise error when still outdated
     if check:
-        raise RuntimeError("Failed to update: " + path)
+        raise RuntimeError(f"Failed to update: {path}")
 
     # Update the file
-    logging.debug("(" + suffix + ") update /etc/apk/repositories")
+    logging.debug(f"({suffix}) update /etc/apk/repositories")
     if os.path.exists(path):
         pmb.helpers.run.root(args, ["rm", path])
     for line in lines_new:
-        pmb.helpers.run.root(args, ["sh", "-c", "echo " +
-                                    shlex.quote(line) + " >> " + path])
+        pmb.helpers.run.root(args, ["sh", "-c", "echo "
+                                    f"{shlex.quote(line)} >> {path}"])
     update_repository_list(args, suffix, True)
 
 
 def check_min_version(args, suffix="native"):
     """
     Check the minimum apk version, before running it the first time in the
     current session (lifetime of one pmbootstrap call).
     """
 
     # Skip if we already did this
-    if suffix in args.cache["apk_min_version_checked"]:
+    if suffix in pmb.helpers.other.cache["apk_min_version_checked"]:
         return
 
     # Skip if apk is not installed yet
-    if not os.path.exists(args.work + "/chroot_" + suffix + "/sbin/apk"):
-        logging.debug("NOTE: Skipped apk version check for chroot '" + suffix +
-                      "', because it is not installed yet!")
+    if not os.path.exists(f"{args.work}/chroot_{suffix}/sbin/apk"):
+        logging.debug(f"NOTE: Skipped apk version check for chroot '{suffix}'"
+                      ", because it is not installed yet!")
         return
 
     # Compare
     version_installed = installed(args, suffix)["apk-tools"]["version"]
-    version_min = pmb.config.apk_tools_static_min_version
-    if pmb.parse.version.compare(version_installed, version_min) == -1:
-        raise RuntimeError("You have an outdated version of the 'apk' package"
-                           " manager installed (your version: " + version_installed +
-                           ", expected at least: " + version_min + "). Delete"
-                           " your http cache and zap all chroots, then try again:"
-                           " 'pmbootstrap zap -hc'")
+    pmb.helpers.apk.check_outdated(
+        args, version_installed,
+        "Delete your http cache and zap all chroots, then try again:"
+        " 'pmbootstrap zap -hc'")
 
     # Mark this suffix as checked
-    args.cache["apk_min_version_checked"].append(suffix)
+    pmb.helpers.other.cache["apk_min_version_checked"].append(suffix)
 
 
-def install_is_necessary(args, build, arch, package, packages_installed):
+def install_build(args, package, arch):
     """
-    This function optionally builds an out of date package, and checks if the
-    version installed inside a chroot is up to date.
-    :param build: Set to true to build the package, if the binary packages are
-                  out of date, and it is in the aports folder.
-    :param packages_installed: Return value from installed().
-    :returns: True if the package needs to be installed/updated, False otherwise.
+    Build an outdated package unless pmbootstrap was invoked with
+    "pmbootstrap install" and the option to build packages during pmb install
+    is disabled.
+
+    :param package: name of the package to build
+    :param arch: architecture of the package to build
+    """
+    # User may have disabled building packages during "pmbootstrap install"
+    if args.action == "install" and not args.build_pkgs_on_install:
+        if not pmb.parse.apkindex.package(args, package, arch, False):
+            raise RuntimeError(f"{package}: no binary package found for"
+                               f" {arch}, and compiling packages during"
+                               " 'pmbootstrap install' has been disabled."
+                               " Consider changing this option in"
+                               " 'pmbootstrap init'.")
+        # Use the existing binary package
+        return
+
+    # Build the package if it's in pmaports and there is no binary package
+    # with the same pkgver and pkgrel. This check is done in
+    # pmb.build.is_necessary, which gets called in pmb.build.package.
+    return pmb.build.package(args, package, arch)
+
+
+def packages_split_to_add_del(packages):
     """
-    # Build package
-    if build:
-        pmb.build.package(args, package, arch)
+    Sort packages into "to_add" and "to_del" lists depending on their pkgname
+    starting with an exclamation mark.
 
-    # No further checks when not installed
-    if package not in packages_installed:
-        return True
-
-    # Make sure, that we really have a binary package
-    data_repo = pmb.parse.apkindex.package(args, package, arch, False)
-    if not data_repo:
-        logging.warning("WARNING: Internal error in pmbootstrap," +
-                        " package '" + package + "' for " + arch +
-                        " has not been built yet, but it should have"
-                        " been. Rebuilding it with force. Please "
-                        " report this, if there is no ticket about this"
-                        " yet!")
-        pmb.build.package(args, package, arch, True)
-        return install_is_necessary(args, build, arch, package,
-                                    packages_installed)
-
-    # Compare the installed version vs. the version in the repos
-    data_installed = packages_installed[package]
-    compare = pmb.parse.version.compare(data_installed["version"],
-                                        data_repo["version"])
-    # a) Installed newer (should not happen normally)
-    if compare == 1:
-        logging.info("WARNING: " + arch + " package '" + package +
-                     "' installed version " + data_installed["version"] +
-                     " is newer, than the version in the repositories: " +
-                     data_repo["version"] +
-                     " See also: <https://postmarketos.org/warning-repo>")
-        return False
-
-    # b) Repo newer
-    elif compare == -1:
-        return True
-
-    # c) Same version, look at last modified
-    elif compare == 0:
-        time_installed = float(data_installed["timestamp"])
-        time_repo = float(data_repo["timestamp"])
-        return time_repo > time_installed
-
-
-def replace_aports_packages_with_path(args, packages, suffix, arch):
-    """
-    apk will only re-install packages with the same pkgname, pkgver and pkgrel,
-    when you give it the absolute path to the package. This function replaces
-    all packages, that were built locally, with the absolute path to the package.
+    :param packages: list of pkgnames
+    :returns: (to_add, to_del) - tuple of lists of pkgnames, e.g.
+              (["hello-world", ...], ["some-conflict-pkg", ...])
     """
-    ret = []
+    to_add = []
+    to_del = []
+
     for package in packages:
-        aport = pmb.helpers.pmaports.find(args, package, False)
-        if aport:
-            data_repo = pmb.parse.apkindex.package(args, package, arch, False)
-            apk_path = ("/mnt/pmbootstrap-packages/" + arch + "/" +
-                        package + "-" + data_repo["version"] + ".apk")
-            if os.path.exists(args.work + "/chroot_" + suffix + apk_path):
-                package = apk_path
-        ret.append(package)
-    return ret
+        if package.startswith("!"):
+            to_del.append(package.lstrip("!"))
+        else:
+            to_add.append(package)
 
+    return (to_add, to_del)
 
-def install(args, packages, suffix="native", build=True):
+
+def packages_get_locally_built_apks(args, packages, arch):
     """
-    :param build: automatically build the package, when it does not exist yet
-                  or needs to be updated, and it is inside the pm-aports
-                  folder. Checking this is expensive - if you know, that all
-                  packages are provides by upstream repos, set this to False!
+    Iterate over packages and if existing, get paths to locally built packages.
+    This is used to force apk to upgrade packages to newer local versions, even
+    if the pkgver and pkgrel did not change.
+
+    :param packages: list of pkgnames
+    :param arch: architecture that the locally built packages should have
+    :returns: list of apk file paths that are valid inside the chroots, e.g.
+              ["/mnt/pmbootstrap-packages/x86_64/hello-world-1-r6.apk", ...]
     """
-    # Initialize chroot
-    check_min_version(args, suffix)
-    pmb.chroot.init(args, suffix)
+    channel = pmb.config.pmaports.read_config(args)["channel"]
+    ret = []
 
-    # Add depends to packages
-    arch = pmb.parse.arch.from_chroot_suffix(args, suffix)
-    packages_with_depends = pmb.parse.depends.recurse(args, packages, suffix)
+    for package in packages:
+        data_repo = pmb.parse.apkindex.package(args, package, arch, False)
+        if not data_repo:
+            continue
+
+        apk_file = f"{package}-{data_repo['version']}.apk"
+        if not os.path.exists(f"{args.work}/packages/{channel}/{arch}/{apk_file}"):
+            continue
 
-    # Filter outdated packages (build them if required)
-    packages_installed = installed(args, suffix)
-    packages_todo = []
-    for package in packages_with_depends:
-        if install_is_necessary(
-                args, build, arch, package, packages_installed):
-            packages_todo.append(package)
-    if not len(packages_todo):
-        return
+        ret.append(f"/mnt/pmbootstrap-packages/{arch}/{apk_file}")
 
+    return ret
+
+
+def install_run_apk(args, to_add, to_add_local, to_del, suffix):
+    """
+    Run apk to add packages, and ensure only the desired packages get
+    explicitly marked as installed.
+
+    :param to_add: list of pkgnames to install, without their dependencies
+    :param to_add_local: return of packages_get_locally_built_apks()
+    :param to_del: list of pkgnames to be deleted, this should be set to
+                   conflicting dependencies in any of the packages to be
+                   installed or their dependencies (e.g. ["osk-sdl"])
+    :param suffix: the chroot suffix, e.g. "native" or "rootfs_qemu-amd64"
+    """
     # Sanitize packages: don't allow '--allow-untrusted' and other options
     # to be passed to apk!
-    for package in packages_todo:
+    for package in to_add + to_add_local + to_del:
         if package.startswith("-"):
-            raise ValueError("Invalid package name: " + package)
+            raise ValueError(f"Invalid package name: {package}")
 
-    # Readable install message without dependencies
-    message = "(" + suffix + ") install"
-    for pkgname in packages:
-        if pkgname not in packages_installed:
-            message += " " + pkgname
-    logging.info(message)
-
-    # Local packages: Using the path instead of pkgname makes apk update
-    # packages of the same version if the build date is different
-    packages_todo = replace_aports_packages_with_path(args, packages_todo,
-                                                      suffix, arch)
+    commands = [["add"] + to_add]
 
     # Use a virtual package to mark only the explicitly requested packages as
-    # explicitly installed, not their dependencies or specific paths (#1212)
-    commands = [["add"] + packages]
-    if packages != packages_todo:
-        commands = [["add", "-u", "--virtual", ".pmbootstrap"] + packages_todo,
-                    ["add"] + packages,
-                    ["del", ".pmbootstrap"]]
-    for command in commands:
+    # explicitly installed, not the ones in to_add_local
+    if to_add_local:
+        commands += [["add", "-u", "--virtual", ".pmbootstrap"] + to_add_local,
+                     ["del", ".pmbootstrap"]]
+
+    if to_del:
+        commands += [["del"] + to_del]
+
+    for (i, command) in enumerate(commands):
         if args.offline:
             command = ["--no-network"] + command
-        pmb.chroot.root(args, ["apk", "--no-progress"] + command, suffix)
+        if i == 0:
+            pmb.helpers.apk.apk_with_progress(args, ["apk"] + command,
+                                              chroot=True, suffix=suffix)
+        else:
+            # Virtual package related commands don't actually install or remove
+            # packages, but only mark the right ones as explicitly installed.
+            # They finish up almost instantly, so don't display a progress bar.
+            pmb.chroot.root(args, ["apk", "--no-progress"] + command,
+                            suffix=suffix)
 
 
-def upgrade(args, suffix="native"):
+def install(args, packages, suffix="native", build=True):
     """
-    Upgrade all packages installed in a chroot
+    Install packages from pmbootstrap's local package index or the pmOS/Alpine
+    binary package mirrors. Iterate over all dependencies recursively, and
+    build missing packages as necessary.
+
+    :param packages: list of pkgnames to be installed
+    :param suffix: the chroot suffix, e.g. "native" or "rootfs_qemu-amd64"
+    :param build: automatically build the package, when it does not exist yet
+                  or needs to be updated, and it is inside pmaports. For the
+                  special case that all packages are expected to be in Alpine's
+                  repositories, set this to False for performance optimization.
     """
-    # Update APKINDEX files
     arch = pmb.parse.arch.from_chroot_suffix(args, suffix)
-    pmb.helpers.repo.update(args, arch)
 
-    # Rebuild and upgrade out-of-date packages
-    packages = list(installed(args, suffix).keys())
-    install(args, packages, suffix)
+    if not packages:
+        logging.verbose("pmb.chroot.apk.install called with empty packages list,"
+                        " ignoring")
+        return
+
+    # Initialize chroot
+    check_min_version(args, suffix)
+    pmb.chroot.init(args, suffix)
+
+    packages_with_depends = pmb.parse.depends.recurse(args, packages, suffix)
+    to_add, to_del = packages_split_to_add_del(packages_with_depends)
+
+    if build:
+        for package in to_add:
+            install_build(args, package, arch)
+
+    to_add_local = packages_get_locally_built_apks(args, to_add, arch)
+    to_add_no_deps, _ = packages_split_to_add_del(packages)
+
+    logging.info(f"({suffix}) install {' '.join(to_add_no_deps)}")
+    install_run_apk(args, to_add_no_deps, to_add_local, to_del, suffix)
 
 
 def installed(args, suffix="native"):
     """
     Read the list of installed packages (which has almost the same format, as
     an APKINDEX, but with more keys).
 
@@ -258,9 +254,9 @@
                   "pkgname": "postmarketos-mkinitfs"
                   "version": "0.0.4-r10",
                   "depends": ["busybox-extras", "lddtree", ...],
                   "provides": ["mkinitfs=0.0.1"]
                 }, ...
               }
     """
-    path = args.work + "/chroot_" + suffix + "/lib/apk/db/installed"
-    return pmb.parse.apkindex.parse(args, path, False)
+    path = f"{args.work}/chroot_{suffix}/lib/apk/db/installed"
+    return pmb.parse.apkindex.parse(path, False)
```

### Comparing `pmbootstrap-1.9.0/pmb/chroot/zap.py` & `pmbootstrap-2.0.0/pmb/chroot/zap.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,164 +1,171 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import glob
 import logging
 import math
 import os
 
 import pmb.chroot
+import pmb.config.pmaports
+import pmb.config.workdir
 import pmb.helpers.pmaports
 import pmb.helpers.run
 import pmb.parse.apkindex
 
 
 def zap(args, confirm=True, dry=False, pkgs_local=False, http=False,
-        pkgs_local_mismatch=False, pkgs_online_mismatch=False, distfiles=False):
+        pkgs_local_mismatch=False, pkgs_online_mismatch=False, distfiles=False,
+        rust=False, netboot=False):
     """
-    Shutdown everything inside the chroots (e.g. distccd, adb), umount
+    Shutdown everything inside the chroots (e.g. adb), umount
     everything and then safely remove folders from the work-directory.
 
     :param dry: Only show what would be deleted, do not delete for real
     :param pkgs_local: Remove *all* self-compiled packages (!)
     :param http: Clear the http cache (used e.g. for the initial apk download)
-    :param pkgs_local_mismatch: Remove the packages, that have a different version
-                          compared to what is in the aports folder.
-    :param pkgs_online_mismatch: Clean out outdated binary packages downloaded from
-                     mirrors (e.g. from Alpine)
+    :param pkgs_local_mismatch: Remove the packages that have
+        a different version compared to what is in the aports folder.
+    :param pkgs_online_mismatch: Clean out outdated binary packages
+        downloaded from mirrors (e.g. from Alpine)
     :param distfiles: Clear the downloaded files cache
+    :param rust: Remove rust related caches
+    :param netboot: Remove images for netboot
 
     NOTE: This function gets called in pmb/config/init.py, with only args.work
     and args.device set!
     """
     # Get current work folder size
     if not dry:
         pmb.chroot.shutdown(args)
         logging.debug("Calculate work folder size")
         size_old = pmb.helpers.other.folder_size(args, args.work)
 
-    # Delete packages with a different version compared to aports, then re-index
+    # Delete packages with a different version compared to aports,
+    # then re-index
     if pkgs_local_mismatch:
         zap_pkgs_local_mismatch(args, confirm, dry)
 
     # Delete outdated binary packages
     if pkgs_online_mismatch:
         zap_pkgs_online_mismatch(args, confirm, dry)
 
     pmb.chroot.shutdown(args)
 
     # Deletion patterns for folders inside args.work
     patterns = [
         "chroot_native",
         "chroot_buildroot_*",
+        "chroot_installer_*",
         "chroot_rootfs_*",
     ]
     if pkgs_local:
         patterns += ["packages"]
     if http:
         patterns += ["cache_http"]
     if distfiles:
         patterns += ["cache_distfiles"]
+    if rust:
+        patterns += ["cache_rust"]
+    if netboot:
+        patterns += ["images_netboot"]
 
     # Delete everything matching the patterns
     for pattern in patterns:
-        pattern = os.path.realpath(args.work + "/" + pattern)
+        pattern = os.path.realpath(f"{args.work}/{pattern}")
         matches = glob.glob(pattern)
         for match in matches:
-            if not confirm or pmb.helpers.cli.confirm(args, "Remove " + match + "?"):
-                logging.info("% rm -rf " + match)
+            if (not confirm or
+                    pmb.helpers.cli.confirm(args, f"Remove {match}?")):
+                logging.info(f"% rm -rf {match}")
                 if not dry:
                     pmb.helpers.run.root(args, ["rm", "-rf", match])
 
+    # Remove config init dates for deleted chroots
+    pmb.config.workdir.clean(args)
+
     # Chroots were zapped, so no repo lists exist anymore
-    args.cache["apk_repository_list_updated"].clear()
+    pmb.helpers.other.cache["apk_repository_list_updated"].clear()
 
     # Print amount of cleaned up space
     if dry:
         logging.info("Dry run: nothing has been deleted")
     else:
         size_new = pmb.helpers.other.folder_size(args, args.work)
-        mb = (size_old - size_new) / 1024 / 1024
-        logging.info("Cleared up ~" + str(math.ceil(mb)) + " MB of space")
+        mb = (size_old - size_new) / 1024
+        logging.info(f"Cleared up ~{math.ceil(mb)} MB of space")
 
 
 def zap_pkgs_local_mismatch(args, confirm=True, dry=False):
-    if not os.path.exists(args.work + "/packages/"):
+    channel = pmb.config.pmaports.read_config(args)["channel"]
+    if not os.path.exists(f"{args.work}/packages/{channel}"):
         return
-    if confirm and not pmb.helpers.cli.confirm(args, "Remove packages that are newer than"
-                                               " the corresponding package in aports?"):
+
+    question = "Remove binary packages that are newer than the corresponding" \
+               f" pmaports (channel '{channel}')?"
+    if confirm and not pmb.helpers.cli.confirm(args, question):
         return
 
     reindex = False
-    for apkindex_path in glob.glob(args.work + "/packages/*/APKINDEX.tar.gz"):
+    pattern = f"{args.work}/packages/{channel}/*/APKINDEX.tar.gz"
+    for apkindex_path in glob.glob(pattern):
         # Delete packages without same version in aports
-        blocks = pmb.parse.apkindex.parse_blocks(args, apkindex_path)
+        blocks = pmb.parse.apkindex.parse_blocks(apkindex_path)
         for block in blocks:
             pkgname = block["pkgname"]
             origin = block["origin"]
             version = block["version"]
             arch = block["arch"]
 
             # Apk path
-            apk_path_short = arch + "/" + pkgname + "-" + version + ".apk"
-            apk_path = args.work + "/packages/" + apk_path_short
+            apk_path_short = f"{arch}/{pkgname}-{version}.apk"
+            apk_path = f"{args.work}/packages/{channel}/{apk_path_short}"
             if not os.path.exists(apk_path):
                 logging.info("WARNING: Package mentioned in index not"
-                             " found: " + apk_path_short)
+                             f" found: {apk_path_short}")
                 continue
 
             # Aport path
             aport_path = pmb.helpers.pmaports.find(args, origin, False)
             if not aport_path:
-                logging.info("% rm " + apk_path_short + " (" + origin +
-                             " aport not found)")
+                logging.info(f"% rm {apk_path_short}"
+                             f" ({origin} aport not found)")
                 if not dry:
                     pmb.helpers.run.root(args, ["rm", apk_path])
                     reindex = True
                 continue
 
             # Clear out any binary apks that do not match what is in aports
-            apkbuild = pmb.parse.apkbuild(args, aport_path + "/APKBUILD")
-            version_aport = apkbuild["pkgver"] + "-r" + apkbuild["pkgrel"]
+            apkbuild = pmb.parse.apkbuild(f"{aport_path}/APKBUILD")
+            version_aport = f"{apkbuild['pkgver']}-r{apkbuild['pkgrel']}"
             if version != version_aport:
-                logging.info("% rm " + apk_path_short + " (" + origin +
-                             " aport: " + version_aport + ")")
+                logging.info(f"% rm {apk_path_short}"
+                             f" ({origin} aport: {version_aport})")
                 if not dry:
                     pmb.helpers.run.root(args, ["rm", apk_path])
                     reindex = True
 
     if reindex:
         pmb.build.other.index_repo(args)
 
 
 def zap_pkgs_online_mismatch(args, confirm=True, dry=False):
     # Check whether we need to do anything
-    paths = glob.glob(args.work + "/cache_apk_*")
+    paths = glob.glob(f"{args.work}/cache_apk_*")
     if not len(paths):
         return
-    if confirm and not pmb.helpers.cli.confirm(args, "Remove outdated binary packages?"):
+    if (confirm and not pmb.helpers.cli.confirm(args,
+                                                "Remove outdated"
+                                                " binary packages?")):
         return
 
     # Iterate over existing apk caches
     for path in paths:
         arch = os.path.basename(path).split("_", 2)[2]
-        suffix = "native" if arch == args.arch_native else "buildroot_" + arch
+        suffix = f"buildroot_{arch}"
+        if arch == pmb.config.arch_native:
+            suffix = "native"
 
         # Clean the cache with apk
-        logging.info("(" + suffix + ") apk -v cache clean")
+        logging.info(f"({suffix}) apk -v cache clean")
         if not dry:
             pmb.chroot.root(args, ["apk", "-v", "cache", "clean"], suffix)
```

### Comparing `pmbootstrap-1.9.0/pmb/chroot/mount.py` & `pmbootstrap-2.0.0/pmb/chroot/mount.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import glob
 import logging
 import os
 import pmb.config
 import pmb.parse
 import pmb.helpers.mount
 
@@ -84,25 +68,30 @@
     # Create pts, shm folders and device nodes
     pmb.helpers.run.root(args, ["mkdir", "-p", dev + "/pts", dev + "/shm"])
     pmb.helpers.run.root(args, ["mount", "-t", "tmpfs",
                                 "-o", "nodev,nosuid,noexec",
                                 "tmpfs", dev + "/shm"])
     create_device_nodes(args, suffix)
 
+    # Setup /dev/fd as a symlink
+    pmb.helpers.run.root(args, ["ln", "-sf", "/proc/self/fd", f"{dev}/"])
+
 
 def mount(args, suffix="native"):
     # Mount tmpfs as the chroot's /dev
     mount_dev_tmpfs(args, suffix)
 
     # Get all mountpoints
     arch = pmb.parse.arch.from_chroot_suffix(args, suffix)
+    channel = pmb.config.pmaports.read_config(args)["channel"]
     mountpoints = {}
     for source, target in pmb.config.chroot_mount_bind.items():
         source = source.replace("$WORK", args.work)
         source = source.replace("$ARCH", arch)
+        source = source.replace("$CHANNEL", channel)
         mountpoints[source] = target
 
     # Mount if necessary
     for source, target in mountpoints.items():
         target_full = args.work + "/chroot_" + suffix + target
         pmb.helpers.mount.bind(args, source, target_full)
```

### Comparing `pmbootstrap-1.9.0/pmb/chroot/apk_static.py` & `pmbootstrap-2.0.0/pmb/chroot/apk_static.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,54 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import os
 import logging
 import shutil
 import tarfile
 import tempfile
 import stat
 
+import pmb.helpers.apk
 import pmb.helpers.run
 import pmb.config
 import pmb.config.load
 import pmb.parse.apkindex
 import pmb.helpers.http
 import pmb.parse.version
 
 
 def read_signature_info(tar):
     """
-    Find various information about the signature, that was used to sign
+    Find various information about the signature that was used to sign
     /sbin/apk.static inside the archive (not to be confused with the normal apk
     archive signature!)
 
     :returns: (sigfilename, sigkey_path)
     """
     # Get signature filename and key
     prefix = "sbin/apk.static.SIGN.RSA."
     sigfilename = None
     for filename in tar.getnames():
         if filename.startswith(prefix):
             sigfilename = filename
             break
     if not sigfilename:
-        raise RuntimeError("Could not find signature filename in apk." +
-                           " This means, that your apk file is damaged. Delete it" +
-                           " and try again. If the problem persists, fill out a bug" +
-                           " report.")
+        raise RuntimeError("Could not find signature filename in apk."
+                           " This means that your apk file is damaged."
+                           " Delete it and try again."
+                           " If the problem persists, fill out a bug report.")
     sigkey = sigfilename[len(prefix):]
-    logging.debug("sigfilename: " + sigfilename)
-    logging.debug("sigkey: " + sigkey)
+    logging.debug(f"sigfilename: {sigfilename}")
+    logging.debug(f"sigkey: {sigkey}")
 
     # Get path to keyfile on disk
-    sigkey_path = pmb.config.apk_keys_path + "/" + sigkey
+    sigkey_path = f"{pmb.config.apk_keys_path}/{sigkey}"
     if "/" in sigkey or not os.path.exists(sigkey_path):
-        logging.debug("sigkey_path: " + sigkey_path)
-        raise RuntimeError("Invalid signature key: " + sigkey)
+        logging.debug(f"sigkey_path: {sigkey_path}")
+        raise RuntimeError(f"Invalid signature key: {sigkey}")
 
     return (sigfilename, sigkey_path)
 
 
 def extract_temp(tar, sigfilename):
     """
     Extract apk.static and signature as temporary files.
@@ -82,27 +67,27 @@
         member = tar.getmember(ret[ftype]["filename"])
 
         handle, path = tempfile.mkstemp(ftype, "pmbootstrap")
         handle = open(handle, "wb")
         ret[ftype]["temp_path"] = path
         shutil.copyfileobj(tar.extractfile(member), handle)
 
-        logging.debug("extracted: " + path)
+        logging.debug(f"extracted: {path}")
         handle.close()
     return ret
 
 
 def verify_signature(args, files, sigkey_path):
     """
     Verify the signature with openssl.
 
     :param files: return value from extract_temp()
     :raises RuntimeError: when verification failed and  removes temp files
     """
-    logging.debug("Verify apk.static signature with " + sigkey_path)
+    logging.debug(f"Verify apk.static signature with {sigkey_path}")
     try:
         pmb.helpers.run.user(args, ["openssl", "dgst", "-sha1", "-verify",
                                     sigkey_path, "-signature", files[
                                         "sig"]["temp_path"],
                                     files["apk"]["temp_path"]])
     except BaseException:
         os.unlink(files["sig"]["temp_path"])
@@ -125,62 +110,63 @@
         files = extract_temp(tar, sigfilename)
 
     # Verify signature
     verify_signature(args, files, sigkey_path)
     os.unlink(files["sig"]["temp_path"])
     temp_path = files["apk"]["temp_path"]
 
-    # Verify the version, that the extracted binary reports
-    logging.debug("Verify the version reported by the apk.static binary" +
-                  " (must match the package version " + version + ")")
+    # Verify the version that the extracted binary reports
+    logging.debug("Verify the version reported by the apk.static binary"
+                  f" (must match the package version {version})")
     os.chmod(temp_path, os.stat(temp_path).st_mode | stat.S_IEXEC)
     version_bin = pmb.helpers.run.user(args, [temp_path, "--version"],
                                        output_return=True)
     version_bin = version_bin.split(" ")[1].split(",")[0]
-    if not version.startswith(version_bin + "-r"):
+    if not version.startswith(f"{version_bin}-r"):
         os.unlink(temp_path)
-        raise RuntimeError("Downloaded apk-tools-static-" + version + ".apk,"
-                           " but the apk binary inside that package reports to be"
-                           " version: " + version_bin + "! Looks like a downgrade attack"
-                           " from a malicious server! Switch the server (-m) and try again.")
+        raise RuntimeError(f"Downloaded apk-tools-static-{version}.apk,"
+                           " but the apk binary inside that package reports"
+                           f" to be version: {version_bin}!"
+                           " Looks like a downgrade attack"
+                           " from a malicious server! Switch the server (-m)"
+                           " and try again.")
 
     # Move it to the right path
-    target_path = args.work + "/apk.static"
+    target_path = f"{args.work}/apk.static"
     shutil.move(temp_path, target_path)
 
 
 def download(args, file):
     """
     Download a single file from an Alpine mirror.
     """
-    base_url = args.mirror_alpine + "edge/main/" + args.arch_native
-    return pmb.helpers.http.download(args, base_url + "/" + file, file)
+    channel_cfg = pmb.config.pmaports.read_config_channel(args)
+    mirrordir = channel_cfg["mirrordir_alpine"]
+    base_url = f"{args.mirror_alpine}{mirrordir}/main/{pmb.config.arch_native}"
+    return pmb.helpers.http.download(args, f"{base_url}/{file}", file)
 
 
 def init(args):
     """
     Download, verify, extract $WORK/apk.static.
     """
     # Get and parse the APKINDEX
     apkindex = pmb.helpers.repo.alpine_apkindex_path(args, "main")
     index_data = pmb.parse.apkindex.package(args, "apk-tools-static",
                                             indexes=[apkindex])
     version = index_data["version"]
 
-    # Extract and verify the apk-tools-static version
-    version_min = pmb.config.apk_tools_static_min_version
-    apk_name = "apk-tools-static-" + version + ".apk"
-    if pmb.parse.version.compare(version, version_min) == -1:
-        raise RuntimeError("Your APKINDEX has an outdated version of"
-                           " apk-tools-static (your version: " + version +
-                           ", expected at least:" + version_min + "). Please" +
-                           " run 'pmbootstrap update'.")
+    # Verify the apk-tools-static version
+    pmb.helpers.apk.check_outdated(
+        args, version, "Run 'pmbootstrap update', then try again.")
 
     # Download, extract, verify apk-tools-static
+    apk_name = f"apk-tools-static-{version}.apk"
     apk_static = download(args, apk_name)
     extract(args, version, apk_static)
 
 
 def run(args, parameters):
     if args.offline:
         parameters = ["--no-network"] + parameters
-    pmb.helpers.run.root(args, [args.work + "/apk.static"] + parameters)
+    pmb.helpers.apk.apk_with_progress(
+        args, [f"{args.work}/apk.static"] + parameters, chroot=False)
```

### Comparing `pmbootstrap-1.9.0/pmb/config/init.py` & `pmbootstrap-2.0.0/pmb/qemu/run.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,393 +1,382 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Pablo Castellano, Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
-import glob
 import os
-
+import re
+import signal
+import shlex
+import shutil
+
+import pmb.build
+import pmb.chroot
+import pmb.chroot.apk
+import pmb.chroot.other
+import pmb.chroot.initfs
 import pmb.config
 import pmb.config.pmaports
-import pmb.helpers.cli
-import pmb.helpers.devices
-import pmb.helpers.logging
 import pmb.helpers.run
-import pmb.helpers.ui
-import pmb.chroot.zap
-import pmb.parse.deviceinfo
-import pmb.parse._apkbuild
-
-
-def ask_for_work_path(args):
-    """
-    Ask for the work path, until we can create it (when it does not exist) and
-    write into it.
-    :returns: (path, exists)
-              * path: is the full path, with expanded ~ sign
-              * exists: is False when the folder did not exist before we tested
-                        whether we can create it
-    """
-    logging.info("Location of the 'work' path. Multiple chroots"
-                 " (native, device arch, device rootfs) will be created"
-                 " in there.")
-    while True:
-        try:
-            work = os.path.expanduser(pmb.helpers.cli.ask(
-                args, "Work path", None, args.work, False))
-            work = os.path.realpath(work)
-            exists = os.path.exists(work)
-
-            # Work must not be inside the pmbootstrap path
-            if (work == pmb.config.pmb_src or
-                    work.startswith(pmb.config.pmb_src + "/")):
-                logging.fatal("ERROR: The work path must not be inside the"
-                              " pmbootstrap path. Please specify another"
-                              " location.")
-                continue
-
-            # Create the folder with a version file
-            if not exists:
-                os.makedirs(work, 0o700, True)
-                with open(work + "/version", "w") as handle:
-                    handle.write(str(pmb.config.work_version) + "\n")
-
-            # Make sure, that we can write into it
-            os.makedirs(work + "/cache_http", 0o700, True)
-            return (work, exists)
-        except OSError:
-            logging.fatal("ERROR: Could not create this folder, or write"
-                          " inside it! Please try again.")
-
-
-def ask_for_ui(args):
-    ui_list = pmb.helpers.ui.list(args)
-    logging.info("Available user interfaces (" +
-                 str(len(ui_list) - 1) + "): ")
-    for ui in ui_list:
-        logging.info("* " + ui[0] + ": " + ui[1])
-    while True:
-        ret = pmb.helpers.cli.ask(args, "User interface", None, args.ui, True)
-        if ret in dict(ui_list).keys():
-            return ret
-        logging.fatal("ERROR: Invalid user interface specified, please type in"
-                      " one from the list above.")
-
-
-def ask_for_keymaps(args, device):
-    info = pmb.parse.deviceinfo(args, device)
-    if "keymaps" not in info or info["keymaps"].strip() == "":
-        return ""
-    options = info["keymaps"].split(' ')
-    logging.info("Available keymaps for device (" + str(len(options)) +
-                 "): " + ", ".join(options))
-    if args.keymap == "":
-        args.keymap = options[0]
-
-    while True:
-        ret = pmb.helpers.cli.ask(args, "Keymap", None, args.keymap, True)
-        if ret in options:
-            return ret
-        logging.fatal("ERROR: Invalid keymap specified, please type in"
-                      " one from the list above.")
-
-
-def ask_for_timezone(args):
-    localtimes = ["/etc/zoneinfo/localtime", "/etc/localtime"]
-    zoneinfo_path = "/usr/share/zoneinfo/"
-    for localtime in localtimes:
-        if not os.path.exists(localtime):
-            continue
-        tz = ""
-        if os.path.exists(localtime):
-            tzpath = os.path.realpath(localtime)
-            tzpath = tzpath.rstrip()
-            if os.path.exists(tzpath):
-                try:
-                    _, tz = tzpath.split(zoneinfo_path)
-                except:
-                    pass
-        if tz:
-            logging.info("Your host timezone: " + tz)
-            if pmb.helpers.cli.confirm(args, "Use this timezone instead of GMT?",
-                                       default="y"):
-                return tz
-    logging.info("WARNING: Unable to determine timezone configuration on host,"
-                 " using GMT.")
-    return "GMT"
-
-
-def ask_for_device_kernel(args, device):
-    """
-    Ask for the kernel that should be used with the device.
-
-    :param device: code name, e.g. "lg-mako"
-    :returns: None if the kernel is hardcoded in depends without subpackages
-    :returns: kernel type ("downstream", "stable", "mainline", ...)
-    """
-    # Get kernels
-    kernels = pmb.parse._apkbuild.kernels(args, device)
-    if not kernels:
-        return args.kernel
-
-    # Get default
-    default = args.kernel
-    if default not in kernels:
-        default = list(kernels.keys())[0]
-
-    # Ask for kernel (extra message when downstream and upstream are available)
-    logging.info("Which kernel do you want to use with your device?")
-    if "downstream" in kernels:
-        logging.info("Downstream kernels are typically the outdated Android"
-                     " kernel forks.")
-    if "downstream" in kernels and len(kernels) > 1:
-        logging.info("Upstream kernels (mainline, stable, ...) get security"
-                     " updates, but may have less working features than"
-                     " downstream kernels.")
-
-    # List kernels
-    logging.info("Available kernels (" + str(len(kernels)) + "):")
-    for type in sorted(kernels.keys()):
-        logging.info("* " + type + ": " + kernels[type])
-    while True:
-        ret = pmb.helpers.cli.ask(args, "Kernel", None, default, True)
-        if ret in kernels.keys():
-            return ret
-        logging.fatal("ERROR: Invalid kernel specified, please type in one"
-                      " from the list above.")
-    return ret
-
-
-def ask_for_device_nonfree(args, device):
-    """
-    Ask the user about enabling proprietary firmware (e.g. Wifi) and userland
-    (e.g. GPU drivers). All proprietary components are in subpackages
-    $pkgname-nonfree-firmware and $pkgname-nonfree-userland, and we show the
-    description of these subpackages (so they can indicate which peripherals
-    are affected).
-
-    :returns: answers as dict, e.g. {"firmware": True, "userland": False}
-    """
-    # Parse existing APKBUILD or return defaults (when called from test case)
-    apkbuild_path = args.aports + "/device/device-" + device + "/APKBUILD"
-    ret = {"firmware": args.nonfree_firmware,
-           "userland": args.nonfree_userland}
-    if not os.path.exists(apkbuild_path):
-        return ret
-    apkbuild = pmb.parse.apkbuild(args, apkbuild_path)
-
-    # Only run when there is a "nonfree" subpackage
-    nonfree_found = False
-    for subpackage in apkbuild["subpackages"]:
-        if subpackage.startswith("device-" + device + "-nonfree"):
-            nonfree_found = True
-    if not nonfree_found:
-        return ret
-
-    # Short explanation
-    logging.info("This device has proprietary components, which trade some of"
-                 " your freedom with making more peripherals work.")
-    logging.info("We would like to offer full functionality without hurting"
-                 " your freedom, but this is currently not possible for your"
-                 " device.")
-
-    # Ask for firmware and userland individually
-    for type in ["firmware", "userland"]:
-        subpkgname = "device-" + device + "-nonfree-" + type
-        if subpkgname in apkbuild["subpackages"]:
-            subpkgdesc = pmb.parse._apkbuild.subpkgdesc(apkbuild_path,
-                                                        "nonfree_" + type)
-            logging.info(subpkgname + ": " + subpkgdesc)
-            ret[type] = pmb.helpers.cli.confirm(args, "Enable this package?",
-                                                default=ret[type])
-    return ret
-
-
-def ask_for_device(args):
-    devices = sorted(pmb.helpers.devices.list_codenames(args))
-    logging.info("Target device (either an existing one, or a new one for"
-                 " porting).")
-    logging.info("Available (" + str(len(devices)) + "): " +
-                 ", ".join(devices))
-    while True:
-        device = pmb.helpers.cli.ask(args, "Device", None, args.device, False,
-                                     "[a-z0-9]+-[a-z0-9]+")
-        device_exists = os.path.exists(args.aports + "/device/device-" +
-                                       device + "/deviceinfo")
-        if not device_exists:
-            if device == args.device:
-                raise RuntimeError(
-                    "This device does not exist anymore, check"
-                    " <https://postmarketos.org/renamed>"
-                    " to see if it was renamed")
-            logging.info("You are about to do a new device port for '" +
-                         device + "'.")
-            if not pmb.helpers.cli.confirm(args, default=True):
-                continue
-
-            pmb.aportgen.generate(args, "device-" + device)
-            pmb.aportgen.generate(args, "linux-" + device)
-        break
-
-    kernel = ask_for_device_kernel(args, device)
-    nonfree = ask_for_device_nonfree(args, device)
-    return (device, device_exists, kernel, nonfree)
-
-
-def ask_for_qemu_native_mesa_driver(args, device, arch_native):
-    # Native QEMU device selected? (e.g. qemu-amd64 on x86_64)
-    if not pmb.parse.arch.qemu_check_device(device, arch_native):
-        return None
-
-    drivers = pmb.config.qemu_native_mesa_drivers
-    logging.info("Which mesa driver do you prefer for your native QEMU device?"
-                 " Only select something other than the default if you are"
-                 " having graphical problems (such as glitches).")
-    while True:
-        ret = pmb.helpers.cli.ask(args, "Mesa driver", drivers,
-                                  args.qemu_native_mesa_driver)
-        if ret in drivers:
-            return ret
-        logging.fatal("ERROR: Please specify a driver from the list. To change"
-                      " it, see qemu_native_mesa_drivers in"
-                      " pmb/config/__init__.py.")
-
-
-def ask_for_build_options(args, cfg):
-    # Allow to skip build options
-    logging.info("Build options: Parallel jobs: " + args.jobs +
-                 ", ccache per arch: " + args.ccache_size)
-
-    if not pmb.helpers.cli.confirm(args, "Change them?",
-                                   default=False):
-        return
-
-    # Parallel job count
-    logging.info("How many jobs should run parallel on this machine, when"
-                 " compiling?")
-    answer = pmb.helpers.cli.ask(args, "Jobs", None, args.jobs,
-                                 validation_regex="[1-9][0-9]*")
-    cfg["pmbootstrap"]["jobs"] = answer
-
-    # Ccache size
-    logging.info("We use ccache to speed up building the same code multiple"
-                 " times. How much space should the ccache folder take up per"
-                 " architecture? After init is through, you can check the current"
-                 " usage with 'pmbootstrap stats'. Answer with 0 for infinite.")
-    regex = "0|[0-9]+(k|M|G|T|Ki|Mi|Gi|Ti)"
-    answer = pmb.helpers.cli.ask(args, "Ccache size", None, args.ccache_size,
-                                 lowercase_answer=False, validation_regex=regex)
-    cfg["pmbootstrap"]["ccache_size"] = answer
-
-
-def ask_for_hostname(args, device):
-    while True:
-        ret = pmb.helpers.cli.ask(args, "Device hostname (short form, e.g. 'foo')",
-                                  None, (args.hostname or device), True)
-        if not pmb.helpers.other.validate_hostname(ret):
-            continue
-        # Don't store device name in user's config (gets replaced in install)
-        if ret == device:
-            return ""
-        return ret
-
-
-def ask_for_ssh_keys(args):
-    if not len(glob.glob(os.path.expanduser("~/.ssh/id_*.pub"))):
-        return False
-    return pmb.helpers.cli.confirm(args,
-                                   "Would you like to copy your SSH public keys to the device?",
-                                   default=args.ssh_keys)
-
-
-def frontend(args):
-    # Work folder (needs to be first, so we can create chroots early)
-    cfg = pmb.config.load(args)
-    work, work_exists = ask_for_work_path(args)
-    cfg["pmbootstrap"]["work"] = work
-
-    # Update args and save config (so chroots and 'pmbootstrap log' work)
-    pmb.helpers.args.update_work(args, work)
-    pmb.config.save(args, cfg)
-
-    # Clone pmaports
-    pmb.config.pmaports.init(args)
-
-    # Device
-    device, device_exists, kernel, nonfree = ask_for_device(args)
-    cfg["pmbootstrap"]["device"] = device
-    cfg["pmbootstrap"]["kernel"] = kernel
-    cfg["pmbootstrap"]["nonfree_firmware"] = str(nonfree["firmware"])
-    cfg["pmbootstrap"]["nonfree_userland"] = str(nonfree["userland"])
-
-    # QEMU mesa driver
-    if cfg["pmbootstrap"]["device"].startswith("qemu-"):
-        driver = ask_for_qemu_native_mesa_driver(args, device, args.arch_native)
-        if driver:
-            cfg["pmbootstrap"]["qemu_native_mesa_driver"] = driver
-
-    # Device keymap
-    if device_exists:
-        cfg["pmbootstrap"]["keymap"] = ask_for_keymaps(args, device)
-
-    # Username
-    cfg["pmbootstrap"]["user"] = pmb.helpers.cli.ask(args, "Username", None,
-                                                     args.user, False,
-                                                     "[a-z_][a-z0-9_-]*")
-    # UI and various build options
-    cfg["pmbootstrap"]["ui"] = ask_for_ui(args)
-    ask_for_build_options(args, cfg)
-
-    # Extra packages to be installed to rootfs
-    logging.info("Additional packages that will be installed to rootfs."
-                 " Specify them in a comma separated list (e.g.: vim,file)"
-                 " or \"none\"")
-    extra = pmb.helpers.cli.ask(args, "Extra packages", None,
-                                args.extra_packages,
-                                validation_regex=r"^([-.+\w]+)(,[-.+\w]+)*$")
-    cfg["pmbootstrap"]["extra_packages"] = extra
-
-    # Configure timezone info
-    cfg["pmbootstrap"]["timezone"] = ask_for_timezone(args)
-
-    # Hostname
-    cfg["pmbootstrap"]["hostname"] = ask_for_hostname(args, device)
-
-    # SSH keys
-    cfg["pmbootstrap"]["ssh_keys"] = str(ask_for_ssh_keys(args))
-
-    # pmaports path (if users change it with: 'pmbootstrap --aports=... init')
-    cfg["pmbootstrap"]["aports"] = args.aports
-
-    # Save config
-    pmb.config.save(args, cfg)
-
-    # Zap existing chroots
-    if (work_exists and device_exists and
-            len(glob.glob(args.work + "/chroot_*")) and
-            pmb.helpers.cli.confirm(args, "Zap existing chroots to apply configuration?", default=True)):
-        setattr(args, "deviceinfo", pmb.parse.deviceinfo(args, device=device))
-
-        # Do not zap any existing packages or cache_http directories
-        pmb.chroot.zap(args, confirm=False)
-
-    logging.info(
-        "WARNING: The applications in the chroots do not get updated automatically.")
-    logging.info("Run 'pmbootstrap zap' to delete all chroots once a day before"
-                 " working with pmbootstrap!")
-    logging.info("It only takes a few seconds, and all packages are cached.")
+import pmb.parse.arch
+import pmb.parse.cpuinfo
+
+
+def system_image(args):
+    """
+    Returns path to rootfs for specified device. In case that it doesn't
+    exist, raise and exception explaining how to generate it.
+    """
+    path = f"{args.work}/chroot_native/home/pmos/rootfs/{args.device}.img"
+    if not os.path.exists(path):
+        logging.debug("Could not find rootfs: " + path)
+        raise RuntimeError("The rootfs has not been generated yet, please "
+                           "run 'pmbootstrap install' first.")
+    return path
+
+
+def create_second_storage(args):
+    """
+    Generate a second storage image if it does not exist.
+    :returns: path to the image or None
+    """
+    path = f"{args.work}/chroot_native/home/pmos/rootfs/{args.device}-2nd.img"
+    pmb.helpers.run.root(args, ["touch", path])
+    pmb.helpers.run.root(args, ["chmod", "a+w", path])
+    resize_image(args, args.second_storage, path)
+    return path
+
+
+def which_qemu(arch):
+    """
+    Finds the qemu executable or raises an exception otherwise
+    """
+    executable = "qemu-system-" + arch
+    if shutil.which(executable):
+        return executable
+    else:
+        raise RuntimeError("Could not find the '" + executable + "' executable"
+                           " in your PATH. Please install it in order to"
+                           " run qemu.")
+
+
+def create_gdk_loader_cache(args):
+    """
+    Create a gdk loader cache that can be used for running GTK UIs outside of
+    the chroot.
+    """
+    gdk_cache_dir = "/usr/lib/gdk-pixbuf-2.0/2.10.0/"
+    custom_cache_path = gdk_cache_dir + "loaders-pmos-chroot.cache"
+    rootfs_native = args.work + "/chroot_native"
+    if os.path.isfile(rootfs_native + custom_cache_path):
+        return rootfs_native + custom_cache_path
+
+    cache_path = gdk_cache_dir + "loaders.cache"
+    if not os.path.isfile(rootfs_native + cache_path):
+        raise RuntimeError("gdk pixbuf cache file not found: " + cache_path)
+
+    pmb.chroot.root(args, ["cp", cache_path, custom_cache_path])
+    cmd = ["sed", "-i", "-e",
+           f"s@\"{gdk_cache_dir}@\"{rootfs_native}{gdk_cache_dir}@",
+           custom_cache_path]
+    pmb.chroot.root(args, cmd)
+    return rootfs_native + custom_cache_path
+
 
-    logging.info("Done!")
+def command_qemu(args, arch, img_path, img_path_2nd=None):
+    """
+    Generate the full qemu command with arguments to run postmarketOS
+    """
+    cmdline = args.deviceinfo["kernel_cmdline"]
+    if args.cmdline:
+        cmdline = args.cmdline
+
+    if "video=" not in cmdline:
+        cmdline += " video=" + args.qemu_video
+
+    logging.debug("Kernel cmdline: " + cmdline)
+
+    port_ssh = str(args.port)
+
+    suffix = "rootfs_" + args.device
+    rootfs = args.work + "/chroot_" + suffix
+    flavor = pmb.chroot.other.kernel_flavor_installed(args, suffix)
+    flavor_suffix = f"-{flavor}"
+    # Backwards compatibility with old mkinitfs (pma#660)
+    pmaports_cfg = pmb.config.pmaports.read_config(args)
+    if pmaports_cfg.get("supported_mkinitfs_without_flavors", False):
+        flavor_suffix = ""
+
+    # Alpine kernels always have the flavor appended to /boot/vmlinuz
+    kernel = f"{rootfs}/boot/vmlinuz{flavor_suffix}"
+    if not os.path.exists(kernel):
+        kernel = f"{kernel}-{flavor}"
+        if not os.path.exists(kernel):
+            raise RuntimeError("failed to find the proper vmlinuz path")
+
+    ncpus = os.cpu_count()
+
+    # QEMU mach-virt's max CPU count is 8, limit it so it will work correctly
+    # on systems with more than 8 CPUs
+    if arch != pmb.config.arch_native and ncpus > 8:
+        ncpus = 8
+
+    if args.host_qemu:
+        qemu_bin = which_qemu(arch)
+        env = {}
+        command = [qemu_bin]
+    else:
+        rootfs_native = args.work + "/chroot_native"
+        env = {"QEMU_MODULE_DIR": f"{rootfs_native}/usr/lib/qemu",
+               "GBM_DRIVERS_PATH": f"{rootfs_native}/usr/lib/xorg/modules/dri",
+               "LIBGL_DRIVERS_PATH": f"{rootfs_native}"
+                                     "/usr/lib/xorg/modules/dri"}
+
+        if "gtk" in args.qemu_display:
+            gdk_cache = create_gdk_loader_cache(args)
+            env.update({"GTK_THEME": "Default",
+                        "GDK_PIXBUF_MODULE_FILE": gdk_cache,
+                        "XDG_DATA_DIRS": rootfs_native + "/usr/local/share:" +
+                        rootfs_native + "/usr/share"})
+
+        command = []
+        if pmb.config.arch_native in ["aarch64", "armv7"]:
+            # Workaround for QEMU failing on aarch64 asymmetric multiprocessor
+            # arch (big/little architecture
+            # https://en.wikipedia.org/wiki/ARM_big.LITTLE) see
+            # https://bugs.linaro.org/show_bug.cgi?id=1443
+            ncpus_bl = pmb.parse.cpuinfo.arm_big_little_first_group_ncpus()
+            if ncpus_bl:
+                ncpus = ncpus_bl
+                logging.info("QEMU will run on big/little architecture on the"
+                             f" first {ncpus} cores (from /proc/cpuinfo)")
+                command += [rootfs_native + "/lib/ld-musl-" +
+                            pmb.config.arch_native + ".so.1"]
+                command += [rootfs_native + "/usr/bin/taskset"]
+                command += ["-c", "0-" + str(ncpus - 1)]
+
+        command += [rootfs_native + "/lib/ld-musl-" +
+                    pmb.config.arch_native + ".so.1"]
+        command += ["--library-path=" + rootfs_native + "/lib:" +
+                    rootfs_native + "/usr/lib:" +
+                    rootfs_native + "/usr/lib/pulseaudio"]
+        command += [rootfs_native + "/usr/bin/qemu-system-" + arch]
+        command += ["-L", rootfs_native + "/usr/share/qemu/"]
+
+    command += ["-nodefaults"]
+    # Only boot a kernel/initramfs directly when not doing EFI boot. This
+    # allows us to load/execute an EFI application on boot, and support
+    # a wide variety of boot loaders.
+    if not args.efi:
+        command += ["-kernel", kernel]
+        command += ["-initrd", rootfs + "/boot/initramfs" + flavor_suffix]
+        command += ["-append", shlex.quote(cmdline)]
+
+    command += ["-smp", str(ncpus)]
+
+    command += ["-m", str(args.memory)]
+
+    command += ["-serial"]
+    if args.qemu_redir_stdio:
+        command += ["mon:stdio"]
+    else:
+        command += ["stdio"]
+
+    command += ["-drive", "file=" + img_path + ",format=raw,if=virtio"]
+    if img_path_2nd:
+        command += ["-drive", "file=" + img_path_2nd + ",format=raw,if=virtio"]
+
+    if args.qemu_tablet:
+        command += ["-device", "virtio-tablet-pci"]
+    else:
+        command += ["-device", "virtio-mouse-pci"]
+    command += ["-device", "virtio-keyboard-pci"]
+    command += ["-netdev", f"user,id=net,hostfwd=tcp:127.0.0.1:{port_ssh}-:22"]
+    command += ["-device", "virtio-net-pci,netdev=net"]
+
+    if arch == "x86_64":
+        command += ["-device", "virtio-vga-gl"]
+    elif arch == "aarch64":
+        command += ["-M", "virt"]
+        command += ["-cpu", "cortex-a57"]
+        command += ["-device", "virtio-gpu-pci"]
+    elif arch == "riscv64":
+        command += ["-M", "virt"]
+        command += ["-device", "virtio-gpu-pci"]
+    else:
+        raise RuntimeError(f"Architecture {arch} not supported by this command"
+                           " yet.")
+
+    if args.efi:
+        command += ["-drive",
+                    "if=pflash,format=raw,readonly=on,file=/usr/share/OVMF/OVMF.fd"]
+
+    # Kernel Virtual Machine (KVM) support
+    native = pmb.config.arch_native == args.deviceinfo["arch"]
+    if args.qemu_kvm and native and os.path.exists("/dev/kvm"):
+        command += ["-enable-kvm"]
+        command += ["-cpu", "host"]
+    else:
+        logging.info("WARNING: QEMU is not using KVM and will run slower!")
+
+    if args.qemu_cpu:
+        command += ["-cpu", args.qemu_cpu]
+
+    display = args.qemu_display
+    if display != "none":
+        display += ",gl=" + ("on" if args.qemu_gl else "off")
+
+    # Separate -show-cursor option is deprecated. If your host qemu fails here,
+    # it's old (#1995).
+    command += ["-display", f"{display},show-cursor=on"]
+
+    # Audio support
+    if args.qemu_audio:
+        command += ["-audio", f"{args.qemu_audio},model=hda"]
+
+    return (command, env)
+
+
+def resize_image(args, img_size_new, img_path):
+    """
+    Truncates an image to a specific size. The value must be larger than the
+    current image size, and it must be specified in MiB or GiB units (powers of
+    1024).
+
+    :param img_size_new: new image size in M or G
+    :param img_path: the path to the image
+    """
+    # Current image size in bytes
+    img_size = os.path.getsize(img_path)
+
+    # Make sure we have at least 1 integer followed by either M or G
+    pattern = re.compile("^[0-9]+[M|G]$")
+    if not pattern.match(img_size_new):
+        raise RuntimeError("IMAGE_SIZE must be in [M]iB or [G]iB, e.g. 2048M"
+                           " or 2G")
+
+    # Remove M or G and convert to bytes
+    img_size_new_bytes = int(img_size_new[:-1]) * 1024 * 1024
+
+    # Convert further for G
+    if (img_size_new[-1] == "G"):
+        img_size_new_bytes = img_size_new_bytes * 1024
+
+    if (img_size_new_bytes >= img_size):
+        logging.info(f"Resize image to {img_size_new}: {img_path}")
+        pmb.helpers.run.root(args, ["truncate", "-s", img_size_new, img_path])
+    else:
+        # Convert to human-readable format
+        # NOTE: We convert to M here, and not G, so that we don't have to
+        # display a size like 1.25G, since decimal places are not allowed by
+        # truncate.
+        # We don't want users thinking they can use decimal numbers, and so in
+        # this example, they would need to use a size greater then 1280M
+        # instead.
+        img_size_str = str(round(img_size / 1024 / 1024)) + "M"
+
+        raise RuntimeError(f"IMAGE_SIZE must be {img_size_str} or greater")
+
+
+def sigterm_handler(number, frame):
+    raise RuntimeError("pmbootstrap was terminated by another process,"
+                       " and killed the QEMU VM it was running.")
+
+
+def install_depends(args, arch):
+    """
+    Install any necessary qemu dependencies in native chroot
+    """
+    depends = [
+        "mesa-dri-gallium",
+        "mesa-egl",
+        "mesa-gl",
+        "qemu",
+        "qemu-audio-alsa",
+        "qemu-audio-pa",
+        "qemu-audio-sdl",
+        "qemu-hw-display-virtio-gpu",
+        "qemu-hw-display-virtio-gpu-gl",
+        "qemu-hw-display-virtio-gpu-pci",
+        "qemu-hw-display-virtio-vga",
+        "qemu-hw-display-virtio-vga-gl",
+        "qemu-system-" + arch,
+        "qemu-ui-gtk",
+        "qemu-ui-opengl",
+        "qemu-ui-sdl",
+    ]
+
+    # QEMU packaging isn't split up as much in 3.12
+    channel_cfg = pmb.config.pmaports.read_config_channel(args)
+    if channel_cfg["branch_aports"] == "3.12-stable":
+        depends.remove("qemu-hw-display-virtio-gpu")
+        depends.remove("qemu-hw-display-virtio-gpu-pci")
+        depends.remove("qemu-hw-display-virtio-vga")
+        depends.remove("qemu-ui-opengl")
+
+    if args.efi:
+        depends.append("ovmf")
+
+    pmb.chroot.apk.install(args, depends)
+
+
+def run(args):
+    """
+    Run a postmarketOS image in qemu
+    """
+    if not args.device.startswith("qemu-"):
+        raise RuntimeError("'pmbootstrap qemu' can be only used with one of "
+                           "the QEMU device packages. Run 'pmbootstrap init' "
+                           "and select the 'qemu' vendor.")
+    arch = pmb.parse.arch.alpine_to_qemu(args.deviceinfo["arch"])
+
+    img_path = system_image(args)
+    img_path_2nd = None
+    if args.second_storage:
+        img_path_2nd = create_second_storage(args)
+
+    if not args.host_qemu:
+        install_depends(args, arch)
+    logging.info("Running postmarketOS in QEMU VM (" + arch + ")")
+
+    qemu, env = command_qemu(args, arch, img_path, img_path_2nd)
+
+    # Workaround: QEMU runs as local user and needs write permissions in the
+    # rootfs, which is owned by root
+    if not os.access(img_path, os.W_OK):
+        pmb.helpers.run.root(args, ["chmod", "666", img_path])
+
+    # Resize the rootfs (or show hint)
+    if args.image_size:
+        resize_image(args, args.image_size, img_path)
+    else:
+        logging.info("NOTE: Run 'pmbootstrap qemu --image-size 2G' to set"
+                     " the rootfs size when you run out of space!")
+
+    # SSH/serial/network hints
+    logging.info("Connect to the VM:")
+    logging.info("* (ssh) ssh -p {port} {user}@localhost".format(**vars(args)))
+    logging.info("* (serial) in this console (stdout/stdin)")
+
+    if args.qemu_redir_stdio:
+        logging.info("NOTE: Ctrl+C is redirected to the VM! To disable this, "
+                     "run: pmbootstrap config qemu_redir_stdio False")
+        logging.info("NOTE: To quit QEMU with this option you can use "
+                     "Ctrl-A, X.")
+
+    if args.ui == "none":
+        logging.warning("WARNING: With UI=none network doesn't work"
+                        " automatically: https://postmarketos.org/qemu-network")
+
+    # Run QEMU and kill it together with pmbootstrap
+    process = None
+    try:
+        signal.signal(signal.SIGTERM, sigterm_handler)
+        process = pmb.helpers.run.user(args, qemu, output="tui", env=env)
+    except KeyboardInterrupt:
+        # In addition to not showing a trace when pressing ^C, let user know
+        # they can override this behavior:
+        logging.info("Quitting because Ctrl+C detected.")
+        logging.info("To override this behavior and have pmbootstrap "
+                     "send Ctrl+C to the VM, run:")
+        logging.info("$ pmbootstrap config qemu_redir_stdio True")
+    finally:
+        if process:
+            process.terminate()
```

### Comparing `pmbootstrap-1.9.0/pmb/data/qemu-user-binfmt.txt` & `pmbootstrap-2.0.0/pmb/data/qemu-user-binfmt.txt`

 * *Files identical despite different names*

### Comparing `pmbootstrap-1.9.0/pmb/export/symlinks.py` & `pmbootstrap-2.0.0/pmb/export/symlinks.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,65 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 import os
 import glob
 
 import pmb.build
 import pmb.chroot.apk
 import pmb.config
+import pmb.config.pmaports
 import pmb.flasher
 import pmb.helpers.file
 
 
 def symlinks(args, flavor, folder):
     """
     Create convenience symlinks to the rootfs and boot files.
     """
 
+    # Backwards compatibility with old mkinitfs (pma#660)
+    suffix = f"-{flavor}"
+    pmaports_cfg = pmb.config.pmaports.read_config(args)
+    if pmaports_cfg.get("supported_mkinitfs_without_flavors", False):
+        suffix = ""
+
     # File descriptions
     info = {
-        "boot.img-" + flavor: "Fastboot compatible boot.img file,"
-        " contains initramfs and kernel",
-        "blob-" + flavor: "Asus boot blob for TF101",
-        "initramfs-" + flavor: "Initramfs",
-        "initramfs-" + flavor + "-extra": "Extra initramfs files in /boot",
-        "uInitrd-" + flavor: "Initramfs, legacy u-boot image format",
-        "uImage-" + flavor: "Kernel, legacy u-boot image format",
-        "vmlinuz-" + flavor: "Linux kernel",
-        args.device + ".img": "Rootfs with partitions for /boot and /",
-        args.device + "-boot.img": "Boot partition image",
-        args.device + "-root.img": "Root partition image",
-        "pmos-" + args.device + ".zip": "Android recovery flashable zip",
+        f"boot.img{suffix}": ("Fastboot compatible boot.img file,"
+                              " contains initramfs and kernel"),
+        "dtbo.img": "Fastboot compatible dtbo image",
+        f"initramfs{suffix}": "Initramfs",
+        f"initramfs{suffix}-extra": "Extra initramfs files in /boot",
+        f"uInitrd{suffix}": "Initramfs, legacy u-boot image format",
+        f"uImage{suffix}": "Kernel, legacy u-boot image format",
+        f"vmlinuz{suffix}": "Linux kernel",
+        f"{args.device}.img": "Rootfs with partitions for /boot and /",
+        f"{args.device}-boot.img": "Boot partition image",
+        f"{args.device}-root.img": "Root partition image",
+        f"pmos-{args.device}.zip": "Android recovery flashable zip",
+        "lk2nd.img": "Secondary Android bootloader",
     }
 
     # Generate a list of patterns
     path_native = args.work + "/chroot_native"
     path_boot = args.work + "/chroot_rootfs_" + args.device + "/boot"
     path_buildroot = args.work + "/chroot_buildroot_" + args.deviceinfo["arch"]
-    patterns = [path_boot + "/*-" + flavor,
-                path_boot + "/*-" + flavor + "-extra",
-                path_native + "/home/pmos/rootfs/" + args.device + ".img",
-                path_native + "/home/pmos/rootfs/" + args.device + "-boot.img",
-                path_native + "/home/pmos/rootfs/" + args.device + "-root.img",
-                path_buildroot +
-                "/var/lib/postmarketos-android-recovery-installer/pmos-" +
-                args.device + ".zip"]
+    patterns = [f"{path_boot}/boot.img{suffix}",
+                f"{path_boot}/initramfs{suffix}*",
+                f"{path_boot}/uInitrd{suffix}",
+                f"{path_boot}/uImage{suffix}",
+                f"{path_boot}/vmlinuz{suffix}",
+                f"{path_boot}/dtbo.img",
+                f"{path_native}/home/pmos/rootfs/{args.device}.img",
+                f"{path_native}/home/pmos/rootfs/{args.device}-boot.img",
+                f"{path_native}/home/pmos/rootfs/{args.device}-root.img",
+                f"{path_buildroot}/var/lib/postmarketos-android-recovery-" +
+                f"installer/pmos-{args.device}.zip",
+                f"{path_boot}/lk2nd.img"]
 
     # Generate a list of files from the patterns
     files = []
     for pattern in patterns:
         files += glob.glob(pattern)
 
     # Iterate through all files
```

### Comparing `pmbootstrap-1.9.0/pmb/export/odin.py` & `pmbootstrap-2.0.0/pmb/export/odin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,108 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 import os
 
 import pmb.build
 import pmb.chroot.apk
 import pmb.config
 import pmb.flasher
 import pmb.helpers.file
 
 
 def odin(args, flavor, folder):
     """
-    Create Odin flashable tar file with kernel and initramfs for devices configured with
-    the flasher method 'heimdall-isorec' and with boot.img for devices with 'heimdall-bootimg'
+    Create Odin flashable tar file with kernel and initramfs
+    for devices configured with the flasher method 'heimdall-isorec'
+    and with boot.img for devices with 'heimdall-bootimg'
     """
     pmb.flasher.init(args)
     suffix = "rootfs_" + args.device
 
+    # Backwards compatibility with old mkinitfs (pma#660)
+    suffix_flavor = f"-{flavor}"
+    pmaports_cfg = pmb.config.pmaports.read_config(args)
+    if pmaports_cfg.get("supported_mkinitfs_without_flavors", False):
+        suffix_flavor = ""
+
     # Validate method
     method = args.deviceinfo["flash_method"]
     if not method.startswith("heimdall-"):
-        raise RuntimeError("An odin flashable tar is not supported for the flash"
-                           " method '" + method + "' specified in the current configuration."
+        raise RuntimeError("An odin flashable tar is not supported"
+                           f" for the flash method '{method}' specified"
+                           " in the current configuration."
                            " Only 'heimdall' methods are supported.")
 
     # Partitions
-    partition_kernel = args.deviceinfo["flash_heimdall_partition_kernel"] or "KERNEL"
-    partition_initfs = args.deviceinfo["flash_heimdall_partition_initfs"] or "RECOVERY"
+    partition_kernel = \
+        args.deviceinfo["flash_heimdall_partition_kernel"] or "KERNEL"
+    partition_initfs = \
+        args.deviceinfo["flash_heimdall_partition_initfs"] or "RECOVERY"
 
     # Temporary folder
     temp_folder = "/tmp/odin-flashable-tar"
-    if os.path.exists(args.work + "/chroot_native" + temp_folder):
+    if os.path.exists(f"{args.work}/chroot_native{temp_folder}"):
         pmb.chroot.root(args, ["rm", "-rf", temp_folder])
 
-    # Odin flashable tar generation script (because redirecting stdin/stdout is not allowed
+    # Odin flashable tar generation script
+    # (because redirecting stdin/stdout is not allowed
     # in pmbootstrap's chroot/shell functions for security reasons)
-    with open(args.work + "/chroot_rootfs_" + args.device + "/tmp/_odin.sh", "w") as handle:
-        odin_kernel_md5 = partition_kernel + ".bin.md5"
-        odin_initfs_md5 = partition_initfs + ".bin.md5"
-        odin_device_tar = args.device + ".tar"
-        odin_device_tar_md5 = args.device + ".tar.md5"
+    odin_script = f"{args.work}/chroot_rootfs_{args.device}/tmp/_odin.sh"
+    with open(odin_script, "w") as handle:
+        odin_kernel_md5 = f"{partition_kernel}.bin.md5"
+        odin_initfs_md5 = f"{partition_initfs}.bin.md5"
+        odin_device_tar = f"{args.device}.tar"
+        odin_device_tar_md5 = f"{args.device}.tar.md5"
 
         handle.write(
             "#!/bin/sh\n"
-            "cd " + temp_folder + "\n")
+            f"cd {temp_folder}\n")
         if method == "heimdall-isorec":
             handle.write(
                 # Kernel: copy and append md5
-                "cp /boot/vmlinuz-" + flavor + " " + odin_kernel_md5 + "\n"
-                "md5sum -t " + odin_kernel_md5 + " >> " + odin_kernel_md5 + "\n"
+                f"cp /boot/vmlinuz{suffix_flavor} {odin_kernel_md5}\n"
+                f"md5sum -t {odin_kernel_md5} >> {odin_kernel_md5}\n"
                 # Initramfs: recompress with lzop, append md5
-                "gunzip -c /boot/initramfs-" + flavor + " | lzop > " + odin_initfs_md5 + "\n"
-                "md5sum -t " + odin_initfs_md5 + " >> " + odin_initfs_md5 + "\n")
+                f"gunzip -c /boot/initramfs{suffix_flavor}"
+                f" | lzop > {odin_initfs_md5}\n"
+                f"md5sum -t {odin_initfs_md5} >> {odin_initfs_md5}\n")
         elif method == "heimdall-bootimg":
             handle.write(
                 # boot.img: copy and append md5
-                "cp /boot/boot.img-" + flavor + " " + odin_kernel_md5 + "\n"
-                "md5sum -t " + odin_kernel_md5 + " >> " + odin_kernel_md5 + "\n")
+                f"cp /boot/boot.img{suffix_flavor} {odin_kernel_md5}\n"
+                f"md5sum -t {odin_kernel_md5} >> {odin_kernel_md5}\n")
         handle.write(
             # Create tar, remove included files and append md5
-            "tar -c -f " + odin_device_tar + " *.bin.md5\n"
+            f"tar -c -f {odin_device_tar} *.bin.md5\n"
             "rm *.bin.md5\n"
-            "md5sum -t " + odin_device_tar + " >> " + odin_device_tar + "\n"
-            "mv " + odin_device_tar + " " + odin_device_tar_md5 + "\n")
+            f"md5sum -t {odin_device_tar} >> {odin_device_tar}\n"
+            f"mv {odin_device_tar} {odin_device_tar_md5}\n")
 
     commands = [["mkdir", "-p", temp_folder],
                 ["cat", "/tmp/_odin.sh"],  # for the log
                 ["sh", "/tmp/_odin.sh"],
                 ["rm", "/tmp/_odin.sh"]
                 ]
     for command in commands:
         pmb.chroot.root(args, command, suffix)
 
     # Move Odin flashable tar to native chroot and cleanup temp folder
     pmb.chroot.user(args, ["mkdir", "-p", "/home/pmos/rootfs"])
-    pmb.chroot.root(args, ["mv", "/mnt/rootfs_" + args.device + temp_folder +
-                           "/" + odin_device_tar_md5, "/home/pmos/rootfs/"]),
+    pmb.chroot.root(args, ["mv", f"/mnt/rootfs_{args.device}{temp_folder}"
+                           f"/{odin_device_tar_md5}", "/home/pmos/rootfs/"]),
     pmb.chroot.root(args, ["chown", "pmos:pmos",
-                           "/home/pmos/rootfs/" + odin_device_tar_md5])
+                           f"/home/pmos/rootfs/{odin_device_tar_md5}"])
     pmb.chroot.root(args, ["rmdir", temp_folder], suffix)
 
     # Create the symlink
-    file = args.work + "/chroot_native/home/pmos/rootfs/" + odin_device_tar_md5
-    link = folder + "/" + odin_device_tar_md5
+    file = f"{args.work}/chroot_native/home/pmos/rootfs/{odin_device_tar_md5}"
+    link = f"{folder}/{odin_device_tar_md5}"
     pmb.helpers.file.symlink(args, file, link)
 
     # Display a readable message
-    msg = " * " + odin_device_tar_md5
+    msg = f" * {odin_device_tar_md5}"
     if method == "heimdall-isorec":
         msg += " (Odin flashable file, contains initramfs and kernel)"
     elif method == "heimdall-bootimg":
         msg += " (Odin flashable file, contains boot.img)"
     logging.info(msg)
```

### Comparing `pmbootstrap-1.9.0/pmb/export/frontend.py` & `pmbootstrap-2.0.0/pmb/export/frontend.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     chroot = args.work + "/chroot_native"
     pattern = chroot + "/home/pmos/rootfs/" + args.device + "*.img"
     if not glob.glob(pattern):
         logging.info("NOTE: To export the rootfs image, run 'pmbootstrap"
                      " install' first (without the 'sdcard' parameter).")
 
     # Rebuild the initramfs, just to make sure (see #69)
-    flavor = pmb.helpers.frontend._parse_flavor(args)
-    pmb.chroot.initfs.build(args, flavor, "rootfs_" + args.device)
+    flavor = pmb.helpers.frontend._parse_flavor(args, args.autoinstall)
+    if args.autoinstall:
+        pmb.chroot.initfs.build(args, flavor, "rootfs_" + args.device)
 
     # Do the export, print all files
     logging.info("Export symlinks to: " + target)
     if args.odin_flashable_tar:
         pmb.export.odin(args, flavor, target)
     pmb.export.symlinks(args, flavor, target)
```

### Comparing `pmbootstrap-1.9.0/pmb/parse/version.py` & `pmbootstrap-2.0.0/pmb/parse/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import collections
 
 """
 In order to stay as compatible to Alpine's apk as possible, this code
 is heavily based on:
 
 https://git.alpinelinux.org/cgit/apk-tools/tree/src/version.c
@@ -53,15 +37,15 @@
 
 def next_token(previous, rest):
     """
     Parse the next token in the rest of the version string, we're
     currently looking at.
 
     We do *not* get the value of the token, or advance the rest string
-    beyond the whole token, that is what the get_token() function does
+    beyond the whole token that is what the get_token() function does
     (see below).
 
     :param previous: the token before
     :param rest: of the version string
     :returns: (next, rest) next is the upcoming token, rest is the
               input "rest" string with one leading '.', '_' or '-'
               character removed (if there was any).
@@ -107,15 +91,15 @@
 def parse_suffix(rest):
     """
     Cut off the suffix of rest (which is now at the beginning of the
     rest variable, but regarding the whole version string, it is a
     suffix), and return a value integer (so it can be compared later,
     "beta" > "alpha" etc).
 
-    :param rest: what is left of the version string, that we are
+    :param rest: what is left of the version string that we are
                  currently parsing, starts with a "suffix" value
                  (see below for valid suffixes).
     :returns: (rest, value, invalid_suffix)
               - rest: is the input "rest" string without the suffix
               - value: is a signed integer (negative for pre-,
                 positive for post-suffixes).
               - invalid_suffix: is true, when rest does not start
@@ -189,15 +173,15 @@
         (rest, value, invalid_suffix) = parse_suffix(rest)
 
     # Invalid previous token
     else:
         value = -1
 
     # Get the next token (for non-leading zeros)
-    if(not len(rest)):
+    if not len(rest):
         next = "end"
     elif next == "invalid" and not invalid_suffix:
         (next, rest) = next_token(previous, rest)
 
     return (next, value, rest)
```

### Comparing `pmbootstrap-1.9.0/pmb/parse/arch.py` & `pmbootstrap-2.0.0/pmb/parse/arch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,56 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import platform
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import fnmatch
+import platform
+import pmb.parse.arch
 
 
 def alpine_native():
     machine = platform.machine()
-    ret = ""
 
     mapping = {
         "i686": "x86",
         "x86_64": "x86_64",
         "aarch64": "aarch64",
+        "arm64": "aarch64",
         "armv6l": "armhf",
-        "armv7l": "armv7"
+        "armv7l": "armv7",
     }
     if machine in mapping:
         return mapping[machine]
     raise ValueError("Can not map platform.machine '" + machine + "'"
                      " to the right Alpine Linux architecture")
-    return ret
 
 
 def from_chroot_suffix(args, suffix):
     if suffix == "native":
-        return args.arch_native
-    if suffix == "rootfs_" + args.device:
+        return pmb.config.arch_native
+    if suffix in [f"rootfs_{args.device}", f"installer_{args.device}"]:
         return args.deviceinfo["arch"]
     if suffix.startswith("buildroot_"):
         return suffix.split("_", 1)[1]
 
     raise ValueError("Invalid chroot suffix: " + suffix +
                      " (wrong device chosen in 'init' step?)")
 
 
 def alpine_to_qemu(arch):
     """
     Convert the architecture to the string used in the QEMU packaging.
+    This corresponds to the package name of e.g. qemu-system-aarch64.
     """
 
     mapping = {
         "x86": "i386",
         "x86_64": "x86_64",
         "armhf": "arm",
         "armv7": "arm",
         "aarch64": "aarch64",
+        "riscv64": "riscv64",
     }
     for pattern, arch_qemu in mapping.items():
         if fnmatch.fnmatch(arch, pattern):
             return arch_qemu
     raise ValueError("Can not map Alpine architecture '" + arch + "'"
                      " to the right Debian architecture.")
 
@@ -74,15 +60,16 @@
     Convert the architecture to the string used inside the kernel sources.
     You can read the mapping from the linux-vanilla APKBUILD for example.
     """
     mapping = {
         "aarch64*": "arm64",
         "arm*": "arm",
         "ppc*": "powerpc",
-        "s390*": "s390"
+        "s390*": "s390",
+        "riscv64*": "riscv",
     }
     for pattern, arch_kernel in mapping.items():
         if fnmatch.fnmatch(arch, pattern):
             return arch_kernel
     return arch
 
 
@@ -91,93 +78,47 @@
     See: abuild source code/functions.sh.in: arch_to_hostspec()
     """
     mapping = {
         "aarch64": "aarch64-alpine-linux-musl",
         "armel": "armv5-alpine-linux-musleabi",
         "armhf": "armv6-alpine-linux-musleabihf",
         "armv7": "armv7-alpine-linux-musleabihf",
+        "loongarch32": "loongarch32-alpine-linux-musl",
+        "loongarchx32": "loongarchx32-alpine-linux-musl",
+        "loongarch64": "loongarch64-alpine-linux-musl",
         "mips": "mips-alpine-linux-musl",
         "mips64": "mips64-alpine-linux-musl",
         "mipsel": "mipsel-alpine-linux-musl",
         "mips64el": "mips64el-alpine-linux-musl",
         "ppc": "powerpc-alpine-linux-musl",
         "ppc64": "powerpc64-alpine-linux-musl",
         "ppc64le": "powerpc64le-alpine-linux-musl",
+        "riscv32": "riscv32-alpine-linux-musl",
+        "riscv64": "riscv64-alpine-linux-musl",
         "s390x": "s390x-alpine-linux-musl",
         "x86": "i586-alpine-linux-musl",
         "x86_64": "x86_64-alpine-linux-musl",
     }
     if arch in mapping:
         return mapping[arch]
 
     raise ValueError("Can not map Alpine architecture '" + arch + "'"
                      " to the right hostspec value")
 
 
-def cpu_emulation_required(args, arch):
+def cpu_emulation_required(arch):
     # Obvious case: host arch is target arch
-    if args.arch_native == arch:
+    if pmb.config.arch_native == arch:
         return False
 
     # Other cases: host arch on the left, target archs on the right
     not_required = {
         "x86_64": ["x86"],
+        "armv7": ["armel", "armhf"],
         "aarch64": ["armel", "armhf", "armv7"],
     }
-    if args.arch_native in not_required:
-        if arch in not_required[args.arch_native]:
+    if pmb.config.arch_native in not_required:
+        if arch in not_required[pmb.config.arch_native]:
             return False
 
     # No match: then it's required
     return True
-
-
-def uname_to_qemu(arch):
-    """
-    Convert the most common architectures returned by 'uname' to those
-    used by the QEMU binary
-    """
-    mapping = {
-        "aarch64": "aarch64",
-        "arm": "arm",
-        "armeb": "arm",
-        "armel": "arm",
-        "armhf": "arm",
-        "armv7l": "arm",
-        "x86_64": "x86_64",
-        "amd64": "x86_64",
-    }
-    if arch in mapping:
-        return mapping[arch]
-
-    raise ValueError("Can not map host architecture '" + arch + "'"
-                     " to the right QEMU value")
-
-
-def qemu_to_pmos_device(arch):
-    """
-    Convert the architecture used in the QEMU binary to the aport name in
-    postmarketOS defining the device
-    """
-    mapping = {
-        "arm": "qemu-vexpress",
-        "aarch64": "qemu-aarch64",
-        "x86_64": "qemu-amd64",
-    }
-    if arch in mapping:
-        return mapping[arch]
-
-    raise ValueError("Can not map QEMU value '" + arch + "'"
-                     " to the right postmarketOS device")
-
-
-def qemu_check_device(device, arch):
-    """
-    Check whether a device has a specific architecture.
-
-    Examples:
-        qemu_check_device("qemu-amd64", "x86_64") is True
-        qemu_check_device("qemu-vexpress", "armel") is True
-        qemu_check_device("qemu-vexpress", "aarch64") is False
-    """
-    arch_qemu = uname_to_qemu(arch)
-    return device == qemu_to_pmos_device(arch_qemu)
```

### Comparing `pmbootstrap-1.9.0/pmb/parse/depends.py` & `pmbootstrap-2.0.0/pmb/parse/depends.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 import pmb.chroot
 import pmb.chroot.apk
 import pmb.helpers.pmaports
 import pmb.parse.apkindex
 import pmb.parse.arch
 
@@ -31,21 +15,21 @@
     """
     # Get the aport
     aport = pmb.helpers.pmaports.find(args, pkgname_depend, False)
     if not aport:
         return None
 
     # Parse its version
-    apkbuild = pmb.parse.apkbuild(args, aport + "/APKBUILD")
+    apkbuild = pmb.parse.apkbuild(f"{aport}/APKBUILD")
     pkgname = apkbuild["pkgname"]
     version = apkbuild["pkgver"] + "-r" + apkbuild["pkgrel"]
 
     # Return the dict
-    logging.verbose(pkgname_depend + ": provided by: " + pkgname + "-" +
-                    version + " in " + aport)
+    logging.verbose(
+        f"{pkgname_depend}: provided by: {pkgname}-{version} in {aport}")
     return {"pkgname": pkgname,
             "depends": apkbuild["depends"],
             "version": version}
 
 
 def package_provider(args, pkgname, pkgnames_install, suffix="native"):
     """
@@ -58,42 +42,47 @@
     providers = pmb.parse.apkindex.providers(args, pkgname, arch, False)
 
     # 0. No provider
     if len(providers) == 0:
         return None
 
     # 1. Only one provider
-    logging.verbose(pkgname + ": provided by: " + ", ".join(providers))
+    logging.verbose(f"{pkgname}: provided by: {', '.join(providers)}")
     if len(providers) == 1:
         return list(providers.values())[0]
 
     # 2. Provider with the same package name
     if pkgname in providers:
-        logging.verbose(pkgname + ": choosing package of the same name as"
-                        " provider")
+        logging.verbose(f"{pkgname}: choosing package of the same name as "
+                        "provider")
         return providers[pkgname]
 
     # 3. Pick a package that will be installed anyway
     for provider_pkgname, provider in providers.items():
         if provider_pkgname in pkgnames_install:
-            logging.verbose(pkgname + ": choosing provider '" +
-                            provider_pkgname + "', because it will be"
-                            " installed anyway")
+            logging.verbose(f"{pkgname}: choosing provider '{provider_pkgname}"
+                            "', because it will be installed anyway")
             return provider
 
     # 4. Pick a package that is already installed
     installed = pmb.chroot.apk.installed(args, suffix)
     for provider_pkgname, provider in providers.items():
         if provider_pkgname in installed:
-            logging.verbose(pkgname + ": choosing provider '" +
-                            provider_pkgname + "', because it is installed in"
-                            " the '" + suffix + "' chroot already")
+            logging.verbose(f"{pkgname}: choosing provider '{provider_pkgname}"
+                            f"', because it is installed in the '{suffix}' "
+                            "chroot already")
             return provider
 
-    # 5. Pick the provider
+    # 5. Pick the provider(s) with the highest priority
+    providers = pmb.parse.apkindex.provider_highest_priority(
+        providers, pkgname)
+    if len(providers) == 1:
+        return list(providers.values())[0]
+
+    # 6. Pick the shortest provider. (Note: Normally apk would fail here!)
     return pmb.parse.apkindex.provider_shortest(providers, pkgname)
 
 
 def package_from_index(args, pkgname_depend, pkgnames_install, package_aport,
                        suffix="native"):
     """
     :returns: None when there is no aport and no binary package, or a dict with
@@ -123,44 +112,68 @@
     """
     Find all dependencies of the given pkgnames.
 
     :param suffix: the chroot suffix to resolve dependencies for. If a package
                    has multiple providers, we look at the installed packages in
                    the chroot to make a decision (see package_provider()).
     :returns: list of pkgnames: consists of the initial pkgnames plus all
-              depends
+              depends. Dependencies explicitly marked as conflicting are
+              prefixed with !.
     """
-    logging.debug("(" + suffix + ") calculate depends of " +
-                  ", ".join(pkgnames) + " (pmbootstrap -v for details)")
+    logging.debug(f"({suffix}) calculate depends of {', '.join(pkgnames)} "
+                  "(pmbootstrap -v for details)")
 
     # Iterate over todo-list until is is empty
     todo = list(pkgnames)
+    required_by = {}
     ret = []
     while len(todo):
         # Skip already passed entries
         pkgname_depend = todo.pop(0)
         if pkgname_depend in ret:
             continue
 
+        # Check if the dependency is explicitly marked as conflicting
+        is_conflict = pkgname_depend.startswith("!")
+        pkgname_depend = pkgname_depend.lstrip("!")
+
         # Get depends and pkgname from aports
         pkgnames_install = list(ret) + todo
         package = package_from_aports(args, pkgname_depend)
         package = package_from_index(args, pkgname_depend, pkgnames_install,
                                      package, suffix)
 
         # Nothing found
         if not package:
-            raise RuntimeError("Could not find dependency '" + pkgname_depend +
-                               "' in any aports folder or APKINDEX. See:"
-                               " <https://postmarketos.org/depends>")
+            if is_conflict:
+                # This package was probably dropped from the repos, so we don't
+                # care if it doesn't exist since it's a conflicting depend that
+                # wouldn't be installed anyways.
+                continue
+            source = 'world'
+            if pkgname_depend in required_by:
+                source = ', '.join(required_by[pkgname_depend])
+            raise RuntimeError(f"Could not find dependency '{pkgname_depend}' "
+                               "in checked out pmaports dir or any APKINDEX. "
+                               f"Required by '{source}'. See: "
+                               "https://postmarketos.org/depends")
 
-        # Append to todo/ret (unless it is a duplicate)
+        # Determine pkgname
         pkgname = package["pkgname"]
+        if is_conflict:
+            pkgname = f"!{pkgname}"
+
+        # Append to todo/ret (unless it is a duplicate)
         if pkgname in ret:
-            logging.verbose(pkgname + ": already found")
+            logging.verbose(f"{pkgname}: already found")
         else:
-            depends = package["depends"]
-            logging.verbose(pkgname + ": depends on: " + ",".join(depends))
-            if depends:
-                todo += depends
+            if not is_conflict:
+                depends = package["depends"]
+                logging.verbose(f"{pkgname}: depends on: {','.join(depends)}")
+                if depends:
+                    todo += depends
+                    for dep in depends:
+                        if dep not in required_by:
+                            required_by[dep] = set()
+                        required_by[dep].add(pkgname_depend)
             ret.append(pkgname)
     return ret
```

### Comparing `pmbootstrap-1.9.0/pmb/parse/apkindex.py` & `pmbootstrap-2.0.0/pmb/parse/apkindex.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,19 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import collections
 import logging
 import os
 import tarfile
 import pmb.chroot.apk
 import pmb.helpers.repo
 import pmb.parse.version
 
 
-def parse_next_block(args, path, lines, start):
+def parse_next_block(path, lines, start):
     """
     Parse the next block in an APKINDEX.
 
     :param path: to the APKINDEX.tar.gz
     :param start: current index in lines, gets increased in this
                   function. Wrapped into a list, so it can be modified
                   "by reference". Example: [5]
@@ -54,14 +38,15 @@
     ret = {}
     mapping = {
         "A": "arch",
         "D": "depends",
         "o": "origin",
         "P": "pkgname",
         "p": "provides",
+        "k": "provider_priority",
         "t": "timestamp",
         "V": "version",
     }
     end_of_block_found = False
     for i in range(start[0], len(lines)):
         # Check for empty line
         start[0] = i + 1
@@ -82,26 +67,24 @@
                 ret[key] = line[2:-1]
 
     # Format and return the block
     if end_of_block_found:
         # Check for required keys
         for key in ["arch", "pkgname", "version"]:
             if key not in ret:
-                raise RuntimeError("Missing required key '" + key +
-                                   "' in block " + str(ret) + ", file: " + path)
+                raise RuntimeError(f"Missing required key '{key}' in block "
+                                   f"{ret}, file: {path}")
 
         # Format optional lists
         for key in ["provides", "depends"]:
             if key in ret and ret[key] != "":
                 # Ignore all operators for now
                 values = ret[key].split(" ")
                 ret[key] = []
                 for value in values:
-                    if value.startswith("!"):
-                        continue
                     for operator in [">", "=", "<", "~"]:
                         if operator in value:
                             value = value.split(operator)[0]
                             break
                     ret[key].append(value)
             else:
                 ret[key] = []
@@ -115,15 +98,15 @@
     return None
 
 
 def parse_add_block(ret, block, alias=None, multiple_providers=True):
     """
     Add one block to the return dictionary of parse().
 
-    :param ret: dictionary of all packages in the APKINDEX, that is
+    :param ret: dictionary of all packages in the APKINDEX that is
                 getting built right now. This function will extend it.
     :param block: return value from parse_next_block().
     :param alias: defaults to the pkgname, could be an alias from the
                   "provides" list.
     :param multiple_providers: assume that there are more than one provider for
                                the alias. This makes sense when parsing the
                                APKINDEX files from a repository (#1122), but
@@ -153,15 +136,15 @@
         if alias not in ret:
             ret[alias] = {}
         ret[alias][pkgname] = block
     else:
         ret[alias] = block
 
 
-def parse(args, path, multiple_providers=True):
+def parse(path, multiple_providers=True):
     """
     Parse an APKINDEX.tar.gz file, and return its content as dictionary.
 
     :param path: path to an APKINDEX.tar.gz file or apk package database
                  (almost the same format, but not compressed).
     :param multiple_providers: assume that there are more than one provider for
                                the alias. This makes sense when parsing the
@@ -190,36 +173,36 @@
         logging.verbose("NOTE: APKINDEX not found, assuming no binary packages"
                         " exist for that architecture: " + path)
         return {}
 
     # Try to get a cached result first
     lastmod = os.path.getmtime(path)
     cache_key = "multiple" if multiple_providers else "single"
-    if path in args.cache["apkindex"]:
-        cache = args.cache["apkindex"][path]
+    if path in pmb.helpers.other.cache["apkindex"]:
+        cache = pmb.helpers.other.cache["apkindex"][path]
         if cache["lastmod"] == lastmod:
             if cache_key in cache:
                 return cache[cache_key]
         else:
-            clear_cache(args, path)
+            clear_cache(path)
 
     # Read all lines
     if tarfile.is_tarfile(path):
         with tarfile.open(path, "r:gz") as tar:
             with tar.extractfile(tar.getmember("APKINDEX")) as handle:
                 lines = handle.readlines()
     else:
         with open(path, "r", encoding="utf-8") as handle:
             lines = handle.readlines()
 
     # Parse the whole APKINDEX file
     ret = collections.OrderedDict()
     start = [0]
     while True:
-        block = parse_next_block(args, path, lines, start)
+        block = parse_next_block(path, lines, start)
         if not block:
             break
 
         # Skip virtual packages
         if "timestamp" not in block:
             logging.verbose("Skipped virtual package " + str(block) + " in"
                             " file: " + path)
@@ -228,21 +211,21 @@
         # Add the next package and all aliases
         parse_add_block(ret, block, None, multiple_providers)
         if "provides" in block:
             for alias in block["provides"]:
                 parse_add_block(ret, block, alias, multiple_providers)
 
     # Update the cache
-    if path not in args.cache["apkindex"]:
-        args.cache["apkindex"][path] = {"lastmod": lastmod}
-    args.cache["apkindex"][path][cache_key] = ret
+    if path not in pmb.helpers.other.cache["apkindex"]:
+        pmb.helpers.other.cache["apkindex"][path] = {"lastmod": lastmod}
+    pmb.helpers.other.cache["apkindex"][path][cache_key] = ret
     return ret
 
 
-def parse_blocks(args, path):
+def parse_blocks(path):
     """
     Read all blocks from an APKINDEX.tar.gz into a list.
 
     :path: full path to the APKINDEX.tar.gz file.
     :returns: all blocks in the APKINDEX, without restructuring them by
               pkgname or removing duplicates with lower versions (use
               parse() if you need these features). Structure:
@@ -255,33 +238,33 @@
         with tar.extractfile(tar.getmember("APKINDEX")) as handle:
             lines = handle.readlines()
 
     # Parse lines into blocks
     ret = []
     start = [0]
     while True:
-        block = pmb.parse.apkindex.parse_next_block(args, path, lines, start)
+        block = pmb.parse.apkindex.parse_next_block(path, lines, start)
         if not block:
             return ret
         ret.append(block)
 
 
-def clear_cache(args, path):
+def clear_cache(path):
     """
     Clear the APKINDEX parsing cache.
 
     :returns: True on successful deletion, False otherwise
     """
     logging.verbose("Clear APKINDEX cache for: " + path)
-    if path in args.cache["apkindex"]:
-        del args.cache["apkindex"][path]
+    if path in pmb.helpers.other.cache["apkindex"]:
+        del pmb.helpers.other.cache["apkindex"][path]
         return True
     else:
         logging.verbose("Nothing to do, path was not in cache:" +
-                        str(args.cache["apkindex"].keys()))
+                        str(pmb.helpers.other.cache["apkindex"].keys()))
         return False
 
 
 def providers(args, package, arch=None, must_exist=True, indexes=None):
     """
     Get all packages, which provide one package.
 
@@ -293,26 +276,26 @@
                     (depending on arch)
     :returns: list of parsed packages. Example for package="so:libGL.so.1":
                   {"mesa-egl": block, "libhybris": block}
               block is the return value from parse_next_block() above.
     """
 
     if not indexes:
-        arch = arch or args.arch_native
+        arch = arch or pmb.config.arch_native
         indexes = pmb.helpers.repo.apkindex_files(args, arch)
 
     for operator in [">", ">=", "=", "<=", "<", "~"]:
         if operator in package:
             package = package.split(operator)[0]
             break
 
     ret = collections.OrderedDict()
     for path in indexes:
         # Skip indexes not providing the package
-        index_packages = parse(args, path)
+        index_packages = parse(path)
         if package not in index_packages:
             continue
 
         # Iterate over found providers
         for provider_pkgname, provider in index_packages[package].items():
             # Skip lower versions of providers we already found
             version = provider["version"]
@@ -333,27 +316,55 @@
     if ret == {} and must_exist:
         logging.debug("Searched in APKINDEX files: " + ", ".join(indexes))
         raise RuntimeError("Could not find package '" + package + "'!")
 
     return ret
 
 
+def provider_highest_priority(providers, pkgname):
+    """
+    Get the provider(s) with the highest provider_priority and log a message.
+
+    :param providers: returned dict from providers(), must not be empty
+    :param pkgname: the package name we are interested in (for the log message)
+    """
+    max_priority = 0
+    priority_providers = collections.OrderedDict()
+    for provider_name, provider in providers.items():
+        priority = int(provider.get("provider_priority", -1))
+        if priority > max_priority:
+            priority_providers.clear()
+            max_priority = priority
+        if priority == max_priority:
+            priority_providers[provider_name] = provider
+
+    if priority_providers:
+        logging.debug(
+            f"{pkgname}: picked provider(s) with highest priority "
+            f"{max_priority}: {', '.join(priority_providers.keys())}")
+        return priority_providers
+
+    # None of the providers seems to have a provider_priority defined
+    return providers
+
+
 def provider_shortest(providers, pkgname):
     """
     Get the provider with the shortest pkgname and log a message. In most cases
     this should be sufficient, e.g. 'mesa-purism-gc7000-egl, mesa-egl' or
     'gtk+2.0-maemo, gtk+2.0'.
 
     :param providers: returned dict from providers(), must not be empty
     :param pkgname: the package name we are interested in (for the log message)
     """
     ret = min(list(providers.keys()), key=len)
     if len(providers) != 1:
-        logging.debug(pkgname + ": has multiple providers (" +
-                      ", ".join(providers.keys()) + "), picked shortest: " + ret)
+        logging.debug(
+            f"{pkgname}: has multiple providers ("
+            f"{', '.join(providers.keys())}), picked shortest: {ret}")
     return providers[ret]
 
 
 def package(args, package, arch=None, must_exist=True, indexes=None):
     """
     Get a specific package's data from an apkindex.
```

### Comparing `pmbootstrap-1.9.0/pmb/aportgen/gcc.py` & `pmbootstrap-2.0.0/pmb/aportgen/gcc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,69 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import pmb.aportgen.core
 import pmb.helpers.git
 import pmb.helpers.run
 
 
 def generate(args, pkgname):
     # Copy original aport
     prefix = pkgname.split("-")[0]
     arch = pkgname.split("-")[1]
     if prefix == "gcc":
-        upstream = pmb.aportgen.core.get_upstream_aport(args, "gcc")
+        upstream = pmb.aportgen.core.get_upstream_aport(args, "gcc", arch)
         based_on = "main/gcc (from Alpine)"
     elif prefix == "gcc4":
-        upstream = args.aports + "/main/gcc4"
+        upstream = f"{args.aports}/main/gcc4"
         based_on = "main/gcc4 (from postmarketOS)"
     elif prefix == "gcc6":
-        upstream = args.aports + "/main/gcc6"
+        upstream = f"{args.aports}/main/gcc6"
         based_on = "main/gcc6 (from postmarketOS)"
     else:
-        raise ValueError("Invalid prefix '" + prefix + "', expected gcc, gcc4 or"
+        raise ValueError(f"Invalid prefix '{prefix}', expected gcc, gcc4 or"
                          " gcc6.")
-    pmb.helpers.run.user(args, ["cp", "-r", upstream, args.work + "/aportgen"])
+    pmb.helpers.run.user(args, ["cp", "-r", upstream, f"{args.work}/aportgen"])
 
-    # Rewrite APKBUILD (only building for x86_64 covers most use cases and
+    # Rewrite APKBUILD (only building for native covers most use cases and
     # saves a lot of build time, can be changed on demand)
     fields = {
         "pkgname": pkgname,
-        "pkgdesc": "Stage2 cross-compiler for " + arch,
-        "arch": "x86_64",
-        "depends": "isl binutils-" + arch + " mpc1",
-        "makedepends_build": "gcc g++ paxmark bison flex texinfo gawk zip gmp-dev mpfr-dev mpc1-dev zlib-dev",
-        "makedepends_host": "linux-headers gmp-dev mpfr-dev mpc1-dev isl-dev zlib-dev musl-dev-" + arch + " binutils-" + arch,
-        "subpackages": "g++-" + arch + ":gpp" if prefix == "gcc" else "",
+        "pkgdesc": f"Stage2 cross-compiler for {arch}",
+        "arch": pmb.config.arch_native,
+        "depends": f"binutils-{arch} mpc1",
+        "makedepends_build": "gcc g++ bison flex texinfo gawk zip"
+                             " gmp-dev mpfr-dev mpc1-dev zlib-dev",
+        "makedepends_host": "linux-headers gmp-dev mpfr-dev mpc1-dev isl-dev"
+                            f" zlib-dev musl-dev-{arch} binutils-{arch}",
+        "subpackages": "",
 
         # gcc6: options is already there, so we need to replace it and not only
         # set it below the header like done below.
-        "options": "!strip !tracedeps",
+        "options": "!strip",
 
         "LIBGOMP": "false",
         "LIBGCC": "false",
         "LIBATOMIC": "false",
         "LIBITM": "false",
     }
 
+    # Latest gcc only, not gcc4 and gcc6
+    if prefix == "gcc":
+        fields["subpackages"] = f"g++-{arch}:gpp" \
+                                f" libstdc++-dev-{arch}:libcxx_dev"
+
     below_header = "CTARGET_ARCH=" + arch + """
         CTARGET="$(arch_to_hostspec ${CTARGET_ARCH})"
+        LANG_D=false
         LANG_OBJC=false
         LANG_JAVA=false
         LANG_GO=false
         LANG_FORTRAN=false
         LANG_ADA=false
-        options="!strip !tracedeps"
+        options="!strip"
 
         # abuild doesn't try to tries to install "build-base-$CTARGET_ARCH"
         # when this variable matches "no*"
         BOOTSTRAP="nobuildbase"
 
         # abuild will only cross compile when this variable is set, but it
         # needs to find a valid package database in there for dependency
@@ -87,12 +79,15 @@
         # pmbootstrap picks it up properly).
         '*subpackages="$subpackages libstdc++:libcxx:*': None,
 
         # We set the cross_configure variable at the beginning, so it does not
         # use CBUILDROOT as sysroot. In the original APKBUILD this is a local
         # variable, but we make it a global one.
         '*_cross_configure=*': None,
+
+        # Do not build foreign arch libgcc, we use the one from Alpine (#2168)
+        '_libgcc=true*': '_libgcc=false',
     }
 
     pmb.aportgen.core.rewrite(args, pkgname, based_on, fields,
                               replace_simple=replace_simple,
                               below_header=below_header)
```

### Comparing `pmbootstrap-1.9.0/pmb/aportgen/__init__.py` & `pmbootstrap-2.0.0/pmb/aportgen/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import os
 import logging
 import pmb.aportgen.binutils
 import pmb.aportgen.busybox_static
 import pmb.aportgen.device
 import pmb.aportgen.gcc
 import pmb.aportgen.linux
@@ -49,31 +33,35 @@
     logging.info("NOTE: If you wanted to package new software in general, try"
                  " 'pmbootstrap newapkbuild' to generate a template.")
     raise ValueError("No generator available for " + pkgname + "!")
 
 
 def generate(args, pkgname):
     if args.fork_alpine:
-        prefix, folder, options = (pkgname, "temp", {"confirm_overwrite": True})
+        prefix, folder, options = (pkgname, "temp",
+                                   {"confirm_overwrite": True})
     else:
         prefix, folder, options = properties(pkgname)
     path_target = args.aports + "/" + folder + "/" + pkgname
 
     # Confirm overwrite
     if options["confirm_overwrite"] and os.path.exists(path_target):
-        logging.warning("WARNING: Target folder already exists: " + path_target)
+        logging.warning("WARNING: Target folder already exists: "
+                        f"{path_target}")
         if not pmb.helpers.cli.confirm(args, "Continue and overwrite?"):
             raise RuntimeError("Aborted.")
 
     if os.path.exists(args.work + "/aportgen"):
         pmb.helpers.run.user(args, ["rm", "-r", args.work + "/aportgen"])
     if args.fork_alpine:
         upstream = pmb.aportgen.core.get_upstream_aport(args, pkgname)
-        pmb.helpers.run.user(args, ["cp", "-r", upstream, args.work + "/aportgen"])
-        pmb.aportgen.core.rewrite(args, pkgname, replace_simple={"# Contributor:*": None, "# Maintainer:*": None})
+        pmb.helpers.run.user(args, ["cp", "-r", upstream,
+                                    f"{args.work}/aportgen"])
+        pmb.aportgen.core.rewrite(args, pkgname, replace_simple={
+            "# Contributor:*": None, "# Maintainer:*": None})
     else:
         # Run pmb.aportgen.PREFIX.generate()
         getattr(pmb.aportgen, prefix.replace("-", "_")).generate(args, pkgname)
 
     # Move to the aports folder
     if os.path.exists(path_target):
         pmb.helpers.run.user(args, ["rm", "-r", path_target])
```

### Comparing `pmbootstrap-1.9.0/pmb/aportgen/device.py` & `pmbootstrap-2.0.0/pmb/aportgen/device.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,251 +1,319 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 import os
+import pmb.helpers.cli
 import pmb.helpers.run
 import pmb.aportgen.core
 import pmb.parse.apkindex
 import pmb.parse.bootimg
 
 
-def ask_for_architecture(args):
+def ask_for_architecture():
     architectures = pmb.config.build_device_architectures
+    # Don't show armhf, new ports shouldn't use this architecture
+    if "armhf" in architectures:
+        architectures.remove("armhf")
     while True:
-        ret = pmb.helpers.cli.ask(args, "Device architecture", architectures,
-                                  architectures[0])
+        ret = pmb.helpers.cli.ask("Device architecture", architectures,
+                                  architectures[0], complete=architectures)
         if ret in architectures:
             return ret
         logging.fatal("ERROR: Invalid architecture specified. If you want to"
-                      " add a new architecture, edit build_device_architectures"
-                      " in pmb/config/__init__.py.")
+                      " add a new architecture, edit"
+                      " build_device_architectures in"
+                      " pmb/config/__init__.py.")
 
 
-def ask_for_manufacturer(args):
+def ask_for_manufacturer():
     logging.info("Who produced the device (e.g. LG)?")
-    return pmb.helpers.cli.ask(args, "Manufacturer", None, None, False)
+    return pmb.helpers.cli.ask("Manufacturer", None, None, False)
 
 
-def ask_for_name(args, manufacturer):
+def ask_for_name(manufacturer):
     logging.info("What is the official name (e.g. Google Nexus 5)?")
-    ret = pmb.helpers.cli.ask(args, "Name", None, None, False)
+    ret = pmb.helpers.cli.ask("Name", None, None, False)
 
     # Always add the manufacturer
     if not ret.startswith(manufacturer) and \
             not ret.startswith("Google"):
         ret = manufacturer + " " + ret
     return ret
 
 
+def ask_for_year():
+    # Regex from https://stackoverflow.com/a/12240826
+    logging.info("In what year was the device released (e.g. 2012)?")
+    return pmb.helpers.cli.ask("Year", None, None, False,
+                               validation_regex=r'^[1-9]\d{3,}$')
+
+
+def ask_for_chassis():
+    types = pmb.config.deviceinfo_chassis_types
+
+    logging.info("What type of device is it?")
+    logging.info("Valid types are: " + ", ".join(types))
+    return pmb.helpers.cli.ask("Chassis", None, None, True,
+                               validation_regex='|'.join(types),
+                               complete=types)
+
+
 def ask_for_keyboard(args):
-    return pmb.helpers.cli.confirm(args, "Does the device have a hardware keyboard?")
+    return pmb.helpers.cli.confirm(args, "Does the device have a hardware"
+                                   " keyboard?")
 
 
 def ask_for_external_storage(args):
-    return pmb.helpers.cli.confirm(args, "Does the device have a sdcard or other"
-                                   " external storage medium?")
+    return pmb.helpers.cli.confirm(args, "Does the device have a sdcard or"
+                                   " other external storage medium?")
 
 
-def ask_for_flash_method(args):
+def ask_for_flash_method():
     while True:
         logging.info("Which flash method does the device support?")
-        method = pmb.helpers.cli.ask(args, "Flash method", pmb.config.flash_methods,
-                                     pmb.config.flash_methods[0])
+        method = pmb.helpers.cli.ask("Flash method",
+                                     pmb.config.flash_methods,
+                                     pmb.config.flash_methods[0],
+                                     complete=pmb.config.flash_methods)
 
         if method in pmb.config.flash_methods:
             if method == "heimdall":
                 heimdall_types = ["isorec", "bootimg"]
                 while True:
-                    logging.info("Does the device use the \"isolated recovery\" or boot.img?")
-                    logging.info("<https://wiki.postmarketos.org/wiki/Deviceinfo_flash_methods#Isorec_or_bootimg.3F>")
-                    heimdall_type = pmb.helpers.cli.ask(args, "Type", heimdall_types,
+                    logging.info("Does the device use the \"isolated"
+                                 " recovery\" or boot.img?")
+                    logging.info("<https://wiki.postmarketos.org/wiki"
+                                 "/Deviceinfo_flash_methods#Isorec_or_bootimg"
+                                 ".3F>")
+                    heimdall_type = pmb.helpers.cli.ask("Type",
+                                                        heimdall_types,
                                                         heimdall_types[0])
                     if heimdall_type in heimdall_types:
                         method += "-" + heimdall_type
                         break
                     logging.fatal("ERROR: Invalid type specified.")
             return method
 
         logging.fatal("ERROR: Invalid flash method specified. If you want to"
                       " add a new flash method, edit flash_methods in"
                       " pmb/config/__init__.py.")
 
 
 def ask_for_bootimg(args):
-    logging.info("You can analyze a known working boot.img file to automatically fill"
-                 " out the flasher information for your deviceinfo file. Either specify"
-                 " the path to an image or press return to skip this step (you can do"
-                 " it later with 'pmbootstrap bootimg_analyze').")
+    logging.info("You can analyze a known working boot.img file to"
+                 " automatically fill out the flasher information for your"
+                 " deviceinfo file. Either specify the path to an image or"
+                 " press return to skip this step (you can do it later with"
+                 " 'pmbootstrap bootimg_analyze').")
 
     while True:
-        path = os.path.expanduser(pmb.helpers.cli.ask(args, "Path", None, "", False))
+        response = pmb.helpers.cli.ask("Path", None, "", False)
+        path = os.path.expanduser(response)
         if not path:
             return None
         try:
             return pmb.parse.bootimg(args, path)
         except Exception as e:
             logging.fatal("ERROR: " + str(e) + ". Please try again.")
 
 
-def generate_deviceinfo_fastboot_content(args, bootimg=None):
+def generate_deviceinfo_fastboot_content(bootimg=None):
     if bootimg is None:
         bootimg = {"cmdline": "",
                    "qcdt": "false",
+                   "mtk_mkimage": "false",
+                   "dtb_second": "false",
                    "base": "",
                    "kernel_offset": "",
                    "ramdisk_offset": "",
                    "second_offset": "",
                    "tags_offset": "",
                    "pagesize": "2048"}
-    return """\
-        deviceinfo_kernel_cmdline=\"""" + bootimg["cmdline"] + """\"
+
+    content = f"""\
+        deviceinfo_kernel_cmdline="{bootimg["cmdline"]}"
         deviceinfo_generate_bootimg="true"
-        deviceinfo_bootimg_qcdt=\"""" + bootimg["qcdt"] + """\"
-        deviceinfo_flash_offset_base=\"""" + bootimg["base"] + """\"
-        deviceinfo_flash_offset_kernel=\"""" + bootimg["kernel_offset"] + """\"
-        deviceinfo_flash_offset_ramdisk=\"""" + bootimg["ramdisk_offset"] + """\"
-        deviceinfo_flash_offset_second=\"""" + bootimg["second_offset"] + """\"
-        deviceinfo_flash_offset_tags=\"""" + bootimg["tags_offset"] + """\"
-        deviceinfo_flash_pagesize=\"""" + bootimg["pagesize"] + """\"
+        deviceinfo_bootimg_qcdt="{bootimg["qcdt"]}"
+        deviceinfo_bootimg_mtk_mkimage="{bootimg["mtk_mkimage"]}"
+        deviceinfo_bootimg_dtb_second="{bootimg["dtb_second"]}"
+        deviceinfo_flash_pagesize="{bootimg["pagesize"]}"
+        """
+
+    if "header_version" in bootimg.keys():
+        content += f"""\
+        deviceinfo_header_version="{bootimg["header_version"]}"
+        """
+
+        if bootimg["header_version"] == "2":
+            content += f"""\
+            deviceinfo_append_dtb="false"
+            deviceinfo_flash_offset_dtb="{bootimg["dtb_offset"]}"
+            """
+
+    if "base" in bootimg.keys():
+        content += f"""\
+        deviceinfo_flash_offset_base="{bootimg["base"]}"
+        deviceinfo_flash_offset_kernel="{bootimg["kernel_offset"]}"
+        deviceinfo_flash_offset_ramdisk="{bootimg["ramdisk_offset"]}"
+        deviceinfo_flash_offset_second="{bootimg["second_offset"]}"
+        deviceinfo_flash_offset_tags="{bootimg["tags_offset"]}"
         """
 
+    return content
+
 
-def generate_deviceinfo(args, pkgname, name, manufacturer, arch, has_keyboard,
-                        has_external_storage, flash_method, bootimg=None):
+def generate_deviceinfo(args, pkgname, name, manufacturer, year, arch,
+                        chassis, has_keyboard, has_external_storage,
+                        flash_method, bootimg=None):
     codename = "-".join(pkgname.split("-")[1:])
+    external_storage = "true" if has_external_storage else "false"
     # Note: New variables must be added to pmb/config/__init__.py as well
-    content = """\
+    content = f"""\
         # Reference: <https://postmarketos.org/deviceinfo>
-        # Please use double quotes only. You can source this file in shell scripts.
+        # Please use double quotes only. You can source this file in shell
+        # scripts.
 
         deviceinfo_format_version="0"
-        deviceinfo_name=\"""" + name + """\"
-        deviceinfo_manufacturer=\"""" + manufacturer + """\"
-        deviceinfo_codename=\"""" + codename + """\"
-        deviceinfo_date=""
+        deviceinfo_name="{name}"
+        deviceinfo_manufacturer="{manufacturer}"
+        deviceinfo_codename="{codename}"
+        deviceinfo_year="{year}"
         deviceinfo_dtb=""
-        deviceinfo_modules_initfs=""
-        deviceinfo_arch=\"""" + arch + """\"
+        deviceinfo_arch="{arch}"
 
         # Device related
-        deviceinfo_keyboard=\"""" + ("true" if has_keyboard else "false") + """\"
-        deviceinfo_external_storage=\"""" + ("true" if has_external_storage else "false") + """\"
+        deviceinfo_chassis="{chassis}"
+        deviceinfo_keyboard="{"true" if has_keyboard else "false"}"
+        deviceinfo_external_storage="{external_storage}"
         deviceinfo_screen_width="800"
         deviceinfo_screen_height="600"
-        deviceinfo_dev_touchscreen=""
-        deviceinfo_dev_touchscreen_calibration=""
-        deviceinfo_dev_keyboard=""
 
         # Bootloader related
-        deviceinfo_flash_method=\"""" + flash_method + """\"
+        deviceinfo_flash_method="{flash_method}"
         """
 
     content_heimdall_bootimg = """\
         deviceinfo_flash_heimdall_partition_kernel=""
-        deviceinfo_flash_heimdall_partition_system=""
+        deviceinfo_flash_heimdall_partition_rootfs=""
         """
 
     content_heimdall_isorec = """\
         deviceinfo_flash_heimdall_partition_kernel=""
         deviceinfo_flash_heimdall_partition_initfs=""
-        deviceinfo_flash_heimdall_partition_system=""
+        deviceinfo_flash_heimdall_partition_rootfs=""
         """
 
     content_0xffff = """\
         deviceinfo_generate_legacy_uboot_initfs="true"
         """
 
     content_uuu = """\
         deviceinfo_generate_legacy_uboot_initfs="true"
         """
 
     if flash_method == "fastboot":
-        content += generate_deviceinfo_fastboot_content(args, bootimg)
+        content += generate_deviceinfo_fastboot_content(bootimg)
     elif flash_method == "heimdall-bootimg":
-        content += generate_deviceinfo_fastboot_content(args, bootimg)
+        content += generate_deviceinfo_fastboot_content(bootimg)
         content += content_heimdall_bootimg
     elif flash_method == "heimdall-isorec":
         content += content_heimdall_isorec
     elif flash_method == "0xffff":
         content += content_0xffff
     elif flash_method == "uuu":
         content += content_uuu
 
     # Write to file
     pmb.helpers.run.user(args, ["mkdir", "-p", args.work + "/aportgen"])
-    with open(args.work + "/aportgen/deviceinfo", "w", encoding="utf-8") as handle:
-        for line in content.split("\n"):
+    path = args.work + "/aportgen/deviceinfo"
+    with open(path, "w", encoding="utf-8") as handle:
+        for line in content.rstrip().split("\n"):
+            handle.write(line.lstrip() + "\n")
+
+
+def generate_modules_initfs(args):
+    content = """\
+    # Remove this comment after reading, or the file if unnecessary (CHANGEME!)
+    # This file can contain a list of modules to be included in the initramfs,
+    # so that they are available in early boot stages. It should have one
+    # module name per line. If there are multiple kernel variants with different
+    # requirements for modules into the initramfs, one modules-initfs.$variant
+    # file should be created for each of them.
+    """
+
+    # Write to file
+    pmb.helpers.run.user(args, ["mkdir", "-p", args.work + "/aportgen"])
+    path = args.work + "/aportgen/modules-initfs"
+    with open(path, "w", encoding="utf-8") as handle:
+        for line in content.rstrip().split("\n"):
             handle.write(line.lstrip() + "\n")
 
 
 def generate_apkbuild(args, pkgname, name, arch, flash_method):
     # Dependencies
-    depends = "postmarketos-base linux-" + "-".join(pkgname.split("-")[1:])
+    depends = ["postmarketos-base",
+               "linux-" + "-".join(pkgname.split("-")[1:])]
     if flash_method in ["fastboot", "heimdall-bootimg"]:
-        depends += " mkbootimg"
+        depends.append("mkbootimg")
     if flash_method == "0xffff":
-        depends += " uboot-tools"
-    depends += " mesa-dri-swrast"
+        depends.append("uboot-tools")
 
     # Whole APKBUILD
-    content = """\
+    depends.sort()
+    depends = ("\n" + " " * 12).join(depends)
+    content = f"""\
         # Reference: <https://postmarketos.org/devicepkg>
-        pkgname=\"""" + pkgname + """\"
-        pkgdesc=\"""" + name + """\"
+        pkgname={pkgname}
+        pkgdesc="{name}"
         pkgver=0.1
         pkgrel=0
         url="https://postmarketos.org"
         license="MIT"
-        arch=\"""" + arch + """\"
+        arch="{arch}"
         options="!check !archcheck"
-        depends=\"""" + depends + """\"
+        depends="
+            {depends}
+        "
         makedepends="devicepkg-dev"
-        source="deviceinfo"
+        source="
+            deviceinfo
+            modules-initfs
+        "
 
-        build() {
+        build() {{
             devicepkg_build $startdir $pkgname
-        }
+        }}
 
-        package() {
+        package() {{
             devicepkg_package $startdir $pkgname
-        }
+        }}
 
-        sha512sums="(run 'pmbootstrap checksum """ + pkgname + """' to fill)"
+        sha512sums="(run 'pmbootstrap checksum {pkgname}' to fill)"
         """
 
     # Write the file
     pmb.helpers.run.user(args, ["mkdir", "-p", args.work + "/aportgen"])
-    with open(args.work + "/aportgen/APKBUILD", "w", encoding="utf-8") as handle:
-        for line in content.split("\n"):
+    path = args.work + "/aportgen/APKBUILD"
+    with open(path, "w", encoding="utf-8") as handle:
+        for line in content.rstrip().split("\n"):
             handle.write(line[8:].replace(" " * 4, "\t") + "\n")
 
 
 def generate(args, pkgname):
-    arch = ask_for_architecture(args)
-    manufacturer = ask_for_manufacturer(args)
-    name = ask_for_name(args, manufacturer)
+    arch = ask_for_architecture()
+    manufacturer = ask_for_manufacturer()
+    name = ask_for_name(manufacturer)
+    year = ask_for_year()
+    chassis = ask_for_chassis()
     has_keyboard = ask_for_keyboard(args)
     has_external_storage = ask_for_external_storage(args)
-    flash_method = ask_for_flash_method(args)
+    flash_method = ask_for_flash_method()
     bootimg = None
     if flash_method in ["fastboot", "heimdall-bootimg"]:
         bootimg = ask_for_bootimg(args)
 
-    generate_deviceinfo(args, pkgname, name, manufacturer, arch, has_keyboard,
-                        has_external_storage, flash_method, bootimg)
+    generate_deviceinfo(args, pkgname, name, manufacturer, year, arch,
+                        chassis, has_keyboard, has_external_storage,
+                        flash_method, bootimg)
+    generate_modules_initfs(args)
     generate_apkbuild(args, pkgname, name, arch, flash_method)
```

### Comparing `pmbootstrap-1.9.0/pmb/aportgen/core.py` & `pmbootstrap-2.0.0/pmb/aportgen/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import fnmatch
 import logging
 import re
 import glob
 import pmb.helpers.git
 
 
@@ -66,27 +50,28 @@
             replace_functions={}, replace_simple={}, below_header="",
             remove_indent=4):
     """
     Append a header to $WORK/aportgen/APKBUILD, delete maintainer/contributor
     lines (so they won't be bugged with issues regarding our generated aports),
     and add reference to the original aport.
 
-    :param path_original: The original path of the automatically generated aport
-    :param fields: key-value pairs of fields, that shall be changed in the
+    :param path_original: The original path of the automatically generated
+        aport.
+    :param fields: key-value pairs of fields that shall be changed in the
         APKBUILD. For example: {"pkgdesc": "my new package", "subpkgs": ""}
-    :param replace_pkgname: When set, $pkgname gets replaced with that string in
-        every line.
+    :param replace_pkgname: When set, $pkgname gets replaced with that string
+        in every line.
     :param replace_functions: Function names and new bodies, for example:
         {"build": "return 0"}
         The body can also be None (deletes the function)
-    :param replace_simple: Lines, that fnmatch the pattern, get
+    :param replace_simple: Lines that fnmatch the pattern, get
         replaced/deleted. Example: {"*test*": "# test", "*mv test.bin*": None}
-    :param below_header: String, that gets directly placed below the header.
-    :param remove_indent: Number of spaces to remove from function body provided
-        to replace_functions.
+    :param below_header: String that gets directly placed below the header.
+    :param remove_indent: Number of spaces to remove from function body
+        provided to replace_functions.
 
     """
     # Header
     if path_original:
         lines_new = [
             "# Automatically generated aport, do not edit!\n",
             "# Generator: pmbootstrap aportgen " + pkgname + "\n",
@@ -121,24 +106,32 @@
                     skip_in_func = False
                 continue
             else:
                 for func, body in replace_functions.items():
                     if line.startswith(func + "() {"):
                         skip_in_func = True
                         if body:
-                            lines_new += format_function(func, body,
-                                                         remove_indent=remove_indent)
+                            lines_new += format_function(
+                                func, body, remove_indent=remove_indent)
                         break
                 if skip_in_func:
                     continue
 
             # Replace fields
             for key, value in fields.items():
                 if line.startswith(key + "="):
-                    line = key + "=\"" + value + "\"\n"
+                    if value:
+                        if key in ["pkgname", "pkgver", "pkgrel"]:
+                            # No quotes to avoid lint error
+                            line = f"{key}={value}\n"
+                        else:
+                            line = f'{key}="{value}"\n'
+                    else:
+                        # Remove line without value to avoid lint error
+                        line = ""
                     break
 
             # Replace $pkgname
             if replace_pkgname and "$pkgname" in line:
                 line = line.replace("$pkgname", replace_pkgname)
 
             # Replace simple
@@ -155,60 +148,75 @@
 
         # Write back
         handle.seek(0)
         handle.write("".join(lines_new))
         handle.truncate()
 
 
-def get_upstream_aport(args, pkgname):
+def get_upstream_aport(args, pkgname, arch=None):
     """
     Perform a git checkout of Alpine's aports and get the path to the aport.
 
     :param pkgname: package name
+    :param arch: Alpine architecture (e.g. "armhf"), defaults to native arch
     :returns: absolute path on disk where the Alpine aport is checked out
               example: /opt/pmbootstrap_work/cache_git/aports/upstream/main/gcc
     """
     # APKBUILD
     pmb.helpers.git.clone(args, "aports_upstream")
     aports_upstream_path = args.work + "/cache_git/aports_upstream"
 
+    # Checkout branch
+    channel_cfg = pmb.config.pmaports.read_config_channel(args)
+    branch = channel_cfg["branch_aports"]
+    logging.info(f"Checkout aports.git branch: {branch}")
+    if pmb.helpers.run.user(args, ["git", "checkout", branch],
+                            aports_upstream_path, check=False):
+        logging.info("NOTE: run 'pmbootstrap pull' and try again")
+        logging.info("NOTE: if it still fails, your aports.git was cloned with"
+                     " an older version of pmbootstrap, as shallow clone."
+                     " Unshallow it, or remove it and let pmbootstrap clone it"
+                     f" again: {aports_upstream_path}")
+        raise RuntimeError("Branch checkout failed.")
+
     # Search package
     paths = glob.glob(aports_upstream_path + "/*/" + pkgname)
     if len(paths) > 1:
         raise RuntimeError("Package " + pkgname + " found in multiple"
                            " aports subfolders.")
     elif len(paths) == 0:
         raise RuntimeError("Package " + pkgname + " not found in alpine"
                            " aports repository.")
     aport_path = paths[0]
 
     # Parse APKBUILD
-    apkbuild = pmb.parse.apkbuild(args, aport_path + "/APKBUILD",
+    apkbuild = pmb.parse.apkbuild(f"{aport_path}/APKBUILD",
                                   check_pkgname=False)
     apkbuild_version = apkbuild["pkgver"] + "-r" + apkbuild["pkgrel"]
 
     # Binary package
     split = aport_path.split("/")
     repo = split[-2]
     pkgname = split[-1]
-    index_path = pmb.helpers.repo.alpine_apkindex_path(args, repo)
+    index_path = pmb.helpers.repo.alpine_apkindex_path(args, repo, arch)
     package = pmb.parse.apkindex.package(args, pkgname, indexes=[index_path])
 
     # Compare version (return when equal)
     compare = pmb.parse.version.compare(apkbuild_version, package["version"])
     if compare == 0:
         return aport_path
 
-    # Different version message
-    logging.error("ERROR: Package '" + pkgname + "' has a different version in"
+    # APKBUILD > binary: this is fine
+    if compare == 1:
+        logging.info(f"NOTE: {pkgname} {arch} binary package has a lower"
+                     f" version {package['version']} than the APKBUILD"
+                     f" {apkbuild_version}")
+        return aport_path
+
+    # APKBUILD < binary: aports.git is outdated
+    logging.error("ERROR: Package '" + pkgname + "' has a lower version in"
                   " local checkout of Alpine's aports (" + apkbuild_version +
                   ") compared to Alpine's binary package (" +
                   package["version"] + ")!")
 
-    # APKBUILD < binary
-    if compare == -1:
-        raise RuntimeError("You can update your local checkout with:"
-                           " 'pmbootstrap chroot --add=git --user -- git -C"
-                           " /mnt/pmbootstrap-git/aports_upstream pull'")
-    # APKBUILD > binary
-    raise RuntimeError("You can force an update of your binary package"
-                       " APKINDEX files with: 'pmbootstrap update'")
+    raise RuntimeError("You can update your local checkout with: "
+                       "'pmbootstrap pull'")
```

### Comparing `pmbootstrap-1.9.0/pmb/aportgen/linux.py` & `pmbootstrap-2.0.0/pmb/aportgen/linux.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,131 +1,128 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import pmb.helpers.run
 import pmb.aportgen.core
 import pmb.parse.apkindex
 import pmb.parse.arch
 
 
 def generate_apkbuild(args, pkgname, deviceinfo, patches):
     device = "-".join(pkgname.split("-")[1:])
     carch = pmb.parse.arch.alpine_to_kernel(deviceinfo["arch"])
 
-    makedepends = "perl sed installkernel bash gmp-dev bc linux-headers elfutils-dev devicepkg-dev"
-
-    package = """
-            # kernel.release
-            install -D "$builddir/include/config/kernel.release" \\
-                "$pkgdir/usr/share/kernel/$_flavor/kernel.release"
-
-            # zImage (find the right one)
-            cd "$builddir/arch/$_carch/boot"
-            _target="$pkgdir/boot/vmlinuz-$_flavor"
-            for _zimg in zImage-dtb Image.gz-dtb *zImage Image; do
-                [ -e "$_zimg" ] || continue
-                msg "zImage found: $_zimg"
-                install -Dm644 "$_zimg" "$_target"
-                break
-            done
-            if ! [ -e "$_target" ]; then
-                error "Could not find zImage in $PWD!"
-                return 1
-            fi"""
+    makedepends = ["bash", "bc", "bison", "devicepkg-dev", "findutils", "flex",
+                   "openssl-dev", "perl"]
 
     build = """
             unset LDFLAGS
-            make ARCH="$_carch" CC="${CC:-gcc}" \\
+            make O="$_outdir" ARCH="$_carch" CC="${CC:-gcc}" \\
                 KBUILD_BUILD_VERSION="$((pkgrel + 1 ))-postmarketOS\""""
 
-    if deviceinfo["bootimg_qcdt"] == "true":
-        makedepends += " dtbtool"
+    package = """
+            downstreamkernel_package "$builddir" "$pkgdir" "$_carch\" \\
+                "$_flavor" "$_outdir\""""
 
-        build += """\n
-            # Generate master DTB (deviceinfo_bootimg_qcdt)
-            dtbTool -s 2048 -p "scripts/dtc/" -o "arch/""" + carch + "/boot/dt.img\" \"arch/" + carch + "/boot/\""
+    if deviceinfo.get("header_version") == "2":
+        package += """
 
-        package += """\n
-            # Master DTB (deviceinfo_bootimg_qcdt)
-            install -Dm644 "$builddir/arch/""" + carch + """/boot/dt.img" \\
-                "$pkgdir/boot/dt.img\""""
+            make dtbs_install O="$_outdir" ARCH="$_carch" \\
+                INSTALL_DTBS_PATH="$pkgdir\"/boot/dtbs"""
 
-    content = """\
+    if deviceinfo["bootimg_qcdt"] == "true":
+        build += """\n
+            # Master DTB (deviceinfo_bootimg_qcdt)"""
+        vendors = ["spreadtrum", "exynos", "other"]
+        soc_vendor = pmb.helpers.cli.ask("SoC vendor", vendors,
+                                         vendors[-1], complete=vendors)
+        if soc_vendor == "spreadtrum":
+            makedepends.append("dtbtool-sprd")
+            build += """
+            dtbTool-sprd -p "$_outdir/scripts/dtc/" \\
+                -o "$_outdir/arch/$_carch/boot"/dt.img \\
+                "$_outdir/arch/$_carch/boot/dts/\""""
+        elif soc_vendor == "exynos":
+            codename = "-".join(pkgname.split("-")[2:])
+            makedepends.append("dtbtool-exynos")
+            build += """
+            dtbTool-exynos -o "$_outdir/arch/$_carch/boot"/dt.img \\
+                $(find "$_outdir/arch/$_carch/boot/dts/\""""
+            build += f" -name *{codename}*.dtb)"
+        else:
+            makedepends.append("dtbtool")
+            build += """
+            dtbTool -o "$_outdir/arch/$_carch/boot"/dt.img \\
+                "$_outdir/arch/$_carch/boot/\""""
+        package += """
+            install -Dm644 "$_outdir/arch/$_carch/boot"/dt.img \\
+                "$pkgdir"/boot/dt.img"""
+
+    makedepends.sort()
+    makedepends = ("\n" + " " * 12).join(makedepends)
+    patches = ("\n" + " " * 12).join(patches)
+    content = f"""\
         # Reference: <https://postmarketos.org/vendorkernel>
-        # Kernel config based on: arch/""" + carch + """/configs/(CHANGEME!)
+        # Kernel config based on: arch/{carch}/configs/(CHANGEME!)
 
-        pkgname=\"""" + pkgname + """\"
+        pkgname={pkgname}
         pkgver=3.x.x
         pkgrel=0
-        pkgdesc=\"""" + deviceinfo["name"] + """ kernel fork\"
-        arch=\"""" + deviceinfo["arch"] + """\"
-        _carch=\"""" + carch + """\"
-        _flavor=\"""" + device + """\"
+        pkgdesc="{deviceinfo["name"]} kernel fork"
+        arch="{deviceinfo["arch"]}"
+        _carch="{carch}"
+        _flavor="{device}"
         url="https://kernel.org"
         license="GPL-2.0-only"
-        options="!strip !check !tracedeps"
-        makedepends=\"""" + makedepends + """\"
-
-        # Compiler: latest GCC from Alpine
-        HOSTCC="${CC:-gcc}"
-        HOSTCC="${HOSTCC#${CROSS_COMPILE}}"
+        options="!strip !check !tracedeps pmb:cross-native"
+        makedepends="
+            {makedepends}
+        "
 
         # Source
         _repository="(CHANGEME!)"
         _commit="ffffffffffffffffffffffffffffffffffffffff"
-        _config="config-${_flavor}.${arch}"
+        _config="config-$_flavor.$arch"
         source="
-            $pkgname-$_commit.tar.gz::https://github.com/LineageOS/${_repository}/archive/${_commit}.tar.gz
-            $_config""" + ("\n" + " " * 12).join([""] + patches) + """
+            $pkgname-$_commit.tar.gz::https://github.com/LineageOS/$_repository/archive/$_commit.tar.gz
+            $_config
+            {patches}
         "
-        builddir="$srcdir/${_repository}-${_commit}"
+        builddir="$srcdir/$_repository-$_commit"
+        _outdir="out"
 
-        prepare() {
+        prepare() {{
             default_prepare
-            downstreamkernel_prepare "$srcdir" "$builddir" "$_config" "$_carch" "$HOSTCC"
-        }
+            . downstreamkernel_prepare
+        }}
 
-        build() {""" + build + """
-        }
+        build() {{{build}
+        }}
 
-        package() {""" + package + """
-        }
+        package() {{{package}
+        }}
 
-        sha512sums="(run 'pmbootstrap checksum """ + pkgname + """' to fill)\""""
+        sha512sums="(run 'pmbootstrap checksum {pkgname}' to fill)"
+        """
 
     # Write the file
-    with open(args.work + "/aportgen/APKBUILD", "w", encoding="utf-8") as handle:
-        for line in content.split("\n"):
-            handle.write(line[8:].replace(" " * 4, "\t") + "\n")
+    with open(f"{args.work}/aportgen/APKBUILD", "w", encoding="utf-8") as hndl:
+        for line in content.rstrip().split("\n"):
+            hndl.write(line[8:].replace(" " * 4, "\t") + "\n")
 
 
 def generate(args, pkgname):
     device = "-".join(pkgname.split("-")[1:])
     deviceinfo = pmb.parse.deviceinfo(args, device)
 
     # Symlink commonly used patches
     pmb.helpers.run.user(args, ["mkdir", "-p", args.work + "/aportgen"])
     patches = [
         "gcc7-give-up-on-ilog2-const-optimizations.patch",
         "gcc8-fix-put-user.patch",
+        "gcc10-extern_YYLOC_global_declaration.patch",
         "kernel-use-the-gnu89-standard-explicitly.patch",
     ]
     for patch in patches:
         pmb.helpers.run.user(args, ["ln", "-s",
                                     "../../.shared-patches/linux/" + patch,
                                     args.work + "/aportgen/" + patch])
```

### Comparing `pmbootstrap-1.9.0/pmb/helpers/file.py` & `pmbootstrap-2.0.0/pmb/helpers/file.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,59 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 import time
+
 import pmb.helpers.run
 
 
 def replace(path, old, new):
     text = ""
     with open(path, "r", encoding="utf-8") as handle:
         text = handle.read()
 
     text = text.replace(old, new)
 
     with open(path, "w", encoding="utf-8") as handle:
         handle.write(text)
 
 
+def replace_apkbuild(args, pkgname, key, new, in_quotes=False):
+    """ Replace one key=value line in an APKBUILD and verify it afterwards.
+        :param pkgname: package name, e.g. "hello-world"
+        :param key: key that should be replaced, e.g. "pkgver"
+        :param new: new value
+        :param in_quotes: expect the value to be in quotation marks ("") """
+    # Read old value
+    path = pmb.helpers.pmaports.find(args, pkgname) + "/APKBUILD"
+    apkbuild = pmb.parse.apkbuild(path)
+    old = apkbuild[key]
+
+    # Prepare old/new strings
+    if in_quotes:
+        line_old = '{}="{}"'.format(key, old)
+        line_new = '{}="{}"'.format(key, new)
+    else:
+        line_old = '{}={}'.format(key, old)
+        line_new = '{}={}'.format(key, new)
+
+    # Replace
+    replace(path, "\n" + line_old + "\n", "\n" + line_new + "\n")
+
+    # Verify
+    del (pmb.helpers.other.cache["apkbuild"][path])
+    apkbuild = pmb.parse.apkbuild(path)
+    if apkbuild[key] != str(new):
+        raise RuntimeError("Failed to set '{}' for pmaport '{}'. Make sure"
+                           " that there's a line with exactly the string '{}'"
+                           " and nothing else in: {}".format(key, pkgname,
+                                                             line_old, path))
+
+
 def is_up_to_date(path_sources, path_target=None, lastmod_target=None):
     """
     Check if a file is up-to-date by comparing the last modified timestamps
     (just like make does it).
 
     :param path_sources: list of full paths to the source files
     :param path_target: full path to the target file
```

### Comparing `pmbootstrap-1.9.0/pmb/helpers/package.py` & `pmbootstrap-2.0.0/pmb/helpers/package.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,52 @@
-#!/usr/bin/env python3
-
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 """
-Functions that work on both pmaports and (binary package) repos. See also:
-- pmb/helpers/pmaports.py (work on pmaports)
-- pmb/helpers/repo.py (work on binary package repos)
+Functions that work with both pmaports and binary package repos. See also:
+- pmb/helpers/pmaports.py (work with pmaports)
+- pmb/helpers/repo.py (work with binary package repos)
 """
-
 import copy
+import logging
 
 import pmb.helpers.pmaports
 import pmb.helpers.repo
 
 
-def get(args, pkgname, arch, replace_subpkgnames=False):
+def get(args, pkgname, arch, replace_subpkgnames=False, must_exist=True):
     """ Find a package in pmaports, and as fallback in the APKINDEXes of the
         binary packages.
         :param pkgname: package name (e.g. "hello-world")
         :param arch: preferred architecture of the binary package. When it
                      can't be found for this arch, we'll still look for another
                      arch to see whether the package exists at all. So make
                      sure to check the returned arch against what you wanted
                      with check_arch(). Example: "armhf"
         :param replace_subpkgnames: replace all subpkgnames with their main
                                     pkgnames in the depends (see #1733)
-        :returns: data from the parsed APKBUILD or APKINDEX in the following
-                  format: {"arch": ["noarch"],
-                           "depends": ["busybox-extras", "lddtree", ...],
-                           "pkgname": "postmarketos-mkinitfs",
-                           "provides": ["mkinitfs=0..1"],
-                           "version": "0.0.4-r10"} """
+        :param must_exist: raise an exception, if not found
+        :returns: * data from the parsed APKBUILD or APKINDEX in the following
+                    format: {"arch": ["noarch"],
+                             "depends": ["busybox-extras", "lddtree", ...],
+                             "pkgname": "postmarketos-mkinitfs",
+                             "provides": ["mkinitfs=0..1"],
+                             "version": "0.0.4-r10"}
+                  * None if the package was not found """
     # Cached result
     cache_key = "pmb.helpers.package.get"
-    if (arch in args.cache[cache_key] and
-            pkgname in args.cache[cache_key][arch] and
-            replace_subpkgnames in args.cache[cache_key][arch][pkgname]):
-        return args.cache[cache_key][arch][pkgname][replace_subpkgnames]
+    if (
+        arch in pmb.helpers.other.cache[cache_key] and
+        pkgname in pmb.helpers.other.cache[cache_key][arch] and
+        replace_subpkgnames in pmb.helpers.other.cache[cache_key][arch][
+            pkgname
+        ]
+    ):
+        return pmb.helpers.other.cache[cache_key][arch][pkgname][
+            replace_subpkgnames
+        ]
 
     # Find in pmaports
     ret = None
     pmaport = pmb.helpers.pmaports.get(args, pkgname, False)
     if pmaport:
         ret = {"arch": pmaport["arch"],
                "depends": pmb.build._package.get_depends(args, pmaport),
@@ -94,45 +83,57 @@
     if ret and isinstance(ret["arch"], str):
         ret["arch"] = [ret["arch"]]
 
     # Replace subpkgnames if desired
     if replace_subpkgnames:
         depends_new = []
         for depend in ret["depends"]:
-            depend = get(args, depend, arch)["pkgname"]
-            if depend not in depends_new:
-                depends_new += [depend]
+            depend_data = get(args, depend, arch, must_exist=False)
+            if not depend_data:
+                logging.warning(f"WARNING: {pkgname}: failed to resolve"
+                                f" dependency '{depend}'")
+                # Can't replace potential subpkgname
+                if depend not in depends_new:
+                    depends_new += [depend]
+                continue
+            depend_pkgname = depend_data["pkgname"]
+            if depend_pkgname not in depends_new:
+                depends_new += [depend_pkgname]
         ret["depends"] = depends_new
 
     # Save to cache and return
     if ret:
-        if arch not in args.cache[cache_key]:
-            args.cache[cache_key][arch] = {}
-        if pkgname not in args.cache[cache_key][arch]:
-            args.cache[cache_key][arch][pkgname] = {}
-        args.cache[cache_key][arch][pkgname][replace_subpkgnames] = ret
+        if arch not in pmb.helpers.other.cache[cache_key]:
+            pmb.helpers.other.cache[cache_key][arch] = {}
+        if pkgname not in pmb.helpers.other.cache[cache_key][arch]:
+            pmb.helpers.other.cache[cache_key][arch][pkgname] = {}
+        pmb.helpers.other.cache[cache_key][arch][pkgname][
+            replace_subpkgnames
+        ] = ret
         return ret
 
     # Could not find the package
+    if not must_exist:
+        return None
     raise RuntimeError("Package '" + pkgname + "': Could not find aport, and"
                        " could not find this package in any APKINDEX!")
 
 
 def depends_recurse(args, pkgname, arch):
     """ Recursively resolve all of the package's dependencies.
         :param pkgname: name of the package (e.g. "device-samsung-i9100")
         :param arch: preferred architecture for binary packages
         :returns: a list of pkgname_start and all its dependencies, e.g:
                   ["busybox-static-armhf", "device-samsung-i9100",
                    "linux-samsung-i9100", ...] """
     # Cached result
     cache_key = "pmb.helpers.package.depends_recurse"
-    if (arch in args.cache[cache_key] and
-            pkgname in args.cache[cache_key][arch]):
-        return args.cache[cache_key][arch][pkgname]
+    if (arch in pmb.helpers.other.cache[cache_key] and
+            pkgname in pmb.helpers.other.cache[cache_key][arch]):
+        return pmb.helpers.other.cache[cache_key][arch][pkgname]
 
     # Build ret (by iterating over the queue)
     queue = [pkgname]
     ret = []
     while len(queue):
         pkgname_queue = queue.pop()
         package = get(args, pkgname_queue, arch)
@@ -144,17 +145,17 @@
 
         # Add the pkgname (not possible subpkgname) to ret
         if package["pkgname"] not in ret:
             ret += [package["pkgname"]]
     ret.sort()
 
     # Save to cache and return
-    if arch not in args.cache[cache_key]:
-        args.cache[cache_key][arch] = {}
-    args.cache[cache_key][arch][pkgname] = ret
+    if arch not in pmb.helpers.other.cache[cache_key]:
+        pmb.helpers.other.cache[cache_key][arch] = {}
+    pmb.helpers.other.cache[cache_key][arch][pkgname] = ret
     return ret
 
 
 def check_arch(args, pkgname, arch, binary=True):
     """ Can a package be built for a certain architecture, or is there a binary
         package for it?
```

### Comparing `pmbootstrap-1.9.0/pmb/helpers/repo_missing.py` & `pmbootstrap-2.0.0/pmb/helpers/repo_missing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 
 import pmb.build
 import pmb.helpers.package
 import pmb.helpers.pmaports
```

### Comparing `pmbootstrap-1.9.0/pmb/helpers/http.py` & `pmbootstrap-2.0.0/pmb/helpers/http.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,27 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import os
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import hashlib
-import shutil
+import json
 import logging
+import os
+import shutil
 import urllib.request
+
 import pmb.helpers.run
 
 
 def download(args, url, prefix, cache=True, loglevel=logging.INFO,
              allow_404=False):
     """ Download a file to disk.
 
         :param url: the http(s) address of to the file to download
         :param prefix: for the cache, to make it easier to find (cache files
                        get a hash of the URL after the prefix)
+        :param cache: if True, and url is cached, do not download it again
         :param loglevel: change to logging.DEBUG to only display the download
                          message in 'pmbootstrap log', not in stdout. We use
                          this when downloading many APKINDEX files at once, no
                          point in showing a dozen messages.
         :param allow_404: do not raise an exception when the server responds
                           with a 404 Not Found error. Only display a warning on
                           stdout (no matter if loglevel is changed).
@@ -48,14 +35,19 @@
     path = (args.work + "/cache_http/" + prefix + "_" +
             hashlib.sha256(url.encode("utf-8")).hexdigest())
     if os.path.exists(path):
         if cache:
             return path
         pmb.helpers.run.user(args, ["rm", path])
 
+    # Offline and not cached
+    if args.offline:
+        raise RuntimeError("File not found in cache and offline flag is"
+                           f" enabled: {url}")
+
     # Download the file
     logging.log(loglevel, "Download " + url)
     try:
         with urllib.request.urlopen(url) as response:
             with open(path, "wb") as handle:
                 shutil.copyfileobj(response, handle)
     # Handle 404
@@ -63,7 +55,40 @@
         if e.code == 404 and allow_404:
             logging.warning("WARNING: file not found: " + url)
             return None
         raise
 
     # Return path in cache
     return path
+
+
+def retrieve(url, headers=None, allow_404=False):
+    """ Fetch the content of a URL and returns it as string.
+
+        :param url: the http(s) address of to the resource to fetch
+        :param headers: dict of HTTP headers to use
+        :param allow_404: do not raise an exception when the server responds
+                          with a 404 Not Found error. Only display a warning
+        :returns: str with the content of the response
+    """
+    # Download the file
+    logging.verbose("Retrieving " + url)
+
+    if headers is None:
+        headers = {}
+
+    req = urllib.request.Request(url, headers=headers)
+    try:
+        with urllib.request.urlopen(req) as response:
+            return response.read()
+    # Handle 404
+    except urllib.error.HTTPError as e:
+        if e.code == 404 and allow_404:
+            logging.warning("WARNING: failed to retrieve content from: " + url)
+            return None
+        raise
+
+
+def retrieve_json(*args, **kwargs):
+    """ Fetch the contents of a URL, parse it as JSON and return it. See
+        retrieve() for the list of all parameters. """
+    return json.loads(retrieve(*args, **kwargs))
```

### Comparing `pmbootstrap-1.9.0/pmb/helpers/logging.py` & `pmbootstrap-2.0.0/pmb/helpers/logging.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,15 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 import os
 import sys
+import pmb.config
+
+logfd = None
 
 
 class log_handler(logging.StreamHandler):
     """
     Write to stdout and to the already opened log file.
     """
     _args = None
@@ -32,22 +19,48 @@
             msg = self.format(record)
 
             # INFO or higher: Write to stdout
             if (not self._args.details_to_stdout and
                 not self._args.quiet and
                     record.levelno >= logging.INFO):
                 stream = self.stream
-                stream.write(msg)
+
+                styles = pmb.config.styles
+
+                msg_col = (
+                    msg.replace(
+                        "NOTE:",
+                        f"{styles['BLUE']}NOTE:{styles['END']}",
+                        1,
+                    )
+                    .replace(
+                        "WARNING:",
+                        f"{styles['YELLOW']}WARNING:{styles['END']}",
+                        1,
+                    )
+                    .replace(
+                        "ERROR:",
+                        f"{styles['RED']}ERROR:{styles['END']}",
+                        1,
+                    )
+                    .replace(
+                        "DONE!",
+                        f"{styles['GREEN']}DONE!{styles['END']}",
+                        1,
+                    )
+                )
+
+                stream.write(msg_col)
                 stream.write(self.terminator)
                 self.flush()
 
             # Everything: Write to logfd
             msg = "(" + str(os.getpid()).zfill(6) + ") " + msg
-            self._args.logfd.write(msg + "\n")
-            self._args.logfd.flush()
+            logfd.write(msg + "\n")
+            logfd.flush()
 
         except (KeyboardInterrupt, SystemExit):
             raise
         except BaseException:
             self.handleError(record)
 
 
@@ -61,37 +74,39 @@
     All stackoverflow user contributions are licensed as CC-BY-SA:
     https://creativecommons.org/licenses/by-sa/3.0/
     """
     logging.VERBOSE = 5
     logging.addLevelName(logging.VERBOSE, "VERBOSE")
     logging.Logger.verbose = lambda inst, msg, * \
         args, **kwargs: inst.log(logging.VERBOSE, msg, *args, **kwargs)
-    logging.verbose = lambda msg, *args, **kwargs: logging.log(logging.VERBOSE, msg,
-                                                               *args, **kwargs)
+    logging.verbose = lambda msg, *args, **kwargs: logging.log(logging.VERBOSE,
+                                                               msg, *args,
+                                                               **kwargs)
 
 
 def init(args):
     """
-    Set log format and add the log file descriptor to args.logfd, add the
+    Set log format and add the log file descriptor to logfd, add the
     verbose log level.
     """
+    global logfd
     # Set log file descriptor (logfd)
     if args.details_to_stdout:
-        setattr(args, "logfd", sys.stdout)
+        logfd = sys.stdout
     else:
         # Require containing directory to exist (so we don't create the work
         # folder and break the folder migration logic, which needs to set the
         # version upon creation)
         dir = os.path.dirname(args.log)
         if os.path.exists(dir):
-            setattr(args, "logfd", open(args.log, "a+"))
+            logfd = open(args.log, "a+")
         else:
-            setattr(args, "logfd", open(os.devnull, "a+"))
+            logfd = open(os.devnull, "a+")
             if args.action != "init":
-                print("WARNING: Can't create log file in '" + dir + "', path"
+                print(f"WARNING: Can't create log file in '{dir}', path"
                       " does not exist!")
 
     # Set log format
     root_logger = logging.getLogger()
     root_logger.handlers = []
     formatter = logging.Formatter("[%(asctime)s] %(message)s",
                                   datefmt="%H:%M:%S")
```

### Comparing `pmbootstrap-1.9.0/pmb/helpers/mount.py` & `pmbootstrap-2.0.0/pmb/helpers/mount.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,16 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import os
 import pmb.helpers.run
 
 
 def ismount(folder):
     """
-    Ismount() implementation, that works for mount --bind.
+    Ismount() implementation that works for mount --bind.
     Workaround for: https://bugs.python.org/issue29707
     """
     folder = os.path.realpath(os.path.realpath(folder))
     with open("/proc/mounts", "r") as handle:
         for line in handle:
             words = line.split()
             if len(words) >= 2 and words[1] == folder:
@@ -57,42 +41,47 @@
         else:
             raise RuntimeError("Mount failed, folder does not exist: " +
                                path)
 
     # Actually mount the folder
     pmb.helpers.run.root(args, ["mount", "--bind", source, destination])
 
-    # Verify, that it has worked
+    # Verify that it has worked
     if not ismount(destination):
         raise RuntimeError("Mount failed: " + source + " -> " + destination)
 
 
-def bind_blockdevice(args, source, destination):
+def bind_file(args, source, destination, create_folders=False):
     """
-    Mount a blockdevice with the --bind option, and create the destination
-    file, if necessary.
+    Mount a file with the --bind option, and create the destination file,
+    if necessary.
     """
     # Skip existing mountpoint
     if ismount(destination):
         return
 
     # Create empty file
     if not os.path.exists(destination):
+        if create_folders:
+            dir = os.path.dirname(destination)
+            if not os.path.isdir(dir):
+                pmb.helpers.run.root(args, ["mkdir", "-p", dir])
+
         pmb.helpers.run.root(args, ["touch", destination])
 
     # Mount
     pmb.helpers.run.root(args, ["mount", "--bind", source,
                                 destination])
 
 
 def umount_all_list(prefix, source="/proc/mounts"):
     """
     Parses `/proc/mounts` for all folders beginning with a prefix.
     :source: can be changed for testcases
-    :returns: a list of folders, that need to be umounted
+    :returns: a list of folders that need to be umounted
     """
     ret = []
     prefix = os.path.realpath(prefix)
     with open(source, "r") as handle:
         for line in handle:
             words = line.split()
             if len(words) < 2:
@@ -107,13 +96,13 @@
                 ret.append(mountpoint)
     ret.sort(reverse=True)
     return ret
 
 
 def umount_all(args, folder):
     """
-    Umount all folders, that are mounted inside a given folder.
+    Umount all folders that are mounted inside a given folder.
     """
     for mountpoint in umount_all_list(folder):
         pmb.helpers.run.root(args, ["umount", mountpoint])
         if ismount(mountpoint):
             raise RuntimeError("Failed to umount: " + mountpoint)
```

### Comparing `pmbootstrap-1.9.0/pmb/helpers/repo.py` & `pmbootstrap-2.0.0/pmb/helpers/repo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,25 @@
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 """
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
+Functions that work with binary package repos. See also:
+- pmb/helpers/pmaports.py (work with pmaports)
+- pmb/helpers/package.py (work with both)
 """
-
-"""
-Functions that work on both (binary package) repos. See also:
-- pmb/helpers/pmaports.py (work on pmaports)
-- pmb/helpers/package.py (work on both)
-"""
-
 import os
 import hashlib
 import logging
+import pmb.config.pmaports
 import pmb.helpers.http
 import pmb.helpers.run
 
 
 def hash(url, length=8):
     """
-    Generate the hash, that APK adds to the APKINDEX and apk packages
+    Generate the hash that APK adds to the APKINDEX and apk packages
     in its apk cache folder. It is the "12345678" part in this example:
     "APKINDEX.12345678.tar.gz".
 
     :param length: The length of the hash in the output file.
 
     See also: official implementation in apk-tools:
     <https://git.alpinelinux.org/cgit/apk-tools/>
@@ -53,58 +36,80 @@
     for i in range(csum_bytes):
         ret += xd[(binary[i] >> 4) & 0xf]
         ret += xd[binary[i] & 0xf]
 
     return ret
 
 
-def urls(args, user_repository=True, postmarketos_mirror=True):
+def urls(args, user_repository=True, postmarketos_mirror=True, alpine=True):
     """
     Get a list of repository URLs, as they are in /etc/apk/repositories.
+    :param user_repository: add /mnt/pmbootstrap-packages
+    :param postmarketos_mirror: add postmarketos mirror URLs
+    :param alpine: add alpine mirror URLs
+    :returns: list of mirror strings, like ["/mnt/pmbootstrap-packages",
+                                            "http://...", ...]
     """
     ret = []
+
+    # Get mirrordirs from channels.cfg (postmarketOS mirrordir is the same as
+    # the pmaports branch of the channel, no need to make it more complicated)
+    channel_cfg = pmb.config.pmaports.read_config_channel(args)
+    mirrordir_pmos = channel_cfg["branch_pmaports"]
+    mirrordir_alpine = channel_cfg["mirrordir_alpine"]
+
     # Local user repository (for packages compiled with pmbootstrap)
     if user_repository:
         ret.append("/mnt/pmbootstrap-packages")
 
     # Upstream postmarketOS binary repository
     if postmarketos_mirror:
         for mirror in args.mirrors_postmarketos:
-            ret.append(mirror)
+            # Remove "master" mirrordir to avoid breakage until bpo is adjusted
+            # (build.postmarketos.org#63) and to give potential other users of
+            # this flag a heads up.
+            if mirror.endswith("/master"):
+                logging.warning("WARNING: 'master' at the end of"
+                                " --mirror-pmOS is deprecated, the branch gets"
+                                " added automatically now!")
+                mirror = mirror[:-1 * len("master")]
+            ret.append(f"{mirror}{mirrordir_pmos}")
 
     # Upstream Alpine Linux repositories
-    directories = ["main", "community"]
-    if args.alpine_version == "edge":
-        directories.append("testing")
-    for dir in directories:
-        ret.append(args.mirror_alpine + args.alpine_version + "/" + dir)
+    if alpine:
+        directories = ["main", "community"]
+        if mirrordir_alpine == "edge":
+            directories.append("testing")
+        for dir in directories:
+            ret.append(f"{args.mirror_alpine}{mirrordir_alpine}/{dir}")
     return ret
 
 
-def apkindex_files(args, arch=None):
+def apkindex_files(args, arch=None, user_repository=True, pmos=True,
+                   alpine=True):
     """
     Get a list of outside paths to all resolved APKINDEX.tar.gz files for a
     specific arch.
     :param arch: defaults to native
+    :param user_repository: add path to index of locally built packages
+    :param pmos: add paths to indexes of postmarketos mirrors
+    :param alpine: add paths to indexes of alpine mirrors
+    :returns: list of absolute APKINDEX.tar.gz file paths
     """
     if not arch:
-        arch = args.arch_native
+        arch = pmb.config.arch_native
 
+    ret = []
     # Local user repository (for packages compiled with pmbootstrap)
-    ret = [args.work + "/packages/" + arch + "/APKINDEX.tar.gz"]
-
-    # Upstream postmarketOS binary repository
-    urls_todo = []
-    for mirror in args.mirrors_postmarketos:
-        if mirror:
-            urls_todo.append(mirror)
+    if user_repository:
+        channel = pmb.config.pmaports.read_config(args)["channel"]
+        ret = [f"{args.work}/packages/{channel}/{arch}/APKINDEX.tar.gz"]
 
     # Resolve the APKINDEX.$HASH.tar.gz files
-    urls_todo += urls(args, False, False)
-    for url in urls_todo:
+    for url in urls(args, False, pmos, alpine):
         ret.append(args.work + "/cache_apk_" + arch + "/APKINDEX." +
                    hash(url) + ".tar.gz")
 
     return ret
 
 
 def update(args, arch=None, force=False, existing_only=False):
@@ -118,17 +123,17 @@
                           this is used by "pmbootstrap update"
 
     :returns: True when files have been downloaded, False otherwise
     """
     # Skip in offline mode, only show once
     cache_key = "pmb.helpers.repo.update"
     if args.offline:
-        if not args.cache[cache_key]["offline_msg_shown"]:
+        if not pmb.helpers.other.cache[cache_key]["offline_msg_shown"]:
             logging.info("NOTE: skipping package index update (offline mode)")
-            args.cache[cache_key]["offline_msg_shown"] = True
+            pmb.helpers.other.cache[cache_key]["offline_msg_shown"] = True
         return False
 
     # Architectures and retention time
     architectures = [arch] if arch else pmb.config.build_device_architectures
     retention_hours = pmb.config.apkindex_retention_time
     retention_seconds = retention_hours * 3600
 
@@ -142,15 +147,15 @@
             # APKINDEX file name from the URL
             url_full = url + "/" + arch + "/APKINDEX.tar.gz"
             cache_apk_outside = args.work + "/cache_apk_" + arch
             apkindex = cache_apk_outside + "/APKINDEX." + hash(url) + ".tar.gz"
 
             # Find update reason, possibly skip non-existing or known 404 files
             reason = None
-            if url_full in args.cache[cache_key]["404"]:
+            if url_full in pmb.helpers.other.cache[cache_key]["404"]:
                 # We already attempted to download this file once in this
                 # session
                 continue
             elif not os.path.exists(apkindex):
                 if existing_only:
                     continue
                 reason = "file does not exist yet"
@@ -170,24 +175,26 @@
     # Bail out or show log message
     if not len(outdated):
         return False
     logging.info("Update package index for " + ", ".join(outdated_arches) +
                  " (" + str(len(outdated)) + " file(s))")
 
     # Download and move to right location
-    for url, target in outdated.items():
+    for (i, (url, target)) in enumerate(outdated.items()):
+        pmb.helpers.cli.progress_print(args, i / len(outdated))
         temp = pmb.helpers.http.download(args, url, "APKINDEX", False,
                                          logging.DEBUG, True)
         if not temp:
-            args.cache[cache_key]["404"].append(url)
+            pmb.helpers.other.cache[cache_key]["404"].append(url)
             continue
         target_folder = os.path.dirname(target)
         if not os.path.exists(target_folder):
             pmb.helpers.run.root(args, ["mkdir", "-p", target_folder])
         pmb.helpers.run.root(args, ["cp", temp, target])
+    pmb.helpers.cli.progress_flush(args)
 
     return True
 
 
 def alpine_apkindex_path(args, repo="main", arch=None):
     """
     Get the path to a specific Alpine APKINDEX file on disk and download it if
@@ -198,14 +205,15 @@
     :returns: full path to the APKINDEX file
     """
     # Repo sanity check
     if repo not in ["main", "community", "testing", "non-free"]:
         raise RuntimeError("Invalid Alpine repository: " + repo)
 
     # Download the file
-    arch = arch or args.arch_native
+    arch = arch or pmb.config.arch_native
     update(args, arch)
 
     # Find it on disk
-    repo_link = args.mirror_alpine + args.alpine_version + "/" + repo
+    channel_cfg = pmb.config.pmaports.read_config_channel(args)
+    repo_link = f"{args.mirror_alpine}{channel_cfg['mirrordir_alpine']}/{repo}"
     cache_folder = args.work + "/cache_apk_" + arch
     return cache_folder + "/APKINDEX." + hash(repo_link) + ".tar.gz"
```

### Comparing `pmbootstrap-1.9.0/pmb/helpers/args.py` & `pmbootstrap-2.0.0/pmb/helpers/args.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,13 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import copy
 import os
 import pmb.config
+import pmb.helpers.git
 
 """ This file constructs the args variable, which is passed to almost all
     functions in the pmbootstrap code base. Here's a listing of the kind of
     information it stores.
 
     1. Argparse
        Variables directly from command line argument parsing (see
@@ -31,58 +16,34 @@
 
        Examples:
        args.action ("zap", "chroot", "build" etc.)
        args.as_root (True when --as-root is passed)
        ...
 
     2. Argparse merged with others
-       Variables from the user's config file (~/.config/pmbootstrap.cfg), that
+       Variables from the user's config file (~/.config/pmbootstrap.cfg) that
        can be overridden from the command line (pmb/parse/arguments.py) and
        fall back to the defaults defined in pmb/config/__init__.py (see
        "defaults = {..."). The user's config file gets generated interactively
         with "pmbootstrap init".
 
        Examples:
        args.aports ("$WORK/cache_git/pmaports", override with --aports)
        args.device ("samsung-i9100", "qemu-amd64" etc.)
        args.work ("/home/user/.local/var/pmbootstrap", override with --work)
 
-    3. Shortcuts
-       Long variables or function calls that always return the same information
-       may have a shortcut defined, to make the code more readable (see
-       add_shortcuts() below).
-
-       Example:
-       args.arch_native ("x86_64" etc.)
-
-    4. Cache
-       pmbootstrap uses this dictionary to save the result of expensive
-       results, so they work a lot faster the next time they are needed in the
-       same session. Usually the cache is written to and read from in the same
-       Python file, with code similar to the following:
-
-       def lookup(args, key):
-           if key in args.cache["mycache"]:
-               return args.cache["mycache"][key]
-           ret = expensive_operation(args, key)
-           args.cache["mycache"][key] = ret
-           return ret
-
-       See add_cache() below for details.
-
-    5. Parsed configs
+    3. Parsed configs
        Similar to the cache above, specific config files get parsed and added
        to args, so they can get accessed quickly (without parsing the configs
        over and over). These configs are not only used in one specific
        location, so having a short name for them increases readability of the
        code as well.
 
        Examples:
        args.deviceinfo (e.g. {"name": "Mydevice", "arch": "armhf", ...})
-       args.pmaports (e.g. {"version": "1", "branch_alpine": "edge", ...})
 """
 
 
 def fix_mirrors_postmarketos(args):
     """ Fix args.mirrors_postmarketos when it is supposed to be empty or the
         default value.
 
@@ -91,15 +52,17 @@
         specify multiple custom mirrors by specifying -mp multiple times on the
         command line. Here we fix the default and no mirrors case.
 
         NOTE: we don't use nargs="+", because it does not play nicely with
         subparsers: <https://bugs.python.org/issue9338> """
     # -mp not specified: use default mirrors
     if not args.mirrors_postmarketos:
-        args.mirrors_postmarketos = pmb.config.defaults["mirrors_postmarketos"]
+        cfg = pmb.config.load(args)
+        args.mirrors_postmarketos = \
+            cfg["pmbootstrap"]["mirrors_postmarketos"].split(",")
 
     # -mp="": use no postmarketOS mirrors (build everything locally)
     if args.mirrors_postmarketos == [""]:
         args.mirrors_postmarketos = []
 
 
 def check_pmaports_path(args):
@@ -126,74 +89,53 @@
 
     # Replace ~ (path variables only)
     for key in ["aports", "config", "log", "work"]:
         if key in args:
             setattr(args, key, os.path.expanduser(getattr(args, key)))
 
 
-def add_shortcuts(args):
-    """ Add convenience shortcuts """
-    setattr(args, "arch_native", pmb.parse.arch.alpine_native())
-
-
-def add_cache(args):
-    """ Add a caching dict (caches parsing of files etc. for the current
-        session) """
-    repo_update = {"404": [], "offline_msg_shown": False}
-    setattr(args, "cache", {"apkindex": {},
-                            "apkbuild": {},
-                            "apk_min_version_checked": [],
-                            "apk_repository_list_updated": [],
-                            "built": {},
-                            "find_aport": {},
-                            "pmb.helpers.package.depends_recurse": {},
-                            "pmb.helpers.package.get": {},
-                            "pmb.helpers.repo.update": repo_update})
-
-
 def add_deviceinfo(args):
     """ Add and verify the deviceinfo (only after initialization) """
     setattr(args, "deviceinfo", pmb.parse.deviceinfo(args))
     arch = args.deviceinfo["arch"]
-    if (arch != args.arch_native and
+    if (arch != pmb.config.arch_native and
             arch not in pmb.config.build_device_architectures):
         raise ValueError("Arch '" + arch + "' is not available in"
                          " postmarketOS. If you would like to add it, see:"
                          " <https://postmarketos.org/newarch>")
 
 
 def init(args):
     # Basic initialization
     fix_mirrors_postmarketos(args)
     pmb.config.merge_with_args(args)
     replace_placeholders(args)
-    add_shortcuts(args)
-    add_cache(args)
+    pmb.helpers.other.init_cache()
 
     # Initialize logs (we could raise errors below)
     pmb.helpers.logging.init(args)
 
     # Initialization code which may raise errors
     check_pmaports_path(args)
     if args.action not in ["init", "config", "bootimg_analyze", "log",
-                           "shutdown", "zap"]:
-        pmb.config.pmaports.read_config_into_args(args)
+                           "pull", "shutdown", "zap"]:
+        pmb.config.pmaports.read_config(args)
         add_deviceinfo(args)
+        pmb.helpers.git.parse_channels_cfg(args)
+
     return args
 
 
 def update_work(args, work):
     """ Update the work path in args.work and wherever $WORK was used. """
     # Start with the unmodified args from argparse
     args_new = copy.deepcopy(args.from_argparse)
 
     # Keep from the modified args:
-    # * the old log file descriptor (so we can close it)
     # * the unmodified args from argparse (to check if --aports was specified)
-    args_new.logfd = args.logfd
     args_new.from_argparse = args.from_argparse
 
     # Generate modified args again, replacing $WORK with the new work folder
     # When args.log is different, this also opens the log in the new location
     args_new.work = work
     args_new = pmb.helpers.args.init(args_new)
```

### Comparing `pmbootstrap-1.9.0/pmb/helpers/pkgrel_bump.py` & `pmbootstrap-2.0.0/pmb/helpers/pkgrel_bump.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,10 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
-import os
 
 import pmb.helpers.file
 import pmb.helpers.pmaports
 import pmb.helpers.repo
 import pmb.parse
 
 
@@ -31,15 +14,15 @@
 
     :param pkgname: name of the package
     :param reason: string to display as reason why it was increased
     :param dry: don't modify the APKBUILD, just print the message
     """
     # Current and new pkgrel
     path = pmb.helpers.pmaports.find(args, pkgname) + "/APKBUILD"
-    apkbuild = pmb.parse.apkbuild(args, path)
+    apkbuild = pmb.parse.apkbuild(path)
     pkgrel = int(apkbuild["pkgrel"])
     pkgrel_new = pkgrel + 1
 
     # Display the message, bail out in dry mode
     logging.info("Increase '" + pkgname + "' pkgrel (" + str(pkgrel) + " -> " +
                  str(pkgrel_new) + ")" + reason)
     if dry:
@@ -47,46 +30,23 @@
 
     # Increase
     old = "\npkgrel=" + str(pkgrel) + "\n"
     new = "\npkgrel=" + str(pkgrel_new) + "\n"
     pmb.helpers.file.replace(path, old, new)
 
     # Verify
-    del(args.cache["apkbuild"][path])
-    apkbuild = pmb.parse.apkbuild(args, path)
+    del pmb.helpers.other.cache["apkbuild"][path]
+    apkbuild = pmb.parse.apkbuild(path)
     if int(apkbuild["pkgrel"]) != pkgrel_new:
         raise RuntimeError("Failed to bump pkgrel for package '" + pkgname +
                            "'. Make sure that there's a line with exactly the"
                            " string '" + old + "' and nothing else in: " +
                            path)
 
 
-def auto_apkindex_files(args):
-    """
-    Get the paths to the APKINDEX files, that need to be analyzed, sorted by
-    arch. Relevant are the local pmbootstrap generated APKINDEX as well as the
-    APKINDEX from the pmOS binary repo.
-
-    :returns: {"armhf": "...../APKINDEX.tar.gz", ...}
-    """
-    pmb.helpers.repo.update(args)
-    ret = {}
-    for arch in pmb.config.build_device_architectures:
-        ret[arch] = []
-        local = args.work + "/packages/" + arch + "/APKINDEX.tar.gz"
-        if os.path.exists(local):
-            ret[arch].append(local)
-
-        for mirror in args.mirrors_postmarketos:
-            path = (args.work + "/cache_apk_" + arch + "/APKINDEX." +
-                    pmb.helpers.repo.hash(mirror) + ".tar.gz")
-            ret[arch].append(path)
-    return ret
-
-
 def auto_apkindex_package(args, arch, aport, apk, dry=False):
     """
     Bump the pkgrel of a specific package if it is outdated in the given
     APKINDEX.
 
     :param arch: the architecture, e.g. "armhf"
     :param aport: parsed APKBUILD of the binary package's origin:
@@ -117,14 +77,18 @@
 
     # Find missing depends
     depends = apk["depends"]
     logging.verbose("{}: checking depends: {}".format(pkgname,
                                                       ", ".join(depends)))
     missing = []
     for depend in depends:
+        if depend.startswith("!"):
+            # Ignore conflict-dependencies
+            continue
+
         providers = pmb.parse.apkindex.providers(args, depend, arch,
                                                  must_exist=False)
         if providers == {}:
             # We're only interested in missing depends starting with "so:"
             # (which means dynamic libraries that the package was linked
             # against) and packages for which no aport exists.
             if (depend.startswith("so:") or
@@ -139,27 +103,28 @@
 
 
 def auto(args, dry=False):
     """
     :returns: list of aport names, where the pkgrel needed to be changed
     """
     ret = []
-    for arch, paths in auto_apkindex_files(args).items():
+    for arch in pmb.config.build_device_architectures:
+        paths = pmb.helpers.repo.apkindex_files(args, arch, alpine=False)
         for path in paths:
             logging.info("scan " + path)
-            index = pmb.parse.apkindex.parse(args, path, False)
+            index = pmb.parse.apkindex.parse(path, False)
             for pkgname, apk in index.items():
                 origin = apk["origin"]
                 # Only increase once!
                 if origin in ret:
-                    logging.verbose("{}: origin '{}' found again".format(pkgname,
-                                                                         origin))
+                    logging.verbose(
+                        f"{pkgname}: origin '{origin}' found again")
                     continue
                 aport_path = pmb.helpers.pmaports.find(args, origin, False)
                 if not aport_path:
                     logging.warning("{}: origin '{}' aport not found".format(
                                     pkgname, origin))
                     continue
-                aport = pmb.parse.apkbuild(args, aport_path + "/APKBUILD")
+                aport = pmb.parse.apkbuild(f"{aport_path}/APKBUILD")
                 if auto_apkindex_package(args, arch, aport, apk, dry):
                     ret.append(pkgname)
     return ret
```

### Comparing `pmbootstrap-1.9.0/pmb/helpers/run_core.py` & `pmbootstrap-2.0.0/pmb/helpers/run_core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,92 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import fcntl
 import logging
+import os
 import selectors
+import shlex
 import subprocess
 import sys
+import threading
 import time
-import os
 import pmb.helpers.run
 
 """ For a detailed description of all output modes, read the description of
     core() at the bottom. All other functions in this file get (indirectly)
     called by core(). """
 
 
-def sanity_checks(output="log", output_return=False, check=None,
-                  kill_as_root=False):
+def flat_cmd(cmd, working_dir=None, env={}):
+    """
+    Convert a shell command passed as list into a flat shell string with
+    proper escaping.
+
+    :param cmd: command as list, e.g. ["echo", "string with spaces"]
+    :param working_dir: when set, prepend "cd ...;" to execute the command
+                        in the given working directory
+    :param env: dict of environment variables to be passed to the command, e.g.
+                {"JOBS": "5"}
+    :returns: the flat string, e.g.
+              echo 'string with spaces'
+              cd /home/pmos;echo 'string with spaces'
+    """
+    # Merge env and cmd into escaped list
+    escaped = []
+    for key, value in env.items():
+        escaped.append(key + "=" + shlex.quote(value))
+    for i in range(len(cmd)):
+        escaped.append(shlex.quote(cmd[i]))
+
+    # Prepend working dir
+    ret = " ".join(escaped)
+    if working_dir:
+        ret = "cd " + shlex.quote(working_dir) + ";" + ret
+
+    return ret
+
+
+def sanity_checks(output="log", output_return=False, check=None):
     """
     Raise an exception if the parameters passed to core() don't make sense
     (all parameters are described in core() below).
     """
-    if output not in ["log", "stdout", "interactive", "tui", "background"]:
+    vals = ["log", "stdout", "interactive", "tui", "background", "pipe"]
+    if output not in vals:
         raise RuntimeError("Invalid output value: " + str(output))
 
     # Prevent setting the check parameter with output="background".
     # The exit code won't be checked when running in background, so it would
     # always by check=False. But we prevent it from getting set to check=False
     # as well, so it does not look like you could change it to check=True.
     if check is not None and output == "background":
         raise RuntimeError("Can't use check with output: background")
 
     if output_return and output in ["tui", "background"]:
         raise RuntimeError("Can't use output_return with output: " + output)
 
-    if kill_as_root and output in ["interactive", "tui", "background"]:
-        raise RuntimeError("Can't use kill_as_root with output: " + output)
-
 
-def background(args, cmd, working_dir=None):
+def background(cmd, working_dir=None):
     """ Run a subprocess in background and redirect its output to the log. """
-    ret = subprocess.Popen(cmd, stdout=args.logfd, stderr=args.logfd,
-                           cwd=working_dir)
-    logging.debug("Started process in background with PID " + str(ret.pid))
+    ret = subprocess.Popen(cmd, stdout=pmb.helpers.logging.logfd,
+                           stderr=pmb.helpers.logging.logfd, cwd=working_dir)
+    logging.debug(f"New background process: pid={ret.pid}, output=background")
     return ret
 
 
-def pipe_read(args, process, output_to_stdout=False, output_return=False,
+def pipe(cmd, working_dir=None):
+    """ Run a subprocess in background and redirect its output to a pipe. """
+    ret = subprocess.Popen(cmd, stdout=subprocess.PIPE,
+                           stdin=subprocess.DEVNULL,
+                           stderr=pmb.helpers.logging.logfd, cwd=working_dir)
+    logging.verbose(f"New background process: pid={ret.pid}, output=pipe")
+    return ret
+
+
+def pipe_read(process, output_to_stdout=False, output_return=False,
               output_return_buffer=False):
     """
     Read all available output from a subprocess and copy it to the log and
     optionally stdout and a buffer variable. This is only meant to be called by
     foreground_pipe() below.
 
     :param process: subprocess.Popen instance
@@ -75,91 +96,92 @@
     :param output_return_buffer: list of bytes that gets extended with the
                                  current output in case output_return is True.
     """
     while True:
         # Copy available output
         out = process.stdout.readline()
         if len(out):
-            args.logfd.buffer.write(out)
+            pmb.helpers.logging.logfd.buffer.write(out)
             if output_to_stdout:
                 sys.stdout.buffer.write(out)
             if output_return:
                 output_return_buffer.append(out)
             continue
 
         # No more output (flush buffers)
-        args.logfd.flush()
+        pmb.helpers.logging.logfd.flush()
         if output_to_stdout:
             sys.stdout.flush()
         return
 
 
-def kill_process_tree(args, pid, ppids, kill_as_root):
+def kill_process_tree(args, pid, ppids, sudo):
     """
     Recursively kill a pid and its child processes
 
     :param pid: process id that will be killed
     :param ppids: list of process id and parent process id tuples (pid, ppid)
-    :param kill_as_root: use sudo to kill the process
+    :param sudo: use sudo to kill the process
     """
-    if kill_as_root:
+    if sudo:
         pmb.helpers.run.root(args, ["kill", "-9", str(pid)],
                              check=False)
     else:
         pmb.helpers.run.user(args, ["kill", "-9", str(pid)],
                              check=False)
 
     for (child_pid, child_ppid) in ppids:
         if child_ppid == str(pid):
-            kill_process_tree(args, child_pid, ppids, kill_as_root)
+            kill_process_tree(args, child_pid, ppids, sudo)
 
 
-def kill_command(args, pid, kill_as_root):
+def kill_command(args, pid, sudo):
     """
     Kill a command process and recursively kill its child processes
 
     :param pid: process id that will be killed
-    :param kill_as_root: use sudo to kill the process
+    :param sudo: use sudo to kill the process
     """
-    cmd = ["ps", "-e", "-o", "pid=,ppid=", "--noheaders"]
+    cmd = ["ps", "-e", "-o", "pid,ppid"]
     ret = subprocess.run(cmd, check=True, stdout=subprocess.PIPE)
     ppids = []
-    proc_entries = ret.stdout.decode("utf-8").rstrip().split('\n')
+    proc_entries = ret.stdout.decode("utf-8").rstrip().split('\n')[1:]
     for row in proc_entries:
         items = row.split()
         if len(items) != 2:
             raise RuntimeError("Unexpected ps output: " + row)
         ppids.append(items)
 
-    kill_process_tree(args, pid, ppids, kill_as_root)
+    kill_process_tree(args, pid, ppids, sudo)
 
 
 def foreground_pipe(args, cmd, working_dir=None, output_to_stdout=False,
                     output_return=False, output_timeout=True,
-                    kill_as_root=False):
+                    sudo=False, stdin=None):
     """
     Run a subprocess in foreground with redirected output and optionally kill
     it after being silent for too long.
 
     :param cmd: command as list, e.g. ["echo", "string with spaces"]
     :param working_dir: path in host system where the command should run
     :param output_to_stdout: copy all output to pmbootstrap's stdout
     :param output_return: return the output of the whole program
     :param output_timeout: kill the process when it doesn't print any output
                            after a certain time (configured with --timeout)
                            and raise a RuntimeError exception
-    :param kill_as_root: use sudo to kill the process when it hits the timeout
+    :param sudo: use sudo to kill the process when it hits the timeout
     :returns: (code, output)
               * code: return code of the program
               * output: ""
               * output: full program output string (output_return is True)
     """
     # Start process in background (stdout and stderr combined)
     process = subprocess.Popen(cmd, stdout=subprocess.PIPE,
-                               stderr=subprocess.STDOUT, cwd=working_dir)
+                               stderr=subprocess.STDOUT, cwd=working_dir,
+                               stdin=stdin)
 
     # Make process.stdout non-blocking
     handle = process.stdout.fileno()
     flags = fcntl.fcntl(handle, fcntl.F_GETFL)
     fcntl.fcntl(handle, fcntl.F_SETFL, flags | os.O_NONBLOCK)
 
     # While process exists wait for output (with timeout)
@@ -177,23 +199,23 @@
         if output_timeout:
             wait_end = time.perf_counter()
             if wait_end - wait_start >= args.timeout:
                 logging.info("Process did not write any output for " +
                              str(args.timeout) + " seconds. Killing it.")
                 logging.info("NOTE: The timeout can be increased with"
                              " 'pmbootstrap -t'.")
-                kill_command(args, process.pid, kill_as_root)
+                kill_command(args, process.pid, sudo)
                 continue
 
         # Read all currently available output
-        pipe_read(args, process, output_to_stdout, output_return,
+        pipe_read(process, output_to_stdout, output_return,
                   output_buffer)
 
     # There may still be output after the process quit
-    pipe_read(args, process, output_to_stdout, output_return, output_buffer)
+    pipe_read(process, output_to_stdout, output_return, output_buffer)
 
     # Return the return code and output (the output gets built as list of
     # output chunks and combined at the end, this is faster than extending the
     # combined string with each new chunk)
     return (process.returncode, b"".join(output_buffer).decode("utf-8"))
 
 
@@ -207,16 +229,63 @@
 
     logging.debug("*** output passed to pmbootstrap stdout, not to this log"
                   " ***")
     process = subprocess.Popen(cmd, cwd=working_dir)
     return process.wait()
 
 
+def check_return_code(args, code, log_message):
+    """
+    Check the return code of a command.
+
+    :param code: exit code to check
+    :param log_message: simplified and more readable form of the command, e.g.
+                        "(native) % echo test" instead of the full command with
+                        entering the chroot and more escaping
+    :raises RuntimeError: when the code indicates that the command failed
+    """
+
+    if code:
+        logging.debug("^" * 70)
+        logging.info("NOTE: The failed command's output is above the ^^^ line"
+                     " in the log file: " + args.log)
+        raise RuntimeError(f"Command failed (exit code {str(code)}): " +
+                           log_message)
+
+
+def sudo_timer_iterate():
+    """
+    Run sudo -v and schedule a new timer to repeat the same.
+    """
+
+    if pmb.config.which_sudo() == "sudo":
+        subprocess.Popen(["sudo", "-v"]).wait()
+    else:
+        subprocess.Popen(pmb.config.sudo(["true"])).wait()
+
+    timer = threading.Timer(interval=60, function=sudo_timer_iterate)
+    timer.daemon = True
+    timer.start()
+
+
+def sudo_timer_start():
+    """
+    Start a timer to call sudo -v periodically, so that the password is only
+    needed once.
+    """
+
+    if "sudo_timer_active" in pmb.helpers.other.cache:
+        return
+    pmb.helpers.other.cache["sudo_timer_active"] = True
+
+    sudo_timer_iterate()
+
+
 def core(args, log_message, cmd, working_dir=None, output="log",
-         output_return=False, check=None, kill_as_root=False):
+         output_return=False, check=None, sudo=False, disable_timeout=False):
     """
     Run a command and create a log entry.
 
     This is a low level function not meant to be used directly. Use one of the
     following instead: pmb.helpers.run.user(), pmb.helpers.run.root(),
                        pmb.chroot.user(), pmb.chroot.root()
 
@@ -227,78 +296,98 @@
     :param working_dir: path in host system where the command should run
     :param output: where to write the output (stdout and stderr) of the
                    process. We almost always write to the log file, which can
                    be read with "pmbootstrap log" (output values: "log",
                    "stdout", "interactive", "background"), so it's easy to
                    trace what pmbootstrap does.
 
-                   The exception is "tui" (text-based user interface), where
+                   The exceptions are "tui" (text-based user interface), where
                    it does not make sense to write to the log file (think of
-                   ncurses UIs, such as "menuconfig").
-
-                   When the output is not set to "interactive", "tui" or
-                   "background", we kill the process if it does not output
-                   anything for 5 minutes (time can be set with "pmbootstrap
-                   --timeout").
+                   ncurses UIs, such as "menuconfig") and "pipe" where the
+                   output is written to a pipe for manual asynchronous
+                   consumption by the caller.
+
+                   When the output is not set to "interactive", "tui",
+                   "background" or "pipe", we kill the process if it does not
+                   output anything for 5 minutes (time can be set with
+                   "pmbootstrap --timeout").
 
                    The table below shows all possible values along with
                    their properties. "wait" indicates that we wait for the
                    process to complete.
 
-                   output value  | timeout | out to log | out to stdout | wait
-                   -----------------------------------------------------------
-                   "log"         | x       | x          |               | x
-                   "stdout"      | x       | x          | x             | x
-                   "interactive" |         | x          | x             | x
-                   "tui"         |         |            | x             | x
-                   "background"  |         | x          |               |
+                   output value  | timeout | out to log | out to stdout | wait | pass stdin
+                   ------------------------------------------------------------------------
+                   "log"         | x       | x          |               | x    |
+                   "stdout"      | x       | x          | x             | x    |
+                   "interactive" |         | x          | x             | x    | x
+                   "tui"         |         |            | x             | x    | x
+                   "background"  |         | x          |               |      |
+                   "pipe"        |         |            |               |      |
 
     :param output_return: in addition to writing the program's output to the
                           destinations above in real time, write to a buffer
                           and return it as string when the command has
                           completed. This is not possible when output is
-                          "background" or "tui".
+                          "background", "pipe" or "tui".
     :param check: an exception will be raised when the command's return code
                   is not 0. Set this to False to disable the check. This
-                  parameter can not be used when the output is "background".
-    :param kill_as_root: use sudo to kill the process when it hits the timeout.
+                  parameter can not be used when the output is "background" or
+                  "pipe".
+    :param sudo: use sudo to kill the process when it hits the timeout.
     :returns: * program's return code (default)
-              * subprocess.Popen instance (output is "background")
+              * subprocess.Popen instance (output is "background" or "pipe")
               * the program's entire output (output_return is True)
     """
-    sanity_checks(output, output_return, check, kill_as_root)
+    sanity_checks(output, output_return, check)
+
+    # Preserve proxy environment variables
+    env = {}
+    for var in ["FTP_PROXY", "ftp_proxy", "HTTP_PROXY", "http_proxy",
+                "HTTPS_PROXY", "https_proxy", "HTTP_PROXY_AUTH"]:
+        if var in os.environ:
+            env[var] = os.environ[var]
+    if env:
+        cmd = ["sh", "-c", flat_cmd(cmd, env=env)]
+
+    if args.sudo_timer and sudo:
+        sudo_timer_start()
 
     # Log simplified and full command (pmbootstrap -v)
     logging.debug(log_message)
     logging.verbose("run: " + str(cmd))
 
     # Background
     if output == "background":
-        return background(args, cmd, working_dir)
+        return background(cmd, working_dir)
+
+    # Pipe
+    if output == "pipe":
+        return pipe(cmd, working_dir)
 
     # Foreground
     output_after_run = ""
     if output == "tui":
         # Foreground TUI
         code = foreground_tui(cmd, working_dir)
     else:
         # Foreground pipe (always redirects to the error log file)
         output_to_stdout = False
         if not args.details_to_stdout and output in ["stdout", "interactive"]:
             output_to_stdout = True
 
-        output_timeout = output in ["log", "stdout"]
+        output_timeout = output in ["log", "stdout"] and not disable_timeout
+
+        stdin = subprocess.DEVNULL if output in ["log", "stdout"] else None
+
         (code, output_after_run) = foreground_pipe(args, cmd, working_dir,
                                                    output_to_stdout,
                                                    output_return,
                                                    output_timeout,
-                                                   kill_as_root)
+                                                   sudo, stdin)
 
     # Check the return code
-    if code and check is not False:
-        logging.debug("^" * 70)
-        logging.info("NOTE: The failed command's output is above the ^^^ line"
-                     " in the log file: " + args.log)
-        raise RuntimeError("Command failed: " + log_message)
+    if check is not False:
+        check_return_code(args, code, log_message)
 
     # Return (code or output string)
     return output_after_run if output_return else code
```

### Comparing `pmbootstrap-1.9.0/pmb/helpers/devices.py` & `pmbootstrap-2.0.0/pmb/helpers/devices.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,69 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import os
 import glob
 import pmb.parse
 
 
-def list_codenames(args):
+def find_path(args, codename, file=''):
+    """
+    Find path to device APKBUILD under `device/*/device-`.
+    :param codename: device codename
+    :param file: file to look for (e.g. APKBUILD or deviceinfo), may be empty
+    :returns: path to APKBUILD
+    """
+    g = glob.glob(args.aports + "/device/*/device-" + codename + '/' + file)
+    if not g:
+        return None
+
+    if len(g) != 1:
+        raise RuntimeError(codename + " found multiple times in the device"
+                           " subdirectory of pmaports")
+
+    return g[0]
+
+
+def list_codenames(args, vendor=None, unmaintained=True):
     """
     Get all devices, for which aports are available
+    :param vendor: vendor name to choose devices from, or None for all vendors
+    :param unmaintained: include unmaintained devices
     :returns: ["first-device", "second-device", ...]
     """
     ret = []
-    for path in glob.glob(args.aports + "/device/device-*"):
+    for path in glob.glob(args.aports + "/device/*/device-*"):
+        if not unmaintained and '/unmaintained/' in path:
+            continue
         device = os.path.basename(path).split("-", 1)[1]
-        ret += [device]
+        if (vendor is None) or device.startswith(vendor + '-'):
+            ret.append(device)
+    return ret
+
+
+def list_vendors(args):
+    """
+    Get all device vendors, for which aports are available
+    :returns: {"vendor1", "vendor2", ...}
+    """
+    ret = set()
+    for path in glob.glob(args.aports + "/device/*/device-*"):
+        vendor = os.path.basename(path).split("-", 2)[1]
+        ret.add(vendor)
     return ret
 
 
 def list_apkbuilds(args):
     """
     :returns: { "first-device": {"pkgname": ..., "pkgver": ...}, ... }
     """
     ret = {}
     for device in list_codenames(args):
-        apkbuild_path = args.aports + "/device/device-" + device + "/APKBUILD"
-        ret[device] = pmb.parse.apkbuild(args, apkbuild_path)
+        apkbuild_path = f"{args.aports}/device/*/device-{device}/APKBUILD"
+        ret[device] = pmb.parse.apkbuild(apkbuild_path)
     return ret
 
 
 def list_deviceinfos(args):
     """
     :returns: { "first-device": {"name": ..., "screen_width": ...}, ... }
     """
```

### Comparing `pmbootstrap-1.9.0/pmb/build/autodetect.py` & `pmbootstrap-2.0.0/pmb/build/autodetect.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,9 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import fnmatch
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 import os
 
 import pmb.config
 import pmb.chroot.apk
 import pmb.helpers.pmaports
 import pmb.parse.arch
@@ -53,53 +36,60 @@
     """
     Find a good default in case the user did not specify for which architecture
     a package should be built.
 
     :returns: arch string like "x86_64" or "armhf". Preferred order, depending
               on what is supported by the APKBUILD:
               * native arch
-              * device arch
+              * device arch (this will be preferred instead if build_default_device_arch is true)
               * first arch in the APKBUILD
     """
     aport = pmb.helpers.pmaports.find(args, pkgname)
     ret = arch_from_deviceinfo(args, pkgname, aport)
     if ret:
         return ret
 
-    apkbuild = pmb.parse.apkbuild(args, aport + "/APKBUILD")
+    apkbuild = pmb.parse.apkbuild(f"{aport}/APKBUILD")
     arches = apkbuild["arch"]
-    if "noarch" in arches or "all" in arches or args.arch_native in arches:
-        return args.arch_native
-
-    arch_device = args.deviceinfo["arch"]
-    if arch_device in arches:
-        return arch_device
 
-    return apkbuild["arch"][0]
+    if args.build_default_device_arch:
+        preferred_arch = args.deviceinfo["arch"]
+        preferred_arch_2nd = pmb.config.arch_native
+    else:
+        preferred_arch = pmb.config.arch_native
+        preferred_arch_2nd = args.deviceinfo["arch"]
+
+    if "noarch" in arches or "all" in arches or preferred_arch in arches:
+        return preferred_arch
+
+    if preferred_arch_2nd in arches:
+        return preferred_arch_2nd
+
+    try:
+        return apkbuild["arch"][0]
+    except IndexError:
+        return None
 
 
-def suffix(args, apkbuild, arch):
-    if arch == args.arch_native:
+def suffix(apkbuild, arch):
+    if arch == pmb.config.arch_native:
         return "native"
 
-    pkgname = apkbuild["pkgname"]
-    if args.cross:
-        for pattern in pmb.config.build_cross_native:
-            if fnmatch.fnmatch(pkgname, pattern):
-                return "native"
+    if "pmb:cross-native" in apkbuild["options"]:
+        return "native"
 
     return "buildroot_" + arch
 
 
 def crosscompile(args, apkbuild, arch, suffix):
     """
-        :returns: None, "native", "crossdirect" or "distcc"
+        :returns: None, "native", "crossdirect"
     """
     if not args.cross:
         return None
-    if not pmb.parse.arch.cpu_emulation_required(args, arch):
+    if not pmb.parse.arch.cpu_emulation_required(arch):
         return None
     if suffix == "native":
         return "native"
-    if args.no_crossdirect:
-        return "distcc"
+    if "!pmb:crossdirect" in apkbuild["options"]:
+        return None
     return "crossdirect"
```

### Comparing `pmbootstrap-1.9.0/pmb/build/other.py` & `pmbootstrap-2.0.0/pmb/build/other.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import glob
 import logging
 import os
 import shlex
 import datetime
 
 import pmb.chroot
@@ -40,15 +24,24 @@
 
     # Clean up folder
     build = args.work + "/chroot_" + suffix + "/home/pmos/build"
     if os.path.exists(build):
         pmb.chroot.root(args, ["rm", "-rf", "/home/pmos/build"], suffix)
 
     # Copy aport contents with resolved symlinks
-    pmb.helpers.run.root(args, ["cp", "-rL", aport + "/", build])
+    pmb.helpers.run.root(args, ["mkdir", "-p", build])
+    for entry in os.listdir(aport):
+        # Don't copy those dirs, as those have probably been generated by running `abuild`
+        # on the host system directly and not cleaning up after itself.
+        # Those dirs might contain broken symlinks and cp fails resolving them.
+        if entry in ["src", "pkg"]:
+            logging.warn(f"WARNING: Not copying {entry}, looks like a leftover from abuild")
+            continue
+        pmb.helpers.run.root(args, ["cp", "-rL", f"{aport}/{entry}", f"{build}/{entry}"])
+
     pmb.chroot.root(args, ["chown", "-R", "pmos:pmos",
                            "/home/pmos/build"], suffix)
 
 
 def is_necessary(args, arch, apkbuild, indexes=None):
     """
     Check if the package has already been built. Compared to abuild's check,
@@ -67,29 +60,36 @@
     # Get old version from APKINDEX
     index_data = pmb.parse.apkindex.package(args, package, arch, False,
                                             indexes)
     if not index_data:
         logging.debug(msg + "No binary package available")
         return True
 
+    # Can't build pmaport for arch: use Alpine's package (#1897)
+    if arch and not pmb.helpers.pmaports.check_arches(apkbuild["arch"], arch):
+        logging.verbose(f"{package}: build is not necessary, because pmaport"
+                        " can't be built for {arch}. Using Alpine's binary"
+                        " package.")
+        return False
+
     # a) Binary repo has a newer version
     version_old = index_data["version"]
     if pmb.parse.version.compare(version_old, version_new) == 1:
         logging.warning("WARNING: package {}: aport version {} is lower than"
                         " {} from the binary repository. {} will be used when"
                         " installing {}. See also:"
                         " <https://postmarketos.org/warning-repo2>"
                         "".format(package, version_new, version_old,
                                   version_old, package))
         return False
 
     # b) Aports folder has a newer version
     if version_new != version_old:
-        logging.debug(msg + "Binary package out of date (binary: " + version_old +
-                      ", aport: " + version_new + ")")
+        logging.debug(f"{msg}Binary package out of date (binary: "
+                      f"{version_old}, aport: {version_new})")
         return True
 
     # Aports and binary repo have the same version.
     return False
 
 
 def index_repo(args, arch=None):
@@ -98,18 +98,19 @@
     cache for that file for the current pmbootstrap session (to prevent
     rebuilding packages twice, in case the rebuild takes less than a second).
 
     :param arch: when not defined, re-index all repos
     """
     pmb.build.init(args)
 
+    channel = pmb.config.pmaports.read_config(args)["channel"]
     if arch:
-        paths = [args.work + "/packages/" + arch]
+        paths = [f"{args.work}/packages/{channel}/{arch}"]
     else:
-        paths = glob.glob(args.work + "/packages/*")
+        paths = glob.glob(f"{args.work}/packages/{channel}/*")
 
     for path in paths:
         if os.path.isdir(path):
             path_arch = os.path.basename(path)
             path_repo_chroot = "/home/pmos/packages/pmos/" + path_arch
             logging.debug("(native) index " + path_arch + " repository")
             description = str(datetime.datetime.now())
@@ -121,15 +122,15 @@
                 ["abuild-sign", "APKINDEX.tar.gz_"],
                 ["mv", "APKINDEX.tar.gz_", "APKINDEX.tar.gz"]
             ]
             for command in commands:
                 pmb.chroot.user(args, command, working_dir=path_repo_chroot)
         else:
             logging.debug("NOTE: Can't build index for: " + path)
-        pmb.parse.apkindex.clear_cache(args, path + "/APKINDEX.tar.gz")
+        pmb.parse.apkindex.clear_cache(f"{path}/APKINDEX.tar.gz")
 
 
 def configure_abuild(args, suffix, verify=False):
     """
     Set the correct JOBS count in abuild.conf
 
     :param verify: internally used to test if changing the config has worked.
@@ -138,22 +139,24 @@
     prefix = "export JOBS="
     with open(path, encoding="utf-8") as handle:
         for line in handle:
             if not line.startswith(prefix):
                 continue
             if line != (prefix + args.jobs + "\n"):
                 if verify:
-                    raise RuntimeError("Failed to configure abuild: " + path +
-                                       "\nTry to delete the file (or zap the chroot).")
+                    raise RuntimeError(f"Failed to configure abuild: {path}"
+                                       "\nTry to delete the file"
+                                       "(or zap the chroot).")
                 pmb.chroot.root(args, ["sed", "-i", "-e",
-                                       "s/^" + prefix + ".*/" + prefix + args.jobs + "/",
-                                       "/etc/abuild.conf"], suffix)
+                                       f"s/^{prefix}.*/{prefix}{args.jobs}/",
+                                       "/etc/abuild.conf"],
+                                suffix)
                 configure_abuild(args, suffix, True)
             return
-    raise RuntimeError("Could not find " + prefix + " line in " + path)
+    pmb.chroot.root(args, ["sed", "-i", f"$ a\\{prefix}{args.jobs}", "/etc/abuild.conf"], suffix)
 
 
 def configure_ccache(args, suffix="native", verify=False):
     """
     Set the maximum ccache size
 
     :param verify: internally used to test if changing the config has worked.
```

### Comparing `pmbootstrap-1.9.0/pmb/build/init.py` & `pmbootstrap-2.0.0/pmb/build/init.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,96 +1,113 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
-import os
-import logging
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import glob
+import logging
+import os
+import pathlib
 
 import pmb.build
 import pmb.config
 import pmb.chroot
 import pmb.chroot.apk
 import pmb.helpers.run
 
 
-def init(args, suffix="native"):
-    # Check if already initialized
-    marker = "/var/local/pmbootstrap_chroot_build_init_done"
-    if os.path.exists(args.work + "/chroot_" + suffix + marker):
+def init_abuild_minimal(args, suffix="native"):
+    """ Initialize a minimal chroot with abuild where one can do
+        'abuild checksum'. """
+    marker = f"{args.work}/chroot_{suffix}/tmp/pmb_chroot_abuild_init_done"
+    if os.path.exists(marker):
         return
 
-    # Initialize chroot, install packages
-    pmb.chroot.apk.install(args, pmb.config.build_packages, suffix,
-                           build=False)
+    pmb.chroot.apk.install(args, ["abuild"], suffix, build=False)
 
     # Fix permissions
     pmb.chroot.root(args, ["chown", "root:abuild",
                            "/var/cache/distfiles"], suffix)
     pmb.chroot.root(args, ["chmod", "g+w",
                            "/var/cache/distfiles"], suffix)
 
+    # Add user to group abuild
+    pmb.chroot.root(args, ["adduser", "pmos", "abuild"], suffix)
+
+    pathlib.Path(marker).touch()
+
+
+def init(args, suffix="native"):
+    """ Initialize a chroot for building packages with abuild. """
+    marker = f"{args.work}/chroot_{suffix}/tmp/pmb_chroot_build_init_done"
+    if os.path.exists(marker):
+        return
+
+    init_abuild_minimal(args, suffix)
+
+    # Initialize chroot, install packages
+    pmb.chroot.apk.install(args, pmb.config.build_packages, suffix,
+                           build=False)
+
     # Generate package signing keys
     chroot = args.work + "/chroot_" + suffix
     if not os.path.exists(args.work + "/config_abuild/abuild.conf"):
         logging.info("(" + suffix + ") generate abuild keys")
         pmb.chroot.user(args, ["abuild-keygen", "-n", "-q", "-a"],
-                        suffix)
+                        suffix, env={"PACKAGER": "pmos <pmos@local>"})
 
         # Copy package signing key to /etc/apk/keys
         for key in glob.glob(chroot +
                              "/mnt/pmbootstrap-abuild-config/*.pub"):
             key = key[len(chroot):]
             pmb.chroot.root(args, ["cp", key, "/etc/apk/keys/"], suffix)
 
-    # Add gzip wrapper, that converts '-9' to '-1'
+    # Add gzip wrapper that converts '-9' to '-1'
     if not os.path.exists(chroot + "/usr/local/bin/gzip"):
         with open(chroot + "/tmp/gzip_wrapper.sh", "w") as handle:
             content = """
                 #!/bin/sh
-                # Simple wrapper, that converts -9 flag for gzip to -1 for speed
-                # improvement with abuild. FIXME: upstream to abuild with a flag!
+                # Simple wrapper that converts -9 flag for gzip to -1 for
+                # speed improvement with abuild. FIXME: upstream to abuild
+                # with a flag!
                 args=""
                 for arg in "$@"; do
                     [ "$arg" == "-9" ] && arg="-1"
                     args="$args $arg"
                 done
                 /bin/gzip $args
             """
             lines = content.split("\n")[1:]
             for i in range(len(lines)):
                 lines[i] = lines[i][16:]
             handle.write("\n".join(lines))
-        pmb.chroot.root(args, ["cp", "/tmp/gzip_wrapper.sh", "/usr/local/bin/gzip"],
-                        suffix)
+        pmb.chroot.root(args, ["cp", "/tmp/gzip_wrapper.sh",
+                               "/usr/local/bin/gzip"], suffix)
         pmb.chroot.root(args, ["chmod", "+x", "/usr/local/bin/gzip"], suffix)
 
-    # Add user to group abuild
-    pmb.chroot.root(args, ["adduser", "pmos", "abuild"], suffix)
-
     # abuild.conf: Don't clean the build folder after building, so we can
     # inspect it afterwards for debugging
     pmb.chroot.root(args, ["sed", "-i", "-e", "s/^CLEANUP=.*/CLEANUP=''/",
                            "/etc/abuild.conf"], suffix)
 
     # abuild.conf: Don't clean up installed packages in strict mode, so
     # abuild exits directly when pressing ^C in pmbootstrap.
     pmb.chroot.root(args, ["sed", "-i", "-e",
                            "s/^ERROR_CLEANUP=.*/ERROR_CLEANUP=''/",
                            "/etc/abuild.conf"], suffix)
 
-    # Mark the chroot as initialized
-    pmb.chroot.root(args, ["touch", marker], suffix)
+    pathlib.Path(marker).touch()
+
+
+def init_compiler(args, depends, cross, arch):
+    cross_pkgs = ["ccache-cross-symlinks"]
+    if "gcc4" in depends:
+        cross_pkgs += ["gcc4-" + arch]
+    elif "gcc6" in depends:
+        cross_pkgs += ["gcc6-" + arch]
+    else:
+        cross_pkgs += ["gcc-" + arch, "g++-" + arch]
+    if "clang" in depends or "clang-dev" in depends:
+        cross_pkgs += ["clang"]
+    if cross == "crossdirect":
+        cross_pkgs += ["crossdirect"]
+        if "rust" in depends or "cargo" in depends:
+            cross_pkgs += depends
+
+    pmb.chroot.apk.install(args, cross_pkgs)
```

### Comparing `pmbootstrap-1.9.0/pmb/build/_package.py` & `pmbootstrap-2.0.0/pmb/build/_package.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,37 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import datetime
 import logging
 import os
 
 import pmb.build
 import pmb.build.autodetect
 import pmb.chroot
 import pmb.chroot.apk
-import pmb.chroot.distccd
 import pmb.helpers.pmaports
 import pmb.helpers.repo
 import pmb.parse
 import pmb.parse.arch
 
 
-def skip_already_built(args, pkgname, arch):
+def skip_already_built(pkgname, arch):
     """
     Check if the package was already built in this session, and add it
     to the cache in case it was not built yet.
 
     :returns: True when it can be skipped or False
     """
-    if arch not in args.cache["built"]:
-        args.cache["built"][arch] = []
-    if pkgname in args.cache["built"][arch]:
+    if arch not in pmb.helpers.other.cache["built"]:
+        pmb.helpers.other.cache["built"][arch] = []
+    if pkgname in pmb.helpers.other.cache["built"][arch]:
         logging.verbose(pkgname + ": already checked this session,"
                         " no need to build it or its dependencies")
         return True
-    args.cache["built"][arch].append(pkgname)
+    pmb.helpers.other.cache["built"][arch].append(pkgname)
     return False
 
 
 def get_apkbuild(args, pkgname, arch):
     """
     Parse the APKBUILD path for pkgname. When there is none, try to find it in
     the binary package APKINDEX files or raise an exception.
@@ -116,15 +99,16 @@
     if "!check" not in apkbuild["options"]:
         ret += apkbuild["checkdepends"]
     if "ignore_depends" not in args or not args.ignore_depends:
         ret += apkbuild["depends"]
     ret = sorted(set(ret))
 
     # Don't recurse forever when a package depends on itself (#948)
-    for pkgname in [apkbuild["pkgname"]] + list(apkbuild["subpackages"]):
+    for pkgname in ([apkbuild["pkgname"]] +
+                    list(apkbuild["subpackages"].keys())):
         if pkgname in ret:
             logging.verbose(apkbuild["pkgname"] + ": ignoring dependency on"
                             " itself: " + pkgname)
             ret.remove(pkgname)
     return ret
 
 
@@ -139,23 +123,38 @@
     depends = get_depends(args, apkbuild)
     logging.verbose(pkgname + ": build/install dependencies: " +
                     ", ".join(depends))
 
     # --no-depends: check for binary packages
     depends_built = []
     if "no_depends" in args and args.no_depends:
+        pmb.helpers.repo.update(args, arch)
         for depend in depends:
+            # Ignore conflicting dependencies
+            if depend.startswith("!"):
+                continue
+            # Check if binary package is missing
             if not pmb.parse.apkindex.package(args, depend, arch, False):
                 raise RuntimeError("Missing binary package for dependency '" +
                                    depend + "' of '" + pkgname + "', but"
                                    " pmbootstrap won't build any depends since"
                                    " it was started with --no-depends.")
+            # Check if binary package is outdated
+            apkbuild_dep = get_apkbuild(args, depend, arch)
+            if apkbuild_dep and \
+               pmb.build.is_necessary(args, arch, apkbuild_dep):
+                raise RuntimeError(f"Binary package for dependency '{depend}'"
+                                   f" of '{pkgname}' is outdated, but"
+                                   f" pmbootstrap won't build any depends"
+                                   f" since it was started with --no-depends.")
     else:
         # Build the dependencies
         for depend in depends:
+            if depend.startswith("!"):
+                continue
             if package(args, depend, arch, strict=strict):
                 depends_built += [depend]
         logging.verbose(pkgname + ": build dependencies: done, built: " +
                         ", ".join(depends_built))
 
     return (depends, depends_built)
 
@@ -172,43 +171,40 @@
     # Check if necessary (this warns about binary version > aport version, so
     # call it even in force mode)
     ret = pmb.build.is_necessary(args, arch, apkbuild)
     if force:
         ret = True
 
     if not ret and len(depends_built):
-        # Warn of potentially outdated package
-        logging.warning("WARNING: " + pkgname + " depends on rebuilt" +
-                        " package(s) " + ",".join(depends_built) + " (use" +
-                        " 'pmbootstrap build " + pkgname + " --force' if" +
-                        " necessary!)")
+        logging.verbose(f"{pkgname}: depends on rebuilt package(s): "
+                        f" {', '.join(depends_built)}")
 
     logging.verbose(pkgname + ": build necessary: " + str(ret))
     return ret
 
 
 def init_buildenv(args, apkbuild, arch, strict=False, force=False, cross=None,
                   suffix="native", skip_init_buildenv=False, src=None):
     """
     Build all dependencies, check if we need to build at all (otherwise we've
     just initialized the build environment for nothing) and then setup the
     whole build environment (abuild, gcc, dependencies, cross-compiler).
 
-    :param cross: None, "native", "distcc", or "crossdirect"
+    :param cross: None, "native", or "crossdirect"
     :param skip_init_buildenv: can be set to False to avoid initializing the
                                build environment. Use this when building
                                something during initialization of the build
                                environment (e.g. qemu aarch64 bug workaround)
     :param src: override source used to build the package with a local folder
     :returns: True when the build is necessary (otherwise False)
     """
 
     depends_arch = arch
     if cross == "native":
-        depends_arch = args.arch_native
+        depends_arch = pmb.config.arch_native
 
     # Build dependencies
     depends, built = build_depends(args, apkbuild, depends_arch, strict)
 
     # Check if build is necessary
     if not is_necessary_warn_depends(args, apkbuild, arch, force, built):
         return False
@@ -221,47 +217,21 @@
     if not strict and "pmb:strict" not in apkbuild["options"] and len(depends):
         pmb.chroot.apk.install(args, depends, suffix)
     if src:
         pmb.chroot.apk.install(args, ["rsync"], suffix)
 
     # Cross-compiler init
     if cross:
-        cross_pkgs = ["ccache-cross-symlinks"]
-        if "gcc4" in depends:
-            cross_pkgs += ["gcc4-" + arch]
-        elif "gcc6" in depends:
-            cross_pkgs += ["gcc6-" + arch]
-        else:
-            cross_pkgs += ["gcc-" + arch, "g++-" + arch]
-        if "clang" in depends or "clang-dev" in depends:
-            cross_pkgs += ["clang"]
-        if cross == "crossdirect":
-            cross_pkgs += ["crossdirect"]
-        pmb.chroot.apk.install(args, cross_pkgs)
-    if cross == "distcc":
-        pmb.chroot.distccd.start(args, arch)
+        pmb.build.init_compiler(args, depends, cross, arch)
     if cross == "crossdirect":
         pmb.chroot.mount_native_into_foreign(args, suffix)
 
     return True
 
 
-def get_gcc_version(args, arch):
-    """
-    Get the GCC version for a specific arch from parsing the right APKINDEX.
-    We feed this to ccache, so it knows the right GCC version, when
-    cross-compiling in a foreign arch chroot with distcc. See the "using
-    ccache with other compiler wrappers" section of their man page:
-    <https://linux.die.net/man/1/ccache>
-    :returns: a string like "6.4.0-r5"
-    """
-    return pmb.parse.apkindex.package(args, "gcc-" + arch,
-                                      args.arch_native)["version"]
-
-
 def get_pkgver(original_pkgver, original_source=False, now=None):
     """
     Get the original pkgver when using the original source. Otherwise, get the
     pkgver with an appended suffix of current date and time. For example:
         _p20180218550502
     When appending the suffix, an existing suffix (e.g. _git20171231) gets
     replaced.
@@ -345,22 +315,61 @@
     apkbuild_path = "/home/pmos/build/APKBUILD"
     shell_cmd = ("cat " + apkbuild_path + " " + append_path + " > " +
                  append_path + "_")
     pmb.chroot.user(args, ["sh", "-c", shell_cmd], suffix)
     pmb.chroot.user(args, ["mv", append_path + "_", apkbuild_path], suffix)
 
 
+def mount_pmaports(args, destination, suffix="native"):
+    """
+    Mount pmaports.git in chroot.
+
+    :param destination: mount point inside the chroot
+    """
+    outside_destination = args.work + "/chroot_" + suffix + destination
+    pmb.helpers.mount.bind(args, args.aports, outside_destination, umount=True)
+
+
+def link_to_git_dir(args, suffix):
+    """
+    Make /home/pmos/build/.git point to the .git dir from pmaports.git, with a
+    symlink so abuild does not fail (#1841).
+
+    abuild expects the current working directory to be a subdirectory of a
+    cloned git repository (e.g. main/openrc from aports.git). If git is
+    installed, it will try to get the last git commit from that repository, and
+    place it in the resulting apk (.PKGINFO) as well as use the date from that
+    commit as SOURCE_DATE_EPOCH (for reproducible builds).
+
+    With that symlink, we actually make it use the last git commit from
+    pmaports.git for SOURCE_DATE_EPOCH and have that in the resulting apk's
+    .PKGINFO.
+    """
+    # Mount pmaports.git in chroot, in case the user did not use pmbootstrap to
+    # clone it (e.g. how we build on sourcehut). Do this here and not at the
+    # initialization of the chroot, because the pmaports dir may not exist yet
+    # at that point. Use umount=True, so we don't have an old path mounted
+    # (some tests change the pmaports dir).
+    destination = "/mnt/pmaports"
+    mount_pmaports(args, destination, suffix)
+
+    # Create .git symlink
+    pmb.chroot.user(args, ["mkdir", "-p", "/home/pmos/build"], suffix)
+    pmb.chroot.user(args, ["ln", "-sf", destination + "/.git",
+                           "/home/pmos/build/.git"], suffix)
+
+
 def run_abuild(args, apkbuild, arch, strict=False, force=False, cross=None,
                suffix="native", src=None):
     """
     Set up all environment variables and construct the abuild command (all
     depending on the cross-compiler method and target architecture), copy
     the aport to the chroot and execute abuild.
 
-    :param cross: None, "native", "distcc", or "crossdirect"
+    :param cross: None, "native", or "crossdirect"
     :param src: override source used to build the package with a local folder
     :returns: (output, cmd, env), output is the destination apk path relative
               to the package folder ("x86_64/hello-1-r2.apk"). cmd and env are
               used by the test case, and they are the full abuild command and
               the environment variables dict generated in this function.
     """
     # Sanity check
@@ -381,32 +390,32 @@
     # Environment variables
     env = {"CARCH": arch,
            "SUDO_APK": "abuild-apk --no-progress"}
     if cross == "native":
         hostspec = pmb.parse.arch.alpine_to_hostspec(arch)
         env["CROSS_COMPILE"] = hostspec + "-"
         env["CC"] = hostspec + "-gcc"
-    if cross == "distcc":
-        env["CCACHE_PREFIX"] = "distcc"
-        env["CCACHE_PATH"] = "/usr/lib/arch-bin-masquerade/" + arch + ":/usr/bin"
-        env["CCACHE_COMPILERCHECK"] = "string:" + get_gcc_version(args, arch)
-        env["DISTCC_HOSTS"] = "@127.0.0.1:/home/pmos/.distcc-sshd/distccd"
-        env["DISTCC_SSH"] = ("ssh -o StrictHostKeyChecking=no -p" +
-                             args.port_distccd)
-        env["DISTCC_BACKOFF_PERIOD"] = "0"
-        if not args.distcc_fallback:
-            env["DISTCC_FALLBACK"] = "0"
-        if args.verbose:
-            env["DISTCC_VERBOSE"] = "1"
     if cross == "crossdirect":
         env["PATH"] = ":".join(["/native/usr/lib/crossdirect/" + arch,
                                 pmb.config.chroot_path])
     if not args.ccache:
         env["CCACHE_DISABLE"] = "1"
 
+    # Cache binary objects from go in this path (like ccache)
+    env["GOCACHE"] = "/home/pmos/.cache/go-build"
+
+    # Cache go modules (git repositories). Usually these should be bundled and
+    # it should not be required to download them at build time, in that case
+    # the APKBUILD sets the GOPATH (and therefore indirectly GOMODCACHE). But
+    # e.g. when using --src they are not bundled, in that case it makes sense
+    # to point GOMODCACHE at pmbootstrap's work dir so the modules are only
+    # downloaded once.
+    if args.go_mod_cache:
+        env["GOMODCACHE"] = "/home/pmos/go/pkg/mod"
+
     # Build the abuild command
     cmd = ["abuild", "-D", "postmarketOS"]
     if strict or "pmb:strict" in apkbuild["options"]:
         if not strict:
             logging.debug(apkbuild["pkgname"] + ": 'pmb:strict' found in"
                           " options, building in strict mode")
         cmd += ["-r"]  # install depends with abuild
@@ -414,72 +423,82 @@
         cmd += ["-d"]  # do not install depends with abuild
     if force:
         cmd += ["-f"]
 
     # Copy the aport to the chroot and build it
     pmb.build.copy_to_buildpath(args, apkbuild["pkgname"], suffix)
     override_source(args, apkbuild, pkgver, src, suffix)
+    link_to_git_dir(args, suffix)
     pmb.chroot.user(args, cmd, suffix, "/home/pmos/build", env=env)
     return (output, cmd, env)
 
 
 def finish(args, apkbuild, arch, output, strict=False, suffix="native"):
     """
     Various finishing tasks that need to be done after a build.
     """
     # Verify output file
-    path = args.work + "/packages/" + output
+    channel = pmb.config.pmaports.read_config(args)["channel"]
+    path = f"{args.work}/packages/{channel}/{output}"
     if not os.path.exists(path):
         raise RuntimeError("Package not found after build: " + path)
 
     # Clear APKINDEX cache (we only parse APKINDEX files once per session and
     # cache the result for faster dependency resolving, but after we built a
     # package we need to parse it again)
-    pmb.parse.apkindex.clear_cache(args, args.work + "/packages/" +
-                                   arch + "/APKINDEX.tar.gz")
+    pmb.parse.apkindex.clear_cache(f"{args.work}/packages/{channel}"
+                                   f"/{arch}/APKINDEX.tar.gz")
 
     # Uninstall build dependencies (strict mode)
     if strict or "pmb:strict" in apkbuild["options"]:
         logging.info("(" + suffix + ") uninstall build dependencies")
         pmb.chroot.user(args, ["abuild", "undeps"], suffix, "/home/pmos/build",
                         env={"SUDO_APK": "abuild-apk --no-progress"})
+        # If the build depends contain postmarketos-keys or postmarketos-base,
+        # abuild will have removed the postmarketOS repository key (pma#1230)
+        pmb.chroot.init_keys(args)
 
 
 def package(args, pkgname, arch=None, force=False, strict=False,
             skip_init_buildenv=False, src=None):
     """
     Build a package and its dependencies with Alpine Linux' abuild.
 
+    If this function is called multiple times on the same pkgname but first
+    with force=False and then force=True the force argument will be ignored due
+    to the package cache.
+    See the skip_already_built() call below.
+
     :param pkgname: package name to be built, as specified in the APKBUILD
     :param arch: architecture we're building for (default: native)
-    :param force: even build, if not necessary
+    :param force: always build, even if not necessary
     :param strict: avoid building with irrelevant dependencies installed by
                    letting abuild install and uninstall all dependencies.
     :param skip_init_buildenv: can be set to False to avoid initializing the
                                build environment. Use this when building
                                something during initialization of the build
                                environment (e.g. qemu aarch64 bug workaround)
     :param src: override source used to build the package with a local folder
     :returns: None if the build was not necessary
               output path relative to the packages folder ("armhf/ab-1-r2.apk")
     """
     # Once per session is enough
-    arch = arch or args.arch_native
-    if skip_already_built(args, pkgname, arch):
+    arch = arch or pmb.config.arch_native
+    if skip_already_built(pkgname, arch):
         return
 
     # Only build when APKBUILD exists
     apkbuild = get_apkbuild(args, pkgname, arch)
     if not apkbuild:
         return
 
     # Detect the build environment (skip unnecessary builds)
     if not check_build_for_arch(args, pkgname, arch):
         return
-    suffix = pmb.build.autodetect.suffix(args, apkbuild, arch)
+    suffix = pmb.build.autodetect.suffix(apkbuild, arch)
     cross = pmb.build.autodetect.crosscompile(args, apkbuild, arch, suffix)
     if not init_buildenv(args, apkbuild, arch, strict, force, cross, suffix,
                          skip_init_buildenv, src):
         return
 
     # Build and finish up
     (output, cmd, env) = run_abuild(args, apkbuild, arch, strict, force, cross,
```

### Comparing `pmbootstrap-1.9.0/pmb/build/envkernel.py` & `pmbootstrap-2.0.0/pmb/build/envkernel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,29 @@
-"""
-Copyright 2019 Robert Yang
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Robert Yang
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 import os
 import re
 
 import pmb.aportgen
 import pmb.build
 import pmb.chroot
 import pmb.helpers
 import pmb.helpers.pmaports
 import pmb.parse
 
 
-def match_kbuild_out(args, word):
+def match_kbuild_out(word):
     """
     Look for paths in the following formats:
       "<prefix>/<kbuild_out>/arch/<arch>/boot"
       "<prefix>/<kbuild_out>/include/config/kernel.release"
 
     :param word: space separated string cut out from a line from an APKBUILD
-                 function body, that might be the kbuild output path
+                 function body that might be the kbuild output path
     :returns: kernel build output directory.
               empty string when a separate build output directory isn't used.
               None, when no output directory is found.
     """
     prefix = "^\\\"?\\$({?builddir}?|{?srcdir}?)\\\"?/"
     kbuild_out = "(.*\\/)*"
 
@@ -59,29 +43,29 @@
 
     logging.debug("word = " + str(word))
     logging.debug("regex match groups = " + str(groups))
     out_dir = groups[1]
     return "" if out_dir is None else out_dir.strip("/")
 
 
-def find_kbuild_output_dir(args, function_body):
+def find_kbuild_output_dir(function_body):
     """
     Guess what the kernel build output directory is. Parses each line of the
     function word by word, looking for paths which contain the kbuild output
     directory.
 
     :param function_body: contents of a function from the kernel APKBUILD
     :returns: kbuild output dir
               None, when output dir is not found
     """
 
     guesses = []
     for line in function_body:
         for item in line.split():
-            kbuild_out = match_kbuild_out(args, item)
+            kbuild_out = match_kbuild_out(item)
             if kbuild_out is not None:
                 guesses.append(kbuild_out)
                 break
 
     # Check if guesses are all the same
     it = iter(guesses)
     first = next(it, None)
@@ -98,15 +82,15 @@
 
 
 def modify_apkbuild(args, pkgname, aport):
     """
     Modify kernel APKBUILD to package build output from envkernel.sh
     """
     apkbuild_path = aport + "/APKBUILD"
-    apkbuild = pmb.parse.apkbuild(args, apkbuild_path)
+    apkbuild = pmb.parse.apkbuild(apkbuild_path)
     if os.path.exists(args.work + "/aportgen"):
         pmb.helpers.run.user(args, ["rm", "-r", args.work + "/aportgen"])
 
     pmb.helpers.run.user(args, ["mkdir", args.work + "/aportgen"])
     pmb.helpers.run.user(args, ["cp", "-r", apkbuild_path,
                          args.work + "/aportgen"])
 
@@ -116,31 +100,68 @@
               "pkgrel": "0",
               "subpackages": "",
               "builddir": "/home/pmos/build/src"}
 
     pmb.aportgen.core.rewrite(args, pkgname, apkbuild_path, fields=fields)
 
 
+def host_build_bindmount(args, chroot, flag_file, mount=False):
+    """
+    Check if the bind mount already exists and unmount it.
+    Then bindmount the current directory into the chroot as
+    /mnt/linux so it can be used by the envkernel abuild wrapper
+    """
+    flag_path = f"{chroot}/{flag_file}"
+    if os.path.exists(flag_path):
+        logging.info("Cleaning up kernel sources bind-mount")
+        pmb.helpers.run.root(args, ["umount", chroot + "/mnt/linux"], check=False)
+        pmb.helpers.run.root(args, ["rm", flag_path])
+
+    if mount:
+        pmb.helpers.mount.bind(args, ".", f"{chroot}/mnt/linux")
+        pmb.helpers.run.root(args, ["touch", flag_path])
+
+
 def run_abuild(args, pkgname, arch, apkbuild_path, kbuild_out):
     """
     Prepare build environment and run abuild.
 
     :param pkgname: package name of a linux kernel aport
     :param arch: architecture for the kernel
     :param apkbuild_path: path to APKBUILD of the kernel aport
     :param kbuild_out: kernel build system output sub-directory
     """
     chroot = args.work + "/chroot_native"
     build_path = "/home/pmos/build"
     kbuild_out_source = "/mnt/linux/.output"
 
+    # If the kernel was cross-compiled on the host rather than with the envkernel
+    # helper, we can still use the envkernel logic to package the artifacts for
+    # development, making it easy to quickly sideload a new kernel or pmbootstrap
+    # to create a boot image
+    # This handles bind mounting the current directory (assumed to be kernel sources)
+    # into the chroot so we can run abuild against it for the currently selected
+    # devices kernel package.
+    flag_file = "envkernel-bind-mounted"
+    host_build = False
+
+    if not pmb.helpers.mount.ismount(chroot + "/mnt/linux"):
+        logging.info("envkernel.sh hasn't run, assuming the kernel was cross compiled"
+                     "on host and using current dir as source")
+        host_build = True
+
+    host_build_bindmount(args, chroot, flag_file, mount=host_build)
+
     if not os.path.exists(chroot + kbuild_out_source):
-        raise RuntimeError("No '.output' dir found in your kernel source dir."
-                           "Compile the " + args.device + " kernel with "
-                           "envkernel.sh first, then try again.")
+        raise RuntimeError("No '.output' dir found in your kernel source dir. "
+                           "Compile the " + args.device + " kernel first and "
+                           "then try again. See https://postmarketos.org/envkernel"
+                           "for details. If building on your host and only using "
+                           "--envkernel for packaging, make sure you have O=.output "
+                           "as an argument to make.")
 
     # Create working directory for abuild
     pmb.build.copy_to_buildpath(args, pkgname)
 
     # Create symlink from abuild working directory to envkernel build directory
     build_output = "" if kbuild_out == "" else "/" + kbuild_out
     if build_output != "":
@@ -154,19 +175,22 @@
 
     cmd = ["cp", apkbuild_path, chroot + build_path + "/APKBUILD"]
     pmb.helpers.run.root(args, cmd)
 
     # Create the apk package
     env = {"CARCH": arch,
            "CHOST": arch,
-           "CBUILD": args.arch_native,
+           "CBUILD": pmb.config.arch_native,
            "SUDO_APK": "abuild-apk --no-progress"}
     cmd = ["abuild", "rootpkg"]
     pmb.chroot.user(args, cmd, working_dir=build_path, env=env)
 
+    # Clean up bindmount if needed
+    host_build_bindmount(args, chroot, flag_file)
+
     # Clean up symlinks
     if build_output != "":
         if os.path.islink(chroot + "/mnt/linux/" + build_output) and \
                 os.path.lexists(chroot + "/mnt/linux/" + build_output):
             pmb.chroot.root(args, ["rm", "/mnt/linux/" + build_output])
     pmb.chroot.root(args, ["rm", build_path + "/src"])
 
@@ -178,23 +202,35 @@
     """
     pkgname = args.packages[0]
     if len(args.packages) > 1 or not pkgname.startswith("linux-"):
         raise RuntimeError("--envkernel needs exactly one linux-* package as "
                            "argument.")
 
     aport = pmb.helpers.pmaports.find(args, pkgname)
-    function_body = pmb.parse.function_body(aport + "/APKBUILD", "package")
-    kbuild_out = find_kbuild_output_dir(args, function_body)
 
     modify_apkbuild(args, pkgname, aport)
     apkbuild_path = args.work + "/aportgen/APKBUILD"
 
     arch = args.deviceinfo["arch"]
-    apkbuild = pmb.parse.apkbuild(args, apkbuild_path, check_pkgname=False)
-    suffix = pmb.build.autodetect.suffix(args, apkbuild, arch)
+    apkbuild = pmb.parse.apkbuild(apkbuild_path, check_pkgname=False)
+    if apkbuild["_outdir"]:
+        kbuild_out = apkbuild["_outdir"]
+    else:
+        function_body = pmb.parse.function_body(aport + "/APKBUILD", "package")
+        kbuild_out = find_kbuild_output_dir(function_body)
+    suffix = pmb.build.autodetect.suffix(apkbuild, arch)
+
+    # Install package dependencies
+    depends, _ = pmb.build._package.build_depends(
+        args, apkbuild, pmb.config.arch_native, strict=False)
+    pmb.build.init(args, suffix)
+    if pmb.parse.arch.cpu_emulation_required(arch):
+        depends.append("binutils-" + arch)
+    pmb.chroot.apk.install(args, depends, suffix)
+
     output = (arch + "/" + apkbuild["pkgname"] + "-" + apkbuild["pkgver"] +
               "-r" + apkbuild["pkgrel"] + ".apk")
     message = "(" + suffix + ") build " + output
     logging.info(message)
 
     run_abuild(args, pkgname, arch, apkbuild_path, kbuild_out)
     pmb.build.other.index_repo(args, arch)
```

### Comparing `pmbootstrap-1.9.0/pmb/build/newapkbuild.py` & `pmbootstrap-2.0.0/pmb/build/newapkbuild.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,9 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import glob
 import os
 import logging
 import pmb.chroot.user
 import pmb.helpers.cli
 import pmb.parse
 
@@ -37,15 +21,15 @@
     pmb.chroot.user(args, ["newapkbuild"] + args_passed, working_dir=build)
     glob_result = glob.glob(build_outside + "/*/APKBUILD")
     if not len(glob_result):
         return
 
     # Paths for copying
     source_apkbuild = glob_result[0]
-    pkgname = pmb.parse.apkbuild(args, source_apkbuild, False)["pkgname"]
+    pkgname = pmb.parse.apkbuild(source_apkbuild, False)["pkgname"]
     target = args.aports + "/" + folder + "/" + pkgname
 
     # Move /home/pmos/build/$pkgname/* to /home/pmos/build/*
     for path in glob.glob(build_outside + "/*/*"):
         path_inside = build + "/" + pkgname + "/" + os.path.basename(path)
         pmb.chroot.user(args, ["mv", path_inside, build])
     pmb.chroot.user(args, ["rmdir", build + "/" + pkgname])
```

### Comparing `pmbootstrap-1.9.0/pmb/build/menuconfig.py` & `pmbootstrap-2.0.0/pmb/build/kconfig.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,49 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import os
 import logging
 
 import pmb.build
 import pmb.build.autodetect
 import pmb.build.checksum
 import pmb.chroot
 import pmb.chroot.apk
 import pmb.chroot.other
 import pmb.helpers.pmaports
 import pmb.helpers.run
 import pmb.parse
 
 
-def get_arch(args, apkbuild):
+def get_arch(apkbuild):
     """
-    Get the architecture, that the user wants to run menuconfig on, depending on
-    the APKBUILD and on the --arch parameter.
+    Take the architecture from the APKBUILD or complain if it's ambiguous. This
+    function only gets called if --arch is not set.
 
     :param apkbuild: looks like: {"pkgname": "linux-...",
                                   "arch": ["x86_64", "armhf", "aarch64"]}
                      or: {"pkgname": "linux-...", "arch": ["armhf"]}
     """
     pkgname = apkbuild["pkgname"]
 
-    # Multiple architectures (requires --arch)
+    # Disabled package (arch="")
+    if not apkbuild["arch"]:
+        raise RuntimeError(f"'{pkgname}' is disabled (arch=\"\"). Please use"
+                           " '--arch' to specify the desired architecture.")
+
+    # Multiple architectures
     if len(apkbuild["arch"]) > 1:
-        if args.arch is None:
-            raise RuntimeError("Package '" + pkgname + "' supports multiple"
-                               " architectures, please use '--arch' to specify"
-                               " the desired architecture.")
-        return args.arch
-
-    # Single architecture (--arch must be unset or match)
-    if args.arch is None or args.arch == apkbuild["arch"][0]:
-        return apkbuild["arch"][0]
-    raise RuntimeError("Package '" + pkgname + "' only supports the '" +
-                       apkbuild["arch"][0] + "' architecture.")
+        raise RuntimeError(f"'{pkgname}' supports multiple architectures"
+                           f" ({', '.join(apkbuild['arch'])}). Please use"
+                           " '--arch' to specify the desired architecture.")
+
+    return apkbuild["arch"][0]
 
 
-def get_outputdir(args, pkgname):
+def get_outputdir(args, pkgname, apkbuild):
     """
     Get the folder for the kernel compilation output.
     For most APKBUILDs, this is $builddir. But some older ones still use
     $srcdir/build (see the discussion in #1551).
     """
     # Old style ($srcdir/build)
     ret = "/home/pmos/build/src/build"
@@ -81,73 +64,93 @@
                           output_return=True).rstrip()
     if os.path.exists(chroot + ret + "/.config"):
         return ret
     # Some Mediatek kernels use a 'kernel' subdirectory
     if os.path.exists(chroot + ret + "/kernel/.config"):
         return os.path.join(ret, "kernel")
 
+    # Out-of-tree builds ($_outdir)
+    if os.path.exists(chroot + ret + "/" + apkbuild["_outdir"] + "/.config"):
+        return os.path.join(ret, apkbuild["_outdir"])
+
     # Not found
     raise RuntimeError("Could not find the kernel config. Consider making a"
                        " backup of your APKBUILD and recreating it from the"
                        " template with: pmbootstrap aportgen " + pkgname)
 
 
-def menuconfig(args, pkgname):
+def extract_and_patch_sources(args, pkgname, arch):
+    pmb.build.copy_to_buildpath(args, pkgname)
+    logging.info("(native) extract kernel source")
+    pmb.chroot.user(args, ["abuild", "unpack"], "native", "/home/pmos/build")
+    logging.info("(native) apply patches")
+    pmb.chroot.user(args, ["abuild", "prepare"], "native",
+                    "/home/pmos/build", output="interactive",
+                    env={"CARCH": arch})
+
+
+def menuconfig(args, pkgname, use_oldconfig):
     # Pkgname: allow omitting "linux-" prefix
-    if pkgname.startswith("linux-"):
-        pkgname_ = pkgname.split("linux-")[1]
-        logging.info("PROTIP: You can simply do 'pmbootstrap kconfig edit " +
-                     pkgname_ + "'")
-    else:
+    if not pkgname.startswith("linux-"):
         pkgname = "linux-" + pkgname
 
     # Read apkbuild
     aport = pmb.helpers.pmaports.find(args, pkgname)
-    apkbuild = pmb.parse.apkbuild(args, aport + "/APKBUILD")
-    arch = get_arch(args, apkbuild)
-    kopt = "menuconfig"
+    apkbuild = pmb.parse.apkbuild(f"{aport}/APKBUILD")
+    arch = args.arch or get_arch(apkbuild)
+    suffix = pmb.build.autodetect.suffix(apkbuild, arch)
+    cross = pmb.build.autodetect.crosscompile(args, apkbuild, arch, suffix)
+    hostspec = pmb.parse.arch.alpine_to_hostspec(arch)
 
     # Set up build tools and makedepends
-    pmb.build.init(args)
+    pmb.build.init(args, suffix)
+    if cross:
+        pmb.build.init_compiler(args, [], cross, arch)
+
     depends = apkbuild["makedepends"]
-    kopt = "menuconfig"
     copy_xauth = False
-    if args.xconfig:
-        depends += ["qt-dev", "font-noto"]
-        kopt = "xconfig"
-        copy_xauth = True
-    elif args.gconfig:
-        depends += ["gtk+2.0-dev", "glib-dev", "libglade-dev", "font-noto"]
-        kopt = "gconfig"
-        copy_xauth = True
+
+    if use_oldconfig:
+        kopt = "oldconfig"
     else:
-        depends += ["ncurses-dev"]
+        kopt = "menuconfig"
+        if args.xconfig:
+            depends += ["qt5-qtbase-dev", "font-noto"]
+            kopt = "xconfig"
+            copy_xauth = True
+        elif args.nconfig:
+            kopt = "nconfig"
+            depends += ["ncurses-dev"]
+        else:
+            depends += ["ncurses-dev"]
+
     pmb.chroot.apk.install(args, depends)
 
     # Copy host's .xauthority into native
     if copy_xauth:
         pmb.chroot.other.copy_xauthority(args)
 
-    # Patch and extract sources
-    pmb.build.copy_to_buildpath(args, pkgname)
-    logging.info("(native) extract kernel source")
-    pmb.chroot.user(args, ["abuild", "unpack"], "native", "/home/pmos/build")
-    logging.info("(native) apply patches")
-    pmb.chroot.user(args, ["abuild", "prepare"], "native",
-                    "/home/pmos/build", output="interactive",
-                    env={"CARCH": arch})
+    extract_and_patch_sources(args, pkgname, arch)
+
+    # Check for background color variable
+    color = os.environ.get("MENUCONFIG_COLOR")
 
     # Run make menuconfig
-    outputdir = get_outputdir(args, pkgname)
+    outputdir = get_outputdir(args, pkgname, apkbuild)
     logging.info("(native) make " + kopt)
+    env = {"ARCH": pmb.parse.arch.alpine_to_kernel(arch),
+           "DISPLAY": os.environ.get("DISPLAY"),
+           "XAUTHORITY": "/home/pmos/.Xauthority"}
+    if cross:
+        env["CROSS_COMPILE"] = f"{hostspec}-"
+        env["CC"] = f"{hostspec}-gcc"
+    if color:
+        env["MENUCONFIG_COLOR"] = color
     pmb.chroot.user(args, ["make", kopt], "native",
-                    outputdir, output="tui",
-                    env={"ARCH": pmb.parse.arch.alpine_to_kernel(arch),
-                         "DISPLAY": os.environ.get("DISPLAY"),
-                         "XAUTHORITY": "/home/pmos/.Xauthority"})
+                    outputdir, output="tui", env=env)
 
     # Find the updated config
     source = args.work + "/chroot_native" + outputdir + "/.config"
     if not os.path.exists(source):
         raise RuntimeError("No kernel config generated: " + source)
 
     # Update the aport (config and checksum)
```

### Comparing `pmbootstrap-1.9.0/pmb/build/checksum.py` & `pmbootstrap-2.0.0/pmb/build/checksum.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,34 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 
 import pmb.chroot
 import pmb.build
 import pmb.helpers.run
 import pmb.helpers.pmaports
 
 
 def update(args, pkgname):
     """ Fetch all sources and update the checksums in the APKBUILD. """
-    pmb.build.init(args)
+    pmb.build.init_abuild_minimal(args)
     pmb.build.copy_to_buildpath(args, pkgname)
     logging.info("(native) generate checksums for " + pkgname)
     pmb.chroot.user(args, ["abuild", "checksum"],
                     working_dir="/home/pmos/build")
 
     # Copy modified APKBUILD back
     source = args.work + "/chroot_native/home/pmos/build/APKBUILD"
     target = pmb.helpers.pmaports.find(args, pkgname) + "/"
     pmb.helpers.run.user(args, ["cp", source, target])
 
 
 def verify(args, pkgname):
     """ Fetch all sources and verify their checksums. """
-    pmb.build.init(args)
+    pmb.build.init_abuild_minimal(args)
     pmb.build.copy_to_buildpath(args, pkgname)
     logging.info("(native) verify checksums for " + pkgname)
 
     # Fetch and verify sources, "fetch" alone does not verify them:
     # https://github.com/alpinelinux/abuild/pull/86
     pmb.chroot.user(args, ["abuild", "fetch", "verify"],
                     working_dir="/home/pmos/build")
```

### Comparing `pmbootstrap-1.9.0/pmb/install/recovery.py` & `pmbootstrap-2.0.0/pmb/install/recovery.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,13 @@
-"""
-Copyright 2019 Attila Szollosi
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Attila Szollosi
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 
 import pmb.chroot
+import pmb.config.pmaports
 import pmb.flasher
 import pmb.helpers.frontend
 
 
 def create_zip(args, suffix):
     """
     Create android recovery compatible installer zip.
@@ -42,25 +27,32 @@
 
     for key in vars:
         pmb.flasher.check_partition_blacklist(args, key, vars[key])
 
     # Create config file for the recovery installer
     options = {
         "DEVICE": args.device,
-        "FLAVOR": flavor,
         "FLASH_KERNEL": args.recovery_flash_kernel,
         "ISOREC": method == "heimdall-isorec",
         "KERNEL_PARTLABEL": vars["$PARTITION_KERNEL"],
         "INITFS_PARTLABEL": vars["$PARTITION_INITFS"],
-        "SYSTEM_PARTLABEL": vars["$PARTITION_SYSTEM"],
+        # Name is still "SYSTEM", not "ROOTFS" in the recovery installer
+        "SYSTEM_PARTLABEL": vars["$PARTITION_ROOTFS"],
         "INSTALL_PARTITION": args.recovery_install_partition,
         "CIPHER": args.cipher,
         "FDE": args.full_disk_encryption,
     }
 
+    # Backwards compatibility with old mkinitfs (pma#660)
+    pmaports_cfg = pmb.config.pmaports.read_config(args)
+    if pmaports_cfg.get("supported_mkinitfs_without_flavors", False):
+        options["FLAVOR"] = ""
+    else:
+        options["FLAVOR"] = f"-{flavor}" if flavor is not None else "-"
+
     # Write to a temporary file
     config_temp = args.work + "/chroot_" + suffix + "/tmp/install_options"
     with open(config_temp, "w") as handle:
         for key, value in options.items():
             if isinstance(value, bool):
                 value = str(value).lower()
             handle.write(key + "='" + value + "'\n")
```

### Comparing `pmbootstrap-1.9.0/pmb/install/blockdevice.py` & `pmbootstrap-2.0.0/pmb/install/blockdevice.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-"""
-Copyright 2019 Oliver Smith
-
-This file is part of pmbootstrap.
-
-pmbootstrap is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-pmbootstrap is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with pmbootstrap.  If not, see <http://www.gnu.org/licenses/>.
-"""
+# Copyright 2023 Oliver Smith
+# SPDX-License-Identifier: GPL-3.0-or-later
 import logging
 import os
 import glob
 import pmb.helpers.mount
 import pmb.install.losetup
 import pmb.helpers.cli
 import pmb.config
 
 
-def previous_install(args):
+def previous_install(args, path):
     """
-    Search the sdcard for possible existence of a previous installation of pmOS.
-    We temporarily mount the possible pmOS_boot partition as /dev/sdcardp1 inside
-    the native chroot to check the label from there.
+    Search the sdcard for possible existence of a previous installation of
+    pmOS. We temporarily mount the possible pmOS_boot partition as
+    /dev/sdcardp1 inside the native chroot to check the label from there.
+    :param path: path to sdcard device (e.g. /dev/mmcblk0)
     """
     label = ""
-    for blockdevice_outside in [args.sdcard + "1", args.sdcard + "p1"]:
+    for blockdevice_outside in [f"{path}1", f"{path}p1"]:
         if not os.path.exists(blockdevice_outside):
             continue
         blockdevice_inside = "/dev/sdcardp1"
-        pmb.helpers.mount.bind_blockdevice(args, blockdevice_outside,
-                                           args.work + "/chroot_native" + blockdevice_inside)
-        label = pmb.chroot.root(args, ["blkid", "-s", "LABEL", "-o", "value",
-                                       blockdevice_inside], output_return=True)
-        pmb.helpers.run.root(args, ["umount", args.work + "/chroot_native" + blockdevice_inside])
+        pmb.helpers.mount.bind_file(args, blockdevice_outside,
+                                    args.work + '/chroot_native' +
+                                    blockdevice_inside)
+        try:
+            label = pmb.chroot.root(args, ["blkid", "-s", "LABEL",
+                                           "-o", "value",
+                                           blockdevice_inside],
+                                    output_return=True)
+        except RuntimeError:
+            logging.info("WARNING: Could not get block device label,"
+                         " assume no previous installation on that partition")
+
+        pmb.helpers.run.root(args, ["umount", args.work + "/chroot_native" +
+                                    blockdevice_inside])
     return "pmOS_boot" in label
 
 
-def mount_sdcard(args):
+def mount_sdcard(args, path):
+    """
+    :param path: path to sdcard device (e.g. /dev/mmcblk0)
+    """
     # Sanity checks
     if args.deviceinfo["external_storage"] != "true":
         raise RuntimeError("According to the deviceinfo, this device does"
                            " not support a sdcard installation.")
-    if not os.path.exists(args.sdcard):
-        raise RuntimeError("The sdcard device does not exist: " +
-                           args.sdcard)
-    for path in glob.glob(args.sdcard + "*"):
-        if pmb.helpers.mount.ismount(path):
-            raise RuntimeError(path + " is mounted! We will not attempt"
-                               " to format this!")
-    logging.info("(native) mount /dev/install (host: " + args.sdcard + ")")
-    pmb.helpers.mount.bind_blockdevice(args, args.sdcard,
-                                       args.work + "/chroot_native/dev/install")
-    if previous_install(args):
+    if not os.path.exists(path):
+        raise RuntimeError(f"The sdcard device does not exist: {path}")
+    for path_mount in glob.glob(f"{path}*"):
+        if pmb.helpers.mount.ismount(path_mount):
+            raise RuntimeError(f"{path_mount} is mounted! Will not attempt to"
+                               " format this!")
+    logging.info(f"(native) mount /dev/install (host: {path})")
+    pmb.helpers.mount.bind_file(args, path,
+                                args.work + "/chroot_native/dev/install")
+    if previous_install(args, path):
         if not pmb.helpers.cli.confirm(args, "WARNING: This device has a"
                                        " previous installation of pmOS."
                                        " CONTINUE?"):
             raise RuntimeError("Aborted.")
     else:
-        if not pmb.helpers.cli.confirm(args, "EVERYTHING ON " + args.sdcard +
-                                       " WILL BE ERASED! CONTINUE?"):
+        if not pmb.helpers.cli.confirm(args, f"EVERYTHING ON {path} WILL BE"
+                                       " ERASED! CONTINUE?"):
             raise RuntimeError("Aborted.")
 
 
-def create_and_mount_image(args, size_boot, size_root):
+def create_and_mount_image(args, size_boot, size_root, size_reserve,
+                           split=False):
     """
     Create a new image file, and mount it as /dev/install.
 
-    :param size_boot: size of the boot partition in bytes
-    :param size_root: size of the root partition in bytes
+    :param size_boot: size of the boot partition in MiB
+    :param size_root: size of the root partition in MiB
+    :param size_reserve: empty partition between root and boot in MiB (pma#463)
+    :param split: create separate images for boot and root partitions
     """
+
     # Short variables for paths
     chroot = args.work + "/chroot_native"
     img_path_prefix = "/home/pmos/rootfs/" + args.device
     img_path_full = img_path_prefix + ".img"
     img_path_boot = img_path_prefix + "-boot.img"
     img_path_root = img_path_prefix + "-root.img"
 
@@ -89,54 +89,60 @@
         outside = chroot + img_path
         if os.path.exists(outside):
             pmb.helpers.mount.umount_all(args, chroot + "/mnt")
             pmb.install.losetup.umount(args, img_path)
             pmb.chroot.root(args, ["rm", img_path])
 
     # Make sure there is enough free space
-    size_mb = round((size_boot + size_root) / (1024**2))
+    size_mb = round(size_boot + size_reserve + size_root)
     disk_data = os.statvfs(args.work)
     free = round((disk_data.f_bsize * disk_data.f_bavail) / (1024**2))
     if size_mb > free:
-        raise RuntimeError("Not enough free space to create rootfs image! (free: " + str(free) + "M, required: " + str(size_mb) + "M)")
+        raise RuntimeError("Not enough free space to create rootfs image! "
+                           f"(free: {free}M, required: {size_mb}M)")
 
     # Create empty image files
     pmb.chroot.user(args, ["mkdir", "-p", "/home/pmos/rootfs"])
     size_mb_full = str(size_mb) + "M"
-    size_mb_boot = str(round(size_boot / (1024**2))) + "M"
-    size_mb_root = str(round(size_root / (1024**2))) + "M"
+    size_mb_boot = str(round(size_boot)) + "M"
+    size_mb_root = str(round(size_root)) + "M"
     images = {img_path_full: size_mb_full}
-    if args.split:
+    if split:
         images = {img_path_boot: size_mb_boot,
                   img_path_root: size_mb_root}
     for img_path, size_mb in images.items():
-        logging.info("(native) create " + os.path.basename(img_path) + " (" + size_mb + ")")
+        logging.info(f"(native) create {os.path.basename(img_path)} "
+                     f"({size_mb})")
         pmb.chroot.root(args, ["truncate", "-s", size_mb, img_path])
 
     # Mount to /dev/install
     mount_image_paths = {img_path_full: "/dev/install"}
-    if args.split:
+    if split:
         mount_image_paths = {img_path_boot: "/dev/installp1",
                              img_path_root: "/dev/installp2"}
 
     for img_path, mount_point in mount_image_paths.items():
         logging.info("(native) mount " + mount_point +
                      " (" + os.path.basename(img_path) + ")")
         pmb.install.losetup.mount(args, img_path)
         device = pmb.install.losetup.device_by_back_file(args, img_path)
-        pmb.helpers.mount.bind_blockdevice(args, device, args.work +
-                                           "/chroot_native" + mount_point)
+        pmb.helpers.mount.bind_file(args, device,
+                                    args.work + "/chroot_native" + mount_point)
 
 
-def create(args, size_boot, size_root):
+def create(args, size_boot, size_root, size_reserve, split, sdcard):
     """
     Create /dev/install (the "install blockdevice").
 
-    :param size_boot: size of the boot partition in bytes
-    :param size_root: size of the root partition in bytes
+    :param size_boot: size of the boot partition in MiB
+    :param size_root: size of the root partition in MiB
+    :param size_reserve: empty partition between root and boot in MiB (pma#463)
+    :param split: create separate images for boot and root partitions
+    :param sdcard: path to sdcard device (e.g. /dev/mmcblk0) or None
     """
     pmb.helpers.mount.umount_all(
         args, args.work + "/chroot_native/dev/install")
-    if args.sdcard:
-        mount_sdcard(args)
+    if sdcard:
+        mount_sdcard(args, sdcard)
     else:
-        create_and_mount_image(args, size_boot, size_root)
+        create_and_mount_image(args, size_boot, size_root, size_reserve,
+                               split)
```

### Comparing `pmbootstrap-1.9.0/LICENSE` & `pmbootstrap-2.0.0/LICENSE`

 * *Files identical despite different names*

