# Comparing `tmp/symbol-shoestring-0.0.4.tar.gz` & `tmp/symbol-shoestring-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbol-shoestring-0.0.4.tar", max compression
+gzip compressed data, was "symbol-shoestring-0.0.5.tar", max compression
```

## Comparing `symbol-shoestring-0.0.4.tar` & `symbol-shoestring-0.0.5.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     9931 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/README.md
--rw-r--r--   0        0        0      879 2023-08-01 12:23:24.309328 symbol-shoestring-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/__init__.py
--rw-r--r--   0        0        0     1937 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/__main__.py
--rw-r--r--   0        0        0        0 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/commands/__init__.py
--rw-r--r--   0        0        0     1552 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/commands/announce_transaction.py
--rw-r--r--   0        0        0     2475 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/commands/health.py
--rw-r--r--   0        0        0     1262 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/commands/import_bootstrap.py
--rw-r--r--   0        0        0     1025 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/commands/init.py
--rw-r--r--   0        0        0     1692 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/commands/min_cosignatures_count.py
--rw-r--r--   0        0        0     1733 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/commands/pemtool.py
--rw-r--r--   0        0        0     1569 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/commands/renew_certificates.py
--rw-r--r--   0        0        0     5270 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/commands/renew_voting_keys.py
--rw-r--r--   0        0        0     3071 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/commands/reset_data.py
--rw-r--r--   0        0        0     5330 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/commands/setup.py
--rw-r--r--   0        0        0     3332 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/commands/signer.py
--rw-r--r--   0        0        0     2246 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/commands/upgrade.py
--rw-r--r--   0        0        0        0 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/healthagents/__init__.py
--rw-r--r--   0        0        0      594 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/healthagents/peer_api.py
--rw-r--r--   0        0        0     3586 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/healthagents/peer_certificate.py
--rw-r--r--   0        0        0      644 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/healthagents/rest_api.py
--rw-r--r--   0        0        0     2985 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/healthagents/rest_https_certificate.py
--rw-r--r--   0        0        0     1686 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/healthagents/voting_keys.py
--rw-r--r--   0        0        0     1573 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/healthagents/websockets.py
--rw-r--r--   0        0        0     5055 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/CertificateFactory.py
--rw-r--r--   0        0        0     3233 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/ConfigurationManager.py
--rw-r--r--   0        0        0     1656 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/FileDownloader.py
--rw-r--r--   0        0        0      360 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/FileTemplater.py
--rw-r--r--   0        0        0     1961 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/HarvesterConfigurator.py
--rw-r--r--   0        0        0      830 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/HeightGrouping.py
--rw-r--r--   0        0        0     3089 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/LinkTransactionBuilder.py
--rw-r--r--   0        0        0      655 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/MultisigAnalyzer.py
--rw-r--r--   0        0        0     2789 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/NodeDownloader.py
--rw-r--r--   0        0        0      578 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/NodeFeatures.py
--rw-r--r--   0        0        0     1412 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/NodewatchClient.py
--rw-r--r--   0        0        0     1381 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/OpensslExecutor.py
--rw-r--r--   0        0        0     3060 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/PackageResolver.py
--rw-r--r--   0        0        0     2139 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/PeerDownloader.py
--rw-r--r--   0        0        0     2372 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/PemUtils.py
--rw-r--r--   0        0        0    12643 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/Preparer.py
--rw-r--r--   0        0        0     3509 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/ShoestringConfiguration.py
--rw-r--r--   0        0        0      371 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/TransactionSerializer.py
--rw-r--r--   0        0        0     3947 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/VoterConfigurator.py
--rw-r--r--   0        0        0        0 2023-08-01 12:16:13.281539 symbol-shoestring-0.0.4/shoestring/internal/__init__.py
--rw-r--r--   0        0        0    15969 2023-08-01 12:20:41.783604 symbol-shoestring-0.0.4/shoestring/lang/en/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    25392 2023-08-01 12:20:41.351601 symbol-shoestring-0.0.4/shoestring/lang/en/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      438 2023-08-01 12:20:41.779605 symbol-shoestring-0.0.4/shoestring/lang/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0        0        0    18950 2023-08-01 12:20:41.567602 symbol-shoestring-0.0.4/shoestring/lang/ja/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    18737 2023-08-01 12:20:41.059598 symbol-shoestring-0.0.4/shoestring/lang/messages.pot
--rw-r--r--   0        0        0      213 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/lang/po.header.txt
--rw-r--r--   0        0        0      270 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/startup/delayrestapi.sh
--rw-r--r--   0        0        0      565 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/startup/mongors.sh
--rw-r--r--   0        0        0      190 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/startup/startBroker.sh
--rw-r--r--   0        0        0      272 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/startup/startServer.sh
--rw-r--r--   0        0        0      102 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/startup/wait.sh
--rw-r--r--   0        0        0     2830 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/templates/docker-compose-dual.yaml
--rw-r--r--   0        0        0      629 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/templates/docker-compose-peer.yaml
--rw-r--r--   0        0        0      299 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/templates/nginx.conf.erb
--rw-r--r--   0        0        0     1004 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/Screen.py
--rw-r--r--   0        0        0     2102 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/ScreenContainer.py
--rw-r--r--   0        0        0     1781 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/ShoestringOperation.py
--rw-r--r--   0        0        0     4774 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/TabbedView.py
--rw-r--r--   0        0        0      843 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/TitleBar.py
--rw-r--r--   0        0        0     2708 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/ValidatingTextBox.py
--rw-r--r--   0        0        0        0 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/__init__.py
--rw-r--r--   0        0        0     3664 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/__main__.py
--rw-r--r--   0        0        0     1970 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/buttons.py
--rw-r--r--   0        0        0      484 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/keybindings.py
--rw-r--r--   0        0        0     1553 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/navigation.py
--rw-r--r--   0        0        0     1635 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/screen_loader.py
--rw-r--r--   0        0        0        0 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/screens/__init__.py
--rw-r--r--   0        0        0     1890 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/screens/certificates.py
--rw-r--r--   0        0        0      652 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/screens/end_screen.py
--rw-r--r--   0        0        0     6498 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/screens/harvesting.py
--rw-r--r--   0        0        0     1625 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/screens/modal.py
--rw-r--r--   0        0        0      799 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/screens/network_type.py
--rw-r--r--   0        0        0     2981 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/screens/node_settings.py
--rw-r--r--   0        0        0      757 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/screens/node_type.py
--rw-r--r--   0        0        0     6789 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/screens/obligatory.py
--rw-r--r--   0        0        0      827 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/screens/root_check.py
--rw-r--r--   0        0        0      799 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/screens/voting.py
--rw-r--r--   0        0        0     1835 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/screens/welcome.py
--rw-r--r--   0        0        0     3810 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/setup_file_generator.py
--rw-r--r--   0        0        0     1744 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/shoestring_dispatcher.py
--rw-r--r--   0        0        0     1095 2023-08-01 12:16:13.285539 symbol-shoestring-0.0.4/shoestring/wizard/styles.py
--rw-r--r--   0        0        0    11476 2023-08-01 12:23:31.511987 symbol-shoestring-0.0.4/setup.py
--rw-r--r--   0        0        0    11035 2023-08-01 12:23:31.513028 symbol-shoestring-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     9931 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/README.md
+-rw-r--r--   0        0        0      879 2023-08-01 17:01:59.866488 symbol-shoestring-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/__init__.py
+-rw-r--r--   0        0        0     1937 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/__init__.py
+-rw-r--r--   0        0        0     1552 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/announce_transaction.py
+-rw-r--r--   0        0        0     2475 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/health.py
+-rw-r--r--   0        0        0     1262 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/import_bootstrap.py
+-rw-r--r--   0        0        0     1025 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/init.py
+-rw-r--r--   0        0        0     1692 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/min_cosignatures_count.py
+-rw-r--r--   0        0        0     1733 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/pemtool.py
+-rw-r--r--   0        0        0     1569 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/renew_certificates.py
+-rw-r--r--   0        0        0     5270 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/renew_voting_keys.py
+-rw-r--r--   0        0        0     3071 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/reset_data.py
+-rw-r--r--   0        0        0     5330 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/setup.py
+-rw-r--r--   0        0        0     3332 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/signer.py
+-rw-r--r--   0        0        0     2246 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/commands/upgrade.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/__init__.py
+-rw-r--r--   0        0        0      594 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/peer_api.py
+-rw-r--r--   0        0        0     3586 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/peer_certificate.py
+-rw-r--r--   0        0        0      644 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/rest_api.py
+-rw-r--r--   0        0        0     2985 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/rest_https_certificate.py
+-rw-r--r--   0        0        0     1686 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/voting_keys.py
+-rw-r--r--   0        0        0     1573 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/healthagents/websockets.py
+-rw-r--r--   0        0        0     5055 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/CertificateFactory.py
+-rw-r--r--   0        0        0     3233 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/ConfigurationManager.py
+-rw-r--r--   0        0        0     1656 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/FileDownloader.py
+-rw-r--r--   0        0        0      360 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/FileTemplater.py
+-rw-r--r--   0        0        0     1961 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/HarvesterConfigurator.py
+-rw-r--r--   0        0        0      830 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/HeightGrouping.py
+-rw-r--r--   0        0        0     3089 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/LinkTransactionBuilder.py
+-rw-r--r--   0        0        0      655 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/MultisigAnalyzer.py
+-rw-r--r--   0        0        0     2789 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/NodeDownloader.py
+-rw-r--r--   0        0        0      578 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/NodeFeatures.py
+-rw-r--r--   0        0        0     1412 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/NodewatchClient.py
+-rw-r--r--   0        0        0     1381 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/OpensslExecutor.py
+-rw-r--r--   0        0        0     3060 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/PackageResolver.py
+-rw-r--r--   0        0        0     2139 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/PeerDownloader.py
+-rw-r--r--   0        0        0     2372 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/PemUtils.py
+-rw-r--r--   0        0        0    12793 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/Preparer.py
+-rw-r--r--   0        0        0     3509 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/ShoestringConfiguration.py
+-rw-r--r--   0        0        0      371 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/TransactionSerializer.py
+-rw-r--r--   0        0        0     3947 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/VoterConfigurator.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/internal/__init__.py
+-rw-r--r--   0        0        0    15969 2023-08-01 16:59:00.626339 symbol-shoestring-0.0.5/shoestring/lang/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    25392 2023-08-01 16:58:59.930338 symbol-shoestring-0.0.5/shoestring/lang/en/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      438 2023-08-01 16:59:00.618339 symbol-shoestring-0.0.5/shoestring/lang/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0        0        0    18950 2023-08-01 16:59:00.338339 symbol-shoestring-0.0.5/shoestring/lang/ja/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    18737 2023-08-01 16:58:59.638338 symbol-shoestring-0.0.5/shoestring/lang/messages.pot
+-rw-r--r--   0        0        0      213 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/lang/po.header.txt
+-rw-r--r--   0        0        0      270 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/startup/delayrestapi.sh
+-rw-r--r--   0        0        0      565 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/startup/mongors.sh
+-rw-r--r--   0        0        0      190 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/startup/startBroker.sh
+-rw-r--r--   0        0        0      272 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/startup/startServer.sh
+-rw-r--r--   0        0        0      102 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/startup/wait.sh
+-rw-r--r--   0        0        0     2830 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/templates/docker-compose-dual.yaml
+-rw-r--r--   0        0        0      629 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/templates/docker-compose-peer.yaml
+-rw-r--r--   0        0        0      299 2023-08-01 16:56:52.526218 symbol-shoestring-0.0.5/shoestring/templates/nginx.conf.erb
+-rw-r--r--   0        0        0     1004 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/Screen.py
+-rw-r--r--   0        0        0     2102 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/ScreenContainer.py
+-rw-r--r--   0        0        0     1781 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/ShoestringOperation.py
+-rw-r--r--   0        0        0     4774 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/TabbedView.py
+-rw-r--r--   0        0        0      843 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/TitleBar.py
+-rw-r--r--   0        0        0     2708 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/ValidatingTextBox.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/__init__.py
+-rw-r--r--   0        0        0     3664 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/__main__.py
+-rw-r--r--   0        0        0     1970 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/buttons.py
+-rw-r--r--   0        0        0      484 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/keybindings.py
+-rw-r--r--   0        0        0     1553 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/navigation.py
+-rw-r--r--   0        0        0     1635 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screen_loader.py
+-rw-r--r--   0        0        0        0 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/__init__.py
+-rw-r--r--   0        0        0     1890 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/certificates.py
+-rw-r--r--   0        0        0      652 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/end_screen.py
+-rw-r--r--   0        0        0     6498 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/harvesting.py
+-rw-r--r--   0        0        0     1625 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/modal.py
+-rw-r--r--   0        0        0      799 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/network_type.py
+-rw-r--r--   0        0        0     2981 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/node_settings.py
+-rw-r--r--   0        0        0      757 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/node_type.py
+-rw-r--r--   0        0        0     6789 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/obligatory.py
+-rw-r--r--   0        0        0      827 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/root_check.py
+-rw-r--r--   0        0        0      799 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/voting.py
+-rw-r--r--   0        0        0     1835 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/screens/welcome.py
+-rw-r--r--   0        0        0     3810 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/setup_file_generator.py
+-rw-r--r--   0        0        0     1744 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/shoestring_dispatcher.py
+-rw-r--r--   0        0        0     1095 2023-08-01 16:56:52.530218 symbol-shoestring-0.0.5/shoestring/wizard/styles.py
+-rw-r--r--   0        0        0    11476 2023-08-01 17:02:08.134248 symbol-shoestring-0.0.5/setup.py
+-rw-r--r--   0        0        0    11035 2023-08-01 17:02:08.137078 symbol-shoestring-0.0.5/PKG-INFO
```

### Comparing `symbol-shoestring-0.0.4/README.md` & `symbol-shoestring-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/pyproject.toml` & `symbol-shoestring-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'symbol-shoestring'
-version = '0.0.4'
+version = '0.0.5'
 description = 'Symbol Shoestring Deployment Tool'
 authors = ['Symbol Contributors <contributors@symbol.dev>']
 maintainers = ['Symbol Contributors <contributors@symbol.dev>']
 license = 'MIT'
 
 readme = 'README.md'
