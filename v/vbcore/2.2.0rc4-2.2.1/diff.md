# Comparing `tmp/vbcore-2.2.0rc4.tar.gz` & `tmp/vbcore-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbcore-2.2.0rc4.tar", last modified: Fri Jul  7 00:26:26 2023, max compression
+gzip compressed data, was "vbcore-2.2.1.tar", last modified: Tue Aug  1 00:16:01 2023, max compression
```

## Comparing `vbcore-2.2.0rc4.tar` & `vbcore-2.2.1.tar`

### file list

```diff
@@ -1,210 +1,216 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.806605 vbcore-2.2.0rc4/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      402 2023-07-07 00:26:26.806605 vbcore-2.2.0rc4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.779605 vbcore-2.2.0rc4/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-all.in
--rw-rw-rw-   0 root         (0) root         (0)     5164 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-all.txt
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-build.in
--rw-rw-rw-   0 root         (0) root         (0)     2093 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-build.txt
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-crypto.in
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-crypto.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-db.in
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-db.txt
--rw-rw-rw-   0 root         (0) root         (0)      384 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-dev.in
--rw-rw-rw-   0 root         (0) root         (0)     5233 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-extra.in
--rw-rw-rw-   0 root         (0) root         (0)     1404 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-extra.txt
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-http.in
--rw-rw-rw-   0 root         (0) root         (0)     1142 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-http.txt
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-net.in
--rw-rw-rw-   0 root         (0) root         (0)      736 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-net.txt
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-scheduler.in
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-scheduler.txt
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-test.in
--rw-rw-rw-   0 root         (0) root         (0)     1755 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/requirements/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-07 00:26:26.806605 vbcore-2.2.0rc4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4745 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.783605 vbcore-2.2.0rc4/vbcore/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1686 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/aio.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7746 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/configurator.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.786605 vbcore-2.2.0rc4/vbcore/crypto/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1266 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/argon.py
--rw-rw-rw-   0 root         (0) root         (0)      942 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/bcrypt.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/crypto/hashes.py
--rw-rw-rw-   0 root         (0) root         (0)     4635 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/csvfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.786605 vbcore-2.2.0rc4/vbcore/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.786605 vbcore-2.2.0rc4/vbcore/data/transformations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.788605 vbcore-2.2.0rc4/vbcore/data/transformations/builders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2026 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/csv.py
--rw-rw-rw-   0 root         (0) root         (0)     5586 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/dicttoxml.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     5880 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/html.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2230 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/xml.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/data/transformations/builders/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.789605 vbcore-2.2.0rc4/vbcore/datastruct/
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/buffer.py
--rw-rw-rw-   0 root         (0) root         (0)     6158 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     2904 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/dictionaries.py
--rw-rw-rw-   0 root         (0) root         (0)     2772 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/lazy.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/datastruct/orderer_set.py
--rw-rw-rw-   0 root         (0) root         (0)     4354 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/date_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.791605 vbcore-2.2.0rc4/vbcore/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15840 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/events.py
--rw-rw-rw-   0 root         (0) root         (0)     4935 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/listener.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     6774 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/mysql_dumper.py
--rw-rw-rw-   0 root         (0) root         (0)     1905 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4942 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/sqla.py
--rw-rw-rw-   0 root         (0) root         (0)     5600 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/support.py
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/db/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.791605 vbcore-2.2.0rc4/vbcore/dictutils/
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/dictutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15787 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/dictutils/flatter_dict.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/dictutils/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/enums.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.792605 vbcore-2.2.0rc4/vbcore/excel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/excel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6661 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/excel/report.py
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.794605 vbcore-2.2.0rc4/vbcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2863 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     8112 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3880 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/gql.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/headers.py
--rw-rw-rw-   0 root         (0) root         (0)     2632 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/httpcode.py
--rw-rw-rw-   0 root         (0) root         (0)     4012 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/httpdumper.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/methods.py
--rw-rw-rw-   0 root         (0) root         (0)     6063 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/rpc.py
--rw-rw-rw-   0 root         (0) root         (0)     2143 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/http/useragent.py
--rw-rw-rw-   0 root         (0) root         (0)     4590 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/importer.py
--rw-rw-rw-   0 root         (0) root         (0)     5279 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.794605 vbcore-2.2.0rc4/vbcore/jsonschema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/jsonschema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.794605 vbcore-2.2.0rc4/vbcore/jsonschema/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/jsonschema/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2118 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/jsonschema/schemas/jsonrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7052 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/jsonschema/support.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/lambdas.py
--rw-rw-rw-   0 root         (0) root         (0)     6516 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/loggers.py
--rw-rw-rw-   0 root         (0) root         (0)     5173 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.795605 vbcore-2.2.0rc4/vbcore/net/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.795605 vbcore-2.2.0rc4/vbcore/net/ftpclient/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/ftpclient/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/ftpclient/legacy.py
--rw-rw-rw-   0 root         (0) root         (0)     6132 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/ftpclient/sftp.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     5363 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/sendmail.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/net/socks_smtp.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.796605 vbcore-2.2.0rc4/vbcore/rule_engine/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/rule_engine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/rule_engine/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3171 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/rule_engine/engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.796605 vbcore-2.2.0rc4/vbcore/standalone/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/standalone/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3309 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/standalone/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     8327 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/standalone/wsgi_gunicorn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.797605 vbcore-2.2.0rc4/vbcore/stringutils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/stringutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1226 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/stringutils/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     2158 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/stringutils/notations.py
--rw-rw-rw-   0 root         (0) root         (0)     4449 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.798605 vbcore-2.2.0rc4/vbcore/tester/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16074 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/asserter.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/fetchmail.py
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     7405 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.798605 vbcore-2.2.0rc4/vbcore/tester/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/plugins/fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tester/plugins/startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.800605 vbcore-2.2.0rc4/vbcore/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6170 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/crypto.py
--rw-rw-rw-   0 root         (0) root         (0)     2111 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/database.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/entrypoint.py
--rw-rw-rw-   0 root         (0) root         (0)     3333 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/ftpclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.800605 vbcore-2.2.0rc4/vbcore/tools/initializer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.803605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.bumpversion.cfg
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.editorconfig
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.flake8
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.803605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.git-hooks/
--rwxrwxrwx   0 root         (0) root         (0)      179 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.git-hooks/pre-commit
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.git-hooks/pre-push
--rw-rw-rw-   0 root         (0) root         (0)     2205 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    16254 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4464 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.803605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     2091 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.804605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/scripts/build.sh
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/scripts/dist-publish.sh
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/scripts/fresh-install.sh
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/scripts/test-builds.sh
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/liccheck.ini
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.805605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/requirements/requirements-build.in
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/requirements/requirements-dev.in
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/requirements/requirements-test.in
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     3738 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.805605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/skel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/skel/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.805605 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/skel/entrypoints/
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/skel/entrypoints/main.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/skel/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/skel/version.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/tox.ini
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/sendmail.py
--rw-rw-rw-   0 root         (0) root         (0)     1865 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/tools/wsgi_gunicorn.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/types.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/version.py
--rw-rw-rw-   0 root         (0) root         (0)     2853 2023-07-07 00:26:15.000000 vbcore-2.2.0rc4/vbcore/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 00:26:26.785605 vbcore-2.2.0rc4/vbcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      402 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5585 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      576 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-07 00:26:26.000000 vbcore-2.2.0rc4/vbcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.545009 vbcore-2.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-08-01 00:15:50.000000 vbcore-2.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      399 2023-08-01 00:16:01.545009 vbcore-2.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-08-01 00:15:50.000000 vbcore-2.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.519008 vbcore-2.2.1/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-all.in
+-rw-rw-rw-   0 root         (0) root         (0)     5389 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-all.txt
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-crypto.in
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-crypto.txt
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-db.in
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-db.txt
+-rw-rw-rw-   0 root         (0) root         (0)      384 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)     5233 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      122 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-extra.in
+-rw-rw-rw-   0 root         (0) root         (0)     1597 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-extra.txt
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-http.in
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-http.txt
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-net.in
+-rw-rw-rw-   0 root         (0) root         (0)      736 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-net.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-scheduler.in
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-scheduler.txt
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-08-01 00:15:50.000000 vbcore-2.2.1/requirements/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 00:16:01.545009 vbcore-2.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2023-08-01 00:15:50.000000 vbcore-2.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.523008 vbcore-2.2.1/vbcore/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7714 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/configurator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.525009 vbcore-2.2.1/vbcore/crypto/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/crypto/argon.py
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/crypto/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/crypto/bcrypt.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/crypto/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/crypto/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/crypto/hashes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4571 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/csvfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.525009 vbcore-2.2.1/vbcore/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.525009 vbcore-2.2.1/vbcore/data/transformations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/data/transformations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.526008 vbcore-2.2.1/vbcore/data/transformations/builders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/data/transformations/builders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/data/transformations/builders/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/data/transformations/builders/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     5512 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/data/transformations/builders/dicttoxml.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/data/transformations/builders/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5834 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/data/transformations/builders/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/data/transformations/builders/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/data/transformations/builders/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/data/transformations/builders/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.528009 vbcore-2.2.1/vbcore/datastruct/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/datastruct/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/datastruct/buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6158 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/datastruct/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2904 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/datastruct/dictionaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2746 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/datastruct/lazy.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/datastruct/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/datastruct/orderer_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     4312 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/date_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.529008 vbcore-2.2.1/vbcore/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15748 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     2955 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     6730 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/mysql_dumper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/repo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.530009 vbcore-2.2.1/vbcore/db/schema_display/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/schema_display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13014 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/schema_display/db_diagram.py
+-rw-rw-rw-   0 root         (0) root         (0)     7938 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/schema_display/model_diagram.py
+-rw-rw-rw-   0 root         (0) root         (0)     4954 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/sqla.py
+-rw-rw-rw-   0 root         (0) root         (0)     5558 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/support.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/db/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.530009 vbcore-2.2.1/vbcore/dictutils/
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/dictutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15749 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/dictutils/flatter_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/dictutils/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/enums.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.531009 vbcore-2.2.1/vbcore/excel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/excel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6661 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/excel/report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3827 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.533008 vbcore-2.2.1/vbcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/http/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     8046 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/http/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/http/gql.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/http/headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2632 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/http/httpcode.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/http/httpdumper.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/http/methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6049 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/http/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/http/rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/http/useragent.py
+-rw-rw-rw-   0 root         (0) root         (0)     4590 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5279 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.533008 vbcore-2.2.1/vbcore/jsonschema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/jsonschema/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.533008 vbcore-2.2.1/vbcore/jsonschema/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/jsonschema/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2118 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/jsonschema/schemas/jsonrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     6964 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/jsonschema/support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2527 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/lambdas.py
+-rw-rw-rw-   0 root         (0) root         (0)     6500 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/loggers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5173 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.534009 vbcore-2.2.1/vbcore/net/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/net/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.534009 vbcore-2.2.1/vbcore/net/ftpclient/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/net/ftpclient/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2349 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/net/ftpclient/legacy.py
+-rw-rw-rw-   0 root         (0) root         (0)     6110 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/net/ftpclient/sftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/net/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5325 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/net/sendmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1552 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/net/socks_smtp.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.535009 vbcore-2.2.1/vbcore/rule_engine/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/rule_engine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/rule_engine/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3157 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/rule_engine/engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.535009 vbcore-2.2.1/vbcore/standalone/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/standalone/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3287 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/standalone/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     8203 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/standalone/wsgi_gunicorn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.535009 vbcore-2.2.1/vbcore/stringutils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/stringutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/stringutils/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2158 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/stringutils/notations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4449 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.536008 vbcore-2.2.1/vbcore/tester/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tester/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15948 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tester/asserter.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tester/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tester/fetchmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tester/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7333 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tester/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.537009 vbcore-2.2.1/vbcore/tester/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tester/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tester/plugins/fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tester/plugins/startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.539008 vbcore-2.2.1/vbcore/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6114 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)     2106 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3651 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/ftpclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.539008 vbcore-2.2.1/vbcore/tools/initializer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.542008 vbcore-2.2.1/vbcore/tools/initializer/skeleton/
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/.bumpversion.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/.flake8
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.542008 vbcore-2.2.1/vbcore/tools/initializer/skeleton/.git-hooks/
+-rwxrwxrwx   0 root         (0) root         (0)      179 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/.git-hooks/pre-commit
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/.git-hooks/pre-push
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    16254 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4464 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.543008 vbcore-2.2.1/vbcore/tools/initializer/skeleton/devops/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/devops/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.544009 vbcore-2.2.1/vbcore/tools/initializer/skeleton/devops/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/devops/scripts/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/devops/scripts/dist-publish.sh
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/devops/scripts/fresh-install.sh
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/devops/scripts/test-builds.sh
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/liccheck.ini
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.544009 vbcore-2.2.1/vbcore/tools/initializer/skeleton/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.545009 vbcore-2.2.1/vbcore/tools/initializer/skeleton/skel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/skel/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.545009 vbcore-2.2.1/vbcore/tools/initializer/skeleton/skel/entrypoints/
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/skel/entrypoints/main.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/skel/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/skel/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/initializer/skeleton/tox.ini
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/sendmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1865 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/tools/wsgi_gunicorn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2853 2023-08-01 00:15:50.000000 vbcore-2.2.1/vbcore/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 00:16:01.524009 vbcore-2.2.1/vbcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-08-01 00:16:01.000000 vbcore-2.2.1/vbcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-08-01 00:16:01.000000 vbcore-2.2.1/vbcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:16:01.000000 vbcore-2.2.1/vbcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-08-01 00:16:01.000000 vbcore-2.2.1/vbcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 00:16:01.000000 vbcore-2.2.1/vbcore.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      556 2023-08-01 00:16:01.000000 vbcore-2.2.1/vbcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-01 00:16:01.000000 vbcore-2.2.1/vbcore.egg-info/top_level.txt
```

### Comparing `vbcore-2.2.0rc4/requirements/requirements-all.txt` & `vbcore-2.2.1/requirements/requirements-all.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     #   aiohttp
 attrs==23.1.0
     # via
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements-http.txt
     #   aiohttp
     #   jsonschema
