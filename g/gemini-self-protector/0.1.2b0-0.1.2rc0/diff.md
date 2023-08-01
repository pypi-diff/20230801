# Comparing `tmp/gemini_self_protector-0.1.2b0.tar.gz` & `tmp/gemini_self_protector-0.1.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_self_protector-0.1.2b0.tar", max compression
+gzip compressed data, was "gemini_self_protector-0.1.2rc0.tar", max compression
```

## Comparing `gemini_self_protector-0.1.2b0.tar` & `gemini_self_protector-0.1.2rc0.tar`

### file list

```diff
@@ -1,133 +1,133 @@
--rwxr-xr-x   0        0        0     1069 2023-04-17 13:13:50.672809 gemini_self_protector-0.1.2b0/LICENSE
--rw-r--r--   0        0        0     6700 2023-06-26 14:16:25.914242 gemini_self_protector-0.1.2b0/README.md
--rw-r--r--   0        0        0      491 2023-07-27 17:03:00.404000 gemini_self_protector-0.1.2b0/pyproject.toml
--rw-r--r--   0        0        0      558 2023-06-19 16:47:36.851640 gemini_self_protector-0.1.2b0/src/gemini_self_protector/__init__.py
--rw-r--r--   0        0        0     1824 2023-06-19 16:47:28.845395 gemini_self_protector-0.1.2b0/src/gemini_self_protector/_audit.py
--rw-r--r--   0        0        0     4000 2023-06-19 16:47:22.196160 gemini_self_protector-0.1.2b0/src/gemini_self_protector/_cli.py
--rw-r--r--   0        0        0    13840 2023-07-04 17:18:00.743973 gemini_self_protector-0.1.2b0/src/gemini_self_protector/_config.py
--rw-r--r--   0        0        0    20786 2023-07-12 14:31:35.889747 gemini_self_protector-0.1.2b0/src/gemini_self_protector/_gemini.py
--rw-r--r--   0        0        0    36293 2023-07-21 12:02:49.953482 gemini_self_protector-0.1.2b0/src/gemini_self_protector/_gui.py
--rw-r--r--   0        0        0     2737 2023-06-14 15:41:22.128264 gemini_self_protector-0.1.2b0/src/gemini_self_protector/_logger.py
--rw-r--r--   0        0        0     3508 2023-07-12 14:32:01.923270 gemini_self_protector-0.1.2b0/src/gemini_self_protector/_model.py
--rw-r--r--   0        0        0    14744 2023-07-27 16:31:01.059064 gemini_self_protector-0.1.2b0/src/gemini_self_protector/_protect.py
--rw-r--r--   0        0        0     1667 2023-06-19 16:46:34.460479 gemini_self_protector-0.1.2b0/src/gemini_self_protector/_template.py
--rw-r--r--   0        0        0    16402 2023-07-21 12:08:02.593658 gemini_self_protector-0.1.2b0/src/gemini_self_protector/_utils.py
--rw-r--r--   0        0        0     6391 2023-07-03 17:31:00.908120 gemini_self_protector-0.1.2b0/src/gemini_self_protector/gemini_self_protector.py
--rw-r--r--   0        0        0     3356 2023-06-20 14:32:27.097647 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/css/dark.css
--rw-r--r--   0        0        0     5484 2023-06-19 17:02:55.146292 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/css/install.css
--rw-r--r--   0        0        0   311910 2023-07-04 17:15:39.423308 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/css/style.css
--rw-r--r--   0        0        0     1544 2023-06-19 17:02:55.149256 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/datta/datta-icon.css
--rw-r--r--   0        0        0     2548 2023-06-19 17:02:55.149663 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.eot
--rw-r--r--   0        0        0     2530 2023-06-19 17:02:55.150002 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.svg
--rw-r--r--   0        0        0     2400 2023-06-19 17:02:55.150303 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.ttf
--rw-r--r--   0        0        0     1544 2023-06-19 17:02:55.150704 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.woff
--rw-r--r--   0        0        0    11805 2023-06-19 17:02:55.151201 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/feather/css/feather.css
--rw-r--r--   0        0        0    55828 2023-06-19 17:02:55.152093 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.eot
--rw-r--r--   0        0        0   191595 2023-06-19 17:02:55.154892 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.svg
--rw-r--r--   0        0        0    55664 2023-06-19 17:02:55.156107 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.ttf
--rw-r--r--   0        0        0    26432 2023-06-19 17:02:55.156890 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.woff
--rw-r--r--   0        0        0    41065 2023-06-19 17:02:55.160256 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/css/fontawesome-all.min.css
--rw-r--r--   0        0        0   111620 2023-06-19 17:02:55.162260 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.eot
--rw-r--r--   0        0        0   599834 2023-06-19 17:02:55.169295 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.svg
--rw-r--r--   0        0        0   111384 2023-06-19 17:02:55.171076 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0    71560 2023-06-19 17:02:55.174761 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff
--rw-r--r--   0        0        0    61336 2023-06-19 17:02:55.175547 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    31272 2023-06-19 17:02:55.176292 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.eot
--rw-r--r--   0        0        0   104706 2023-06-19 17:02:55.177586 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.svg
--rw-r--r--   0        0        0    31044 2023-06-19 17:02:55.178645 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    14724 2023-06-19 17:02:55.179411 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff
--rw-r--r--   0        0        0    12188 2023-06-19 17:02:55.179988 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   133140 2023-06-19 17:02:55.181538 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.eot
--rw-r--r--   0        0        0   488395 2023-06-19 17:02:55.190179 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.svg
--rw-r--r--   0        0        0   132920 2023-06-19 17:02:55.194157 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0    63836 2023-06-19 17:02:55.195167 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0        0        0    50372 2023-06-19 17:02:55.204039 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     3822 2023-06-19 17:02:55.204861 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/browser/chrome.png
--rw-r--r--   0        0        0     4809 2023-06-19 17:02:55.205402 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/browser/firefox.png
--rw-r--r--   0        0        0     4359 2023-06-19 17:02:55.205942 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/browser/ie.png
--rw-r--r--   0        0        0     3379 2023-06-19 17:02:55.206498 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/browser/opera.png
--rw-r--r--   0        0        0     4915 2023-06-19 17:02:55.207015 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/browser/safari.png
--rw-r--r--   0        0        0    15406 2023-06-21 08:29:54.000000 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/favicon.ico
--rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/gemini-7.png
--rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/logo-dark.png
--rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/logo-thumb.png
--rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/logo.png
--rw-r--r--   0        0        0    31417 2023-06-19 17:02:55.211234 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img-slide-1.jpg
--rw-r--r--   0        0        0    66369 2023-06-19 17:02:55.212675 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img-slide-2.jpg
--rw-r--r--   0        0        0    22071 2023-06-19 17:02:55.213564 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img-slide-3.jpg
--rw-r--r--   0        0        0    21820 2023-06-19 17:02:55.214458 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img-slide-4.jpg
--rw-r--r--   0        0        0    33652 2023-06-19 17:02:55.215162 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img-slide-5.jpg
--rw-r--r--   0        0        0   246009 2023-06-19 17:02:55.221542 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img1.jpg
--rw-r--r--   0        0        0   165567 2023-06-19 17:02:55.223424 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img2.jpg
--rw-r--r--   0        0        0   168914 2023-06-19 17:02:55.225478 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img3.jpg
--rw-r--r--   0        0        0     9287 2023-06-19 17:02:55.226420 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/avatar-1.jpg
--rw-r--r--   0        0        0     9372 2023-06-19 17:02:55.227034 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/avatar-2.jpg
--rw-r--r--   0        0        0     9408 2023-06-19 17:02:55.227611 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/avatar-3.jpg
--rw-r--r--   0        0        0     8489 2023-06-19 17:02:55.228264 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/avatar-4.jpg
--rw-r--r--   0        0        0     9350 2023-06-19 17:02:55.228810 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/avatar-5.jpg
--rw-r--r--   0        0        0   411771 2023-06-19 17:02:55.233572 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/monkey-man.jpg
--rw-r--r--   0        0        0    42085 2023-06-19 17:02:55.234686 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/profile.jpg
--rw-r--r--   0        0        0     1662 2023-06-19 17:02:55.235481 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/user-1.png
--rw-r--r--   0        0        0     1560 2023-06-19 17:02:55.236026 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/user-2.png
--rw-r--r--   0        0        0    32086 2023-06-22 15:43:25.323112 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/box.png
--rw-r--r--   0        0        0   104704 2023-06-19 17:02:55.237763 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/dashborad-1.png
--rw-r--r--   0        0        0   170223 2023-06-19 17:02:55.238852 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/dashborad-2.png
--rw-r--r--   0        0        0   115557 2023-06-19 17:02:55.240831 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/dashborad-3.png
--rw-r--r--   0        0        0    14068 2023-06-19 17:02:55.241456 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/dashborad-4.png
--rw-r--r--   0        0        0     6239 2023-06-19 17:02:55.242061 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/dashborad-5.png
--rw-r--r--   0        0        0     8193 2023-06-19 17:02:55.245012 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/dashborad-6.png
--rw-r--r--   0        0        0   111459 2023-06-19 17:02:55.245681 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/emoticon.png
--rw-r--r--   0        0        0     2070 2023-06-19 17:02:55.246414 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/js/dark-mode.js
--rw-r--r--   0        0        0    10781 2023-07-12 14:30:13.012279 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/js/install.js
--rw-r--r--   0        0        0     8283 2023-06-20 14:50:28.132874 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/js/pages/chart-morris-custom.js
--rw-r--r--   0        0        0     4186 2023-06-19 17:02:55.248210 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/js/pages/google-maps.js
--rw-r--r--   0        0        0    15246 2023-06-19 17:02:55.248828 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/js/pcoded.min.js
--rw-r--r--   0        0        0   117119 2023-06-19 17:02:55.250050 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/js/vendor-all.min.js
--rw-r--r--   0        0        0   209436 2023-06-19 17:02:55.251932 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/amcharts.js
--rw-r--r--   0        0        0   168766 2023-06-19 17:02:55.253536 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/ammap.min.js
--rw-r--r--   0        0        0    12853 2023-06-19 17:02:55.254172 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/gauge.js
--rw-r--r--   0        0        0      664 2023-06-19 17:02:55.254824 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/dragIconRoundBig.svg
--rw-r--r--   0        0        0      533 2023-06-19 17:02:55.255352 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/lens.svg
--rw-r--r--   0        0        0     2915 2023-06-19 17:02:55.256048 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/light.js
--rw-r--r--   0        0        0    14700 2023-06-19 17:02:55.256659 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/pie.min.js
--rw-r--r--   0        0        0     6464 2023-06-19 17:02:55.260444 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/radar.js
--rw-r--r--   0        0        0    49474 2023-06-19 17:02:55.261308 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/serial.js
--rw-r--r--   0        0        0    30335 2023-06-19 17:02:55.262045 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/usaLow.js
--rw-r--r--   0        0        0   130785 2023-06-19 17:02:55.263354 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/worldLow.js
--rw-r--r--   0        0        0    57902 2023-06-19 17:02:55.264343 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/animation/css/animate.min.css
--rw-r--r--   0        0        0   173477 2023-06-20 14:32:33.510617 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   183849 2023-06-20 14:32:39.581340 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   123727 2023-06-20 14:32:53.377164 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0    57656 2023-06-20 14:33:05.897034 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0    22774 2023-06-20 14:32:56.220296 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/popover.js
--rw-r--r--   0        0        0      433 2023-06-19 17:02:55.269431 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/chart-morris/css/morris.css
--rw-r--r--   0        0        0    35652 2023-06-19 17:02:55.270307 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/morris.min.js
--rw-r--r--   0        0        0    92631 2023-06-19 17:02:55.271715 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/raphael.min.js
--rw-r--r--   0        0        0    45950 2023-06-19 17:02:55.272798 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/google-maps/js/gmaps.js
--rw-r--r--   0        0        0    86927 2023-06-19 17:02:55.274313 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/jquery/js/jquery.min.js
--rw-r--r--   0        0        0     2850 2023-06-19 17:02:55.275041 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css
--rw-r--r--   0        0        0    11662 2023-06-19 17:02:55.275780 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js
--rw-r--r--   0        0        0   461387 2023-06-19 17:02:55.278722 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/jquery-ui/js/jquery-ui.js
--rw-r--r--   0        0        0     7416 2023-06-20 14:30:54.723653 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/toastify/toastify-js.js
--rw-r--r--   0        0        0     1774 2023-06-20 14:34:31.583987 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/toastify/toastify.min.css
--rw-r--r--   0        0        0     3582 2023-06-19 17:02:55.282733 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/scss/dark.scss
--rw-r--r--   0        0        0     2873 2023-06-20 13:40:16.409928 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/accounts/login.html
--rw-r--r--   0        0        0    11196 2023-07-04 17:16:01.979812 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/acl.html
--rw-r--r--   0        0        0    23042 2023-07-21 12:07:10.268507 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/config.html
--rw-r--r--   0        0        0     7827 2023-07-04 17:16:19.165269 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/dependency.html
--rw-r--r--   0        0        0     4563 2023-07-04 17:16:27.724233 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/endpoint.html
--rw-r--r--   0        0        0     5184 2023-07-05 11:53:27.086067 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/feedback.html
--rw-r--r--   0        0        0    32271 2023-07-21 12:20:25.954872 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/index.html
--rw-r--r--   0        0        0      845 2023-06-19 17:02:55.286540 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/page-403.html
--rw-r--r--   0        0        0      846 2023-06-19 17:02:55.287062 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/page-404.html
--rw-r--r--   0        0        0     1130 2023-06-19 17:02:55.287848 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/page-500.html
--rw-r--r--   0        0        0     3050 2023-06-19 17:02:55.288892 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/page-blank.html
--rw-r--r--   0        0        0     8348 2023-06-19 17:02:55.289793 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/profile.html
--rw-r--r--   0        0        0     7700 2023-06-19 17:02:55.291327 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/includes/navigation.html
--rw-r--r--   0        0        0      547 2023-06-19 17:02:55.291941 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/includes/scripts.html
--rw-r--r--   0        0        0     5310 2023-07-12 14:31:09.510236 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/includes/sidebar.html
--rw-r--r--   0        0        0    15819 2023-07-12 14:30:33.367878 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/install.html
--rw-r--r--   0        0        0     1683 2023-07-12 14:31:24.110465 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/key.html
--rw-r--r--   0        0        0     2842 2023-06-19 17:02:55.293834 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/layouts/base-fullscreen.html
--rw-r--r--   0        0        0     2945 2023-06-19 17:02:55.294311 gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/layouts/base.html
--rw-r--r--   0        0        0     7454 1970-01-01 00:00:00.000000 gemini_self_protector-0.1.2b0/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-04-17 13:13:50.672809 gemini_self_protector-0.1.2rc0/LICENSE
+-rw-r--r--   0        0        0     6700 2023-06-26 14:16:25.914242 gemini_self_protector-0.1.2rc0/README.md
+-rw-r--r--   0        0        0      491 2023-08-01 15:44:13.588166 gemini_self_protector-0.1.2rc0/pyproject.toml
+-rw-r--r--   0        0        0      558 2023-06-19 16:47:36.851640 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/__init__.py
+-rw-r--r--   0        0        0     1824 2023-06-19 16:47:28.845395 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_audit.py
+-rw-r--r--   0        0        0     4000 2023-06-19 16:47:22.196160 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_cli.py
+-rw-r--r--   0        0        0    13840 2023-07-04 17:18:00.743973 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_config.py
+-rw-r--r--   0        0        0    20786 2023-07-12 14:31:35.889747 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_gemini.py
+-rw-r--r--   0        0        0    36293 2023-07-21 12:02:49.953482 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_gui.py
+-rw-r--r--   0        0        0     2737 2023-06-14 15:41:22.128264 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_logger.py
+-rw-r--r--   0        0        0     3508 2023-07-12 14:32:01.923270 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_model.py
+-rw-r--r--   0        0        0    14821 2023-08-01 15:42:07.419272 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_protect.py
+-rw-r--r--   0        0        0     1667 2023-06-19 16:46:34.460479 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_template.py
+-rw-r--r--   0        0        0    16852 2023-08-01 15:40:41.704292 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_utils.py
+-rw-r--r--   0        0        0     6391 2023-07-03 17:31:00.908120 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/gemini_self_protector.py
+-rw-r--r--   0        0        0     3356 2023-06-20 14:32:27.097647 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/css/dark.css
+-rw-r--r--   0        0        0     5484 2023-06-19 17:02:55.146292 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/css/install.css
+-rw-r--r--   0        0        0   311910 2023-07-04 17:15:39.423308 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/css/style.css
+-rw-r--r--   0        0        0     1544 2023-06-19 17:02:55.149256 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/datta/datta-icon.css
+-rw-r--r--   0        0        0     2548 2023-06-19 17:02:55.149663 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.eot
+-rw-r--r--   0        0        0     2530 2023-06-19 17:02:55.150002 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.svg
+-rw-r--r--   0        0        0     2400 2023-06-19 17:02:55.150303 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.ttf
+-rw-r--r--   0        0        0     1544 2023-06-19 17:02:55.150704 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.woff
+-rw-r--r--   0        0        0    11805 2023-06-19 17:02:55.151201 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/feather/css/feather.css
+-rw-r--r--   0        0        0    55828 2023-06-19 17:02:55.152093 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.eot
+-rw-r--r--   0        0        0   191595 2023-06-19 17:02:55.154892 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.svg
+-rw-r--r--   0        0        0    55664 2023-06-19 17:02:55.156107 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.ttf
+-rw-r--r--   0        0        0    26432 2023-06-19 17:02:55.156890 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.woff
+-rw-r--r--   0        0        0    41065 2023-06-19 17:02:55.160256 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/css/fontawesome-all.min.css
+-rw-r--r--   0        0        0   111620 2023-06-19 17:02:55.162260 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0        0        0   599834 2023-06-19 17:02:55.169295 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0        0        0   111384 2023-06-19 17:02:55.171076 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0    71560 2023-06-19 17:02:55.174761 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0        0        0    61336 2023-06-19 17:02:55.175547 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    31272 2023-06-19 17:02:55.176292 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0        0        0   104706 2023-06-19 17:02:55.177586 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0        0        0    31044 2023-06-19 17:02:55.178645 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    14724 2023-06-19 17:02:55.179411 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0        0        0    12188 2023-06-19 17:02:55.179988 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   133140 2023-06-19 17:02:55.181538 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0        0        0   488395 2023-06-19 17:02:55.190179 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0        0        0   132920 2023-06-19 17:02:55.194157 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0    63836 2023-06-19 17:02:55.195167 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0        0        0    50372 2023-06-19 17:02:55.204039 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     3822 2023-06-19 17:02:55.204861 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/browser/chrome.png
+-rw-r--r--   0        0        0     4809 2023-06-19 17:02:55.205402 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/browser/firefox.png
+-rw-r--r--   0        0        0     4359 2023-06-19 17:02:55.205942 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/browser/ie.png
+-rw-r--r--   0        0        0     3379 2023-06-19 17:02:55.206498 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/browser/opera.png
+-rw-r--r--   0        0        0     4915 2023-06-19 17:02:55.207015 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/browser/safari.png
+-rw-r--r--   0        0        0    15406 2023-06-21 08:29:54.000000 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/favicon.ico
+-rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/gemini-7.png
+-rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/logo-dark.png
+-rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/logo-thumb.png
+-rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/logo.png
+-rw-r--r--   0        0        0    31417 2023-06-19 17:02:55.211234 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img-slide-1.jpg
+-rw-r--r--   0        0        0    66369 2023-06-19 17:02:55.212675 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img-slide-2.jpg
+-rw-r--r--   0        0        0    22071 2023-06-19 17:02:55.213564 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img-slide-3.jpg
+-rw-r--r--   0        0        0    21820 2023-06-19 17:02:55.214458 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img-slide-4.jpg
+-rw-r--r--   0        0        0    33652 2023-06-19 17:02:55.215162 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img-slide-5.jpg
+-rw-r--r--   0        0        0   246009 2023-06-19 17:02:55.221542 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img1.jpg
+-rw-r--r--   0        0        0   165567 2023-06-19 17:02:55.223424 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img2.jpg
+-rw-r--r--   0        0        0   168914 2023-06-19 17:02:55.225478 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img3.jpg
+-rw-r--r--   0        0        0     9287 2023-06-19 17:02:55.226420 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/avatar-1.jpg
+-rw-r--r--   0        0        0     9372 2023-06-19 17:02:55.227034 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/avatar-2.jpg
+-rw-r--r--   0        0        0     9408 2023-06-19 17:02:55.227611 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/avatar-3.jpg
+-rw-r--r--   0        0        0     8489 2023-06-19 17:02:55.228264 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/avatar-4.jpg
+-rw-r--r--   0        0        0     9350 2023-06-19 17:02:55.228810 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/avatar-5.jpg
+-rw-r--r--   0        0        0   411771 2023-06-19 17:02:55.233572 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/monkey-man.jpg
+-rw-r--r--   0        0        0    42085 2023-06-19 17:02:55.234686 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/profile.jpg
+-rw-r--r--   0        0        0     1662 2023-06-19 17:02:55.235481 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/user-1.png
+-rw-r--r--   0        0        0     1560 2023-06-19 17:02:55.236026 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/user-2.png
+-rw-r--r--   0        0        0    32086 2023-06-22 15:43:25.323112 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/box.png
+-rw-r--r--   0        0        0   104704 2023-06-19 17:02:55.237763 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/dashborad-1.png
+-rw-r--r--   0        0        0   170223 2023-06-19 17:02:55.238852 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/dashborad-2.png
+-rw-r--r--   0        0        0   115557 2023-06-19 17:02:55.240831 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/dashborad-3.png
+-rw-r--r--   0        0        0    14068 2023-06-19 17:02:55.241456 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/dashborad-4.png
+-rw-r--r--   0        0        0     6239 2023-06-19 17:02:55.242061 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/dashborad-5.png
+-rw-r--r--   0        0        0     8193 2023-06-19 17:02:55.245012 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/dashborad-6.png
+-rw-r--r--   0        0        0   111459 2023-06-19 17:02:55.245681 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/emoticon.png
+-rw-r--r--   0        0        0     2070 2023-06-19 17:02:55.246414 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/js/dark-mode.js
+-rw-r--r--   0        0        0    10781 2023-07-12 14:30:13.012279 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/js/install.js
+-rw-r--r--   0        0        0     8283 2023-06-20 14:50:28.132874 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/js/pages/chart-morris-custom.js
+-rw-r--r--   0        0        0     4186 2023-06-19 17:02:55.248210 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/js/pages/google-maps.js
+-rw-r--r--   0        0        0    15246 2023-06-19 17:02:55.248828 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/js/pcoded.min.js
+-rw-r--r--   0        0        0   117119 2023-06-19 17:02:55.250050 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/js/vendor-all.min.js
+-rw-r--r--   0        0        0   209436 2023-06-19 17:02:55.251932 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/amcharts.js
+-rw-r--r--   0        0        0   168766 2023-06-19 17:02:55.253536 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/ammap.min.js
+-rw-r--r--   0        0        0    12853 2023-06-19 17:02:55.254172 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/gauge.js
+-rw-r--r--   0        0        0      664 2023-06-19 17:02:55.254824 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/dragIconRoundBig.svg
+-rw-r--r--   0        0        0      533 2023-06-19 17:02:55.255352 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/lens.svg
+-rw-r--r--   0        0        0     2915 2023-06-19 17:02:55.256048 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/light.js
+-rw-r--r--   0        0        0    14700 2023-06-19 17:02:55.256659 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/pie.min.js
+-rw-r--r--   0        0        0     6464 2023-06-19 17:02:55.260444 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/radar.js
+-rw-r--r--   0        0        0    49474 2023-06-19 17:02:55.261308 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/serial.js
+-rw-r--r--   0        0        0    30335 2023-06-19 17:02:55.262045 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/usaLow.js
+-rw-r--r--   0        0        0   130785 2023-06-19 17:02:55.263354 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/worldLow.js
+-rw-r--r--   0        0        0    57902 2023-06-19 17:02:55.264343 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/animation/css/animate.min.css
+-rw-r--r--   0        0        0   173477 2023-06-20 14:32:33.510617 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   183849 2023-06-20 14:32:39.581340 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   123727 2023-06-20 14:32:53.377164 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0    57656 2023-06-20 14:33:05.897034 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0    22774 2023-06-20 14:32:56.220296 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/popover.js
+-rw-r--r--   0        0        0      433 2023-06-19 17:02:55.269431 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/chart-morris/css/morris.css
+-rw-r--r--   0        0        0    35652 2023-06-19 17:02:55.270307 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/morris.min.js
+-rw-r--r--   0        0        0    92631 2023-06-19 17:02:55.271715 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/raphael.min.js
+-rw-r--r--   0        0        0    45950 2023-06-19 17:02:55.272798 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/google-maps/js/gmaps.js
+-rw-r--r--   0        0        0    86927 2023-06-19 17:02:55.274313 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/jquery/js/jquery.min.js
+-rw-r--r--   0        0        0     2850 2023-06-19 17:02:55.275041 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css
+-rw-r--r--   0        0        0    11662 2023-06-19 17:02:55.275780 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js
+-rw-r--r--   0        0        0   461387 2023-06-19 17:02:55.278722 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/jquery-ui/js/jquery-ui.js
+-rw-r--r--   0        0        0     7416 2023-06-20 14:30:54.723653 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/toastify/toastify-js.js
+-rw-r--r--   0        0        0     1774 2023-06-20 14:34:31.583987 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/toastify/toastify.min.css
+-rw-r--r--   0        0        0     3582 2023-06-19 17:02:55.282733 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/scss/dark.scss
+-rw-r--r--   0        0        0     2873 2023-06-20 13:40:16.409928 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/accounts/login.html
+-rw-r--r--   0        0        0    11196 2023-07-04 17:16:01.979812 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/acl.html
+-rw-r--r--   0        0        0    23042 2023-07-21 12:07:10.268507 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/config.html
+-rw-r--r--   0        0        0     7827 2023-07-04 17:16:19.165269 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/dependency.html
+-rw-r--r--   0        0        0     4563 2023-07-04 17:16:27.724233 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/endpoint.html
+-rw-r--r--   0        0        0     5184 2023-07-05 11:53:27.086067 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/feedback.html
+-rw-r--r--   0        0        0    32271 2023-07-21 12:20:25.954872 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/index.html
+-rw-r--r--   0        0        0      845 2023-06-19 17:02:55.286540 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/page-403.html
+-rw-r--r--   0        0        0      846 2023-06-19 17:02:55.287062 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/page-404.html
+-rw-r--r--   0        0        0     1130 2023-06-19 17:02:55.287848 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/page-500.html
+-rw-r--r--   0        0        0     3050 2023-06-19 17:02:55.288892 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/page-blank.html
+-rw-r--r--   0        0        0     8348 2023-06-19 17:02:55.289793 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/profile.html
+-rw-r--r--   0        0        0     7700 2023-06-19 17:02:55.291327 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/includes/navigation.html
+-rw-r--r--   0        0        0      547 2023-06-19 17:02:55.291941 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/includes/scripts.html
+-rw-r--r--   0        0        0     5310 2023-07-12 14:31:09.510236 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/includes/sidebar.html
+-rw-r--r--   0        0        0    15819 2023-07-12 14:30:33.367878 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/install.html
+-rw-r--r--   0        0        0     1683 2023-07-12 14:31:24.110465 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/key.html
+-rw-r--r--   0        0        0     2842 2023-06-19 17:02:55.293834 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/layouts/base-fullscreen.html
+-rw-r--r--   0        0        0     2945 2023-06-19 17:02:55.294311 gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/layouts/base.html
+-rw-r--r--   0        0        0     7455 1970-01-01 00:00:00.000000 gemini_self_protector-0.1.2rc0/PKG-INFO
```

### Comparing `gemini_self_protector-0.1.2b0/LICENSE` & `gemini_self_protector-0.1.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/README.md` & `gemini_self_protector-0.1.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/__init__.py` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/__init__.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/_audit.py` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_audit.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/_cli.py` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_cli.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/_config.py` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_config.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/_gemini.py` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_gemini.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/_gui.py` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_gui.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/_logger.py` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_logger.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/_model.py` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_model.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/_protect.py` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_protect.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
                 return {"Status": status, "Ticket": _ticket}
             else:
                 logger.error("[x_x] Invalid Protect Mode. Protect mode must be: monitor - protection - off")
                 status = True
                 return {"Status": status}
 
         except Exception as e:
-            logger.error("[x_x] Something went wrong, please check your error message.\n Message - {}".format(e))
+            logger.error("[x_x] Something went wrong, please check your error message.\n Message - {}".format('_Protect.__protect_flask_response__', e))
 
     def __protect_flask_response__(safe_redirect, original_response, gemini_protect_mode) -> None:
         try:
             if int(safe_redirect):
                 _method = request.method
                 _full_path = request.full_path
                 _headers = str(request.headers)
@@ -288,8 +288,8 @@
                     status = True
                     return {"Status": status}
             else:
                 status = True
                 return {"Status": status}
 
         except Exception as e:
-            logger.error("[x_x] Something went wrong, please check your error message.\n Message - {}".format(e))
+            logger.error("[x_x] Something went wrong, please check your error message.\n Message - {}".format('_Protect.__protect_flask_request__', e))
```

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/_template.py` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_template.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/_utils.py` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,91 +12,95 @@
 from ._logger import logger
 from datetime import datetime, timezone
 
 
 class _Utils(object):
 
     def decoder(string):