```

### Comparing `symbol-shoestring-0.0.4/shoestring/__main__.py` & `symbol-shoestring-0.0.5/shoestring/__main__.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/commands/announce_transaction.py` & `symbol-shoestring-0.0.5/shoestring/commands/announce_transaction.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/commands/health.py` & `symbol-shoestring-0.0.5/shoestring/commands/health.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/commands/import_bootstrap.py` & `symbol-shoestring-0.0.5/shoestring/commands/import_bootstrap.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/commands/init.py` & `symbol-shoestring-0.0.5/shoestring/commands/init.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/commands/min_cosignatures_count.py` & `symbol-shoestring-0.0.5/shoestring/commands/min_cosignatures_count.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/commands/pemtool.py` & `symbol-shoestring-0.0.5/shoestring/commands/pemtool.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/commands/renew_certificates.py` & `symbol-shoestring-0.0.5/shoestring/commands/renew_certificates.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/commands/renew_voting_keys.py` & `symbol-shoestring-0.0.5/shoestring/commands/renew_voting_keys.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/commands/reset_data.py` & `symbol-shoestring-0.0.5/shoestring/commands/reset_data.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/commands/setup.py` & `symbol-shoestring-0.0.5/shoestring/commands/setup.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/commands/signer.py` & `symbol-shoestring-0.0.5/shoestring/commands/signer.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/commands/upgrade.py` & `symbol-shoestring-0.0.5/shoestring/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/healthagents/peer_api.py` & `symbol-shoestring-0.0.5/shoestring/healthagents/peer_api.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/healthagents/peer_certificate.py` & `symbol-shoestring-0.0.5/shoestring/healthagents/peer_certificate.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/healthagents/rest_api.py` & `symbol-shoestring-0.0.5/shoestring/healthagents/rest_api.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/healthagents/rest_https_certificate.py` & `symbol-shoestring-0.0.5/shoestring/healthagents/rest_https_certificate.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/healthagents/voting_keys.py` & `symbol-shoestring-0.0.5/shoestring/healthagents/voting_keys.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/healthagents/websockets.py` & `symbol-shoestring-0.0.5/shoestring/healthagents/websockets.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/CertificateFactory.py` & `symbol-shoestring-0.0.5/shoestring/internal/CertificateFactory.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/ConfigurationManager.py` & `symbol-shoestring-0.0.5/shoestring/internal/ConfigurationManager.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/FileDownloader.py` & `symbol-shoestring-0.0.5/shoestring/internal/FileDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/HarvesterConfigurator.py` & `symbol-shoestring-0.0.5/shoestring/internal/HarvesterConfigurator.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/HeightGrouping.py` & `symbol-shoestring-0.0.5/shoestring/internal/HeightGrouping.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/LinkTransactionBuilder.py` & `symbol-shoestring-0.0.5/shoestring/internal/LinkTransactionBuilder.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/MultisigAnalyzer.py` & `symbol-shoestring-0.0.5/shoestring/internal/MultisigAnalyzer.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/NodeDownloader.py` & `symbol-shoestring-0.0.5/shoestring/internal/NodeDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/NodeFeatures.py` & `symbol-shoestring-0.0.5/shoestring/internal/NodeFeatures.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/NodewatchClient.py` & `symbol-shoestring-0.0.5/shoestring/internal/NodewatchClient.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/OpensslExecutor.py` & `symbol-shoestring-0.0.5/shoestring/internal/OpensslExecutor.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/PackageResolver.py` & `symbol-shoestring-0.0.5/shoestring/internal/PackageResolver.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/PeerDownloader.py` & `symbol-shoestring-0.0.5/shoestring/internal/PeerDownloader.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/PemUtils.py` & `symbol-shoestring-0.0.5/shoestring/internal/PemUtils.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/Preparer.py` & `symbol-shoestring-0.0.5/shoestring/internal/Preparer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import os
 import shutil