+    #   referencing
 backoff==2.2.1
     # via
     #   -r requirements/requirements-extra.txt
     #   gql
 bcrypt==4.0.1
     # via
     #   -r requirements/requirements-crypto.txt
@@ -53,15 +54,15 @@
 chardet==5.1.0
     # via -r requirements/requirements-extra.txt
 charset-normalizer==2.1.1
     # via
     #   -r requirements/requirements-http.txt
     #   aiohttp
     #   requests
-click==8.1.3
+click==8.1.4
     # via -r requirements/requirements.txt
 cryptography==41.0.1
     # via
     #   -r requirements/requirements-net.txt
     #   paramiko
 defusedxml==0.7.1
     # via -r requirements/requirements-extra.txt
@@ -76,28 +77,34 @@
     #   aiosignal
 gql==3.4.1
     # via -r requirements/requirements-extra.txt
 graphql-core==3.2.3
     # via
     #   -r requirements/requirements-extra.txt
     #   gql
+graphviz==0.20.1
+    # via -r requirements/requirements-db.txt
 greenlet==2.0.2
     # via
     #   -r requirements/requirements-db.txt
     #   sqlalchemy
 gunicorn==20.1.0
     # via -r requirements/requirements-extra.txt
 idna==3.4
     # via
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements-http.txt
     #   requests
     #   yarl
-jsonschema==4.17.3
+jsonschema==4.18.0
     # via -r requirements/requirements-extra.txt
+jsonschema-specifications==2023.6.1
+    # via
+    #   -r requirements/requirements-extra.txt
+    #   jsonschema
 multidict==6.0.4
     # via
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements-http.txt
     #   aiohttp
     #   yarl
 openpyxl==3.1.2
@@ -112,29 +119,23 @@
     # via -r requirements/requirements.txt
 pycparser==2.21
     # via
     #   -r requirements/requirements-crypto.txt
     #   -r requirements/requirements-net.txt
     #   cffi
 pydot==1.4.2
-    # via
-    #   -r requirements/requirements-db.txt
-    #   sqlalchemy-schemadisplay
+    # via -r requirements/requirements-db.txt
 pynacl==1.5.0
     # via
     #   -r requirements/requirements-net.txt
     #   paramiko
 pyparsing==3.1.0
     # via
     #   -r requirements/requirements-db.txt
     #   pydot
-pyrsistent==0.19.3
-    # via
-    #   -r requirements/requirements-extra.txt
-    #   jsonschema
 pysocks==1.7.1
     # via -r requirements/requirements-net.txt
 python-dateutil==2.8.2
     # via
     #   -r requirements/requirements-extra.txt
     #   -r requirements/requirements.txt
     #   bson
@@ -145,38 +146,46 @@
     # via -r requirements/requirements.txt
 pytz==2023.3
     # via
     #   -r requirements/requirements-scheduler.txt
     #   apscheduler
 pyyaml==6.0
     # via -r requirements/requirements.txt
+referencing==0.29.1
+    # via
+    #   -r requirements/requirements-extra.txt
+    #   jsonschema
+    #   jsonschema-specifications
 requests==2.31.0
     # via -r requirements/requirements-http.txt
+rpds-py==0.8.10
+    # via
+    #   -r requirements/requirements-extra.txt
+    #   jsonschema
+    #   referencing
 rule-engine==3.6.0
     # via -r requirements/requirements-extra.txt
 six==1.16.0
     # via
     #   -r requirements/requirements-scheduler.txt
     #   -r requirements/requirements.txt
     #   apscheduler
     #   bson
     #   python-dateutil
-sqlalchemy==2.0.17
-    # via -r requirements/requirements-db.txt
-sqlalchemy-schemadisplay==1.3
+sqlalchemy==2.0.18
     # via -r requirements/requirements-db.txt
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   -r requirements/requirements-db.txt
     #   sqlalchemy
 tzlocal==5.0.1
     # via
     #   -r requirements/requirements-scheduler.txt
     #   apscheduler
-ua-parser==0.16.1
+ua-parser==0.18.0
     # via
     #   -r requirements/requirements-http.txt
     #   user-agents
 urllib3==2.0.3
     # via
     #   -r requirements/requirements-http.txt
     #   requests
```

### Comparing `vbcore-2.2.0rc4/requirements/requirements-build.txt` & `vbcore-2.2.1/requirements/requirements-build.txt`

 * *Files 7% similar despite different names*

```diff
@@ -28,19 +28,19 @@
     # via readme-renderer
 filelock==3.12.2
     # via
     #   tox
     #   virtualenv
 idna==3.4
     # via requests
-importlib-metadata==6.7.0
+importlib-metadata==6.8.0
     # via
     #   keyring
     #   twine
-jaraco-classes==3.2.3
+jaraco-classes==3.3.0
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 keyring==24.2.0
     # via twine
@@ -52,27 +52,27 @@
     # via jaraco-classes
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
 pkginfo==1.9.6
     # via twine
-platformdirs==3.8.0
+platformdirs==3.8.1
     # via
     #   tox
     #   virtualenv
 pluggy==1.2.0
     # via tox
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
-pyproject-api==1.5.2
+pyproject-api==1.5.3
     # via tox
 readme-renderer==40.0
     # via twine
 requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
@@ -86,23 +86,23 @@
     # via keyring
 six==1.16.0
     # via bleach
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.6.3
+tox==4.6.4
     # via -r requirements/requirements-build.in
 twine==4.0.2
     # via -r requirements/requirements-build.in
 urllib3==2.0.3
     # via
     #   requests
     #   twine
 virtualenv==20.23.1
     # via tox
 webencodings==0.5.1
     # via bleach
 wheel==0.40.0
     # via -r requirements/requirements-build.in
-zipp==3.15.0
+zipp==3.16.0
     # via importlib-metadata
```

### Comparing `vbcore-2.2.0rc4/requirements/requirements-crypto.txt` & `vbcore-2.2.1/requirements/requirements-crypto.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/requirements/requirements-dev.txt` & `vbcore-2.2.1/requirements/requirements-dev.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-dev.txt --resolver=backtracking requirements/requirements-dev.in
 #
-astroid==2.15.5
+astroid==2.15.6
     # via pylint
 attrs==23.1.0
     # via
     #   -c requirements/requirements-test.txt
     #   flake8-bugbear
 autoflake==2.2.0
     # via -r requirements/requirements-dev.in
@@ -28,27 +28,27 @@
     # via
     #   -c requirements/requirements-build.txt
     #   cryptography
 charset-normalizer==2.1.1
     # via
     #   -c requirements/requirements-test.txt
     #   requests
-click==8.1.3
+click==8.1.4
     # via
     #   -c requirements/requirements-all.txt
     #   black
     #   pip-tools
     #   safety
 colorama==0.4.6
     # via
     #   -c requirements/requirements-build.txt
     #   radon
 coloredlogs==15.0.1
     # via -r requirements/requirements-dev.in
-configparser==5.3.0
+configparser==6.0.0
     # via liccheck
 cryptography==41.0.1
     # via
     #   -c requirements/requirements-build.txt
     #   types-paramiko
 dill==0.3.6
     # via pylint
@@ -107,17 +107,17 @@
     #   safety
 pathspec==0.11.1
     # via black
 pbr==5.11.1
     # via stevedore
 pip-tools==6.14.0
     # via -r requirements/requirements-dev.in
-pipdeptree==2.9.3
+pipdeptree==2.9.4
     # via -r requirements/requirements-dev.in
-platformdirs==3.8.0
+platformdirs==3.8.1
     # via
     #   -c requirements/requirements-build.txt
     #   black
     #   pylint
 pycodestyle==2.10.0
     # via flake8
 pycparser==2.21
@@ -191,23 +191,23 @@
     # via -r requirements/requirements-dev.in
 types-pytz==2023.3.0.0
     # via -r requirements/requirements-dev.in
 types-pyyaml==6.0.12.10
     # via -r requirements/requirements-dev.in
 types-requests==2.31.0.1
     # via -r requirements/requirements-dev.in
-types-setuptools==68.0.0.0
+types-setuptools==68.0.0.1
     # via -r requirements/requirements-dev.in
 types-toml==0.10.8.6
     # via -r requirements/requirements-dev.in
 types-urllib3==1.26.25.13
     # via types-requests
 types-xmltodict==0.13.0.2
     # via -r requirements/requirements-dev.in
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   -c requirements/requirements-all.txt
     #   astroid
     #   mypy
 urllib3==2.0.3
     # via
     #   -c requirements/requirements-test.txt
```

### Comparing `vbcore-2.2.0rc4/requirements/requirements-extra.txt` & `vbcore-2.2.1/requirements/requirements-extra.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements-extra.txt --resolver=backtracking requirements/requirements-extra.in
 #
 attrs==23.1.0
-    # via jsonschema
+    # via
+    #   jsonschema
+    #   referencing
 backoff==2.2.1
     # via gql
 chardet==5.1.0
     # via -r requirements/requirements-extra.in
 defusedxml==0.7.1
     # via -r requirements/requirements-extra.in
 et-xmlfile==1.1.0
@@ -20,28 +22,36 @@
     # via gql
 gunicorn==20.1.0
     # via -r requirements/requirements-extra.in
 idna==3.4
     # via
     #   -c requirements/requirements-build.txt
     #   yarl
-jsonschema==4.17.3
+jsonschema==4.18.0
     # via -r requirements/requirements-extra.in
+jsonschema-specifications==2023.6.1
+    # via jsonschema
 multidict==6.0.4
     # via yarl
 openpyxl==3.1.2
     # via -r requirements/requirements-extra.in
 ply==3.11
     # via rule-engine
