# Comparing `tmp/tlslite-ng-0.8.0a44.tar.gz` & `tmp/tlslite-ng-0.8.0a45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlslite-ng-0.8.0a44.tar", last modified: Fri Jun  9 15:24:55 2023, max compression
+gzip compressed data, was "tlslite-ng-0.8.0a45.tar", last modified: Tue Aug  1 15:43:28 2023, max compression
```

## Comparing `tlslite-ng-0.8.0a44.tar` & `tlslite-ng-0.8.0a45.tar`

### file list

```diff
@@ -1,503 +1,503 @@
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.286687 tlslite-ng-0.8.0a44/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)       34 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a44/.checkignore
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      715 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/.codeclimate.yml
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.223686 tlslite-ng-0.8.0a44/.github/
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.227687 tlslite-ng-0.8.0a44/.github/workflows/
--rw-r--r--   0 hkario   (20970) hkario   (20970)    22563 2023-06-09 15:16:43.000000 tlslite-ng-0.8.0a44/.github/workflows/ci.yml
--rw-r--r--   0 hkario   (20970) hkario   (20970)      128 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/.gitignore
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      177 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a44/.landscape.yaml
--rw-rw-r--   0 hkario   (20970) hkario   (20970)       28 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a44/.pep257
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6804 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/.travis.yml
--rw-r--r--   0 hkario   (20970) hkario   (20970)     5749 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/CONTRIBUTING.md
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    27882 2015-08-12 15:24:17.000000 tlslite-ng-0.8.0a44/LICENSE
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      131 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/MANIFEST.in
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4231 2021-07-27 19:18:05.000000 tlslite-ng-0.8.0a44/Makefile
--rw-r--r--   0 hkario   (20970) hkario   (20970)     3337 2023-06-09 15:24:55.285687 tlslite-ng-0.8.0a44/PKG-INFO
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2099 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/README
--rw-r--r--   0 hkario   (20970) hkario   (20970)    39628 2023-06-09 15:23:17.000000 tlslite-ng-0.8.0a44/README.md
--rw-r--r--   0 hkario   (20970) hkario   (20970)     2199 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/SECURITY.md
--rw-r--r--   0 hkario   (20970) hkario   (20970)      209 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/build-requirements-2.6.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      149 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/build-requirements-2.7.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      224 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/build-requirements-3.3.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      140 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/build-requirements-3.4.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)       79 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/build-requirements.txt
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.234686 tlslite-ng-0.8.0a44/docs/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     7622 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/Makefile
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.223686 tlslite-ng-0.8.0a44/docs/_build/
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.242687 tlslite-ng-0.8.0a44/docs/_build/html/
--rw-r--r--   0 hkario   (20970) hkario   (20970)      230 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/.buildinfo
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.248687 tlslite-ng-0.8.0a44/docs/_build/html/_sources/
--rw-r--r--   0 hkario   (20970) hkario   (20970)      445 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)       58 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      146 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.api.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      225 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.basedb.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.bufferedsocket.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      177 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.checker.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      142 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.constants.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.defragmenter.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      143 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.dh.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      183 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.errors.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.extensions.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.handshakehashes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      163 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.handshakehelpers.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.handshakesettings.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      233 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.integration.asyncstatemachine.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.integration.clienthelper.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      224 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.integration.httptlsconnection.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.integration.imap4_tls.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.integration.pop3_tls.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      592 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.integration.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.integration.smtp_tls.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      251 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.integration.tlsasyncdispatchermixin.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      242 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.integration.tlssocketservermixin.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.integration.xmlrpcserver.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.integration.xmlrpctransport.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.keyexchange.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.mathtls.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      189 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.messages.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.messagesocket.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.recordlayer.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      785 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.session.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      208 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.sessioncache.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.tlsconnection.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.tlsrecordlayer.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.aes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.aesgcm.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.asn1parser.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.chacha.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      215 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.chacha20_poly1305.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.cipherfactory.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.codec.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.compat.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.constanttime.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.cryptomath.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.datefuncs.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2019-01-22 17:40:43.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.deprecations.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.dns_utils.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.ecc.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.ecdsakey.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.keyfactory.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      170 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.lists.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.openssl_aes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.openssl_rc4.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.openssl_rsakey.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.openssl_tripledes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.pem.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.poly1305.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.pycrypto_aes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.pycrypto_aesgcm.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.pycrypto_rc4.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.pycrypto_rsakey.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.pycrypto_tripledes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.python_aes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.python_aesgcm.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.python_chacha20_poly1305.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.python_rc4.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.python_rsakey.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.rc4.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.rijndael.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.rsakey.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)     1316 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.tackwrapper.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.tlshashlib.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.tripledes.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.x25519.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      202 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.verifierdb.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      158 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.x509.rst.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.x509certchain.rst.txt
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.250687 tlslite-ng-0.8.0a44/docs/_build/html/_static/
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4418 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15180 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.250687 tlslite-ng-0.8.0a44/docs/_build/html/_static/css/
--rw-r--r--   0 hkario   (20970) hkario   (20970)     2922 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/css/badge_only.css
--rw-r--r--   0 hkario   (20970) hkario   (20970)   128848 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 hkario   (20970) hkario   (20970)     8171 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/doctools.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)      429 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)      286 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/file.png
--rw-r--r--   0 hkario   (20970) hkario   (20970)   288580 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/jquery-3.6.0.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)    89501 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/jquery.js
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.250687 tlslite-ng-0.8.0a44/docs/_build/html/_static/js/
--rw-r--r--   0 hkario   (20970) hkario   (20970)      934 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)     5023 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4758 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/language_data.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)       90 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/minus.png
--rw-r--r--   0 hkario   (20970) hkario   (20970)       90 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/plus.png
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4846 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/pygments.css
--rw-r--r--   0 hkario   (20970) hkario   (20970)    17088 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)    68420 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)    19530 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a44/docs/_build/html/_static/underscore.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)   252491 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/genindex.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4704 2023-06-09 15:24:50.000000 tlslite-ng-0.8.0a44/docs/_build/html/index.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7955 2023-06-09 15:24:50.000000 tlslite-ng-0.8.0a44/docs/_build/html/modules.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11361 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/objects.inv
--rw-r--r--   0 hkario   (20970) hkario   (20970)    21834 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/py-modindex.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     3593 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/search.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)   161575 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/searchindex.js
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7635 2023-06-09 15:24:50.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.api.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14507 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.basedb.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15038 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.bufferedsocket.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12591 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.checker.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)   278477 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.constants.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12414 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.defragmenter.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     9820 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.dh.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    40595 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.errors.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)   163760 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.extensions.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    13049 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.handshakehashes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14256 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.handshakehelpers.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    33544 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.handshakesettings.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    19608 2023-06-09 15:24:50.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15981 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.asyncstatemachine.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    13925 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.clienthelper.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6874 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15108 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.httptlsconnection.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14811 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.imap4_tls.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12135 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.pop3_tls.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11674 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.smtp_tls.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    20642 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.tlsasyncdispatchermixin.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12512 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.tlssocketservermixin.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11939 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.xmlrpcserver.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15905 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.xmlrpctransport.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    58370 2023-06-09 15:24:51.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.keyexchange.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    67608 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.mathtls.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)   143539 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.messages.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    18129 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.messagesocket.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    35655 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.recordlayer.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    20952 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.session.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11817 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.sessioncache.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    47436 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.tlsconnection.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    43739 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.tlsrecordlayer.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7786 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.aes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     8459 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.aesgcm.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    13626 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.asn1parser.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12725 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.chacha.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10067 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.chacha20_poly1305.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    18141 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.cipherfactory.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    33216 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.codec.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    16967 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.compat.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    18018 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.constanttime.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    34260 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.cryptomath.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10078 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.datefuncs.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14255 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.deprecations.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6466 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.dns_utils.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7761 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.ecc.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    21776 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.ecdsakey.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10584 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    19234 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.keyfactory.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     9265 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.lists.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    16689 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.openssl_aes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10907 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.openssl_rc4.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    17482 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.openssl_rsakey.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11632 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.openssl_tripledes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14357 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.pem.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     8842 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.poly1305.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10515 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.pycrypto_aes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7817 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.pycrypto_aesgcm.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10063 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.pycrypto_rc4.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14657 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.pycrypto_rsakey.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10746 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.pycrypto_tripledes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     8560 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.python_aes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     5897 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.python_aesgcm.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6017 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.python_chacha20_poly1305.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10047 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.python_rc4.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14650 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.python_rsakey.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7538 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.rc4.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11634 2023-06-09 15:24:52.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.rijndael.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    38486 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.rsakey.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     5238 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.tackwrapper.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6794 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.tlshashlib.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7979 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.tripledes.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10907 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.x25519.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15655 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.verifierdb.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    14761 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.x509.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15974 2023-06-09 15:24:53.000000 tlslite-ng-0.8.0a44/docs/_build/html/tlslite.x509certchain.html
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10006 2023-06-09 15:20:46.000000 tlslite-ng-0.8.0a44/docs/conf.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      445 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/docs/index.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     7740 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/make.bat
--rw-rw-r--   0 hkario   (20970) hkario   (20970)       58 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/modules.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      146 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.api.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      225 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.basedb.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.bufferedsocket.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      177 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.checker.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      142 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.constants.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.defragmenter.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      143 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.dh.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      183 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.errors.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.extensions.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.handshakehashes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      163 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.handshakehelpers.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.handshakesettings.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      233 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.integration.asyncstatemachine.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.integration.clienthelper.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      224 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.integration.httptlsconnection.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.integration.imap4_tls.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.integration.pop3_tls.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      592 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.integration.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.integration.smtp_tls.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      251 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.integration.tlsasyncdispatchermixin.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      242 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.integration.tlssocketservermixin.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.integration.xmlrpcserver.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.integration.xmlrpctransport.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.keyexchange.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.mathtls.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      189 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.messages.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.messagesocket.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.recordlayer.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      785 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.session.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      208 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.sessioncache.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.tlsconnection.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.tlsrecordlayer.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.aes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.aesgcm.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.asn1parser.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.chacha.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      215 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.chacha20_poly1305.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.cipherfactory.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.codec.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.compat.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.constanttime.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.cryptomath.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.datefuncs.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2019-01-22 17:40:43.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.deprecations.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.dns_utils.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.ecc.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.ecdsakey.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.keyfactory.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      170 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.lists.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.openssl_aes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.openssl_rc4.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.openssl_rsakey.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.openssl_tripledes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.pem.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.poly1305.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.pycrypto_aes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.pycrypto_aesgcm.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.pycrypto_rc4.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.pycrypto_rsakey.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.pycrypto_tripledes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.python_aes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.python_aesgcm.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.python_chacha20_poly1305.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.python_rc4.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.python_rsakey.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.rc4.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.rijndael.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.rsakey.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1316 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.tackwrapper.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.tlshashlib.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.tripledes.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.utils.x25519.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      202 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.verifierdb.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      158 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.x509.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/docs/tlslite.x509certchain.rst
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    10645 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/pylintrc
--rw-r--r--   0 hkario   (20970) hkario   (20970)       16 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/requirements.txt
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.251686 tlslite-ng-0.8.0a44/scripts/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1903 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/scripts/speed.py
--rwxr-xr-x   0 hkario   (20970) hkario   (20970)    25679 2023-02-10 13:29:50.000000 tlslite-ng-0.8.0a44/scripts/tls.py
--rwxrwxr-x   0 hkario   (20970) hkario   (20970)     3774 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/scripts/tlsdb.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)       38 2023-06-09 15:24:55.286687 tlslite-ng-0.8.0a44/setup.cfg
--rwxr-xr-x   0 hkario   (20970) hkario   (20970)     1931 2023-06-09 15:21:00.000000 tlslite-ng-0.8.0a44/setup.py
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.261687 tlslite-ng-0.8.0a44/tests/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      124 2015-10-14 14:17:40.000000 tlslite-ng-0.8.0a44/tests/.coverage
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tests/TACK1.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tests/TACK2.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tests/TACK_Key1.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tests/TACK_Key2.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      650 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a44/tests/TACKs.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a44/tests/TACKunrelated.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      579 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/clientECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      241 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/clientECKey.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)      485 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tests/clientEd25519Cert.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)      119 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tests/clientEd25519Key.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      924 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a44/tests/clientX509Cert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      891 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a44/tests/clientX509Key.pem
--rwxrwxr-x   0 hkario   (20970) hkario   (20970)      327 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tests/httpsclient.py
--rwxrwxr-x   0 hkario   (20970) hkario   (20970)      113 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tests/httpsserver.sh
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      152 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tests/index.html
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      579 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverBrainpoolP256r1ECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      227 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverBrainpoolP256r1ECKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      664 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverBrainpoolP384r1ECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      292 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverBrainpoolP384r1ECKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      757 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverBrainpoolP512r1ECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      361 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverBrainpoolP512r1ECKey.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6628 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tests/serverDSACert.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)     1224 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tests/serverDSAKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      554 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2261 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverECDSANonCACert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      302 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverECDSANonCAKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      241 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverECKey.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)      489 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tests/serverEd25519Cert.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)      119 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tests/serverEd25519Key.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)      591 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tests/serverEd448Cert.pem
--rw-r--r--   0 hkario   (20970) hkario   (20970)      156 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tests/serverEd448Key.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      660 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverP384ECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      306 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverP384ECKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      761 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverP521ECCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      384 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverP521ECKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4302 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverRSANonCACert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1675 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tests/serverRSANonCAKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1224 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tests/serverRSAPSSCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1700 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tests/serverRSAPSSKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1229 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tests/serverRSAPSSSigCert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1704 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tests/serverRSAPSSSigKey.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1094 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tests/serverX509Cert.pem
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1704 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tests/serverX509Key.pem
--rwxr-xr-x   0 hkario   (20970) hkario   (20970)   114602 2023-02-10 13:29:50.000000 tlslite-ng-0.8.0a44/tests/tlstest.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    24576 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tests/verifierDB
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.264687 tlslite-ng-0.8.0a44/tlslite/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      878 2021-08-06 12:04:22.000000 tlslite-ng-0.8.0a44/tlslite/__init__.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     1400 2023-06-09 15:21:10.000000 tlslite-ng-0.8.0a44/tlslite/api.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4092 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/basedb.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2836 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/bufferedsocket.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2725 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tlslite/checker.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    66261 2023-02-10 13:29:50.000000 tlslite-ng-0.8.0a44/tlslite/constants.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4430 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/defragmenter.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      914 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tlslite/dh.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6838 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/errors.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    68340 2023-02-10 13:29:50.000000 tlslite-ng-0.8.0a44/tlslite/extensions.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4137 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/handshakehashes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6725 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/handshakehelpers.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    32163 2023-02-10 13:29:50.000000 tlslite-ng-0.8.0a44/tlslite/handshakesettings.py
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.264687 tlslite-ng-0.8.0a44/tlslite/integration/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      396 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tlslite/integration/__init__.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     7202 2019-01-22 17:40:44.000000 tlslite-ng-0.8.0a44/tlslite/integration/asyncstatemachine.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tlslite/integration/clienthelper.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4514 2018-07-30 10:15:07.000000 tlslite-ng-0.8.0a44/tlslite/integration/httptlsconnection.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3680 2021-01-14 12:41:41.000000 tlslite-ng-0.8.0a44/tlslite/integration/imap4_tls.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3199 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tlslite/integration/pop3_tls.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3026 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tlslite/integration/smtp_tls.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4964 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/integration/tlsasyncdispatchermixin.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2320 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/integration/tlssocketservermixin.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1909 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tlslite/integration/xmlrpcserver.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     5332 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/integration/xmlrpctransport.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    43331 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/keyexchange.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    45528 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/mathtls.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    77918 2023-02-10 13:29:50.000000 tlslite-ng-0.8.0a44/tlslite/messages.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6250 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/messagesocket.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     5933 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/ocsp.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    51706 2021-06-07 14:03:52.000000 tlslite-ng-0.8.0a44/tlslite/recordlayer.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6906 2023-02-10 13:29:50.000000 tlslite-ng-0.8.0a44/tlslite/session.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3552 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tlslite/sessioncache.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3545 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/signed.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)   212380 2023-02-10 13:29:50.000000 tlslite-ng-0.8.0a44/tlslite/tlsconnection.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    60589 2023-02-10 13:29:50.000000 tlslite-ng-0.8.0a44/tlslite/tlsrecordlayer.py
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.269687 tlslite-ng-0.8.0a44/tlslite/utils/
--rw-r--r--   0 hkario   (20970) hkario   (20970)      837 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/__init__.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1222 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/aes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4966 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/aesccm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6866 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/aesgcm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3802 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/asn1parser.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4821 2017-02-17 16:14:00.000000 tlslite-ng-0.8.0a44/tlslite/utils/chacha.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3123 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/chacha20_poly1305.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     5957 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/cipherfactory.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    15543 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/codec.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7229 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/compat.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6399 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/constanttime.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12585 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/cryptomath.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2278 2016-07-29 18:32:10.000000 tlslite-ng-0.8.0a44/tlslite/utils/datefuncs.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     8742 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/deprecations.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1468 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tlslite/utils/dns_utils.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     3144 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/dsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2676 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/ecc.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     5590 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/ecdsakey.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4766 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/eddsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      483 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/format_output.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10460 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/keyfactory.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1549 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/lists.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4539 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/openssl_aes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      733 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/openssl_aesccm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      664 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/openssl_aesgcm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      709 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tlslite/utils/openssl_rc4.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     7156 2023-06-09 15:16:43.000000 tlslite-ng-0.8.0a44/tlslite/utils/openssl_rsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1801 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/openssl_tripledes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3667 2016-07-29 18:32:10.000000 tlslite-ng-0.8.0a44/tlslite/utils/pem.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1504 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tlslite/utils/poly1305.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      840 2018-03-27 13:27:30.000000 tlslite-ng-0.8.0a44/tlslite/utils/pycrypto_aes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      446 2015-08-12 15:24:17.000000 tlslite-ng-0.8.0a44/tlslite/utils/pycrypto_aesgcm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      764 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tlslite/utils/pycrypto_rc4.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2644 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/pycrypto_rsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      872 2018-03-27 13:27:30.000000 tlslite-ng-0.8.0a44/tlslite/utils/pycrypto_tripledes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3667 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/python_aes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      271 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/python_aesccm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      268 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/python_aesgcm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      316 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a44/tlslite/utils/python_chacha20_poly1305.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     3777 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/python_dsakey.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     3388 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/python_ecdsakey.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     2101 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/python_eddsakey.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    11034 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/python_key.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1073 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/tlslite/utils/python_rc4.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     4691 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/python_rsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    16932 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/python_tripledes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      561 2015-08-12 15:24:17.000000 tlslite-ng-0.8.0a44/tlslite/utils/rc4.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    53143 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/rijndael.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    26348 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/utils/rsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      334 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a44/tlslite/utils/tackwrapper.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1024 2016-01-08 16:25:14.000000 tlslite-ng-0.8.0a44/tlslite/utils/tlshashlib.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3079 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/utils/tlshmac.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      870 2018-02-01 13:32:10.000000 tlslite-ng-0.8.0a44/tlslite/utils/tripledes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3255 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tlslite/utils/x25519.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3702 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/tlslite/verifierdb.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    10386 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/tlslite/x509.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3323 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/tlslite/x509certchain.py
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.269687 tlslite-ng-0.8.0a44/tlslite_ng.egg-info/
--rw-r--r--   0 hkario   (20970) hkario   (20970)     3337 2023-06-09 15:24:54.000000 tlslite-ng-0.8.0a44/tlslite_ng.egg-info/PKG-INFO
--rw-r--r--   0 hkario   (20970) hkario   (20970)    18045 2023-06-09 15:24:55.000000 tlslite-ng-0.8.0a44/tlslite_ng.egg-info/SOURCES.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)        1 2023-06-09 15:24:54.000000 tlslite-ng-0.8.0a44/tlslite_ng.egg-info/dependency_links.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)       16 2023-06-09 15:24:54.000000 tlslite-ng-0.8.0a44/tlslite_ng.egg-info/requires.txt
--rw-r--r--   0 hkario   (20970) hkario   (20970)        8 2023-06-09 15:24:54.000000 tlslite-ng-0.8.0a44/tlslite_ng.egg-info/top_level.txt
-drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-06-09 15:24:55.285687 tlslite-ng-0.8.0a44/unit_tests/
--rw-rw-r--   0 hkario   (20970) hkario   (20970)        0 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/unit_tests/__init__.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3336 2018-06-29 15:54:59.000000 tlslite-ng-0.8.0a44/unit_tests/mocksock.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    18932 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tls1_3_vectors.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     4414 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_bufferedsocket.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    12726 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_constants.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6979 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_defragmenter.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2245 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_dh.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    95114 2023-02-10 13:29:50.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_extensions.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3383 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_handshakehashes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    17133 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_handshakehelpers.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    15363 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_handshakesettings.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)   126491 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_keyexchange.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     9991 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_mathtls.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)   148581 2023-02-10 13:29:50.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_messages.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    12586 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_messagesocket.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    25676 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_ocsp.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)   117035 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_recordlayer.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1834 2016-04-14 13:26:36.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_session.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1275 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_sessioncache.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2611 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_signed.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    19118 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_tlsconnection.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    36862 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_tlsrecordlayer.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2931 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_aes_split.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    10191 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_aescbc.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    22930 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_aesccm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    10558 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_aesctr.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    14665 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_aesgcm.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2143 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_asn1.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    15890 2016-01-07 16:34:17.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_chacha.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     5662 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_chacha20_poly1305.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    11423 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_codec.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      789 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_compat.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    16432 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_constanttime.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    26699 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_cryptomath.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3442 2016-01-08 16:25:14.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_cryptomath_m2crypto.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    16100 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_deprecations.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1286 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_dns_utils.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     8381 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_ecc.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     2228 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_ecdsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    13810 2019-01-22 17:40:44.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_keyfactory.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     1694 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_lists.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     7573 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_poly1305.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)    21266 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_python_dsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3998 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_python_ecdsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     7738 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_python_key.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     6754 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_rijndael.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)   170557 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_rsakey.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)      765 2016-01-08 16:25:14.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_tlshashlib.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    20642 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_tripledes.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)     3178 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_tripledes_split.py
--rw-rw-r--   0 hkario   (20970) hkario   (20970)    14421 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_x25519.py
--rw-r--r--   0 hkario   (20970) hkario   (20970)     6997 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a44/unit_tests/test_tlslite_x509.py
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.208925 tlslite-ng-0.8.0a45/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)       34 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/.checkignore
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      715 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/.codeclimate.yml
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.142925 tlslite-ng-0.8.0a45/.github/
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.148925 tlslite-ng-0.8.0a45/.github/workflows/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    23071 2023-07-11 11:45:08.000000 tlslite-ng-0.8.0a45/.github/workflows/ci.yml
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      128 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/.gitignore
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      177 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/.landscape.yaml
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)       28 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/.pep257
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6804 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/.travis.yml
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     5749 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/CONTRIBUTING.md
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    27882 2015-08-12 15:24:17.000000 tlslite-ng-0.8.0a45/LICENSE
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      131 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/MANIFEST.in
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4231 2021-07-27 19:18:05.000000 tlslite-ng-0.8.0a45/Makefile
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     3337 2023-08-01 15:43:28.208925 tlslite-ng-0.8.0a45/PKG-INFO
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2099 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/README
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    39629 2023-08-01 15:39:53.000000 tlslite-ng-0.8.0a45/README.md
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     2199 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/SECURITY.md
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      209 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/build-requirements-2.6.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      149 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/build-requirements-2.7.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      224 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/build-requirements-3.3.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      140 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/build-requirements-3.4.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       79 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/build-requirements.txt
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.155925 tlslite-ng-0.8.0a45/docs/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     7622 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/Makefile
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.142925 tlslite-ng-0.8.0a45/docs/_build/
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.164925 tlslite-ng-0.8.0a45/docs/_build/html/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      230 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/.buildinfo
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.171925 tlslite-ng-0.8.0a45/docs/_build/html/_sources/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      445 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       58 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      146 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.api.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      225 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.basedb.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.bufferedsocket.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      177 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.checker.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      142 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.constants.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.defragmenter.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      143 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.dh.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      183 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.errors.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.extensions.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.handshakehashes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      163 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.handshakehelpers.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.handshakesettings.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      233 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.asyncstatemachine.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.clienthelper.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      224 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.httptlsconnection.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.imap4_tls.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.pop3_tls.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      592 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.smtp_tls.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      251 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.tlsasyncdispatchermixin.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      242 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.tlssocketservermixin.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.xmlrpcserver.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.xmlrpctransport.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.keyexchange.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.mathtls.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      189 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.messages.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.messagesocket.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.recordlayer.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      785 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.session.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      208 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.sessioncache.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.tlsconnection.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.tlsrecordlayer.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.aes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.aesgcm.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.asn1parser.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.chacha.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      215 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.chacha20_poly1305.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.cipherfactory.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.codec.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.compat.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.constanttime.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.cryptomath.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.datefuncs.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2019-01-22 17:40:43.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.deprecations.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.dns_utils.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.ecc.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.ecdsakey.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.keyfactory.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      170 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.lists.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.openssl_aes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.openssl_rc4.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.openssl_rsakey.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.openssl_tripledes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.pem.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.poly1305.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.pycrypto_aes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.pycrypto_aesgcm.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.pycrypto_rc4.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.pycrypto_rsakey.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.pycrypto_tripledes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.python_aes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.python_aesgcm.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.python_chacha20_poly1305.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.python_rc4.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.python_rsakey.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.rc4.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.rijndael.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.rsakey.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     1316 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.tackwrapper.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.tlshashlib.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.tripledes.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.x25519.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      202 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.verifierdb.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      158 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.x509.rst.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.x509certchain.rst.txt
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.172925 tlslite-ng-0.8.0a45/docs/_build/html/_static/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4418 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15180 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.172925 tlslite-ng-0.8.0a45/docs/_build/html/_static/css/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     2922 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/css/badge_only.css
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   128848 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     8171 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      429 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      286 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/file.png
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   288580 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/jquery-3.6.0.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    89501 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/jquery.js
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.173925 tlslite-ng-0.8.0a45/docs/_build/html/_static/js/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      934 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     5023 2022-07-22 22:37:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4758 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       90 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/minus.png
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       90 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/plus.png
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4846 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    17088 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    68420 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    19530 2023-02-01 14:49:18.000000 tlslite-ng-0.8.0a45/docs/_build/html/_static/underscore.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   252791 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/genindex.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4704 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/index.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7955 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/modules.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11369 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/objects.inv
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    21834 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/py-modindex.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     3593 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/search.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   161631 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/searchindex.js
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7635 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.api.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14507 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.basedb.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15038 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.bufferedsocket.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12591 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.checker.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   278477 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.constants.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12414 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.defragmenter.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     9820 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.dh.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    40595 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.errors.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   164652 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.extensions.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    13049 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.handshakehashes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14256 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.handshakehelpers.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    33544 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.handshakesettings.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    19608 2023-08-01 15:43:23.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15981 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.asyncstatemachine.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    13925 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.clienthelper.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6874 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15108 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.httptlsconnection.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14811 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.imap4_tls.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12135 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.pop3_tls.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11674 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.smtp_tls.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    20642 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.tlsasyncdispatchermixin.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12512 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.tlssocketservermixin.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11939 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.xmlrpcserver.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15905 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.xmlrpctransport.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    58370 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.keyexchange.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    67608 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.mathtls.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   143539 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.messages.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    18129 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.messagesocket.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    35655 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.recordlayer.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    20952 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.session.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11817 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.sessioncache.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    47436 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.tlsconnection.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    43739 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.tlsrecordlayer.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7786 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.aes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     8459 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.aesgcm.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    13626 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.asn1parser.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12725 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.chacha.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10067 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.chacha20_poly1305.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    18141 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.cipherfactory.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    33216 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.codec.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    16967 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.compat.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    18018 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.constanttime.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    34260 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.cryptomath.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10078 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.datefuncs.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14255 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.deprecations.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6466 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.dns_utils.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7761 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.ecc.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    21776 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.ecdsakey.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10584 2023-08-01 15:43:24.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    19234 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.keyfactory.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     9265 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.lists.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    16689 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_aes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10907 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_rc4.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    17482 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_rsakey.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11632 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_tripledes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14357 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pem.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     8842 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.poly1305.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10515 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_aes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7817 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_aesgcm.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10063 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_rc4.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14657 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_rsakey.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10746 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_tripledes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     8560 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_aes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     5897 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_aesgcm.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6017 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_chacha20_poly1305.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10047 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_rc4.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14650 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_rsakey.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7538 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.rc4.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11634 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.rijndael.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    38486 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.rsakey.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     5238 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.tackwrapper.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6794 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.tlshashlib.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7979 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.tripledes.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10907 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.x25519.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15655 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.verifierdb.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    14761 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.x509.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15974 2023-08-01 15:43:25.000000 tlslite-ng-0.8.0a45/docs/_build/html/tlslite.x509certchain.html
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10006 2023-08-01 15:39:03.000000 tlslite-ng-0.8.0a45/docs/conf.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      445 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/docs/index.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     7740 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/make.bat
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)       58 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/modules.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      146 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.api.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      225 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.basedb.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.bufferedsocket.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      177 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.checker.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      142 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.constants.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.defragmenter.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      143 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.dh.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      183 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.errors.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.extensions.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.handshakehashes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      163 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.handshakehelpers.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.handshakesettings.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      233 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.asyncstatemachine.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.clienthelper.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      224 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.httptlsconnection.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.imap4_tls.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.pop3_tls.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      592 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.smtp_tls.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      251 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.tlsasyncdispatchermixin.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      242 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.tlssocketservermixin.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.xmlrpcserver.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.integration.xmlrpctransport.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.keyexchange.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.mathtls.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      189 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.messages.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.messagesocket.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.recordlayer.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      785 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      167 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.session.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      208 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.sessioncache.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.tlsconnection.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.tlsrecordlayer.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.aes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.aesgcm.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.asn1parser.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.chacha.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      215 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.chacha20_poly1305.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.cipherfactory.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      179 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.codec.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.compat.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.constanttime.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.cryptomath.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.datefuncs.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2019-01-22 17:40:43.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.deprecations.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.dns_utils.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.ecc.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.ecdsakey.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.keyfactory.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      170 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.lists.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.openssl_aes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.openssl_rc4.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.openssl_rsakey.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      206 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.openssl_tripledes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      164 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.pem.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.poly1305.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.pycrypto_aes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.pycrypto_aesgcm.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      200 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.pycrypto_rc4.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      209 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.pycrypto_rsakey.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      218 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.pycrypto_tripledes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.python_aes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.python_aesgcm.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      227 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.python_chacha20_poly1305.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      194 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.python_rc4.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      203 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.python_rsakey.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      173 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.rc4.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.rijndael.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.rsakey.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1316 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      188 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.tackwrapper.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.tlshashlib.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      191 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.tripledes.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      182 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.utils.x25519.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      202 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.verifierdb.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      158 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.x509.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      185 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/docs/tlslite.x509certchain.rst
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    10645 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/pylintrc
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       16 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/requirements.txt
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.173925 tlslite-ng-0.8.0a45/scripts/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1903 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/scripts/speed.py
+-rwxr-xr-x   0 hkario   (20970) hkario   (20970)    25679 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/scripts/tls.py
+-rwxrwxr-x   0 hkario   (20970) hkario   (20970)     3774 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/scripts/tlsdb.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       38 2023-08-01 15:43:28.208925 tlslite-ng-0.8.0a45/setup.cfg
+-rwxr-xr-x   0 hkario   (20970) hkario   (20970)     1931 2023-08-01 15:40:02.000000 tlslite-ng-0.8.0a45/setup.py
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.185925 tlslite-ng-0.8.0a45/tests/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      124 2015-10-14 14:17:40.000000 tlslite-ng-0.8.0a45/tests/.coverage
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/TACK1.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/TACK2.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/TACK_Key1.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/TACK_Key2.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      650 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a45/tests/TACKs.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      325 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a45/tests/TACKunrelated.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      579 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/clientECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      241 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/clientECKey.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      485 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/clientEd25519Cert.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      119 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/clientEd25519Key.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      924 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a45/tests/clientX509Cert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      891 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a45/tests/clientX509Key.pem
+-rwxrwxr-x   0 hkario   (20970) hkario   (20970)      327 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/httpsclient.py
+-rwxrwxr-x   0 hkario   (20970) hkario   (20970)      113 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/httpsserver.sh
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      152 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/index.html
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      579 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverBrainpoolP256r1ECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      227 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverBrainpoolP256r1ECKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      664 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverBrainpoolP384r1ECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      292 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverBrainpoolP384r1ECKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      757 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverBrainpoolP512r1ECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      361 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverBrainpoolP512r1ECKey.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6628 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/serverDSACert.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     1224 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/serverDSAKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      554 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2261 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverECDSANonCACert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      302 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverECDSANonCAKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      241 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverECKey.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      489 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/serverEd25519Cert.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      119 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/serverEd25519Key.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      591 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/serverEd448Cert.pem
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      156 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tests/serverEd448Key.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      660 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverP384ECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      306 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverP384ECKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      761 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverP521ECCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      384 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverP521ECKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4302 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverRSANonCACert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1675 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tests/serverRSANonCAKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1224 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tests/serverRSAPSSCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1700 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tests/serverRSAPSSKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1229 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tests/serverRSAPSSSigCert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1704 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tests/serverRSAPSSSigKey.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1094 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/serverX509Cert.pem
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1704 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/serverX509Key.pem
+-rwxr-xr-x   0 hkario   (20970) hkario   (20970)   114602 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tests/tlstest.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    24576 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tests/verifierDB
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.188925 tlslite-ng-0.8.0a45/tlslite/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      878 2021-08-06 12:04:22.000000 tlslite-ng-0.8.0a45/tlslite/__init__.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     1400 2023-08-01 15:39:10.000000 tlslite-ng-0.8.0a45/tlslite/api.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4092 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/basedb.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2836 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/bufferedsocket.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2725 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/checker.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    66261 2023-08-01 14:03:51.000000 tlslite-ng-0.8.0a45/tlslite/constants.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4430 2023-08-01 14:03:51.000000 tlslite-ng-0.8.0a45/tlslite/defragmenter.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      914 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/dh.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6838 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/errors.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    68800 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tlslite/extensions.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4137 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/handshakehashes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6725 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/handshakehelpers.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    32163 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tlslite/handshakesettings.py
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.189925 tlslite-ng-0.8.0a45/tlslite/integration/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      396 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tlslite/integration/__init__.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     7202 2019-01-22 17:40:44.000000 tlslite-ng-0.8.0a45/tlslite/integration/asyncstatemachine.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6197 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/integration/clienthelper.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4514 2018-07-30 10:15:07.000000 tlslite-ng-0.8.0a45/tlslite/integration/httptlsconnection.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3680 2021-01-14 12:41:41.000000 tlslite-ng-0.8.0a45/tlslite/integration/imap4_tls.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3199 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/integration/pop3_tls.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3026 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/integration/smtp_tls.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4964 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/integration/tlsasyncdispatchermixin.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2320 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/integration/tlssocketservermixin.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1909 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/integration/xmlrpcserver.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     5332 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/integration/xmlrpctransport.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    43331 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/keyexchange.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    45528 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/mathtls.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    78203 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tlslite/messages.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6250 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/messagesocket.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     5933 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/ocsp.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    51706 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tlslite/recordlayer.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6906 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tlslite/session.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3552 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/sessioncache.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3545 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/signed.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   212380 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/tlslite/tlsconnection.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    60589 2023-08-01 14:03:51.000000 tlslite-ng-0.8.0a45/tlslite/tlsrecordlayer.py
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.194925 tlslite-ng-0.8.0a45/tlslite/utils/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)      837 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/__init__.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1222 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/aes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4966 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/aesccm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6866 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/aesgcm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3802 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/asn1parser.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4821 2017-02-17 16:14:00.000000 tlslite-ng-0.8.0a45/tlslite/utils/chacha.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3123 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/chacha20_poly1305.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     5957 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/cipherfactory.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    15543 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/codec.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7229 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/compat.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6399 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/constanttime.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12585 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/cryptomath.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2278 2016-07-29 18:32:10.000000 tlslite-ng-0.8.0a45/tlslite/utils/datefuncs.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     8742 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/deprecations.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1468 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/utils/dns_utils.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     3144 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/dsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2676 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/ecc.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     5590 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/ecdsakey.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4766 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/eddsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      483 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/format_output.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10460 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/keyfactory.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1549 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/lists.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4539 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/openssl_aes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      733 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/openssl_aesccm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      664 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/openssl_aesgcm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      709 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tlslite/utils/openssl_rc4.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     7156 2023-07-11 11:45:08.000000 tlslite-ng-0.8.0a45/tlslite/utils/openssl_rsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1801 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/openssl_tripledes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3667 2016-07-29 18:32:10.000000 tlslite-ng-0.8.0a45/tlslite/utils/pem.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1504 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/utils/poly1305.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      840 2018-03-27 13:27:30.000000 tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_aes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      446 2015-08-12 15:24:17.000000 tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_aesgcm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      764 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_rc4.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2644 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_rsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      872 2018-03-27 13:27:30.000000 tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_tripledes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3667 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_aes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      271 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_aesccm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      268 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_aesgcm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      316 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_chacha20_poly1305.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     3777 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_dsakey.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     3388 2023-07-10 15:01:18.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_ecdsakey.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     2101 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_eddsakey.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    11034 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_key.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1073 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_rc4.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     4691 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_rsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    16932 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/python_tripledes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      561 2015-08-12 15:24:17.000000 tlslite-ng-0.8.0a45/tlslite/utils/rc4.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    53143 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/rijndael.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    26348 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/utils/rsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      334 2014-10-31 17:46:51.000000 tlslite-ng-0.8.0a45/tlslite/utils/tackwrapper.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1024 2016-01-08 16:25:14.000000 tlslite-ng-0.8.0a45/tlslite/utils/tlshashlib.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3079 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/utils/tlshmac.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      870 2018-02-01 13:32:10.000000 tlslite-ng-0.8.0a45/tlslite/utils/tripledes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3255 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/utils/x25519.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3702 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/tlslite/verifierdb.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    10386 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/tlslite/x509.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3323 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/tlslite/x509certchain.py
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.194925 tlslite-ng-0.8.0a45/tlslite_ng.egg-info/
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     3337 2023-08-01 15:43:27.000000 tlslite-ng-0.8.0a45/tlslite_ng.egg-info/PKG-INFO
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    18045 2023-08-01 15:43:28.000000 tlslite-ng-0.8.0a45/tlslite_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)        1 2023-08-01 15:43:27.000000 tlslite-ng-0.8.0a45/tlslite_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)       16 2023-08-01 15:43:27.000000 tlslite-ng-0.8.0a45/tlslite_ng.egg-info/requires.txt
+-rw-r--r--   0 hkario   (20970) hkario   (20970)        8 2023-08-01 15:43:27.000000 tlslite-ng-0.8.0a45/tlslite_ng.egg-info/top_level.txt
+drwxr-xr-x   0 hkario   (20970) hkario   (20970)        0 2023-08-01 15:43:28.208925 tlslite-ng-0.8.0a45/unit_tests/
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)        0 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/unit_tests/__init__.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3336 2018-06-29 15:54:59.000000 tlslite-ng-0.8.0a45/unit_tests/mocksock.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    18932 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tls1_3_vectors.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     4414 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_bufferedsocket.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    12726 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_constants.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6979 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_defragmenter.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2245 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_dh.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    95334 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_extensions.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3383 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_handshakehashes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    17133 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_handshakehelpers.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    15363 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_handshakesettings.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   126491 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_keyexchange.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     9991 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_mathtls.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   150116 2023-07-31 18:53:31.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_messages.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    12586 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_messagesocket.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    25676 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_ocsp.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)   117035 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_recordlayer.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1834 2016-04-14 13:26:36.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_session.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1275 2015-07-14 10:24:03.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_sessioncache.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2611 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_signed.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    19118 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_tlsconnection.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    36862 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_tlsrecordlayer.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2931 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aes_split.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    10191 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aescbc.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    22930 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aesccm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    10558 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aesctr.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    14665 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aesgcm.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2143 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_asn1.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    15890 2016-01-07 16:34:17.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_chacha.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     5662 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_chacha20_poly1305.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    11423 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_codec.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      789 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_compat.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    16432 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_constanttime.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    26699 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_cryptomath.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3442 2016-01-08 16:25:14.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_cryptomath_m2crypto.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    16100 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_deprecations.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1286 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_dns_utils.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     8381 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_ecc.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     2228 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_ecdsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    13810 2019-01-22 17:40:44.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_keyfactory.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     1694 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_lists.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     7573 2015-12-09 15:06:01.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_poly1305.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)    21266 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_python_dsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3998 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_python_ecdsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     7738 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_python_key.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     6754 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_rijndael.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)   170557 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_rsakey.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)      765 2016-01-08 16:25:14.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_tlshashlib.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    20642 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_tripledes.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)     3178 2020-12-18 23:03:24.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_tripledes_split.py
+-rw-rw-r--   0 hkario   (20970) hkario   (20970)    14421 2018-03-27 16:03:06.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_x25519.py
+-rw-r--r--   0 hkario   (20970) hkario   (20970)     6997 2023-02-08 17:37:53.000000 tlslite-ng-0.8.0a45/unit_tests/test_tlslite_x509.py
```

### Comparing `tlslite-ng-0.8.0a44/.codeclimate.yml` & `tlslite-ng-0.8.0a45/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/.github/workflows/ci.yml` & `tlslite-ng-0.8.0a45/.github/workflows/ci.yml`

 * *Files 5% similar despite different names*

```diff
@@ -67,30 +67,30 @@
             python-version: 3.9
             opt-deps: ['m2crypto']
           - name: py3.10 with m2crypto
             os: ubuntu-latest
             python-version: '3.10'
             opt-deps: ['m2crypto']
           - name: py2.7 with pycrypto