+import sys
 import tempfile
 from collections import namedtuple
 from pathlib import Path
 
 from symbolchain.symbol.Network import NetworkTimestamp
 
 from .CertificateFactory import CertificateFactory
@@ -31,14 +32,18 @@
 	'timesync',
 	'user'
 ]
 API_EXTENSIONS = ['database', 'extensions-broker', 'logging-broker', 'messaging', 'pt']
 HARVESTER_EXTENSIONS = ['harvesting']
 
 
+def _qualify_resource(resource_name):
+	return Path(sys.modules[__name__].__file__).parent.parent / resource_name
+
+
 class Preparer:
 	"""Prepares a Symbol directory for execution."""
 
 	# pylint: disable=too-many-instance-attributes
 
 	class DirectoryLocator:
 		"""Provides easy access to output locations."""
@@ -291,15 +296,15 @@
 
 	def configure_https(self):
 		"""Configures https proxy."""
 
 		if not self.config.node.api_https:
 			return
 
-		self._copy_file('shoestring/templates/nginx.conf.erb', self.directories.https_proxy)
+		self._copy_file(_qualify_resource('templates/nginx.conf.erb'), self.directories.https_proxy)
 		(self.directories.https_proxy / 'nginx.conf.erb').chmod(0o400)
 
 	def configure_keys(self, current_finalization_epoch=1, grace_period_epochs=1):
 		"""Configures key pairs based on enabled features."""
 
 		if NodeFeatures.HARVESTER in self.config.node.features:
 			self.harvester_configurator.generate_harvester_key_files(self.directories.keys)