-pyrsistent==0.19.3
-    # via jsonschema
 python-dateutil==2.8.2
     # via
     #   -c requirements/requirements.txt
     #   rule-engine
+referencing==0.29.1
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+rpds-py==0.8.10
+    # via
+    #   jsonschema
+    #   referencing
 rule-engine==3.6.0
     # via -r requirements/requirements-extra.in
 six==1.16.0
     # via
     #   -c requirements/requirements-build.txt
     #   python-dateutil
 xmltodict==0.13.0
```

### Comparing `vbcore-2.2.0rc4/requirements/requirements-http.txt` & `vbcore-2.2.1/requirements/requirements-http.txt`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     #   yarl
 multidict==6.0.4
     # via
     #   aiohttp
     #   yarl
 requests==2.31.0
     # via -r requirements/requirements-http.in
-ua-parser==0.16.1
+ua-parser==0.18.0
     # via user-agents
 urllib3==2.0.3
     # via
     #   -c requirements/requirements-build.txt
     #   requests
 user-agents==2.2.0
     # via -r requirements/requirements-http.in
```

### Comparing `vbcore-2.2.0rc4/requirements/requirements-net.txt` & `vbcore-2.2.1/requirements/requirements-net.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/requirements/requirements-scheduler.txt` & `vbcore-2.2.1/requirements/requirements-scheduler.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/requirements/requirements-test.txt` & `vbcore-2.2.1/requirements/requirements-test.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     # via
     #   -c requirements/requirements-build.txt
     #   requests
 coverage[toml]==7.2.7
     # via
     #   -r requirements/requirements-test.in
     #   pytest-cov
-exceptiongroup==1.1.1
+exceptiongroup==1.1.2
     # via
     #   hypothesis
     #   pytest
-hypothesis==6.80.0
+hypothesis==6.80.1
     # via -r requirements/requirements-test.in
 idna==3.4
     # via
     #   -c requirements/requirements-build.txt
     #   requests
 iniconfig==2.0.0
     # via pytest
```

### Comparing `vbcore-2.2.0rc4/requirements/requirements.txt` & `vbcore-2.2.1/requirements/requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --no-emit-index-url --no-emit-trusted-host --output-file=requirements/requirements.txt --resolver=backtracking requirements/requirements.in
 #
 bson==0.5.10
     # via -r requirements/requirements.in
-click==8.1.3
+click==8.1.4
     # via -r requirements/requirements.in
 psutil==5.9.5
     # via -r requirements/requirements.in
 python-dateutil==2.8.2
     # via
     #   -r requirements/requirements.in
     #   bson
```

### Comparing `vbcore-2.2.0rc4/setup.py` & `vbcore-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,17 +127,15 @@
 install_requires = read_requirements(os.path.join(REQ_PATH, "requirements.in"))
 tests_requires = read_requirements(os.path.join(REQ_PATH, "requirements-test.in"))
 db_requires = read_requirements(os.path.join(REQ_PATH, "requirements-db.in"))
 crypto_requires = read_requirements(os.path.join(REQ_PATH, "requirements-crypto.in"))
 http_requires = read_requirements(os.path.join(REQ_PATH, "requirements-http.in"))
 net_requires = read_requirements(os.path.join(REQ_PATH, "requirements-net.in"))
 extra_requires = read_requirements(os.path.join(REQ_PATH, "requirements-extra.in"))
-scheduler_requires = read_requirements(
-    os.path.join(REQ_PATH, "requirements-scheduler.in")
-)
+scheduler_requires = read_requirements(os.path.join(REQ_PATH, "requirements-scheduler.in"))
 
 setup(
     name=PKG_NAME,
     url=URL,
     license=LICENSE,
     description=DESCRIPTION,
     platforms=PLATFORMS,
```

### Comparing `vbcore-2.2.0rc4/vbcore/aio.py` & `vbcore-2.2.1/vbcore/aio.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/base.py` & `vbcore-2.2.1/vbcore/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/batch.py` & `vbcore-2.2.1/vbcore/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,15 @@
         self._return_exceptions = return_exceptions
 
     async def batch(self):
         tasks = []
         for task in self._tasks:
             func, args = self.prepare_task(task)
             tasks.append(
-                aio.async_wrapper(func, **args)
-                if not aio.is_async(func)
-                else func(**args)
+                aio.async_wrapper(func, **args) if not aio.is_async(func) else func(**args)
             )
 
         return await aio.collect(*tasks, return_exc=self._return_exceptions)
 
     def run(self) -> t.List:
         loop = aio.get_event_loop()
         return loop.run_until_complete(self.batch())
```

### Comparing `vbcore-2.2.0rc4/vbcore/configurator.py` & `vbcore-2.2.1/vbcore/configurator.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,17 +32,15 @@
         cast: t.Callable[[str], t.Any] = str,
     ) -> t.Any:
         env_var = os.environ.get(key)
         if env_var:
             try:
                 return cast(env_var)
             except Exception as exc:
-                raise ValueError(
-                    f"unable to cast config key '{key}' to type: {cast}"
-                ) from exc
+                raise ValueError(f"unable to cast config key '{key}' to type: {cast}") from exc
 
         if required and not default:
             raise EnvironmentError(f"envvar '{key}' required or provide a default")
 
         return default
```

### Comparing `vbcore-2.2.0rc4/vbcore/context.py` & `vbcore-2.2.1/vbcore/context.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/crypto/argon.py` & `vbcore-2.2.1/vbcore/crypto/argon.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,14 @@
     @cached_property
     def hasher(self) -> argon2.PasswordHasher:
         return argon2.PasswordHasher(**self.options.to_dict())
 
     def hash(self, data: HashableType) -> str:
         return self.hasher.hash(data)
 
-    def verify(
-        self, given_hash: str, data: HashableType, raise_exc: bool = False
-    ) -> bool:
+    def verify(self, given_hash: str, data: HashableType, raise_exc: bool = False) -> bool:
         try:
             return self.hasher.verify(given_hash, data)
         except (Argon2Error, InvalidHash) as exc:
             if raise_exc is True:
                 raise VBInvalidHashError(given_hash, orig=exc) from exc
             return False
```

### Comparing `vbcore-2.2.0rc4/vbcore/crypto/base.py` & `vbcore-2.2.1/vbcore/crypto/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,17 +20,15 @@
     @abc.abstractmethod
     def hash(self, data: HashableType) -> str:
         """
         @param data:
         """
 
     @abc.abstractmethod
-    def verify(
-        self, given_hash: str, data: HashableType, raise_exc: bool = False
-    ) -> bool:
+    def verify(self, given_hash: str, data: HashableType, raise_exc: bool = False) -> bool:
         """
         @param given_hash:
         @param data:
         @param raise_exc:
         """
 
     def to_bytes(self, data: str) -> bytes:
```

### Comparing `vbcore-2.2.0rc4/vbcore/crypto/bcrypt.py` & `vbcore-2.2.1/vbcore/crypto/bcrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,15 @@
     def prepare_data(self, data: HashableType) -> bytes:
         return self.to_bytes(data) if isinstance(data, str) else data
 
     def hash(self, data: HashableType) -> str:
         hashed = bcrypt.hashpw(self.prepare_data(data), self.salt())
         return self.to_string(hashed)
 
-    def verify(
-        self, given_hash: str, data: HashableType, raise_exc: bool = False
-    ) -> bool:
+    def verify(self, given_hash: str, data: HashableType, raise_exc: bool = False) -> bool:
         try:
             return bcrypt.checkpw(
                 self.prepare_data(data),
                 self.to_bytes(given_hash),
             )
         except ValueError as exc:
             if raise_exc:
```

### Comparing `vbcore-2.2.0rc4/vbcore/crypto/factory.py` & `vbcore-2.2.1/vbcore/crypto/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/crypto/hashes.py` & `vbcore-2.2.1/vbcore/crypto/hashes.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 class BuiltinHash(Hasher[HashOptions]):
     ALGO: t.ClassVar[str]
 
     def hash(self, data: HashableType) -> str:
         data = self.to_bytes(data) if isinstance(data, str) else data
         return hashlib.new(self.ALGO, data=data).hexdigest()
 
-    def verify(
-        self, given_hash: str, data: HashableType, raise_exc: bool = False
-    ) -> bool:
+    def verify(self, given_hash: str, data: HashableType, raise_exc: bool = False) -> bool:
         if hmac.compare_digest(given_hash, self.hash(data)):
             return True
 
         if raise_exc:
             raise VBInvalidHashError(given_hash)
 
         return False
```

### Comparing `vbcore-2.2.0rc4/vbcore/csvfile.py` & `vbcore-2.2.1/vbcore/csvfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,31 +17,27 @@
     encoding: str = "utf-8"
     delimiter: str = "|"
     dialect: str = "unix"
     encoding_errors: str = "replace"
     quoting: int = csv.QUOTE_NONE
     escape_char: str = "\\"
     allow_extra_fields: bool = True
-    supported_encodings: t.List[str] = field(
-        default_factory=lambda: ["ascii", "ISO-8859-1"]
-    )
+    supported_encodings: t.List[str] = field(default_factory=lambda: ["ascii", "ISO-8859-1"])
 
 
 class CSVHandler(FileHandler):
     def __init__(
         self,
         filename: OptStr = None,
         fields: t.Optional[StrList] = None,
         params: t.Optional[CSVParams] = None,
     ):
         self.fields = fields or []
         self.params = params or CSVParams()