-            os: ubuntu-latest
+            os: ubuntu-20.04
             python-version: 2.7
             opt-deps: ['pycrypto']
           - name: py3.6 with pycrypto
             os: ubuntu-20.04
             # note: 3.6 is the last version where pycrypto is installable
             python-version: 3.6
             opt-deps: ['pycrypto']
           - name: py3.10 with pycryptodome
             os: ubuntu-latest
             python-version: '3.10'
             # we don't support pycryptodome, just test that when it's installed
             # it doesn't break pycrypto code
             opt-deps: ['pycryptodome']
           - name: py2.7 with gmpy
-            os: ubuntu-latest
+            os: ubuntu-20.04
             python-version: 2.7
             opt-deps: ['gmpy']
           - name: py3.6 with gmpy
             os: ubuntu-20.04
             python-version: 3.6
             opt-deps: ['gmpy']
           - name: py3.7 with gmpy
@@ -106,15 +106,15 @@
             python-version: 3.9
             opt-deps: ['gmpy']
           - name: py3.10 with gmpy
             os: ubuntu-latest
             python-version: '3.10'
             opt-deps: ['gmpy']
           - name: py2.7 with gmpy2
-            os: ubuntu-latest
+            os: ubuntu-20.04
             python-version: 2.7
             opt-deps: ['gmpy2']
           - name: py3.6 with gmpy2
             os: ubuntu-20.04
             python-version: 3.6
             opt-deps: ['gmpy2']
           - name: py3.7 with gmpy2