@@ -331,18 +336,18 @@
 
 			factory.package(self.directories.certificates)
 
 	def configure_docker(self, template_mapping):
 		"""Prepares docker-compose file."""
 
 		if NodeFeatures.API in self.config.node.features:
-			self._copy_tree_readonly('shoestring/startup', self.directories.startup)
+			self._copy_tree_readonly(_qualify_resource('startup'), self.directories.startup)
 
 		compose_template_filename_postfix = 'dual' if NodeFeatures.API in self.config.node.features else 'peer'
-		compose_template_filename = f'shoestring/templates/docker-compose-{compose_template_filename_postfix}.yaml'
+		compose_template_filename = _qualify_resource(f'templates/docker-compose-{compose_template_filename_postfix}.yaml')
 		compose_output_filepath = self.directory / 'docker-compose.yaml'
 		apply_template(compose_template_filename, template_mapping, compose_output_filepath)
 		compose_output_filepath.chmod(0o400)
 
 	def prepare_linking_transaction(self, account_public_key, existing_links, timestamp):
 		"""Creates an aggregate transaction containing account key link and unlink transactions """
```

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/ShoestringConfiguration.py` & `symbol-shoestring-0.0.5/shoestring/internal/ShoestringConfiguration.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/internal/VoterConfigurator.py` & `symbol-shoestring-0.0.5/shoestring/internal/VoterConfigurator.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/lang/en/LC_MESSAGES/messages.mo` & `symbol-shoestring-0.0.5/shoestring/lang/en/LC_MESSAGES/messages.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-08-01 12:20+0000\n"
+"POT-Creation-Date: 2023-08-01 16:59+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `symbol-shoestring-0.0.4/shoestring/lang/en/LC_MESSAGES/messages.po` & `symbol-shoestring-0.0.5/shoestring/lang/en/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -116,25 +116,25 @@
 #: shoestring/commands/announce_transaction.py:15
 #: shoestring/commands/min_cosignatures_count.py:18
 #: shoestring/commands/renew_voting_keys.py:32 shoestring/commands/setup.py:61
 msgid "general-connecting-to-node"
 msgstr "connecting to {endpoint}"
 
 #: shoestring/commands/init.py:17 shoestring/commands/reset_data.py:57