-        """Decode a string using the specified encoding type."""
+        try:
+            """Decode a string using the specified encoding type."""
 
-        # Remove the invalid escape sequences  - # Remove the backslash
-        string = string.replace('\%', '%').replace(
-            '\\', '').replace('<br/>', '')
-
-        string = string.encode().decode('unicode_escape')
-
-        string = urllib.parse.unquote(string)
-
-        string = html.unescape(string)
-
-        # Use a regular expression to find all base64-encoded segments in the string
-        base64_pattern = r'( |,|;)base64,([A-Za-z0-9+/]*={0,2})'
-
-        # Iterate over the matches and decode the base64-encoded data
-        match = re.search(base64_pattern, string)
-        if match:
-            encoded_string = match.group(2)
-
-            # Try first base64-decode
-            try:
-                decoded_string = base64.b64decode(encoded_string).decode()
-                string = string.replace(encoded_string, decoded_string)
-            except:
-                pass
-
-            # Try second base64-decode
-            try:
-                string = string.replace('\%', '%').replace(
-                    '\\', '').replace('<br/>', '').replace(' ', '')
-                match = re.search(base64_pattern, string)
-
-                if match:
-                    encoded_string = match.group(2)
-                    try:
-                        decoded_string = base64.b64decode(
-                            encoded_string).decode()
-                        string = string.replace(encoded_string, decoded_string)
-                    except:
-                        pass
-            except:
-                pass
-
-        # Use a regular expression to find all url end with .js
-        url_pattern = r'(?:https?://|//).+\.js'
-
-        matches = re.findall(url_pattern, string)
-
-        if matches:
-            for match in matches:
-                # alert('noobpk') - 5dc6f09bb9f90381814ff9fcbfe0a685
-                string = string.replace(
-                    match, ' 5dc6f09bb9f90381814ff9fcbfe0a685')
-
-        # Lowercase string
-        string = string.lower()
-
-        # Use a regular expression to find all query
-        sql_pattern = [
-            r'(select.+)|(select.+(?:from|where|and).+)|(exec.+)'
-            r".*--$"
-        ]
-
-        for pattern in sql_pattern:
-            if re.search(pattern, string, re.IGNORECASE):
+            # Remove the invalid escape sequences  - # Remove the backslash
+            string = string.replace('\%', '%').replace(
+                '\\', '').replace('<br/>', '')
+
+            string = string.encode().decode('unicode_escape')
+
+            string = urllib.parse.unquote(string)
+
+            string = html.unescape(string)
+
+            # Use a regular expression to find all base64-encoded segments in the string
+            base64_pattern = r'( |,|;)base64,([A-Za-z0-9+/]*={0,2})'
+
+            # Iterate over the matches and decode the base64-encoded data
+            match = re.search(base64_pattern, string)
+            if match:
+                encoded_string = match.group(2)
+
+                # Try first base64-decode
+                try:
+                    decoded_string = base64.b64decode(encoded_string).decode()
+                    string = string.replace(encoded_string, decoded_string)
+                except:
+                    pass
+
+                # Try second base64-decode
+                try:
+                    string = string.replace('\%', '%').replace(
+                        '\\', '').replace('<br/>', '').replace(' ', '')
+                    match = re.search(base64_pattern, string)
+
+                    if match:
+                        encoded_string = match.group(2)
+                        try:
+                            decoded_string = base64.b64decode(
+                                encoded_string).decode()
+                            string = string.replace(encoded_string, decoded_string)
+                        except:
+                            pass
+                except:
+                    pass
+
+            # Use a regular expression to find all url end with .js
+            url_pattern = r'(?:https?://|//).+\.js'
+
+            matches = re.findall(url_pattern, string)
+
+            if matches:
+                for match in matches:
+                    # alert('noobpk') - 5dc6f09bb9f90381814ff9fcbfe0a685
+                    string = string.replace(
+                        match, ' 5dc6f09bb9f90381814ff9fcbfe0a685')
+
+            # Lowercase string
+            string = string.lower()
+
+            # Use a regular expression to find all query
+            sql_pattern = [
+                r'(select.+)|(select.+(?:from|where|and).+)|(exec.+)'
+                r".*--$"
+            ]
+
+            for pattern in sql_pattern:
+                match = re.search(pattern, string, re.IGNORECASE)
+                if match is not None:
                 # select * from noobpk; - 90e87fc8ba835e0d2bfeec5e3799ecfe