@@ -131,15 +131,15 @@
             opt-deps: ['gmpy2']
           - name: py3.10 with gmpy2
             os: ubuntu-latest
             python-version: '3.10'
             opt-deps: ['gmpy2']
           # finally test with multiple dependencies installed at the same time
           - name: py2.7 with m2crypto, pycrypto, gmpy, and gmpy2
-            os: ubuntu-latest
+            os: ubuntu-20.04
             python-version: 2.7
             opt-deps: ['m2crypto', 'pycrypto', 'gmpy', 'gmpy2']
           - name: py3.6 with m2crypto, pycrypto, gmpy, and gmpy2
             os: ubuntu-20.04
             python-version: 3.6
             opt-deps: ['m2crypto', 'pycrypto', 'gmpy', 'gmpy2']
           - name: py3.7 with m2crypto, gmpy, and gmpy2
@@ -203,18 +203,28 @@
         run: |
           git status
           git remote -v
       - name: Ensure we have baseline branch for quality coverage
         run: git fetch origin master:refs/remotes/origin/master
       - name: Set up Python ${{ matrix.python-version }}
         # we use containers to use the native python version from them
-        if: ${{ !matrix.container }}
+        if: ${{ !matrix.container && matrix.python-version != '2.7' }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
+      - name: Ensure python 2.7
+        if: matrix.python-version == '2.7'
+        run: |
+          sudo apt-get update
+          sudo apt-get install -y \
+            python2.7 python2.7-dev python-pip-whl
+          sudo ln -sf python2.7 /usr/bin/python
+          export PYTHONPATH=`echo /usr/share/python-wheels/pip-*py2*.whl`
+          sudo --preserve-env=PYTHONPATH python -m pip install --upgrade pip setuptools wheel
+          sudo chown -R $USER /usr/local/lib/python2.7
       - name: Display Python version
         run: python -c "import sys; print(sys.version)"
       - name: Display installed python package versions
         run: |
           pip list || :
       - name: Ensure working pip on 3.3
         if: ${{ matrix.python-version == '3.3' }}
```

### Comparing `tlslite-ng-0.8.0a44/.travis.yml` & `tlslite-ng-0.8.0a45/.travis.yml`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/CONTRIBUTING.md` & `tlslite-ng-0.8.0a45/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/LICENSE` & `tlslite-ng-0.8.0a45/LICENSE`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/Makefile` & `tlslite-ng-0.8.0a45/Makefile`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/PKG-INFO` & `tlslite-ng-0.8.0a45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlslite-ng
-Version: 0.8.0a44
+Version: 0.8.0a45
 Summary: Pure python implementation of SSL and TLS.
 Home-page: https://github.com/tlsfuzzer/tlslite-ng
 Author: Hubert Kario
 Author-email: hkario@redhat.com
 License: LGPLv2
 Keywords: ssl,tls,pure-python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tlslite-ng-0.8.0a44/README` & `tlslite-ng-0.8.0a45/README`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/README.md` & `tlslite-ng-0.8.0a45/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-tlslite-ng version 0.8.0-alpha44 (2022-06-09)
+tlslite-ng version 0.8.0-alpha45 (2023-08-01)
 
 [![Build Status](https://github.com/tlsfuzzer/tlslite-ng/workflows/GitHub%20CI/badge.svg?branch=master)](https://github.com/tlsfuzzer/tlslite-ng/actions?query=workflow%3A%22GitHub+CI%22+branch%3Amaster)
 [![Read the Docs](https://img.shields.io/readthedocs/tlslite-ng)](https://tlslite-ng.readthedocs.io/en/latest/)
 [![Coverage Status](https://coveralls.io/repos/tlsfuzzer/tlslite-ng/badge.svg?branch=master)](https://coveralls.io/r/tlsfuzzer/tlslite-ng?branch=master)
 [![Code Climate](https://codeclimate.com/github/tlsfuzzer/tlslite-ng/badges/gpa.svg)](https://codeclimate.com/github/tlsfuzzer/tlslite-ng)
 
 Table of Contents
@@ -24,15 +24,15 @@
 ===============
 
 tlslite-ng is an open source python library that implements SSL and
 [TLS](https://en.wikipedia.org/wiki/Transport_Layer_Security)
 cryptographic protocols. It can be used either as a standalone wrapper around
 python socket interface or as a backend for multiple other libraries.
 tlslite-ng is pure python, however it can use other libraries for faster crypto
-operations. tlslite-ng integrates with several stdlib neworking libraries.
+operations. tlslite-ng integrates with several stdlib networking libraries.
 
 API documentation is available in the `docs/_build/html` directory of the PyPI
 package
 or can be automatically generated using `make docs` with Sphinx installed.
 
 If you have questions or feedback, feel free to contact me (Hubert Kario
 &lt;hkario at redhat.com>). Issues and pull
```

### Comparing `tlslite-ng-0.8.0a44/SECURITY.md` & `tlslite-ng-0.8.0a45/SECURITY.md`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/Makefile` & `tlslite-ng-0.8.0a45/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.integration.rst.txt` & `tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.integration.rst.txt`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.rst.txt` & `tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.rst.txt`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_sources/tlslite.utils.rst.txt` & `tlslite-ng-0.8.0a45/docs/_build/html/_sources/tlslite.utils.rst.txt`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/basic.css` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/css/badge_only.css` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/css/theme.css` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/doctools.js` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/jquery-3.6.0.js` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/jquery.js` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/js/badge_only.js` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/js/theme.js` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/language_data.js` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/pygments.css` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/searchtools.js` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/underscore-1.13.1.js` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/_static/underscore.js` & `tlslite-ng-0.8.0a45/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/genindex.html` & `tlslite-ng-0.8.0a45/docs/_build/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>Index &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -422,16 +422,20 @@
 </li>
         <li><a href="tlslite.utils.openssl_tripledes.html#tlslite.utils.openssl_tripledes.OpenSSL_TripleDES.__module__">(tlslite.utils.openssl_tripledes.OpenSSL_TripleDES attribute)</a>
 </li>
       </ul></li>
       <li><a href="tlslite.extensions.html#tlslite.extensions.ALPNExtension.__repr__">__repr__() (tlslite.extensions.ALPNExtension method)</a>
 
       <ul>
+        <li><a href="tlslite.extensions.html#tlslite.extensions.ClientKeyShareExtension.__repr__">(tlslite.extensions.ClientKeyShareExtension method)</a>
+</li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.IntExtension.__repr__">(tlslite.extensions.IntExtension method)</a>
 </li>
+        <li><a href="tlslite.extensions.html#tlslite.extensions.KeyShareEntry.__repr__">(tlslite.extensions.KeyShareEntry method)</a>
+</li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.ListExtension.__repr__">(tlslite.extensions.ListExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.NPNExtension.__repr__">(tlslite.extensions.NPNExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SNIExtension.__repr__">(tlslite.extensions.SNIExtension method)</a>
 </li>
         <li><a href="tlslite.extensions.html#tlslite.extensions.SNIExtension.ServerName.__repr__">(tlslite.extensions.SNIExtension.ServerName method)</a>
```

#### html2text {}

```diff
@@ -63,61 +63,61 @@
           o (tlslite.extensions.SignatureAlgorithmsExtension_method)
           o (tlslite.extensions.SNIExtension_method)
           o (tlslite.extensions.SRPExtension_method)
           o (tlslite.extensions.SrvPreSharedKeyExtension_method)
           o (tlslite.extensions.SrvSupportedVersionsExtension_method)
           o (tlslite.extensions.StatusRequestExtension_method)
           o (tlslite.extensions.SupportedGroupsExtension_method)
-          o (tlslite.extensions.SupportedVersionsExtension_method)
-          o (tlslite.extensions.TACKExtension_method)                                * __module___
-          o (tlslite.extensions.TACKExtension.TACK_method)                             (tlslite.integration.httptlsconnection.HTTPTLSConnection
-          o (tlslite.extensions.TLSExtension_method)                                   attribute)
-          o (tlslite.extensions.VarBytesExtension_method)                                  o (tlslite.utils.openssl_aes.OpenSSL_AES_attribute)
-          o (tlslite.extensions.VarListExtension_method)                                   o (tlslite.utils.openssl_aes.OpenSSL_CTR_attribute)
-          o (tlslite.extensions.VarSeqListExtension_method)                                o (tlslite.utils.openssl_rc4.OpenSSL_RC4_attribute)
-          o (tlslite.handshakehashes.HandshakeHashes_method)                               o (tlslite.utils.openssl_rsakey.OpenSSL_RSAKey
-          o (tlslite.handshakesettings.HandshakeSettings_method)                             attribute)
-          o (tlslite.handshakesettings.Keypair_method)                                     o (tlslite.utils.openssl_tripledes.OpenSSL_TripleDES
-          o (tlslite.handshakesettings.VirtualHost_method)                                   attribute)
-          o (tlslite.integration.asyncstatemachine.AsyncStateMachine_method)         * __repr__()_(tlslite.extensions.ALPNExtension_method)
-          o (tlslite.integration.clienthelper.ClientHelper_method)                         o (tlslite.extensions.IntExtension_method)
-          o (tlslite.integration.httptlsconnection.HTTPTLSConnection_method)               o (tlslite.extensions.ListExtension_method)
-          o (tlslite.integration.imap4_tls.IMAP4_TLS_method)                               o (tlslite.extensions.NPNExtension_method)
-          o (tlslite.integration.pop3_tls.POP3_TLS_method)                                 o (tlslite.extensions.SNIExtension_method)
-          o (tlslite.integration.tlsasyncdispatchermixin.TLSAsyncDispatcherMixIn           o (tlslite.extensions.SNIExtension.ServerName
-            method)                                                                          method)
-          o (tlslite.integration.xmlrpcserver.MultiPathTLSXMLRPCServer_method)             o (tlslite.extensions.SRPExtension_method)
-          o (tlslite.integration.xmlrpcserver.TLSXMLRPCServer_method)                      o (tlslite.extensions.SrvSupportedVersionsExtension
-          o (tlslite.integration.xmlrpctransport.XMLRPCTransport_method)                     method)
-          o (tlslite.keyexchange.ADHKeyExchange_method)                                    o (tlslite.extensions.StatusRequestExtension_method)
-          o (tlslite.keyexchange.AECDHKeyExchange_method)                                  o (tlslite.extensions.TACKExtension_method)
-          o (tlslite.keyexchange.DHE_RSAKeyExchange_method)                                o (tlslite.extensions.TACKExtension.TACK_method)
-          o (tlslite.keyexchange.ECDHE_RSAKeyExchange_method)                              o (tlslite.extensions.TLSExtension_method)
-          o (tlslite.keyexchange.ECDHKeyExchange_method)                                   o (tlslite.extensions.VarBytesExtension_method)
-          o (tlslite.keyexchange.FFDHKeyExchange_method)                                   o (tlslite.messages.Alert_method)
-          o (tlslite.keyexchange.KeyExchange_method)                                       o (tlslite.messages.Certificate_method)
-          o (tlslite.keyexchange.RawDHKeyExchange_method)                                  o (tlslite.messages.CertificateEntry_method)
-          o (tlslite.keyexchange.RSAKeyExchange_method)                                    o (tlslite.messages.ClientHello_method)
-          o (tlslite.keyexchange.SRPKeyExchange_method)                                    o (tlslite.messages.RecordHeader3_method)
-          o (tlslite.messages.Alert_method)                                                o (tlslite.messages.ServerHello_method)
-          o (tlslite.messages.ApplicationData_method)                                      o (tlslite.messages.ServerHelloDone_method)
-          o (tlslite.messages.Certificate_method)                                          o (tlslite.messages.ServerKeyExchange_method)
-          o (tlslite.messages.CertificateEntry_method)                               * __setitem__()_(tlslite.basedb.BaseDB_method)
-          o (tlslite.messages.CertificateRequest_method)                                   o (tlslite.sessioncache.SessionCache_method)
-          o (tlslite.messages.CertificateStatus_method)                                    o (tlslite.verifierdb.VerifierDB_method)
-          o (tlslite.messages.CertificateVerify_method)                              * __str__()_(tlslite.errors.TLSError_method)
-          o (tlslite.messages.ChangeCipherSpec_method)                                     o (tlslite.errors.TLSLocalAlert_method)
-          o (tlslite.messages.ClientFinished_method)                                       o (tlslite.errors.TLSRemoteAlert_method)
-          o (tlslite.messages.ClientHello_method)                                          o (tlslite.messages.Alert_method)
-          o (tlslite.messages.ClientKeyExchange_method)                                    o (tlslite.messages.ClientHello_method)
-          o (tlslite.messages.ClientMasterKey_method)                                      o (tlslite.messages.Heartbeat_method)
-          o (tlslite.messages.EncryptedExtensions_method)                                  o (tlslite.messages.RecordHeader3_method)
-          o (tlslite.messages.Finished_method)                                             o (tlslite.messages.ServerHello_method)
-          o (tlslite.messages.HandshakeMsg_method)
-          o (tlslite.messages.Heartbeat_method)
+          o (tlslite.extensions.SupportedVersionsExtension_method)                   * __module___
+          o (tlslite.extensions.TACKExtension_method)                                  (tlslite.integration.httptlsconnection.HTTPTLSConnection
+          o (tlslite.extensions.TACKExtension.TACK_method)                             attribute)
+          o (tlslite.extensions.TLSExtension_method)                                       o (tlslite.utils.openssl_aes.OpenSSL_AES_attribute)
+          o (tlslite.extensions.VarBytesExtension_method)                                  o (tlslite.utils.openssl_aes.OpenSSL_CTR_attribute)
+          o (tlslite.extensions.VarListExtension_method)                                   o (tlslite.utils.openssl_rc4.OpenSSL_RC4_attribute)
+          o (tlslite.extensions.VarSeqListExtension_method)                                o (tlslite.utils.openssl_rsakey.OpenSSL_RSAKey
+          o (tlslite.handshakehashes.HandshakeHashes_method)                                 attribute)
+          o (tlslite.handshakesettings.HandshakeSettings_method)                           o (tlslite.utils.openssl_tripledes.OpenSSL_TripleDES
+          o (tlslite.handshakesettings.Keypair_method)                                       attribute)
+          o (tlslite.handshakesettings.VirtualHost_method)                           * __repr__()_(tlslite.extensions.ALPNExtension_method)
+          o (tlslite.integration.asyncstatemachine.AsyncStateMachine_method)               o (tlslite.extensions.ClientKeyShareExtension
+          o (tlslite.integration.clienthelper.ClientHelper_method)                           method)
+          o (tlslite.integration.httptlsconnection.HTTPTLSConnection_method)               o (tlslite.extensions.IntExtension_method)
+          o (tlslite.integration.imap4_tls.IMAP4_TLS_method)                               o (tlslite.extensions.KeyShareEntry_method)
+          o (tlslite.integration.pop3_tls.POP3_TLS_method)                                 o (tlslite.extensions.ListExtension_method)
+          o (tlslite.integration.tlsasyncdispatchermixin.TLSAsyncDispatcherMixIn           o (tlslite.extensions.NPNExtension_method)
+            method)                                                                        o (tlslite.extensions.SNIExtension_method)
+          o (tlslite.integration.xmlrpcserver.MultiPathTLSXMLRPCServer_method)             o (tlslite.extensions.SNIExtension.ServerName
+          o (tlslite.integration.xmlrpcserver.TLSXMLRPCServer_method)                        method)
+          o (tlslite.integration.xmlrpctransport.XMLRPCTransport_method)                   o (tlslite.extensions.SRPExtension_method)
+          o (tlslite.keyexchange.ADHKeyExchange_method)                                    o (tlslite.extensions.SrvSupportedVersionsExtension
+          o (tlslite.keyexchange.AECDHKeyExchange_method)                                    method)
+          o (tlslite.keyexchange.DHE_RSAKeyExchange_method)                                o (tlslite.extensions.StatusRequestExtension_method)
+          o (tlslite.keyexchange.ECDHE_RSAKeyExchange_method)                              o (tlslite.extensions.TACKExtension_method)
+          o (tlslite.keyexchange.ECDHKeyExchange_method)                                   o (tlslite.extensions.TACKExtension.TACK_method)
+          o (tlslite.keyexchange.FFDHKeyExchange_method)                                   o (tlslite.extensions.TLSExtension_method)
+          o (tlslite.keyexchange.KeyExchange_method)                                       o (tlslite.extensions.VarBytesExtension_method)
+          o (tlslite.keyexchange.RawDHKeyExchange_method)                                  o (tlslite.messages.Alert_method)
+          o (tlslite.keyexchange.RSAKeyExchange_method)                                    o (tlslite.messages.Certificate_method)
+          o (tlslite.keyexchange.SRPKeyExchange_method)                                    o (tlslite.messages.CertificateEntry_method)
+          o (tlslite.messages.Alert_method)                                                o (tlslite.messages.ClientHello_method)
+          o (tlslite.messages.ApplicationData_method)                                      o (tlslite.messages.RecordHeader3_method)
+          o (tlslite.messages.Certificate_method)                                          o (tlslite.messages.ServerHello_method)
+          o (tlslite.messages.CertificateEntry_method)                                     o (tlslite.messages.ServerHelloDone_method)
+          o (tlslite.messages.CertificateRequest_method)                                   o (tlslite.messages.ServerKeyExchange_method)
+          o (tlslite.messages.CertificateStatus_method)                              * __setitem__()_(tlslite.basedb.BaseDB_method)
+          o (tlslite.messages.CertificateVerify_method)                                    o (tlslite.sessioncache.SessionCache_method)
+          o (tlslite.messages.ChangeCipherSpec_method)                                     o (tlslite.verifierdb.VerifierDB_method)
+          o (tlslite.messages.ClientFinished_method)                                 * __str__()_(tlslite.errors.TLSError_method)
+          o (tlslite.messages.ClientHello_method)                                          o (tlslite.errors.TLSLocalAlert_method)
+          o (tlslite.messages.ClientKeyExchange_method)                                    o (tlslite.errors.TLSRemoteAlert_method)
+          o (tlslite.messages.ClientMasterKey_method)                                      o (tlslite.messages.Alert_method)
+          o (tlslite.messages.EncryptedExtensions_method)                                  o (tlslite.messages.ClientHello_method)
+          o (tlslite.messages.Finished_method)                                             o (tlslite.messages.Heartbeat_method)
+          o (tlslite.messages.HandshakeMsg_method)                                         o (tlslite.messages.RecordHeader3_method)
+          o (tlslite.messages.Heartbeat_method)                                            o (tlslite.messages.ServerHello_method)
           o (tlslite.messages.HelloMessage_method)
           o (tlslite.messages.HelloRequest_method)
           o (tlslite.messages.KeyUpdate_method)
           o (tlslite.messages.Message_method)
           o (tlslite.messages.NewSessionTicket_method)
           o (tlslite.messages.NextProtocol_method)
           o (tlslite.messages.RecordHeader_method)
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/index.html` & `tlslite-ng-0.8.0a45/docs/_build/html/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to tlslite-ng’s documentation! &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>Welcome to tlslite-ng’s documentation! &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/modules.html` & `tlslite-ng-0.8.0a45/docs/_build/html/modules.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/py-modindex.html` & `tlslite-ng-0.8.0a45/docs/_build/html/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Python Module Index &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>Python Module Index &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/search.html` & `tlslite-ng-0.8.0a45/docs/_build/html/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>Search &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/searchindex.js` & `tlslite-ng-0.8.0a45/docs/_build/html/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1248,14 +1248,15 @@
         "variant": [11, 29],
         "6091": 11,
         "certtyp": 11,
         "identifi": [11, 28, 49, 71],
         "clientkeyshareextens": 11,
         "hello": [11, 13, 14, 28, 33],
         "share": [11, 14, 26, 28, 75],
+        "output": [11, 27, 50, 71],
         "client_shar": 11,
         "advertis": [11, 14, 17, 28, 33],
         "definit": 11,
         "cookieextens": 11,
         "varbytesextens": 11,
         "customnameextens": 11,
         "field_nam": 11,
@@ -1452,15 +1453,14 @@
         "those": [11, 27, 28, 29, 34],
         "special": 11,
         "_certificateextens": 11,
         "_hrrextens": 11,
         "effect": 11,
         "Will": [11, 29, 42, 45, 52],
         "them": [11, 22, 29],
-        "output": [11, 27, 50, 71],
         "child": [11, 28, 38],
         "overrid": 11,
         "render": 11,
         "arg": [11, 16, 24, 28, 30, 73],
         "kwarg": [11, 24, 28, 73],
         "legaci": 11,
         "so": [11, 13, 14, 22, 30, 33, 34, 47, 51, 71],
@@ -3540,14 +3540,15 @@
             [11, 2, 1, "", "parse"]
         ],
         "tlslite.extensions.ClientCertTypeExtension": [
             [11, 2, 1, "", "__init__"]
         ],
         "tlslite.extensions.ClientKeyShareExtension": [
             [11, 2, 1, "", "__init__"],
+            [11, 2, 1, "", "__repr__"],
             [11, 2, 1, "", "create"],
             [11, 6, 1, "", "extData"],
             [11, 2, 1, "", "parse"]
         ],
         "tlslite.extensions.CookieExtension": [
             [11, 2, 1, "", "__init__"]
         ],
@@ -3574,14 +3575,15 @@
             [11, 2, 1, "", "__init__"],
             [11, 2, 1, "", "__repr__"],
             [11, 6, 1, "", "extData"],
             [11, 2, 1, "", "parse"]
         ],
         "tlslite.extensions.KeyShareEntry": [
             [11, 2, 1, "", "__init__"],
+            [11, 2, 1, "", "__repr__"],
             [11, 2, 1, "", "create"],
             [11, 2, 1, "", "parse"],
             [11, 2, 1, "", "write"]
         ],
         "tlslite.extensions.ListExtension": [
             [11, 2, 1, "", "__init__"],
             [11, 2, 1, "", "__repr__"]
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.api.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.api.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.api module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.api module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.basedb.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.basedb.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.basedb module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.basedb module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.bufferedsocket.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.bufferedsocket.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.bufferedsocket module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.bufferedsocket module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.checker.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.checker.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.checker module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.checker module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.constants.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.constants.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.constants module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.constants module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.defragmenter.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.defragmenter.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.defragmenter module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.defragmenter module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.dh.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.dh.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.dh module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.dh module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.errors.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.errors.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.errors module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.errors module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.extensions.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.extensions.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.extensions module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.extensions module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -243,14 +243,20 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="tlslite.extensions.ClientKeyShareExtension.__init__">
 <span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.extensions.ClientKeyShareExtension.__init__" title="Permalink to this definition"></a></dt>
 <dd><p>Create instance of the object.</p>
 </dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="tlslite.extensions.ClientKeyShareExtension.__repr__">
+<span class="sig-name descname"><span class="pre">__repr__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.extensions.ClientKeyShareExtension.__repr__" title="Permalink to this definition"></a></dt>
+<dd><p>Output human readable representation of the object.</p>
+</dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="tlslite.extensions.ClientKeyShareExtension.create">
 <span class="sig-name descname"><span class="pre">create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">client_shares</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.extensions.ClientKeyShareExtension.create" title="Permalink to this definition"></a></dt>
 <dd><p>Set the advertised client shares in the extension.</p>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="tlslite.extensions.ClientKeyShareExtension.extData">
@@ -515,14 +521,20 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="tlslite.extensions.KeyShareEntry.__init__">
 <span class="sig-name descname"><span class="pre">__init__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.extensions.KeyShareEntry.__init__" title="Permalink to this definition"></a></dt>
 <dd><p>Initialise the object.</p>
 </dd></dl>
 
 <dl class="py method">
+<dt class="sig sig-object py" id="tlslite.extensions.KeyShareEntry.__repr__">
+<span class="sig-name descname"><span class="pre">__repr__</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.extensions.KeyShareEntry.__repr__" title="Permalink to this definition"></a></dt>
+<dd><p>Returns human readable representation of the extension.</p>
+</dd></dl>
+
+<dl class="py method">
 <dt class="sig sig-object py" id="tlslite.extensions.KeyShareEntry.create">
 <span class="sig-name descname"><span class="pre">create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">group</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">key_exchange</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">private</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#tlslite.extensions.KeyShareEntry.create" title="Permalink to this definition"></a></dt>
 <dd><p>Initialise the Key Share Entry from Key Share extension.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>group</strong> (<a class="reference external" href="https://docs.python.org/3/library/functions.html#int" title="(in Python v3.11)"><em>int</em></a>) – ID of the key share</p></li>
```

#### html2text {}

```diff
@@ -106,14 +106,16 @@
             See also: create() and parse()
   classtlslite.extensions.ClientKeyShareExtensionï
       Bases: TLSExtension
       Class for handling the Client Hello version of the Key Share extension.
       Extension for sending the key shares to server
         __init__()ï
             Create instance of the object.
+        __repr__()ï
+            Output human readable representation of the object.
         create(client_shares)ï
             Set the advertised client shares in the extension.
         propertyextDataï
             Return the on the wire raw encoding of the extension
               Return type:
                   bytearray
         parse(parser)ï
@@ -228,14 +230,16 @@
               Return type:
                   Extension
   classtlslite.extensions.KeyShareEntryï
       Bases: object
       Handler for of the item of the Key Share extension.
         __init__()ï
             Initialise the object.
+        __repr__()ï
+            Returns human readable representation of the extension.
         create(group, key_exchange, private=None)ï
             Initialise the Key Share Entry from Key Share extension.
               Parameters:
                       * group (int) â ID of the key share
                       * key_exchange (bytearray) â value of the key share
                       * private (object) â private value for the given share
                         (wonât be encoded during serialisation)
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.handshakehashes.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.handshakehashes.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.handshakehashes module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.handshakehashes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.handshakehelpers.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.handshakehelpers.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.handshakehelpers module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.handshakehelpers module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.handshakesettings.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.handshakesettings.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.handshakesettings module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.handshakesettings module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite package &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite package &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.asyncstatemachine.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.asyncstatemachine.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.asyncstatemachine module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.integration.asyncstatemachine module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.clienthelper.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.clienthelper.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.clienthelper module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.integration.clienthelper module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration package &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.integration package &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.httptlsconnection.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.httptlsconnection.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.httptlsconnection module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.integration.httptlsconnection module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.imap4_tls.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.imap4_tls.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.imap4_tls module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.integration.imap4_tls module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.pop3_tls.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.pop3_tls.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.pop3_tls module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.integration.pop3_tls module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.smtp_tls.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.smtp_tls.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.smtp_tls module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.integration.smtp_tls module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.tlsasyncdispatchermixin.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.tlsasyncdispatchermixin.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.tlsasyncdispatchermixin module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.integration.tlsasyncdispatchermixin module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.tlssocketservermixin.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.tlssocketservermixin.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.tlssocketservermixin module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.integration.tlssocketservermixin module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.xmlrpcserver.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.xmlrpcserver.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.xmlrpcserver module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.integration.xmlrpcserver module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.integration.xmlrpctransport.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.integration.xmlrpctransport.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.integration.xmlrpctransport module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.integration.xmlrpctransport module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.keyexchange.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.keyexchange.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.keyexchange module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.keyexchange module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.mathtls.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.mathtls.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.mathtls module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.mathtls module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.messages.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.messages.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.messages module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.messages module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.messagesocket.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.messagesocket.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.messagesocket module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.messagesocket module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.recordlayer.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.recordlayer.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.recordlayer module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.recordlayer module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.session.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.session.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.session module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.session module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.sessioncache.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.sessioncache.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.sessioncache module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.sessioncache module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.tlsconnection.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.tlsconnection.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.tlsconnection module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.tlsconnection module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.tlsrecordlayer.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.tlsrecordlayer.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.tlsrecordlayer module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.tlsrecordlayer module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.aes.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.aes.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.aes module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.aes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.aesgcm.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.aesgcm.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.aesgcm module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.aesgcm module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.asn1parser.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.asn1parser.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.asn1parser module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.asn1parser module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.chacha.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.chacha.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.chacha module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.chacha module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.chacha20_poly1305.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.chacha20_poly1305.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.chacha20_poly1305 module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.chacha20_poly1305 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.cipherfactory.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.cipherfactory.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.cipherfactory module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.cipherfactory module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.codec.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.codec.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.codec module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.codec module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.compat.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.compat.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.compat module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.compat module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.constanttime.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.constanttime.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.constanttime module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.constanttime module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.cryptomath.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.cryptomath.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.cryptomath module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.cryptomath module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.datefuncs.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.datefuncs.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.datefuncs module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.datefuncs module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.deprecations.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.deprecations.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.deprecations module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.deprecations module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.dns_utils.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.dns_utils.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.dns_utils module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.dns_utils module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.ecc.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.ecc.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.ecc module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.ecc module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.ecdsakey.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.ecdsakey.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.ecdsakey module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.ecdsakey module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils package &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils package &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.keyfactory.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.keyfactory.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.keyfactory module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.keyfactory module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.lists.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.lists.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.lists module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.lists module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.openssl_aes.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_aes.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.openssl_aes module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.openssl_aes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.openssl_rc4.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_rc4.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.openssl_rc4 module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.openssl_rc4 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.openssl_rsakey.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_rsakey.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.openssl_rsakey module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.openssl_rsakey module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.openssl_tripledes.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.openssl_tripledes.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.openssl_tripledes module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.openssl_tripledes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.pem.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pem.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.pem module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.pem module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.poly1305.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.poly1305.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.poly1305 module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.poly1305 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.pycrypto_aes.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_aes.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.pycrypto_aes module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.pycrypto_aes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.pycrypto_aesgcm.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_aesgcm.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.pycrypto_aesgcm module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.pycrypto_aesgcm module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.pycrypto_rc4.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_rc4.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.pycrypto_rc4 module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.pycrypto_rc4 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.pycrypto_rsakey.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_rsakey.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.pycrypto_rsakey module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.pycrypto_rsakey module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.pycrypto_tripledes.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.pycrypto_tripledes.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.pycrypto_tripledes module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.pycrypto_tripledes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.python_aes.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_aes.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.python_aes module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.python_aes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.python_aesgcm.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_aesgcm.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.python_aesgcm module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.python_aesgcm module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.python_chacha20_poly1305.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_chacha20_poly1305.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.python_chacha20_poly1305 module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.python_chacha20_poly1305 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.python_rc4.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_rc4.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.python_rc4 module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.python_rc4 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.python_rsakey.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.python_rsakey.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.python_rsakey module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.python_rsakey module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.rc4.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.rc4.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.rc4 module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.rc4 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.rijndael.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.rijndael.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.rijndael module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.rijndael module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.rsakey.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.rsakey.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.rsakey module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.rsakey module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.tackwrapper.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.tackwrapper.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.tackwrapper module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.tackwrapper module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.tlshashlib.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.tlshashlib.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.tlshashlib module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.tlshashlib module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.tripledes.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.tripledes.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.tripledes module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.tripledes module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.utils.x25519.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.utils.x25519.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.utils.x25519 module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.utils.x25519 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.verifierdb.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.verifierdb.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.verifierdb module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.verifierdb module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.x509.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.x509.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.x509 module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.x509 module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/_build/html/tlslite.x509certchain.html` & `tlslite-ng-0.8.0a45/docs/_build/html/tlslite.x509certchain.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>tlslite.x509certchain module &mdash; tlslite-ng 0.8.0-alpha44 documentation</title>
+  <title>tlslite.x509certchain module &mdash; tlslite-ng 0.8.0-alpha45 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
```

### Comparing `tlslite-ng-0.8.0a44/docs/conf.py` & `tlslite-ng-0.8.0a45/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = u'0.8'
 # The full version, including alpha/beta/rc tags.
-release = u'0.8.0-alpha44'
+release = u'0.8.0-alpha45'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `tlslite-ng-0.8.0a44/docs/make.bat` & `tlslite-ng-0.8.0a45/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/tlslite.integration.rst` & `tlslite-ng-0.8.0a45/docs/tlslite.integration.rst`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/tlslite.rst` & `tlslite-ng-0.8.0a45/docs/tlslite.rst`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/docs/tlslite.utils.rst` & `tlslite-ng-0.8.0a45/docs/tlslite.utils.rst`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/pylintrc` & `tlslite-ng-0.8.0a45/pylintrc`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/scripts/speed.py` & `tlslite-ng-0.8.0a45/scripts/speed.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/scripts/tls.py` & `tlslite-ng-0.8.0a45/scripts/tls.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/scripts/tlsdb.py` & `tlslite-ng-0.8.0a45/scripts/tlsdb.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/setup.py` & `tlslite-ng-0.8.0a45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, "README")) as f:
     README = f.read()
 
 setup(name="tlslite-ng",
-      version="0.8.0-alpha44",
+      version="0.8.0-alpha45",
       author="Hubert Kario",
       author_email="hkario@redhat.com",
       url="https://github.com/tlsfuzzer/tlslite-ng",
       description="Pure python implementation of SSL and TLS.",
       long_description=README,
       license="LGPLv2",
       scripts=["scripts/tls.py", "scripts/tlsdb.py"],
```

### Comparing `tlslite-ng-0.8.0a44/tests/TACKs.pem` & `tlslite-ng-0.8.0a45/tests/TACKs.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/clientECCert.pem` & `tlslite-ng-0.8.0a45/tests/clientECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/clientX509Cert.pem` & `tlslite-ng-0.8.0a45/tests/clientX509Cert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/clientX509Key.pem` & `tlslite-ng-0.8.0a45/tests/clientX509Key.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverBrainpoolP256r1ECCert.pem` & `tlslite-ng-0.8.0a45/tests/serverBrainpoolP256r1ECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverBrainpoolP384r1ECCert.pem` & `tlslite-ng-0.8.0a45/tests/serverBrainpoolP384r1ECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverBrainpoolP512r1ECCert.pem` & `tlslite-ng-0.8.0a45/tests/serverBrainpoolP512r1ECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverDSACert.pem` & `tlslite-ng-0.8.0a45/tests/serverDSACert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverDSAKey.pem` & `tlslite-ng-0.8.0a45/tests/serverDSAKey.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverECCert.pem` & `tlslite-ng-0.8.0a45/tests/serverECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverECDSANonCACert.pem` & `tlslite-ng-0.8.0a45/tests/serverECDSANonCACert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverEd448Cert.pem` & `tlslite-ng-0.8.0a45/tests/serverEd448Cert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverP384ECCert.pem` & `tlslite-ng-0.8.0a45/tests/serverP384ECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverP521ECCert.pem` & `tlslite-ng-0.8.0a45/tests/serverP521ECCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverRSANonCACert.pem` & `tlslite-ng-0.8.0a45/tests/serverRSANonCACert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverRSANonCAKey.pem` & `tlslite-ng-0.8.0a45/tests/serverRSANonCAKey.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverRSAPSSCert.pem` & `tlslite-ng-0.8.0a45/tests/serverRSAPSSCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverRSAPSSKey.pem` & `tlslite-ng-0.8.0a45/tests/serverRSAPSSKey.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverRSAPSSSigCert.pem` & `tlslite-ng-0.8.0a45/tests/serverRSAPSSSigCert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverRSAPSSSigKey.pem` & `tlslite-ng-0.8.0a45/tests/serverRSAPSSSigKey.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverX509Cert.pem` & `tlslite-ng-0.8.0a45/tests/serverX509Cert.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/serverX509Key.pem` & `tlslite-ng-0.8.0a45/tests/serverX509Key.pem`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/tlstest.py` & `tlslite-ng-0.8.0a45/tests/tlstest.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tests/verifierDB` & `tlslite-ng-0.8.0a45/tests/verifierDB`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/__init__.py` & `tlslite-ng-0.8.0a45/tlslite/__init__.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/api.py` & `tlslite-ng-0.8.0a45/tlslite/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Author: Trevor Perrin
 # See the LICENSE file for legal information regarding use of this file.
 
-__version__ = "0.8.0-alpha44"
+__version__ = "0.8.0-alpha45"
 from .constants import AlertLevel, AlertDescription, Fault
 from .errors import *
 from .checker import Checker
 from .handshakesettings import HandshakeSettings
 from .session import Session
 from .sessioncache import SessionCache
 from .tlsconnection import TLSConnection
```

### Comparing `tlslite-ng-0.8.0a44/tlslite/basedb.py` & `tlslite-ng-0.8.0a45/tlslite/basedb.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/bufferedsocket.py` & `tlslite-ng-0.8.0a45/tlslite/bufferedsocket.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/checker.py` & `tlslite-ng-0.8.0a45/tlslite/checker.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/constants.py` & `tlslite-ng-0.8.0a45/tlslite/constants.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/defragmenter.py` & `tlslite-ng-0.8.0a45/tlslite/defragmenter.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/dh.py` & `tlslite-ng-0.8.0a45/tlslite/dh.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/errors.py` & `tlslite-ng-0.8.0a45/tlslite/errors.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/extensions.py` & `tlslite-ng-0.8.0a45/tlslite/extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1787,14 +1787,20 @@
 
         :param Writer writer: buffer to write the data to
         """
         writer.addTwo(self.group)
         writer.addTwo(len(self.key_exchange))
         writer.bytes += self.key_exchange
 
+    def __repr__(self):
+        """Returns human readable representation of the extension."""
+        return "KeyShareEntry(group={0},key_exchange={1})".format(
+            GroupName.toStr(self.group),
+            repr(self.key_exchange))
+
 
 class HeartbeatExtension(IntExtension):
     """
     Heartbeat extension from RFC 6520
 
     :type mode: int
     :ivar mode: mode if peer is allowed or nor allowed to send responses
@@ -1870,14 +1876,19 @@
         parser.stopLengthCheck()
 
         if parser.getRemainingLength():
             raise DecodeError("Trailing data in client Key Share extension")
 
         return self
 
+    def __repr__(self):
+        """Output human readable representation of the object."""
+        return "ClientKeyShareExtension(client_shares=[{0}])".format(
+            ",".join(repr(i) for i in self.client_shares))
+
 
 class ServerKeyShareExtension(TLSExtension):
     """
     Class for handling the Server Hello variant of the Key Share extension.
 
     Extension for sending the key shares to client
     """
```

### Comparing `tlslite-ng-0.8.0a44/tlslite/handshakehashes.py` & `tlslite-ng-0.8.0a45/tlslite/handshakehashes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/handshakehelpers.py` & `tlslite-ng-0.8.0a45/tlslite/handshakehelpers.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/handshakesettings.py` & `tlslite-ng-0.8.0a45/tlslite/handshakesettings.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/integration/asyncstatemachine.py` & `tlslite-ng-0.8.0a45/tlslite/integration/asyncstatemachine.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/integration/clienthelper.py` & `tlslite-ng-0.8.0a45/tlslite/integration/clienthelper.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/integration/httptlsconnection.py` & `tlslite-ng-0.8.0a45/tlslite/integration/httptlsconnection.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/integration/imap4_tls.py` & `tlslite-ng-0.8.0a45/tlslite/integration/imap4_tls.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/integration/pop3_tls.py` & `tlslite-ng-0.8.0a45/tlslite/integration/pop3_tls.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/integration/smtp_tls.py` & `tlslite-ng-0.8.0a45/tlslite/integration/smtp_tls.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/integration/tlsasyncdispatchermixin.py` & `tlslite-ng-0.8.0a45/tlslite/integration/tlsasyncdispatchermixin.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/integration/tlssocketservermixin.py` & `tlslite-ng-0.8.0a45/tlslite/integration/tlssocketservermixin.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/integration/xmlrpcserver.py` & `tlslite-ng-0.8.0a45/tlslite/integration/xmlrpcserver.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/integration/xmlrpctransport.py` & `tlslite-ng-0.8.0a45/tlslite/integration/xmlrpctransport.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/keyexchange.py` & `tlslite-ng-0.8.0a45/tlslite/keyexchange.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/mathtls.py` & `tlslite-ng-0.8.0a45/tlslite/mathtls.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/messages.py` & `tlslite-ng-0.8.0a45/tlslite/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,47 +338,53 @@
         self.ssl2 = ssl2
         self.client_version = (0, 0)
         self.random = bytearray(32)
         self.session_id = bytearray(0)
         self.cipher_suites = []         # a list of 16-bit values
         self.compression_methods = []   # a list of 8-bit values
 
+    def _ciphers_to_str(self):
+        ciphers = ", ".join(
+            CipherSuite.ietfNames.get(i, str(i))
+            for i in self.cipher_suites)
+        return "[{0}]".format(ciphers)
+
     def __str__(self):
         """
         Return human readable representation of Client Hello.
 
         :rtype: str
         """
         if self.session_id.count(bytearray(b'\x00')) == len(self.session_id)\
                 and len(self.session_id) != 0:
             session = "bytearray(b'\\x00'*{0})".format(len(self.session_id))
         else:
             session = repr(self.session_id)
         ret = "client_hello,version({0[0]}.{0[1]}),random(...),"\
-              "session ID({1!s}),cipher suites({2!r}),"\
+              "session ID({1!s}),cipher suites({2}),"\
               "compression methods({3!r})".format(
                   self.client_version, session,
-                  self.cipher_suites, self.compression_methods)
+                  self._ciphers_to_str(), self.compression_methods)
 
         if self.extensions is not None:
             ret += ",extensions({0!r})".format(self.extensions)
 
         return ret
 
     def __repr__(self):
         """
         Return machine readable representation of Client Hello.
 
         :rtype: str
         """
         return "ClientHello(ssl2={0}, client_version=({1[0]}.{1[1]}), "\
-               "random={2!r}, session_id={3!r}, cipher_suites={4!r}, "\
+               "random={2!r}, session_id={3!r}, cipher_suites={4}, "\
                "compression_methods={5}, extensions={6})".format(
                    self.ssl2, self.client_version, self.random,
-                   self.session_id, self.cipher_suites,
+                   self.session_id, self._ciphers_to_str(),
                    self.compression_methods, self.extensions)
 
     @property
     def certificate_types(self):
         """
         Return the list of certificate types supported.
 
@@ -1888,14 +1894,16 @@
         self.type = 1
         return self
 
     def parse(self, p):
         p.setLengthCheck(1)
         self.type = p.get(1)
         p.stopLengthCheck()
+        if p.getRemainingLength():
+            raise DecodeError("Multi-byte CCS message")
         return self
 
     def write(self):
         w = Writer()
         w.add(self.type, 1)
         return w.bytes
```

### Comparing `tlslite-ng-0.8.0a44/tlslite/messagesocket.py` & `tlslite-ng-0.8.0a45/tlslite/messagesocket.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/ocsp.py` & `tlslite-ng-0.8.0a45/tlslite/ocsp.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/recordlayer.py` & `tlslite-ng-0.8.0a45/tlslite/recordlayer.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/session.py` & `tlslite-ng-0.8.0a45/tlslite/session.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/sessioncache.py` & `tlslite-ng-0.8.0a45/tlslite/sessioncache.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/signed.py` & `tlslite-ng-0.8.0a45/tlslite/signed.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/tlsconnection.py` & `tlslite-ng-0.8.0a45/tlslite/tlsconnection.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/tlsrecordlayer.py` & `tlslite-ng-0.8.0a45/tlslite/tlsrecordlayer.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/__init__.py` & `tlslite-ng-0.8.0a45/tlslite/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/aes.py` & `tlslite-ng-0.8.0a45/tlslite/utils/aes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/aesccm.py` & `tlslite-ng-0.8.0a45/tlslite/utils/aesccm.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/aesgcm.py` & `tlslite-ng-0.8.0a45/tlslite/utils/aesgcm.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/asn1parser.py` & `tlslite-ng-0.8.0a45/tlslite/utils/asn1parser.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/chacha.py` & `tlslite-ng-0.8.0a45/tlslite/utils/chacha.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/chacha20_poly1305.py` & `tlslite-ng-0.8.0a45/tlslite/utils/chacha20_poly1305.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/cipherfactory.py` & `tlslite-ng-0.8.0a45/tlslite/utils/cipherfactory.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/codec.py` & `tlslite-ng-0.8.0a45/tlslite/utils/codec.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/compat.py` & `tlslite-ng-0.8.0a45/tlslite/utils/compat.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/constanttime.py` & `tlslite-ng-0.8.0a45/tlslite/utils/constanttime.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/cryptomath.py` & `tlslite-ng-0.8.0a45/tlslite/utils/cryptomath.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/datefuncs.py` & `tlslite-ng-0.8.0a45/tlslite/utils/datefuncs.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/deprecations.py` & `tlslite-ng-0.8.0a45/tlslite/utils/deprecations.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/dns_utils.py` & `tlslite-ng-0.8.0a45/tlslite/utils/dns_utils.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/dsakey.py` & `tlslite-ng-0.8.0a45/tlslite/utils/dsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/ecc.py` & `tlslite-ng-0.8.0a45/tlslite/utils/ecc.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/ecdsakey.py` & `tlslite-ng-0.8.0a45/tlslite/utils/ecdsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/eddsakey.py` & `tlslite-ng-0.8.0a45/tlslite/utils/eddsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/keyfactory.py` & `tlslite-ng-0.8.0a45/tlslite/utils/keyfactory.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/lists.py` & `tlslite-ng-0.8.0a45/tlslite/utils/lists.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/openssl_aes.py` & `tlslite-ng-0.8.0a45/tlslite/utils/openssl_aes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/openssl_aesccm.py` & `tlslite-ng-0.8.0a45/tlslite/utils/openssl_aesccm.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/openssl_aesgcm.py` & `tlslite-ng-0.8.0a45/tlslite/utils/openssl_aesgcm.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/openssl_rc4.py` & `tlslite-ng-0.8.0a45/tlslite/utils/openssl_rc4.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/openssl_rsakey.py` & `tlslite-ng-0.8.0a45/tlslite/utils/openssl_rsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/openssl_tripledes.py` & `tlslite-ng-0.8.0a45/tlslite/utils/openssl_tripledes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/pem.py` & `tlslite-ng-0.8.0a45/tlslite/utils/pem.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/poly1305.py` & `tlslite-ng-0.8.0a45/tlslite/utils/poly1305.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/pycrypto_aes.py` & `tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_aes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/pycrypto_rc4.py` & `tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_rc4.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/pycrypto_rsakey.py` & `tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_rsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/pycrypto_tripledes.py` & `tlslite-ng-0.8.0a45/tlslite/utils/pycrypto_tripledes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/python_aes.py` & `tlslite-ng-0.8.0a45/tlslite/utils/python_aes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/python_dsakey.py` & `tlslite-ng-0.8.0a45/tlslite/utils/python_dsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/python_ecdsakey.py` & `tlslite-ng-0.8.0a45/tlslite/utils/python_ecdsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/python_eddsakey.py` & `tlslite-ng-0.8.0a45/tlslite/utils/python_eddsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/python_key.py` & `tlslite-ng-0.8.0a45/tlslite/utils/python_key.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/python_rc4.py` & `tlslite-ng-0.8.0a45/tlslite/utils/python_rc4.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/python_rsakey.py` & `tlslite-ng-0.8.0a45/tlslite/utils/python_rsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/python_tripledes.py` & `tlslite-ng-0.8.0a45/tlslite/utils/python_tripledes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/rc4.py` & `tlslite-ng-0.8.0a45/tlslite/utils/rc4.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/rijndael.py` & `tlslite-ng-0.8.0a45/tlslite/utils/rijndael.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/rsakey.py` & `tlslite-ng-0.8.0a45/tlslite/utils/rsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/tlshashlib.py` & `tlslite-ng-0.8.0a45/tlslite/utils/tlshashlib.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/tlshmac.py` & `tlslite-ng-0.8.0a45/tlslite/utils/tlshmac.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/tripledes.py` & `tlslite-ng-0.8.0a45/tlslite/utils/tripledes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/utils/x25519.py` & `tlslite-ng-0.8.0a45/tlslite/utils/x25519.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/verifierdb.py` & `tlslite-ng-0.8.0a45/tlslite/verifierdb.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/x509.py` & `tlslite-ng-0.8.0a45/tlslite/x509.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite/x509certchain.py` & `tlslite-ng-0.8.0a45/tlslite/x509certchain.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/tlslite_ng.egg-info/PKG-INFO` & `tlslite-ng-0.8.0a45/tlslite_ng.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlslite-ng
-Version: 0.8.0a44
+Version: 0.8.0a45
 Summary: Pure python implementation of SSL and TLS.
 Home-page: https://github.com/tlsfuzzer/tlslite-ng
 Author: Hubert Kario
 Author-email: hkario@redhat.com
 License: LGPLv2
 Keywords: ssl,tls,pure-python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tlslite-ng-0.8.0a44/tlslite_ng.egg-info/SOURCES.txt` & `tlslite-ng-0.8.0a45/tlslite_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/mocksock.py` & `tlslite-ng-0.8.0a45/unit_tests/mocksock.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tls1_3_vectors.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tls1_3_vectors.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_bufferedsocket.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_bufferedsocket.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_constants.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_constants.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_defragmenter.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_defragmenter.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_dh.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_dh.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_extensions.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_extensions.py`

 * *Files 0% similar despite different names*

```diff
@@ -2193,14 +2193,21 @@
 
         self.kse.write(w)
 
         self.assertEqual(w.bytes, bytearray(b'\x00\x12'  # group ID
                                             b'\x00\x02'  # share length
                                             b'\x01\x01'))  # key share
 
+    def test_repr(self):
+        self.kse.create(18, bytearray(b'\x01\x01'))
+
+        self.assertEqual(
+            "KeyShareEntry(group=secp192k1,key_exchange="
+            "bytearray(b'\\x01\\x01'))", repr(self.kse))
+
 
 class TestKeyShareExtension(unittest.TestCase):
     def setUp(self):
         self.cks = ClientKeyShareExtension()
 
     def test___init__(self):
         self.assertIsNotNone(self.cks)
```

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_handshakehashes.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_handshakehashes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_handshakehelpers.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_handshakehelpers.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_handshakesettings.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_handshakesettings.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_keyexchange.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_keyexchange.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_mathtls.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_mathtls.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_messages.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,14 +486,42 @@
         client_hello = ClientHello().create((3,0), bytearray(4), bytearray(0),\
                 [])
 
         self.assertEqual("client_hello,version(3.0),random(...),"\
                 "session ID(bytearray(b'')),cipher suites([]),"\
                 "compression methods([0])", str(client_hello))
 
+    def test___str___with_one_cipher_suite(self):
+        client_hello = ClientHello().create((3,0), bytearray(4), bytearray(0),\
+                [CipherSuite.TLS_RSA_WITH_AES_128_CBC_SHA])
+
+        self.assertEqual("client_hello,version(3.0),random(...),"
+                "session ID(bytearray(b'')),cipher suites(["
+                "TLS_RSA_WITH_AES_128_CBC_SHA]),"
+                "compression methods([0])", str(client_hello))
+
+    def test___str___with_unassigned_cipher_suite(self):
+        client_hello = ClientHello().create((3,0), bytearray(4), bytearray(0),\
+                [93])
+
+        self.assertEqual("client_hello,version(3.0),random(...),"\
+                "session ID(bytearray(b'')),cipher suites([93]),"\
+                "compression methods([0])", str(client_hello))
+
+    def test___str___with_cipher_suites(self):
+        client_hello = ClientHello().create((3,0), bytearray(4), bytearray(0),\
+                [CipherSuite.TLS_RSA_WITH_AES_128_CBC_SHA,
+                 CipherSuite.TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA])
+
+        self.assertEqual("client_hello,version(3.0),random(...),"
+                "session ID(bytearray(b'')),cipher suites(["
+                "TLS_RSA_WITH_AES_128_CBC_SHA, "
+                "TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA]),"
+                "compression methods([0])", str(client_hello))
+
     def test___str___with_all_null_session_id(self):
         client_hello = ClientHello().create((3,0), bytearray(4), bytearray(10),\
                 [])
 
         self.assertEqual("client_hello,version(3.0),random(...),"\
                 "session ID(bytearray(b'\\x00'*10)),cipher suites([]),"\
                 "compression methods([0])", str(client_hello))
@@ -3246,14 +3274,22 @@
 
         ccs = ChangeCipherSpec()
         ccs = ccs.parse(parser)
 
         self.assertIsInstance(ccs, ChangeCipherSpec)
         self.assertEqual(ccs.type, 1)
 
+    def test_parse_wrong_size(self):
+        parser = Parser(bytearray(b'\x01\x01'))
+
+        ccs = ChangeCipherSpec()
+
+        with self.assertRaises(SyntaxError):
+            ccs.parse(parser)
+
 
 class TestNextProtocol(unittest.TestCase):
     def test___init__(self):
         np = NextProtocol()
 
         self.assertIsNotNone(np)
         self.assertIsNone(np.next_proto)
```

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_messagesocket.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_messagesocket.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_ocsp.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_ocsp.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_recordlayer.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_recordlayer.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_session.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_session.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_sessioncache.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_sessioncache.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_signed.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_signed.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_tlsconnection.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_tlsconnection.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_tlsrecordlayer.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_tlsrecordlayer.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_aes_split.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aes_split.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_aescbc.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aescbc.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_aesccm.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aesccm.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_aesctr.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aesctr.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_aesgcm.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_aesgcm.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_asn1.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_asn1.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_chacha.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_chacha.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_chacha20_poly1305.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_chacha20_poly1305.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_codec.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_codec.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_compat.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_compat.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_constanttime.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_constanttime.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_cryptomath.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_cryptomath.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_cryptomath_m2crypto.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_cryptomath_m2crypto.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_deprecations.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_deprecations.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_dns_utils.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_dns_utils.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_ecc.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_ecc.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_ecdsakey.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_ecdsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_keyfactory.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_keyfactory.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_lists.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_lists.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_poly1305.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_poly1305.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_python_dsakey.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_python_dsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_python_ecdsakey.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_python_ecdsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_python_key.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_python_key.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_rijndael.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_rijndael.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_rsakey.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_rsakey.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_tlshashlib.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_tlshashlib.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_tripledes.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_tripledes.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_tripledes_split.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_tripledes_split.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_utils_x25519.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_utils_x25519.py`

 * *Files identical despite different names*

### Comparing `tlslite-ng-0.8.0a44/unit_tests/test_tlslite_x509.py` & `tlslite-ng-0.8.0a45/unit_tests/test_tlslite_x509.py`

 * *Files identical despite different names*