-#: shoestring/internal/Preparer.py:184
+#: shoestring/internal/Preparer.py:189
 #: shoestring/internal/VoterConfigurator.py:53
 msgid "general-copying-file"
 msgstr "copying FILE {source_path} into {destination_path}"
 
-#: shoestring/commands/reset_data.py:62 shoestring/internal/Preparer.py:190
+#: shoestring/commands/reset_data.py:62 shoestring/internal/Preparer.py:195
 msgid "general-copying-tree"
 msgstr "copying TREE {source_path} to {destination_path}"
 
 #: shoestring/commands/renew_voting_keys.py:46
-#: shoestring/internal/Preparer.py:383
+#: shoestring/internal/Preparer.py:388
 msgid "general-created-aggregate-transaction"
 msgstr "created aggregate transaction with hash {transaction_hash}"
 
 #: shoestring/healthagents/peer_api.py:19
 msgid "health-peer-api-error"
 msgstr "cannot access peer API at {host} on port {port}"
```

### Comparing `symbol-shoestring-0.0.4/shoestring/lang/ja/LC_MESSAGES/messages.po` & `symbol-shoestring-0.0.5/shoestring/lang/ja/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -112,25 +112,25 @@
 #: shoestring/commands/announce_transaction.py:15
 #: shoestring/commands/min_cosignatures_count.py:18
 #: shoestring/commands/renew_voting_keys.py:32 shoestring/commands/setup.py:61
 msgid "general-connecting-to-node"
 msgstr ""
 
 #: shoestring/commands/init.py:17 shoestring/commands/reset_data.py:57
-#: shoestring/internal/Preparer.py:184
+#: shoestring/internal/Preparer.py:189
 #: shoestring/internal/VoterConfigurator.py:53
 msgid "general-copying-file"
 msgstr ""
 
-#: shoestring/commands/reset_data.py:62 shoestring/internal/Preparer.py:190
+#: shoestring/commands/reset_data.py:62 shoestring/internal/Preparer.py:195
 msgid "general-copying-tree"
 msgstr ""
 
 #: shoestring/commands/renew_voting_keys.py:46
-#: shoestring/internal/Preparer.py:383
+#: shoestring/internal/Preparer.py:388
 msgid "general-created-aggregate-transaction"
 msgstr ""
 
 #: shoestring/healthagents/peer_api.py:19
 msgid "health-peer-api-error"
 msgstr ""
```

### Comparing `symbol-shoestring-0.0.4/shoestring/lang/messages.pot` & `symbol-shoestring-0.0.5/shoestring/lang/messages.pot`

 * *Files 0% similar despite different names*

```diff
@@ -105,25 +105,25 @@
 #: shoestring/commands/announce_transaction.py:15
 #: shoestring/commands/min_cosignatures_count.py:18
 #: shoestring/commands/renew_voting_keys.py:32 shoestring/commands/setup.py:61
 msgid "general-connecting-to-node"
 msgstr ""
 
 #: shoestring/commands/init.py:17 shoestring/commands/reset_data.py:57