-        super().__init__(
-            filename, self.params.encoding, self.params.supported_encodings
-        )
+        super().__init__(filename, self.params.encoding, self.params.supported_encodings)
 
     def open(self, filename: OptStr = None, **kwargs) -> t.IO:
         return super().open(
             filename,
             newline=self.params.new_line,
             encoding=self.params.encoding,
             errors=self.params.encoding_errors,
@@ -53,17 +49,15 @@
         if lines <= 0:
             raise VBEmptyFileError(
                 filename,
                 "no record found in the file" if lines == 0 else "header is missing",
             )
 
     @contextmanager
-    def reader(
-        self, filename: OptStr = None
-    ) -> t.Generator[csv.DictReader, None, None]:
+    def reader(self, filename: OptStr = None) -> t.Generator[csv.DictReader, None, None]:
         with self.open(filename) as file:
             reader = csv.DictReader(
                 file,
                 delimiter=self.params.delimiter,
                 quoting=self.params.quoting,
                 escapechar=self.params.escape_char,
             )
@@ -95,17 +89,15 @@
         return {k: v for k, v in record.items() if k in self.fields}
 
     def readlines(self, filename: OptStr = None) -> t.Generator[dict, None, None]:
         with self.reader(filename) as reader:
             for record in reader:
                 yield self.after_read_hook(record)
 
-    def coroutine_writer(
-        self, filename: OptStr = None, **kwargs
-    ) -> WriterCoroutineType:
+    def coroutine_writer(self, filename: OptStr = None, **kwargs) -> WriterCoroutineType:
         with self.writer(filename, **kwargs) as writer:
             writer.writeheader()
             while True:
                 records: RecordType = (yield)  # noqa: E275
                 _records = [records] if isinstance(records, dict) else records
                 for r in _records:
                     writer.writerow(self.pre_write_hook(r))
```

### Comparing `vbcore-2.2.0rc4/vbcore/data/transformations/builders/base.py` & `vbcore-2.2.1/vbcore/data/transformations/builders/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/data/transformations/builders/csv.py` & `vbcore-2.2.1/vbcore/data/transformations/builders/csv.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/data/transformations/builders/dicttoxml.py` & `vbcore-2.2.1/vbcore/data/transformations/builders/dicttoxml.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,45 +94,39 @@
         else:
             raise TypeError(f"Unsupported data type: {val} ({type(val).__name__})")
 
     return "".join(output)
 
 
 # pylint: disable=too-many-branches
-def convert_list(
-    items: Iterable[Any], attr_type: bool, default_item_name: str, cdata: bool
-) -> str:
+def convert_list(items: Iterable[Any], attr_type: bool, default_item_name: str, cdata: bool) -> str:
     output = []
     item_name = default_item_name
 
     for item in items:
         attr_string = make_attr_string(item, attr_type)
 
         if isinstance(item, (numbers.Number, str)):
             output.append(convert_kv(item_name, item, attr_string, cdata))
         elif hasattr(item, "isoformat"):  # datetime
             output.append(convert_kv(item_name, item.isoformat(), attr_string, cdata))
         elif isinstance(item, bool):
-            output.append(
-                f"<{item_name}{attr_string}>{str(item).lower()}</{item_name}>"
-            )
+            output.append(f"<{item_name}{attr_string}>{str(item).lower()}</{item_name}>")
         elif isinstance(item, dict):
             content = convert_dict(item, attr_type, default_item_name, cdata)
             if not attr_type:
                 output.append(f"<{item_name}>{content}</{item_name}>")
             else:
                 output.append(f'<{item_name} type="dict">{content}</{item_name}>')
         elif isinstance(item, Iterable):
             content = convert_list(item, attr_type, default_item_name, cdata)
             if not attr_type:
                 output.append(f"<{item_name} {attr_string}>{content}</{item_name}>")
             else:
-                output.append(
-                    f'<{item_name} type="list"{attr_string}>{content}</{item_name}>'
-                )
+                output.append(f'<{item_name} type="list"{attr_string}>{content}</{item_name}>')
         elif item is None:
             output.append(f"<{item_name}{attr_string}></{item_name}>")
         else:
             raise TypeError(f"Unsupported data type: {item} ({type(item).__name__})")
 
     return "".join(output)
```

### Comparing `vbcore-2.2.0rc4/vbcore/data/transformations/builders/factory.py` & `vbcore-2.2.1/vbcore/data/transformations/builders/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/data/transformations/builders/html.py` & `vbcore-2.2.1/vbcore/data/transformations/builders/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,15 @@
         for row in rows:
             dumped.extend(self.dump_row(row))
         return [self.tag_open_body, *dumped, self.tag_close_body]
 
     def build(self, rows: List[dict], table_id: str | None = None) -> str:
         headers = self.prepare_headers(rows)
         tag_open_table = (
-            self.tag_open_table_id.format(id=table_id)
-            if table_id
-            else self.tag_open_table
+            self.tag_open_table_id.format(id=table_id) if table_id else self.tag_open_table
         )
         return f"{self.separator}".join(
             [
                 tag_open_table,
                 *self.dump_header(headers),
                 *self.dump_body(rows),
                 self.tag_close_table,
@@ -120,17 +118,15 @@
         return root.find(self.xpath_table) or root
 
     @classmethod
     def extract_text(cls, elem: Element) -> str:
         return parse_value("".join(elem.itertext()))
 
     def extract_header(self, head: Element) -> List[str]:
-        headers = [
-            self.extract_text(elem) for elem in head.findall(self.xpath_head_item)
-        ]
+        headers = [self.extract_text(elem) for elem in head.findall(self.xpath_head_item)]
         if not headers:
             raise ValueError("no headers found")
         return headers
 
     def extract_row(self, headers: List[str], row: Element) -> dict:
         return {
             headers[index]: self.extract_text(col)
```

### Comparing `vbcore-2.2.0rc4/vbcore/data/transformations/builders/json.py` & `vbcore-2.2.1/vbcore/data/transformations/builders/json.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/data/transformations/builders/xml.py` & `vbcore-2.2.1/vbcore/data/transformations/builders/xml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/data/transformations/builders/yaml.py` & `vbcore-2.2.1/vbcore/data/transformations/builders/yaml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/datastruct/buffer.py` & `vbcore-2.2.1/vbcore/datastruct/buffer.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/datastruct/cache.py` & `vbcore-2.2.1/vbcore/datastruct/cache.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/datastruct/dictionaries.py` & `vbcore-2.2.1/vbcore/datastruct/dictionaries.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/datastruct/lazy.py` & `vbcore-2.2.1/vbcore/datastruct/lazy.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,28 +62,25 @@
         *args,
         package: OptStr = None,
         message: OptStr = None,
         subclass_of: t.Optional[t.Type] = None,
         instance_of: t.Optional[t.Type] = None,
     ) -> t.Tuple[t.Any, ...]:
         return tuple(
-            cls.do_import(name, package, message, subclass_of, instance_of)
-            for name in args
+            cls.do_import(name, package, message, subclass_of, instance_of) for name in args
         )
 
 
 class LazyDump(Lazy):
     def __str__(self):
         return self()
 
 
 class Dumper(Lazy):
-    def __init__(
-        self, data: t.Any, *args, callback: t.Optional[t.Callable] = None, **kwargs
-    ):
+    def __init__(self, data: t.Any, *args, callback: t.Optional[t.Callable] = None, **kwargs):
         super().__init__(callback or str, data, *args, **kwargs)
         self.data = data
 
     def dump(self) -> str:
         return self(self.data)
 
     def __str__(self):
```

### Comparing `vbcore-2.2.0rc4/vbcore/datastruct/orderer_set.py` & `vbcore-2.2.1/vbcore/datastruct/orderer_set.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/date_helper.py` & `vbcore-2.2.1/vbcore/date_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,15 @@
         return cls.date_to_str(now, fmt)
 
     @classmethod
     def date_to_str(cls, date: DateType, fmt: OptStr = None) -> str:
         return date.strftime(fmt or DateTimeFmt.ISO)
 
     @classmethod
-    def str_to_date(
-        cls, date: str, fmt: OptStr = None, is_iso: bool = False, **kwargs
-    ) -> datetime:
+    def str_to_date(cls, date: str, fmt: OptStr = None, is_iso: bool = False, **kwargs) -> datetime:
         """
 
         :param date: input string date
         :param fmt: format input date (optional: could be detected from string)
         :param is_iso: flag for implicit iso format
         :param kwargs: passed to date_parse
         :return: return parsed date
@@ -127,21 +125,17 @@
     @classmethod
     def pretty_date(cls, date: AnyDateType) -> str:
         if isinstance(date, str):
             return cls.change_format(date, out_fmt=DateTimeFmt.PRETTY, raise_exc=True)
         return cls.date_to_str(date, fmt=DateTimeFmt.PRETTY)
 
     @classmethod
-    def from_iso_format(
-        cls, str_date: str, fmt: str, exc: bool = True
-    ) -> t.Optional[str]:
+    def from_iso_format(cls, str_date: str, fmt: str, exc: bool = True) -> t.Optional[str]:
         return DateHelper.change_format(
             str_date, in_fmt=DateTimeFmt.ISO, out_fmt=fmt, raise_exc=exc
         )
 
     @classmethod
-    def to_iso_format(
-        cls, str_date: str, fmt: OptStr = None, exc: bool = True
-    ) -> t.Optional[str]:
+    def to_iso_format(cls, str_date: str, fmt: OptStr = None, exc: bool = True) -> t.Optional[str]:
         return DateHelper.change_format(
             str_date, in_fmt=fmt, out_fmt=DateTimeFmt.ISO, raise_exc=exc
         )
```

### Comparing `vbcore-2.2.0rc4/vbcore/db/events.py` & `vbcore-2.2.1/vbcore/db/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,36 +269,26 @@
         data.exc,
     )
 
 
 @filters(
     "postgresql",
     sqla_exc.ProgrammingError,
-    (
-        r".* constraint \"(?P<constraint>.+)\" "
-        "of relation "
-        '"(?P<relation>.+)" does not exist'
-    ),
+    r'.* constraint \"(?P<constraint>.+)\" of relation "(?P<relation>.+)" does not exist',
 )
 @filters(
     "mysql",
     sqla_exc.InternalError,
     r".*1025,.*Error on rename of '.+/(?P<relation>.+)' to ",
-    (
-        ".*1091,.*Can't DROP (?:FOREIGN KEY )?['`](?P<constraint>.+)['`]; "
-        "check that .* exists"
-    ),
+    ".*1091,.*Can't DROP (?:FOREIGN KEY )?['`](?P<constraint>.+)['`]; check that .* exists",
 )
 @filters(
     "mysql",
     sqla_exc.OperationalError,
-    (
-        r".*1091,.*Can't DROP (?:FOREIGN KEY )?['`](?P<constraint>.+)['`]; "
-        "check that .* exists"
-    ),
+    r".*1091,.*Can't DROP (?:FOREIGN KEY )?['`](?P<constraint>.+)['`]; check that .* exists",
 )
 def _check_constraint_non_existing(data: ExceptionData):
     raise DBNonExistentConstraint(
         try_match(data.match, "relation"),
         try_match(data.match, "constraint"),
         data.exc,
     )
```

### Comparing `vbcore-2.2.0rc4/vbcore/db/exceptions.py` & `vbcore-2.2.1/vbcore/db/exceptions.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/db/listener.py` & `vbcore-2.2.1/vbcore/db/listener.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/db/mixins.py` & `vbcore-2.2.1/vbcore/db/mixins.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,23 +14,17 @@
     hybrid_property = property  # pylint: disable=C0103
 else:
     from sqlalchemy.ext.hybrid import hybrid_property
 
 
 class Column:
     id: t.ClassVar = partial(sa.Column, sa.Integer, primary_key=True)
-    uuid: t.ClassVar = partial(
-        sa.Column, sa.String(36), primary_key=True, default=lambda: get_uuid
-    )
-    auto: t.ClassVar = partial(
-        sa.Column, sa.Integer, primary_key=True, autoincrement=True
-    )
-    date_created: t.ClassVar = partial(
-        sa.Column, sa.DateTime, server_default=sa.func.now()
-    )
+    uuid: t.ClassVar = partial(sa.Column, sa.String(36), primary_key=True, default=lambda: get_uuid)
+    auto: t.ClassVar = partial(sa.Column, sa.Integer, primary_key=True, autoincrement=True)
+    date_created: t.ClassVar = partial(sa.Column, sa.DateTime, server_default=sa.func.now())
     date_updated: t.ClassVar = partial(sa.Column, sa.DateTime, onupdate=sa.func.now())
     description: t.ClassVar = partial(sa.Column, sa.Text(), nullable=True)
 
 
 class BaseMixin:
     __table__: sa.Table
```

### Comparing `vbcore-2.2.0rc4/vbcore/db/mysql_dumper.py` & `vbcore-2.2.1/vbcore/db/mysql_dumper.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,17 +96,15 @@
             if database not in self.ignore_databases:
                 yield database
 
     def get_tables(self, database: str) -> t.Iterator[str]:
         cmdline = self.mysql_cmdline("show tables", database=database)
         return self.execute_text(cmdline)
 
-    def all_tables(
-        self, db_prefix: OptStr = None
-    ) -> t.Generator[CoupleStr, None, None]:
+    def all_tables(self, db_prefix: OptStr = None) -> t.Generator[CoupleStr, None, None]:
         for database in self.get_databases(db_prefix):
             for table in self.get_tables(database):
                 yield database, table
 
     def dump_table(self, database: str, table: str) -> MySQLDump:
         cmdline = self.mysqldump_cmdline(database=database, table=table)
         result = self.execute_binary(cmdline)
@@ -134,17 +132,15 @@
         filename = "_".join(filter(None, (*args, current_datetime)))
         return os.path.join(self.folder, f"{filename}.{ext}")
 
     def backup_single_files(self, file_prefix: OptStr = None, db_prefix: OptStr = None):
         for database, table in self.dumper.all_tables(db_prefix):
             self.log.info("dumping table: %s.%s ......", database, table)
             dump = self.dumper.dump_table(database, table)
-            filename = self.prepare_filename(
-                file_prefix, f"{database}.{table}", ext="sql"
-            )
+            filename = self.prepare_filename(file_prefix, f"{database}.{table}", ext="sql")
             with open(filename, mode="wb") as file:
                 file.write(dump.dump)
 
             self.log.info(
                 "table: %s.%s successfully dumped at: %s",
                 database,
                 table,
```

### Comparing `vbcore-2.2.0rc4/vbcore/db/schema.py` & `vbcore-2.2.1/vbcore/db/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,75 @@
 import importlib
 import typing as t
 
-from sqlalchemy import create_mock_engine, MetaData  # type: ignore
+from sqlalchemy import create_mock_engine, MetaData
 from sqlalchemy.engine import Engine
-from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.orm import class_mapper
-from sqlalchemy_schemadisplay import create_schema_graph, create_uml_graph
 
+from vbcore.db.schema_display.db_diagram import create_schema_graph
+from vbcore.db.schema_display.model_diagram import create_uml_graph
+from vbcore.db.sqla import SQLAConnector
 from vbcore.loggers import Log
 from vbcore.types import OptStr
 
 
 def model_to_uml(
     module: str,
-    show_operations: bool = False,
+    show_operations: bool = True,
     show_attributes: bool = True,
-    show_inherited: bool = True,
     show_datatypes: bool = True,
+    show_inherited: bool = True,
+    show_multiplicity_one: bool = True,
     **kwargs,
 ):
     mappers = []
     models = importlib.import_module(module)
 
     for attr in dir(models):
-        if attr[0] == "_":
-            continue
         try:
             cls = getattr(models, attr)
             mappers.append(class_mapper(cls))
-        except SQLAlchemyError as exc:
-            Log.get(__name__).warning(exc, exc_info=True)
+        except Exception as exc:  # pylint: disable=broad-exception-caught
+            Log.get(__name__).debug(exc)
 
     return create_uml_graph(
         mappers,
         show_operations=show_operations,
         show_attributes=show_attributes,
-        show_inherited=show_inherited,
         show_datatypes=show_datatypes,
+        show_inherited=show_inherited,
+        show_multiplicity_one=show_multiplicity_one,
         **kwargs,
     )
 
 
 def db_to_schema(
     url: str,
     show_datatypes: bool = True,
     show_indexes: bool = True,
     concentrate: bool = True,
     rankdir: str = "TB",
     **kwargs,
 ):
+    connector = SQLAConnector(url)
     return create_schema_graph(
-        metadata=MetaData(url),  # type: ignore
+        engine=connector.engine,
+        metadata=connector.metadata,
         show_datatypes=show_datatypes,
         show_indexes=show_indexes,
         concentrate=concentrate,
         rankdir=rankdir,
+        format_schema_name={"bold": True, "fontsize": "12"},
+        format_table_name={"bold": True, "fontsize": "12"},
         **kwargs,
     )
 
 
 def dump_model_ddl(metadata: MetaData, dialect: OptStr = None):
     dialect = dialect or "sqlite"
 
     def executor(sql, *_, **__):
-        compiled = sql.compile(dialect=engine.dialect).replace("\n\n", "")
-        print(compiled, ";", sep="")  # type: ignore
+        compiled = sql.compile(dialect=engine.dialect)
+        print(compiled.replace("\n\n", ""), ";", sep="")
 
     engine = create_mock_engine(f"{dialect}://", executor=executor)
     metadata.create_all(t.cast(Engine, engine))
```

### Comparing `vbcore-2.2.0rc4/vbcore/db/sqla.py` & `vbcore-2.2.1/vbcore/db/sqla.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,16 +51,16 @@
         self._session_options = session_options or {}
         self._session_options.setdefault("class_", session_class)
         self._session_options.setdefault("autoflush", autoflush)
         self._session_options.setdefault("autocommit", autocommit)
         self._session_options.setdefault("expire_on_commit", expire_on_commit)
         self._factory: t.Optional[sessionmaker] = None
 
-    @staticmethod
-    def register_loaders(session: SessionType, loaders: LoadersType):
+    @classmethod
+    def register_loaders(cls, session: SessionType, loaders: LoadersType) -> None:
         for loader in loaders:
             callback = partial(loader.load_values, session)
             Listener.register_after_create(loader.__table__, callback)
 
     def create_all(self, loaders: LoadersType = ()) -> None:
         if loaders:
             with self.connection() as session:
```

### Comparing `vbcore-2.2.0rc4/vbcore/db/support.py` & `vbcore-2.2.1/vbcore/db/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,31 +59,27 @@
                 query = self.fetch(**lookup)
                 if lock:
                     query = query.with_for_update()
                     obj = query.one()
                 return obj, False
             return obj, True
 
-    def get_or_create(
-        self, defaults: t.Optional[dict] = None, **kwargs
-    ) -> t.Tuple[t.Any, bool]:
+    def get_or_create(self, defaults: t.Optional[dict] = None, **kwargs) -> t.Tuple[t.Any, bool]:
         """
         @param defaults: attribute used to create record
         @param kwargs: filters used to fetch record or create
         @return created object and is_created flag
         """
         try:
             return self.fetch(**kwargs).one(), False
         except NoResultError:
             params = self._prepare_params(defaults, **kwargs)
             return self._create_object(kwargs, params)
 
-    def update_or_create(
-        self, defaults: t.Optional[dict] = None, **kwargs
-    ) -> t.Tuple[t.Any, bool]:
+    def update_or_create(self, defaults: t.Optional[dict] = None, **kwargs) -> t.Tuple[t.Any, bool]:
         """
         @param defaults: attribute used to create record
         @param kwargs: filters used to fetch record or create
         @return updated object and is_created flag
         """
         defaults = defaults or {}
         with self.session.begin_nested():
@@ -104,17 +100,15 @@
 
         return obj, False
 
     def fetch(self, *args, fields: tuple = (), **kwargs) -> Query:
         columns = fields or (self.model,)
         return self.session.query(*columns).filter(*args).filter_by(**kwargs)
 
-    def delete(
-        self, *args, synchronize: SynchronizeSessionArgument = "evaluate", **kwargs
-    ) -> int:
+    def delete(self, *args, synchronize: SynchronizeSessionArgument = "evaluate", **kwargs) -> int:
         row_count = self.fetch(*args, **kwargs).delete(synchronize)
         if self._commit:
             self.session.commit()
         return row_count
 
     def bulk_insert(self, records: t.Iterable[Model]) -> None:
         self.session.add_all(records)
```

### Comparing `vbcore-2.2.0rc4/vbcore/db/views.py` & `vbcore-2.2.1/vbcore/db/views.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/dictutils/flatter_dict.py` & `vbcore-2.2.1/vbcore/dictutils/flatter_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,17 +279,15 @@
 
         :rtype: list
         """
         keys = []
 
         for key, value in self._values.items():
             if isinstance(value, (FlatDict, dict)):
-                nested = [
-                    self._delimiter.join([str(key), str(k)]) for k in value.keys()
-                ]
+                nested = [self._delimiter.join([str(key), str(k)]) for k in value.keys()]
                 keys += nested if nested else [key]
             else:
                 keys.append(key)
 
         return keys
 
     def pop(self, key, default=NO_DEFAULT):
```

### Comparing `vbcore-2.2.0rc4/vbcore/dispatcher.py` & `vbcore-2.2.1/vbcore/dispatcher.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/enums.py` & `vbcore-2.2.1/vbcore/enums.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/excel/report.py` & `vbcore-2.2.1/vbcore/excel/report.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/exceptions.py` & `vbcore-2.2.1/vbcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/factory.py` & `vbcore-2.2.1/vbcore/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/files.py` & `vbcore-2.2.1/vbcore/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,17 @@
         extra = (
             f"(confidence: {confidence}, language: {language})"
             if language
             else f"(confidence: {confidence})"
         )
         suffix = f"\nSupported encodings are {tuple(supported)}"
         if encoding:
-            super().__init__(
-                f"{prefix} file encoding '{encoding}' {extra} not supported!{suffix}"
-            )
+            super().__init__(f"{prefix} file encoding '{encoding}' {extra} not supported!{suffix}")
         else:
-            super().__init__(
-                f"{prefix} unable to detect file encoding {extra}!{suffix}"
-            )
+            super().__init__(f"{prefix} unable to detect file encoding {extra}!{suffix}")
 
 
 class FileHandler:
     def __init__(
         self,
         filename: OptStr = None,
         encoding: OptStr = None,
@@ -93,17 +89,15 @@
                 detector.feed(line)
                 if detector.done:
                     break
             detector.close()
 
         return EncodingData(**detector.result)
 
-    def check_encoding(
-        self, filename: OptStr = None, extra_supported: t.Sequence[str] = ()
-    ):
+    def check_encoding(self, filename: OptStr = None, extra_supported: t.Sequence[str] = ()):
         encoding = self.detect_encoding(filename)
         supported_encodings = [
             self.encoding,
             *self.supported_encodings,
             *extra_supported,
         ]
         if encoding.encoding not in supported_encodings:
```

### Comparing `vbcore-2.2.0rc4/vbcore/http/batch.py` & `vbcore-2.2.1/vbcore/http/batch.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/http/client.py` & `vbcore-2.2.1/vbcore/http/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,17 +136,15 @@
     @staticmethod
     def prepare_response(
         body: t.Optional[t.Any] = None,
         status: int = httpcode.SUCCESS,
         headers: t.Optional[t.Dict[str, str]] = None,
         exception: t.Optional[Exception] = None,
     ) -> ResponseData:
-        return ResponseData(
-            body=body, status=status, headers=headers or {}, exception=exception
-        )
+        return ResponseData(body=body, status=status, headers=headers or {}, exception=exception)
 
     def request(
         self,
         uri: str,
         method: str = HttpMethod.GET,
         dump_body: t.Optional[DumpBodyType] = None,
         raise_on_exc: bool = False,
@@ -162,17 +160,15 @@
             timeout = kwargs.pop("timeout", None) or self._timeout
             response = send_request(method, url, timeout=timeout, **kwargs)
         except NetworkError as exc:
             self.log.exception(exc)
             if raise_on_exc or self._raise_on_exc:
                 raise  # pragma: no cover
 
-            return self.prepare_response(
-                status=httpcode.SERVICE_UNAVAILABLE, exception=exc
-            )
+            return self.prepare_response(status=httpcode.SERVICE_UNAVAILABLE, exception=exc)
 
         log_resp = self.dump_response(response, dump_body=dump_body[1])
         try:
             response.raise_for_status()
             self.log.info("%s", log_resp)
         except HTTPStatusError as exc:
             self.log.warning("%s", log_resp)
@@ -221,17 +217,15 @@
         self._version = version
         self._request_id = None
 
     @property
     def request_id(self):
         return self._request_id
 
-    def request(
-        self, method, request_id=None, **kwargs
-    ):  # pylint: disable=arguments-differ
+    def request(self, method, request_id=None, **kwargs):  # pylint: disable=arguments-differ
         self._request_id = request_id or get_uuid()
         return self._request(method, **kwargs)
 
     def notification(self, method, **kwargs):
         self._request_id = None
         return self._request(method, **kwargs)
```

### Comparing `vbcore-2.2.0rc4/vbcore/http/gql.py` & `vbcore-2.2.1/vbcore/http/gql.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/http/headers.py` & `vbcore-2.2.1/vbcore/http/headers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/http/httpcode.py` & `vbcore-2.2.1/vbcore/http/httpcode.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/http/httpdumper.py` & `vbcore-2.2.1/vbcore/http/httpdumper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/http/proxy.py` & `vbcore-2.2.1/vbcore/http/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,17 +164,15 @@
         return client.notification(
             self.request_method(),
             params=self.request_params(),
             stream=self._stream if stream is None else stream,
             headers=self.request_headers(),
         )
 
-    def prepare_response(
-        self, resp: t.Optional[ObjectDict] = None, **kwargs
-    ) -> Response:
+    def prepare_response(self, resp: t.Optional[ObjectDict] = None, **kwargs) -> Response:
         body = resp
         headers: t.Dict[str, str] = {
             HeaderEnum.CONTENT_TYPE: self.response_content_type,
             **kwargs,
         }
         status = httpcode.NO_CONTENT if resp is None else httpcode.SUCCESS
```

### Comparing `vbcore-2.2.0rc4/vbcore/http/rpc.py` & `vbcore-2.2.1/vbcore/http/rpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,37 +12,31 @@
 
     def as_dict(self) -> ObjectDict:
         return ObjectDict(code=self.code, message=self.message, data=self.data)
 
 
 class RPCParseError(RPCError):
     def __init__(self, message=None, data=None):
-        super().__init__(
-            -32700, message or "Invalid JSON was received by the server", data
-        )
+        super().__init__(-32700, message or "Invalid JSON was received by the server", data)
 
 
 class RPCInvalidRequest(RPCError):
     def __init__(
         self,
         message=None,
         data=None,
         req_id=None,
     ):
-        super().__init__(
-            -32600, message or "The JSON sent is not a valid Request object", data
-        )
+        super().__init__(-32600, message or "The JSON sent is not a valid Request object", data)
         self.req_id = req_id
 
 
 class RPCMethodNotFound(RPCError):
     def __init__(self, message=None, data=None):
-        super().__init__(
-            -32601, message or "The method does not exist or is not available", data
-        )
+        super().__init__(-32601, message or "The method does not exist or is not available", data)
 
 
 class RPCInvalidParams(RPCError):
     def __init__(self, message=None, data=None):
         super().__init__(-32602, message or "Invalid method parameter(s)", data)
```

### Comparing `vbcore-2.2.0rc4/vbcore/http/useragent.py` & `vbcore-2.2.1/vbcore/http/useragent.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/importer.py` & `vbcore-2.2.1/vbcore/importer.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/json.py` & `vbcore-2.2.1/vbcore/json.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/jsonschema/schemas/jsonrpc.py` & `vbcore-2.2.1/vbcore/jsonschema/schemas/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/jsonschema/support.py` & `vbcore-2.2.1/vbcore/jsonschema/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,15 @@
 
         report = []
         json_object[e.path[-1]] = orig
         json_error = cls.dumper(json_object)
 
         for lineno, text in enumerate(io.StringIO(json_error)):
             # pylint: disable=consider-using-f-string
-            line_text = "{:4}: {}".format(
-                lineno + 1, ">" * 3 if lineno == err_line else " " * 3
-            )
+            line_text = "{:4}: {}".format(lineno + 1, ">" * 3 if lineno == err_line else " " * 3)
             report.append(line_text + text.rstrip("\n"))
 
         report = report[max(0, err_line - lines_before) : err_line + 1 + lines_after]
         return cls.message_format.format(
             line=err_line + 1, report="\n".join(report), message=e.message or str(e)
         )
 
@@ -134,35 +132,29 @@
     null = ObjectDict(type="null")
     integer = ObjectDict(type="integer")
     string = ObjectDict(type="string")
     number = ObjectDict(type="number")
     boolean = ObjectDict(type="boolean")
     datetime = ObjectDict(type="string", format="date-time")
     any_object = ObjectDict(type="object", additionalProperties=True)
-    any = ObjectDict(
-        type=["integer", "string", "number", "boolean", "array", "object", "null"]
-    )
+    any = ObjectDict(type=["integer", "string", "number", "boolean", "array", "object", "null"])
 
     class Opt:
         integer = ObjectDict(type=["integer", "null"])
         string = ObjectDict(type=["string", "null"])
         number = ObjectDict(type=["number", "null"])
         boolean = ObjectDict(type=["boolean", "null"])
 
     @classmethod
     def oneof(cls, *args, **kwargs) -> ObjectDict:
-        return ObjectDict(
-            oneOf=list(args) if len(args) > 1 else [*args, cls.null], **kwargs
-        )
+        return ObjectDict(oneOf=list(args) if len(args) > 1 else [*args, cls.null], **kwargs)
 
     @classmethod
     def anyof(cls, *args, **kwargs) -> ObjectDict:
-        return ObjectDict(
-            anyOf=list(args) if len(args) > 1 else [*args, cls.null], **kwargs
-        )
+        return ObjectDict(anyOf=list(args) if len(args) > 1 else [*args, cls.null], **kwargs)
 
     @classmethod
     def ref(cls, path: str, **kwargs) -> ObjectDict:
         return ObjectDict(**{"$ref": f"#{path}", **kwargs})
 
     @classmethod
     def enum(cls, *args, **kwargs) -> ObjectDict:
```

### Comparing `vbcore-2.2.0rc4/vbcore/lambdas.py` & `vbcore-2.2.1/vbcore/lambdas.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,17 +106,15 @@
         closed: bool = False,
         left: bool = False,
         right: bool = False,
     ) -> bool:
         return op_in_range(value, range_, closed=closed, left=left, right=right)
 
 
-def chunk_iterator(
-    iterable: t.Iterable[T], chunk_size: int
-) -> t.Generator[t.List[T], None, None]:
+def chunk_iterator(iterable: t.Iterable[T], chunk_size: int) -> t.Generator[t.List[T], None, None]:
     _iterable = iter(iterable)
 
     while True:
         chunk = []
         try:
             for _ in range(chunk_size):
                 chunk.append(next(_iterable))
```

### Comparing `vbcore-2.2.0rc4/vbcore/loggers.py` & `vbcore-2.2.1/vbcore/loggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,17 +60,15 @@
     level: str = "INFO"
     force: bool = True
     config_file: OptStr = None
     listen_for_reload: bool = False
     listener_daemon: bool = True
     listener_port: int = DEFAULT_LISTENER_PORT
     default_date_format = "%Y-%m-%d %H:%M:%S"
-    default_format: str = (
-        "%(asctime)s.%(msecs)03d | %(levelname)-8s | %(name)s | %(message)s"
-    )
+    default_format: str = "%(asctime)s.%(msecs)03d | %(levelname)-8s | %(name)s | %(message)s"
 
 
 class SetupLoggers:
     def __init__(
         self,
         config: t.Optional[LoggingSettings] = None,
         config_file: OptStr = None,
```

### Comparing `vbcore-2.2.0rc4/vbcore/misc.py` & `vbcore-2.2.1/vbcore/misc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/net/ftpclient/legacy.py` & `vbcore-2.2.1/vbcore/net/ftpclient/legacy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import contextlib
 import re
 from dataclasses import dataclass
-from ftplib import FTP  # nosec
-from typing import Generator, Optional
+from ftplib import FTP, FTP_TLS  # nosec
+from functools import cached_property
+from typing import Generator, Optional, Union
 
 from vbcore.base import BaseDTO
 from vbcore.loggers import VBLoggerMixin
 from vbcore.types import OptStr
 
 
 @dataclass(frozen=True, kw_only=True)
@@ -14,28 +15,36 @@
     host: str
     port: int
     user: OptStr = None
     password: OptStr = None
     timeout: int = 300
     debug: bool = False
     encoding: str = "utf-8"
+    tls: bool = False
 
 
 class FTPHandler(VBLoggerMixin):
     def __init__(self, options: FTPOptions):
         self.options = options
-        self.client = FTP(timeout=options.timeout, encoding=options.encoding)  # nosec
+
+    @cached_property
+    def client(self) -> Union[FTP, FTP_TLS]:
+        ftp_class = FTP_TLS if self.options.tls else FTP  # nosec
+        return ftp_class(timeout=self.options.timeout, encoding=self.options.encoding)
 
     @contextlib.contextmanager
     def connect(self) -> Generator[FTP, None, None]:
         opts = self.options
         with self.client as ftp:
             ftp.debugging = 3 if opts.debug else 0
             ftp.connect(opts.host, opts.port)
             ftp.login(opts.user, opts.password or "")
+
+            if self.options.tls and isinstance(ftp, FTP_TLS):
+                ftp.prot_p()
             yield ftp
 
     def download_file(self, remote_path: str, local_path: str):
         with self.connect() as conn:
             with open(local_path, "wb") as file:
                 self.log.info("downloading '%s' -> '%s'...", remote_path, local_path)
                 conn.retrbinary(f"RETR {remote_path}", file.write)
```

### Comparing `vbcore-2.2.0rc4/vbcore/net/ftpclient/sftp.py` & `vbcore-2.2.1/vbcore/net/ftpclient/sftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,17 +133,15 @@
 
     def filter_file(
         self,
         filename: str,
         only: Optional[re.Pattern] = None,
         exclude: Optional[re.Pattern] = None,
     ) -> bool:
-        is_filtered = bool(
-            exclude and exclude.match(filename) or only and not only.match(filename)
-        )
+        is_filtered = bool(exclude and exclude.match(filename) or only and not only.match(filename))
         if is_filtered:
             self.log.info("file '%s' filtered", filename)
         return is_filtered
 
     def upload_dir(
         self,
         local_path: str = ".",
```

### Comparing `vbcore-2.2.0rc4/vbcore/net/helpers.py` & `vbcore-2.2.1/vbcore/net/helpers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/net/sendmail.py` & `vbcore-2.2.1/vbcore/net/sendmail.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,17 +65,15 @@
 
     @classmethod
     def add_attachments(cls, message: MIMEBase, files: StrList):
         for filename in files:
             with FileHandler(filename).open_binary() as file:
                 attach = MIMEApplication(file.read())
                 filename = os.path.basename(filename)
-                attach.add_header(
-                    "Content-Disposition", f"attachment; filename={filename}"
-                )
+                attach.add_header("Content-Disposition", f"attachment; filename={filename}")
                 message.attach(attach)
 
     @classmethod
     def message(cls, addresses: MessageAddresses, data: MessageData) -> MIMEMultipart:
         message = MIMEMultipart("alternative")
         message["From"] = addresses.sender
         message["Subject"] = data.subject
```

### Comparing `vbcore-2.2.0rc4/vbcore/net/socks_smtp.py` & `vbcore-2.2.1/vbcore/net/socks_smtp.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,15 @@
         proxy_type: t.Optional[ProxyType] = None,
         **kwargs,
     ):
         self.proxy_args = kwargs
         self.proxy_type = proxy_type
         super().__init__(host, port, local_hostname, timeout, source_address)
 
-    def create_socks_connection(
-        self, host: str, port: int, timeout: int
-    ) -> socks.socksocket:
+    def create_socks_connection(self, host: str, port: int, timeout: int) -> socks.socksocket:
         if self.proxy_type is None:
             # noinspection PyProtectedMember,PyUnresolvedReferences
             get_socket = super()._get_socket  # type: ignore
             return get_socket(host, port, timeout)
 
         if self.debuglevel > 0:
             # noinspection PyUnresolvedReferences
```

### Comparing `vbcore-2.2.0rc4/vbcore/rule_engine/base.py` & `vbcore-2.2.1/vbcore/rule_engine/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/rule_engine/engine.py` & `vbcore-2.2.1/vbcore/rule_engine/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,17 +78,15 @@
 
     def first_match(self, rules: t.List[RuleInfo], data: dict) -> t.Optional[RuleInfo]:
         for result in self.apply(rules, data):
             if result[1] is True:
                 return result[0]
         return None
 
-    def perform_on_match(
-        self, rules: t.List[RuleInfo], data: dict, *args, **kwargs
-    ) -> StrDict:
+    def perform_on_match(self, rules: t.List[RuleInfo], data: dict, *args, **kwargs) -> StrDict:
         results: StrDict = {}
         for rule, result in self.apply(rules, data):
             if rule.evaluate is True or result is True:
                 results[rule.id] = rule.action.perform(
                     data, *args, rule=rule, rule_result=result, **kwargs
                 )
         return results
```

### Comparing `vbcore-2.2.0rc4/vbcore/standalone/scheduler.py` & `vbcore-2.2.1/vbcore/standalone/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,15 @@
         self,
         task: t.Union[t.Callable, str],
         *args,
         params: OptDict = None,
         **kwargs,
     ) -> Job:
         job_id = self.get_id()
-        job = self._scheduler.add_job(
-            task, args=args, kwargs=params, id=job_id, **kwargs
-        )
+        job = self._scheduler.add_job(task, args=args, kwargs=params, id=job_id, **kwargs)
         self.log.debug("added job '%s' with id '%s'", task, job_id)
         return job
 
     def __del__(self):
         try:
             self._scheduler.shutdown()
         except AttributeError:
```

### Comparing `vbcore-2.2.0rc4/vbcore/standalone/wsgi_gunicorn.py` & `vbcore-2.2.1/vbcore/standalone/wsgi_gunicorn.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,17 +47,15 @@
     ):
         load_dotenv()
         self.worker_type = worker_type or WorkerType.DEFAULT
         self.application = app
         self.options = kwargs
         super().__init__()
 
-    def from_env_config(
-        self, conf_key: str, opt_key: str, default: t.Any = MISSING, **kwargs
-    ):
+    def from_env_config(self, conf_key: str, opt_key: str, default: t.Any = MISSING, **kwargs):
         _default = self.options.get(opt_key, default)
         if default == _default == MISSING:
             self.cfg.set(opt_key, config(conf_key, **kwargs))
             return
         try:
             self.cfg.set(opt_key, config(conf_key, **kwargs))
         except UndefinedValueError:
@@ -73,29 +71,21 @@
         self.from_env_config("GU_PROC_NAME", "proc_name", None)
         self.from_env_config("GU_TIMEOUT", "timeout", 60, cast=int)
         self.from_env_config("GU_BACKLOG", "backlog", 2048, cast=int)
         self.from_env_config("GU_KEEP_ALIVE", "keepalive", 5, cast=int)
         self.from_env_config("GU_CHDIR", "chdir", util.getcwd())
         self.from_env_config("GU_USER", "user", os.geteuid())
         self.from_env_config("GU_GROUP", "group", os.getegid())
-        self.from_env_config(
-            "GU_FORWARDED_ALLOW_IPS", "forwarded_allow_ips", "127.0.0.1"
-        )
+        self.from_env_config("GU_FORWARDED_ALLOW_IPS", "forwarded_allow_ips", "127.0.0.1")
         self.from_env_config("GU_WORKER_CLASS", "worker_class", self.worker_type.value)
         self.from_env_config("GU_THREADS", "threads", cpu_count() * 2 + 1, cast=int)
         self.from_env_config("GU_WORKERS", "workers", cpu_count(), cast=int)
-        self.from_env_config(
-            "GU_WORKER_CONNECTIONS", "worker_connections", 1000, cast=int
-        )
-        self.from_env_config(
-            "GU_LOG_LEVEL", "loglevel", "info", cast=Choices(LOG_LEVELS)
-        )
-        self.from_env_config(
-            "GU_ACCESS_LOG_FORMAT", "access_log_format", self.access_log_format
-        )
+        self.from_env_config("GU_WORKER_CONNECTIONS", "worker_connections", 1000, cast=int)
+        self.from_env_config("GU_LOG_LEVEL", "loglevel", "info", cast=Choices(LOG_LEVELS))
+        self.from_env_config("GU_ACCESS_LOG_FORMAT", "access_log_format", self.access_log_format)
 
     @property
     def access_log_format(self):
         return (
             ' %(h)s %(l)s %(u)s %(t)s "%(r)s" %(s)s %(b)s "%(f)s" "%(a)s"'
             " %({x-request-id}i)s %(L)s"  # custom
         )
@@ -194,17 +184,15 @@
     @classmethod
     def _worker_exit(cls, server, worker):
         server.log.debug("worker (pid: %s) exited", worker.pid)
         cls.worker_exit(server, worker)
 
     @classmethod
     def _nworkers_changed(cls, server, new_value, old_value):
-        server.log.info(
-            "number of workers changed from %s to %s", old_value or 0, new_value
-        )
+        server.log.info("number of workers changed from %s to %s", old_value or 0, new_value)
         cls.nworkers_changed(server, new_value, old_value)
 
     @classmethod
     def _on_exit(cls, server):
         server.log.info("server (pid: %s) exited", server.pid)
         cls.on_exit(server)
```

### Comparing `vbcore-2.2.0rc4/vbcore/stringutils/misc.py` & `vbcore-2.2.1/vbcore/stringutils/misc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/stringutils/notations.py` & `vbcore-2.2.1/vbcore/stringutils/notations.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/system.py` & `vbcore-2.2.1/vbcore/system.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/tester/asserter.py` & `vbcore-2.2.1/vbcore/tester/asserter.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,17 +65,15 @@
 
         return _inner
 
     @classmethod
     def fail(cls, that: OptStr = None, error: OptStr = None):
         if not that:
             raise cls.exception(error)
-        raise cls.exception(
-            cls.fail_message.format(that=that, error=f": {error}" if error else "")
-        )
+        raise cls.exception(cls.fail_message.format(that=that, error=f": {error}" if error else ""))
 
     @classmethod
     def assert_that(
         cls,
         func: CallBackType,
         actual: t.Any,
         expected: OptAny = None,
@@ -244,22 +242,18 @@
     def assert_not_empty_dict(cls, actual, error: OptStr = None):
         callback, _ = Operator.NOT_EQUALS.value
         cls.assert_that(callback, actual, {}, f"'{actual}' is not empty dict", error)
 
 
 class JSONValidatorMixin(BaseAssert, JSONSchema):
     @classmethod
-    def assert_json_schema(
-        cls, data: dict, schema: t.Union[dict, str], strict: bool = True
-    ):
+    def assert_json_schema(cls, data: dict, schema: t.Union[dict, str], strict: bool = True):
         cls.assert_different(JSONSchema, object, error="you must install jsonschema")
         if strict and not schema:
-            cls.assert_that(
-                lambda a, e: a is not None, actual=schema, error="Missing schema"
-            )
+            cls.assert_that(lambda a, e: a is not None, actual=schema, error="Missing schema")
         try:
             cls.validate(data, schema, raise_exc=True)
             valid, message = True, None
         except cls.service.ValidationError as exc:
             valid, message = False, cls.error_report(exc, data)
 
         cls.assert_that(
@@ -319,17 +313,15 @@
         opmess = "equals to"
         if greater:
             opmess = "greater than"
         elif lesser:
             opmess = "less than"
 
         that = f"occurrences of '{expected}' in '{actual}' are {opmess} '{occurrences}'"
-        cls.assert_that(
-            find_all, error=error, that=that, actual=actual, expected=expected
-        )
+        cls.assert_that(find_all, error=error, that=that, actual=actual, expected=expected)
 
 
 class HttpAsserter(BaseAssert):
     @classmethod
     def assert_status_code(
         cls,
         response,
@@ -354,17 +346,15 @@
             if in_range is True:
                 message = f"{prefix_mess} in range {list(code)}"
                 cls.assert_range(status_code, code, error=message, closed=True)
             elif is_in is True:
                 message = f"{prefix_mess} one of {code}"
                 cls.assert_in(status_code, code, error=message)
             else:
-                cls.fail(
-                    error="one of (is_in, in_range) must be true if a list of codes is given"
-                )
+                cls.fail(error="one of (is_in, in_range) must be true if a list of codes is given")
         else:
             if greater is True:
                 message = f"{prefix_mess} greater than {code}"
                 cls.assert_greater(status_code, code, error=message)
             elif lesser is True:
                 message = f"{prefix_mess} less than {code}"
                 cls.assert_lesser(status_code, code, error=message)
```

### Comparing `vbcore-2.2.0rc4/vbcore/tester/fetchmail.py` & `vbcore-2.2.1/vbcore/tester/fetchmail.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,17 +15,15 @@
         endpoint: str,
         username: t.Optional[str] = None,
         password: t.Optional[str] = None,
         retry: int = 3,
         wait: int = 1,
         timeout: int = 3,
     ):
-        super().__init__(
-            endpoint, username=username, password=password, timeout=timeout
-        )
+        super().__init__(endpoint, username=username, password=password, timeout=timeout)
         self.retry = retry
         self.wait = wait
 
     def fetch(self, recipient: str, subject: str) -> t.List[ObjectDict]:
         response = []
         resp = self.request("/", raise_on_exc=True)
         emails = resp.body.data if isinstance(resp.body, ObjectDict) else resp
@@ -33,17 +31,15 @@
             if recipient in email.recipients_envelope:
                 if subject and email.subject != subject:
                     continue
                 response.append(email)
 
         return response
 
-    def perform(
-        self, recipient: str, subject: str, delete: bool = True
-    ) -> t.List[ObjectDict]:
+    def perform(self, recipient: str, subject: str, delete: bool = True) -> t.List[ObjectDict]:
         for _ in range(0, self.retry):
             res = self.fetch(recipient, subject)
             if delete:
                 for r in res:
                     self.request(uri=f"/{r.id}", method="DELETE")
             if res:
                 return res
```

### Comparing `vbcore-2.2.0rc4/vbcore/tester/helpers.py` & `vbcore-2.2.1/vbcore/tester/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 from base64 import b64encode
 from unittest.mock import AsyncMock, MagicMock
 
 from vbcore.datastruct import ObjectDict
 from vbcore.tester.fetchmail import FetchMail
 
 
-def fetch_emails(
-    subject: str, recipient: t.Optional[str] = None, **kwargs
-) -> t.List[ObjectDict]:
+def fetch_emails(subject: str, recipient: t.Optional[str] = None, **kwargs) -> t.List[ObjectDict]:
     return FetchMail(**kwargs).perform(recipient=recipient, subject=subject)
 
 
 def basic_auth_header(username: str, password: str) -> t.Dict[str, str]:
     token = b64encode(f"{username}:{password}".encode()).decode()
     return {"Authorization": f"Basic {token}"}
```

### Comparing `vbcore-2.2.0rc4/vbcore/tester/http.py` & `vbcore-2.2.1/vbcore/tester/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,29 +37,25 @@
     def set_auth(self, config):
         config = config or {}
         auth_type = config.get("type")
         if auth_type == "basic" and config.get("username"):
             password = config.get("password") or config["username"]
             self.auth = basic_auth_header(config.get("username"), password)
 
-    def assert_status_code(
-        self, code: int, in_range: bool = False, is_in: bool = False
-    ):
+    def assert_status_code(self, code: int, in_range: bool = False, is_in: bool = False):
         status_code = self.response.status_code
         if type(code) in (list, tuple):
             if in_range:
                 Asserter.assert_range(status_code, code)
             if is_in:
                 Asserter.assert_in(status_code, code)
         else:
             Asserter.assert_equals(status_code, code)
 
-    def assert_header(
-        self, name: str, value: str, is_in: bool = False, regex: bool = False
-    ):
+    def assert_header(self, name: str, value: str, is_in: bool = False, regex: bool = False):
         header = self.response.headers.get(name)
         if is_in:
             Asserter.assert_in(value, header)
         elif regex:
             Asserter.assert_match(value, header)
         else:
             Asserter.assert_equals(header, value)
@@ -208,20 +204,16 @@
         self.perform(req, res)
 
     def test_get(self, res_id, request=None, response=None):
         req, res = self._normalize(request, response, url=self.resource_url(res_id))
         self.perform(req, res)
 
     def test_put(self, res_id, request=None, response=None):
-        req, res = self._normalize(
-            request, response, HttpMethod.PUT, self.resource_url(res_id)
-        )
+        req, res = self._normalize(request, response, HttpMethod.PUT, self.resource_url(res_id))
         self.perform(req, res)
 
     def test_delete(self, res_id, request=None, response=None):
-        req, res = self._normalize(
-            request, response, HttpMethod.DELETE, self.resource_url(res_id)
-        )
+        req, res = self._normalize(request, response, HttpMethod.DELETE, self.resource_url(res_id))
         res.setdefault("status", {"code": httpcode.NO_CONTENT})
         res.setdefault("headers", {})
         res["headers"][HeaderEnum.CONTENT_TYPE] = None
         self.perform(req, res)
```

### Comparing `vbcore-2.2.0rc4/vbcore/tools/cli.py` & `vbcore-2.2.1/vbcore/tools/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,15 @@
 CliOutputFile = partial(CliFile, writable=True)
 CliInputFile = partial(CliFile, exists=True, readable=True)
 CliOutputDir = partial(CliDir, exists=True, writable=True)
 CliInputDir = partial(CliDir, exists=True, readable=True)
 
 
 class Cli:
-    option: t.ClassVar = partial(
-        click.option, show_default=True, show_envvar=True, default=None
-    )
+    option: t.ClassVar = partial(click.option, show_default=True, show_envvar=True, default=None)
     print: t.ClassVar = partial(click.echo, color=True)
     error: t.ClassVar = partial(click.echo, color=True, err=True)
     argument: t.ClassVar = partial(click.argument, required=True)
 
     @classmethod
     def abort(cls, message: str, exit_code: int = -1):
         cls.error(TextBold.red(message))
@@ -42,26 +40,20 @@
 
 class CliOpt:
     string: t.ClassVar = partial(Cli.option, type=click.STRING)
     boolean: t.ClassVar = partial(Cli.option, type=click.BOOL)
     date: t.ClassVar = partial(Cli.option, type=click.DateTime(DateFmt.ISO))
     datetime: t.ClassVar = partial(Cli.option, type=click.DateTime(DateTimeFmt.ISO))
     multi: t.ClassVar = partial(Cli.option, multiple=True, metavar="(multiple)")
-    flag: t.ClassVar = partial(
-        boolean, is_flag=True, default=False, help="[default: False]"
-    )
-    dict: t.ClassVar = partial(
-        multi, default={}, callback=option_as_dict, metavar="KEY[=VAL]"
-    )
+    flag: t.ClassVar = partial(boolean, is_flag=True, default=False, help="[default: False]")
+    dict: t.ClassVar = partial(multi, default={}, callback=option_as_dict, metavar="KEY[=VAL]")
     verbose: t.ClassVar = partial(Cli.option, "-v", "--verbose", count=True)
 
     @classmethod
-    def choice(
-        cls, *args, values: t.Sequence[str], case_sensitive: bool = True, **kwargs
-    ):
+    def choice(cls, *args, values: t.Sequence[str], case_sensitive: bool = True, **kwargs):
         return Cli.option(*args, type=click.Choice(values, case_sensitive), **kwargs)
 
     @classmethod
     def integer(
         cls,
         *args,
         min_val: OptInt = None,
```

### Comparing `vbcore-2.2.0rc4/vbcore/tools/crypto.py` & `vbcore-2.2.1/vbcore/tools/crypto.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/tools/database.py` & `vbcore-2.2.1/vbcore/tools/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,24 +27,24 @@
         graph = model_to_uml(from_models)
     elif from_database:
         graph = db_to_schema(from_database)
     else:
         raise click.UsageError("One of -m or -d are required")
 
     try:
-        graph.write_png(file)  # pylint: disable=E1101
+        graph.write_png(file)  # pylint: disable=no-member
     except OSError as exc:
         Cli.abort(f"{str(exc)}\ntry to install 'graphviz'")
 
 
 @main.command(name="dump-ddl")
 @CliOpt.choice("--dialect", default="sqlite", values=DIALECTS)
 @CliReqOpt.string("-m", "--metadata", help="metadata module")
 def dump_ddl(dialect, metadata):
-    """Dumps the CREATE table statements for a given metadata"""
+    """Dumps the DDL statements for a given metadata"""
     dump_model_ddl(metadata, dialect)
 
 
 @main.command(name="mysql-backup")
 @Cli.argument("db_url")
 @CliOpt.string("--folder", default=".", type=CliOutputDir())
 @CliOpt.multi("-i", "--ignore-database")
```

### Comparing `vbcore-2.2.0rc4/vbcore/tools/entrypoint.py` & `vbcore-2.2.1/vbcore/tools/entrypoint.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/tools/ftpclient.py` & `vbcore-2.2.1/vbcore/tools/ftpclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import functools
 import re
 from typing import TYPE_CHECKING, Union
 
 import click
 
 from vbcore.datastruct.lazy import LazyImporter
+from vbcore.loggers import Log
 from vbcore.net.ftpclient.legacy import FTPHandler, FTPOptions
 from vbcore.tools.cli import CliInputDir, CliInputFile, CliOpt, CliOutputFile, CliReqOpt
 
 if TYPE_CHECKING:
     from vbcore.net.ftpclient.sftp import SFTPHandler, SFTPOptions
 else:
     SFTPHandler, SFTPOptions = LazyImporter.import_many(
@@ -17,29 +18,31 @@
         message="you must install vbcore[net]",
     )
 
 main = click.Group(name="ftpclient", help="ftp client handler")
 
 
 def factory(options: dict) -> Union[FTPHandler, SFTPHandler]:
-    no_secure = options.pop("no_secure", False)
-    if no_secure:
-        return FTPHandler(FTPOptions.from_dict(**options))
-    return SFTPHandler(SFTPOptions.from_dict(**options))
+    over_ssh = options.pop("ssh", False)
+    if over_ssh:
+        return SFTPHandler(SFTPOptions.from_dict(**options))
+    return FTPHandler(FTPOptions.from_dict(**options))
 
 
 def common_options(func):
     @CliOpt.flag("--debug", envvar="FTP_DEBUG")
     @CliOpt.integer("--timeout", envvar="FTP_TIMEOUT", default=300)
-    @CliOpt.flag("--no-secure", envvar="FTP_NO_SECURE")
+    @CliOpt.flag("--ssh", envvar="FTP_OVER_SSH")
+    @CliOpt.flag("--tls", envvar="FTP_OVER_TLS")
     @CliReqOpt.string("-H", "--host", envvar="FTP_HOST")
     @CliReqOpt.integer("-P", "--port", envvar="FTP_PORT")
     @CliOpt.string("-u", "--user", envvar="FTP_USER")
     @CliOpt.string("-p", "--password", envvar="FTP_PASSWORD")
     @CliOpt.flag("--debug", envvar="FTP_DEBUG")
+    @CliOpt.string("--encoding", envvar="FTP_ENCODING", default="utf-8")
     @CliOpt.string(
         "-P",
         "--private-key-file",
         envvar="FTP_PK_FILE",
         type=CliInputFile(),
     )
     @CliOpt.choice(
@@ -57,46 +60,50 @@
 
 
 @main.command(name="download", help="download a single file")
 @CliReqOpt.string("-r", "--remote")
 @CliReqOpt.string("-l", "--local", type=CliOutputFile())
 @common_options
 def download(remote, local, **kwargs):
-    factory(kwargs).download_file(remote, local)
+    with Log.execution_time():
+        factory(kwargs).download_file(remote, local)
 
 
 @main.command(name="upload", help="upload a single file")
 @CliReqOpt.string("-r", "--remote")
 @CliReqOpt.string("-l", "--local", type=CliInputFile())
 @common_options
 def upload(remote, local, **kwargs):
-    factory(kwargs).upload_file(local, remote)
+    with Log.execution_time():
+        factory(kwargs).upload_file(local, remote)
 
 
 @main.command(name="download-dir", help="download files from remote directory")
 @CliOpt.string("-r", "--remote", default=".")
 @CliOpt.string("-l", "--local", type=CliInputDir(), default=".")
 @CliOpt.string("--only")
 @CliOpt.string("--exclude")
 @common_options
 def download_dir(remote, local, only, exclude, **kwargs):
-    factory(kwargs).download_dir(
-        remote_path=remote,
-        local_path=local,
-        only=re.compile(only) if only else None,
-        exclude=re.compile(exclude) if exclude else None,
-    )
+    with Log.execution_time():
+        factory(kwargs).download_dir(
+            remote_path=remote,
+            local_path=local,
+            only=re.compile(only) if only else None,
+            exclude=re.compile(exclude) if exclude else None,
+        )
 
 
 @main.command(name="upload-dir", help="upload files from local directory")
 @CliOpt.string("-r", "--remote", default=".")
 @CliOpt.string("-l", "--local", type=CliInputDir(), default=".")
 @CliOpt.string("--only")
 @CliOpt.string("--exclude")
 @common_options
 def upload_dir(remote, local, only, exclude, **kwargs):
-    factory(kwargs).upload_dir(
-        local_path=local,
-        remote_path=remote,
-        only=re.compile(only) if only else None,
-        exclude=re.compile(exclude) if exclude else None,
-    )
+    with Log.execution_time():
+        factory(kwargs).upload_dir(
+            local_path=local,
+            remote_path=remote,
+            only=re.compile(only) if only else None,
+            exclude=re.compile(exclude) if exclude else None,
+        )
```

### Comparing `vbcore-2.2.0rc4/vbcore/tools/initializer/init.py` & `vbcore-2.2.1/vbcore/tools/initializer/init.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.gitignore` & `vbcore-2.2.1/vbcore/tools/initializer/skeleton/.gitignore`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/.pylintrc` & `vbcore-2.2.1/vbcore/tools/initializer/skeleton/.pylintrc`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/Makefile` & `vbcore-2.2.1/vbcore/tools/initializer/skeleton/Makefile`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/README.md` & `vbcore-2.2.1/vbcore/tools/initializer/skeleton/README.md`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml` & `vbcore-2.2.1/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/liccheck.ini` & `vbcore-2.2.1/vbcore/tools/initializer/skeleton/liccheck.ini`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/tools/initializer/skeleton/setup.py` & `vbcore-2.2.1/vbcore/tools/initializer/skeleton/setup.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/tools/scheduler.py` & `vbcore-2.2.1/vbcore/tools/scheduler.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/tools/sendmail.py` & `vbcore-2.2.1/vbcore/tools/sendmail.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/tools/wsgi_gunicorn.py` & `vbcore-2.2.1/vbcore/tools/wsgi_gunicorn.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/types.py` & `vbcore-2.2.1/vbcore/types.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore/yaml.py` & `vbcore-2.2.1/vbcore/yaml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.2.0rc4/vbcore.egg-info/SOURCES.txt` & `vbcore-2.2.1/vbcore.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -81,18 +81,23 @@
 vbcore/datastruct/orderer_set.py
 vbcore/db/__init__.py
 vbcore/db/events.py
 vbcore/db/exceptions.py
 vbcore/db/listener.py
 vbcore/db/mixins.py
 vbcore/db/mysql_dumper.py
+vbcore/db/repo.py
 vbcore/db/schema.py
 vbcore/db/sqla.py
 vbcore/db/support.py
+vbcore/db/types.py
 vbcore/db/views.py
+vbcore/db/schema_display/__init__.py
+vbcore/db/schema_display/db_diagram.py
+vbcore/db/schema_display/model_diagram.py
 vbcore/dictutils/__init__.py
 vbcore/dictutils/flatter_dict.py
 vbcore/dictutils/misc.py
 vbcore/excel/__init__.py
 vbcore/excel/report.py
 vbcore/http/__init__.py
 vbcore/http/batch.py
```

### Comparing `vbcore-2.2.0rc4/vbcore.egg-info/requires.txt` & `vbcore-2.2.1/vbcore.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 click
 python-dateutil
 python-decouple
 python-dotenv
 pyyaml
 psutil
 sqlalchemy
-sqlalchemy_schemadisplay
+graphviz
+pydot
 argon2-cffi
 bcrypt
 aiohttp
 requests
 user_agents
 pysocks
 paramiko
@@ -35,15 +36,16 @@
 
 [crypto]
 argon2-cffi
 bcrypt
 
 [db]
 sqlalchemy
-sqlalchemy_schemadisplay
+graphviz
+pydot
 
 [extra]
 chardet
 jsonschema
 rule_engine
 gql
 gunicorn
```