-                string = string.replace(
-                    match[0], ' 90e87fc8ba835e0d2bfeec5e3799ecfe')
-                break
+                    string = string.replace(match[0], ' 90e87fc8ba835e0d2bfeec5e3799ecfe')
+                    break
 
-        string = string.encode('utf-7').decode()
+            string = string.encode('utf-7').decode()
 
-        # Lowercase string
-        string = string.lower()
+            # Lowercase string
+            string = string.lower()
 
-        return string
+            return string
+        except Exception as e:
+            logger.error(
+                "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Utils.decoder', e))
 
     def web_vuln_detect_predict(payload) -> None:
         """
         It takes a payload as input and returns the accuracy of the prediction
 
         :param payload: The payload is the data that you want to send to the API. In this case, it's the
         data that you want to predict
```

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/gemini_self_protector.py` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/gemini_self_protector.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/css/dark.css` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/css/dark.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/css/install.css` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/css/install.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/css/style.css` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/datta/datta-icon.css` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/datta/datta-icon.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.eot` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.svg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.ttf` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.woff` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/feather/css/feather.css` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/feather/css/feather.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.eot` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.svg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.ttf` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.woff` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/css/fontawesome-all.min.css` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/css/fontawesome-all.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.eot` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.svg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.eot` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.svg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.eot` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.svg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/browser/chrome.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/browser/chrome.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/browser/firefox.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/browser/firefox.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/browser/ie.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/browser/ie.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/browser/opera.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/browser/opera.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/browser/safari.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/browser/safari.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/favicon.ico` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/gemini-7.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/gemini-7.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/logo-dark.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/logo-dark.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/logo-thumb.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/logo-thumb.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/logo.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img-slide-1.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img-slide-1.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img-slide-2.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img-slide-2.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img-slide-3.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img-slide-3.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img-slide-4.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img-slide-4.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img-slide-5.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img-slide-5.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img1.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img1.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img2.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img2.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/slider/img3.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/slider/img3.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/avatar-1.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/avatar-1.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/avatar-2.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/avatar-2.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/avatar-3.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/avatar-3.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/avatar-4.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/avatar-4.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/avatar-5.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/avatar-5.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/monkey-man.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/monkey-man.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/profile.jpg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/profile.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/user-1.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/user-1.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/user/user-2.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/user/user-2.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/box.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/box.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/dashborad-1.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/dashborad-1.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/dashborad-2.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/dashborad-2.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/dashborad-3.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/dashborad-3.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/dashborad-4.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/dashborad-4.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/dashborad-5.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/dashborad-5.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/dashborad-6.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/dashborad-6.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/images/widget/emoticon.png` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/images/widget/emoticon.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/js/dark-mode.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/js/dark-mode.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/js/install.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/js/install.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/js/pages/chart-morris-custom.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/js/pages/chart-morris-custom.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/js/pages/google-maps.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/js/pages/google-maps.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/js/pcoded.min.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/js/pcoded.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/js/vendor-all.min.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/js/vendor-all.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/amcharts.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/amcharts.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/ammap.min.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/ammap.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/gauge.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/gauge.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/dragIconRoundBig.svg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/dragIconRoundBig.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/lens.svg` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/lens.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/light.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/light.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/pie.min.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/pie.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/radar.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/radar.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/serial.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/serial.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/usaLow.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/usaLow.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/amchart/js/worldLow.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/amchart/js/worldLow.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/animation/css/animate.min.css` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/animation/css/animate.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.css` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.min.css` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.min.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/popover.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/popover.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/morris.min.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/morris.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/raphael.min.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/raphael.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/google-maps/js/gmaps.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/google-maps/js/gmaps.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/jquery/js/jquery.min.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/jquery/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/jquery-ui/js/jquery-ui.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/jquery-ui/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/toastify/toastify-js.js` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/toastify/toastify-js.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/plugins/toastify/toastify.min.css` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/plugins/toastify/toastify.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/assets/scss/dark.scss` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/assets/scss/dark.scss`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/accounts/login.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/accounts/login.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/acl.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/acl.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/config.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/config.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/dependency.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/dependency.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/endpoint.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/endpoint.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/feedback.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/feedback.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/index.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/index.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/page-403.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/page-403.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/page-404.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/page-404.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/page-500.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/page-500.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/page-blank.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/page-blank.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/home/profile.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/home/profile.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/includes/navigation.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/includes/navigation.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/includes/scripts.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/includes/scripts.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/includes/sidebar.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/includes/sidebar.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/install.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/install.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/key.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/key.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/layouts/base-fullscreen.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/layouts/base-fullscreen.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/src/gemini_self_protector/resource/templates/layouts/base.html` & `gemini_self_protector-0.1.2rc0/src/gemini_self_protector/resource/templates/layouts/base.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2b0/PKG-INFO` & `gemini_self_protector-0.1.2rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-self-protector
-Version: 0.1.2b0
+Version: 0.1.2rc0
 Summary: Runtime Application Self-Protection
 License: MIT
 Author: lethanhphuc
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