-#: shoestring/internal/Preparer.py:184
+#: shoestring/internal/Preparer.py:189
 #: shoestring/internal/VoterConfigurator.py:53
 msgid "general-copying-file"
 msgstr ""
 
-#: shoestring/commands/reset_data.py:62 shoestring/internal/Preparer.py:190
+#: shoestring/commands/reset_data.py:62 shoestring/internal/Preparer.py:195
 msgid "general-copying-tree"
 msgstr ""
 
 #: shoestring/commands/renew_voting_keys.py:46
-#: shoestring/internal/Preparer.py:383
+#: shoestring/internal/Preparer.py:388
 msgid "general-created-aggregate-transaction"
 msgstr ""
 
 #: shoestring/healthagents/peer_api.py:19
 msgid "health-peer-api-error"
 msgstr ""
```

### Comparing `symbol-shoestring-0.0.4/shoestring/startup/mongors.sh` & `symbol-shoestring-0.0.5/shoestring/startup/mongors.sh`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/templates/docker-compose-dual.yaml` & `symbol-shoestring-0.0.5/shoestring/templates/docker-compose-dual.yaml`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/templates/docker-compose-peer.yaml` & `symbol-shoestring-0.0.5/shoestring/templates/docker-compose-peer.yaml`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/Screen.py` & `symbol-shoestring-0.0.5/shoestring/wizard/Screen.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/ScreenContainer.py` & `symbol-shoestring-0.0.5/shoestring/wizard/ScreenContainer.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/ShoestringOperation.py` & `symbol-shoestring-0.0.5/shoestring/wizard/ShoestringOperation.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/TabbedView.py` & `symbol-shoestring-0.0.5/shoestring/wizard/TabbedView.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/TitleBar.py` & `symbol-shoestring-0.0.5/shoestring/wizard/TitleBar.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/ValidatingTextBox.py` & `symbol-shoestring-0.0.5/shoestring/wizard/ValidatingTextBox.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/__main__.py` & `symbol-shoestring-0.0.5/shoestring/wizard/__main__.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/buttons.py` & `symbol-shoestring-0.0.5/shoestring/wizard/buttons.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/navigation.py` & `symbol-shoestring-0.0.5/shoestring/wizard/navigation.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/screen_loader.py` & `symbol-shoestring-0.0.5/shoestring/wizard/screen_loader.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/screens/certificates.py` & `symbol-shoestring-0.0.5/shoestring/wizard/screens/certificates.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/screens/end_screen.py` & `symbol-shoestring-0.0.5/shoestring/wizard/screens/end_screen.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/screens/harvesting.py` & `symbol-shoestring-0.0.5/shoestring/wizard/screens/harvesting.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/screens/modal.py` & `symbol-shoestring-0.0.5/shoestring/wizard/screens/modal.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/screens/network_type.py` & `symbol-shoestring-0.0.5/shoestring/wizard/screens/network_type.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/screens/node_settings.py` & `symbol-shoestring-0.0.5/shoestring/wizard/screens/node_settings.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/screens/node_type.py` & `symbol-shoestring-0.0.5/shoestring/wizard/screens/node_type.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/screens/obligatory.py` & `symbol-shoestring-0.0.5/shoestring/wizard/screens/obligatory.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/screens/root_check.py` & `symbol-shoestring-0.0.5/shoestring/wizard/screens/root_check.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/screens/voting.py` & `symbol-shoestring-0.0.5/shoestring/wizard/screens/voting.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/screens/welcome.py` & `symbol-shoestring-0.0.5/shoestring/wizard/screens/welcome.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/setup_file_generator.py` & `symbol-shoestring-0.0.5/shoestring/wizard/setup_file_generator.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/shoestring_dispatcher.py` & `symbol-shoestring-0.0.5/shoestring/wizard/shoestring_dispatcher.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/shoestring/wizard/styles.py` & `symbol-shoestring-0.0.5/shoestring/wizard/styles.py`

 * *Files identical despite different names*

### Comparing `symbol-shoestring-0.0.4/setup.py` & `symbol-shoestring-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
  'symbol-lightapi==0.0.4',
  'symbol-sdk-python==3.0.11',
  'websockets==11.0.3',
  'zenlog==1.1']
 
 setup_kwargs = {
     'name': 'symbol-shoestring',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Symbol Shoestring Deployment Tool',
     'long_description': '# shoestring\n\n# CLI Commands\n\n## Setup Commands\n\n### init\n\nExtracts a template shoestring configuration file from a package that the user can then customize.\n\n```\ninit [--package PACKAGE] config\n\n  config             path to shoestring configuration file\n  --package PACKAGE  Network configuration package. Possible values: (name | file:///filename | http(s)://uri) (default: mainnet)\n```\n\n### min-cosignatures-count\n\nAutomatically detects the minimum cosignatures required for an account and optionally updates the shoestring configuration file.\n\n```\nmin-cosignatures-count --config CONFIG --ca-key-path CA_KEY_PATH [--update]\n\n  --config CONFIG           path to shoestring configuration file\n  --ca-key-path CA_KEY_PATH path to main private key PEM file\n  --update                  update the shoestring configuration file\n```\n\n### import-bootstrap\n\nImports settings from a symbol-bootstap installation.\n\n\n```\nimport-bootstrap --config CONFIG --bootstrap BOOTSTRAP\n\n  --config CONFIG       path to shoestring configuration file\n  --bootstrap BOOTSTRAP path to bootstrap target directory\n```\n\n### pemtool\n\nGenerates a main private key PEM file that can be used by shoestring.\n\n```\npemtool --output OUTPUT [--input INPUT] [--ask-pass] [--force]\n\n  --output OUTPUT  output PEM key file\n  --input INPUT    input private key file (optional)\n  --ask-pass       encrypt PEM with a password (password prompt will be shown)\n  --force          overwrite output file if it already exists\n```\n\n### setup\n\nSets up a Symbol node from scratch\n\n```\nsetup \\\n    --config CONFIG \\\n    [--package PACKAGE] \\\n    [--directory DIRECTORY] \\\n    [--overrides OVERRIDES] \\\n    [--metadata METADATA] \\\n    [--security {default,paranoid,insecure}] \\\n    --ca-key-path CA_KEY_PATH\n\n  --config CONFIG           path to shoestring configuration file\n  --package PACKAGE         Network configuration package. Possible values: (name | file:///filename | http(s)://uri) (default: mainnet)\n  --directory DIRECTORY     installation directory (default: $HOME)\n  --overrides OVERRIDES     path to custom user settings\n  --metadata METADATA       custom node metadata (this is only valid for API roles)\n  --security                security mode (default: default)\n  --ca-key-path CA_KEY_PATH path to main private key PEM file\n```\n\nPlease note that only security mode "default" is supported at this time.\n\nThis command will generate a transaction that will need to be sent to the network using `announce-transaction` to update the network state.\n\n## Operational Commands\n\n### signer\n\nSigns a transaction that can then be announced to the network\n\n```\nsigner --config CONFIG --ca-key-path CA_KEY_PATH [--save] filename\n\n  filename                  transaction binary payload\n  --config CONFIG           path to shoestring configuration file\n  --ca-key-path CA_KEY_PATH path to main private key PEM file\n  --save                    save signed payload into same file as input\n```\n\n### announce-transaction\n\nAnnounces a transaction to the network.\n\n```\nannounce-transaction --config CONFIG --transaction TRANSACTION\n\n  --config CONFIG           path to shoestring configuration file\n  --transaction TRANSACTION file containing serialized transaction to send\n```\n\n### health\n\nChecks the health of the local Symbol node.\n\n\n```\nhealth [-h] --config CONFIG [--directory DIRECTORY]\n\n  --config CONFIG       path to shoestring configuration file\n  --directory DIRECTORY installation directory (default: $HOME)\n```\n\n## Upgrade Commands\n\n### upgrade\n\nUpgrades a node to the latest client version.\n\n```\nupgrade \\\n    --config CONFIG \\\n    [--package PACKAGE] \\\n    [--directory DIRECTORY] \\\n    [--overrides OVERRIDES] \\\n    [--metadata METADATA]\n\n  --config CONFIG           path to shoestring configuration file\n  --package PACKAGE         Network configuration package. Possible values: (name | file:///filename | http(s)://uri) (default: mainnet)\n  --directory DIRECTORY     installation directory (default: $HOME)\n  --overrides OVERRIDES     path to custom user settings\n  --metadata METADATA       custom node metadata (this is only valid for API roles)\n```\n\n### renew-certificates\n\nRenews peer certificates.\n\n```\nrenew-certificates --config CONFIG [--directory DIRECTORY] --ca-key-path CA_KEY_PATH [--renew-ca]\n\n  --config CONFIG           path to shoestring configuration file\n  --directory DIRECTORY     installation directory (default: $HOME)\n  --ca-key-path CA_KEY_PATH path to main private key PEM file\n  --renew-ca                renews CA certificate too\n```\n\nWhen `--renew-ca` is set, both CA and node certificates will be regenerated. Otherwise, only node certificate will be.\n\n### renew-voting-keys\n\nRenews voting keys.\n\n```\nrenew-voting-keys --config CONFIG [--directory DIRECTORY]\n\n  --config CONFIG           path to shoestring configuration file\n  --directory DIRECTORY     installation directory (default: $HOME)\n```\n\nThis command will generate a transaction that will need to be sent to the network using `announce-transaction` to update the network state.\n\n### reset-data\n\nResets blockchain state to allow a resync from scratch.\n\n```\nreset-data --config CONFIG [--directory DIRECTORY] [--purge-harvesters]\n\n  --config CONFIG           path to shoestring configuration file\n  --directory DIRECTORY     installation directory (default: $HOME)\n  --purge-harvesters        purge harvesters.dat file\n```\n\nWhen `--purge-harvesters` is set, delegates discovered using old keys will be discarded.\n\n\n## Files\n\n### Shoestring Configuration INI\n\nINI file used by shoestring to customize a Symbol node deployment.\nIt is composed of five sections: `network`, `images`, `services`, `transaction`, `imports`, `node`.\n\n#### network\n\nDescribes properties of network that deployed node should connect with.\nThese should match values in `config-network.properties` Symbol configuration file.\nIf `init` command is used, these values shouldn\'t be modified\n\n```\nname                  Network name\nidentifier            Network numeric identifier\nepochAdjustment       Network epoch adjustment\ngenerationHashSeed    Network generation hash seed\n```\n\n#### images\n\nDescribes Symbol docker images to use.\nIf `init` command is used, these values shouldn\'t be modified\n```\nclient  Catapult client docker image\nrest    REST docker image\n```\n\n#### services\n\nDescribes network services to use during deployment.\nIf `init` command is used, these values shouldn\'t be modified\n\n```\nnodewatch  URL to nodewatch service.\n```\n\n#### transactions\n\nDescribes properties of generated transactions.\nIf `init` command is used, most of these values _generally_ shouldn\'t be modified.\n`min-cosignatures-count` command can be used to automatically update `minCosignaturesCount` setting.\n\nGeneral properties:\n```\nfeeMultiplier             Min fee multiplier of generated transactions\ntimeoutHours              Timeout of generated transactions (in hours)\nminCosignaturesCount      Minimum number of cosignatures generated transactions will require\n```\n\nWhen `signer` command is signing an aggregate bonded transaction, it will additionally generate a hash lock transaction\nusing the following properties:\n```\nhashLockDuration          Hash lock duration in blocks\ncurrencyMosaicId          Network currency mosaid id\nlockedFundsPerAggregate   Locked funds per aggregate\n```\n\n#### imports\n\nDescribes keys to import.\nThese need to be manually set if there are harvesting and/or voting keys that need to be imported.\n\n```\nharvester Path to a config-harvesting.properties Symbol configuration file containing harvesting keys to import\nvoter     Path to a directory containing private_key_tree*.day files to import\n```\n\n#### node\n\nDescribes settings to customize a node.\n\n`features` supports the following:\n* `PEER` - Peer support\n* `API` - REST support\n* `HARVESTER` - Node will be configured to harvest and accept delegated harvesters\n* `VOTER` - Node will be configured to vote\n\n`caPassword` supports all available openssl passphrase options: https://www.openssl.org/docs/man3.0/man1/openssl-passphrase-options.html.\n\n```\nfeatures       One or more node features to deploy (| delimited)\nuserId         User id of node used to set process and file permissons\ngroupId        Group id of node used to set process and file permissons\ncaPassword     Password of CA (main) PEM private key file (if applicable)\napiHttps       Set to enable HTTPS REST (only applicable when features include API)\n\ncaCommonName   Common name of generated CA certificates\nnodeCommonName Common name of generated Node certificates\n```\n\n### Overrides\n\nINI file that is used to customize advanced Symbol settings.\n\nSections should have the format `[<config-short-name>.<config-section>]`.\nSection contents will then be applied to the appropriate Symbol configuration file.\n\nFor example, in order to set two custom settings:\n1. `connectTimeout` - located in the `config-node.properties` file in section `node`\n1. `maxUnlockedAccounts` - located in the `config-harvesting.properties` file in section `harvesting`\n\nThe following snippet will suffice:\n\n```ini\n[node.node]\n\nconnectTimeout = 5s\n\n[harvesting.harvesting]\n\nmaxUnlockedAccounts = 2\n```\n\nNotice that these custom settings are applied *BEFORE* shoestring updates the Symbol configuration files.\nIn cases of conflicts, the shoestring changes will take precedence.\n\n### Node Metadata\n\nJSON file that is ingested and used to replace the contents of `nodeMetadata` in rest.json.\nThis data is then accessible via the `node/metadata` REST endpoint.\nThis file is optional and only used for deployments including API role.\n\n## Prerequisites:\n\n    apt-get install python3 python3-pip openssl\n    python3 -m pip install -r requirements.txt\n\n## Temporarily (until lightapi package fix):\n\n```\ncd product/lightapi/python\n./scripts/ci/setup_lint.sh\n./scripts/ci/lint.sh\n./scripts/ci/test.sh\n\n# to run shoestring\n\nPYTHONPATH=}full path here{/product/lightapi/python python3 -m shoestring\n```\n',
     'author': 'Symbol Contributors',
     'author_email': 'contributors@symbol.dev',
     'maintainer': 'Symbol Contributors',
     'maintainer_email': 'contributors@symbol.dev',
     'url': 'https://github.com/symbol/product/tree/main/tools/shoestring',
```

### Comparing `symbol-shoestring-0.0.4/PKG-INFO` & `symbol-shoestring-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbol-shoestring
-Version: 0.0.4
+Version: 0.0.5
 Summary: Symbol Shoestring Deployment Tool
 Home-page: https://github.com/symbol/product/tree/main/tools/shoestring
 License: MIT
 Keywords: symbol,shoestring,deployment,node
 Author: Symbol Contributors
 Author-email: contributors@symbol.dev
 Maintainer: Symbol Contributors
```

